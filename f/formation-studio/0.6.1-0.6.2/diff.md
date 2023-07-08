# Comparing `tmp/formation-studio-0.6.1.tar.gz` & `tmp/formation-studio-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formation-studio-0.6.1.tar", last modified: Wed Jun  7 11:04:15 2023, max compression
+gzip compressed data, was "formation-studio-0.6.2.tar", last modified: Sat Jul  8 12:00:12 2023, max compression
```

## Comparing `formation-studio-0.6.1.tar` & `formation-studio-0.6.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.677651 formation-studio-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 11:03:54.000000 formation-studio-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 11:03:54.000000 formation-studio-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-07 11:04:15.677651 formation-studio-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-07 11:03:54.000000 formation-studio-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/formats/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/meth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.649651 formation-studio-0.6.1/formation_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.649651 formation-studio-0.6.1/hoverset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.657651 formation-studio-0.6.1/hoverset/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.bak
--rw-r--r--   0 runner    (1001) docker     (123)  6268365 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.dir
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/keymap.py
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.657651 formation-studio-0.6.1/hoverset/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/platform/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/color.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/pickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/ui/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/themes/light.css
--rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/util/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 11:03:54.000000 formation-studio-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 11:03:54.000000 formation-studio-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:04:15.677651 formation-studio-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.665651 formation-studio-0.6.1/studio/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.665651 formation-studio-0.6.1/studio/debugtools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/element_pane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/style_pane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.669651 formation-studio-0.6.1/studio/feature/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/component_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    35484 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/design.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/eventspane.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/stylepane.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/variablepane.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    35873 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    38284 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/parsers/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.641651 formation-studio-0.6.1/studio/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   225382 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation.ico
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation.png
--rw-r--r--   0 runner    (1001) docker     (123)   218818 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/menus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.677651 formation-studio-0.6.1/studio/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/editors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.548840 formation-studio-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 11:59:51.000000 formation-studio-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-08 11:59:51.000000 formation-studio-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-07-08 12:00:12.548840 formation-studio-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-07-08 11:59:51.000000 formation-studio-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.528840 formation-studio-0.6.2/formation/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.528840 formation-studio-0.6.2/formation/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/formats/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/formats/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/formats/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.528840 formation-studio-0.6.2/formation/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/handlers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/handlers/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/handlers/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/handlers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/meth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-08 11:59:51.000000 formation-studio-0.6.2/formation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.528840 formation-studio-0.6.2/formation_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 12:00:12.000000 formation-studio-0.6.2/formation_studio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.528840 formation-studio-0.6.2/hoverset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.536840 formation-studio-0.6.2/hoverset/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/image.bak
+-rw-r--r--   0 runner    (1001) docker     (123)  6268365 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/image.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/image.dir
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.536840 formation-studio-0.6.2/hoverset/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/platform/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.540840 formation-studio-0.6.2/hoverset/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/color.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.540840 formation-studio-0.6.2/hoverset/ui/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/themes/light.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/ui/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.540840 formation-studio-0.6.2/hoverset/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/util/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/util/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-08 11:59:51.000000 formation-studio-0.6.2/hoverset/util/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-08 11:59:51.000000 formation-studio-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 11:59:51.000000 formation-studio-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:00:12.548840 formation-studio-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.540840 formation-studio-0.6.2/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.540840 formation-studio-0.6.2/studio/debugtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/element_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/debugtools/style_pane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.544840 formation-studio-0.6.2/studio/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/component_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35423 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/eventspane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/stylepane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/feature/variablepane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.544840 formation-studio-0.6.2/studio/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35873 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/lib/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38274 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.544840 formation-studio-0.6.2/studio/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/parsers/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.524839 formation-studio-0.6.2/studio/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.544840 formation-studio-0.6.2/studio/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   225382 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/resources/images/formation.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/resources/images/formation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   218818 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/resources/images/formation_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/resources/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.548840 formation-studio-0.6.2/studio/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/tools/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/tools/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/tools/menus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:00:12.548840 formation-studio-0.6.2/studio/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/editors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-08 11:59:51.000000 formation-studio-0.6.2/studio/updates.py
```

### Comparing `formation-studio-0.6.1/LICENSE.txt` & `formation-studio-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/PKG-INFO` & `formation-studio-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.1/README.md` & `formation-studio-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/formats/__init__.py` & `formation-studio-0.6.2/formation/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/formats/_base.py` & `formation-studio-0.6.2/formation/formats/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/formats/_json.py` & `formation-studio-0.6.2/formation/formats/_json.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/formats/_xml.py` & `formation-studio-0.6.2/formation/formats/_xml.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/handlers/__init__.py` & `formation-studio-0.6.2/formation/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/handlers/command.py` & `formation-studio-0.6.2/formation/handlers/command.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/handlers/image.py` & `formation-studio-0.6.2/formation/handlers/image.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/handlers/layout.py` & `formation-studio-0.6.2/formation/handlers/layout.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/handlers/misc.py` & `formation-studio-0.6.2/formation/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/loader.py` & `formation-studio-0.6.2/formation/loader.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/meth.py` & `formation-studio-0.6.2/formation/meth.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/preprocessors.py` & `formation-studio-0.6.2/formation/preprocessors.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation/utils.py` & `formation-studio-0.6.2/formation/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/formation_studio.egg-info/PKG-INFO` & `formation-studio-0.6.2/formation_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.1/formation_studio.egg-info/SOURCES.txt` & `formation-studio-0.6.2/formation_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/actions.py` & `formation-studio-0.6.2/hoverset/data/actions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/image.bak` & `formation-studio-0.6.2/hoverset/data/image.bak`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/image.dat` & `formation-studio-0.6.2/hoverset/data/image.dat`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/image.dir` & `formation-studio-0.6.2/hoverset/data/image.dir`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/images.py` & `formation-studio-0.6.2/hoverset/data/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     if image is None:
         raise FileNotFoundError(
             "Incorrect image shelve path specified, use set_image_resource_path function to set the correct path!"
         )
     # Resize the image to required size
     if color:
         image = _recolor(image, color)
-    image.thumbnail((width, height), Image.ANTIALIAS)
+    image.thumbnail((width, height), Image.LANCZOS)
     return image
 
 
 def get_tk_image(identifier: str, width=25, height=25, **kwargs):
     """
     Fetch a tkinter compatible image from the image database.
     It's a wrapper around the get_image function
```

