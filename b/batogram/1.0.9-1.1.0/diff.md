# Comparing `tmp/batogram-1.0.9.tar.gz` & `tmp/batogram-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batogram-1.0.9.tar", last modified: Sun Jun  4 17:50:27 2023, max compression
+gzip compressed data, was "batogram-1.1.0.tar", last modified: Sat Jul  8 19:31:18 2023, max compression
```

## Comparing `batogram-1.0.9.tar` & `batogram-1.1.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.974586 batogram-1.0.9/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.9/LICENSE
--rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.9/MANIFEST.in
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:50:27.974586 batogram-1.0.9/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4611 2023-06-04 17:11:53.000000 batogram-1.0.9/README.md
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.920585 batogram-1.0.9/batogram/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-06-04 17:50:01.000000 batogram-1.0.9/batogram/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/__main__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/about.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4673 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/amplitudegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/appsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/appsettingsmodal.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.931585 batogram-1.0.9/batogram/assets/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/3669170_home_ic_icon.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-left-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-left-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-right-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-right-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/batogram.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/download-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/drag-move-2-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/expand-left-right-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/expand-up-down-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/fullscreen-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/home-4-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/zoom-in-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7549 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/audiofileservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/breadcrumbservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/buttonframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/chunky_spectrogram.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.954586 batogram-1.0.9/batogram/colour_maps/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L01.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L03.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L05.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L06.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L07.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L08.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L09.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L16.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L17.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L18.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L19.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L20.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/black-body-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/inferno-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colourmap.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1658 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/common.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1817 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/constants.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.964586 batogram-1.0.9/batogram/external/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/guano.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/tooltip.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/fileinfoframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2968 2023-05-17 18:30:45.000000 batogram-1.0.9/batogram/frames.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5588 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/graphsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/historianservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    31653 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/layouts.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    31047 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/markers.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/modalwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/morebncframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12440 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/moreframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/morerenderingframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6851 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/morescaleframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4635 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/profilegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/readoutframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/rendering.py
--rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35201 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/rootwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/runner.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.973586 batogram-1.0.9/batogram/samples/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/samples/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    21200 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/spectrogramgraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    16042 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/spectrogrammouseservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    17007 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/validatingwidgets.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/wavfileparser.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.924585 batogram-1.0.9/batogram.egg-info/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2282 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/SOURCES.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/dependency_links.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/entry_points.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/requires.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/top_level.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-06-04 17:49:38.000000 batogram-1.0.9/pyproject.toml
--rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-06-04 17:50:27.974586 batogram-1.0.9/setup.cfg
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.826130 batogram-1.1.0/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.1.0/LICENSE
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.1.0/MANIFEST.in
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6612 2023-07-08 19:31:18.825130 batogram-1.1.0/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4665 2023-07-08 18:52:21.000000 batogram-1.1.0/README.md
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.762129 batogram-1.1.0/batogram/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-07-08 19:30:38.000000 batogram-1.1.0/batogram/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/__main__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/about.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4673 2023-06-11 17:57:11.000000 batogram-1.1.0/batogram/amplitudegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7302 2023-06-11 18:04:31.000000 batogram-1.1.0/batogram/appsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/appsettingsmodal.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.784129 batogram-1.1.0/batogram/assets/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/3669170_home_ic_icon.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/arrow-left-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/arrow-left-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/arrow-right-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/arrow-right-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/batogram.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/download-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/drag-move-2-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/expand-left-right-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/expand-up-down-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/fullscreen-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/home-4-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/assets/zoom-in-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7567 2023-06-12 15:59:34.000000 batogram-1.1.0/batogram/audiofileservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/breadcrumbservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/buttonframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5264 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/chunky_spectrogram.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.816130 batogram-1.1.0/batogram/colour_maps/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L01.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L03.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L05.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L06.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L07.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L08.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L09.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L16.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L17.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L18.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L19.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/CET-L20.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/black-body-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/inferno-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colour_maps/kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/colourmap.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1658 2023-06-04 16:54:05.000000 batogram-1.1.0/batogram/common.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1817 2023-06-04 16:54:05.000000 batogram-1.1.0/batogram/constants.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.818130 batogram-1.1.0/batogram/external/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/external/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19293 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/external/guano.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/external/tooltip.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2155 2023-06-15 14:49:16.000000 batogram-1.1.0/batogram/fileinfoframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2968 2023-05-17 18:30:45.000000 batogram-1.1.0/batogram/frames.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6668 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/graphsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/historianservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    31679 2023-06-11 17:57:47.000000 batogram-1.1.0/batogram/layouts.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    32723 2023-06-15 15:38:39.000000 batogram-1.1.0/batogram/markers.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2224 2023-06-11 18:05:29.000000 batogram-1.1.0/batogram/modalwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    28228 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/morebncframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    12710 2023-06-15 13:47:21.000000 batogram-1.1.0/batogram/moreframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4653 2023-06-12 15:50:28.000000 batogram-1.1.0/batogram/moreotherframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6733 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/morerenderingframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6859 2023-06-12 14:18:33.000000 batogram-1.1.0/batogram/morescaleframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4635 2023-06-11 17:57:11.000000 batogram-1.1.0/batogram/profilegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3924 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/readoutframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    71391 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/rendering.py
+-rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35540 2023-06-15 14:47:58.000000 batogram-1.1.0/batogram/rootwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1583 2023-06-11 18:06:10.000000 batogram-1.1.0/batogram/runner.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.825130 batogram-1.1.0/batogram/samples/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.1.0/batogram/samples/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29321 2023-06-11 17:57:47.000000 batogram-1.1.0/batogram/spectrogramgraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    17244 2023-06-11 17:57:47.000000 batogram-1.1.0/batogram/spectrogrammouseservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    18010 2023-07-03 08:37:34.000000 batogram-1.1.0/batogram/validatingwidgets.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    14843 2023-07-08 18:40:41.000000 batogram-1.1.0/batogram/wavfileparser.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-07-08 19:31:18.775129 batogram-1.1.0/batogram.egg-info/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6612 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2309 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/SOURCES.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/dependency_links.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/entry_points.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/requires.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-07-08 19:31:18.000000 batogram-1.1.0/batogram.egg-info/top_level.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-07-08 19:30:23.000000 batogram-1.1.0/pyproject.toml
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-07-08 19:31:18.826130 batogram-1.1.0/setup.cfg
```

### Comparing `batogram-1.0.9/LICENSE` & `batogram-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/PKG-INFO` & `batogram-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.9
+Version: 1.1.0
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,16 +46,17 @@
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
 * Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
 * Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
+* Support for reassignment spectrograms for increased resolution.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, Linux and macOS (experimental) operating systems.
+* Runs on Windows, Linux operating systems, maybe macOS.
 
 Installation
 ------------
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
```

### Comparing `batogram-1.0.9/README.md` & `batogram-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
 * Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
 * Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
+* Support for reassignment spectrograms for increased resolution.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, Linux and macOS (experimental) operating systems.
+* Runs on Windows, Linux operating systems, maybe macOS.
 
 Installation
 ------------
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
```

### Comparing `batogram-1.0.9/batogram/__main__.py` & `batogram-1.1.0/batogram/__main__.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/about.py` & `batogram-1.1.0/batogram/about.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/amplitudegraphframe.py` & `batogram-1.1.0/batogram/amplitudegraphframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/appsettings.py` & `batogram-1.1.0/batogram/appsettings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# Copyright (c) 2023 John Mears
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import os
 from typing import Tuple, Optional
 
 import numpy as np
 
 from dataclasses import dataclass
 from pathlib import Path
```

### Comparing `batogram-1.0.9/batogram/appsettingsmodal.py` & `batogram-1.1.0/batogram/appsettingsmodal.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/assets/batogram.png` & `batogram-1.1.0/batogram/assets/batogram.png`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/audiofileservice.py` & `batogram-1.1.0/batogram/audiofileservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,23 +110,23 @@
         # The data seems sane, so go ahead and try to use it:
 
         # See if there is a sample rate in the GUANO. If there is, use it, because the
         # header sometimes reflects data stored in TE form:
         guano_key = 'Samplerate'
         if guanodata is not None and guano_key in guanodata:
             self._sample_rate = guanodata[guano_key]
-
-        self._sample_rate = sample_rate
+        else:
+            self._sample_rate = sample_rate
         self._sample_count = sample_count
         self._time_range = AxisRange(0, sample_count / self._sample_rate)
         self._frequency_range = AxisRange(0, self._sample_rate / 2.0)
         self._channels = channels
         self._bytes_per_value = int(chunks.header.bits_per_sample / 8)
 
-        # Force the amplitude range to be symmetrical:
+        # Force the amplitude range to be symmetrical:z
         abs_a_max = max(-data.data_range[0], data.data_range[1])
         self._amplitude_range = AxisRange(-abs_a_max, abs_a_max)
 
         # Construct a string that can be used to know if a new (or the same) file has been loaded:
         self._data_serial = "{}:{}".format(self._filepath, time.time())
 
         # Prepare some metadata that will be used for the UI:
```

### Comparing `batogram-1.0.9/batogram/breadcrumbservice.py` & `batogram-1.1.0/batogram/breadcrumbservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/buttonframe.py` & `batogram-1.1.0/batogram/buttonframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/chunky_spectrogram.py` & `batogram-1.1.0/batogram/chunky_spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import numpy as np
 
 from scipy.signal import spectrogram
 # from timeit import default_timer as timer
 
 
-def chunky_spectrogram(*args, **kwargs):
+def chunky_spectrogram(dtype, *args, **kwargs):
     """Scipy's spectrogram calculations uses quite a lot of memory. One reason is because creates *all* the
     segments that will be FFTed, which results in duplication of data depending on the overlap, then
     FFTs as a next step on all of them - rather than pipelining.
 
     We can manage memory usage by feeding scipy *chunks* of data, which we can concatenate afterwards."""
 
     # Split the input in chunks which overlap by half the window size.
@@ -83,15 +83,15 @@
         # t2 = timer()
         # print("Spectrogram: {}".format(t2 - t1))
         new_segments = len(times)
 
         if first_segment:
             all_freqs = freqs    # Note the frequencies from the first response. Subsequent ones are the same.
             all_times = np.zeros(total_segments, dtype=np.single)       # dtype is important for memory conservation.
-            all_spectra = np.zeros((len(freqs), total_segments), dtype=np.single)
+            all_spectra = np.zeros((len(freqs), total_segments), dtype=dtype)  # Complex data
             segments_to_skip = 0
             previous_time = 0
         else:
             # Other than the first time around, we discard the initial data point
             # as it duplicates the last point of the previous chunk.
             segments_to_skip = 1
```

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L01.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L01.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L03.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L03.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L05.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L05.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L06.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L06.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L07.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L07.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L08.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L08.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L09.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L09.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L16.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L16.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L17.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L17.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L18.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L18.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L19.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L19.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/CET-L20.csv` & `batogram-1.1.0/batogram/colour_maps/CET-L20.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/black-body-table-byte-1024.csv` & `batogram-1.1.0/batogram/colour_maps/black-body-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv` & `batogram-1.1.0/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/inferno-table-byte-1024.csv` & `batogram-1.1.0/batogram/colour_maps/inferno-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colour_maps/kindlmann-table-byte-1024.csv` & `batogram-1.1.0/batogram/colour_maps/kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/colourmap.py` & `batogram-1.1.0/batogram/colourmap.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/common.py` & `batogram-1.1.0/batogram/common.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/constants.py` & `batogram-1.1.0/batogram/constants.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/external/guano.py` & `batogram-1.1.0/batogram/external/guano.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     :ivar bytes wav_data:  the `data` subchunk of a .WAV file consisting of its actual audio data,
                            lazily-loaded and cached for performance
     :ivar wavparams wav_params:  namedtuple of .WAV parameters (nchannels, sampwidth, framerate, nframes, comptype, compname)
     """
 
     _coersion_rules = {
         'Filter HP': float, 'Length': float, 'Loc Elevation': float,
-        'Loc Accuracy': int, 'Samplerate': int,
+        'Loc Accuracy': float, 'Samplerate': int,
         'TE': lambda value: int(value) if value else 1,
         'Loc Position': lambda value: tuple(float(v) for v in value.split()),
         'Timestamp': parse_timestamp,
         'Note': lambda value: value.replace('\\n', '\n'),
     }
     _serialization_rules = {
         'Loc Position': lambda value: '%f %f' % value,
```

### Comparing `batogram-1.0.9/batogram/external/tooltip.py` & `batogram-1.1.0/batogram/external/tooltip.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/fileinfoframe.py` & `batogram-1.1.0/batogram/fileinfoframe.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,32 +16,36 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 from .frames import DrawableFrame
+from .rendering import SpectrogramPipeline, GraphParams
 
 
 class FileInfoFrame(DrawableFrame):
     """A Frame that contains a short summary of info relating to the data file being
     displayed."""
 
-    def __init__(self, parent, data_context):
+    def __init__(self, parent, data_context: "DataContext"):
         super().__init__(parent)
         self._dc = data_context
 
         self._label = tk.Label(self, text="", width=1, anchor=tk.CENTER)
         self._label.grid(row=0, column=0, sticky="nsew")
         self.columnconfigure(0, weight=1)
 
     def draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
         super().draw(draw_scope)
+        text = ""
         a = self._dc.afs
         if a is not None:
             md = a.get_metadata()
-            channel_text = "channels" if md.channels > 1 else "channel"
-            text = "{}: {:.1f} s at {:.1f} kHz, {} {}".format(
-                md.file_name, md.length_seconds,  md.sample_rate / 1000.0, md.channels, channel_text)
-        else:
-            text = ""
+            if md.channels == 1:
+                c = "1 channel"
+            else:
+                c = "{} channels".format(md.channels)
+            text = "{}: {:.1f} s at {:.1f} kHz, {}".format(
+                md.file_name, md.length_seconds,  md.sample_rate / 1000.0, c)
+
         self._label.config(text=text)
```

### Comparing `batogram-1.0.9/batogram/frames.py` & `batogram-1.1.0/batogram/frames.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/graphsettings.py` & `batogram-1.1.0/batogram/graphsettings.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,66 +47,89 @@
 
 INTERPOLATION_OPTIONS = {0: "None", 1: "Linear", 2: "Quadratic", 3: "Cubic"}
 DEFAULT_INTERPOLATION = 2       # Linear is fairly smooth and fairly fast,
                                 # and avoids edge artifacts that quadratic generates.
 
 # Note: boxcar window blows up in the calculations involving infinity
 WINDOW_TYPE_OPTIONS = {"hann": "Hann", "hamming": "Hamming", "blackman": "Blackman", "tukey": "Tukey 0.5",
-                       "bartlett": "Bartlett", "flattop": "Flat top"}
+                       "bartlett": "Bartlett", "flattop": "Flat top", "boxcar": "Rectangular"}
+                        # ("kaiser", 3): "Kaiser" is recommended in a paper but results in lots of spread.
 DEFAULT_WINDOW_TYPE = "hann"
 
