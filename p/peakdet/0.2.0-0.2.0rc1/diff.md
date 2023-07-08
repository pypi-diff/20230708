# Comparing `tmp/peakdet-0.2.0.tar.gz` & `tmp/peakdet-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakdet-0.2.0.tar", last modified: Sat Jul  8 00:23:20 2023, max compression
+gzip compressed data, was "dist/peakdet-0.2.0rc1.tar", last modified: Fri Sep 18 09:38:24 2020, max compression
```

## Comparing `peakdet-0.2.0.tar` & `peakdet-0.2.0rc1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.936616 peakdet-0.2.0/
--rw-r--r--   0 nemo      (1000) nemo      (1000)    11357 2020-10-05 08:30:05.000000 peakdet-0.2.0/LICENSE
--rw-r--r--   0 nemo      (1000) nemo      (1000)       65 2020-10-05 08:30:05.000000 peakdet-0.2.0/MANIFEST.in
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     7926 2023-07-08 00:23:20.936616 peakdet-0.2.0/PKG-INFO
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     6895 2023-07-08 00:07:58.000000 peakdet-0.2.0/README.md
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     3199 2020-10-16 09:29:15.000000 peakdet-0.2.0/README.rst
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.936616 peakdet-0.2.0/peakdet/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      748 2020-10-16 09:29:15.000000 peakdet-0.2.0/peakdet/__init__.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      497 2023-07-08 00:23:20.936616 peakdet-0.2.0/peakdet/_version.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     4395 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/analytics.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.928616 peakdet-0.2.0/peakdet/cli/
--rw-r--r--   0 nemo      (1000) nemo      (1000)        0 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/cli/__init__.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     9927 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/cli/run.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     7131 2023-07-08 00:21:15.000000 peakdet-0.2.0/peakdet/editor.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     1568 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/external.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     6818 2022-11-21 10:26:04.000000 peakdet-0.2.0/peakdet/io.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     1321 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/modalities.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     8619 2023-07-08 00:21:15.000000 peakdet-0.2.0/peakdet/operations.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     7525 2023-07-08 00:21:15.000000 peakdet-0.2.0/peakdet/physio.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.932616 peakdet-0.2.0/peakdet/tests/
--rw-r--r--   0 nemo      (1000) nemo      (1000)       85 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/__init__.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.932616 peakdet-0.2.0/peakdet/tests/data/
--rw-r--r--   0 nemo      (1000) nemo      (1000)   386488 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/ECG.csv
--rw-r--r--   0 nemo      (1000) nemo      (1000)   117398 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/ECG.phys
--rw-r--r--   0 nemo      (1000) nemo      (1000)   110335 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/PPG.csv
--rw-r--r--   0 nemo      (1000) nemo      (1000)   143967 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/RESP.csv
--rw-r--r--   0 nemo      (1000) nemo      (1000)       28 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/header.csv
--rw-r--r--   0 nemo      (1000) nemo      (1000)      176 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/history.json
--rw-r--r--   0 nemo      (1000) nemo      (1000)     2087 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/data/rtpeaks.csv
--rw-r--r--   0 nemo      (1000) nemo      (1000)      428 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_analytics.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)      954 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_editor.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)      683 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_external.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     3236 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_io.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     3484 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_operations.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     2928 2023-01-13 16:17:22.000000 peakdet-0.2.0/peakdet/tests/test_physio.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     2927 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/test_utils.py
--rw-r--r--   0 nemo      (1000) nemo      (1000)     1302 2020-10-05 08:30:05.000000 peakdet-0.2.0/peakdet/tests/utils.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     7388 2023-07-08 00:21:15.000000 peakdet-0.2.0/peakdet/utils.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-07-08 00:23:20.928616 peakdet-0.2.0/peakdet.egg-info/
--rw-r--r--   0 nemo      (1000) nemo      (1000)     7926 2023-07-08 00:23:20.000000 peakdet-0.2.0/peakdet.egg-info/PKG-INFO
--rw-r--r--   0 nemo      (1000) nemo      (1000)      937 2023-07-08 00:23:20.000000 peakdet-0.2.0/peakdet.egg-info/SOURCES.txt
--rw-r--r--   0 nemo      (1000) nemo      (1000)        1 2023-07-08 00:23:20.000000 peakdet-0.2.0/peakdet.egg-info/dependency_links.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)        1 2022-07-26 13:14:57.000000 peakdet-0.2.0/peakdet.egg-info/not-zip-safe
--rw-r--r--   0 nemo      (1000) nemo      (1000)      428 2023-07-08 00:23:20.000000 peakdet-0.2.0/peakdet.egg-info/requires.txt
--rw-r--r--   0 nemo      (1000) nemo      (1000)        8 2023-07-08 00:23:20.000000 peakdet-0.2.0/peakdet.egg-info/top_level.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     1947 2023-07-08 00:23:20.936616 peakdet-0.2.0/setup.cfg
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      374 2023-01-13 16:17:22.000000 peakdet-0.2.0/setup.py
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)    11357 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/LICENSE
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)       65 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/MANIFEST.in
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     4375 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/PKG-INFO
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     3199 2020-09-17 17:22:46.000000 peakdet-0.2.0rc1/README.rst
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      748 2020-09-18 08:22:59.000000 peakdet-0.2.0rc1/peakdet/__init__.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      501 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet/_version.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     4395 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/analytics.py
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet/cli/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)        0 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/cli/__init__.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     9927 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/cli/run.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     4862 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/editor.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     1568 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/external.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     1051 2020-09-18 09:34:29.000000 peakdet-0.2.0rc1/peakdet/info.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     6818 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/io.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     1321 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/modalities.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     7343 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/operations.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     3967 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/physio.py
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet/tests/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)       85 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/__init__.py
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet/tests/data/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)   386488 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/ECG.csv
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)   117398 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/tests/data/ECG.phys
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)   110335 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/PPG.csv
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)   143967 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/RESP.csv
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)       28 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/header.csv
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      176 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/history.json
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     2087 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/data/rtpeaks.csv
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      428 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/test_analytics.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      954 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/tests/test_editor.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      683 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/test_external.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     3236 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/tests/test_io.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     3484 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/tests/test_operations.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     2062 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/test_physio.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     2927 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/tests/test_utils.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     1302 2019-07-19 18:49:32.000000 peakdet-0.2.0rc1/peakdet/tests/utils.py
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     6490 2020-09-17 15:44:46.000000 peakdet-0.2.0rc1/peakdet/utils.py
+drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/peakdet.egg-info/
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     4375 2020-09-18 09:38:24.000000 peakdet-0.2.0rc1/peakdet.egg-info/PKG-INFO
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      913 2020-09-18 09:38:24.000000 peakdet-0.2.0rc1/peakdet.egg-info/SOURCES.txt
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)        1 2020-09-18 09:38:24.000000 peakdet-0.2.0rc1/peakdet.egg-info/dependency_links.txt
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      164 2020-09-18 09:38:24.000000 peakdet-0.2.0rc1/peakdet.egg-info/requires.txt
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)        8 2020-09-18 09:38:24.000000 peakdet-0.2.0rc1/peakdet.egg-info/top_level.txt
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)      344 2020-09-18 09:38:24.165721 peakdet-0.2.0rc1/setup.cfg
+-rw-rw-r--   0 nemo      (1000) nemo      (1000)     1485 2020-09-18 09:34:52.000000 peakdet-0.2.0rc1/setup.py
```

### Comparing `peakdet-0.2.0/LICENSE` & `peakdet-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/README.rst` & `peakdet-0.2.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/__init__.py` & `peakdet-0.2.0rc1/peakdet/__init__.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/analytics.py` & `peakdet-0.2.0rc1/peakdet/analytics.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/cli/run.py` & `peakdet-0.2.0rc1/peakdet/cli/run.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/editor.py` & `peakdet-0.2.0rc1/peakdet/editor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,115 @@
 # -*- coding: utf-8 -*-
