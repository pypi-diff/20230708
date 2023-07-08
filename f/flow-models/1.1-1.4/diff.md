# Comparing `tmp/flow_models-1.1.tar.gz` & `tmp/flow_models-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flow_models-1.1.tar", last modified: Fri Jan 15 23:24:08 2021, max compression
+gzip compressed data, was "flow_models-1.4.tar", last modified: Sat Jul  8 21:36:00 2023, max compression
```

## Comparing `flow_models-1.1.tar` & `flow_models-1.4.tar`

### file list

```diff
@@ -1,30 +1,43 @@
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2021-01-15 23:24:08.812473 flow_models-1.1/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     3700 2021-01-15 23:24:08.812473 flow_models-1.1/PKG-INFO
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     4082 2021-01-08 03:11:47.000000 flow_models-1.1/README.md
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2021-01-15 23:24:08.812473 flow_models-1.1/flow_models/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)       20 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/__init__.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     1440 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/convert.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)    14525 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/fit.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     4328 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/generate.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     4322 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/hist.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     7978 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/hist_np.py
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2021-01-15 23:24:08.812473 flow_models-1.1/flow_models/lib/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)        0 2021-01-08 03:11:47.000000 flow_models-1.1/flow_models/lib/__init__.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     4266 2021-01-08 03:11:47.000000 flow_models-1.1/flow_models/lib/data.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)    11669 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/lib/io.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     9841 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/lib/kde.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     3905 2021-01-08 03:11:47.000000 flow_models-1.1/flow_models/lib/mix.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     9944 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/lib/plot.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     1689 2021-01-08 03:11:47.000000 flow_models-1.1/flow_models/lib/util.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     5973 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/merge.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     4259 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/plot.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     3796 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/sort.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     3709 2021-01-15 23:21:37.000000 flow_models-1.1/flow_models/summary.py
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2021-01-15 23:24:08.812473 flow_models-1.1/flow_models.egg-info/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     3700 2021-01-15 23:24:08.000000 flow_models-1.1/flow_models.egg-info/PKG-INFO
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)      581 2021-01-15 23:24:08.000000 flow_models-1.1/flow_models.egg-info/SOURCES.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)        1 2021-01-15 23:24:08.000000 flow_models-1.1/flow_models.egg-info/dependency_links.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)      414 2021-01-15 23:24:08.000000 flow_models-1.1/flow_models.egg-info/entry_points.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)       12 2021-01-15 23:24:08.000000 flow_models-1.1/flow_models.egg-info/top_level.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)       38 2021-01-15 23:24:08.812473 flow_models-1.1/setup.cfg
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     1935 2021-01-15 23:21:37.000000 flow_models-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 21:35:51.000000 flow_models-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 21:36:00.638553 flow_models-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 21:35:51.000000 flow_models-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.634554 flow_models-1.4/flow_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/cut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/elephants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/first_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/first_mirror/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/hist_np.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/cryptopan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23462 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/series_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:36:00.638553 flow_models-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-08 21:35:51.000000 flow_models-1.4/setup.py
```

### Comparing `flow_models-1.1/PKG-INFO` & `flow_models-1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: flow_models
-Version: 1.1
+Version: 1.4
 Summary: A framework for analysis and modeling of IP network flows
 Home-page: https://github.com/piotrjurkiewicz/flow-models
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
-Description: # flow-models: A framework for analysis and modeling of IP network flows
-        
-        Packages like `flow-tools` or `nfdump` provide tools for filtering and calculating simple summary/top-N statistics
-        from network flow records. They lack, however, any capabilities for analysis and modeling of flow features (length,
-        size, duration, rate, etc.) distributions. The goal of this framework is to fill this gap.
-        
-        `flow-models` is a software framework for creating precise and reproducible statistical flow models from
-        NetFlow/IPFIX flow records. It can be used to merge split records, calculate histograms of flow features and create
-        General Mixture Models fitting them. Created models can be used both as an input in analytical calculations and to
-        generate realistic traffic in simulations.
-        
-        The framework can be installed from [Python Package Index (PyPI)](https://pypi.org/project/flow-models/) using the
-        following command:
-        
-            pip install flow-models
-        
-        A detailed documentation, including usage examples, is available at: https://flow-models.readthedocs.io
-        
-        Apart from the framework, the Git repository also contains a library of flow models created with it, including
-        histograms and fitted mixture models.
-        
-        ## Provided tools
-        
-        The framework currently includes the following tools:
-        
-        - `merge` -- merges flows which were split across multiple records due to *active timeout*
-        - `sort` -- sorts flow records according to specified fields (requires `numpy`)
-        - `hist` -- calculates histograms of flows length, size, duration or rate
-        - `hist_np` -- calculates histograms using multiple threads (requires `numpy`, much faster, but uses more memory)
-        - `fit` -- creates General Mixture Models (GMM) fitted to flow records (requires `scipy`)
-        - `plot` -- generates plots from flow records and fitted models (requires `pandas` and `scipy`)
-        - `generate` -- generates flow records from histograms or mixture models
-        - `summary` -- produces TeX tables containing summary statistics of flow dataset (requires `scipy`)
-        - `convert` -- converts flow records between supported formats
-        
-        Following the Unix philosophy, each tool is a separate Python program aimed at a single purpose. Features provided
-        by the tools are orthogonal and they are tailored to be used sequentially in data-processing pipelines.
-        
-        ## Models library
-        
-        The repository of flow models, containing histogram CSV files, fitted mixture models and plots, is available at: https://github.com/piotrjurkiewicz/flow-models
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# flow-models: A framework for analysis and modeling of IP network flows
+
+Packages like `flow-tools` or `nfdump` provide tools for filtering and calculating simple summary/top-N statistics
+from network flow records. They lack, however, any capabilities for analysis and modeling of flow features (length,
+size, duration, rate, etc.) distributions. The goal of this framework is to fill this gap.
+
+`flow-models` is a software framework for creating precise and reproducible statistical flow models from
+NetFlow/IPFIX flow records. It can be used to merge split records, calculate histograms of flow features and create
+General Mixture Models fitting them. Created models can be used both as an input in analytical calculations and to
+generate realistic traffic in simulations.
+
+The framework can be installed from [Python Package Index (PyPI)](https://pypi.org/project/flow-models/) using the
+following command:
+
+    pip install flow-models
+
+A detailed documentation, including usage examples, is available at: https://flow-models.readthedocs.io
+
+Apart from the framework, the Git repository also contains a library of flow models created with it, including
+histograms and fitted mixture models.
+
+## Provided tools
+
+The framework currently includes the following tools:
+
+- `merge` -- merges flows which were split across multiple records due to *active timeout*
+- `sort` -- sorts flow records according to specified fields (requires `numpy`)
+- `hist` -- calculates histograms of flows length, size, duration or rate
+- `hist_np` -- calculates histograms using multiple threads (requires `numpy`, much faster, but uses more memory)
+- `fit` -- creates General Mixture Models (GMM) fitted to flow records (requires `scipy`)
+- `plot` -- generates plots from flow records and fitted models (requires `pandas` and `scipy`)
+- `generate` -- generates flow records from histograms or mixture models
+- `summary` -- produces TeX tables containing summary statistics of flow dataset (requires `scipy`)
+- `convert` -- converts flow records between supported formats
+
+Following the Unix philosophy, each tool is a separate Python program aimed at a single purpose. Features provided
+by the tools are orthogonal and they are tailored to be used sequentially in data-processing pipelines.
+
+## Models library
+
+The repository of flow models, containing histogram CSV files, fitted mixture models and plots, is available at: https://github.com/piotrjurkiewicz/flow-models
```

### Comparing `flow_models-1.1/README.md` & `flow_models-1.4/README.md`

 * *Files identical despite different names*

### Comparing `flow_models-1.1/flow_models/fit.py` & `flow_models-1.4/flow_models/fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,19 +162,43 @@
             ng += 1
     for n in range(lognorm_number):
         mix.append([0.1, 'lognorm', [2.0, 0, geom[ng]]])
         ng += 1
 
     return mix
 
-def fit(path, y_value, max_iter=100, initial=None, max_pareto_w=None, cb=None):
-    path = pathlib.Path(path)
-    logmsg(f'Processing: {path}')
+def fit(in_file, y_value, max_iter=100, initial=None, max_pareto_w=None, cb=None):
+    """
+    Fit distribution mixture to flow histogram.
+
+    Parameters
+    ----------
+    in_file : os.PathLike
+        input histogram file
+    y_value : str
+        y axis value
+    max_iter : int, default 100
+        maximum number of iterations
+    initial : dict, optional
+        initial mixture
+    max_pareto_w : float, optional
+        maximum pareto weight
+    cb : function, optional
+        callback function to call after each iteration
+
+    Returns
+    ------
+    dict
+        {'mix': result_mix, 'sum': np.sum(weights)}
+    """
 
-    data = pd.read_csv(path, index_col=0, sep=',', low_memory=False, usecols=lambda n: not n.endswith('_ssq'))
+    in_file = pathlib.Path(in_file)
+    logmsg(f'Processing: {in_file}')
+
+    data = pd.read_csv(in_file, index_col=0, sep=',', low_memory=False, usecols=lambda n: not n.endswith('_ssq'))
     x = data.index.values
     weights = data[f'{y_value}_sum'].values
 
     if isinstance(initial, dict):
         mix = initial_mix(initial, x)
     else:
         mix = json.load(open(str(initial)))
@@ -195,15 +219,15 @@
 
     fig, ax = plt.subplots(2, 2, figsize=(15, 10))
     ax = ax.flatten()
 
     rv = [{}]
 
     root = tkinter.Tk()
-    root.wm_title("flow-models-fit")
+    root.wm_title("flow_models.fit")
 
     style = tkinter.ttk.Style()
     style.theme_use('default')
     style.configure("black.Horizontal.TProgressbar", background='black')
 
     animate = tkinter.IntVar()
     y_var = tkinter.StringVar()
@@ -215,15 +239,15 @@
     toolbar = tkinter.Frame(master=root)
     toolbar.grid(row=10, column=0, sticky=W)
     toolbar = NavigationToolbar2Tk(canvas, toolbar)
     toolbar.update()
 
     dd = load_data([kwargs['path']])
     df = list(dd.values())[0]
-    idx = np.unique(np.rint(np.geomspace(df.index.min(), df.index.max(), LINE_NBINS)).astype(int))
+    idx = np.unique(np.rint(np.geomspace(df.index.min(), df.index.max(), LINE_NBINS)).astype(np.int64))
 
     first_plot = False
 
     def plot_data(*_):
         if not first_plot or y_var.get() and y_var.get() != kwargs['y_value']:
             if y_var.get():
                 kwargs['y_value'] = y_var.get()
@@ -386,15 +410,15 @@
 
     if mode:
         initial = mode
     else:
         initial = app_args.initial
 
     with measure_memory(app_args.measure_memory):
-        args = dict(path=app_args.file, y_value=app_args.y, max_iter=app_args.i, initial=initial, max_pareto_w=app_args.mpw)
+        args = dict(in_file=app_args.file, y_value=app_args.y, max_iter=app_args.i, initial=initial, max_pareto_w=app_args.mpw)
         if app_args.interactive:
             gui(**args)
         else:
             new_mix = fit(**args)
             save(pathlib.Path() / args['y_value'], new_mix, args)
```

### Comparing `flow_models-1.1/flow_models/hist_np.py` & `flow_models-1.4/flow_models/hist_np.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 #!/usr/bin/python3
 """
 Calculates histograms using multiple threads (requires `numpy`, much faster, but uses more memory).
 """
 
-import argparse
 import concurrent.futures
 import functools
 import os
 import pathlib
-import sys
 
 import numpy as np
 
-from .lib.io import load_array_np, write_line, write_none
+from .lib.io import write_line, write_none, IOArgumentParser, load_arrays, FILTER_HELP
 from .lib.util import logmsg, bin_calc_log, measure_memory
 
+EPILOG = \
+f"""
+Use this tool to calculate histogram of flow features.
+
+The output is a histogram of a selected feature in csv_hist format.
+
+Feature selection is being done with -x parameter. Additionally -b parameter can be
+specified, which will make histogram logarithmically binned to help reduce its size.
+
+{FILTER_HELP}
+
+Skipping of flow records can be done with skip_in and count_in parameters.
+They specify how many flow records should be skipped (skip_in) and then read (count_in)
+from input.
+
+Example: (calculates logarithmically binned histogram of flow length from the sorted directory)
+
+    flow_models.hist -i binary -x length -b 12 sorted
+"""
+
 # MAX_MEM = 64 * (1024 ** 3)
 MAX_MEM = os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES') // 4
 N_JOBS = 4
 
 X_VALUES = ['length', 'size']
 OUT_FORMATS = {'csv_hist': write_line, 'none': write_none}
 
@@ -29,26 +47,26 @@
         if 'duration' in mm:
             dur = mm['duration'][start:stop]
         else:
             dur = (mm['last'][start:stop] - mm['first'][start:stop]) * 1000
             dur += mm['last_ms'][start:stop]
             dur -= mm['first_ms'][start:stop]
             dur[mm['packets'][start:stop] == 1] = 0
-            if column == 'duration':
-                return dur
+        if column == 'duration':
+            return dur
         if column == 'rate':
-            rate = np.zeros(stop - start)
+            rate = np.zeros_like(dur, dtype=np.float64)
             np.divide(8000 * mm['octets'][start:stop], dur, out=rate, where=dur != 0)
             return rate
     else:
         raise ValueError(f'Cannot compute column: {column}')
 
-def calc_chunk(memory_maps, key_column, start, stop, columns, algorithm='bincount'):
+def calc_chunk(memory_maps, key_column, start, stop, columns, filtered=..., algorithm='bincount'):
     sums = {}
-    key_array = memory_maps[key_column][start:stop]
+    key_array = memory_maps[key_column][start:stop][filtered]
     max_key = key_array.max()
 
     if max_key * 8 < MAX_MEM:
         hist = np.bincount(key_array.view('q'))
         bins = np.nonzero(hist)[0]
         sums['flows'] = hist[bins]
     else:
@@ -58,62 +76,51 @@
 
     max_bin = bins.max()
     assert max_bin == max_key
     bins = bins.astype(np.min_scalar_type(max_bin))
 
     if algorithm == 'bincount':
         for column in columns:
-            hist = np.bincount(key_array.view('q'), get_column_array(memory_maps, column, start, stop))[bins]
+            hist = np.bincount(key_array.view('q'), get_column_array(memory_maps, column, start, stop)[filtered])[bins]
             sums[column] = hist
     elif algorithm == 'addat':
         assert len(key_array) < 2_147_483_648
         indices = np.searchsorted(bins, key_array)
         indices = indices.astype(np.min_scalar_type(len(bins)))
         for column in columns:
             hist = np.zeros(len(bins))
-            np.add.at(hist, indices, get_column_array(memory_maps, column, start, stop))
+            np.add.at(hist, indices, get_column_array(memory_maps, column, start, stop)[filtered])
             sums[column] = hist
         if 'flows' not in sums:
             hist = np.zeros(len(bins))
             np.add.at(hist, indices, 1)
             sums['flows'] = hist
     else:
         raise ValueError('Unknown algorithm', algorithm)
 
     return bins, sums
 
-def calc_dir(path,  x_value, columns):
+def calc_dir(path, x_value, columns, counters=None, filter_expr=None):
+
+    if counters is None:
+        counters = {'skip_in': 0, 'count_in': None, 'skip_out': 0, 'count_out': None}
 
     logmsg(f'Processing directory: {path}')
     assert path.is_dir()
 
     key_columns = {'length': 'packets',
                    'size': 'octets'}
     key_column = key_columns[x_value]
-    size = None
-    memory_maps = {}
 
-    for name in columns:
+    if 'duration' in columns or 'rate' in columns:
+        fields_to_load = columns + ['first', 'first_ms', 'last', 'last_ms']
+    else:
+        fields_to_load = columns
 
-        try:
-            name, dtype, in_mm = load_array_np(path / name, 'r')
-            assert name not in memory_maps
-            if size is None:
-                size = in_mm.size
-            else:
-                assert in_mm.size == size
-            memory_maps[name] = in_mm
-            logmsg(f'Loaded array: {path / name}')
-        except FileNotFoundError:
-            logmsg(f'Not found array: {path / name}, will try to compute this column')
-
-    if ('duration' in columns or 'rate' in columns) and 'duration' not in memory_maps:
-        for name in ['first', 'first_ms', 'last', 'last_ms']:
-            logmsg(f'Loading array: {path / name}')
-            memory_maps[name] = load_array_np(path / name, 'r')[2]
+    arrays, filtered, size = load_arrays(path, fields_to_load, counters, filter_expr, require_numpy=True)
 
     i = 0
     while True:
         i += 1
         chunk_size = size // i + 1
         if chunk_size * 8 < MAX_MEM / 2.2 and chunk_size // N_JOBS + 1 < 2_147_483_648:
             break
@@ -124,15 +131,15 @@
     logmsg(f'Calculating directory: {path} using {N_JOBS} workers in {i * N_JOBS} chunks')
 
     results = []
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=N_JOBS) as executor:
         futures = {}
         for start, stop in zip(starts, stops):
-            future = executor.submit(calc_chunk, memory_maps, key_column, start, stop, columns)
+            future = executor.submit(calc_chunk, arrays, key_column, start, stop, columns, filtered)
             futures[future] = start, stop
         for future in concurrent.futures.as_completed(futures):
             start, stop = futures[future]
             try:
                 result = future.result()
                 results.append(result)
             except Exception as exc:
@@ -141,59 +148,94 @@
             else:
                 logmsg(f'Done directory: {path} chunk: [{start}:{stop}]')
 
     logmsg(f'Done directory: {path} chunk: all')
 
     return results
 
-def histogram(in_files, out_file, in_format='binary', out_format='csv_hist', bin_exp=0, x_value='length', additional_columns=()):
+def hist(in_files, output, in_format='binary', out_format='csv_hist', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, bin_exp=0, x_value='length', additional_columns=()):
+    """
+    Calculates histograms of flows length, size, duration or rate.
+
+    Parameters
+    ----------
+    in_files : list[os.PathLike]
+        input files paths
+    output : os.PathLike | io.TextIOWrapper
+        output file or directory path or stream
+    in_format : str, default 'binary'
+        input format
+    out_format : str, default 'csv_hist'
+        output format
+    skip_in : int, default 0
+        number of flows to skip at the beginning of input
+    count_in : int, default None, meaning all flows
+        number of flows to read from input
+    skip_out : int, default 0
+        not supported
+    count_out : int, default None, meaning all flows
+        not supported
+    filter_expr : CodeType, optional
+        filter expression
+    bin_exp: int, default 0
+        bin width exponent of 2
+    x_value : str, default 'length'
+        x axis value
+    additional_columns : list[str], optional
+        additional column to sum
+    """
 
     assert in_format == 'binary'
+    if count_out is not None:
+        raise NotImplementedError
+    if skip_out != 0:
+        raise NotImplementedError
 
     if bin_exp == 0:
         bin_calc_fn = None
     else:
         bin_calc_fn = bin_calc_log
 
     writer = OUT_FORMATS[out_format]
     columns = ['packets', 'octets'] + additional_columns
 
     if isinstance(in_files, list):
         dirs = [pathlib.Path(f) for f in in_files]
     else:
-        dirs = [pathlib.Path(in_files)]
+        raise ValueError()
 
+    counters = {'skip_in': skip_in, 'count_in': count_in, 'skip_out': skip_out, 'count_out': count_out}
     results = []
 
     for d in dirs:
-        results += calc_dir(d, x_value, columns)
+        results += calc_dir(d, x_value, columns, counters, filter_expr)
 
     bins = functools.reduce(np.union1d, (bins for bins, _ in results))
     sums = {c: np.zeros(len(bins)) for c in ['flows'] + columns}
 
     for bn, data in results:
         indices = np.searchsorted(bins, bn)
         for c in sums:
             sums[c][indices] += data[c]
 
     header_line = 'bin_lo,bin_hi,'
     header_line += ','.join(c + '_sum' for c in sums)
 
     written = 0
 
-    writer = writer(out_file, header_line)
+    writer = writer(output, header_line)
     next(writer)
 
     if bin_calc_fn is None:
         for n, bin_lo in enumerate(bins):
             bin_lo = int(bin_lo)
             writer.send(f'{bin_lo},{bin_lo + 1},' + ','.join(str(int(float(s[n]))) for s in sums.values()))
             written += 1
     else:
-        bin_lo, bin_hi = bin_calc_fn(bins[0], bin_exp)
+        bin_lo, bin_hi = bin_calc_fn(bins.item(0), bin_exp)
         bin_sums = [0.0] * len(sums)
         for n, x in enumerate(bins):
             x = int(x)
             if x >= bin_hi:
                 writer.send(f'{bin_lo},{bin_hi},' + ','.join(str(int(float(s))) for s in bin_sums))
                 written += 1
                 bin_lo, bin_hi = bin_calc_fn(x, bin_exp)
@@ -204,27 +246,28 @@
         written += 1
 
     writer.close()
 
     logmsg(f'Finished all directories. Flows: NA Written: {written}')
 
 def parser():
-    p = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter, description=__doc__)
-    p.add_argument('files', nargs='+', help='input dirs')
-    p.add_argument('-i', default='binary', choices=['binary'], help='format of input files')
-    p.add_argument('-o', default='csv_hist', choices=['csv_hist'], help='format of output')
-    p.add_argument('-O', default=sys.stdout, help='file for output')
-    p.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
-    p.add_argument('-b', default=0, type=int, help='bin width exponent of 2')
-    p.add_argument('-c', action='append', default=[], help='additional column to sum')
+    p = IOArgumentParser(description=__doc__, epilog=EPILOG)
+    p._option_string_actions['-i'].choices = ['binary']
+    p._option_string_actions['-i'].default = 'binary'
+    p._option_string_actions['-o'].choices = OUT_FORMATS
+    p._option_string_actions['-o'].default = 'csv_hist'
+    p.add_argument('-b', '--bin-exp', default=0, type=int, help='bin width exponent of 2')
+    p.add_argument('-x', '--x-value', default='length', choices=X_VALUES, help='x axis value')
+    p.add_argument('-c', '--additional-columns', action='append', default=[], help='additional column to sum')
     p.add_argument('--measure-memory', action='store_true', help='collect and print memory statistics')
     return p
 
 def main():
     app_args = parser().parse_args()
 
     with measure_memory(app_args.measure_memory):