### Comparing `formation-studio-0.6.1/hoverset/data/keymap.py` & `formation-studio-0.6.2/hoverset/data/keymap.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/preferences.py` & `formation-studio-0.6.2/hoverset/data/preferences.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/data/utils.py` & `formation-studio-0.6.2/hoverset/data/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/platform/__init__.py` & `formation-studio-0.6.2/hoverset/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/platform/functions.py` & `formation-studio-0.6.2/hoverset/platform/functions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/animation.py` & `formation-studio-0.6.2/hoverset/ui/animation.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/color.tcl` & `formation-studio-0.6.2/hoverset/ui/color.tcl`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/dialogs.py` & `formation-studio-0.6.2/hoverset/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/loaders.py` & `formation-studio-0.6.2/hoverset/ui/loaders.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/menu.py` & `formation-studio-0.6.2/hoverset/ui/menu.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/panels.py` & `formation-studio-0.6.2/hoverset/ui/panels.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/pickers.py` & `formation-studio-0.6.2/hoverset/ui/pickers.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/styles.py` & `formation-studio-0.6.2/hoverset/ui/styles.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/themes/default.css` & `formation-studio-0.6.2/hoverset/ui/themes/default.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/themes/light.css` & `formation-studio-0.6.2/hoverset/ui/themes/light.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/widgets.py` & `formation-studio-0.6.2/hoverset/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/ui/windows.py` & `formation-studio-0.6.2/hoverset/ui/windows.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/util/__init__.py` & `formation-studio-0.6.2/hoverset/util/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/util/color.py` & `formation-studio-0.6.2/hoverset/util/color.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/util/execution.py` & `formation-studio-0.6.2/hoverset/util/execution.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/hoverset/util/validators.py` & `formation-studio-0.6.2/hoverset/util/validators.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/pyproject.toml` & `formation-studio-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/cli.py` & `formation-studio-0.6.2/studio/cli.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/context.py` & `formation-studio-0.6.2/studio/context.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/debugtools/common.py` & `formation-studio-0.6.2/studio/debugtools/common.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/debugtools/debugger.py` & `formation-studio-0.6.2/studio/debugtools/debugger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # ======================================================================= #
 # Copyright (C) 2022 Hoverset Group.                                      #
 # ======================================================================= #
 