-"""Functions and class for performing interactive editing of physiological data."""
+"""
+Functions and class for performing interactive editing of physiological data
+"""
 
 import functools
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.widgets import SpanSelector
 from peakdet import operations, utils
 
 
 class _PhysioEditor():
     """
-    Class for editing physiological data.
+    Class for editing physiological data
 
     Parameters
     ----------
     data : Physio_like
         Physiological data to be edited
     """
 
     def __init__(self, data):
         # save reference to data and generate "time" for interpretable X-axis
         self.data = utils.check_physio(data, copy=True)
         fs = 1 if data.fs is None else data.fs
         self.time = np.arange(0, len(data.data) / fs, 1 / fs)
-        # Read if there is support data
-        self.suppdata = data.suppdata
 
         # we need to create these variables in case someone doesn't "quit"
         # the plot appropriately (i.e., clicks X instead of pressing ctrl+q)
-        self.deleted, self.rejected, self.included = set(), set(), set()
-
-        # make main plot objects depending on supplementary data
-        if self.suppdata is None:
-            self.fig, self._ax = plt.subplots(nrows=1, ncols=1,
-                                              tight_layout=True, sharex=True)
-        else:
-            self.fig, self._ax = plt.subplots(nrows=2, ncols=1,
-                                              tight_layout=True, sharex=True,
-                                              gridspec_kw={'height_ratios': [3, 2]})
+        self.deleted, self.rejected = set(), set()
 