-        histogram(app_args.files, app_args.O, app_args.i, app_args.o, app_args.b, app_args.x, app_args.c)
+        delattr(app_args, 'measure_memory')
+        hist(**vars(app_args))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `flow_models-1.1/flow_models/lib/kde.py` & `flow_models-1.4/flow_models/lib/kde.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.1/flow_models/lib/plot.py` & `flow_models-1.4/flow_models/lib/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 def plot_pdf(data, idx=None, x_val='length', what='flows', mode=frozenset(['points', 'mixture']), normalize=True, fft=False):
     kwargs = {'cmap': STYLE[what][1]}
     plots = []
 
     if isinstance(data, pd.DataFrame):
         if idx is None:
-            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(int))
+            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(np.int64))
 
         data = data.loc[:, 'bin_hi':what + '_sum']
 
         pdfi = pdf_from_cdf(data, idx, what)
         xmin, xmax, ymin, ymax = calc_minmax(idx, pdfi)
 
         if 'line' in mode:
@@ -164,15 +164,15 @@
     plt.legend(frameon=False)
     return plots
 
 def plot_cdf(data, idx=None, x_val='length', what='flows', mode=frozenset(['mixture'])):
     plots = []
     if isinstance(data, pd.DataFrame):
         if idx is None:
-            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(int))
+            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(np.int64))
         if 'line' in mode:
             cdfd = data[what + '_sum'].cumsum() / data[what + '_sum'].sum()
             cdfi = scipy.interpolate.interp1d(cdfd.index, cdfd, 'linear', bounds_error=False)(idx)
             plots += plt.plot(idx, cdfi, STYLE[what][0] + '-', lw=2, ms=1, alpha=0.5,
                               label=what + ' (infered from data points)')
     else:
         plots += plot_mixture(data, idx, x_val, what, mode, 'cdf')
@@ -181,15 +181,15 @@
     plt.legend(frameon=False)
     return plots
 
 def plot_avg(data, idx=None, x_val='length', what='packets', mode=frozenset(['mixture'])):
     plots = []
     if isinstance(data, pd.DataFrame):
         if idx is None:
-            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(int))
+            idx = np.unique(np.rint(np.geomspace(data.index.min(), data.index.max(), LINE_NBINS)).astype(np.int64))
 
         if what in ['packets', 'octets']:
             avg_points, avg_line = avg_data(data, idx, what)
             color = 'g' if what == 'packets' else 'b'
             plt.xscale('log')
             plt.yscale('log')
         elif what in ['packet_size', 'packet_iat']:
```