+SPECTROGRAM_TYPE_STANDARD = 0
+SPECTROGRAM_TYPE_REASSIGNMENT = 1
+SPECTROGRAM_TYPE_ADAPTIVE = 2
+SPECTROGRAM_TYPE_OPTIONS = {SPECTROGRAM_TYPE_STANDARD: "Standard",
+                            SPECTROGRAM_TYPE_REASSIGNMENT: "Reassignment",
+                            SPECTROGRAM_TYPE_ADAPTIVE: "Auto based on zoom"}
+DEFAULT_SPECTROGRAM_TYPE = SPECTROGRAM_TYPE_STANDARD
+
+DEFAULT_FFT_WINDOW_PADDING_FACTOR = 1
+FFT_WINDOW_PADDING_FACTOR = {DEFAULT_FFT_WINDOW_PADDING_FACTOR: "1", 2: "2", 4: "4", 8: "8"}
+
 BNC_ADAPTIVE_MODE = 0
 BNC_MANUAL_MODE = 1
 BNC_INTERACTIVE_MODE = 2
-BNC_MODES = {BNC_ADAPTIVE_MODE: "Auto", BNC_MANUAL_MODE: "Manual", BNC_INTERACTIVE_MODE: "Interactive"}
+
+MULTICHANNEL_COMBINED_MODE = 0
+# MULTICHANNEL_STEREO_MODE = 1
+MULTICHANNEL_SINGLE_MODE = 2
 
 
 @dataclass
 class GraphSettings:
     """Settings relating to a specific graph panel."""
     time_range: Optional[AxisRange]
     zero_based_time: bool
     frequency_range: Optional[AxisRange]
     show_grid: bool
     show_profile: bool
-    fft_samples: int
-    fft_overlap: int
+    window_samples: int
+    window_overlap: int
     window_type: str
+    window_padding_factor: int
     zoom_interpolation: int
     colour_mapping_path: str
     colour_mapping_steps: int
     do_histogram_normalization: bool
     bnc_adjust_type: int
     bnc_background_threshold_percent: float
     bnc_manual_min: float  # bnc manual min and max are percentages of the data range.
     bnc_manual_max: float
     show_time_markers: bool
     show_frequency_markers: bool
+    multichannel_mode: int
+    multichannel_channel: int
+    spectrogram_type: int
 
     def __init__(self,
                  on_app_modified_settings: Callable[[int], NoReturn],
                  on_user_applied_settings: Callable[[int], NoReturn],
                  show_profile=True):
         self.time_range = AxisRange(0, 1)
         self.zero_based_time = True
         self.frequency_range = AxisRange(0, 1)
         self._on_app_modified_settings: Callable[[int], NoReturn] = on_app_modified_settings  # Call this to signal that the UI needs to refresh.
         self._on_user_applied_settings: Callable[[int], NoReturn] = on_user_applied_settings  # Call this to signal that the application needs to refresh.
         self.show_grid = True
         self.show_profile = show_profile
-        self.fft_samples = DEFAULT_FFT_SAMPLES
-        self.fft_overlap = DEFAULT_FFT_OVERLAP_PERCENT
+        self.window_samples = DEFAULT_FFT_SAMPLES
+        self.window_overlap = DEFAULT_FFT_OVERLAP_PERCENT
         self.window_type = DEFAULT_WINDOW_TYPE
+        self.window_padding_factor = DEFAULT_FFT_WINDOW_PADDING_FACTOR
         self.zoom_interpolation = DEFAULT_INTERPOLATION
         self.do_histogram_normalization = False
         self.bnc_adjust_type = BNC_ADAPTIVE_MODE
-        self.bnc_background_threshold_percent = 80.0
+        self.bnc_background_threshold_percent = 60.0
         self.bnc_manual_min, self.bnc_manual_max = 0.0, 1.0
         self.show_time_markers = False
         self.show_frequency_markers = False
+        self.multichannel_mode = MULTICHANNEL_COMBINED_MODE
+        self.multichannel_channel = 0
+        self.spectrogram_type = SPECTROGRAM_TYPE_STANDARD
 
     def on_app_modified_settings(self, draw_scope: int = DrawableFrame.DRAW_ALL) -> NoReturn:
         """Signal to the settings UI that the underlying settings values have changed."""
         self._on_app_modified_settings(draw_scope)
 
     def on_user_applied_settings(self, draw_scope: int = DrawableFrame.DRAW_ALL) -> NoReturn:
         """Signal to the application that the underlying settings values have changed."""
@@ -116,7 +139,10 @@
         # Always start with auto BnC, so that the manual range
         # gets initialized to something sensible:
         self.bnc_adjust_type = BNC_ADAPTIVE_MODE
         # Always start with markers disabled: any existing marker positions may be outside
         # the range of view:
         self.show_time_markers = False
         self.show_frequency_markers = False
+
+        # Reset various things for the new file:
+        self.spectrogram_type = SPECTROGRAM_TYPE_STANDARD
```

### Comparing `batogram-1.0.9/batogram/historianservice.py` & `batogram-1.1.0/batogram/historianservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/layouts.py` & `batogram-1.1.0/batogram/layouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,24 +151,23 @@
 
     def rect_to_values(self, pixel_rect) \
             -> Optional[Tuple[float, float, float, float]]:
         """Scale the pixel rectangle supplied to real axis values."""
 
         l, t, r, b = pixel_rect
         if self._x_axis and self._y_axis:
-            # if clamp:
             vl = self._x_axis.canvas_to_axis(l)
             vr = self._x_axis.canvas_to_axis(r)
             vt = self._y_axis.canvas_to_axis(t)
             vb = self._y_axis.canvas_to_axis(b)
             return vl, vt, vr, vb
         else:
             return None
 
-    def canvas_to_axis(self, p_canvas):
+    def canvas_to_axis(self, p_canvas: Tuple[int, int]) -> Optional[Tuple[float, float]]:
         """Scale the pixel position relative to the canvas origin to real axis values."""
 
         t_canvas, f_canvas = p_canvas
         if self._x_axis and self._y_axis:
             # We can get the axis values of t and f from the axis scale:
             t_axis = self._x_axis.canvas_to_axis(t_canvas)
             f_axis = self._y_axis.canvas_to_axis(f_canvas)
```

### Comparing `batogram-1.0.9/batogram/markers.py` & `batogram-1.1.0/batogram/markers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# Copyright (c) 2023 John Mears
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import tkinter as tk
 from abc import ABC, abstractmethod
 from typing import Tuple, Optional, Callable, Type, List
 
 from .constants import AXIS_FONT_NAME, AXIS_FONT_HEIGHT
 from .common import AxisRange, clip_to_range, AreaTuple, RangeTuple
 
@@ -215,18 +235,18 @@
     def draw_text_impl(self, canvas: "SpectrogramCanvas", band_rect: AreaTuple,
                        text: List[str], is_clipped: Tuple[bool, bool]) -> List[int]:
         text_ids = []
         if len(text) == 2:
             l, t, r, b = band_rect
             delta = 2  # Avoid crowding.
             if not is_clipped[0]:
-                text_ids.append(canvas.create_text(r - delta, t, text=text[0],
+                text_ids.append(canvas.create_text(l - delta, t, text=text[0],
                                                    fill=MARKER_TEXT_COLOUR, font=AXIS_FONT, anchor=tk.SE))
             if not is_clipped[1]:
-                text_ids.append(canvas.create_text(r - delta, b, text=text[1],
+                text_ids.append(canvas.create_text(l - delta, b, text=text[1],
                                                    fill=MARKER_TEXT_COLOUR, font=AXIS_FONT, anchor=tk.SE))
 
         return text_ids
 
     def draw_overflows(self, canvas: "SpectrogramCanvas", band_pixel_width: RangeTuple,
                        band_pixel_length: RangeTuple, axis_pixel_range: RangeTuple):
         if band_pixel_length[0] > axis_pixel_range[0]:
@@ -250,15 +270,15 @@
             w0, p,
             int((w0 + w1) / 2), p - abs(w0 - w1) / 1.3,
             w1, p,
             fill=MARKER_DRAGGER_COLOUR, outline=MARKER_DRAGGER_COLOUR)
 
 
 class AbstractMarker(ABC):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  initial_axis_value: Optional[float], tag_name: str, get_other: Callable,
                  helper: Type[AbstractHelper], drag_curser: str):
         self._axis_value: Optional[float] = initial_axis_value
         self._pixel_value: Optional[int] = None
         self._pair = pair
         self._sgf = sgf
         self._tag_name: str = tag_name
@@ -332,14 +352,17 @@
 
     def _mouse_leaves_dragger(self, _):
         # Only if we aren't currently dragging - avoids cursor flicker during the drag.
         if self._start_event is None and self._saved_cursor is not None:
             self._canvas.config(cursor=self._saved_cursor)
             self._saved_cursor = None
 
+    def set_position(self, value: float):
+        self._axis_value = value
+
     def _on_click(self, event):
         # print("_on_click: {}".format(event))
         self._start_event = event
         self._start_pixel_value = self._pixel_value
 
         # Set the cursor at the canvas level so it doesn't flicker during dragging:
         self._canvas.config(cursor=self._drag_curser)
@@ -406,15 +429,15 @@
         """Convert the supplied pixel value to an axis value."""
         lower, upper = self._pixel_range
         v = (p - lower) / (upper - lower) * (self._axis_range.max - self._axis_range.min) + self._axis_range.min
         return v
 
 
 class TimeMarker(AbstractMarker, ABC):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  initial_axis_value: Optional[float], tag_name: str, get_other: Callable,
                  helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, initial_axis_value, tag_name, get_other, helper, LR_DRAG_CURSOR)
 
     def create_drawer(self, marker_rect: AreaTuple, pixel_value: int, line_span: RangeTuple) \
             -> Tuple[Callable, RangeTuple]:
         marker_l, marker_t, marker_r, marker_b = marker_rect
@@ -454,30 +477,30 @@
         self._axis_value = self._pixel_to_value(x_current)
 
     def get_pixels_dragged(self, event, start_event):
         return event.x - start_event.x
 
 
 class LowerTimeMarker(TimeMarker):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  axis_value: Optional[float], get_other: Callable, helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, axis_value, "lower_marker", get_other, helper)
 
     def do_move(self, x: int):
         super().do_move(x)
         # Notify the pair to redraw the band before we move the marker:
         self._pair.do_move_lower(x)
 
     def get_allowed_for_other(self) -> Tuple[Optional[int], Optional[int]]:
         # The other marker needs to be higher than this one.
         return self.get_pixel_value() + CLEARANCE_PIXELS, None
 
 
 class UpperTimeMarker(TimeMarker):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  axis_value: Optional[float], get_other: Callable, helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, axis_value, "upper_marker", get_other, helper)
 
     def do_move(self, x: int):
         super().do_move(x)
         # Notify the pair to redraw the band before we move the marker:
         self._pair.do_move_upper(x)
@@ -485,15 +508,15 @@
     def get_allowed_for_other(self) -> Tuple[Optional[int], Optional[int]]:
         # The other marker needs to be lower than us.
         return None, self.get_pixel_value() - CLEARANCE_PIXELS
 
 
 class FrequencyMarker(AbstractMarker, ABC):
 
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  initial_axis_value: Optional[float], tag_name: str, get_other: Callable,
                  helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, initial_axis_value, tag_name, get_other, helper, UD_DRAG_CURSOR)
 
     def create_drawer(self, marker_rect: AreaTuple, pixel_value: int, line_span: RangeTuple) \
             -> Tuple[Callable, RangeTuple]:
         marker_l, marker_t, marker_r, marker_b = marker_rect
@@ -533,44 +556,44 @@
         self._axis_value = self._pixel_to_value(pixel_current)
 
     def get_pixels_dragged(self, event, start_event):
         return event.y - start_event.y
 
 
 class LowerFrequencyMarker(FrequencyMarker):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  axis_value: Optional[float], get_other: Callable, helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, axis_value, "lower_frequency_marker", get_other, helper)
 
     def do_move(self, x: int):
         super().do_move(x)
         # Notify the pair to redraw the band before we move the marker:
         self._pair.do_move_lower(x)
 
     def get_allowed_for_other(self) -> Tuple[Optional[int], Optional[int]]:
         # The other marker needs to be higher than this one.
         return None, self.get_pixel_value() - CLEARANCE_PIXELS
 
 
 class UpperFrequencyMarker(FrequencyMarker):
-    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[MarkerPair]", sgf: "SpectrogramGraphFrame",
+    def __init__(self, canvas: "SpectrogramCanvas", pair: "Type[AbstractMarkerPair]", sgf: "SpectrogramGraphFrame",
                  axis_value: Optional[float], get_other: Callable, helper: Type[AbstractHelper]):
         super().__init__(canvas, pair, sgf, axis_value, "upper_frequency_marker", get_other, helper)
 
     def do_move(self, x: int):
         super().do_move(x)
         # Notify the pair to redraw the band before we move the marker:
         self._pair.do_move_upper(x)
 
     def get_allowed_for_other(self) -> Tuple[Optional[int], Optional[int]]:
         # The other marker needs to be lower than us.
         return self.get_pixel_value() + CLEARANCE_PIXELS, None
 
 
-class MarkerPair(ABC):
+class AbstractMarkerPair(ABC):
     """Abstract MarkerPair that doesn't know if it is vertical or horizontal."""
 
     def __init__(self, canvas: "SpectrogramCanvas", sgf: "SpectrogramGraphFrame",
                  lower_marker: AbstractMarker, upper_marker: AbstractMarker, helper: Type[AbstractHelper]):
         self._lower_marker: AbstractMarker = lower_marker
         self._upper_marker: AbstractMarker = upper_marker
         self._sgf = sgf
@@ -579,14 +602,24 @@
         self._lower_overflow_id = self._upper_overflow_id = None
         self._axis_range: Optional[AxisRange] = None
         self._axis_pixel_range: Optional[RangeTuple] = None
         self._helper: Type[AbstractHelper] = helper
         self._band_rect: Optional[AreaTuple] = None
         self._is_clipped: Tuple[bool, bool] = False, False
 
+    def set_positions(self, positions: Tuple[Optional[float], Optional[float]]):
+        v_lower, v_upper = positions
+        if v_lower is not None:
+            self._lower_marker.set_position(v_lower)
+        if v_upper is not None:
+            self._upper_marker.set_position(v_upper)
+
+    def get_positions(self) -> Tuple[float, float]:
+        return self._lower_marker.get_axis_value(), self._upper_marker.get_axis_value()
+
     def get_lower_marker(self) -> AbstractMarker:
         return self._lower_marker
 
     def get_upper_marker(self) -> AbstractMarker:
         return self._upper_marker
 
     def clip_to_pixel_range(self, v: int):
@@ -628,15 +661,15 @@
                                                                    self._axis_pixel_range, text_list)
 
         # Draw the markers step 1: do the actual drawing here so that they are above the band:
         self._lower_id = lower_drawer()
         self._upper_id = upper_drawer()
 
 