+        # make main plot objects
+        self.fig, self.ax = plt.subplots(nrows=1, ncols=1, tight_layout=True)
         self.fig.canvas.mpl_connect('scroll_event', self.on_wheel)
         self.fig.canvas.mpl_connect('key_press_event', self.on_key)
 
-        # Set axis handler
-        self.ax = self._ax if self.suppdata is None else self._ax[0]
-
-        # three selectors for:
-        #    1. rejection (central mouse),
-        #    2. addition (right mouse), and
-        #    3. deletion (left mouse)
-        delete = functools.partial(self.on_edit, method='delete')
-        reject = functools.partial(self.on_edit, method='reject')
-        insert = functools.partial(self.on_edit, method='insert')
-        self.span2 = SpanSelector(self.ax, delete, 'horizontal',
+        # two selectors for rejection (left mouse) and deletion (right mouse)
+        reject = functools.partial(self.on_remove, reject=True)
+        delete = functools.partial(self.on_remove, reject=False)
+        self.span1 = SpanSelector(self.ax, reject, 'horizontal',
                                   button=1, useblit=True,
                                   rectprops=dict(facecolor='red', alpha=0.3))
-        self.span1 = SpanSelector(self.ax, reject, 'horizontal',
-                                  button=2, useblit=True,
-                                  rectprops=dict(facecolor='blue', alpha=0.3))
-        self.span3 = SpanSelector(self.ax, insert, 'horizontal',
+        self.span2 = SpanSelector(self.ax, delete, 'horizontal',
                                   button=3, useblit=True,
-                                  rectprops=dict(facecolor='green', alpha=0.3))
+                                  rectprops=dict(facecolor='blue', alpha=0.3))
 
         self.plot_signals(False)
 
     def plot_signals(self, plot=True):
-        """Clear axes and plots data / peaks / troughs."""
+        """ Clears axes and plots data / peaks / troughs """
         # don't reset x-/y-axis zooms on replot
         if plot:
             xlim, ylim = self.ax.get_xlim(), self.ax.get_ylim()
         else:
             xlim, ylim = (-5, None), (None, None)
 
         # clear old data + redraw, retaining x-/y-axis zooms
         self.ax.clear()
         self.ax.plot(self.time, self.data, 'b',
                      self.time[self.data.peaks],
                      self.data[self.data.peaks], '.r',
                      self.time[self.data.troughs],
                      self.data[self.data.troughs], '.g')
-
-        if self.suppdata is not None:
-            self._ax[1].plot(self.time, self.suppdata, 'k', linewidth=0.7)
-            self._ax[1].set_ylim(-.5, .5)
-
         self.ax.set(xlim=xlim, ylim=ylim, yticklabels='')
         self.fig.canvas.draw()
 
     def on_wheel(self, event):
-        """Move axis on wheel scroll."""
+        """ Moves axis on wheel scroll """
         (xlo, xhi), move = self.ax.get_xlim(), event.step * -10
         self.ax.set_xlim(xlo + move, xhi + move)
         self.fig.canvas.draw()
 
     def quit(self):
-        """Quit editor."""
+        """ Quits editor """
         plt.close(self.fig)
 
     def on_key(self, event):
-        """Undo last span select or quits peak editor."""
+        """ Undoes last span select or quits peak editor """
         # accept both control or Mac command key as selector
         if event.key in ['ctrl+z', 'super+d']:
             self.undo()
         elif event.key in ['ctrl+q', 'super+d']:
             self.quit()
 
-    def on_edit(self, xmin, xmax, *, method):
-        """
-        Edit peaks by rejection, deletion, or insert.
-
-        Removes specified peaks by either rejection / deletion, OR
-        Include one peak by finding the max in the selection.
-
-        method accepts 'insert', 'reject', 'delete'
-        """
-        if method not in ['insert', 'reject', 'delete']:
-            raise ValueError(f'Action "{method}" not supported.')
-
+    def on_remove(self, xmin, xmax, *, reject):
+        """ Removes specified peaks by either rejection / deletion """
         tmin, tmax = np.searchsorted(self.time, (xmin, xmax))
         pmin, pmax = np.searchsorted(self.data.peaks, (tmin, tmax))
+        bad = np.arange(pmin, pmax, dtype=int)
 
-        if method == 'insert':
-            tmp = np.argmax(self.data.data[tmin:tmax]) if tmin != tmax else 0
-            newpeak = tmin + tmp
-            if newpeak == tmin:
-                self.plot_signals()
-                return
-        else:
-            bad = np.arange(pmin, pmax, dtype=int)
-            if len(bad) == 0:
-                self.plot_signals()
-                return
+        if len(bad) == 0:
+            return
 
-        if method == 'reject':
+        if reject:
             rej, fcn = self.rejected, operations.reject_peaks
-        elif method == 'delete':
-            rej, fcn = self.deleted, operations.delete_peaks
-
-        # store edits in local history & call function
-        if method == 'insert':
-            self.included.add(newpeak)
-            self.data = operations.add_peaks(self.data, newpeak)
         else:
-            rej.update(self.data.peaks[bad].tolist())
-            self.data = fcn(self.data, self.data.peaks[bad])
+            rej, fcn = self.deleted, operations.delete_peaks
 
+        # store edits in local history
+        rej.update(self.data.peaks[bad].tolist())
+        self.data = fcn(self.data, self.data.peaks[bad])
         self.plot_signals()
 
     def undo(self):
-        """Reset last span select peak removal."""
+        """ Resets last span select peak removal """
         # check if last history entry was a manual reject / delete
-        relevant = ['reject_peaks', 'delete_peaks', 'add_peaks']
-        if self.data._history[-1][0] not in relevant:
+        if self.data._history[-1][0] not in ['reject_peaks', 'delete_peaks']:
             return
 
         # pop off last edit and delete
         func, peaks = self.data._history.pop()
 
         if func == 'reject_peaks':
             self.data._metadata['reject'] = np.setdiff1d(
@@ -165,17 +119,11 @@
         elif func == 'delete_peaks':
             self.data._metadata['peaks'] = np.insert(
                 self.data._metadata['peaks'],
                 np.searchsorted(self.data._metadata['peaks'], peaks['remove']),
                 peaks['remove']
             )
             self.deleted.difference_update(peaks['remove'])
-        elif func == 'add_peaks':
-            self.data._metadata['peaks'] = np.delete(
-                self.data._metadata['peaks'],
-                np.searchsorted(self.data._metadata['peaks'], peaks['add']),
-            )
-            self.included.remove(peaks['add'])
+
         self.data._metadata['troughs'] = utils.check_troughs(self.data,
-                                                             self.data.peaks,
-                                                             self.data.troughs)
+                                                             self.data.peaks)
         self.plot_signals()
```

### Comparing `peakdet-0.2.0/peakdet/external.py` & `peakdet-0.2.0rc1/peakdet/external.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/io.py` & `peakdet-0.2.0rc1/peakdet/io.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/modalities.py` & `peakdet-0.2.0rc1/peakdet/modalities.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/operations.py` & `peakdet-0.2.0rc1/peakdet/operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,19 +88,15 @@
 
     # generate original and target "time" series
     t_orig = np.linspace(0, len(data) / data.fs, len(data))
     t_new = np.linspace(0, len(data) / data.fs, int(len(data) * factor))
 
     # interpolate data and generate new Physio object
     interp = interpolate.interp1d(t_orig, data, kind=kind)(t_new)
-    if data.suppdata is None:
-        suppinterp = None
-    else:
-        suppinterp = interpolate.interp1d(t_orig, data.suppdata, kind=kind)(t_new)
-    interp = utils.new_physio_like(data, interp, fs=target_fs, suppdata=suppinterp)
+    interp = utils.new_physio_like(data, interp, fs=target_fs)
 
     return interp
 
 
 @utils.make_operation()
 def peakfind_physio(data, *, thresh=0.2, dist=None):
     """
@@ -155,15 +151,15 @@
     Returns
     -------
     data : Physio_like
     """
 
     data = utils.check_physio(data, ensure_fs=False, copy=True)
     data._metadata['peaks'] = np.setdiff1d(data._metadata['peaks'], remove)
-    data._metadata['troughs'] = utils.check_troughs(data, data.peaks, data.troughs)
+    data._metadata['troughs'] = utils.check_troughs(data, data.peaks)
 
     return data
 
 
 @utils.make_operation()
 def reject_peaks(data, remove):
     """
@@ -177,60 +173,14 @@
     Returns
     -------
     data : Physio_like
     """
 
     data = utils.check_physio(data, ensure_fs=False, copy=True)
     data._metadata['reject'] = np.append(data._metadata['reject'], remove)
-    data._metadata['troughs'] = utils.check_troughs(data, data.peaks, data.troughs)
-
-    return data
-
-
-@utils.make_operation()
-def add_peaks(data, add):
-    """
-    Add `newpeak` to add them in `data`
-
-    Parameters
-    ----------
-    data : Physio_like
-    add : int
-
-    Returns
-    -------
-    data : Physio_like
-    """
-
-    data = utils.check_physio(data, ensure_fs=False, copy=True)
-    idx = np.searchsorted(data._metadata['peaks'], add)
-    data._metadata['peaks'] = np.insert(data._metadata['peaks'], idx, add)
-    data._metadata['troughs'] = utils.check_troughs(data, data.peaks)
-
-    return data
-
-
-@utils.make_operation()
-def add_peaks(data, add):
-    """
-    Add `newpeak` to add them in `data`
-
-    Parameters
-    ----------
-    data : Physio_like
-    add : int
-
-    Returns
-    -------
-    data : Physio_like
-    """
-
-    data = utils.check_physio(data, ensure_fs=False, copy=True)
-    idx = np.searchsorted(data._metadata['peaks'], add)
-    data._metadata['peaks'] = np.insert(data._metadata['peaks'], idx, add)
     data._metadata['troughs'] = utils.check_troughs(data, data.peaks)
 
     return data
 
 
 def edit_physio(data):
     """
@@ -252,22 +202,21 @@
     # no point in manual edits if peaks/troughs aren't defined
     if not (len(data.peaks) and len(data.troughs)):
         return
 
     # perform manual editing
     edits = editor._PhysioEditor(data)
     plt.show(block=True)
+    delete, reject = sorted(edits.deleted), sorted(edits.rejected)
 
     # replay editing on original provided data object
-    if len(edits.rejected) > 0:
-        data = reject_peaks(data, remove=sorted(edits.rejected))
-    if len(edits.deleted) > 0:
-        data = delete_peaks(data, remove=sorted(edits.deleted))
-    if len(edits.included) > 0:
-        data = add_peaks(data, add=sorted(edits.included))
+    if reject is not None:
+        data = reject_peaks(data, remove=reject)
+    if delete is not None:
+        data = delete_peaks(data, remove=delete)
 
     return data
 
 
 def plot_physio(data, *, ax=None):
     """
     Plots `data` and associated peaks / troughs
```

### Comparing `peakdet-0.2.0/peakdet/tests/data/ECG.csv` & `peakdet-0.2.0rc1/peakdet/tests/data/ECG.csv`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/data/ECG.phys` & `peakdet-0.2.0rc1/peakdet/tests/data/ECG.phys`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/data/PPG.csv` & `peakdet-0.2.0rc1/peakdet/tests/data/PPG.csv`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/data/RESP.csv` & `peakdet-0.2.0rc1/peakdet/tests/data/RESP.csv`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/data/rtpeaks.csv` & `peakdet-0.2.0rc1/peakdet/tests/data/rtpeaks.csv`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/test_editor.py` & `peakdet-0.2.0rc1/peakdet/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/test_external.py` & `peakdet-0.2.0rc1/peakdet/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/test_io.py` & `peakdet-0.2.0rc1/peakdet/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/test_operations.py` & `peakdet-0.2.0rc1/peakdet/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/test_utils.py` & `peakdet-0.2.0rc1/peakdet/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/tests/utils.py` & `peakdet-0.2.0rc1/peakdet/tests/utils.py`

 * *Files identical despite different names*

### Comparing `peakdet-0.2.0/peakdet/utils.py` & `peakdet-0.2.0rc1/peakdet/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,91 +137,74 @@
     if not isinstance(data, physio.Physio):
         data = load_physio(data)
     if ensure_fs and np.isnan(data.fs):
         raise ValueError('Provided data does not have valid sampling rate.')
     if copy is True:
         return new_physio_like(data, data.data,
                                copy_history=True,
-                               copy_metadata=True,
-                               copy_suppdata=True)
+                               copy_metadata=True)
     return data
 
 
