# Comparing `tmp/ccmplots-0.1.2.tar.gz` & `tmp/ccmplots-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccmplots-0.1.2.tar", last modified: Mon May 29 09:38:12 2023, max compression
+gzip compressed data, was "ccmplots-0.1.3.tar", last modified: Sat Jul  8 16:55:04 2023, max compression
```

## Comparing `ccmplots-0.1.2.tar` & `ccmplots-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/
--rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.2/MANIFEST.in
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:38:12.383209 ccmplots-0.1.2/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)     1540 2023-05-29 08:40:44.000000 ccmplots-0.1.2/README.md
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/
--rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.2/ccmplots/__init__.py
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/styles/
--rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-05-29 08:20:50.000000 ccmplots-0.1.2/ccmplots/styles/ccm.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/styles/customization/
--rw-rw-r--   0 torben    (1000) torben    (1000)       85 2023-05-29 09:37:45.000000 ccmplots-0.1.2/ccmplots/styles/customization/large_font.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.2/ccmplots/styles/customization/no-latex.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.2/ccmplots/styles/customization/sans.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.2/ccmplots/styles/customization/square.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.2/ccmplots/styles/customization/tum4c.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots.egg-info/
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)      478 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/SOURCES.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/dependency_links.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/requires.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/top_level.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-05-29 09:38:02.000000 ccmplots-0.1.2/pyproject.toml
--rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-05-29 09:38:12.383209 ccmplots-0.1.2/setup.cfg
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-07-08 16:55:04.977344 ccmplots-0.1.3/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.3/MANIFEST.in
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-07-08 16:55:04.973344 ccmplots-0.1.3/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1728 2023-07-08 16:50:52.000000 ccmplots-0.1.3/README.md
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-07-08 16:55:04.973344 ccmplots-0.1.3/ccmplots/
+-rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.3/ccmplots/__init__.py
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-07-08 16:55:04.973344 ccmplots-0.1.3/ccmplots/styles/
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-07-08 16:47:19.000000 ccmplots-0.1.3/ccmplots/styles/ccm.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-07-08 16:55:04.973344 ccmplots-0.1.3/ccmplots/styles/customization/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       59 2023-07-08 16:49:20.000000 ccmplots-0.1.3/ccmplots/styles/customization/bw_palette.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       85 2023-05-29 09:37:45.000000 ccmplots-0.1.3/ccmplots/styles/customization/large_font.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.3/ccmplots/styles/customization/no-latex.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.3/ccmplots/styles/customization/sans.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.3/ccmplots/styles/customization/square.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.3/ccmplots/styles/customization/tum4c.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-07-08 16:55:04.973344 ccmplots-0.1.3/ccmplots.egg-info/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-07-08 16:55:04.000000 ccmplots-0.1.3/ccmplots.egg-info/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)      528 2023-07-08 16:55:04.000000 ccmplots-0.1.3/ccmplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-07-08 16:55:04.000000 ccmplots-0.1.3/ccmplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-07-08 16:55:04.000000 ccmplots-0.1.3/ccmplots.egg-info/requires.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-07-08 16:55:04.000000 ccmplots-0.1.3/ccmplots.egg-info/top_level.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-07-08 16:51:36.000000 ccmplots-0.1.3/pyproject.toml
+-rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-07-08 16:55:04.977344 ccmplots-0.1.3/setup.cfg
```

### Comparing `ccmplots-0.1.2/README.md` & `ccmplots-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 plt.show()
 ```
 
 The code above produces the following figure which has the default aspect ratio of 6/5. The width of the base style "ccm" is 3.5 inches which corresponds to approx 89 mm. 
 
 ![image](examples/simple.svg "Simple figure")
 
-The width of a column in the base style "ccm" can be combined with other styles such as "square" or "sans". Furthermore, the color cycler can be modified. Currently, there is only one additional pre-defined color cycle available which is called "tum4c" and comprises the 4 main TUM colors.
+The width of a column in the base style "ccm" can be combined with other styles such as "square" or "sans". Furthermore, the color cycler can be modified. Currently, there is only one additional pre-defined color cycle available which is called "tum4c" and comprises the 4 main TUM colors. The default font size is 8 (this is the font size in Elsevier articles). If the font size should be increase to 11 (to match manuscript text size) "large_font" can be added.
 
 ```python
-plt.style.use(["ccm","sans","square","tum4c"])
+plt.style.use(["ccm", "square", "bw_palette", "large_font"])
 
 ```
 ![image](examples/simple_sans.svg "Simple figure")
 
 
 Among other things, the examples folder contains the python code to create the following figure:
```

### Comparing `ccmplots-0.1.2/ccmplots/__init__.py` & `ccmplots-0.1.3/ccmplots/__init__.py`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.2/ccmplots/styles/ccm.mplstyle` & `ccmplots-0.1.3/ccmplots/styles/ccm.mplstyle`

 * *Files identical despite different names*