-class TimeMarkerPair(MarkerPair):
+class TimeMarkerPair(AbstractMarkerPair):
     _tag_name = "band"
 
     def __init__(self, canvas: "SpectrogramCanvas", sgf: "SpectrogramGraphFrame",
                  lower_value: Optional[float], upper_value: Optional[float]):
         helper: Type[AbstractHelper] = TimeHelper()
         super().__init__(canvas, sgf,
                          LowerTimeMarker(canvas, self, sgf, lower_value, self.get_upper_marker, helper),
@@ -664,15 +697,15 @@
             text = "{0:.1f} ms".format(v_span * 1000)
         else:
             text = "{0:.3f} s".format(v_span)
 
         return [text]
 
 
-class FrequencyMarkerPair(MarkerPair):
+class FrequencyMarkerPair(AbstractMarkerPair):
     _tag_name = "frequency_band"
 
     def __init__(self, canvas: "SpectrogramCanvas", sgf: "SpectrogramGraphFrame",
                  lower_value: Optional[float], upper_value: Optional[float]):
         helper: Type[AbstractHelper] = FrequencyHelper()
         super().__init__(canvas, sgf,
                          LowerFrequencyMarker(canvas, self, sgf, lower_value, self.get_upper_marker, helper),
```

### Comparing `batogram-1.0.9/batogram/morebncframe.py` & `batogram-1.1.0/batogram/morebncframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,20 @@
 import numpy as np
 
 from . import colourmap
 from abc import abstractmethod, ABC
 from typing import Any, List, Tuple, Optional
 from .common import clip_to_range
 from .frames import DrawableFrame
-from .validatingwidgets import ValidatingMapOptionMenu, ValidatingFrameHelper, ValidatingRadiobutton, \
+from .validatingwidgets import ValidatingFrameHelper, ValidatingRadiobutton, \
     DoubleValidatingEntry
-from .graphsettings import GraphSettings, BNC_MODES, borderwidth, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, \
+from .graphsettings import GraphSettings, borderwidth, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, \
     BNC_INTERACTIVE_MODE
 
 
-class BnCModeOptionMenu(ValidatingMapOptionMenu):
-    """A menu listing BnC modes."""
-
-    def __init__(self, parent, controlling_frame, container, value_validator=None):
-        super().__init__(parent, controlling_frame, container, BNC_MODES, value_validator)
-
-
 class ValidatingFrame(tk.Frame, ValidatingFrameHelper):
     def __init__(self, parent, settings: GraphSettings):
         super().__init__(parent)
         ValidatingFrameHelper.__init__(self, parent, settings)
 
 
 class HistogramInterface(ABC):
@@ -72,18 +65,18 @@
 
     def __init__(self, parent, button_frame, settings: GraphSettings, pad):
         super().__init__(parent, borderwidth=borderwidth)
         ValidatingFrameHelper.__init__(self, parent, settings)
 
         self._settings = settings
 
-        def threshold_validator(v): return self.double_value_validator(v, minimum_value=0.0, maximum_value=100.0,
-                                                                       message="The background threshold must bein the range 0 to 100.")
+        def threshold_validator(v): return self.generic_value_validator(v, minimum_value=0.0, maximum_value=100.0,
+                                                                        message="The background threshold must bein the range 0 to 100.")
 
-        self._mode_var = tk.IntVar(value=BNC_MODES)  # Note: can't be a local variable.
+        self._mode_var = tk.IntVar(value=BNC_ADAPTIVE_MODE)  # Note: can't be a local variable.
         self._auto_radiobutton = ValidatingRadiobutton(self, button_frame, self, "Auto",
                                                        self._mode_var, BNC_ADAPTIVE_MODE)
         self._auto_radiobutton.grid(row=0, column=0, sticky="W")
 
         auto_details_frame = ValidatingFrame(self, settings)
 
         self._auto_label1 = tk.Label(auto_details_frame, text="Background removal:", anchor=tk.W)
@@ -108,16 +101,16 @@
 
         self._manual_label1 = tk.Label(manual_details_frame, text="Range:", anchor=tk.W)
         self._manual_label1.grid(row=0, column=0, sticky="W")
         self._manual_min = DoubleValidatingEntry(manual_details_frame, button_frame, self, width=7, decimal_places=1)
         self._manual_min.grid(row=0, column=1, sticky="W")
         self._manual_label2 = tk.Label(manual_details_frame, text="to", anchor=tk.W)
         self._manual_label2.grid(row=0, column=2, sticky="W")
-        def db_max_validator(v): return self.double_value_validator(v, minimum_entry=self._manual_min,
-                                                                    message="The maximum must be greater than the minimum.")
+        def db_max_validator(v): return self.generic_value_validator(v, minimum_entry=self._manual_min,
+                                                                     message="The maximum must be greater than the minimum.")
 
         self._manual_max = DoubleValidatingEntry(manual_details_frame, button_frame, self, width=7, decimal_places=1,
                                                  value_validator=db_max_validator)
         self._manual_max.grid(row=0, column=3, sticky="W")
         self._manual_label3 = tk.Label(manual_details_frame, text="dB", anchor="e")
         self._manual_label3.grid(row=0, column=4, sticky="W")
 
@@ -500,16 +493,19 @@
         # Cache some things in case of redraw:
         self._data = data
         self._width = width
         # Draw the histogram:
         self._draw(width, height)
 
     def _draw(self, width: int, height: int):
+        # Slight hack: we ignore the lowest few percent of data to avoid artificial wide ranging values
+        # in reassignment spectrum:
+        vmin = np.percentile(self._data, 5)
         # density=False to avoid log10(0) error
-        self._histogram, self._bin_edges = np.histogram(self._data, width)
+        self._histogram, self._bin_edges = np.histogram(self._data[self._data > vmin], width)
         hmin, hmax = 0, self._histogram.max()  # Range to draw.
 
         # Don't try to draw the histogram if the canvas is very small - which happens when the canvas
         # is out of sight because it has been grid_removed.
         if hmax > 0 and width > 10 and height > 10:
             # Construct the points in the profile line:
             points = [(x, height * (1 - (self._histogram[x] - hmin) / hmax)) for x in range(len(self._histogram))]
```

### Comparing `batogram-1.0.9/batogram/moreframe.py` & `batogram-1.1.0/batogram/moreframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import numpy as np
 
 from .graphsettings import GraphSettings
 
 from tkinter import scrolledtext
 from tkinter import messagebox, ttk, font
 from .morebncframe import HistogramInterface, BrightnessContrastFrame
+from .moreotherframe import OtherFrame
 from .morerenderingframe import RenderingFrame
 from .morescaleframe import ScaleFrame
 from .external.tooltip import ToolTip
 from .validatingwidgets import ControllingFrameMixin
 from .external.guano import GuanoFile
 
 
@@ -233,29 +234,34 @@
         self._bnc_frame = BrightnessContrastFrame(self, button_frame, settings, pad)
         self.add(self._bnc_frame, text="Brightness/Contrast")
         self._histogram_interface = self._bnc_frame.get_histogram_interface()
 
         self._processing_frame = RenderingFrame(self, button_frame, settings, pad)
         self.add(self._processing_frame, text="Rendering")
 
+        self._other_frame = OtherFrame(self, button_frame, settings, pad)
+        self.add(self._other_frame, text="Other")
+
         # Tab key moves between tabs:
         self.enable_traversal()
 
     def copy_settings_to_widgets(self):
         """Called by the application when it has changed a setting. This method updates the UI accordingly."""
         self._axis_frame.copy_settings_to_widgets()
         self._processing_frame.copy_settings_to_widgets()
         self._bnc_frame.copy_settings_to_widgets()
+        self._other_frame.copy_settings_to_widgets()
 
     def copy_widgets_to_settings(self):
         """Called by the controlling frame when the user has applied a new set of settings from
         the UI."""
         self._axis_frame.copy_widgets_to_settings()
         self._processing_frame.copy_widgets_to_settings()
         self._bnc_frame.copy_widgets_to_settings()
+        self._other_frame.copy_widgets_to_settings()
 
     def set_guano_data(self, data: GuanoFile):
         self._guano_frame.set_guano_data(data)
 
     def show_histogram(self, data: np.ndarray):
         self._histogram_interface.show_histogram(data)
```

### Comparing `batogram-1.0.9/batogram/morerenderingframe.py` & `batogram-1.1.0/batogram/morerenderingframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import math
 import tkinter as tk
 
 from .graphsettings import FFT_SAMPLES_OPTIONS, FFT_OVERLAP_PERCENT_OPTIONS, INTERPOLATION_OPTIONS, WINDOW_TYPE_OPTIONS, \
-    borderwidth, GraphSettings
+    borderwidth, GraphSettings, SPECTROGRAM_TYPE_OPTIONS, FFT_WINDOW_PADDING_FACTOR
 from .validatingwidgets import ValidatingMapOptionMenu, ValidatingFrameHelper
 
 
 class FFTSamplesOptionMenu(ValidatingMapOptionMenu):
     """A drop down menu listing available number of samples per FFT segment."""
 
     def __init__(self, parent, controlling_frame, container, value_validator=None):
@@ -48,54 +48,77 @@
 
 class WindowTypeOptionMenu(ValidatingMapOptionMenu):
     """A drop down menu listing available FFT window types."""
     def __init__(self, parent, controlling_frame, container, value_validator=None):
         super().__init__(parent, controlling_frame, container, WINDOW_TYPE_OPTIONS, value_validator)
 
 
+class SpectrogramTypeOptionMenu(ValidatingMapOptionMenu):
+    """A drop down menu listing available spectrogram types."""
+    def __init__(self, parent, controlling_frame, container, value_validator=None):
+        super().__init__(parent, controlling_frame, container, SPECTROGRAM_TYPE_OPTIONS, value_validator)
+
+
+class WindowPaddingOptionMenu(ValidatingMapOptionMenu):
+    """A drop down menu listing available FFT window types."""
+    def __init__(self, parent, controlling_frame, container, value_validator=None):
+        super().__init__(parent, controlling_frame, container, FFT_WINDOW_PADDING_FACTOR, value_validator)
+
+
 class RenderingFrame(tk.Frame, ValidatingFrameHelper):
     """A Frame containing settings relating to rendering the spectrogram."""
 
     def __init__(self, parent, controlling_frame, settings: GraphSettings, pad):
         super().__init__(parent, borderwidth=borderwidth)
         ValidatingFrameHelper.__init__(self, parent, settings)
 
         self._settings = settings
 
-        tk.Label(self, text="FFT samples:", anchor="e", padx=pad).grid(row=0, column=0, sticky="EW")
-        tk.Label(self, text="FFT overlap:", anchor="e", padx=pad).grid(row=1, column=0, sticky="EW")
-        tk.Label(self, text="Window type:", anchor="e", padx=pad).grid(row=0, column=3, sticky="EW")
-        tk.Label(self, text="Image interpolation:", anchor="e", padx=pad).grid(row=1, column=3, sticky="EW")
-
         tk.Label(self, text="%", anchor="e", padx=pad).grid(row=1, column=2, sticky="EW")
 
         def fft_samples_validator(v):
             log_v = math.log2(v)
             valid = log_v == int(log_v)
             return "FFT sample number must be a power of 2" if not valid else None
 
+        tk.Label(self, text="Window samples:", anchor="e", padx=pad).grid(row=0, column=0, sticky="EW")
         self._samples_listbox = FFTSamplesOptionMenu(self, controlling_frame, self,
                                                      value_validator=fft_samples_validator)
         self._samples_listbox.grid(row=0, column=1, sticky="EW")
 
+        tk.Label(self, text="Window overlap:", anchor="e", padx=pad).grid(row=1, column=0, sticky="EW")
         self._overlap_listbox = FFTOverlapOptionMenu(self, controlling_frame, self)
         self._overlap_listbox.grid(row=1, column=1, sticky="EW")
 
+        tk.Label(self, text="Spectrogram type:", anchor="e", padx=pad).grid(row=2, column=0, sticky="EW")
+        self._spectrogram_type_listbox = SpectrogramTypeOptionMenu(self, controlling_frame, self)
+        self._spectrogram_type_listbox.grid(row=2, column=1, sticky="EW")
+
+        tk.Label(self, text="Window type:", anchor="e", padx=pad).grid(row=0, column=3, sticky="EW")
         self._window_type_listbox = WindowTypeOptionMenu(self, controlling_frame, self)
         self._window_type_listbox.grid(row=0, column=4, sticky="EW")
 
+        tk.Label(self, text="Window padding factor:", anchor="e", padx=pad).grid(row=1, column=3, sticky="EW")
+        self._window_padding_listbox = WindowPaddingOptionMenu(self, controlling_frame, self)
+        self._window_padding_listbox.grid(row=1, column=4, sticky="EW")
+
+        tk.Label(self, text="Image interpolation:", anchor="e", padx=pad).grid(row=2, column=3, sticky="EW")
         self._interpolation_order_listbox = InterpolationOptionMenu(self, controlling_frame, self)
-        self._interpolation_order_listbox.grid(row=1, column=4, sticky="EW")
+        self._interpolation_order_listbox.grid(row=2, column=4, sticky="EW")
 
         self.copy_settings_to_widgets()
 
     def copy_settings_to_widgets(self):
-        self._samples_listbox.set_value(self._settings.fft_samples)
-        self._overlap_listbox.set_value(self._settings.fft_overlap)
+        self._samples_listbox.set_value(self._settings.window_samples)
+        self._overlap_listbox.set_value(self._settings.window_overlap)
         self._window_type_listbox.set_value(self._settings.window_type)
+        self._window_padding_listbox.set_value(self._settings.window_padding_factor)
         self._interpolation_order_listbox.set_value(self._settings.zoom_interpolation)
+        self._spectrogram_type_listbox.set_value(self._settings.spectrogram_type)
 
     def copy_widgets_to_settings(self):
-        self._settings.fft_samples = self._samples_listbox.get_value()
-        self._settings.fft_overlap = self._overlap_listbox.get_value()
+        self._settings.window_samples = self._samples_listbox.get_value()
+        self._settings.window_overlap = self._overlap_listbox.get_value()
         self._settings.window_type = self._window_type_listbox.get_value()
+        self._settings.window_padding_factor = self._window_padding_listbox.get_value()
         self._settings.zoom_interpolation = self._interpolation_order_listbox.get_value()
+        self._settings.spectrogram_type = self._spectrogram_type_listbox.get_value()
```

### Comparing `batogram-1.0.9/batogram/morescaleframe.py` & `batogram-1.1.0/batogram/morescaleframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,38 +44,38 @@
         tk.Label(self, text="Time:", anchor="e").grid(row=1, column=0, sticky="EW", padx=pad)
         tk.Label(self, text="s", anchor="e").grid(row=1, column=3, sticky="W")
         tk.Label(self, text="Frequency:", anchor="e").grid(row=2, column=0, sticky="EW", padx=pad)
         tk.Label(self, text="kHz", anchor="e").grid(row=2, column=3, sticky="W")
 
         width = 8
 
-        def t_min_validator(v): return self.double_value_validator(v, minimum_value=0,
-                                                                   message="The minimum time must be zero or positive.")
+        def t_min_validator(v): return self.generic_value_validator(v, minimum_value=0,
+                                                                    message="The minimum time must be zero or positive.")
 
         self._t_min = DoubleValidatingEntry(self, controlling_frame, self, width=width, decimal_places=self._TIME_DPS,
                                             value_validator=t_min_validator)
         self._t_min.grid(row=1, column=1, padx=pad)
 
-        def t_max_validator(v): return self.double_value_validator(v, minimum_entry=self._t_min,
-                                                                   message="The maximum time must be greater than the minimum.")
+        def t_max_validator(v): return self.generic_value_validator(v, minimum_entry=self._t_min,
+                                                                    message="The maximum time must be greater than the minimum.")
 
         self._t_max = DoubleValidatingEntry(self, controlling_frame, self, width=width, decimal_places=self._TIME_DPS,
                                             value_validator=t_max_validator)
         self._t_max.grid(row=1, column=2, padx=pad)
 
-        def f_min_validator(v): return self.double_value_validator(v, minimum_value=0,
-                                                                   message="The minimum frequency must be zero or postive.")
+        def f_min_validator(v): return self.generic_value_validator(v, minimum_value=0,
+                                                                    message="The minimum frequency must be zero or postive.")
 
         self._f_min = DoubleValidatingEntry(self, controlling_frame, self, width=width,
                                             decimal_places=self._FREQUENCY_DPS,
                                             scaler=self._FREQUENCY_SCALER, value_validator=f_min_validator)
         self._f_min.grid(row=2, column=1, padx=pad)
 
-        def f_max_validator(v): return self.double_value_validator(v, minimum_entry=self._f_min,
-                                                                   message="The maximum frequency must be greater than the minimum.")
+        def f_max_validator(v): return self.generic_value_validator(v, minimum_entry=self._f_min,
+                                                                    message="The maximum frequency must be greater than the minimum.")
 
         self._f_max = DoubleValidatingEntry(self, controlling_frame, self, width=width,
                                             decimal_places=self._FREQUENCY_DPS,
                                             scaler=self._FREQUENCY_SCALER, value_validator=f_max_validator)
         self._f_max.grid(row=2, column=2, padx=pad)
 
         self._show_time_markers_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show markers")
```

### Comparing `batogram-1.0.9/batogram/profilegraphframe.py` & `batogram-1.1.0/batogram/profilegraphframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.9/batogram/readoutframe.py` & `batogram-1.1.0/batogram/readoutframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         self._parent = parent
 
         self._settings_button: SettingsButton = SettingsButton(self)
         self._settings_button.grid(row=0, column=0, sticky="ns", padx=(0, 10))
 
         self._parameters_variable = tk.StringVar(value="")
-        self._parameters_label = tk.Label(self, textvariable=self._parameters_variable, width=20, anchor=tk.W)
+        self._parameters_label = tk.Label(self, textvariable=self._parameters_variable, width=40, anchor=tk.W)
         self._parameters_label.grid(row=0, column=1, sticky="nsew")
 
         self._coords_variable = tk.StringVar(value="")
         self._coords_label = tk.Label(self, textvariable=self._coords_variable, width=20, anchor=tk.E)
         self._coords_label.grid(row=0, column=2, sticky="nsew")
 
         self.columnconfigure(0, weight=0)
@@ -76,12 +76,21 @@
             t, f = position
             text = "{:.4} s, {:.1f} kHz".format(t, f / 1000.0, power)
         if power is not None:
             text += ", {:.1f} dB".format(power)
         self._coords_variable.set(text)
 
     def update_graph_parameters(self, params: GraphParams):
-        self._parameters_variable.set("{} {}, {}% overlap".format(
-            WINDOW_TYPE_OPTIONS[params.window_type], params.fft_samples, params.fft_overlap))
+        if params.specific_channel is None:
+            if params.num_channels == 1:
+                channel_text = "1 channel"
+            else:
+                channel_text = "{} channels combined".format(params.num_channels)
+        else:
+            channel_text = "channel {} only".format(params.specific_channel)
+
+        self._parameters_variable.set("{} {}, {}% overlap, {}x window padding, {}".format(
+            WINDOW_TYPE_OPTIONS[params.window_type], params.window_samples, params.window_overlap,
+            params.window_padding_factor, channel_text))
 
     def get_settings_button(self) -> SettingsButton:
         return self._settings_button
```

### Comparing `batogram-1.0.9/batogram/rendering.py` & `batogram-1.1.0/batogram/rendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 from threading import Lock, Thread, Condition
 from typing import Type, Tuple, Optional, Any, Callable
 from scipy import ndimage
 from .audiofileservice import AudioFileService, RawDataReader
 from .chunky_spectrogram import chunky_spectrogram
 from .common import AxisRange, AreaTuple, clip_to_range
 from .graphsettings import GraphSettings, ADAPTIVE_FFT_SAMPLES, ADAPTIVE_FFT_OVERLAP_PERCENT, \
-    FFT_OVERLAP_PERCENT_OPTIONS, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, BNC_INTERACTIVE_MODE
+    FFT_OVERLAP_PERCENT_OPTIONS, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, BNC_INTERACTIVE_MODE, MULTICHANNEL_SINGLE_MODE, \
+    SPECTROGRAM_TYPE_REASSIGNMENT, SPECTROGRAM_TYPE_STANDARD, SPECTROGRAM_TYPE_ADAPTIVE
 
 
 class RenderingRequest:
     """The base class for rendering pipeline requests of any kind."""
 
     def __init__(self, data_area: AreaTuple, file_data: AudioFileService.RenderingData):
         self.data_area: AreaTuple = data_area
@@ -113,15 +114,15 @@
                 # You called, my lord?
 
                 # Atomically consume any request before we release the condition lock:
                 pending_request_tuple: Optional[PendingRequestTuple] = self._pending_request_tuple
                 self._pending_request_tuple = None
 
             if self._shutting_down:
-                print("Exiting from pipeline thread.")
+                # print("Exiting from pipeline thread.")
                 return
 
             if pending_request_tuple is None:  # I suppose this might happen if there is a race I haven't thought of.
                 continue
 
             request, on_completion, on_error = pending_request_tuple
 
@@ -240,16 +241,19 @@
 
 
 @dataclass
 class GraphParams:
     """Parameters for the graph that will be displayed in the UI."""
 
     window_type: str
-    fft_samples: int
-    fft_overlap: float
+    window_samples: int
+    window_overlap: float
+    window_padding_factor: int
+    num_channels: int  # How many channels are in the input data.
+    specific_channel: Optional[int]  # None if we combined all channels, otherwise the single channel number we used.
 
 
 class BnCHelper:
     """Helper functions used for Brightness and Contrast handling."""
 
     @staticmethod
     def get_scalar_vmax(data):
@@ -257,17 +261,22 @@
         try:
             vmax = data.max()
         except ValueError as e:
             vmax = 0.0
         return vmax
 
     @staticmethod
-    def get_scalar_vmin(data, percent: float):
+    def get_scalar_vmin(data: np.ndarray, percent: float):
         try:
-            vmin = np.percentile(data, percent)
+            # Percentile corresponds to area of the image, which depends strongly on standard versus
+            # reassigned spectrogram. That means different percents needed. So, we do a simple
+            # percentage of the range instead.
+            # vmin = np.percentile(data, percent)
+
+            vmin = (data.max() - data.min()) * percent / 100.0 + data.min()
         except IndexError as e:
             vmin = 0.0
         return vmin
 
 
 @dataclass
 class SpectrogramCalcData:
@@ -287,26 +296,26 @@
     first_time_index_for_amp: int
     last_time_index_for_amp: int  # Half open
 
     first_freq_index: int
     last_freq_index: int  # Half open
     actual_freq_axis_min: float
     actual_freq_axis_max: float
-    actual_fft_samples: int
-    actual_fft_overlap_percent: float
-    actual_fft_overlap_samples: int
+    actual_window_samples: int
+    actual_window_overlap_percent: float
+    actual_window_overlap_samples: int
     step_count: int
 
     def __init__(self, settings: GraphSettings, axis_time_range: AxisRange, axis_frequency_range: AxisRange,
                  file_data: AudioFileService.RenderingData, screen_factors: Tuple[float, float],
                  canvas_width: int, canvas_height: int):
         """
             Do all the scale and offset calculations we will need to render a spectrogram.
 
-            Note: we choose t=0 axis time to be the middle of the first sfft segment. This
+            Note: we choose t=0 axis time to be the middle of the first padded window segment. This
             avoids the complication of the first segment offset being more than subsequent ones
             if we chose t=0 to be the left of the first segment. This results in possible negative
             time indexes, which client code clips to 0 and ignores.
 
             At the ends of the time range we clip the time to what is actually available, which
             can result offsets near the ends. Never mind.
 
@@ -314,61 +323,65 @@
             which appears in the UI as a blank at the end, relative to the length of data calculated based
             on the sample rate and number of points in the file.
         """
 
         # General preparation:
         sample_rate: int = file_data.sample_rate
 
-        if settings.fft_samples == ADAPTIVE_FFT_SAMPLES:
-            self.actual_fft_samples = self._calculate_auto_fft_samples(sample_rate, screen_factors)
+        if settings.window_samples == ADAPTIVE_FFT_SAMPLES:
+            self.actual_window_samples = self._calculate_auto_window_samples(sample_rate, screen_factors)
         else:
-            self.actual_fft_samples = settings.fft_samples
+            self.actual_window_samples = settings.window_samples
 
-        if settings.fft_overlap == ADAPTIVE_FFT_OVERLAP_PERCENT:
-            self.actual_fft_overlap_percent = self._calculate_auto_fft_overlap(
-                sample_rate, self.actual_fft_samples, screen_factors)
+        if settings.window_overlap == ADAPTIVE_FFT_OVERLAP_PERCENT:
+            self.actual_window_overlap_percent = self._calculate_auto_window_overlap(
+                sample_rate, self.actual_window_samples, screen_factors)
         else:
-            self.actual_fft_overlap_percent = settings.fft_overlap
+            self.actual_window_overlap_percent = settings.window_overlap
 
-        # print("fft_samples = {}, fft_overlap = {}".format(self.actual_fft_samples, self.actual_fft_overlap_percent))
-        self.actual_fft_overlap_samples = int(self.actual_fft_overlap_percent / 100.0 * self.actual_fft_samples)
-        self.step_count: int = int(self.actual_fft_samples - self.actual_fft_overlap_samples)
-        half_segment_offset: int = int(self.actual_fft_samples / 2)  # Ignore the rounding error, small.
-        step_time: float = (self.actual_fft_samples - self.actual_fft_overlap_samples) / sample_rate
+        # Note: window overlap samples may be different from the final segment overlap samples, because of padding:
+        self.actual_window_overlap_samples = int(self.actual_window_overlap_percent / 100.0 * self.actual_window_samples)
+        self.actual_window_overlap_samples = max(1, self.actual_window_overlap_samples)     # Sanity.
+        self.step_count: int = int(self.actual_window_samples - self.actual_window_overlap_samples)
+        step_time: float = self.step_count / sample_rate
+        self.nfft = self.actual_window_samples * settings.window_padding_factor
+        self.nfft_overlap_samples = self.nfft - self.step_count
+        half_nfft_offset: int = int(self.nfft / 2)  # Ignore the rounding error, small.
         time_points = file_data.sample_count
-        # max_segment_count: int = int((time_points - half_segment_offset) / self.step_count) + 1  # Ignore any leftover time points.
         max_segment_count: int = int(
-            (time_points - self.actual_fft_overlap_samples) / self.step_count)  # Ignore any leftover time points.
+            (time_points - self.nfft_overlap_samples) / self.step_count)  # Ignore any leftover time points.
         time_axis_min, time_axis_max = axis_time_range.get_tuple()
         freq_axis_min, freq_axis_max = axis_frequency_range.get_tuple()
 
         # ************** Calculations relating to the time axis **************
 
         def time_to_segment_index(t: float) -> int:
             """Get the segment number corresponding to the axis time. t=0 at the centre of
             the first segment, and offsets are constant between there and subsequent
             centres. We round down intentionally."""
             segment_index = int(t / step_time)  # This rounds *down* to the nearest step
             return segment_index
 
         def segment_index_to_time(i: int) -> float:
-            """Get the axis time corresponding to a segment index - which is the time at the centre of the segment."""
-            t = i * step_time  # - step_time / 2
+            """Get the axis time corresponding to a segment index - which is the time at the centre of the
+            padded segment."""
+            t = i * step_time
             return t
 
         def segment_index_to_time_index(segment_index: int):
-            """Get the index of the FIRST time value that is part of the segment."""
-            # Offset for the spacing of centres - a negative time range index may result.
-            time_index = int(segment_index * self.step_count - half_segment_offset)
+            """Get the index of the FIRST time value that is part of the segment.
+            The result may be negative."""
+            # Offset for the spacing of centres - a negative time range index may result:
+            time_index = int(segment_index * self.step_count - half_nfft_offset)
             return time_index
 
         def time_to_time_index(t: float):
-            """Get the index of the time sample at the centre of the segment whose centre
+            """Get the index of the time sample at the centre of the padded segment whose centre
             is this axis time."""
-            time_index = int(t * sample_rate) + half_segment_offset
+            time_index = int(t * sample_rate)   # + half_nfft_offset
             return time_index
 
         # Convert the axis ranges supplied to data index ranges, rounding outwards.
         # t=0 is the centre of the first sfft segment, so it depends in the window size.
         # This convention avoids varying time offsets as different window sizes are selected.
 
         self.first_segment_index = time_to_segment_index(time_axis_min)
@@ -377,39 +390,40 @@
 
         # Allow a left and right margin to hide any edge artifacts from zooming. The
         # result is data indexes that may be outside the range of available data:
         margin: int = 10
         self.first_segment_index -= margin
         self.last_segment_index += margin
 
-        # Limit the segment indexes to the possible range, last segment index is half open:
+        # Clip the segment indexes to the possible range, last segment index is half open:
         self.first_segment_index = max(0, self.first_segment_index)  # Shouldn't be needed.
         self.last_segment_index = min(max_segment_count, self.last_segment_index)
 
         # Convert the segment index range to a time index range. We know the time indexes are sane,
         # because we clipped the segment indexes above. These time index ranges are the range needed
-        # to calculate the segments - not the time range of the segments.
+        # to *calculate* the segments - not the time range of the segment centres.
         self.first_time_index_for_segs = segment_index_to_time_index(self.first_segment_index)
         # Note: (1) the last_segment_index is half open so - 1. (2) include the full index range for the previous
         # segment so that it can be calculated.
-        self.last_time_index_for_segs = segment_index_to_time_index(
-            self.last_segment_index - 1) + self.actual_fft_samples
+        self.last_time_index_for_segs = segment_index_to_time_index(self.last_segment_index - 1) + self.nfft
 
         # Reverse calculate to the time range we actually cover, which is the segment centres.
         self.actual_time_axis_min = segment_index_to_time(self.first_segment_index)
         self.actual_time_axis_max = segment_index_to_time(self.last_segment_index - 1)  # -1 because half open range
 
         # Calculate the time index range corresponding to the actual axis values:
         self.first_time_index_for_amp = time_to_time_index(self.actual_time_axis_min)
         self.last_time_index_for_amp = time_to_time_index(self.actual_time_axis_max)
 
         # ************** Calculations relating to the frequency axis **************
 
         file_fmin, file_fmax = file_data.frequency_range.get_tuple()
-        freq_points: int = int(self.actual_fft_samples / 2 + 1)  # Includes f=0 and f=nyquist, so +1.
+        # Zero padding the window by a factor makes it longer and increases frequency
+        # points in the same ratio:
+        freq_points: int = int(self.actual_window_samples * settings.window_padding_factor / 2 + 1)  # Includes f=0 and f=nyquist, so +1.
 
         def frequency_to_index(f: float) -> int:
             # Round to nearest index:
             return int((f - file_fmin) / (file_fmax - file_fmin) * freq_points + 0.5)
 
         def index_to_frequency(i: int) -> float:
             # + 0.5 because the index is a frequencey range and we take the
@@ -449,15 +463,15 @@
 
         pixels_per_hz: float = canvas_height / (freq_axis_max - freq_axis_min)
         self.freq_dilated_pixels: int = int(
             pixels_per_hz * (self.actual_freq_axis_max - self.actual_freq_axis_min) + 0.5)
         self.freq_offset_pixels: int = int((freq_axis_min - self.actual_freq_axis_min) * pixels_per_hz + 0.5)
 
     @staticmethod
-    def _calculate_auto_fft_samples(sample_rate: int, screen_factors: Tuple[float, float]) -> int:
+    def _calculate_auto_window_samples(sample_rate: int, screen_factors: Tuple[float, float]) -> int:
         """Select a number of FFT samples that roughly results in square image elements on the screen."""
 
         # Overlapping of windows increases the resultant sample rate:
         # overlap_ratio = 100.0 / (100.0 - fft_overlap_percent)
 
         # It seems to work best if we ignore overlapping - which doesn't actually increase
         # time resolution, just smooths over time:
@@ -466,27 +480,25 @@
         aspect_factor, _ = screen_factors
 
         fft_samples_squared = sample_rate * sample_rate * overlap_ratio * aspect_factor
 
         fft_samples = int(scipy.sqrt(fft_samples_squared) + 0.5)
 
         # Round to the nearest factor of 2:
-        rounded_fft_samples = 2 ** int(scipy.log2(fft_samples) + 0.5)
-        rounded_fft_samples *= 2  # Subjectively, this looks better.
+        rounded_window_samples = 2 ** int(scipy.log2(fft_samples) + 0.5)
+        rounded_window_samples *= 2  # Subjectively, this looks better.
 
         # These limits need to make the range of samples that can be selected manually:
-        rounded_fft_samples = max(64, rounded_fft_samples)
-        rounded_fft_samples = min(4096, rounded_fft_samples)
-
-        # print("calculated fft samples = {}".format(rounded_fft_samples))
+        rounded_window_samples = max(64, rounded_window_samples)
+        rounded_window_samples = min(4096, rounded_window_samples)
 
-        return rounded_fft_samples
+        return rounded_window_samples
 
     @staticmethod
-    def _calculate_auto_fft_overlap(sample_rate, fft_samples, screen_factors) -> int:
+    def _calculate_auto_window_overlap(sample_rate, fft_samples, screen_factors) -> int:
 
         _, pixels_per_second = screen_factors  # Screen scaling.
         fft_window_time: float = fft_samples / sample_rate
         fft_window_pixels: float = pixels_per_second * fft_window_time
 
         # Choose an overlap that results in no more than half a data point per screen pixel:
         multiplier: float = 2.0 / fft_window_pixels
@@ -514,24 +526,28 @@
 
     def __init__(self):
         pass
 
     @staticmethod
     def _estimate_memory_needed(file_data: AudioFileService.RenderingData,
                                 calc_data: SpectrogramCalcData) -> Tuple[int, int]:
-        """Estimate the memory needed to render a spectrogram from file with the settings provided."""
+        """
+        Estimate the memory needed to render a spectrogram from file with the settings provided.
+        Note: this assumes a standard spectrogram. A reassignment spectrogram needs more,
+        because it stores phase and because it allocates more memory to calculate
+        cross products.
+        """
 
         # First, the memory needed to load the raw data from file:
         file_data_samples_needed: int = (calc_data.last_time_index_for_segs - calc_data.first_time_index_for_segs) \
                                         * file_data.channels
         file_data_bytes_needed: int = file_data_samples_needed * file_data.bytes_per_value
 
         # Space needed to store the spectrum data. Divide by two because we discard the phase info.
-        overlap_factor: float = calc_data.actual_fft_samples / (
-                calc_data.actual_fft_samples - calc_data.actual_fft_overlap_samples)
+        overlap_factor: float = calc_data.nfft/ (calc_data.nfft - calc_data.nfft_overlap_samples)
         spectrum_data_bytes_needed: int = int(file_data_samples_needed * overlap_factor * np.float32(0).nbytes / 2)
 
         total_bytes_needed: int = spectrum_data_bytes_needed + file_data_bytes_needed
 
         return total_bytes_needed, file_data_bytes_needed
 
 
@@ -540,15 +556,15 @@
 
     def __init__(self, settings: GraphSettings, spectrogram_step: "SpectrogramFftStep",
                  data_reader_step: "SpectrogramDataReaderStep"):
         super().__init__(settings)
         PipelineHelper.__init__(self)
 
         self._completion_data = None
-        self._graph_params = None
+        self._graph_params: GraphParams = None
         self._histogram_interface = None
         self._spectrogram_step = spectrogram_step
         self._data_reader_step = data_reader_step
         self._zoom_step = SpectrogramZoomStep(settings)
         self._bnc_step = SpectrogramBNCStep(settings)
         self._apply_colour_map_step = SpectrogramApplyColourMapStep(settings)
 
@@ -610,22 +626,22 @@
             None, params)
 
         if rawdata.min() == rawdata.max():
             raise FailGracefullyException("Range of raw data values is zero")
 
         # Include the actual fft samples and overlap to force a cache miss when they change:
         params = raw_data_serial, sample_rate, sample_count, request.axis_time_range, \
-            calc_data.actual_fft_samples, calc_data.actual_fft_overlap_samples, calc_data.actual_fft_overlap_percent, \
+            calc_data.actual_window_samples, calc_data.actual_window_overlap_samples, calc_data.actual_window_overlap_percent, \
             request.is_reference
         (specdata, self._graph_params), specdata_serial, _ = \
             self._spectrogram_step.process_data((rawdata, raw_data_offset), params)
 
         del rawdata  # Allow the gc to reclaim this memory.
 
-        params = raw_data_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
+        params = specdata_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
             file_time_range, file_frequency_range, calc_data
         zoomed_specdata, zoomed_serial, _ = self._zoom_step.process_data(specdata, params)
 
         params = (zoomed_serial,)
         (bnc_specdata, auto_vrange), bnc_serial, _ = self._bnc_step.process_data(zoomed_specdata, params)
         # auto_vrange is the auto range chosen, or None if not in autorange mode.
 
@@ -688,28 +704,36 @@
         super().__init__(settings)
 
     @dataclass
     class RelevantSettings:
         fft_samples: int
         fft_overlap: int
         window_type: str
+        window_padding_factor: int
+        multichannel_mode: int
+        multichannel_channel: int
+        spectrogram_type: int
 
         def __init__(self, settings: GraphSettings):
-            self.fft_samples = settings.fft_samples
-            self.fft_overlap = settings.fft_overlap
+            self.fft_samples = settings.window_samples
+            self.fft_overlap = settings.window_overlap
             self.window_type = settings.window_type
+            self.window_padding_factor = settings.window_padding_factor
+            self.multichannel_mode = settings.multichannel_mode
+            self.multichannel_channel = settings.multichannel_channel
+            self.spectrogram_type = settings.spectrogram_type
 
     def get_relevant_settings(self) -> RelevantSettings:
         """Get the settings subset that is relevant to this step. We will use this as a basis
         for cache invalidation."""
         return SpectrogramFftStep.RelevantSettings(self._settings)
 
     def _implementation(self, inputdata, params):
-        previous_serial, sample_rate, file_data_samples, axis_time_range, actual_fft_samples, \
-            actual_fft_overlap_samples, actual_fft_overlap_percent, is_reference = params
+        previous_serial, sample_rate, file_data_samples, axis_time_range, actual_window_samples, \
+            actual_window_overlap_samples, actual_window_overlap_percent, is_reference = params
         rs = self.get_relevant_settings()
 
         # Input data is a subset of raw data from the input file, chosen to include
         # the axis range required. It consists of the data itself, and the offset from the
         # start of the data file in samples:
         data_read, data_read_offset = inputdata
         _, data_sample_count = data_read.shape
@@ -717,46 +741,50 @@
 
         # We will calculate the spectogram corresponding of the somewhat enlarged actual axis range
         # in the SpectrogramCalcData. Later on, when we zoom the data to fit the display, we will discard
         # the excess data. That means we fft the range of data indexes in the SpectrogramCalcData.
 
         # print("calculating spectrogram: {}: {}", params, inputdata.shape)
 
-        frequencies, combined_spectrogram = self._do_spectrogram(data_read, sample_rate, rs.window_type,
-                                                                 actual_fft_samples, actual_fft_overlap_samples)
+        frequencies, combined_spectrogram, channel_usage_tuple = self._do_spectrogram(
+            data_read, sample_rate, rs.window_type, actual_window_samples, actual_window_overlap_samples, rs)
 
         # print("delta_t = {}".format(delta_t))
 
         # We now have spectrogram data corresponding to *actual* axis range, ie spanning from the middle of the
         # first segment to the middle of the last segment.
 
         # Make sure there aren't any zero values that would make log10 below fail:
         if combined_spectrogram.min() == 0.0:
             # s = np.sort(combined_spectrogram)
-            arbitrary_small_number = 1E-20  # TODO review this arbitrary small number.
+            arbitrary_small_number = 1E-10  # TODO review this arbitrary small number.
             combined_spectrogram = np.where(combined_spectrogram <= 0, arbitrary_small_number, combined_spectrogram)
 
         # Convert the resulting spectrogram to dB.
         # Multiplier is 10, not 20, because _do_spectrogram has already squared it.
         db_spectrogram = 10 * np.log10(combined_spectrogram)
 
         # Apply frequency response correction if required.
         response_data = appsettings.instance.ref_mic_response_data if is_reference else appsettings.instance.main_mic_response_data
         if response_data is not None:
             frequency_response = self._calculate_frequency_response(frequencies, response_data)
             # We need to change the shape of the frequency response so that it will "broadcast" over the spectrogram:
             frequency_response = frequency_response.reshape(-1, 1)
             db_spectrogram -= frequency_response
 
+        num_channels, specific_channel = channel_usage_tuple
+
         return db_spectrogram, \
-            GraphParams(fft_samples=actual_fft_samples, fft_overlap=actual_fft_overlap_percent,
-                        window_type=rs.window_type)
+            GraphParams(window_samples=actual_window_samples, window_overlap=actual_window_overlap_percent,
+                        window_type=rs.window_type, num_channels=num_channels,
+                        window_padding_factor=rs.window_padding_factor, specific_channel=specific_channel)
 
     @staticmethod
-    def _calculate_frequency_response(frequencies: np.ndarray, mic_response_data: Tuple[CubicSpline, float, float, float, float])\
+    def _calculate_frequency_response(frequencies: np.ndarray,
+                                      mic_response_data: Tuple[CubicSpline, float, float, float, float]) \
             -> np.ndarray:
         """Interpolate/extrapolate the microphones response to match the frequency buckets suppled."""
 
         cs, f_min, f_max, r_min, r_max = mic_response_data
         interpolated = cs(frequencies)
         # Override the spline's extrapolation with constant extrapolation (much safer):
         for i in range(len(frequencies)):
@@ -764,77 +792,275 @@
             if f < f_min:
                 interpolated[i] = r_min
             if f > f_max:
                 interpolated[i] = r_max
 
         return interpolated
 
-    @staticmethod
-    def _do_spectrogram(data: np.ndarray, sample_rate: int, window_type, actual_fft_samples: int, overlap: int) \
-            -> Tuple[np.ndarray, np.ndarray]:
+    def _do_spectrogram(self, data: np.ndarray, sample_rate: int, window_type: str, actual_window_samples: int,
+                        overlap: int, rs: RelevantSettings) -> Tuple[np.ndarray, np.ndarray, Tuple]:
         """
         Calculate the spectrogram that is the scalar sum of powers from all channels - ie,
         ignoring phase.
         """
 
-        # Create a spectrogram for each channel:
-        spectrograms = []
-        frequencies = None
-        for d in data:
-            # print("spectrogram of {} points".format(len(d)))
-            # t1 = process_time()
-            fbuckets, _, spectrum_data = chunky_spectrogram(
-                d, fs=sample_rate,
-                window=window_type,
-                nperseg=actual_fft_samples,
-                noverlap=overlap,
-                nfft=None,
-                # detrend=False, # Defaults to constant.
-                return_onesided=True,
-                scaling='density',
-                # So that power dB is independent of window size.
-                # Power per Hz.
-                axis=-1,
-                mode='psd')  # psd to square the data to get power.
+        # Figure out which channels to process:
+        channels_available, samples = data.shape
+        channel_used: Optional[int] = None
+        if rs.multichannel_mode == MULTICHANNEL_SINGLE_MODE and 0 <= rs.multichannel_channel < channels_available:
+            channels_to_process = [rs.multichannel_channel]
+            channel_used = rs.multichannel_channel
+        else:
+            channels_to_process = [i for i in range(0, channels_available)]
 
-            if frequencies is None:
-                frequencies = fbuckets
+        # Create the window at this level so that we have most control over it.
+        # Take account of padding to calculate the actual fft samples:
+        nfft = actual_window_samples * rs.window_padding_factor
+        window_data = scipy.signal.get_window(window_type, actual_window_samples)
+        half_pad = int(((nfft - actual_window_samples) / 2))
+        padded_window_data = np.pad(window_data, (half_pad, half_pad))
+
+        # Calculate a corrresponding overlap taking into account the padding:
+        step = actual_window_samples - overlap      # Independet of window padding.
+        adjusted_overlap = nfft - step
 
-            # t2 = process_time()
-            # print("chunked_spectrogram time: {}".format(t2 - t1))
-            # t1 = process_time()
+        # Create a spectrogram for each channel:
+        spectrograms = []
+        frequency_buckets = None
+        for channel in channels_to_process:
+            fn = self._do_standard_spectrogram
+            if rs.spectrogram_type == SPECTROGRAM_TYPE_REASSIGNMENT:
+                fn = self._do_reassignment_spectrogram
+            elif rs.spectrogram_type == SPECTROGRAM_TYPE_STANDARD:
+                fn = self._do_standard_spectrogram
+            elif rs.spectrogram_type == SPECTROGRAM_TYPE_ADAPTIVE:
+                time_span = samples / sample_rate
+                time_threshold = 0.1        # Reassigment spectrum if they zoom in this far.
+                fn = self._do_standard_spectrogram if time_span > time_threshold else self._do_reassignment_spectrogram
 
-            spectrograms.append(spectrum_data)
+            stft_power, frequency_buckets, _ = fn(data, channel, sample_rate, padded_window_data, nfft, adjusted_overlap)
 
-            # t2 = process_time()
-        #            print("data faffing time: {}".format(t2 - t1))
+            spectrograms.append(stft_power)
 
         # Create a combined spectrogram by summing the power amplitudes. ndarray earns its keep here:
-        # the alternative of doing this by looping dumbly is quite slow.
+        # the alternative of doing this by looping dumbly is very slow.
         # This results in the same data type as in the input array:
 
         _, n_segments = spectrograms[0].shape
 
         # Do the sum in chunks, as ndarray.sum inexplicably assigns lots of memory.
-        chunk_size: int = 10000  # TODO
+        chunk_size: int = 10000  # Arbitrary - optimize this
         samples_done = 0
         while samples_done < n_segments:
             # Create a sub-range of all the ndarrays in the python array:
             to_sum = min(chunk_size, n_segments - samples_done)
             segment_sub_range = samples_done, samples_done + to_sum
             sub_spectrograms = [s[:, slice(*segment_sub_range)] for s in spectrograms]
             # Write the sum into the first spectrum array to conserve memory:
             chunk_data_target = spectrograms[0][:, samples_done:samples_done + to_sum]
             np.sum(sub_spectrograms, axis=0, out=chunk_data_target)
             samples_done += to_sum
 
-        # np.sum(spectrograms, axis=0, out=combined_spectrogram)  # Sum across all axes. Hungry on memory.
-
         # return combined_spectrogram
-        return frequencies, spectrograms[0]
+        return frequency_buckets, spectrograms[0], (channels_available, channel_used)
+
+    @staticmethod
+    def _do_standard_spectrogram(data: np.ndarray, channel: int,
+                                 sample_rate: int, window_type: str, nfft: int, overlap: int,
+                                 prune_data: bool = False):
+        """
+        Create a standard windowed spectrogram.
+        """
+
+        channel_data = data[channel, :]
+        frequency_buckets, time_buckets, stft_power = chunky_spectrogram(
+            np.single,
+            channel_data, fs=sample_rate,
+            window=window_type,
+            nperseg=nfft,
+            noverlap=overlap,
+            nfft=None,
+            # detrend=False, # Defaults to constant.
+            return_onesided=True,
+            scaling='density',  # So that power dB is independent of window size. Power per Hz.
+            axis=-1,
+            mode='psd')  # psd to square the data to get power.
+
+        return stft_power, frequency_buckets, time_buckets
+
+    @staticmethod
+    def _do_reassignment_spectrogram(data: np.ndarray, channel: int,
+                                     sample_rate: int, window_type: str, nfft: int, nfft_overlap: int,
+                                     prune_data: bool = False):
+        """
+        Create a reassigned spectrum using Nelson's method, with optional pruning.
+
+        In fact the pruning is not useful - reducing the noise significantly would also eliminate FM
+        parts of bat chirps.
+
+        References:
+            Various methods with algorithms: http://www.acousticslab.org/learnmoresra/files/fulopfitz2006jasa119.pdf
+            When to use what window: https://download.ni.com/evaluation/pxi/Understanding%20FFTs%20and%20Windowing.pdf
+            Despeckling: http://www.acousticslab.org/learnmoresra/files/fitzfulop2006dsp.pdf
+            Someone's implementation of Nelson's method: https://github.com/bzamecnik/tfr/tree/master/tfr
+            Reference on Nelson's method, similar to the paper above: https://www.researchgate.net/publication/251405072_The_Reassigned_Spectrogram
+        """
+
+        # Slight hack: we discard a single data value so that the data and delayed data arrays
+        # are the same length:
+        channel_data = data[channel, 1:-1]
+        channel_data_delayed = data[channel, :-2]
+
+        def spectrogram(d: np.ndarray):
+            """Handy function to avoid repeating the long argument list below."""
+            return chunky_spectrogram(
+                np.csingle,
+                d, fs=sample_rate,
+                window=window_type,
+                nperseg=nfft,
+                noverlap=nfft_overlap,
+                nfft=None,
+                # detrend=False, # Defaults to constant.
+                return_onesided=True,
+                scaling='density',
+                # So that power dB is independent of window size.
+                # Power per Hz.
+                axis=-1,
+                mode='complex')  # psd to square the data to get power.
+
+        # Needed for pruning:
+        stft_del, stft_freq_del = None, None
+
+        # print("spectrogram of {} points".format(len(d)))
+        # t1 = process_time()
+        frequency_buckets, time_buckets, stft = spectrogram(channel_data)
+        _, _, stft_1 = spectrogram(
+            channel_data_delayed)  # stft_del. Intentionally generic variable name, we will repurpose it.
+
+        # TODO: handle case where the window is padded. In Nelson, win_size is padded to fftn, and they are the same
+        # if there is no padding. Some constants below need adjusting for the padded case.
+
+        # Nelson's method of reassignment, used below, has fairly simple maths and avoids any need
+        # to do fiddly phase unwrapping.
+
+        # We use del to signal which data we are done with so the garbage collector can reused the
+        # storage as required.
+
+        window_width = nfft / sample_rate
+        half_window_width = window_width / 2.0
+
+        if prune_data:
+            stft_del = stft_1.copy()
+
+        # Calculate the channelized instantaneous frequency:
+        # stft_1 is STFTDel at this point.
+        stft_1 = stft * np.conjugate(stft_1)  # In place. cross_spectrum_matrix_1, overwriting stft_del.
+        k1 = sample_rate / (2 * np.pi)
+        stft_1 = k1 * np.angle(stft_1)  # In place, overwriting cross_spectrum_matrix_1.
+        cif = stft_1.view()
+
+        # Calculate the local group delay. These are offset to be relative to the centre of the
+        # sfft window.
+        # Create a copy of the transform that is rotated up/to the right by one frequency:
+        stft_2 = np.roll(stft, 1, axis=0)  # !!! storage allocation. stft_freq_del.
+        if prune_data:
+            stft_freq_del = stft_2.copy()
+        stft_2 = stft * np.conjugate(stft_2)  # In place. Overwrite STFTfreqdel stft_freq_del cross_spectrum_matrix_1.
+        k2 = window_width / (2 * np.pi)
+        angle = np.angle(stft_2)  # !!! storage allocation
+        del stft_2
+
+        # Change the range of the angle from -pi/+pi to 0/2pi, to avoid splitting the same signal
+        # into two parts:
+        angle[angle < 0] += 2 * np.pi  # In place, no storage allocation.
+        # Time adjustment in seconds:
+        angle = half_window_width - k2 * angle  # In place
+        lgd = angle.view()
+        del angle
+
+        cif_deriv: Optional[np.ndarray] = None
+        if prune_data:
+            stft_freq_time_del = np.roll(stft_del, 1, axis=0)  # !!! storage allocation.
+            mix_cif = stft * np.conjugate(stft_del) * np.conjugate((stft_freq_del * np.conjugate(stft_freq_time_del)))
+            angle = np.angle(mix_cif)
+            # Remap the data angle range to 0 to 2 pi:
+            angle[angle < 0] += 2 * np.pi  # In place, no storage allocation.
+            k3 = sample_rate / (2 * np.pi)
+            cif_deriv = k3 * (angle ** 2)
+
+        # Calculate power from complex value. Avoid the sqrt() that abs() would imply for performance.
+        stft = stft.real ** 2 + stft.imag ** 2  # In place: Overwright stft with its squared magnitude.
+
+        # Use the cif and lgd data to move the values into different frequency buckets:
+        reassigned_stft_power = SpectrogramFftStep._reassign(stft, cif, lgd, frequency_buckets, time_buckets)
+        del stft
+
+        if cif_deriv is not None:
+            # Prune data values by setting them to zero depending on the coindexed value in the second derivative:
+            # print("min = {}, max = {}".format(cif_deriv.min(), cif_deriv.max()))
+            threshold: float = 10.0
+            reassigned_stft_power[cif_deriv > threshold] = 0  # Zero out the data we don't want.
+
+        return reassigned_stft_power, frequency_buckets, time_buckets
+
+    @staticmethod
+    def _reassign(data: np.ndarray, cif: np.ndarray, lgd: np.ndarray, frequency_buckets: np.ndarrary,
+                  time_buckets: np.ndarrary):
+
+        data_num_freqs, data_num_times = data.shape
+
+        # Construct bucket bin edges limits centred on each nominal freqency or time:
+        df = frequency_buckets[1] - frequency_buckets[0]
+        frequency_bucket_edges = np.append(frequency_buckets, frequency_buckets[-1] + df) - df / 2
+        dt = time_buckets[2] - time_buckets[1]
+        time_bucket_edges = np.append(time_buckets, time_buckets[-1] + dt) - dt / 2
+
+        resultant_times = time_buckets.reshape((1, data_num_times))
+        resultant_times = np.repeat(resultant_times, data_num_freqs, 0)
+        resultant_times = resultant_times + lgd  # lgd is delta to apply to the nominal time.
+
+        shape = data.shape
+        reassigned_data, _, _ = np.histogram2d(
+            cif.flatten(), resultant_times.flatten(),  # Flatten the reassigned data into two vectors.
+            bins=(frequency_bucket_edges, time_bucket_edges),  # Corresponding bucket edges for each dimensions.
+            weights=data.flatten())  # The data.
+        reassigned_data.reshape(shape)
+        return reassigned_data
+
+    @staticmethod
+    def _reassign_old(data: np.ndarray, cif: np.ndarray, nominal_frequencies: np.ndarrary):
+        # Construct frequency bucket bin edges limits centred on each nominal freqency:
+        df = nominal_frequencies[1] - nominal_frequencies[0]
+        bucket_edges = np.append(nominal_frequencies, nominal_frequencies[-1] + df) - df / 2
+
+        # We will work one column at a time, so need to transpose the data:
+        transposed_data = np.transpose(data)
+        transposed_cif = np.transpose(cif)
+
+        for t in range(transposed_data.shape[0]):
+            data_col = transposed_data[t]
+            cif_col = transposed_cif[t]
+
+            # Discard distant reassigments, these are likely to be noise.
+            max_reassignment = 5
+            target_buckets = np.where(np.abs(cif_col - nominal_frequencies) < df * max_reassignment, cif_col, 0)
+            # target_buckets = cif_col
+
+            # Map the reassigned buckets to the nominal frequency buckets, weighted by
+            # the reassigned signal intensity:
+            reassigned_col, _ = np.histogram(target_buckets, bins=bucket_edges, weights=data_col)
+
+            # Hack - add in a fraction of the original signal+noise:
+            # reassigned_col = np.where(reassigned_col == 0.0, data_col / 10.0, reassigned_col)
+
+            # Copy the reassigned column back to the original data array:
+            transposed_data[t, :] = reassigned_col
+
+        # Transpose back once we have finished:
+        data = np.transpose(transposed_data)
 
 
 class SpectrogramZoomStep(PipelineStep):
     """Zoom the data in or out to match the number of pixels we went to fill in the display."""
 
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
@@ -1234,15 +1460,15 @@
 
         params = filedata_serial, request.raw_data_reader, calc_data.first_time_index_for_segs, \
             calc_data.last_time_index_for_segs, appsettings.instance.serial_number
         (rawdata, raw_data_offset), raw_data_serial, _ = self._data_reader_step.process_data(
             None, params)
 
         params = raw_data_serial, sample_rate, sample_count, request.axis_time_range, \
-            calc_data.actual_fft_samples, calc_data.actual_fft_overlap_samples, calc_data.actual_fft_overlap_percent, \
+            calc_data.actual_window_samples, calc_data.actual_window_overlap_samples, calc_data.actual_window_overlap_percent, \
             request.is_reference
         (specdata, self._graph_params), specdata_serial, spectrogram_serial = \
             self._spectrogram_step.process_data((rawdata, raw_data_offset), params)
 
         del rawdata  # Allow the gc to reclaim this memory.
 
         params = raw_data_serial, height, width, request.axis_time_range, request.axis_frequency_range, \
```

### Comparing `batogram-1.0.9/batogram/rootwindow.py` & `batogram-1.1.0/batogram/rootwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     spectrogram: Optional[SpectrogramPipeline]
     profile: Optional[ProfilePipeline]
 
 
 class PanelFrame(tk.Frame):
     """This is a Frame which contains the set of graphs relating to the main or the reference data."""
 
-    def __init__(self, parent, root, pipelines, data_context, settings, settings_frame, pad, is_reference):
+    def __init__(self, parent, root, pipelines: GraphPipelines, data_context, settings, settings_frame, pad, is_reference):
         super().__init__(parent)
 
         self._pipelines = pipelines
         self._dc = data_context
         self._settings = settings
         self._settings_frame = settings_frame
 
@@ -787,20 +787,24 @@
 
     def _show_about(self):
         window = AboutWindow(self)
         window.grab_set()
         window.wait_window()
 
     def _show_settings(self):
-        modal = AppSettingsWindow(self, appsettings.instance, lambda: self._on_settings_ok())
+        previous_data_directory = appsettings.instance.data_directory
+        modal = AppSettingsWindow(self, appsettings.instance, lambda: self._on_settings_ok(previous_data_directory))
         modal.grab_set()
         modal.wait_window()
 
-    def _on_settings_ok(self):
+    def _on_settings_ok(self, previous_data_directory: str):
         # Refresh some things from the updated settings values:
+        if previous_data_directory != appsettings.instance.data_directory:
+            # Force the new data directory to be used when next opening the a file:
+            self._first_file_open = True
         self._apply_settings()
         self._main_pane.draw()
         self._ref_pane.draw()
 
     @staticmethod
     def _apply_settings():
         # Refresh some things from the updated settings values:
```

### Comparing `batogram-1.0.9/batogram/spectrogramgraphframe.py` & `batogram-1.1.0/batogram/spectrogramgraphframe.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 from typing import Tuple, Optional
 
-from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, AXIS_FONT_HEIGHT, MIN_F_RANGE, MIN_T_RANGE, \
+from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, MIN_F_RANGE, MIN_T_RANGE, \
     AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import RawDataReader, AudioFileService
-from .common import AxisRange, clip_to_range
+from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
-from .markers import TimeMarkerPair, FrequencyMarkerPair
-from .spectrogrammouseservice import SpectrogramMouseService, CursorMode
+from .markers import TimeMarkerPair, FrequencyMarkerPair, AbstractMarkerPair
+from .spectrogrammouseservice import SpectrogramMouseService, CursorMode, DragMode
 from .rendering import SpectrogramPipelineRequest
 from .moreframe import HistogramInterface
 
 
 class SpectrogramCanvas(tk.Canvas):
     """A Canvas containing a spectrogram."""
 
@@ -47,14 +47,63 @@
     def notify_draw_complete(self):
         self._mouse_service.notify_draw_complete()
 
     def preempt_mouse(self, preempt: bool):
         self._mouse_service.preempt_mouse(preempt)
 
 
+class RightMouseMenu(tk.Menu):
+    def __init__(self, parent: "SpectrogramGraphFrame", screen_end_pos: Tuple[int, int],
+                 canvas_end_pos: Tuple[int, int], region: Tuple[int, int, int, int],
+                 settings: "GraphSettings", drag_mode: DragMode):
+        super().__init__(parent, tearoff=0)
+
+        self._screen_pos = screen_end_pos
+
+        # If drag mode is undefined, a point was clicked:
+        is_region: bool = True if drag_mode else False
+
+        region_option_state = tk.ACTIVE if is_region else tk.DISABLED
+        position_option_state = tk.DISABLED if is_region else tk.ACTIVE
+
+        # Submenu for placing markers:
+        placement_menu = tk.Menu(self, tearoff=0)
+
+        # Adding Menu Items
+        self.add_command(label="Zoom to region", state=region_option_state,
+                         command=lambda: parent.on_zoom_to_rect(region))
+        self.add_command(label="Centre on position", state=position_option_state,
+                         # Centering is special case of zooming about centre:
+                         command=lambda: parent.on_zoom_about_centre(canvas_end_pos, 1.0, False))
+        self.add_command(label="Mark selected region", state=region_option_state,
+                         command=lambda: parent.mark_region(region, drag_mode))
+        self.add_cascade(label="Place...", menu=placement_menu)
+        placement_menu.add_command(label="left marker", state=position_option_state,
+                                   command=lambda: parent.on_place_left_marker(canvas_end_pos))
+        placement_menu.add_command(label="top marker", state=position_option_state,
+                                   command=lambda: parent.on_place_top_marker(canvas_end_pos))
+        placement_menu.add_command(label="right marker", state=position_option_state,
+                                   command=lambda: parent.on_place_right_marker(canvas_end_pos))
+        placement_menu.add_command(label="bottom marker", state=position_option_state,
+                                   command=lambda: parent.on_place_bottom_marker(canvas_end_pos))
+        self.add_command(label="Hide markers",
+                         state=tk.ACTIVE if (
+                                                    settings.show_time_markers or settings.show_frequency_markers) and not is_region else tk.DISABLED,
+                         command=lambda: parent.on_hide_markers())
+        self.add_command(label="Close menu")
+
+    def show(self):
+        try:
+            # Locate relative to the entire screen:
+            self.tk_popup(*self._screen_pos, 0)  # Locate menu entry zero at the point provided.
+        finally:
+            # Release the grab
+            self.grab_release()
+
+
 class SpectrogramGraphFrame(GraphFrame):
     """A graph frame containing a spectrogram."""
 
     def __init__(self, parent: "PanelFrame", root, pipeline, data_context, settings, initial_cursor_mode, is_reference):
         super().__init__(parent, root, pipeline, data_context, settings)
 
         self._is_reference = is_reference
@@ -71,16 +120,17 @@
         self._scroller_f = None
 
         self._parent = parent
 
         # Optional time marker pair, depends whether the user has enabled time markers or not:
         self._time_marker_pair: Optional[TimeMarkerPair] = None
         self._frequency_marker_pair: Optional[FrequencyMarkerPair] = None
-        # self._time_marker_pair: Optional[TimeMarkerPair] = TimeMarkerPair(self._canvas, self, 0.2, 0.4)
-        # self._frequency_marker_pair: Optional[FrequencyMarkerPair] = FrequencyMarkerPair(self._canvas, self, 20000, 50000)
+        # Any pending marker positions to be applied:
+        self._pending_time_marker_positions: Tuple[Optional[float], Optional[float]] = None, None
+        self._pending_frequency_marker_positions: Tuple[Optional[float], Optional[float]] = None, None
 
         self.bind("<Configure>", self._on_canvas_change)
         self.bind(MAIN_SPECTROGAM_COMPLETER_EVENT, self._do_completer)
 
     def set_histogram_interface(self, interface: HistogramInterface):
         self._histogram_interface = interface
 
@@ -173,33 +223,79 @@
 
         # Allow the screen update to happen:
         self.update_idletasks()
 
         self._canvas.notify_draw_complete()
 
     def _show_hide_markers(self, time_range: AxisRange, frequency_range: AxisRange):
-        """Create or destory markers depending on the settings."""
+        """Create or destroy markers depending on the settings."""
 
         if self._settings.show_time_markers:
-            if self._time_marker_pair is None:
-                # Create a marker pair that is visible in the current time scale:
-                delta = time_range.max - time_range.min
-                self._time_marker_pair = TimeMarkerPair(self._canvas, self,
-                                                        time_range.min + delta / 3, time_range.max - delta / 3)
+            self._time_marker_pair = self._create_or_update_marker(axis_range=time_range,
+                                                                   marker_pair=self._time_marker_pair,
+                                                                   pending_marker_positions=self._pending_time_marker_positions,
+                                                                   marker_class=TimeMarkerPair)
         else:
             self._time_marker_pair = None
+        self._pending_time_marker_positions = None, None  # We've consumed any pending values now.
 
         if self._settings.show_frequency_markers:
-            if self._frequency_marker_pair is None:
-                # Create a marker pair that is visible in the current frequency scale:
-                delta = frequency_range.max - frequency_range.min
-                self._frequency_marker_pair = FrequencyMarkerPair(self._canvas, self,
-                                                                  frequency_range.min + delta / 3, frequency_range.max - delta / 3)
+            self._frequency_marker_pair = self._create_or_update_marker(axis_range=frequency_range,
+                                                                        marker_pair=self._frequency_marker_pair,
+                                                                        pending_marker_positions=self._pending_frequency_marker_positions,
+                                                                        marker_class=FrequencyMarkerPair)
         else:
             self._frequency_marker_pair = None
+        self._pending_frequency_marker_positions = None, None  # We've consumed any pending values now.
+
+    def _create_or_update_marker(self, marker_pair: AbstractMarkerPair, axis_range: AxisRange,
+                                 pending_marker_positions: Tuple[Optional[float], Optional[float]],
+                                 marker_class) -> AbstractMarkerPair:
+        if marker_pair is None:
+            # Default positions are visible in the current scaling:
+            delta = axis_range.max - axis_range.min
+            # Handle the case where a marker is placed the wrong side of the other marker.
+            # We need to adjust the marker that is *not* currently being placed.
+            min_value, max_value = self._adjust_marker_range(
+                (axis_range.min + delta / 3, axis_range.max - delta / 3),
+                pending_marker_positions, axis_range)
+            marker_pair = marker_class(self._canvas, self, min_value, max_value)
+        else:
+            existing_min, existing_max = marker_pair.get_positions()
+            min_value, max_value = self._adjust_marker_range((
+                existing_min, existing_max),
+                pending_marker_positions, axis_range)
+            marker_pair.set_positions((min_value, max_value))
+
+        return marker_pair
+
+    @staticmethod
+    def _adjust_marker_range(existing_range: Tuple[float, float],
+                             pending_marker_positions: Tuple[Optional[float], Optional[float]],
+                             axis_range: AxisRange) -> Tuple[float, float]:
+        """Create a suitable range for markers, respecting:
+            * Update one marker, leaving the other at its existing position.
+            * However, if that leaves them in the wrong order, move the other marker.
+        """
+
+        resulting_min, resulting_max = existing_range
+        if pending_marker_positions[0] is not None:
+            # We are placing the lower marker.
+            resulting_min = pending_marker_positions[0]
+        if pending_marker_positions[1] is not None:
+            # We are placing the upper marker.
+            resulting_max = pending_marker_positions[1]
+
+        # Keep min and max in the right order:
+        if resulting_max <= resulting_min:
+            resulting_max = (resulting_min + axis_range.max) / 2
+        if resulting_min >= resulting_max:
+            resulting_min = (resulting_max + axis_range.min) / 2
+
+        return resulting_min, resulting_max
 
     def set_cursor_mode(self, mode):
         if mode == CursorMode.CURSOR_ZOOM:
             self._canvas.config(cursor="cross")
         elif mode == CursorMode.CURSOR_PAN:
             self._canvas.config(cursor="fleur")
         else:
@@ -492,7 +588,66 @@
         width, height = self.get_canvas_size()
         dt, df = delta(self._dc.time_range), delta(self._dc.frequency_range)
         window_factor = (height * dt) / (width * df)
 
         pixels_per_second = width / dt
 
         return window_factor, pixels_per_second
+
+    def do_mouse_menu(self, end_pos: Tuple[int, int],
+                      region: Tuple[int, int, int, int],
+                      drag_mode: DragMode):
+        end_screen_pos = self._canvas.winfo_rootx() + end_pos[0], self._canvas.winfo_rooty() + end_pos[1]
+        menu = RightMouseMenu(self, end_screen_pos, end_pos, region, self._settings, drag_mode)
+        menu.show()
+
+    def on_place_left_marker(self, canvas_pos: Tuple[int, int]):
+        self._settings.show_time_markers = True
+        self._settings.on_app_modified_settings()
+        axis_time, _ = self._layout.canvas_to_axis(canvas_pos)
+        self._pending_time_marker_positions = axis_time, None
+        self.draw()
+
+    def on_place_right_marker(self, canvas_pos: Tuple[int, int]):
+        self._settings.show_time_markers = True
+        self._settings.on_app_modified_settings()
+        axis_time, _ = self._layout.canvas_to_axis(canvas_pos)
+        self._pending_time_marker_positions = None, axis_time
+        self.draw()
+
+    def on_place_top_marker(self, canvas_pos: Tuple[int, int]):
+        self._settings.show_frequency_markers = True
+        self._settings.on_app_modified_settings()
+        _, axis_frequency = self._layout.canvas_to_axis(canvas_pos)
+        self._pending_frequency_marker_positions = None, axis_frequency
+        self.draw()
+
+    def on_place_bottom_marker(self, canvas_pos: Tuple[int, int]):
+        self._settings.show_frequency_markers = True
+        self._settings.on_app_modified_settings()
+        _, axis_frequency = self._layout.canvas_to_axis(canvas_pos)
+        self._pending_frequency_marker_positions = axis_frequency, None
+        self.draw()
+
+    def on_hide_markers(self):
+        self._settings.show_time_markers = False
+        self._settings.show_frequency_markers = False
+        self._settings.on_app_modified_settings()
+        self.draw()
+
+    def mark_region(self, region: Tuple[int, int, int, int], drag_mode: DragMode):
+        # Convert the drag region pixels to axis values:
+        top_left = region[0], region[1]
+        bottom_right = region[2], region[3]
+        t1, f1 = self._layout.canvas_to_axis(top_left)
+        t2, f2 = self._layout.canvas_to_axis(bottom_right)
+
+        if drag_mode == DragMode.DRAG_HORIZONTAL or drag_mode == DragMode.DRAG_RECTANGLE:
+            self._settings.show_time_markers = True
+            self._pending_time_marker_positions = t1, t2
+
+        if drag_mode == DragMode.DRAG_VERTICAL or drag_mode == DragMode.DRAG_RECTANGLE:
+            self._settings.show_frequency_markers = True
+            self._pending_frequency_marker_positions = f2, f1  # Axis value ordering is oppostie to pixel value ordering.
+
+        self._settings.on_app_modified_settings()
+        self.draw()
```

### Comparing `batogram-1.0.9/batogram/spectrogrammouseservice.py` & `batogram-1.1.0/batogram/spectrogrammouseservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,31 @@
     DRAG_HORIZONTAL = 0
     DRAG_VERTICAL = 1
     DRAG_RECTANGLE = 2
 
 
 class MouseState(Enum):
     START = 1
-    LEFT_DRAGGING = 2
+    LEFTRIGHT_DRAGGING = 2
     MIDDLE_DRAGGING = 3
 
 
 class SpectrogramMouseService:
     """This class provides mouse behaviour for the spectrogram."""
 
     # Zoom factor per mouse wheel click:
     _ZOOM_FACTOR = 0.60
 
     # Wheel clicks within this number of seconds will be considered
     # to be part of the same zoom operation, and only recentre initially.
     _WHEEL_TIMEOUT = 1.0
 
-    def __init__(self, canvas: tk.Canvas, initial_cursor_mode, graph_frame):
+    def __init__(self, canvas: tk.Canvas, initial_cursor_mode, graph_frame: "SpectrogramGraphFrame"):
         self._cursor_mode = initial_cursor_mode
-        self._graph_frame = graph_frame
+        self._graph_frame: "SpectrogramGraphFrame" = graph_frame
         self._canvas = canvas
 
         self._state: MouseState = MouseState.START
         self._start_position = None
         self._rect = None
         self._line = None
         self._line1 = None
@@ -88,16 +88,19 @@
         canvas.bind('<ButtonRelease-2>', self._on_button2_release)
         canvas.bind('<Shift-ButtonRelease-2>', self._on_shift_button2_release)
         canvas.bind('<B2-Motion>', self._on_button2_move)
         canvas.bind('<Shift-B2-Motion>', self._on_shift_button2_move)
 
         # Right mouse button:
         canvas.bind('<ButtonPress-3>', self._on_button3_press)
+        canvas.bind('<Shift-ButtonPress-3>', self._on_button3_press)
         canvas.bind('<ButtonRelease-3>', self._on_button3_release)
+        canvas.bind('<Shift-ButtonRelease-3>', self._on_shift_button3_release)
         canvas.bind('<B3-Motion>', self._on_button3_move)
+        canvas.bind('<Shift-B3-Motion>', self._on_shift_button3_move)
 
         # Any mouse motion:
         canvas.bind('<Motion>', self._on_move)
         canvas.bind('<Leave>', self._on_leave)
 
         # Mouse wheel:
         self._bind_wheel()
@@ -108,51 +111,80 @@
 
     def _on_button1_press(self, event):
         # print("1+")
         if self._preempted:
             return
 
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_press(event)
+            self._on_select_press(event)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_press(event)
 
     def _on_button1_move(self, event):
         # print("SpectrogramMouseService._on_button1_move")
         if self._preempted:
             return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_move(event, is_shift=False)
+            self._on_select_move(event, is_shift=False)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_move(event, is_shift=False)
 
     def _on_shift_button1_move(self, event):
         if self._preempted:
             return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_move(event, is_shift=True)
+            self._on_select_move(event, is_shift=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_move(event, is_shift=True)
 
     def _on_button1_release(self, event):
         if self._preempted:
             return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_release(event, is_shift=False)
+            self._on_select_release(event, is_shift=False, is_button1=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_release(event, is_shift=False)
 
     def _on_shift_button1_release(self, event):
         if self._preempted:
             return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_release(event, is_shift=True)
+            self._on_select_release(event, is_shift=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_release(event, is_shift=True)
 
+    def _on_button3_press(self, event):
+        # print("3+")
+        if self._preempted:
+            return
+
+        self._on_select_press(event)
+
+    def _on_button3_move(self, event):
+        # print("SpectrogramMouseService._on_button3_move")
+        if self._preempted:
+            return
+        self._on_select_move(event, is_shift=False)
+
+    def _on_shift_button3_move(self, event):
+        if self._preempted:
+            return
+        self._on_select_move(event, is_shift=True)
+
+    def _on_button3_release(self, event):
+        # print("3-")
+        pos = event.x, event.y
+        self._on_select_release(event, is_shift=False, is_button1=False)
+
+    def _on_shift_button3_release(self, event):
+        # print("SpectrogramMouseService._on_shift_button3_release")
+        if self._preempted:
+            return
+        self._on_select_release(event, is_shift=True)
+
     def _on_button2_press(self, event):
         # print("2+")
         self._on_pan_press(event)
 
     def _on_button2_release(self, event):
         # print("2-")
         self._on_pan_release(event, is_shift=False)
@@ -165,26 +197,14 @@
         # print("B2 move")
         self._on_pan_move(event, is_shift=False)
 
     def _on_shift_button2_move(self, event):
         # print("B2 move")
         self._on_pan_move(event, is_shift=True)
 
-    def _on_button3_press(self, _):
-        # print("3+")
-        if self._state == MouseState.LEFT_DRAGGING:
-            self._reset()
-
-    def _on_button3_release(self, event):
-        # print("3-")
-        pass
-
-    def _on_button3_move(self, event):
-        pass
-
     def _on_wheel(self, event):
         # print("wheel {}".format(event))
         if event.delta > 0:
             self._wheel_action(event, self._ZOOM_FACTOR, frequency_clamped=False)
         else:
             self._wheel_action(event, 1.0 / self._ZOOM_FACTOR, frequency_clamped=False)
 
@@ -232,15 +252,16 @@
         self._canvas.bind('<Shift-Button-4>', self._on_shift_wheel_up)
         self._canvas.bind('<Button-5>', self._on_wheel_down)
         self._canvas.bind('<Shift-Button-5>', self._on_shift_wheel_down)
         # For Windows:
         self._canvas.bind("<MouseWheel>", self._on_wheel)
         self._canvas.bind("<Shift-MouseWheel>", self._on_shift_wheel)
 
-    def _on_zoom_drag_complete(self, start: Tuple[int, int], end: Tuple[int, int], mode: DragMode):
+    def _on_select_drag_complete(self, start: Tuple[int, int], end: Tuple[int, int],
+                                 mode: DragMode, is_button1: bool):
         """
         * Coordinates provided are relative to the top left corner of the canvas.
         * "start" and "end" are not in any particular order.
         * Coordinates may be outside the range of the canvas, if the drag moves off the edge.
         """
         # print("rectangle selected: {}, {}".format(start, end))
 
@@ -254,32 +275,41 @@
         if mode == DragMode.DRAG_HORIZONTAL:
             t, b = 0, self._canvas_height
         elif mode == DragMode.DRAG_VERTICAL:
             l, r = 0, self._canvas_width
         elif mode == DragMode.DRAG_RECTANGLE:
             pass
 
-    # Notify whoever it concerns that they need to rescale to the area selected:
-        self._graph_frame.on_zoom_to_rect((l, t, r, b))
+        region = l, t, r, b
+
+        if is_button1:
+            # If a significant area was selected:
+            if mode:
+                # Notify whoever it concerns that they need to rescale to the area selected:
+                self._graph_frame.on_zoom_to_rect((l, t, r, b))
+        else:
+            # Display a menu of options:
+            self._graph_frame.do_mouse_menu(end, region, mode)
+            pass
 
     def _reset(self):
         self._state = MouseState.START
         self._start_position = None
         self._last_drag_mode = None
         self._delete_canvas_items()
 
-    def _on_zoom_press(self, event):
+    def _on_select_press(self, event):
         self._reset()
         self._canvas_height = self._canvas.winfo_height()
         self._canvas_width = self._canvas.winfo_width()
-        self._state = MouseState.LEFT_DRAGGING
+        self._state = MouseState.LEFTRIGHT_DRAGGING
         self._start_position = event.x, event.y
 
-    def _on_zoom_move(self, event, is_shift: bool):
-        if self._state == MouseState.LEFT_DRAGGING:
+    def _on_select_move(self, event, is_shift: bool):
+        if self._state == MouseState.LEFTRIGHT_DRAGGING:
             # If this is not the first move event, we need to delete the previous rectangle we drew:
             self._delete_canvas_items()
             mode: DragMode = self._get_drag_mode(event, is_shift)
             if mode is not None:
                 if mode == DragMode.DRAG_HORIZONTAL:
                     self._line1 = self._canvas.create_line(
                         self._start_position[0], 0, self._start_position[0], self._canvas_height,
@@ -294,23 +324,21 @@
                     self._line2 = self._canvas.create_line(
                         0, event.y, self._canvas_width, event.y,
                         fill=DRAG_RECTANGLE_COLOUR)
                 elif mode == DragMode.DRAG_RECTANGLE:
                     self._rect = self._canvas.create_rectangle(*self._start_position, event.x, event.y,
                                                                outline=DRAG_RECTANGLE_COLOUR)
 
-    def _on_zoom_release(self, event, is_shift: bool):
+    def _on_select_release(self, event, is_shift: bool, is_button1: bool):
         self._delete_canvas_items()
-        if self._state == MouseState.LEFT_DRAGGING:
+        if self._state == MouseState.LEFTRIGHT_DRAGGING:
             self._state = MouseState.START
             end = event.x, event.y
-            if self._start_position != end:
-                mode = self._get_drag_mode(event, is_shift)
-                if mode is not None:
-                    self._on_zoom_drag_complete(self._start_position, end, mode)
+            mode = self._get_drag_mode(event, is_shift)
+            self._on_select_drag_complete(self._start_position, end, mode, is_button1)
 
             self._start_position = None
 
     def _on_pan_press(self, event):
         self._reset()
         self._state = MouseState.MIDDLE_DRAGGING
         self._start_position = event.x, event.y
```

### Comparing `batogram-1.0.9/batogram/validatingwidgets.py` & `batogram-1.1.0/batogram/validatingwidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 result_msg = "Unable to parse field value {}".format(s)
 
             if self._vem_value_validator:
                 error_msg = self._vem_value_validator(value)
                 if error_msg:
                     result_msg = error_msg
         finally:
-            # As a side effect, highlight and focus the entruy:
+            # As a side effect, highlight and focus the entry:
             self._set_validity(result_msg is None)
             self.update_status()
             self.focus_set()
             return result_msg
 
     def get_value(self):
         native = self._vem_variable.get()
@@ -222,14 +222,29 @@
         return np.format_float_positional(value / self._scaler, precision=self._decimal_places, fractional=True, trim='-')
 
     def native_to_value(self, native):
         """This can throw ValueError, though won't if the field validation regex is right"""
         return float(native) * self._scaler
 
 
+class IntegerValidatingEntry(AbstractValidatingEntry):
+    """Oven ready validating entry for integer data"""
+    def __init__(self, parent, controlling_frame, container, width, value_validator=None):
+        AbstractValidatingEntry.__init__(self, parent, controlling_frame, container, width, validate='key',
+                                         validatecommand=(parent.validatecommand_integer, '%V', '%P'),
+                                         value_validator=value_validator)
+
+    def value_to_native(self, value):
+        return str(value)
+
+    def native_to_value(self, native):
+        """This can throw ValueError, though won't if the field validation regex is right"""
+        return int(native)
+
+
 class ValidatingCheckbutton(tk.Checkbutton, AbstractValidatingWidgetMixin):
     """Oven ready validating entry for check boxes"""
 
     def __init__(self, parent, controlling_frame, container, text, value_validator=None):
         variable = tk.IntVar()
         tk.Checkbutton.__init__(self, parent, text=text, variable=variable)
         AbstractValidatingWidgetMixin.__init__(self, parent, controlling_frame, container, variable, value_validator)
@@ -354,26 +369,32 @@
     def value_to_native(self, value):
         return self._dictionary[value]
 
 
 class ValidatingFrameHelper:
     """A handy helper for any frame containing validating widgets"""
     _RE_FLOAT = re.compile(r'[+-]?[0-9]*\.?[0-9]*')
+    _RE_INTEGER = re.compile(r'[0-9]*')
 
     def __init__(self, parent, settings):
         self._vfm_parent = parent
         self._vfm_settings = settings
         self.validatecommand_float = self.register(self.float_or_empty_entry_validator)
+        self.validatecommand_integer = self.register(self.integer_or_empty_entry_validator)
 
     def float_or_empty_entry_validator(self, action, p):
         result = self._RE_FLOAT.fullmatch(p)
         return True if result is not None else False
 
+    def integer_or_empty_entry_validator(self, action, p):
+        result = self._RE_INTEGER.fullmatch(p)
+        return True if result is not None else False
+
     @staticmethod
-    def double_value_validator(v: float, minimum_value=None, maximum_value=None, minimum_entry=None, message=None):
+    def generic_value_validator(v: Any, minimum_value=None, maximum_value=None, minimum_entry=None, message=None):
         if minimum_value is not None:
             if v < minimum_value:
                 return message if message is not None else "Value must be greater than {}".format(minimum_value)
 
         if maximum_value is not None:
             if v > maximum_value:
                 return message if message is not None else "Value must be less than {}".format(maximum_value)
```

### Comparing `batogram-1.0.9/batogram/wavfileparser.py` & `batogram-1.1.0/batogram/wavfileparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import io
 import numpy as np
 
 from dataclasses import dataclass
 from typing import List, Callable, Any, Tuple, Optional
 from .external.guano import GuanoFile
 
-
 class WavFileError(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, *kwargs)
 
 
 class WavFileParser:
     """A parser for wav files. It's simplest to implement our own, as off the shelf
@@ -155,14 +154,17 @@
         #   00000050  4d 4d 4d 4d 4d 4d 4d 00  64 61 74 61 40 47 4c 00  |MMMMMMM.data@GL.|
 
         excess_data = chunk_size - required_chunk_size
         if excess_data > 0:
             print("Discarding {} excess bytes from the end of fmt".format(excess_data))
             self._f.read(excess_data)
 
+        if self._is_odd(chunk_size):
+            self._read_int8("padding")      # Allow for padding 0 byte if the chunk is an odd length. Actually, it isn't.
+
         return WavFileParser.Header(num_channels=num_channels, sample_rate_hz=sample_rate_hz,
                                     bits_per_sample=bits_per_sample)
 
     def _skim_data(self, header: Header) -> Optional[Data]:
         """Process the data chunk without storing any of the data."""
 
         data_byte_count = self._read_int32("ChunkSize")
@@ -196,16 +198,18 @@
                 break   # Hit the end prematurely.
 
         # Sometimes headers are wrong, because they are written in advance of the data.
         # Note the actual sample count. This is what we will use.
         actual_sample_count: int = samples_read
 
         # We have been seeking around in the file to read data, so we need
-        # to seek to the end of data chunk now to not confused the caller:
+        # to seek to the end of data chunk now to not confuse the caller:
         self._f.seek(self._start_of_data + data_byte_count)
+        if self._is_odd(data_byte_count):
+            self._read_int8("padding")      # Allow for padding 0 byte if the chunk is an odd length.
 
         return WavFileParser.Data(actual_sample_count=actual_sample_count,
                                   data_range=(min_value, max_value),
                                   data_byte_count=data_byte_count)
 
     def read_data(self, index_range: Tuple[int, int]) -> Tuple[Optional[np.ndarray], int]:
         """Read the request range of data (half open), and return the data and actual count read."""
@@ -242,34 +246,46 @@
         # guesses the length to write up front, then the actual length is defined by the
         # amount of data in the file.
 
         if self._fmt_header.num_channels > 1:
             actual_samples_read = int(actual_values_read / self._fmt_header.num_channels)
             data = data.reshape((actual_samples_read, self._fmt_header.num_channels))
 
+        if self._is_odd(actual_samples_read * bytes_per_sample):
+            self._read_int8("padding")      # Allow for padding 0 byte if the chunk is an odd length.
+
         return data, actual_samples_read
 
     def _read_guan(self) -> Optional[GuanoFile]:
         # https://www.wildlifeacoustics.com/SCHEMA/GUANO.html
         # https://github.com/riggsd/guano-py/blob/master/guano.py
 
         chunk_size_bytes = self._read_int32("ChunkSize")
         metadata = self._f.read(chunk_size_bytes)
-        gf = GuanoFile.from_string(metadata)
+        try:
+            gf = GuanoFile.from_string(metadata, strict=False)
+        except Exception as e:
+            # Fail open if the guano is bad:
+            print("Exception raised parsing guano data: {}".format(e))
 
         # for key, value in gf.items():
         #    print('{}: {}'.format(key, value))
 
+        if self._is_odd(chunk_size_bytes):
+            self._read_int8("padding")      # Allow for padding 0 byte if the chunk is an odd length.
+
         return gf
 
     def _skip_chunk(self):
         """Consume and ignore an entire chunk, assuming the chunk id has already been read."""
-        chunk_size = self._read_int32("ChunkSize")
+        bytes_to_skip = self._read_int32("ChunkSize")
+        if self._is_odd(bytes_to_skip):
+            bytes_to_skip += 1      # Allow for padding 0 byte if the chunk is an odd length.
         t = self._f.tell()
-        self._f.seek(t + chunk_size)
+        self._f.seek(t + bytes_to_skip)
 
     def _check_value(self, fieldname: str, value, check: Callable, text: str):
         if not check(value):
             raise WavFileError("Unexpected value for {} in {}: found {}: {}"
                                .format(fieldname, self._filepath, value, text))
 
     def _read_int32(self, fieldname: str, expected: Optional[int] = None) -> int:
@@ -284,14 +300,26 @@
         b = self._f.read(2)
         n = int.from_bytes(b, byteorder='little')
         if expected is not None and n != expected:
             raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
                                .format(fieldname, self._filepath, n, expected))
         return n
 
+    def _read_int8(self, fieldname: str, expected: Optional[int] = None) -> int:
+        b = self._f.read(1)
+        n = int.from_bytes(b, byteorder='little')
+        if expected is not None and n != expected:
+            raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
+                               .format(fieldname, self._filepath, n, expected))
+        return n
+
     def _read_text_bytes(self, length, fieldname, expected: Optional[bytes] = None) -> List[bytes]:
         b = self._f.read(length)
         if expected is not None and b != expected:
             raise WavFileError("Unexpected value for {} in {}: found {}, expected {}"
                                .format(fieldname, self._filepath, b, expected))
 
         return b
+
+    @staticmethod
+    def _is_odd(i: int) -> bool:
+        return i & 1
```

### Comparing `batogram-1.0.9/batogram.egg-info/PKG-INFO` & `batogram-1.1.0/batogram.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.9
+Version: 1.1.0
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,16 +46,17 @@
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
 * Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
 * Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
+* Support for reassignment spectrograms for increased resolution.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, Linux and macOS (experimental) operating systems.
+* Runs on Windows, Linux operating systems, maybe macOS.
 
 Installation
 ------------
 
 ### Windows
 
 There are currently two approaches to installing Batogram on Windows. The first and simplest
```

### Comparing `batogram-1.0.9/batogram.egg-info/SOURCES.txt` & `batogram-1.1.0/batogram.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 batogram/graphsettings.py
 batogram/historianservice.py
 batogram/layouts.py
 batogram/markers.py
 batogram/modalwindow.py
 batogram/morebncframe.py
 batogram/moreframe.py
+batogram/moreotherframe.py
 batogram/morerenderingframe.py
 batogram/morescaleframe.py
 batogram/profilegraphframe.py
 batogram/readoutframe.py
 batogram/rendering.py
 batogram/rootwindow.py
 batogram/runner.py
```

### Comparing `batogram-1.0.9/pyproject.toml` & `batogram-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "batogram"
-version = "1.0.9"   # Set this to the version number during release, and revert to 0.0.0 between releases.
+version = "1.1.0"   # Set this to the version number during release, and revert to 0.0.0 between releases.
 authors = [
     {name = "John Mears", email = "john+batogram@themears.co.uk"},
 ]
 description = "Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["bat", "spectrogram", "chiropterology", "fourier", "ultrasonic", "ultrasound", "echo", "GUANO"]
```