-def new_physio_like(ref_physio, data, *, fs=None, suppdata=None, dtype=None,
-                    copy_history=True, copy_metadata=True, copy_suppdata=True):
+def new_physio_like(ref_physio, data, *, fs=None, dtype=None,
+                    copy_history=True, copy_metadata=True):
     """
     Makes `data` into physio object like `ref_data`
 
     Parameters
     ----------
     ref_physio : Physio_like
         Reference `Physio` object
     data : array_like
         Input physiological data
     fs : float, optional
         Sampling rate of `data`. If not supplied, assumed to be the same as
         in `ref_physio`
-    suppdata : array_like, optional
-        New supplementary data. If not supplied, assumed to be the same.
     dtype : data_type, optional
         Data type to convert `data` to, if conversion needed. Default: None
     copy_history : bool, optional
         Copy history from `ref_physio` to new physio object. Default: True
-    copy_metadata : bool, optional
-        Copy metadata from `ref_physio` to new physio object. Default: True
-    copy_suppdata : bool, optional
-        Copy suppdata from `ref_physio` to new physio object. Default: True
 
     Returns
     -------
     data : peakdet.Physio
         Loaded physio object with provided `data`
     """
 
     if fs is None:
         fs = ref_physio.fs
     if dtype is None:
         dtype = ref_physio.data.dtype
     history = list(ref_physio.history) if copy_history else []
     metadata = dict(**ref_physio._metadata) if copy_metadata else None
 
