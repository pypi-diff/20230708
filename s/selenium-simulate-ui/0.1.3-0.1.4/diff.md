# Comparing `tmp/selenium_simulate_ui-0.1.3.tar.gz` & `tmp/selenium_simulate_ui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_simulate_ui-0.1.3.tar", last modified: Sat Jul  8 10:32:30 2023, max compression
+gzip compressed data, was "selenium_simulate_ui-0.1.4.tar", last modified: Sat Jul  8 10:45:54 2023, max compression
```

## Comparing `selenium_simulate_ui-0.1.3.tar` & `selenium_simulate_ui-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:32:30.953554 selenium_simulate_ui-0.1.3/
--rw-rw-rw-   0        0        0    11357 2023-07-08 07:33:00.000000 selenium_simulate_ui-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      261 2023-07-08 10:32:30.917121 selenium_simulate_ui-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 07:33:00.000000 selenium_simulate_ui-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 10:32:30.916123 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-08 10:32:30.000000 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-07-08 10:32:30.000000 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:32:30.000000 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 10:32:30.000000 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:32:30.000000 selenium_simulate_ui-0.1.3/selenium_simulate_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 10:32:30.953554 selenium_simulate_ui-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-07-08 10:32:14.000000 selenium_simulate_ui-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:45:54.049906 selenium_simulate_ui-0.1.4/
+-rw-rw-rw-   0        0        0    11357 2023-07-08 07:33:00.000000 selenium_simulate_ui-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-07-08 10:45:54.048868 selenium_simulate_ui-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 07:33:00.000000 selenium_simulate_ui-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 10:45:54.046872 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-07-08 10:45:53.000000 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-08 10:45:53.000000 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:45:53.000000 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 10:45:53.000000 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:45:53.000000 selenium_simulate_ui-0.1.4/selenium_simulate_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:45:54.049906 selenium_simulate_ui-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      450 2023-07-08 10:45:47.000000 selenium_simulate_ui-0.1.4/setup.py
```

### Comparing `selenium_simulate_ui-0.1.3/LICENSE` & `selenium_simulate_ui-0.1.4/LICENSE`

 * *Files identical despite different names*