+_global_freeze = dict(globals())
+
 import sys
 import tkinter
 import logging
 import subprocess
 
 from hoverset.data.images import load_tk_image
 from hoverset.data.utils import get_resource_path
@@ -15,14 +17,16 @@
 from studio.debugtools.preferences import Preferences
 from studio.debugtools.element_pane import ElementPane
 from studio.debugtools.style_pane import StylePane
 
 from studio.resource_loader import ResourceLoader
 import studio
 
+from tkinterDnD.tk import _init_tkdnd
+
 logger = logging.getLogger("Debugger")
 
 
 class Elements(PanedWindow):
 
     def __init__(self, master, debugger):
         super().__init__(master)
@@ -40,14 +44,15 @@
 class Debugger(Window):
     _instance = None
 
     def __init__(self, master):
         self.pref = Preferences.acquire()
         Application.load_styles(self, self.pref.get("resource::theme"))
         super(Window, self).__init__(master)
+        _init_tkdnd(self)
         self.geometry(self.pref.get("debugger::geometry"))
         self.set_up_mousewheel()
         Debugger._instance = self
         self.master = self.root = self.position_ref = master
         self.setup_window()
         self.set_up_mousewheel()
         self.wm_transient(master)
@@ -190,15 +195,18 @@
             else:
                 logger.error("No python file supplied")
                 return
         ResourceLoader.load(Preferences.acquire())
         cls._hook()
         with open(path) as file:
             code = compile(file.read(), path, 'exec')
-        exec(code, {'__name__': '__main__'})
+
+        # Ensure hooked application thinks it is running as __main__
+        _global_freeze.update({"__name__": "__main__", "__file__": path})
+        exec(code, _global_freeze)
 
     @classmethod
     def run_process(cls, path) -> subprocess.Popen:
         return subprocess.Popen(["formation-dbg", path])
 
 
 def main():
```

### Comparing `formation-studio-0.6.1/studio/debugtools/element_pane.py` & `formation-studio-0.6.2/studio/debugtools/element_pane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/debugtools/layouts.py` & `formation-studio-0.6.2/studio/debugtools/layouts.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/debugtools/style_pane.py` & `formation-studio-0.6.2/studio/debugtools/style_pane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/_base.py` & `formation-studio-0.6.2/studio/feature/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/component_tree.py` & `formation-studio-0.6.2/studio/feature/component_tree.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/components.py` & `formation-studio-0.6.2/studio/feature/components.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/design.py` & `formation-studio-0.6.2/studio/feature/design.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     def _open_default(self):
         self.update_idletasks()
         from studio.lib import legacy
         width = max(self.width - self._padding * 2, 300)
         height = max(self.height - self._padding * 2, 300)
         self.add(
-            legacy.Toplevel, self._padding, self._padding,
+            legacy.Tk, self._padding, self._padding,
             width=width, height=height
         )
         self.builder.generate()
         self.design_path = None
 
     @property
     def _ids(self):
@@ -464,22 +464,21 @@
         if obj_class.group != Groups.container and self.root_obj is None:
             # We only need a container as the root widget
             self._show_root_widget_warning()
             return
         silent = kwargs.get("silently", False)
         name = self._get_unique(obj_class)
         obj = obj_class(self, name)
-        if hasattr(obj, 'initial_dimensions'):
-            width, height = obj.initial_dimensions
-        else:
-            width = kwargs.get(
-                "width",
-                self._base_font.measure(name) + self.WIDGET_INIT_PADDING
-            )
-            height = kwargs.get("height", self.WIDGET_INIT_HEIGHT)
+        width, height = getattr(obj, "initial_dimensions", (
+            self._base_font.measure(name) + self.WIDGET_INIT_PADDING,
+            self.WIDGET_INIT_HEIGHT
+        ))
+        width = kwargs.get("width", width)
+        height = kwargs.get("height", height)
+
         obj.layout = kwargs.get("intended_layout", None)
         self._attach(obj)  # apply extra bindings required
         # If the object has a layout which actually the layout at the point of creation prepare and pass it
         # to the layout
         if isinstance(layout, Container):
             bounds = (x, y, x + width, y + height)
             bounds = geometry.resolve_bounds(bounds, self)