-    if suppdata is None:
-        suppdata = ref_physio._suppdata if copy_suppdata else None
-
     # make new class
     out = ref_physio.__class__(np.array(data, dtype=dtype),
-                               fs=fs, history=history, metadata=metadata,
-                               suppdata=suppdata)
+                               fs=fs, history=history, metadata=metadata)
     return out
 
 
-def check_troughs(data, peaks, troughs=None):
+def check_troughs(data, peaks):
     """
     Confirms that `troughs` exists between every set of `peaks` in `data`
 
     Parameters
     ----------
     data : array-like
         Input data for which `troughs` and `peaks` were detected
     peaks : array-like
         Indices of suspected peak locations in `data`
-    troughs : array-like or None, optional
-        Indices of suspected troughs locations in `data`, if any.
 
     Returns
     -------
     troughs : np.ndarray
         Indices of trough locations in `data`, dependent on `peaks`
     """
-    # If there's a through after all peaks, keep it.
-    if troughs is not None and troughs[-1] > peaks[-1]:
-        all_troughs = np.zeros(peaks.size, dtype=int)
-        all_troughs[-1] == troughs[-1]
-    else:
-        all_troughs = np.zeros(peaks.size - 1, dtype=int)
+
+    all_troughs = np.zeros(peaks.size - 1, dtype=int)
 
     for f in range(peaks.size - 1):
         dp = data[peaks[f]:peaks[f + 1]]
         idx = peaks[f] + np.argwhere(dp == dp.min())[0]
         all_troughs[f] = idx
 
     return all_troughs
```

### Comparing `peakdet-0.2.0/peakdet.egg-info/SOURCES.txt` & `peakdet-0.2.0rc1/peakdet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 LICENSE
 MANIFEST.in
-README.md
 README.rst
 setup.cfg
 setup.py
 peakdet/__init__.py
 peakdet/_version.py
 peakdet/analytics.py
 peakdet/editor.py
 peakdet/external.py
+peakdet/info.py
 peakdet/io.py
 peakdet/modalities.py
 peakdet/operations.py
 peakdet/physio.py
 peakdet/utils.py
 peakdet.egg-info/PKG-INFO
 peakdet.egg-info/SOURCES.txt
 peakdet.egg-info/dependency_links.txt
-peakdet.egg-info/not-zip-safe
 peakdet.egg-info/requires.txt
 peakdet.egg-info/top_level.txt
 peakdet/cli/__init__.py
 peakdet/cli/run.py
 peakdet/tests/__init__.py
 peakdet/tests/test_analytics.py
 peakdet/tests/test_editor.py
```