### Comparing `flow_models-1.1/flow_models/plot.py` & `flow_models-1.4/flow_models/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         fig = plt.figure(figsize=FIGSIZE)
         ax = plt.subplot(1, 1, 1)
 
     plt.subplots_adjust(0, 0, 1, 1)
 
     for obj, df in data.items():
         if idx is None:
-            idx = np.unique(np.rint(np.geomspace(df.index.min(), df.index.max(), LINE_NBINS)).astype(int))
+            idx = np.unique(np.rint(np.geomspace(df.index.min(), df.index.max(), LINE_NBINS)).astype(np.int64))
         for what in ['flows', 'packets', 'octets']:
             logmsg('Drawing CDF', obj, what)
             plot_cdf(df, idx, x_val, what, mode={'line', 'mixture', *cdf_modes})
     ax.set_xlabel(f'Flow {x_val} [{UNITS[x_val]}]')
     ax.set_ylabel('CDF (Fraction of)')
     if not single:
         out = 'cdf'
@@ -92,16 +92,16 @@
     p.add_argument('--format', default='png', choices=['png', 'pdf'], help='plot file format')
     p.add_argument('--single', action='store_true', help='plot PDF and CDF in single file')
     p.add_argument('--no-normalize', action='store_false', help='do not normalize PDF datapoints')
     p.add_argument('--fft', action='store_true', help='use FFT for calculating KDE')
     p.add_argument('-P', action='append', default=[], choices=MODES_PDF, help='additional PDF plot modes (can be specified multiple times)')
     p.add_argument('-C', action='append', default=[], choices=MODES_CDF, help='additional CDF plot modes (can be specified multiple times)')
     p.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
