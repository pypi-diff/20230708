# Comparing `tmp/Subsearch-2.36.0rc3.tar.gz` & `tmp/Subsearch-2.36.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.36.0rc3.tar", last modified: Fri Jun  2 16:06:15 2023, max compression
+gzip compressed data, was "Subsearch-2.36.1.tar", last modified: Sat Jul  8 17:59:54 2023, max compression
```

## Comparing `Subsearch-2.36.0rc3.tar` & `Subsearch-2.36.1.tar`

### file list

```diff
@@ -1,113 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.117186 Subsearch-2.36.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-02 16:06:15.117186 Subsearch-2.36.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:06:15.117186 Subsearch-2.36.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.105185 Subsearch-2.36.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.105185 Subsearch-2.36.0rc3/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:06:14.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 16:06:15.000000 Subsearch-2.36.0rc3/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.109186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.113186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.113186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.113186 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.113186 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.113186 Subsearch-2.36.0rc3/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:06:15.117186 Subsearch-2.36.0rc3/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/app_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-02 16:05:56.000000 Subsearch-2.36.0rc3/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.064437 Subsearch-2.36.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 17:59:36.000000 Subsearch-2.36.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-08 17:59:36.000000 Subsearch-2.36.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 17:59:54.064437 Subsearch-2.36.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-08 17:59:36.000000 Subsearch-2.36.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-08 17:59:36.000000 Subsearch-2.36.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:59:54.064437 Subsearch-2.36.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-08 17:59:36.000000 Subsearch-2.36.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.052436 Subsearch-2.36.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:59:53.000000 Subsearch-2.36.1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/app_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/spritesheet_data.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/gui_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/settings_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.064437 Subsearch-2.36.1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/app_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.36.0rc3/LICENSE` & `Subsearch-2.36.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/PKG-INFO` & `Subsearch-2.36.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.0rc3
+Version: 2.36.1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.36.0rc3/README.md` & `Subsearch-2.36.1/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/pyproject.toml` & `Subsearch-2.36.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.14", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0"]
+dependencies = ["selectolax==0.3.14", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0", "pillow==9.5.0"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -40,16 +40,16 @@
 include = ["subsearch*"]
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
-optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.0", "mypy==1.3.0", "pipreqs==0.4.13"]
-dev = ["pytest==7.3.1", "pytest-cov==4.1.0", "tox==4.5.2"]
+optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.2", "mypy==1.4.1", "pipreqs==0.4.13"]
+dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "tox==4.6.4"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
```

### Comparing `Subsearch-2.36.0rc3/setup.py` & `Subsearch-2.36.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     from cx_Freeze import Executable, setup
 
     from subsearch.data import __guid__
 
     sys.path.insert(0, os.path.abspath(os.path.dirname(__file__)))
 
-    icon = "src/subsearch/gui/assets/icon/subsearch.ico"
+    icon = "src/subsearch/gui/assets/subsearch.ico"
     app_name = "Subsearch"
     registry_path = rf"Software\Classes\*\shell\Subsearch"
     script_component = "_cx_executable0__Executable_script_src_subsearch___main__.py_"
     subsearch_key = (f"{app_name}_key", -1, registry_path, None, None, script_component)
     subsearch_icon = (f"{app_name}_regz_icon", -1, registry_path, "Icon", None, script_component)
     subsearch_appliesto = (f"{app_name}_regz_appliesto", -1, registry_path, "AppliesTo", None, script_component)
     subsearch_command = (f"{app_name}_key_command", -1, rf"{registry_path}\command", None, "", script_component)
```

### Comparing `Subsearch-2.36.0rc3/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.36.1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.0rc3
+Version: 2.36.1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/__init__.py` & `Subsearch-2.36.1/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/core.py` & `Subsearch-2.36.1/src/subsearch/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,45 @@
 from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.gui import tab_manager
 from subsearch.providers import opensubtitles, subscene, yifysubtitles
 from subsearch.utils import (
     app_integrity,
     file_manager,
     io_json,
-    io_winreg,
     log,
+    state_machine,
     string_parser,
 )
 
 
-class Initializer:
+class Initializer(state_machine.CoreState):
     def __init__(self) -> None:
+        state_machine.CoreState.__create__(self.unknown)
+        self.set_state(self.initializing)
         app_integrity.initialize_application()
         self.app_config = io_json.get_app_config()
         if video_data is not None:
             file_manager.create_directory(video_data.subs_directory)
-            self.file_exist = True
             self.file_hash = file_manager.get_hash(video_data.file_path)
         else:
-            self.file_exist = False
+            self.set_state(self.no_file_found)
             self.file_hash = ""
         self.results: dict[str, list[DownloadData]] = {}
         self.skipped_downloads: dict[str, list[PrettifiedDownloadData]] = {}
         self.skipped_combined: list[PrettifiedDownloadData] = []
         self.downloads: dict[str, int] = {}
         self.language_data = io_json.get_language_data()
 
         for provider in self.app_config.providers.keys():
             self.results[provider] = []
             self.skipped_downloads[provider] = []
             self.downloads[provider] = 0
 
         self.ran_download_tab = False
+        self.foreign_only = io_json.get_json_key("foreign_only")
         self.skip_step = SkipStep(self)
         if self.file_exist:
             self.release_data = string_parser.get_release_metadata(video_data.filename, self.file_hash)
             create_provider_urls = string_parser.CreateProviderUrls(
                 self.file_hash, self.app_config, self.release_data, self.language_data
             )
             self.provider_urls = create_provider_urls.retrieve_urls()
@@ -49,14 +51,15 @@
                 release_data=self.release_data,
                 app_config=self.app_config,
                 provider_urls=self.provider_urls,
                 language_data=self.language_data,
             )
             log.set_logger_data(**self.search_kwargs)
             log.output_parameters()