```

### Comparing `formation-studio-0.6.1/studio/feature/eventspane.py` & `formation-studio-0.6.2/studio/feature/eventspane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/stylepane.py` & `formation-studio-0.6.2/studio/feature/stylepane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/feature/variablepane.py` & `formation-studio-0.6.2/studio/feature/variablepane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/__init__.py` & `formation-studio-0.6.2/studio/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/canvas.py` & `formation-studio-0.6.2/studio/lib/canvas.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/layouts.py` & `formation-studio-0.6.2/studio/lib/layouts.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/legacy.py` & `formation-studio-0.6.2/studio/lib/legacy.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/menu.py` & `formation-studio-0.6.2/studio/lib/menu.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/native.py` & `formation-studio-0.6.2/studio/lib/native.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/properties.py` & `formation-studio-0.6.2/studio/lib/properties.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/pseudo.py` & `formation-studio-0.6.2/studio/lib/pseudo.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/lib/toplevel.py` & `formation-studio-0.6.2/studio/lib/toplevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
 
     setattr(menu, "add", _add_hook)
     setattr(menu, "delete", _delete_hook)
     setattr(menu, "_clear_hooks", _clear_hooks)
 
 
 class _Toplevel(tk.Frame):
-    impl = tk.Toplevel
     _images = None
 
     def __init__(self, master, id_):
         super().__init__(master)
         self.id = id_
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(1, weight=1)
@@ -448,15 +447,17 @@
 
 class Toplevel(ToplevelContainer, _Toplevel):
     group = Groups.container
     icon = 'window'
     is_toplevel = True
     display_name = 'Toplevel'
     impl = tk.Toplevel
+    initial_dimensions = 200, 230
 
 
 class Tk(ToplevelContainer, _Toplevel):
     group = Groups.container
     icon = 'window'
     is_toplevel = True
     display_name = 'Tk'
     impl = tk.Tk
+    initial_dimensions = 200, 230
```

### Comparing `formation-studio-0.6.1/studio/lib/variables.py` & `formation-studio-0.6.2/studio/lib/variables.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/main.py` & `formation-studio-0.6.2/studio/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import functools
 import os
 import sys
 import time
 import tkinter
 import webbrowser
-from tkinter import filedialog, Toplevel
+from tkinter import filedialog
 
 import tkinterDnD
 
 from studio.feature.design import DesignContext, MultiSaveDialog
 from studio.feature import FEATURES, StylePane
 from studio.feature._base import BaseFeature, FeaturePane
 from studio.tools import ToolManager
```

### Comparing `formation-studio-0.6.1/studio/parsers/loader.py` & `formation-studio-0.6.2/studio/parsers/loader.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/preferences.py` & `formation-studio-0.6.2/studio/preferences.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/resource_loader.py` & `formation-studio-0.6.2/studio/resource_loader.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/resources/images/formation.ico` & `formation-studio-0.6.2/studio/resources/images/formation.ico`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/resources/images/formation.png` & `formation-studio-0.6.2/studio/resources/images/formation.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/resources/images/formation_icon.png` & `formation-studio-0.6.2/studio/resources/images/formation_icon.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/resources/images/logo.png` & `formation-studio-0.6.2/studio/resources/images/logo.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/tools/__init__.py` & `formation-studio-0.6.2/studio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/tools/_base.py` & `formation-studio-0.6.2/studio/tools/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/tools/canvas.py` & `formation-studio-0.6.2/studio/tools/canvas.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/tools/menus.py` & `formation-studio-0.6.2/studio/tools/menus.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/about.py` & `formation-studio-0.6.2/studio/ui/about.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/editors.py` & `formation-studio-0.6.2/studio/ui/editors.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/geometry.py` & `formation-studio-0.6.2/studio/ui/geometry.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/highlight.py` & `formation-studio-0.6.2/studio/ui/highlight.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/tree.py` & `formation-studio-0.6.2/studio/ui/tree.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/ui/widgets.py` & `formation-studio-0.6.2/studio/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.1/studio/updates.py` & `formation-studio-0.6.2/studio/updates.py`

 * *Files identical despite different names*