-    p.add_argument('histogram', help='csv_hist file to plot')
-    p.add_argument('mixture', nargs='?', help='mixture directory to plot')
+    p.add_argument('histogram', type=str, help='csv_hist file to plot')
+    p.add_argument('mixture', nargs='?', type=str, help='mixture directory to plot')
     return p
 
 def main():
     app_args = parser().parse_args()
 
     files = [app_args.histogram]
     if app_args.mixture:
```

### Comparing `flow_models-1.1/flow_models/summary.py` & `flow_models-1.4/flow_models/summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 
 from .lib.data import UNITS, detect_x_value
 from .lib.util import logmsg
 
+EPILOG = \
+f"""
+This tool can be used to generate LaTeX summary of flow histogram statistics.
+
+Example:
+
+    flow_models.summary histograms/udp/length.csv
+"""
+
 X_VALUES = ['length', 'size', 'duration', 'rate']
 Y_VALUES = ['flows', 'packets', 'octets']
 
 def summary(obj, x_val=None):
     if isinstance(obj, (str, pathlib.Path)):
         file = pathlib.Path(obj)
         logmsg(f'Loading file {file}')
@@ -33,18 +42,18 @@
 
 def stats_summary(data):
     if isinstance(data, pd.DataFrame):
         s = ['\\begin{tabular}{@{}lrr@{}}',
              '\\toprule',
              '\\textbf{Dataset name} & XXX & \\\\',
              '\\textbf{Exporter} & XXX & \\\\',
-             '\\textbf{L2 technology} & Ethernet & \\\\',
+             '\\textbf{L2 technology} & XXX & \\\\',
              '\\textbf{Sampling rate} & none & \\\\',
-             '\\textbf{Active timeout} & 300 & seconds \\\\',
-             '\\textbf{Inactive timeout} & 15 & seconds \\\\',
+             '\\textbf{Active timeout} & XXX & seconds \\\\',
+             '\\textbf{Inactive timeout} & XXX & seconds \\\\',
              '\\midrule']
         for what in Y_VALUES:
             col = what + '_sum'
             if col in data:
                 tot = data[col].sum()
                 s.append('\\textbf{Number of %s} & ' % what + '{:,}'.format(tot).replace(',', ' ') + f' & {what} \\\\')
         for what in X_VALUES:
@@ -87,15 +96,15 @@
         for n in range(len(points)):
             s.append(f'{points[n]} & ' + ' & '.join(f'{vals[what][n]:.4f}' for what in Y_VALUES) + ' \\\\')
         s += ['\\bottomrule',
               '\\end{tabular}']
         return '\n'.join(s)
 
 def parser():
-    p = argparse.ArgumentParser(description=__doc__)
+    p = argparse.ArgumentParser(description=__doc__, epilog=EPILOG)
     p.add_argument('-x', choices=X_VALUES, help='x axis value')
     p.add_argument('file', help='csv_hist file to summarize')
     return p
 
 def main():
     app_args = parser().parse_args()
```

### Comparing `flow_models-1.1/flow_models.egg-info/PKG-INFO` & `flow_models-1.4/flow_models.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: flow-models
-Version: 1.1
+Version: 1.4
 Summary: A framework for analysis and modeling of IP network flows
 Home-page: https://github.com/piotrjurkiewicz/flow-models
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
-Description: # flow-models: A framework for analysis and modeling of IP network flows
-        
-        Packages like `flow-tools` or `nfdump` provide tools for filtering and calculating simple summary/top-N statistics
-        from network flow records. They lack, however, any capabilities for analysis and modeling of flow features (length,
-        size, duration, rate, etc.) distributions. The goal of this framework is to fill this gap.
-        
-        `flow-models` is a software framework for creating precise and reproducible statistical flow models from
-        NetFlow/IPFIX flow records. It can be used to merge split records, calculate histograms of flow features and create
-        General Mixture Models fitting them. Created models can be used both as an input in analytical calculations and to
-        generate realistic traffic in simulations.
-        
-        The framework can be installed from [Python Package Index (PyPI)](https://pypi.org/project/flow-models/) using the
-        following command:
-        
-            pip install flow-models
-        
-        A detailed documentation, including usage examples, is available at: https://flow-models.readthedocs.io
-        
-        Apart from the framework, the Git repository also contains a library of flow models created with it, including
-        histograms and fitted mixture models.
-        
-        ## Provided tools
-        
-        The framework currently includes the following tools:
-        
-        - `merge` -- merges flows which were split across multiple records due to *active timeout*
-        - `sort` -- sorts flow records according to specified fields (requires `numpy`)
-        - `hist` -- calculates histograms of flows length, size, duration or rate
-        - `hist_np` -- calculates histograms using multiple threads (requires `numpy`, much faster, but uses more memory)
-        - `fit` -- creates General Mixture Models (GMM) fitted to flow records (requires `scipy`)
-        - `plot` -- generates plots from flow records and fitted models (requires `pandas` and `scipy`)
-        - `generate` -- generates flow records from histograms or mixture models
-        - `summary` -- produces TeX tables containing summary statistics of flow dataset (requires `scipy`)
-        - `convert` -- converts flow records between supported formats
-        
-        Following the Unix philosophy, each tool is a separate Python program aimed at a single purpose. Features provided
-        by the tools are orthogonal and they are tailored to be used sequentially in data-processing pipelines.
-        
-        ## Models library
-        
-        The repository of flow models, containing histogram CSV files, fitted mixture models and plots, is available at: https://github.com/piotrjurkiewicz/flow-models
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# flow-models: A framework for analysis and modeling of IP network flows
+
+Packages like `flow-tools` or `nfdump` provide tools for filtering and calculating simple summary/top-N statistics
+from network flow records. They lack, however, any capabilities for analysis and modeling of flow features (length,
+size, duration, rate, etc.) distributions. The goal of this framework is to fill this gap.
+
+`flow-models` is a software framework for creating precise and reproducible statistical flow models from
+NetFlow/IPFIX flow records. It can be used to merge split records, calculate histograms of flow features and create
+General Mixture Models fitting them. Created models can be used both as an input in analytical calculations and to
+generate realistic traffic in simulations.
+
+The framework can be installed from [Python Package Index (PyPI)](https://pypi.org/project/flow-models/) using the
+following command:
+
+    pip install flow-models
+
+A detailed documentation, including usage examples, is available at: https://flow-models.readthedocs.io
+
+Apart from the framework, the Git repository also contains a library of flow models created with it, including
+histograms and fitted mixture models.
+
+## Provided tools
+
+The framework currently includes the following tools:
+
+- `merge` -- merges flows which were split across multiple records due to *active timeout*
+- `sort` -- sorts flow records according to specified fields (requires `numpy`)
+- `hist` -- calculates histograms of flows length, size, duration or rate
+- `hist_np` -- calculates histograms using multiple threads (requires `numpy`, much faster, but uses more memory)
+- `fit` -- creates General Mixture Models (GMM) fitted to flow records (requires `scipy`)
+- `plot` -- generates plots from flow records and fitted models (requires `pandas` and `scipy`)
+- `generate` -- generates flow records from histograms or mixture models
+- `summary` -- produces TeX tables containing summary statistics of flow dataset (requires `scipy`)
+- `convert` -- converts flow records between supported formats
+
+Following the Unix philosophy, each tool is a separate Python program aimed at a single purpose. Features provided
+by the tools are orthogonal and they are tailored to be used sequentially in data-processing pipelines.
+
+## Models library
+
+The repository of flow models, containing histogram CSV files, fitted mixture models and plots, is available at: https://github.com/piotrjurkiewicz/flow-models
```