+            self.set_state(self.initialized)
 
     def all_providers_disabled(self) -> bool:
         self.app_config = io_json.get_app_config()
         if (
             self.app_config.providers["subscene_site"] is False
             and self.app_config.providers["opensubtitles_site"] is False
             and self.app_config.providers["opensubtitles_hash"] is False
@@ -72,57 +75,55 @@
 
 
 class AppSteps(Initializer):
     def __init__(self) -> None:
         self.start = time.perf_counter()
         Initializer.__init__(self)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {__version__}")
-        if io_winreg.registry_key_exists() is False and io_json.get_json_key("context_menu"):
-            io_json.create_application_config_json()
-            io_winreg.add_context_menu()
-        if io_winreg.registry_key_exists() and io_winreg.key_no_value() and io_json.get_json_key("context_menu"):
-            io_winreg.add_context_menu()
-        if self.file_exist is False:
+        if not self.file_exist:
             tab_manager.open_tab("search")
             return None
-        self.foreign_only = io_json.get_json_key("foreign_only")
 
         if " " in video_data.filename:
             log.warning_spaces_in_filename()
         log.output_header("Search started")
 
     def _provider_opensubtitles(self) -> None:
         if self.skip_step.opensubtitles():
             return None
+        self.set_state(self.scraping_opensubtitles)
         # log.output_header("Searching on opensubtitles")
         _opensubs = opensubtitles.OpenSubtitles(**self.search_kwargs)
         if self.app_config.providers["opensubtitles_hash"] and self.file_hash != "":
             self.results["opensubtitles_hash"] = _opensubs.parse_hash_results()
         if self.app_config.providers["opensubtitles_site"]:
             self.results["opensubtitles_site"] = _opensubs.parse_site_results()
         self.skipped_downloads["opensubtitles_site"] = _opensubs._sorted_list()
 
     def _provider_subscene(self) -> None:
         if self.skip_step.subscene():
             return None
+        self.set_state(self.scraping_subscene)
         _subscene = subscene.Subscene(**self.search_kwargs)
         self.results["subscene_site"] = _subscene.parse_site_results()
         self.skipped_downloads["subscene_site"] = _subscene._sorted_list()
 
     def _provider_yifysubtitles(self) -> None:
         if self.skip_step.yifysubtitles():
             return None
+        self.set_state(self.scraping_yifysubtitles)
         _yifysubs = yifysubtitles.YifiSubtitles(**self.search_kwargs)
         self.results["yifysubtitles_site"] = _yifysubs.parse_site_results()
         self.skipped_downloads["yifysubtitles_site"] = _yifysubs._sorted_list()
 
     def _download_files(self) -> None:
         if self.skip_step.download_files():
             return None
         log.output_header(f"Downloading subtitles")
+        self.set_state(self.downloading_files)
         for provider, data in self.results.items():
             if self.app_config.providers[provider] is False:
                 continue
             if not data:
                 continue
             self.downloads[provider] = self.download_results(data)
         log.output_done_with_tasks(end_new_line=True)
@@ -133,116 +134,116 @@
         for data_list in self.skipped_downloads.values():
             if not data_list:
                 continue
             for data in data_list:
                 self.skipped_combined.append(data)
 
         if self.skipped_combined:
-            tab_manager.open_tab("download", formatted_data=self.skipped_combined)
+            tab_manager.open_tab("download", data=self.skipped_combined)
             self.ran_download_tab = True
         log.output_done_with_tasks(end_new_line=True)
 
     def _extract_zip_files(self) -> None:
         if self.skip_step.extract_zip():
             return None
+        self.set_state(self.extracting_files)
         log.output_header("Extracting downloads")
         file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
         log.output_done_with_tasks(end_new_line=True)
 
     def _clean_up(self) -> None:
-        if self.file_exist is False:
+        if not self.file_exist:
             return None
+        self.set_state(self.cleaning_up)
         if self.app_config.rename_best_match:
             log.output_header("Renaming best match")
             file_manager.rename_best_match(f"{self.release_data.release}.srt", video_data.directory_path, ".srt")
             log.output_done_with_tasks(end_new_line=True)
 
         log.output_header("Cleaning up")
         file_manager.clean_up_files(video_data.subs_directory, "nfo")
         file_manager.delete_temp_files(app_paths.tmpdir)
         if file_manager.directory_is_empty(video_data.subs_directory):
             file_manager.del_directory(video_data.subs_directory)
         log.output_done_with_tasks(end_new_line=True)
 
     def _pre_exit(self) -> None:
         elapsed = time.perf_counter() - self.start
+        self.set_state(self.exiting)
         log.output(f"Finished in {elapsed} seconds")
 
         if self.app_config.show_terminal is False:
             return None
         if file_manager.running_from_exe():
             return None
 
         try:
             input("Ctrl + c or Enter to exit")
         except KeyboardInterrupt:
             pass
 
 
 class SkipStep:
-    def __init__(self, cls):
+    def __init__(self, cls: AppSteps | Initializer):
         self.cls = cls
 
     def opensubtitles(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
         if self.cls.foreign_only:
             return True
-        if io_json.check_language_compatibility("opensubtitles") is False:
+        if not io_json.check_language_compatibility("opensubtitles"):
             return True
-        if (
-            self.cls.app_config.providers["opensubtitles_hash"] is False
-            and self.cls.app_config.providers["opensubtitles_site"] is False
-        ):
+        if not (self.cls.app_config.providers["opensubtitles_hash"] and self.cls.app_config.providers["opensubtitles_site"]):
             return True
         return False
 
     def subscene(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
-        if io_json.check_language_compatibility("subscene") is False:
+        if not io_json.check_language_compatibility("subscene"):
             return True
-        if self.cls.app_config.providers["subscene_site"] is False:
+        if not self.cls.app_config.providers["subscene_site"]:
             return True
         return False
 
     def yifysubtitles(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
         if self.cls.foreign_only:
             return True
-        if io_json.check_language_compatibility("yifysubtitles") is False:
+        if not io_json.check_language_compatibility("yifysubtitles"):
             return True
         if self.cls.release_data.tvseries:
             return True
-        if self.cls.provider_urls.yifysubtitles == "N/A":
+        if self.cls.provider_urls.yifysubtitles == "":
             return True
-        if self.cls.app_config.providers["yifysubtitles_site"] is False:
+        if not self.cls.app_config.providers["yifysubtitles_site"]:
             return True
         return False
 
     def download_files(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
         if not any(self.cls.results.values()):
             return True
         return False
 
     def not_downloaded(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
         number_of_downloads = sum(v for v in self.cls.downloads.values())
         if self.cls.app_config.manual_download_fail and number_of_downloads > 0:
             return True
 
         if self.cls.app_config.manual_download_mode and number_of_downloads < 1:
             return False
         return False
 
     def extract_zip(self) -> bool:
-        if self.cls.file_exist is False:
+        if not self.cls.file_exist:
             return True
         if self.cls.ran_download_tab:
             return True
         if self.cls.all_providers_disabled():
             return True
         return False
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/data/data_initializer.py` & `Subsearch-2.36.1/src/subsearch/data/data_initializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         AppPaths: An instance of AppPaths representing the path configuration for Subsearch application.
     """
     home = Path(__file__).resolve().parent.parent
     return AppPaths(
         home=home,
         data=Path(home) / "data",
         gui=Path(home) / "gui",
+        gui_assets=Path(home) / "gui" / "assets",
+        gui_app_theme=Path(home) / "gui" / "app_theme",
         providers=Path(home) / "providers",
         utils=Path(home) / "utils",
-        icon=Path(home) / "gui" / "assets" / "icon" / "subsearch.ico",
-        tabs=Path(home) / "gui" / "assets" / "tabs",
         tmpdir=Path(tempfile.gettempdir()) / f"tmp_subsearch",
         appdata_local=Path.home() / "AppData" / "Local" / "Subsearch",
     )
 
 
 @no_type_check
 def video_file() -> FileData:
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/data/data_objects.py` & `Subsearch-2.36.1/src/subsearch/data/data_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     name: str
     alpha_1: str
     alpha_2b: str
     incompatibility: list[str]
     subscene_id: int
 
 
-@dataclass(order=True)
+@dataclass(order=True, slots=True)
 class ProviderAlphaCodeData:
     provider: str
     alpha_code: str
 
 
-@dataclass(order=True)
+@dataclass(order=True, slots=True)
 class AppPaths:
     """
     A dataclass representing the paths used in the application.
 
     Attributes:
         home (Path): The root directory of the application.
         data (Path): The directory where data related to the application is stored.
@@ -33,23 +33,23 @@
         tmpdir(Path): The directory containing temporary files & folders.
         appdata_local(Path): The directory containing the persistent application files.
     """
 
     home: Path
     data: Path
     gui: Path
+    gui_assets: Path
+    gui_app_theme: Path
     providers: Path
     utils: Path
-    icon: Path
-    tabs: Path
     tmpdir: Path
     appdata_local: Path
 
 
-@dataclass(order=True)
+@dataclass(order=True, slots=True)
 class FileData:
     """
      Class representing file information.
 
     Attributes:
         filename (str): Name of the file.
         file_extension (str): Extension of the file.
@@ -63,15 +63,15 @@
     file_extension: str
     file_path: Path
     directory_path: Path
     subs_directory: Path
     tmp_directory: Path
 
 
-@dataclass(order=True)
+@dataclass(order=True, slots=True)
 class AppConfig:
     """
     Data class for storing user preferences and settings.
 
     Attributes:
         current_language (str): The currently selected language.
         subtitle_type (dict[str, bool]): A dictionary used to store user's preference regarding subtitle types.
@@ -105,24 +105,24 @@
     log_to_file: bool
     file_extensions: dict[str, bool]
     providers: dict[str, bool]
     hearing_impaired: bool
     non_hearing_impaired: bool
 
 
-@dataclass(order=True)
+@dataclass(order=True, slots=True)
 class SubsceneCookie:
     dark_theme: bool
     sort_subtitle_by_date: str
     language_filter: int
-    hearing_impaired: bool
+    hearing_impaired: int
     foreigen_only: bool
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True, slots=True)
 class ReleaseData:
     """
     Data class representing data associated with a media release.
 
     Attributes:
         title (str): Title of the media.
         year (int): Year of the media release.
@@ -144,15 +144,15 @@
     episode_ordinal: str
     tvseries: bool
     release: str
     group: str
     file_hash: str
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True, slots=True)
 class ProviderUrls:
     """
     A dataclass to represent URLs for different subtitle providers.
 
     Attributes:
         subscene(str): URL of the subscene provider.
         opensubtitles(str): URL of the opensubtitles provider.
@@ -162,15 +162,15 @@
 
     subscene: str
     opensubtitles: str
     opensubtitles_hash: str
     yifysubtitles: str
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True, slots=True)
 class DownloadData:
     """
     A data class representing metadata for the to be downloaded subtitle file.
 
     Attributes:
         provider (str): The subtitle provider used to obtain the subtitle file.
         name (str): The name of the media file associated with the subtitle file.
@@ -184,15 +184,15 @@
     name: str
     file_path: str
     url: str
     idx_num: int
     idx_lenght: int
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True, slots=True)
 class PrettifiedDownloadData:
     """
     Represents prettified version of DownloadData.
 
     Attributes:
         provider (str): The name of the metadata provider.
         release (str): The name of the movie or TV show release.
@@ -207,36 +207,36 @@
     release: str
     url: str
     pct_result: int
     formatted_release: str
     formatted_url: str
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True)
 class GUISizes:
     """
     Sub dataclass containing sizes for the GUI
     """
 
     root_width: int = 738
     root_height: int = 720
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True)
 class GUIPositions:
     """
     Sub dataclass containing sizes for the GUI
     """
 
     content_x: int = int(GUISizes().root_width / 2)
     content_y: int = int(GUISizes().root_height / 2 - 41)
     content_hidden_x: int = int(GUISizes().root_width * 2)
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True)
 class GUIColors:
     """
     Sub dataclass containing colors for the GUI
 
     Colors:
         purple: #b294bb
         red: #bc473b
@@ -279,15 +279,15 @@
     dark_grey: str = "#1a1b1b"
     mid_grey_black: str = "#111111"
     light_black: str = "#0e0e0e"
     black: str = "#151515"
     dark_black: str = "#000000"
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True)
 class GUIFonts:
     """
     Sub dataclass containing fonts and their styles and or size
 
     Fonts:
         cas6b: Cascadia 6 bold
         cas8: Cascadia 8
@@ -303,27 +303,27 @@
     cas8i: str = "Cascadia 8 italic"
     cas8b: str = "Cascadia 8 bold"
     cas10b: str = "Cascadia 10 bold"
     cas11: str = "Cascadia 11"
     cas20b: str = "Cascadia 20 bold"
 
 
-@dataclass(frozen=True, order=True)
+@dataclass(order=True, frozen=True)
 class GUIData:
     """
     Dataclass containing GUI data
     """
 
     size = GUISizes
     pos = GUIPositions
     fonts = GUIFonts
     colors = GUIColors
 
 
-GUI_DATA = GUIData()
+gui = GUIData()
 
 SUPPORTED_FILE_EXTENSIONS = [
     ".avi",
     ".mp4",
     ".mkv",
     ".mpg",
     ".mpeg",
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/data/languages.json` & `Subsearch-2.36.1/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# Made by rdbende @ https://github.com/rdbende/Sun-Valley-ttk-theme
-# Modified and new assets by vagabondHustler
-
-package require Tk 8.6
-
-namespace eval ttk::theme::ttk_styls {
-    variable version 1.0
-    package provide ttk::theme::ttk_style $version
-
-    ttk::style theme create ttk_style -parent clam -settings {
-        proc load_images {imgdir} {
-            variable images
-            foreach file [glob -directory $imgdir *.png] {
-                set images([file tail [file rootname $file]]) \
-                [image create photo -file $file -format png]
-            }
-        }
-        load_images [file join [file dirname [info script]] btn]
-        load_images [file join [file dirname [info script]] scrollbar]
-        load_images [file join [file dirname [info script]] scale]
-        load_images [file join [file dirname [info script]] checkbox]
-
-        array set colors {
-            -fg             "#bdbdbd"
-            -bg             "#1a1b1b"
-            -disabledfg     "#595959"
-            -selectfg       "#ffffff"
-            -selectbg       "#2f60d8"
-        }
-
-         ttk::style layout TButton {
-            Button.button -children {
-                Button.padding -children {
-                    Button.label -side left -expand 1
-                } 
-            }
-        }
-
-        ttk::style layout Vertical.TScrollbar {
-            Vertical.Scrollbar.trough -sticky ns -children {
-                Vertical.Scrollbar.uparrow -side top
-                Vertical.Scrollbar.downarrow -side bottom
-                Vertical.Scrollbar.thumb -expand 1
-            }
-        }
-
-        ttk::style layout Horizontal.TScrollbar {
-            Horizontal.Scrollbar.trough -sticky ew -children {
-                Horizontal.Scrollbar.leftarrow -side left
-                Horizontal.Scrollbar.rightarrow -side right
-                Horizontal.Scrollbar.thumb -expand 1
-            }
-        }
-
-        ttk::style layout TCheckbutton {
-            Checkbutton.button -children {
-                Checkbutton.padding -children {
-                    Checkbutton.indicator -side left
-                    Checkbutton.label -side right -expand 1
-                }
-            }
-        }
-
-        # Button
-        ttk::style configure TButton -padding {4 4} -anchor center -foreground $colors(-fg)
-
-        ttk::style map TButton -foreground \
-            [list disabled #bdbdbd \
-                pressed #4c4c4c]
-
-        ttk::style element create Button.button image \
-            [list $images(btn_rest) \
-                {selected disabled} $images(btn_disabled) \
-                disabled $images(btn_disabled) \
-                selected $images(btn_rest) \
-                pressed $images(btn_pressed) \
-                active $images(btn_hover) \
-            ] -border 4 -sticky nsew
-
-        # Scrollbar
-        ttk::style element create Horizontal.Scrollbar.trough image $images(scroll_hor_trough) -sticky ew -border 6
-        ttk::style element create Horizontal.Scrollbar.thumb image $images(scroll_hor_thumb) -sticky ew -border 3
-
-        ttk::style element create Horizontal.Scrollbar.rightarrow image $images(scroll_right) -sticky {} -width 12
-        ttk::style element create Horizontal.Scrollbar.leftarrow image $images(scroll_left) -sticky {} -width 12
-
-        ttk::style element create Vertical.Scrollbar.trough image $images(scroll_vert_trough) -sticky ns -border 6
-        ttk::style element create Vertical.Scrollbar.thumb image $images(scroll_vert_thumb) -sticky ns -border 3
-
-        ttk::style element create Vertical.Scrollbar.uparrow image $images(scroll_up) -sticky {} -height 12
-        ttk::style element create Vertical.Scrollbar.downarrow image $images(scroll_down) -sticky {} -height 12
-
-        # Scale
-        ttk::style element create Horizontal.Scale.trough image $images(scale_trough_hor) \
-            -border 5 -padding 0
-
-        ttk::style element create Vertical.Scale.trough image $images(scale_trough_vert) \
-            -border 5 -padding 0
-
-        ttk::style element create Scale.slider \
-            image [list $images(scale_thumb_rest) \
-                disabled $images(scale_thumb_disabled) \
-                pressed $images(scale_thumb_pressed) \
-                active $images(scale_thumb_hover) \
-            ] -sticky {}
-        
-        # Checkbutton
-        ttk::style configure TCheckbutton -width 16 -padding {1 1} -border 0 -foreground $colors(-fg) -background $colors(-bg)
-
-        ttk::style element create Checkbutton.indicator image \
-            [list $images(check_unsel_rest) \
-                {alternate disabled} $images(check_tri_disabled) \
-                {selected disabled} $images(check_disabled) \
-                disabled $images(check_unsel_disabled) \
-                {pressed alternate} $images(check_tri_hover) \
-                {active alternate} $images(check_tri_hover) \
-                alternate $images(check_tri_rest) \
-                {pressed selected} $images(check_hover) \
-                {active selected} $images(check_hover) \
-                selected $images(check_rest) \
-                {pressed !selected} $images(check_unsel_pressed) \
-                active $images(check_unsel_hover) \
-            ] -width 26 -sticky w
-
-       
-    }
-}
+source [file join [file dirname [info script]] spritesheet_data.tcl]
+
+namespace eval ttk_subsearch_theme {
+    package provide ttk::theme::ttk_subsearch_theme 0.1.0
+
+    # Load Images
+    proc load_images {imgfile} {
+        variable sprites
+        image create photo spritesheet -file $imgfile -format png
+        foreach {name x y width height} $::sprite_data {
+            set sprites($name) [image create photo -width $width -height $height]
+            $sprites($name) copy spritesheet -from $x $y [expr {$x + $width}] [expr {$y + $height}]
+        }
+    }
+
+    load_images [file join [file dirname [file dirname [info script]]] assets spritesheet.png]
+
+
+    # Theme Creation
+    ttk::style theme create ttk_subsearch_theme -parent clam -settings {
+
+        # Color Settings
+        array set colors {
+            -fg             "#bdbdbd"
+            -bg             "#1a1b1b"
+            -disabledfg     "#595959"
+            -selectfg       "#ffffff"
+            -selectbg       "#2f60d8"
+        }
+
+        # Button Layout
+        ttk::style layout TButton {
+            Button.button -children {
+                Button.padding -children {
+                    Button.label -side left -expand 1
+                }
+            }
+        }
+
+        # Vertical Scrollbar Layout
+        ttk::style layout Vertical.TScrollbar {
+            Vertical.Scrollbar.trough -sticky ns -children {
+                Vertical.Scrollbar.uparrow -side top
+                Vertical.Scrollbar.downarrow -side bottom
+                Vertical.Scrollbar.thumb -expand 1
+            }
+        }
+
+        # Horizontal Scrollbar Layout
+        ttk::style layout Horizontal.TScrollbar {
+            Horizontal.Scrollbar.trough -sticky ew -children {
+                Horizontal.Scrollbar.leftarrow -side left
+                Horizontal.Scrollbar.rightarrow -side right
+                Horizontal.Scrollbar.thumb -expand 1
+            }
+        }
+
+        # Checkbutton Layout
+        ttk::style layout TCheckbutton {
+            Checkbutton.button -children {
+                Checkbutton.padding -children {
+                    Checkbutton.indicator -side left
+                    Checkbutton.label -side right -expand 1
+                }
+            }
+        }
+
+        # Button Configuration
+        ttk::style configure TButton -padding {4 4} -anchor center -foreground $colors(-fg)
+
+        ttk::style map TButton -foreground \
+            [list disabled #bdbdbd \
+                pressed #4c4c4c]
+
+        ttk::style element create Button.button image \
+            [list $sprites(btn_rest) \
+                {selected disabled} $sprites(btn_disabled) \
+                disabled $sprites(btn_disabled) \
+                selected $sprites(btn_rest) \
+                pressed $sprites(btn_pressed) \
+                active $sprites(btn_hover) \
+            ] -border 4 -sticky nsew
+
+        # Scrollbar Elements
+        ttk::style element create Horizontal.Scrollbar.trough image $sprites(scroll_hor_trough) -sticky ew -border 6
+        ttk::style element create Horizontal.Scrollbar.thumb image $sprites(scroll_hor_thumb) -sticky ew -border 3
+
+        ttk::style element create Horizontal.Scrollbar.rightarrow image $sprites(scroll_right) -sticky {} -width 12
+        ttk::style element create Horizontal.Scrollbar.leftarrow image $sprites(scroll_left) -sticky {} -width 12
+
+        ttk::style element create Vertical.Scrollbar.trough image $sprites(scroll_vert_trough) -sticky ns -border 6
+        ttk::style element create Vertical.Scrollbar.thumb image $sprites(scroll_vert_thumb) -sticky ns -border 3
+
+        ttk::style element create Vertical.Scrollbar.uparrow image $sprites(scroll_up) -sticky {} -height 12
+        ttk::style element create Vertical.Scrollbar.downarrow image $sprites(scroll_down) -sticky {} -height 12
+
+        # Scale Elements
+        ttk::style element create Horizontal.Scale.trough image $sprites(scale_trough_hor) -border 5 -padding 0
+
+        ttk::style element create Vertical.Scale.trough image $sprites(scale_trough_vert) -border 5 -padding 0
+
+        ttk::style element create Scale.slider \
+            image [list $sprites(scale_thumb_rest) \
+                disabled $sprites(scale_thumb_disabled) \
+                pressed $sprites(scale_thumb_pressed) \
+                active $sprites(scale_thumb_hover) \
+            ] -sticky {}
+
+        # Checkbutton Configuration
+        ttk::style configure TCheckbutton -width 16 -padding {1 1} -border 0 -foreground $colors(-fg) -background $colors(-bg)
+
+        ttk::style element create Checkbutton.indicator image \
+            [list $sprites(check_unsel_rest) \
+                {alternate disabled} $sprites(check_tri_disabled) \
+                {selected disabled} $sprites(check_disabled) \
+                disabled $sprites(check_unsel_disabled) \
+                {pressed alternate} $sprites(check_tri_hover) \
+                {active alternate} $sprites(check_tri_hover) \
+                alternate $sprites(check_tri_rest) \
+                {pressed selected} $sprites(check_hover) \
+                {active selected} $sprites(check_hover) \
+                selected $sprites(check_rest) \
+                {pressed !selected} $sprites(check_unsel_pressed) \
+                active $sprites(check_unsel_hover) \
+            ] -width 26 -sticky w
+    }
+}
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.36.1/src/subsearch/gui/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-# Made by rdbende @ https://github.com/rdbende/Sun-Valley-ttk-theme
-# Modified and new assets by vagabondHustler
+source [file join [file dirname [info script]] ttk_subsearch_theme.tcl]
 
+option add *tearOff 0
 
-source [file join [file dirname [info script]] dark.tcl]
+proc set_theme {} {
+    
+    ttk::style theme use "ttk_subsearch_theme"
 
-option add *tearOff 0
+    array set colors {
+        -fg             "#ffffff"
+        -bg             "#1c1c1c"
+        -disabledfg     "#59959"
+        -selectfg       "#ffffff"
+        -selectbg       "#2f60d8"
+    }
+    
+    ttk::style configure . \
+        -background $colors(-bg) \
+        -foreground $colors(-fg) \
+        -troughcolor $colors(-bg) \
+        -focuscolor $colors(-selectbg) \
+        -selectbackground $colors(-selectbg) \
+        -selectforeground $colors(-selectfg) \
+        -insertwidth 1 \
+        -insertcolor $colors(-fg) \
+        -fieldbackground $colors(-bg) \
+        -font {"Cascadia" 8 bold} \
+        -borderwidth 0 \
+        -relief flat
+
+    tk_setPalette \
+        background [ttk::style lookup . -background] \
+        foreground [ttk::style lookup . -foreground] \
+        highlightColor [ttk::style lookup . -focuscolor] \
+        selectBackground [ttk::style lookup . -selectbackground] \
+        selectForeground [ttk::style lookup . -selectforeground] \
+        activeBackground [ttk::style lookup . -selectbackground] \
+        activeForeground [ttk::style lookup . -selectforeground]
+    
+    ttk::style map . -foreground [list disabled $colors(-disabledfg)]
 
-proc set_theme {mode} {
-    if {$mode == "dark"} {
-        ttk::style theme use "ttk_style"
-
-        array set colors {
-            -fg             "#ffffff"
-            -bg             "#1c1c1c"
-            -disabledfg     "#59959"
-            -selectfg       "#ffffff"
-            -selectbg       "#2f60d8"
-        }
-        
-        ttk::style configure . \
-            -background $colors(-bg) \
-            -foreground $colors(-fg) \
-            -troughcolor $colors(-bg) \
-            -focuscolor $colors(-selectbg) \
-            -selectbackground $colors(-selectbg) \
-            -selectforeground $colors(-selectfg) \
-            -insertwidth 1 \
-            -insertcolor $colors(-fg) \
-            -fieldbackground $colors(-bg) \
-            -font {"Cascadia" 8 bold} \
-            -borderwidth 0 \
-            -relief flat
-
-        tk_setPalette \
-            background [ttk::style lookup . -background] \
-            foreground [ttk::style lookup . -foreground] \
-            highlightColor [ttk::style lookup . -focuscolor] \
-            selectBackground [ttk::style lookup . -selectbackground] \
-            selectForeground [ttk::style lookup . -selectforeground] \
-            activeBackground [ttk::style lookup . -selectbackground] \
-            activeForeground [ttk::style lookup . -selectforeground]
-        
-        ttk::style map . -foreground [list disabled $colors(-disabledfg)]
+    option add *font [ttk::style lookup . -font]
 
-        option add *font [ttk::style lookup . -font]
     
-    }
 }
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tab_manager.py` & `Subsearch-2.36.1/src/subsearch/gui/tab_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tkinter as tk
 from typing import Any
 
-from subsearch.data import GUI_DATA, __version__, app_paths
+from subsearch.data import __version__, gui
 from subsearch.data.data_objects import PrettifiedDownloadData
-from subsearch.gui import set_theme, tkinter_utils
+from subsearch.gui import gui_toolkit, root
 from subsearch.gui.tabs import dowload_tab, language_tab, search_tab, settings_tab
-from subsearch.utils import file_manager, io_json, io_winreg
+from subsearch.utils import file_manager
 
 
 class TabManager(tk.Frame):
     """
     A class used to manage the tabs of a parent widget.
 
     Args:
@@ -31,162 +31,142 @@
         enter_tab(event): Called when mouse enters a tab button. Bind '<ButtonPress>' event to the button widget.
         leave_tab(event):  Called when mouse leaves a tab button. Unbind '<ButtonPress>' event from the button widget, and call 'activate_tabs()' and 'deactivate_tabs()' methods.
         get_btn(dict_, event_, equals=True): Helper method to retrieve the button widget and its key.
     """
 
     def __init__(self, parent, tabs: dict[str, Any], active_tab: str) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.mid_grey_black, width=GUI_DATA.size.root_width, height=82)
+        self.configure(bg=gui.colors.mid_grey_black, width=gui.size.root_width, height=82)
         relx_value = 0.0
         btn_kwargs: dict[str, Any] = dict(
-            master=self, width=54, height=54, bg=GUI_DATA.colors.mid_grey_black, highlightthickness=0
+            master=self, width=54, height=54, bg=gui.colors.mid_grey_black, highlightthickness=0
         )
         self.parent = parent
         self.tabs = tabs
         self.buttons = {}
 
         for tab_key in tabs.keys():
             self.buttons[tab_key] = tk.Canvas(**btn_kwargs)
 
         for btn_key, btn_widget in self.buttons.items():
             relx_value += 0.2
             btn_widget.place(relx=relx_value, rely=0.5, anchor="center")
             btn_widget.bind("<Enter>", self.enter_tab)
             btn_widget.bind("<Leave>", self.leave_tab)
-            tkinter_utils.asset_tab(btn_widget, btn_key, "rest")
+            gui_toolkit.asset_tab(btn_widget, btn_key, "rest")
 
-        tkinter_utils.set_default_grid_size(self)
+        gui_toolkit.set_default_grid_size(self)
         self.active_tab = active_tab
         self.activate_tabs()
 
     def activate_tabs(self) -> None:
-        self.tabs[self.active_tab].place(x=GUI_DATA.pos.content_x, y=GUI_DATA.pos.content_y, anchor="center")
-        tkinter_utils.asset_tab(self.buttons[self.active_tab], self.active_tab, "press")
-        self.parent.title(f"Subsearch {__version__} - {self.active_tab} tab")
+        self.tabs[self.active_tab].place(x=gui.pos.content_x, y=gui.pos.content_y, anchor="center")
+        gui_toolkit.asset_tab(self.buttons[self.active_tab], self.active_tab, "press")
+        self.parent.title(f"Subsearch {__version__} - {self.active_tab.capitalize()} tab")
 
     def release_tab(self, event) -> None:
         btn_key, _btn_widget = self.get_btn(self.buttons, event)
         self.active_tab = btn_key
         self.activate_tabs()
         self.deactivate_tabs()
 
     def press_tab(self, event) -> None:
         btn_key, btn_widget = self.get_btn(self.buttons, event, False)
         btn_widget.bind("<ButtonRelease>", self.release_tab)
-        tkinter_utils.asset_tab(btn_widget, btn_key, "press", y=20)
+        gui_toolkit.asset_tab(btn_widget, btn_key, "press", y=20)
 
     def deactivate_tabs(self) -> None:
         for btn_key, btn_widget in self.buttons.items():
             if self.active_tab == btn_key:
                 continue
-            self.tabs[btn_key].place(x=GUI_DATA.pos.content_hidden_x, y=GUI_DATA.pos.content_y, anchor="nw")
-            tkinter_utils.asset_tab(btn_widget, btn_key, "rest")
+            self.tabs[btn_key].place(x=gui.pos.content_hidden_x, y=gui.pos.content_y, anchor="nw")
+            gui_toolkit.asset_tab(btn_widget, btn_key, "rest")
 
     def enter_tab(self, event) -> None:
         _btn_key, btn_widget = self.get_btn(self.buttons, event)
         btn_widget.bind("<ButtonPress>", self.press_tab)
+        gui_toolkit.asset_tab(self.buttons[_btn_key], _btn_key, "hover")
 
     def leave_tab(self, event) -> None:
         _btn_key, btn_value = self.get_btn(self.buttons, event)
         btn_value.unbind("<ButtonPress>")
-        self.activate_tabs()
-        self.deactivate_tabs()
+        gui_toolkit.asset_tab(self.buttons[_btn_key], _btn_key, "rest" if _btn_key != self.active_tab else "press")
 
     def get_btn(self, dict_, event_, equals=True):
         for btn_key, btn_widget in dict_.items():
             if event_.widget == btn_widget and equals:
                 return btn_key, btn_widget
             if event_.widget == btn_widget and not equals:
                 return btn_key, btn_widget
 
 
 class TabLanguage(tk.Frame):
     def __init__(self, parent) -> None:
-        tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        tk.Frame.__init__(self, parent, width=gui.size.root_width, height=gui.size.root_height)
+        self.configure(bg=gui.colors.dark_grey)
         language_tab.SelectLanguage(self).pack(anchor="center", expand=True)
 
 
 class TabSearch(tk.Frame):
     def __init__(self, parent) -> None:
-        tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        tk.Frame.__init__(self, parent, width=gui.size.root_width, height=gui.size.root_height)
+        self.configure(bg=gui.colors.dark_grey)
         search_tab.Providers(self).pack(anchor="center")
-        tk.Frame(self, height=80, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
+        tk.Frame(self, height=80, bg=gui.colors.dark_grey).pack(anchor="center", expand=True)
         search_tab.SubtitleType(self).pack(anchor="center")
         search_tab.SearchThreshold(self).pack(anchor="center")
         search_tab.ForeignOnly(self).pack(anchor="center")
         search_tab.RenameBestMatch(self).pack(anchor="center")
 
 
 class TabSettings(tk.Frame):
     def __init__(self, parent) -> None:
-        tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        tk.Frame.__init__(self, parent, width=gui.size.root_width, height=gui.size.root_height)
+        self.configure(bg=gui.colors.dark_grey)
         settings_tab.FileExtensions(self).pack(anchor="center")
-        tk.Frame(self, height=80, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
+        tk.Frame(self, height=80, bg=gui.colors.dark_grey).pack(anchor="center", expand=True)
         settings_tab.ShowContextMenu(self).pack(anchor="center")
         settings_tab.ShowContextMenuIcon(self).pack(anchor="center")
         settings_tab.ShowDownloadWindow(self).pack(anchor="center")
         settings_tab.UseThreading(self).pack(anchor="center")
         settings_tab.MultipleAppInstances(self).pack(anchor="center")
         settings_tab.LogToFile(self).pack(anchor="center")
         if file_manager.running_from_exe() is False:
             settings_tab.ShowTerminalOnSearch(self).pack(anchor="center")
-        tk.Frame(self, height=20, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
+        tk.Frame(self, height=20, bg=gui.colors.dark_grey).pack(anchor="center", expand=True)
         settings_tab.CheckForUpdates(self).pack(anchor="center")
 
 
 class TabDownload(tk.Frame):
     def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
-        tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        tk.Frame.__init__(self, parent, width=gui.size.root_width, height=gui.size.root_height)
+        self.configure(bg=gui.colors.dark_grey)
         dowload_tab.DownloadList(self, formatted_data).pack(anchor="center")
 
 
 def open_tab(active_tab: str, **kwargs) -> None:
     """
     Opens a new tab depending on the active_tab argument passed in.
 
     Args:
         active_tab (str): A string representing which tab to activate.
-        **kwargs: Arbitrary keyword arguments that should contain "formatted_data",
-                  a list of FormattedMetadata.
 
     Returns:
         None: This function does not return anything, it manipulates the GUI instead.
     """
     try:
-        formatted_data: list[PrettifiedDownloadData] = kwargs["formatted_data"]
+        data: list[PrettifiedDownloadData] = kwargs["data"]
     except KeyError:
-        formatted_data = None  # type: ignore
-    root = initialize_root()
-    set_theme("dark")
-    tkinter_utils.set_custom_btn_styles()
+        data = []
+    root
+    gui_toolkit.configure_root(root)
+    gui_toolkit.set_ttk_theme(root)
+    gui_toolkit.set_custom_btn_styles()
     tabs = {
         "language": TabLanguage(root),
         "search": TabSearch(root),
         "settings": TabSettings(root),
-        "download": TabDownload(root, formatted_data),
+        "download": TabDownload(root, data),
     }
     footer = TabManager(root, tabs, active_tab.lower())
-    footer.place(y=GUI_DATA.size.root_height - 82)
+    footer.place(y=gui.size.root_height - 82)
     root.mainloop()
-
-
-def initialize_root():
-    """
-    Initialize the root Tkinter window for the Subsearch application.
-
-    Returns:
-        tk.Tk: The initialized Tkinter root window.
-    """
-    if io_json.APPCON_JSON.exists() is False:
-        io_json.create_application_config_json()
-    if io_json.get_json_key("context_menu"):
-        io_winreg.add_context_menu()
-    root = tk.Tk(className=f"Subsearch")
-    root.configure(background=GUI_DATA.colors.dark_grey)
-    root.iconbitmap(app_paths.icon)
-    root.geometry(tkinter_utils.WindowPosition.set(root))  # type: ignore
-    root.resizable(False, False)
-    return root
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.36.1/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import re
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.data import GUI_DATA, app_paths, video_data
+from subsearch.data import app_paths, gui, video_data
 from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.providers import subscene
 from subsearch.utils import file_manager, log
 
 
 class DownloadList(tk.Frame):
     def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
         tk.Frame.__init__(self, parent)
         root_posx, root_posy = parent.winfo_reqwidth(), parent.winfo_reqheight()
-        self.configure(bg=GUI_DATA.colors.dark_grey, width=root_posx, height=root_posy - 82)
+        self.configure(bg=gui.colors.dark_grey, width=root_posx, height=root_posy - 82)
         if formatted_data is not None:
             formatted_data.sort(key=lambda x: x.pct_result, reverse=True)
         self.formatted_data = formatted_data
         self.subscene_scrape = subscene.SubsceneScraper()
         self.extent = 0
         self.scrollbar = ttk.Scrollbar(self, orient="vertical", style="Vertical.TScrollbar")
         self.sub_listbox = tk.Listbox(
             self,
             height=root_posy,
-            bg=GUI_DATA.colors.dark_grey,
-            fg=GUI_DATA.colors.light_grey,
-            font=GUI_DATA.fonts.cas8b,
+            bg=gui.colors.dark_grey,
+            fg=gui.colors.light_grey,
+            font=gui.fonts.cas8b,
             bd=0,
             border=0,
             borderwidth=0,
             highlightthickness=0,
             activestyle="none",
             yscrollcommand=self.scrollbar.set,
         )
@@ -75,15 +75,15 @@
         self.sub_listbox.delete(int(item_num))
         self.sub_listbox.insert(int(item_num), f"» DOWNLOADING «")
         for enum, _provider, _release, _url in zip(
             self._providers.keys(), self._providers.values(), self._releases.values(), self._urls.values()
         ):
             if enum != int(item_num):
                 continue
-            self.sub_listbox.itemconfig(int(enum), {"fg": GUI_DATA.colors.blue})
+            self.sub_listbox.itemconfig(int(enum), {"fg": gui.colors.blue})
             if _provider == "subscene":
                 download_url = self.subscene_scrape.get_download_url(_url)
             else:
                 download_url = _url
             path = f"{ app_paths.tmpdir}\\__{_provider}__{item_num}.zip"
             enum = DownloadData(
                 provider=f"Downloading from {_provider}",
@@ -95,8 +95,8 @@
             )  # type: ignore
             file_manager.download_subtitle(enum)  # type: ignore
             file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
             file_manager.delete_temp_files(app_paths.tmpdir)
             break
         self.sub_listbox.delete(int(item_num))
         self.sub_listbox.insert(int(item_num), f"✔ {_release}")
-        self.sub_listbox.itemconfig(int(item_num), {"fg": GUI_DATA.colors.green})
+        self.sub_listbox.itemconfig(int(item_num), {"fg": gui.colors.green})
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.36.1/src/subsearch/gui/tabs/language_tab.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.data import GUI_DATA
-from subsearch.gui import tkinter_utils
+from subsearch.data import gui
+from subsearch.gui import gui_toolkit
 from subsearch.utils import io_json
 
 
 class SelectLanguage(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.active_btn = None
         self.rownum = 0
         self.colnum = 1
         self.checkbox_values = {}
         self.name_find_key = {}
         self.tip_present = False
         self.languages = io_json.get_available_languages()
@@ -34,23 +34,23 @@
             if valuevar.get() == 1:
                 self.active_btn = btn
 
             btn.bind("<Enter>", self.enter_button)
             btn.bind("<Leave>", self.leave_button)
             self.rownum += 1
             self.name_find_key[language_data["name"]] = language
-        tkinter_utils.set_default_grid_size(self, width_=6)
+        gui_toolkit.set_default_grid_size(self, width_=6)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         json_key = self.name_find_key[btn["text"]]
         providers = ", ".join(([_i.title() for _i in self.languages[json_key]["incompatibility"]]))
         if providers:
             tip_text = f"If enabled, '{providers}' will be automatically skipped."
-            self.tip = tkinter_utils.ToolTip(btn, btn, tip_text)
+            self.tip = gui_toolkit.ToolTip(btn, btn, tip_text)
             self.tip.show()
             self.tip_present = True
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def leave_button(self, event) -> None:
         btn = event.widget
         if self.tip_present:
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.36.1/src/subsearch/gui/tabs/search_tab.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.data import GUI_DATA
-from subsearch.gui import tkinter_utils
+from subsearch.data import gui
+from subsearch.gui import gui_toolkit
 from subsearch.utils import io_json
 
 
 class Providers(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.providers = io_json.get_json_key("providers")
         self.data = io_json.get_json_data()
         label = tk.Label(self, text="Search providers")
-        label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
+        label.configure(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
         label.grid(row=1, column=0, sticky="w", padx=2, pady=2)
         self.rownum = 0
         self.colnum = 2
         self.checkbox_value = {}
         self.last_key = ""
         for key, value in self.providers.items():
             btn_txt = key.split("_")[-1].capitalize()
@@ -26,29 +26,29 @@
             valuevar.set(value)
             if self.last_key.startswith(lbl_txt):
                 self.colnum += 1
             if self.last_key != lbl_txt:
                 self.rownum += 1
                 self.colnum = 2
                 _lbl = tk.Label(self, text=lbl_txt)
-                _lbl.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
+                _lbl.configure(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
                 _lbl.grid(row=self.rownum, column=2, sticky="w", padx=2, pady=2)
             else:
                 self.rownum -= 1
             self.rownum += 1
             self.last_key = lbl_txt
             btn = ttk.Checkbutton(self, text=btn_txt, onvalue=True, offvalue=False, variable=valuevar)
             btn.grid(row=self.rownum, column=self.colnum, pady=2)
             self.checkbox_value[btn] = key, valuevar
             if self.data["providers"][key] is True:
                 btn.configure(state="normal")
 
             btn.bind("<Enter>", self.enter_button)
             btn.bind("<Leave>", self.leave_button)
-        tkinter_utils.set_default_grid_size(self)
+        gui_toolkit.set_default_grid_size(self)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def leave_button(self, event) -> None:
         btn = event.widget
@@ -69,36 +69,36 @@
         io_json.set_json_data(self.data)
 
     def toggle_providers(self, event) -> None:
         btn = event.widget
         key = btn["text"].replace(" ", "_").lower()
         if self.data["providers"][key] is True:
             self.data["providers"][key] = False
-            btn.configure(fg=GUI_DATA.colors.red)
+            btn.configure(fg=gui.colors.red)
         elif self.data["providers"][key] is False:
             self.data["providers"][key] = True
-            btn.configure(fg=GUI_DATA.colors.green)
+            btn.configure(fg=gui.colors.green)
         io_json.set_json_data(self.data)
 
 
 class SubtitleType(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.subtitle_type = io_json.get_json_key("subtitle_type")
         self.string_var = tk.StringVar()
         self.data = io_json.get_json_data()
         label = tk.Label(self, text="Subtitle type")
-        label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
+        label.configure(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
         label.grid(row=1, column=0, sticky="w", padx=2, pady=2)
         self.clabel = tk.Label(self, textvariable=self.string_var)
-        self.clabel.configure(bg=GUI_DATA.colors.dark_grey, font=GUI_DATA.fonts.cas8b)
+        self.clabel.configure(bg=gui.colors.dark_grey, font=gui.fonts.cas8b)
         self.clabel.grid(row=1, column=1, sticky="nsew", padx=2, pady=2)
         self.sub_type_txt()
-        tkinter_utils.VarColorPicker(self.string_var, self.clabel)
+        gui_toolkit.VarColorPicker(self.string_var, self.clabel)
         self.rownum = 0
         self.colnum = 2
         self.checkbox_values = {}
         for key, value in self.subtitle_type.items():
             if key.startswith("non"):
                 _text = "Regular"
             else:
@@ -110,15 +110,15 @@
                 self.rownum = 1
                 self.colnum += 1
             btn = ttk.Checkbutton(self, text=_text, onvalue=True, offvalue=False, variable=valuevar)
             btn.grid(row=self.rownum, column=self.colnum, pady=2)
             self.checkbox_values[btn] = key, valuevar
 
             btn.bind("<Enter>", self.enter_button)
-            tkinter_utils.set_default_grid_size(self)
+            gui_toolkit.set_default_grid_size(self)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def press_button(self, event) -> None:
         btn = event.widget
@@ -140,39 +140,39 @@
         nonhi_sub = self.data["subtitle_type"]["non_hearing_impaired"]
         if (hi_sub and nonhi_sub) or (hi_sub is False and nonhi_sub is False):
             self.string_var.set(f"Both")
         if hi_sub and nonhi_sub is False:
             self.string_var.set(f"Only HI")
         if hi_sub is False and nonhi_sub:
             self.string_var.set(f"Only non-HI")
-        tkinter_utils.VarColorPicker(self.string_var, self.clabel)
+        gui_toolkit.VarColorPicker(self.string_var, self.clabel)
 
 
 class SearchThreshold(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.pct_threashold = io_json.get_json_key("percentage_threshold")
         self.current_value = tk.IntVar()
         self.current_value.set(self.pct_threashold)
         self.string_var = tk.StringVar()
         self.string_var.set(f"{self.pct_threashold} %")
         label = tk.Label(self, text="Search threshold")
-        label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
+        label.configure(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
         label.grid(row=0, column=0, sticky="w", padx=0, pady=2)
         self.clabel = tk.Label(self, textvariable=self.string_var)
-        self.clabel.configure(bg=GUI_DATA.colors.dark_grey, font=GUI_DATA.fonts.cas8b)
+        self.clabel.configure(bg=gui.colors.dark_grey, font=gui.fonts.cas8b)
         self.clabel.grid(row=0, column=1, sticky="nsew", padx=2, pady=2)
-        tkinter_utils.VarColorPicker(self.string_var, self.clabel, True)
-        x, y = tkinter_utils.calculate_btn_size(self, 36)
+        gui_toolkit.VarColorPicker(self.string_var, self.clabel, True)
+        x, y = gui_toolkit.calculate_btn_size(self, 36)
         self.slider = ttk.Scale(self, from_=0, to=100, orient="horizontal", variable=self.current_value, length=x - 2)
         self.slider.grid(column=2, row=0, sticky="we", padx=4)
         self.slider.bind("<Enter>", self.enter_button)
         self.slider.bind("<Leave>", self.leave_button)
-        tkinter_utils.set_default_grid_size(self)
+        gui_toolkit.set_default_grid_size(self)
 
     def get_value(self):
         return self.current_value.get()
 
     def set_value(self, event) -> None:
         self.string_var.set(f"{self.get_value()} %")
 
@@ -206,31 +206,31 @@
         if btn == self.slider:
             self.slider.configure(command=self.set_value)
             self.update_config()
 
     def update_config(self) -> None:
         update_svar = self.current_value.get()
         io_json.set_config_key_value("percentage_threshold", update_svar)
-        tkinter_utils.VarColorPicker(self.string_var, self.clabel, True)
+        gui_toolkit.VarColorPicker(self.string_var, self.clabel, True)
 
 
-class ForeignOnly(tkinter_utils.ToggleableFrameButton):
+class ForeignOnly(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
         text = f"If 'True', 'OpenSubtitles, Yifysubtitles' will be automatically skipped."
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Foreign language only", "foreign_only", tip_text=text)
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Foreign language only", "foreign_only", tip_text=text)
 
 
-class RenameBestMatch(tkinter_utils.ToggleableFrameButton):
+class RenameBestMatch(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Rename best match", "rename_best_match")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Rename best match", "rename_best_match")
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.36.1/src/subsearch/gui/tabs/settings_tab.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import tkinter as tk
 import webbrowser
 from tkinter import ttk
 
-from subsearch.data import GUI_DATA, __version__
-from subsearch.gui import tkinter_utils
+from subsearch.data import __version__, gui
+from subsearch.gui import gui_toolkit
 from subsearch.utils import io_json, update
 
 
 class FileExtensions(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.data = io_json.get_json_data()
         self.file_extensions = io_json.get_json_key("file_extensions")
         number_of_buttons = len(self.file_extensions.items())
         label = tk.Label(self, text="File extensions")
-        label.configure(tkinter_utils.DEFAULT_LABEL_CONFIG)
-        label.grid(tkinter_utils.DEFAULT_LABEL_GRID)
+        label.configure(gui_toolkit.DEFAULT_LABEL_CONFIG)
+        label.grid(gui_toolkit.DEFAULT_LABEL_GRID)
         self.rownum = 0
         self.colnum = 0
         self.checkbox_value = {}
         number_of_rows = 4
 
         for _i, (key, value) in zip(range(number_of_buttons), self.file_extensions.items()):
             self.rownum += 1
@@ -30,15 +30,15 @@
 
             valuevar = tk.BooleanVar()
             valuevar.set(value)
             btn = ttk.Checkbutton(self, text=key, onvalue=True, offvalue=False, variable=valuevar)
             btn.grid(row=self.rownum, column=self.colnum, pady=2)
             self.checkbox_value[btn] = key, valuevar
             btn.bind("<Enter>", self.enter_button)
-        tkinter_utils.set_default_grid_size(self)
+        gui_toolkit.set_default_grid_size(self)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def press_button(self, event) -> None:
         btn = event.widget
@@ -58,109 +58,109 @@
 
     def update_registry(self) -> None:
         from subsearch.utils import io_winreg
 
         io_winreg.write_all_valuex()
 
 
-class ShowContextMenu(tkinter_utils.ToggleableFrameButton):
+class ShowContextMenu(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Context menu", "context_menu", write_to_reg=True)
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Context menu", "context_menu", write_to_reg=True)
 
 
-class ShowContextMenuIcon(tkinter_utils.ToggleableFrameButton):
+class ShowContextMenuIcon(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Context menu icon", "context_menu_icon")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Context menu icon", "context_menu_icon")
 
 
-class ShowDownloadWindow(tkinter_utils.ToggleableFrameButton):
+class ShowDownloadWindow(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Download window", "manual_download_fail")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Download window", "manual_download_fail")
 
 
-class ShowTerminalOnSearch(tkinter_utils.ToggleableFrameButton):
+class ShowTerminalOnSearch(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Terminal on search", "show_terminal", show_if_exe=False)
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Terminal on search", "show_terminal", show_if_exe=False)
 
 
-class LogToFile(tkinter_utils.ToggleableFrameButton):
+class LogToFile(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Log to file", "log_to_file")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Log to file", "log_to_file")
 
 
-class UseThreading(tkinter_utils.ToggleableFrameButton):
+class UseThreading(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Use threading", "use_threading")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Use threading", "use_threading")
 
 
-class MultipleAppInstances(tkinter_utils.ToggleableFrameButton):
+class MultipleAppInstances(gui_toolkit.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
 
     def __init__(self, parent) -> None:
-        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Multiple app instances", "multiple_app_instances")
+        gui_toolkit.ToggleableFrameButton.__init__(self, parent, "Multiple app instances", "multiple_app_instances")
 
 
 class CheckForUpdates(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
-        self.latest_version = None
+        self.configure(bg=gui.colors.dark_grey)
+        self.latest_version = ""
         self.btn_search = ttk.Button(
             self,
             text="Search for updates",
             width=40,
         )
         self.btn_visit_release_page = ttk.Button(
             self,
             text="Open in webbrowser",
             width=40,
         )
         self.btn_search.grid(row=0, column=2, pady=2)
         self.btn_search.bind("<Enter>", self.enter_button)
-        tkinter_utils.set_default_grid_size(self)
+        gui_toolkit.set_default_grid_size(self)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         if btn == self.btn_search:
             btn.bind("<ButtonRelease-1>", self.search_button)
 
     def search_button(self, event) -> None:
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.36.1/src/subsearch/gui/gui_toolkit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import tkinter as tk
-from pathlib import Path
 from tkinter import Label, StringVar, ttk
 
-from subsearch.data import GUI_DATA, __version__, app_paths
+from PIL import Image, ImageTk
+
+from subsearch.data import __version__, app_paths, gui
+from subsearch.gui import spritesheet_data
 from subsearch.utils import file_manager, io_json, io_winreg
 
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
 WS_EX_TOOLWINDOW = 0x00000080
 
-DEFAULT_LABEL_CONFIG = dict(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
+DEFAULT_LABEL_CONFIG = dict(bg=gui.colors.dark_grey, fg=gui.colors.white_grey, font=gui.fonts.cas8b)
 DEFAULT_LABEL_GRID = dict(row=0, column=0, sticky="w", padx=2, pady=2)
 DEFAULT_BTN_TOGGLE_GRID = dict(row=0, column=2, pady=2)
 
 
-def get_tab_png(tab: str) -> Path:
-    """
-    Get the path of the PNG file for a given tab.
-
-    Args:
-        tab (str): The name of the tab.
-
-    Returns:
-        Path: The path of the PNG file for the specified tab.
-
-    Raises:
-        None.
-    """
-    return Path(app_paths.tabs) / tab
+def get_sprite(sprite_name):
+    spritesheet_path = app_paths.gui_assets / "spritesheet.png"
+    spritesheet_image = Image.open(spritesheet_path)
+    sprite_x = spritesheet_data[sprite_name][0]
+    sprite_y = spritesheet_data[sprite_name][1]
+    sprite_width = spritesheet_data[sprite_name][2]
+    sprite_height = spritesheet_data[sprite_name][3]
+    sprite = spritesheet_image.crop((sprite_x, sprite_y, sprite_x + sprite_width, sprite_y + sprite_height))
+    return sprite
 
 
 def calculate_btn_size(cls, width_=18, height_=2) -> tuple[int, int]:
     """
     Calculate the required size of a button based on its content.
 
     Args:
@@ -92,16 +89,16 @@
     Args:
         cls (class): The class representing the application.
         img (str): The name of the image file.
         type (str): The type of the image file.
         x (int, optional): The width of the image in pixels. Defaults to 27.
         y (int, optional): The height of the image in pixels. Defaults to 27.
     """
-    path = get_tab_png(f"{img}_{type}.png")
-    png = tk.PhotoImage(file=path)
+    path = get_sprite(f"{img}_{type}")
+    png = ImageTk.PhotoImage(path)
     update_asset(cls, png, x, y)
 
 
 def update_asset(cls, img, x, y) -> None:
     """
     Updates an asset in a tkinter canvas with the provided image.
 
@@ -128,16 +125,16 @@
         None
 
     Returns:
         None
     """
 
     custom_style = ttk.Style()
-    custom_style.configure("True.TButton", foreground=GUI_DATA.colors.green)
-    custom_style.configure("False.TButton", foreground=GUI_DATA.colors.red)
+    custom_style.configure("True.TButton", foreground=gui.colors.green)
+    custom_style.configure("False.TButton", foreground=gui.colors.red)
 
 
 class WindowPosition(tk.Frame):
     """
     A class that creates and manages the positioning of a tkinter frame.
 
     Args:
@@ -163,16 +160,16 @@
         Args:
             parent: The parent widget.
         """
         tk.Frame.__init__(self, parent)
 
     def set(
         self,
-        w=GUI_DATA.size.root_width,
-        h=GUI_DATA.size.root_height,
+        w=gui.size.root_width,
+        h=gui.size.root_height,
         ws_value_offset=0,
         hs_value_offset=0,
         other: bool = False,
     ):
         """
         Set the size of the current window/Frame
 
@@ -219,32 +216,32 @@
         self.string_var = string_var
         self.clabel = clabel
         self.is_pct = is_pct
         self.pick()
 
     def pick(self) -> None:
         if self.string_var.get() == "True":
-            self.clabel.configure(fg=GUI_DATA.colors.green)
+            self.clabel.configure(fg=gui.colors.green)
         elif self.string_var.get() == "False":
-            self.clabel.configure(fg=GUI_DATA.colors.red)
+            self.clabel.configure(fg=gui.colors.red)
         elif self.string_var.get() == "Both":
-            self.clabel.configure(fg=GUI_DATA.colors.blue)
+            self.clabel.configure(fg=gui.colors.blue)
         elif self.string_var.get().startswith("Only"):
-            self.clabel.configure(fg=GUI_DATA.colors.green)
+            self.clabel.configure(fg=gui.colors.green)
 
         if self.is_pct:
             _pct = io_json.get_json_key("percentage_threshold")
             if _pct in range(75, 101):
-                self.clabel.configure(fg=GUI_DATA.colors.green)
+                self.clabel.configure(fg=gui.colors.green)
             elif _pct in range(50, 75):
-                self.clabel.configure(fg=GUI_DATA.colors.green_brown)
+                self.clabel.configure(fg=gui.colors.green_brown)
             elif _pct in range(25, 50):
-                self.clabel.configure(fg=GUI_DATA.colors.red_brown)
+                self.clabel.configure(fg=gui.colors.red_brown)
             elif _pct in range(0, 25):
-                self.clabel.configure(fg=GUI_DATA.colors.red)
+                self.clabel.configure(fg=gui.colors.red)
 
 
 class ToolTip(tk.Toplevel):
     """
     A toplevel widget that displays a message when the user hovers over a specified widget
 
     Args:
@@ -253,33 +250,33 @@
         *_text (str): The text to be displayed in the tooltip
         _background (str): The background color of the tooltip
 
     Methods:
         show(): Creates and displays a toplevel widget containing the text to be displayed in the tooltip
     """
 
-    def __init__(self, parent, _widget, *_text, _background=GUI_DATA.colors.light_black):
+    def __init__(self, parent, _widget, *_text, _background=gui.colors.light_black):
         self.parent = parent
         self.widget = _widget
         self.text = _text
         self.background = _background
 
     def show(self) -> None:
         tk.Toplevel.__init__(self, self.parent)
-        self.configure(background=GUI_DATA.colors.light_black)
+        self.configure(background=gui.colors.light_black)
         # remove the standard window titlebar from the tooltip
         self.overrideredirect(True)
         # unpack *args and put each /n on a new line
         lines = "\n".join(self.text)
-        frame = tk.Frame(self, background=GUI_DATA.colors.light_black)
+        frame = tk.Frame(self, background=gui.colors.light_black)
         label = tk.Label(
             frame,
             text=lines,
             background=self.background,
-            foreground=GUI_DATA.colors.white_grey,
+            foreground=gui.colors.white_grey,
             justify="left",
         )
         # get size of the label to use later for positioning and sizing of the tooltip
         x, y = label.winfo_reqwidth(), label.winfo_reqheight()
         # set the size of the tooltip background to be 1px larger than the label
         frame.configure(width=x + 1, height=y + 1)
 
@@ -304,34 +301,32 @@
 
 class ToggleableFrameButton(tk.Frame):
     """
     A button that toggles a configuration setting on or off.
 
     Args:
         parent (tk.Widget): The parent widget.
-        setting_label (str): Name of the setting to be displayeed.
+        setting_label (str): Name of the setting to be displayed.
         config_key (str): Key in the configuration file where the state is stored.
         write_to_reg (bool, optional): Whether to also write the state to registry. Defaults to False.
         show_if_exe (bool, optional): Only show the button if the program is not running from an executable. Defaults to True.
     """
 
-    def __init__(
-        self, parent, setting_label: str, config_key: str, write_to_reg: bool = False, show_if_exe=True, tip_text=None
-    ) -> None:
+    def __init__(self, parent, setting_label: str, config_key: str, **kwargs) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.configure(bg=gui.colors.dark_grey)
         self.string_var = tk.StringVar()
         self.string_var.set(f"{io_json.get_json_key(config_key)}")
         self.setting_name = setting_label
         self.config_key = config_key
-        self.write_to_reg = write_to_reg
-        self.show_if_exe = show_if_exe
-        self.tip_text = tip_text
+        self.write_to_reg = kwargs.get("write_to_reg", False)
+        self.show_if_exe = kwargs.get("write_to_reg", True)
+        self.tip_text = kwargs.get("tip_text", None)
         self.tip_present = False
-        if show_if_exe is False and file_manager.running_from_exe():
+        if self.show_if_exe is False and file_manager.running_from_exe():
             return None
         label = tk.Label(self, text=self.setting_name)
         label.configure(DEFAULT_LABEL_CONFIG)
         label.grid(DEFAULT_LABEL_GRID)
         btn_toggle = ttk.Button(
             self,
             textvariable=self.string_var,
@@ -398,7 +393,28 @@
         btn = event.widget
         self.string_var.set(f"False")
         btn["style"] = f"{self.string_var.get()}.TButton"
         io_json.set_config_key_value(self.config_key, False)
         if self.write_to_reg:
             io_winreg.remove_context_menu()
         self.enter_button(event)
+
+
+def set_ttk_theme(root):
+    initializer_tcl = app_paths.gui_app_theme / "ttk_theme_initializer.tcl"
+    root.tk.call("source", str(initializer_tcl))
+    root.tk.call("set_theme")
+
+
+def configure_root(root):
+    """
+    Initialize the root Tkinter window for the Subsearch application.
+
+    Returns:
+        tk.Tk: The initialized Tkinter root window.
+    """
+    if io_json.get_json_key("context_menu"):
+        io_winreg.add_context_menu()
+    root.configure(background=gui.colors.dark_grey)
+    root.iconbitmap(app_paths.gui_assets / "subsearch.ico")
+    root.geometry(WindowPosition.set(root))  # type: ignore
+    root.resizable(False, False)
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/providers/generic.py` & `Subsearch-2.36.1/src/subsearch/providers/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from pathlib import Path
 
 import cloudscraper
 from selectolax.parser import HTMLParser
 
 from subsearch.data.data_objects import (
     AppConfig,
     DownloadData,
@@ -15,15 +15,15 @@
 from subsearch.utils import io_json
 
 
 class CustomSubsceneHeader:
     def __init__(self, app_config: AppConfig) -> None:
         self.app_config = app_config
 
-    def _get_hearing_impaired_int(self) -> Literal[2, 1, 0]:
+    def _get_hearing_impaired_int(self) -> int:
         if self.app_config.hearing_impaired and self.app_config.non_hearing_impaired:
             value = 0
         if self.app_config.hearing_impaired and not self.app_config.non_hearing_impaired:
             value = 1
         if self.app_config.non_hearing_impaired and not self.app_config.hearing_impaired:
             value = 2
         return value
@@ -129,15 +129,15 @@
     if header_ is None:
         response = scraper.get(url)
     else:
         response = scraper.get(url, headers=header_)
     return HTMLParser(response.text)
 
 
-def create_download_data(provider: str, tmp_directory: str, to_be_downloaded: dict[str, str]) -> list[DownloadData]:
+def create_download_data(provider: str, tmp_directory: Path, to_be_downloaded: dict[str, str]) -> list[DownloadData]:
     """
     Creates a list of data for each downloaded file.
 
     Args:
         provider (str): The name of the file provider.
         tmp_directory (str): The directory where the temporary downloaded files will be saved.
         to_be_downloaded (dict[str,str]): A dictionary with the name and url of each file to be downloaded.
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.36.1/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/providers/subscene.py` & `Subsearch-2.36.1/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.36.1/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/app_integrity.py` & `Subsearch-2.36.1/src/subsearch/utils/app_integrity.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/exceptions.py` & `Subsearch-2.36.1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/file_manager.py` & `Subsearch-2.36.1/src/subsearch/utils/file_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import struct
 import sys
 import zipfile
 from pathlib import Path
 
-from subsearch.data import __guid__, app_paths, video_data
+from subsearch.data import __guid__, video_data
 from subsearch.data.data_objects import DownloadData
 from subsearch.providers.generic import get_cloudscraper
 from subsearch.utils import log, string_parser
 
 
 def running_from_exe() -> bool:
     """
@@ -75,15 +75,15 @@
         extension (str): The file type of the subtitles i.e ".srt".
 
     Returns:
         None.
     """
     if video_data is None:
         return None
-    best_match = (0, "")
+    best_match = (0, Path())
     for file in Path(video_data.subs_directory).glob(f"*{extension}"):
         value = string_parser.calculate_match(file.name, release_name)
         if value >= best_match[0]:
             best_match = value, file
     if not best_match[1]:
         return None
     file_to_rename = best_match[1]
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.36.1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/io_json.py` & `Subsearch-2.36.1/src/subsearch/utils/io_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     data = get_json_data(LANGS_JSON)
     language_data = LanguageData(**data[language])
     return language_data
 
 
 def get_language_data_value(key: str):
     data = get_language_data()
-    return data[key]
+    return data.__dict__[key]
 
 
 def get_available_languages() -> dict:
     return get_json_data(LANGS_JSON)
 
 
 def get_provider_alpha_code_type(provider: str) -> ProviderAlphaCodeData:
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/io_winreg.py` & `Subsearch-2.36.1/src/subsearch/utils/io_winreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         str: Path of the icon file to be used in the context menu, or an empty string if the configuration specifies
              that it should not be shown.
     """
     from subsearch.utils import io_json
 
     show_icon: str = io_json.get_json_key("context_menu_icon")
     if show_icon:
-        return str(app_paths.icon)
+        return str(app_paths.gui_assets / "subsearch.ico")
     else:
         return ""
 
 
 def get_appliesto_value() -> str:
     """
     Retrieve the latest json value from file `raw_json`.
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/log.py` & `Subsearch-2.36.1/src/subsearch/utils/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     Args:
         data: A dictionary containing the header and the data.
 
     Returns:
         None
     """
-    data = {
+    data: dict = {
         "User data": [
             {"Language": f"{language_data.name}, {language_data.alpha_1}, {language_data.alpha_2b}"},
             {"Use HI subtitle": app_config.hearing_impaired},
             {"Use non-HI subtitle": app_config.non_hearing_impaired},
             {"Match threshold": f"{app_config.percentage_threshold}%"},
             {"Use site subscene": app_config.providers["subscene_site"]},
             {"Use site opensubtitles": app_config.providers["opensubtitles_site"]},
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.36.1/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/string_parser.py` & `Subsearch-2.36.1/src/subsearch/utils/string_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,72 +32,72 @@
     """
     Find and return the title of a media file by year.
 
     Args:
         string (str): The file name.
 
     Returns:
-        str: The part of the file name before the year, with '.' replaced by ' ', or "N/A" if no match is found.
+        str: The part of the file name before the year, with '.' replaced by ' ', or "" if no match is found.
     """
     re_title = re.findall("^(.*)\.[1-2][0-9]{3}\.", string)
     if re_title:
         title: str = re_title[0]
         title = title.replace(".", " ")
         return title
-    return "N/A"
+    return ""
 
 
 def find_title_by_show(string: str) -> str:
     """
     Find and return the title of a media file by show.
 
     Args:
         string (str): The file name.
 
     Returns:
-        str: The part of the filename before the season and episode values, with '.' replaced by ' ', or "N/A" if no match is found.
+        str: The part of the filename before the season and episode values, with '.' replaced by ' ', or "" if no match is found.
     """
     re_title = re.findall("^(.*)\.[s]\d*[e]\d*\.", string)
     if re_title:
         title: str = re_title[0]
         title = title.replace(".", " ")
         return title
-    return "N/A"
+    return ""
 
 
 def find_season_episode(string: str) -> str:
     """
     Find and return the season and episode values of a media file.
 
     Args:
         string (str): The file name.
 
     Returns:
-        str: A string consisting of the season and episode values formatted like "s01e01", or "N/A" if no match is found.
+        str: A string consisting of the season and episode values formatted like "s01e01", or "" if no match is found.
     """
     re_se = re.findall("\.([s]\d*[e]\d*)\.", string)
     if re_se:
         se: str = re_se[0]
         return se
-    return "N/A"
+    return ""
 
 
 def convert_to_ordinal_string(string: str) -> tuple[str, str, str, str, bool]:
     """
     Converts the numeric TV series values (season and episode numbers) in a filename to their ordinal versions(if any).
 
     Args:
         string (str): The TV series values as pulled out from the filename as a single string, e.g., `s01e01`.
 
     Returns:
         tuple(str, str, str, str, bool): A tuple containing separated season and episode strings, corresponding ordinal
             strings, and a Boolean flag indicating whether the input string was matched successfully.
     """
-    if string == "N/A":
-        season, season_ordinal, episode, episode_ordinal = "N/A", "N/A", "N/A", "N/A"
+    if string == "":
+        season, season_ordinal, episode, episode_ordinal = "", "", "", ""
         show_bool = False
     else:
         season, episode = string.replace("s", "").replace("e", " ").split(" ")
         season_ordinal = num2words(int(season), lang="en", to="ordinal")
         episode_ordinal = num2words(int(episode), lang="en", to="ordinal")
         show_bool = True
     return season, season_ordinal, episode, episode_ordinal, show_bool
@@ -202,18 +202,18 @@
         """
         Gets the Url for the YifySubtitles website to search for subtitles for movies.
 
         Returns:
             str: The url to search for subtitles on yifysubtitles.org
         """
         if self.release_data.tvseries:
-            return "N/A"
+            return ""
         domain = "https://yifysubtitles.org"
         tt_id = imdb_lookup.FindImdbID(self.release_data.title, self.release_data.year).id
-        return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else "N/A"
+        return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else ""
 
     def _subscene_search_parameters(self) -> str:
         """
         Gets the search parameters for Subscene to search for the appropriate subtitles based on File name and season ordinal.
 
         Returns:
             str: The search parameter value for Subscene to search for the applicable subtitles.
```

### Comparing `Subsearch-2.36.0rc3/src/subsearch/utils/update.py` & `Subsearch-2.36.1/src/subsearch/utils/update.py`

 * *Files identical despite different names*

