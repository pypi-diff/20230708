# Comparing `tmp/igorwriter-0.4.1.tar.gz` & `tmp/igorwriter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igorwriter-0.4.1.tar", last modified: Sun Jul  2 02:51:43 2023, max compression
+gzip compressed data, was "igorwriter-0.5.0.tar", last modified: Sat Jul  8 09:40:04 2023, max compression
```

## Comparing `igorwriter-0.4.1.tar` & `igorwriter-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.976578 igorwriter-0.4.1/
--rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4816 2023-07-02 02:51:43.976578 igorwriter-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4307 2023-07-02 02:51:23.000000 igorwriter-0.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.964584 igorwriter-0.4.1/igorwriter/
--rw-rw-rw-   0        0        0       53 2023-07-01 17:36:50.000000 igorwriter-0.4.1/igorwriter/__init__.py
--rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtin_names.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.973584 igorwriter-0.4.1/igorwriter/builtins/
--rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/functions.txt
--rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/keywords.txt
--rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/operations.txt
--rw-rw-rw-   0        0        0      213 2023-07-01 17:22:58.000000 igorwriter-0.4.1/igorwriter/errors.py
--rw-rw-rw-   0        0        0    18287 2023-07-01 17:36:50.000000 igorwriter-0.4.1/igorwriter/igorwave.py
--rw-rw-rw-   0        0        0     1511 2019-11-16 05:32:31.000000 igorwriter-0.4.1/igorwriter/utils.py
--rw-rw-rw-   0        0        0     2807 2023-07-01 17:22:58.000000 igorwriter-0.4.1/igorwriter/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.970590 igorwriter-0.4.1/igorwriter.egg-info/
--rw-rw-rw-   0        0        0     4816 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-02 02:51:43.980579 igorwriter-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-07-02 02:51:23.000000 igorwriter-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.975587 igorwriter-0.4.1/tests/
--rw-rw-rw-   0        0        0     4191 2023-07-01 17:22:58.000000 igorwriter-0.4.1/tests/test_names.py
--rw-rw-rw-   0        0        0     1256 2019-11-16 04:29:14.000000 igorwriter-0.4.1/tests/test_utils.py
--rw-rw-rw-   0        0        0    12984 2023-07-01 17:36:50.000000 igorwriter-0.4.1/tests/test_wave.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:40:04.032771 igorwriter-0.5.0/
+-rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     6012 2023-07-08 09:40:04.032771 igorwriter-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5469 2023-07-08 09:35:28.000000 igorwriter-0.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-08 09:40:04.025765 igorwriter-0.5.0/igorwriter/
+-rw-rw-rw-   0        0        0       53 2023-07-04 12:29:43.000000 igorwriter-0.5.0/igorwriter/__init__.py
+-rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.5.0/igorwriter/builtin_names.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:40:04.030771 igorwriter-0.5.0/igorwriter/builtins/
+-rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.5.0/igorwriter/builtins/functions.txt
+-rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.5.0/igorwriter/builtins/keywords.txt
+-rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.5.0/igorwriter/builtins/operations.txt
+-rw-rw-rw-   0        0        0      214 2023-07-07 17:00:52.000000 igorwriter-0.5.0/igorwriter/errors.py
+-rw-rw-rw-   0        0        0    22884 2023-07-08 09:15:02.000000 igorwriter-0.5.0/igorwriter/igorwave.py
+-rw-rw-rw-   0        0        0     1529 2023-07-07 16:02:45.000000 igorwriter-0.5.0/igorwriter/utils.py
+-rw-rw-rw-   0        0        0     3012 2023-07-07 16:02:45.000000 igorwriter-0.5.0/igorwriter/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:40:04.028770 igorwriter-0.5.0/igorwriter.egg-info/
+-rw-rw-rw-   0        0        0     6012 2023-07-08 09:40:04.000000 igorwriter-0.5.0/igorwriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-08 09:40:04.000000 igorwriter-0.5.0/igorwriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:40:04.000000 igorwriter-0.5.0/igorwriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 09:40:04.000000 igorwriter-0.5.0/igorwriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 09:40:04.000000 igorwriter-0.5.0/igorwriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-08 09:40:04.033771 igorwriter-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-08 09:35:28.000000 igorwriter-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:40:04.031770 igorwriter-0.5.0/tests/
+-rw-rw-rw-   0        0        0     4113 2023-07-07 16:02:45.000000 igorwriter-0.5.0/tests/test_names.py
+-rw-rw-rw-   0        0        0     1102 2023-07-07 16:02:45.000000 igorwriter-0.5.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0    17985 2023-07-08 09:15:02.000000 igorwriter-0.5.0/tests/test_wave.py
```

### Comparing `igorwriter-0.4.1/LICENSE.txt` & `igorwriter-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.1/PKG-INFO` & `igorwriter-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igorwriter
-Version: 0.4.1
+Version: 0.5.0
 Summary: Write IGOR binary (.ibw) or text (.itx) files from numpy array
 Home-page: https://github.com/t-onoz/igorwriter
 Author: t-onoz
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,19 @@
 IgorWriter
 ==========
 
 Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
 
 Features
 --------
-- Compatible with multi-dimensional arrays (up to 4 dimensions)
-- Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
-- Data units (:code:`IgorWave.set_datascale`)
-- Dimension scaling (:code:`IgorWave.set_dimscale`)
-- Dimension labels (:code:`IgorWave.set_dimlabel`)
+* Compatible with multi-dimensional arrays (up to 4 dimensions)
+* Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
+* Data units (:code:`IgorWave.set_datascale`)
+* Dimension scaling (:code:`IgorWave.set_dimscale`)
+* Dimension labels (:code:`IgorWave.set_dimlabel`)
 
 Installation
 ------------
 .. code-block:: doscon
 
     $ pip install igorwriter
 
@@ -54,63 +54,97 @@
 >>> wave.set_dimscale('x', 0, 0.01, 's')
 
 A two-dimensional array with dimension labels
 
 >>> a2 = np.random.random((10, 3))
 >>> wave = IgorWave(a2, name='wave2d')
 >>> # you may set optional dimension labels
->>> wave.set_dimlabel(0, -1, 'points') # entire label for rows
->>> wave.set_dimlabel(1, -1, 'values') # entire label for columns
+>>> wave.set_dimlabel(0, -1, 'points') # label for entire rows
+>>> wave.set_dimlabel(1, -1, 'values') # label for entire columns
 >>> wave.set_dimlabel(1, 0, 'ValueA')  # label for column 0
 >>> wave.set_dimlabel(1, 1, 'ValueB')  # label for column 1
 >>> wave.set_dimlabel(1, 2, 'ValueC')  # label for column 2
 >>> wave.save('my2dwave.ibw')
 
+Unicode support
+---------------
+From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding.
+If you use Igor Pro 6 or older and want to use non-ascii characters, set :code:`unicode=False` when calling :code:`IgorWave()`.
+It will fall back to system text encoding (Windows-1252, Shift JIS, etc.).
+
 Wave Names
 ----------
 There are restrictions on object names in IGOR. From v0.2.0, this package deals with illegal object names.
 
->>> wave = IgorWave(array, name='\'this_is_illegal\'', on_errors='fix')  # fix illegal names automatically
-RenameWarning: name "'this_is_illegal'" is fixed as '_this_is_illegal_' (reason: name must not contain " ' : ; or any control characters.)
->>> print(wave.name)
-_this_is_illegal_
->>> wave = IgorWave(array, name='\'this_is_illegal\'', on_errors='raise')  # raise errors
+>>> wave = IgorWave(array, name='wave:0', on_errors='fix')  # fix illegal names automatically
+RenameWarning: name 'wave:0' is fixed as 'wave_0' (reason: name must not contain " ' : ; or any control characters.)
+>>> wave.name
+'wave_0'
+>>> wave = IgorWave(array, name='wave:0', on_errors='raise')  # raise errors
 Traceback (most recent call last):
 ...
-igorwriter.errors.InvalidNameError: name must not contain " ' : ; or any control characters.
+InvalidNameError: name must not contain " ' : ; or any control characters.
+
+
+Pint integration
+----------------
+If `Pint <https://github.com/hgrecco/pint>`_ Quantity objects are passed to IgorWave, data units will be set automatically.
+
+>>> import pint
+>>> ureg = pint.UnitRegistry()
+>>> w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
+>>> w.save_itx('wave_with_units.itx')
+...
+X SetScale d,0,0,"m / s",'wave_with_units'
+X SetScale /P x,0.0,1.0,"",'wave_with_units'
+
 
-Exporting pandas.DataFrame
---------------------------
-Convenience functions for saving DataFrame in a Igor Text file or a series of Igor Binary Wave files are provided.
+
+Pandas integration
+------------------
+You can easily export DataFrame objects with convenience functions.
 
 >>> from igorwriter import utils
 >>> utils.dataframe_to_itx(df, 'df.itx')   # all Series are exported in one file
 >>> waves = utils.dataframe_to_ibw(df, prefix='df_bin')   # each Series is saved in a separate file, <prefix>_<column>.ibw
 >>> waves  # dictionary of generated IgorWaves. You can change wave names, set data units, set dimension scaling, etc.
 {'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
 
+IgorWriter tries to convert index info on pandas.Series objects.
+
+* If the index is evenly-spaced, wave dimension scaling is set accordingly.
+* Index names are interpreted as the dimension labels.
+
 Notes on Image Plots
 --------------------
 Image Plot in IGOR and :code:`imshow` in matplotlib use different convention for x and y axes:
 
 - Rows as x, columns as y (IGOR)
 - Columns as x, rows as y (Matplotlib)
 
-Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods. 
+Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods.
 If you use e.g. 
 
 >>> wave.save('path.ibw', image=True)
     
 :code:`plt.imshow` and Image Plot will give the same results.
 
 
 Changelog
 =========
 
 
+v0.5.0 (2023-07-08)
+-------------------
+- UTF-8 as default encoding. You can instead use system text encoding by setting :code:`unicode=False` to IgorWave().
+- Automatic conversion from pandas index to dimension scaling.
+- Exporting 64-bit integer waves (requires Igor Pro 7 or later).
+- BUG FIX: Igor Text files created from np.bool\_ arrays were broken.
+
+
 v0.4.1 (2023-07-02)
 -------------------
 - Added support for np.str\_, np.bytes\_ arrays.
 - Automatic type conversion for np.object\_ arrays.
 - Added support for dimension scaling (:code:`IgorWave.set_simlabel`).
```

### Comparing `igorwriter-0.4.1/README.rst` & `igorwriter-0.5.0/igorwriter.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,171 @@
-IgorWriter
-==========
-
-Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
-
-Features
---------
-- Compatible with multi-dimensional arrays (up to 4 dimensions)
-- Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
-- Data units (:code:`IgorWave.set_datascale`)
-- Dimension scaling (:code:`IgorWave.set_dimscale`)
-- Dimension labels (:code:`IgorWave.set_dimlabel`)
-
-Installation
-------------
-.. code-block:: doscon
-
-    $ pip install igorwriter
-
-Usage
------
-
-Basic usage
-
->>> import numpy as np
->>> from igorwriter import IgorWave
->>> array = np.array([1,2,3,4,5,6])
->>> # make IgorWave objects
->>> wave = IgorWave(array, name='mywave')
->>> wave2 = IgorWave(array.astype(np.float32), name='mywave2')
->>> # save data
->>> wave.save('mywave.ibw')
->>> wave.save_itx('mywave.itx')
->>> with open('multi_waves.itx', 'w') as fp:
->>>     # Igor Text files can contain multiples waves per file
->>>     wave.save_itx(fp)
->>>     wave2.save_itx(fp)
-
-Data units, dimension scaling
-
->>> wave.set_datascale('DataUnit')
->>> wave.set_dimscale('x', 0, 0.01, 's')
-
-A two-dimensional array with dimension labels
-
->>> a2 = np.random.random((10, 3))
->>> wave = IgorWave(a2, name='wave2d')
->>> # you may set optional dimension labels
->>> wave.set_dimlabel(0, -1, 'points') # entire label for rows
->>> wave.set_dimlabel(1, -1, 'values') # entire label for columns
->>> wave.set_dimlabel(1, 0, 'ValueA')  # label for column 0
->>> wave.set_dimlabel(1, 1, 'ValueB')  # label for column 1
->>> wave.set_dimlabel(1, 2, 'ValueC')  # label for column 2
->>> wave.save('my2dwave.ibw')
-
-Wave Names
-----------
-There are restrictions on object names in IGOR. From v0.2.0, this package deals with illegal object names.
-
->>> wave = IgorWave(array, name='\'this_is_illegal\'', on_errors='fix')  # fix illegal names automatically
-RenameWarning: name "'this_is_illegal'" is fixed as '_this_is_illegal_' (reason: name must not contain " ' : ; or any control characters.)
->>> print(wave.name)
-_this_is_illegal_
->>> wave = IgorWave(array, name='\'this_is_illegal\'', on_errors='raise')  # raise errors
-Traceback (most recent call last):
-...
-igorwriter.errors.InvalidNameError: name must not contain " ' : ; or any control characters.
-
-Exporting pandas.DataFrame
---------------------------
-Convenience functions for saving DataFrame in a Igor Text file or a series of Igor Binary Wave files are provided.
-
->>> from igorwriter import utils
->>> utils.dataframe_to_itx(df, 'df.itx')   # all Series are exported in one file
->>> waves = utils.dataframe_to_ibw(df, prefix='df_bin')   # each Series is saved in a separate file, <prefix>_<column>.ibw
->>> waves  # dictionary of generated IgorWaves. You can change wave names, set data units, set dimension scaling, etc.
-{'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
-
-Notes on Image Plots
---------------------
-Image Plot in IGOR and :code:`imshow` in matplotlib use different convention for x and y axes:
-
-- Rows as x, columns as y (IGOR)
-- Columns as x, rows as y (Matplotlib)
-
-Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods. 
-If you use e.g. 
-
->>> wave.save('path.ibw', image=True)
-    
-:code:`plt.imshow` and Image Plot will give the same results.
-
-
-Changelog
-=========
-
-
-v0.4.1 (2023-07-02)
--------------------
-- Added support for np.str\_, np.bytes\_ arrays.
-- Automatic type conversion for np.object\_ arrays.
-- Added support for dimension scaling (:code:`IgorWave.set_simlabel`).
-
-
-v0.3.0 (2019-11-16)
--------------------
-- Added :code:`utils.dict_to_{ibw, itx}` 
-- Set datascale automatically for pint Quantity object.
-- Added support for np.datetime64 array.
-
-
-v0.2.3 (2019-11-09)
--------------------
-- Added support for 64-bit integers (by automatically casting onto 32-bit integers on save). 
-
-
-v0.2.0 (2019-11-08)
--------------------
-- Added utilities for pandas (:code:`utils.dataframe_to_{ibw, itx}` ).
-- Added unittest scripts. 
-- Added wave name validator. 
-- BUG FIX: long (> 3 bytes) units for dimension scaling were ignored in
-  save_itx() 
-- IgorWriter now uses system locale encoding rather than ASCII (the default behavior of
-  IGOR Pro prior to ver. 7.00) 
+Metadata-Version: 2.1
+Name: igorwriter
+Version: 0.5.0
+Summary: Write IGOR binary (.ibw) or text (.itx) files from numpy array
+Home-page: https://github.com/t-onoz/igorwriter
+Author: t-onoz
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.txt
+
+IgorWriter
+==========
+
+Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
+
+Features
+--------
+* Compatible with multi-dimensional arrays (up to 4 dimensions)
+* Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
+* Data units (:code:`IgorWave.set_datascale`)
+* Dimension scaling (:code:`IgorWave.set_dimscale`)
+* Dimension labels (:code:`IgorWave.set_dimlabel`)
+
+Installation
+------------
+.. code-block:: doscon
+
+    $ pip install igorwriter
+
+Usage
+-----
+
+Basic usage
+
+>>> import numpy as np
+>>> from igorwriter import IgorWave
+>>> array = np.array([1,2,3,4,5,6])
+>>> # make IgorWave objects
+>>> wave = IgorWave(array, name='mywave')
+>>> wave2 = IgorWave(array.astype(np.float32), name='mywave2')
+>>> # save data
+>>> wave.save('mywave.ibw')
+>>> wave.save_itx('mywave.itx')
+>>> with open('multi_waves.itx', 'w') as fp:
+>>>     # Igor Text files can contain multiples waves per file
+>>>     wave.save_itx(fp)
+>>>     wave2.save_itx(fp)
+
+Data units, dimension scaling
+
+>>> wave.set_datascale('DataUnit')
+>>> wave.set_dimscale('x', 0, 0.01, 's')
+
+A two-dimensional array with dimension labels
+
+>>> a2 = np.random.random((10, 3))
+>>> wave = IgorWave(a2, name='wave2d')
+>>> # you may set optional dimension labels
+>>> wave.set_dimlabel(0, -1, 'points') # label for entire rows
+>>> wave.set_dimlabel(1, -1, 'values') # label for entire columns
+>>> wave.set_dimlabel(1, 0, 'ValueA')  # label for column 0
+>>> wave.set_dimlabel(1, 1, 'ValueB')  # label for column 1
+>>> wave.set_dimlabel(1, 2, 'ValueC')  # label for column 2
+>>> wave.save('my2dwave.ibw')
+
+Unicode support
+---------------
+From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding.
+If you use Igor Pro 6 or older and want to use non-ascii characters, set :code:`unicode=False` when calling :code:`IgorWave()`.
+It will fall back to system text encoding (Windows-1252, Shift JIS, etc.).
+
+Wave Names
+----------
+There are restrictions on object names in IGOR. From v0.2.0, this package deals with illegal object names.
+
+>>> wave = IgorWave(array, name='wave:0', on_errors='fix')  # fix illegal names automatically
+RenameWarning: name 'wave:0' is fixed as 'wave_0' (reason: name must not contain " ' : ; or any control characters.)
+>>> wave.name
+'wave_0'
+>>> wave = IgorWave(array, name='wave:0', on_errors='raise')  # raise errors
+Traceback (most recent call last):
+...
+InvalidNameError: name must not contain " ' : ; or any control characters.
+
+
+Pint integration
+----------------
+If `Pint <https://github.com/hgrecco/pint>`_ Quantity objects are passed to IgorWave, data units will be set automatically.
+
+>>> import pint
+>>> ureg = pint.UnitRegistry()
+>>> w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
+>>> w.save_itx('wave_with_units.itx')
+...
+X SetScale d,0,0,"m / s",'wave_with_units'
+X SetScale /P x,0.0,1.0,"",'wave_with_units'
+
+
+
+Pandas integration
+------------------
+You can easily export DataFrame objects with convenience functions.
+
+>>> from igorwriter import utils
+>>> utils.dataframe_to_itx(df, 'df.itx')   # all Series are exported in one file
+>>> waves = utils.dataframe_to_ibw(df, prefix='df_bin')   # each Series is saved in a separate file, <prefix>_<column>.ibw
+>>> waves  # dictionary of generated IgorWaves. You can change wave names, set data units, set dimension scaling, etc.
+{'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
+
+IgorWriter tries to convert index info on pandas.Series objects.
+
+* If the index is evenly-spaced, wave dimension scaling is set accordingly.
+* Index names are interpreted as the dimension labels.
+
+Notes on Image Plots
+--------------------
+Image Plot in IGOR and :code:`imshow` in matplotlib use different convention for x and y axes:
+
+- Rows as x, columns as y (IGOR)
+- Columns as x, rows as y (Matplotlib)
+
+Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods.
+If you use e.g. 
+
+>>> wave.save('path.ibw', image=True)
+    
+:code:`plt.imshow` and Image Plot will give the same results.
+
+
+Changelog
+=========
+
+
+v0.5.0 (2023-07-08)
+-------------------
+- UTF-8 as default encoding. You can instead use system text encoding by setting :code:`unicode=False` to IgorWave().
+- Automatic conversion from pandas index to dimension scaling.
+- Exporting 64-bit integer waves (requires Igor Pro 7 or later).
+- BUG FIX: Igor Text files created from np.bool\_ arrays were broken.
+
+
+v0.4.1 (2023-07-02)
+-------------------
+- Added support for np.str\_, np.bytes\_ arrays.
+- Automatic type conversion for np.object\_ arrays.
+- Added support for dimension scaling (:code:`IgorWave.set_simlabel`).
+
+
+v0.3.0 (2019-11-16)
+-------------------
+- Added :code:`utils.dict_to_{ibw, itx}` 
+- Set datascale automatically for pint Quantity object.
+- Added support for np.datetime64 array.
+
+
+v0.2.3 (2019-11-09)
+-------------------
+- Added support for 64-bit integers (by automatically casting onto 32-bit integers on save). 
+
+
+v0.2.0 (2019-11-08)
+-------------------
+- Added utilities for pandas (:code:`utils.dataframe_to_{ibw, itx}` ).
+- Added unittest scripts. 
+- Added wave name validator. 
+- BUG FIX: long (> 3 bytes) units for dimension scaling were ignored in
+  save_itx() 
+- IgorWriter now uses system locale encoding rather than ASCII (the default behavior of
+  IGOR Pro prior to ver. 7.00)
```

### Comparing `igorwriter-0.4.1/igorwriter/builtins/functions.txt` & `igorwriter-0.5.0/igorwriter/builtins/functions.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.1/igorwriter/builtins/operations.txt` & `igorwriter-0.5.0/igorwriter/builtins/operations.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.1/igorwriter/igorwave.py` & `igorwriter-0.5.0/igorwriter/igorwave.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function, unicode_literals
 import os
-import locale
 import ctypes
 import struct
-import numpy as np
-
-import igorwriter.errors
+import warnings
+from locale import getpreferredencoding as _getpreferredencoding
 
+import numpy as np
 try:
-    from pint.errors import UnitStrippedWarning
+    from pandas import Series
 except ImportError:
-    class UnitStrippedWarning(UserWarning):
+    class Series:
+        pass
+try:
+    from pint import Quantity
+except ImportError:
+    class Quantity:
         pass
-import warnings
 
+import igorwriter.errors
 from igorwriter import validator
-from igorwriter.errors import TypeConversionWarning
+from igorwriter.errors import TypeConversionWarning, StrippedSeriesIndexWarning, InvalidNameError
 
 MAXDIMS = 4
 MAX_WAVE_NAME2 = 18  # Maximum length of wave name in version 1 and 2 files. Does not include the trailing null.
 MAX_WAVE_NAME5 = 31  # Maximum length of wave name in version 5 files. Does not include the trailing null.
 MAX_UNIT_CHARS = 3
-
-ENCODING = locale.getpreferredencoding()
+ENCODING = None
 
 TYPES = {
     np.bytes_: 0,
-    np.str_: 0,
-    np.bool_: 8,
     np.int8: 8,
     np.int16: 0x10,
     np.int32: 0x20,
+    np.int64: 0x80,  # requires Igor Pro 7 or later
     np.uint8: 8 + 0x40,
     np.uint16: 0x10 + 0x40,
     np.uint32: 0x20 + 0x40,
+    np.uint64: 0x80 + 0x40,  # requires Igor Pro 7 or later
     np.float32: 2,
     np.float64: 4,
     np.complex64: 2 + 1,
     np.complex128: 4 + 1,
 }
 ITX_TYPES = {
-    np.bool_: '/B',
     np.int8: '/B',
     np.int16: '/W',
     np.int32: '/I',
+    np.int64: '/L',  # requires Igor Pro 7 or later
     np.uint8: '/U/B',
     np.uint16: '/U/W',
     np.uint32: '/U/I',
+    np.uint64: '/U/L',   # requires Igor Pro 7 or later
     np.float32: '/S',
     np.float64: '/D',
     np.complex64: '/C/S',
     np.complex128: '/C/D',
     np.bytes_: '/T',
-    np.str_: '/T',
 }
 
 
 class BinHeader5(ctypes.Structure):
     _pack_ = 2
     _fields_ = [
         ('version', ctypes.c_int16),					# Version number for backwards compatibility.
@@ -83,15 +84,18 @@
     _fields_ = [
         ('next', ctypes.c_byte * 4),  # link to next wave in linked list.
         ('creationDate', ctypes.c_uint32),  # DateTime of creation.
         ('modDate', ctypes.c_uint32),  # DateTime of last modification.
         ('npnts', ctypes.c_int32),  # Total number of points (multiply dimensions up to first zero).
         ('type', ctypes.c_int16),  # See types (e.g. NT_FP64) above. Zero for text waves.
         ('dLock', ctypes.c_int16),  # Reserved. Write zero. Ignore on read.
-        ('whpad1', ctypes.c_char * 6),  # Reserved. Write zero. Ignore on read.
+        ('whpad1', ctypes.c_char * 3),  # Reserved. Write zero. Ignore on read.
+        ('waveNameEncoding', ctypes.c_byte),
+        ('waveUnitsEncoding', ctypes.c_byte),
+        ('waveNoteEncoding', ctypes.c_byte),
         ('whVersion', ctypes.c_int16),  # Write 1. Ignore on read.
         ('bname', ctypes.c_char * (MAX_WAVE_NAME5 + 1)),  # Name of wave plus trailing null.
         ('whpad2', ctypes.c_int32),  # Reserved. Write zero. Ignore on read.
         ('dFolder', ctypes.c_byte * 4),  # Used in memory only. Write zero. Ignore on read.
 
         # Dimensioning info. [0] == rows, [1] == cols etc
         ('nDim', ctypes.c_int32 * MAXDIMS),  # Number of items in a dimension -- 0 means no data.
@@ -110,15 +114,17 @@
         ('dataEUnits', ctypes.c_byte * 4),  # Used in memory only. Write zero. Ignore on read.
         ('dimEUnits', (ctypes.c_byte * 4) * MAXDIMS),  # Used in memory only. Write zero. Ignore on read.
         ('dimLabels', (ctypes.c_byte * 4) * MAXDIMS),  # Used in memory only. Write zero. Ignore on read.
         
         ('waveNoteH', ctypes.c_byte * 4),  # Used in memory only. Write zero. Ignore on read.
 
         ('platform', ctypes.c_char),  # 0=unspecified, 1=Macintosh, '2=Windows', Added for Igor Pro 5.5.
-        ('spare', ctypes.c_char * 3),
+        ('spare', ctypes.c_char),
+        ('waveDimLabelEncoding', ctypes.c_byte),
+        ('textWaveContentEncoding', ctypes.c_byte),
 
         ('whUnused', ctypes.c_int32 * 13),  # Reserved. Write zero. Ignore on read.
 
         ('vRefNum', ctypes.c_int32),
         ('dirID', ctypes.c_int32),  # Used in memory only. Write zero. Ignore on read.
 
         # The following stuff is considered private to Igor.
@@ -126,82 +132,100 @@
 
         # ('wData', ctypes.c_float * 1),  # The start of the array of data. Must be 64 bit aligned.
     ]
 
     def __init__(self):
         super(WaveHeader5, self).__init__()
         self.sfA = (1,) * MAXDIMS
+        self.whVersion = 1
 
 
 class IgorWave5(object):
-    def __init__(self, array, name='wave0', on_errors='fix'):
+    def __init__(self, array, name='wave0', on_errors='fix', unicode=True, int64_support=False):
         """
 
         :param array: array_like object
         :param name: wave name
         :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise exception.
+        :param unicode: enables unicode support (encoding texts with utf-8).
+            If you use Igor Pro 6 or older and want to use non-ascii characters, set it to False.
+        :param int64_support: enables 64-bit integer support (requires Igor Pro 7 or later).
+            Note: If enabled, it will break backward compatibility for Igor Pro 6 or earlier.
         """
         self._bin_header = BinHeader5()
         self._wave_header = WaveHeader5()
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore', category=UnitStrippedWarning)
-            self.array = np.asarray(array)
-        self.rename(name, on_errors=on_errors)
+        if unicode:
+            self._wave_header.waveNameEncoding = 1
+            self._wave_header.waveUnitsEncoding = 1
+            self._wave_header.waveNoteEncoding = 1
+            self._wave_header.waveDimLabelEncoding = 1
+            self._wave_header.textWaveContentEncoding = 1
+            self._encoding = 'utf-8'
+        else:
+            self._encoding = _getpreferredencoding()
+        self._int64_support = int64_support
+        self.rename(name, on_errors)
         self._extended_data_units = b''
         self._extended_dimension_units = [b'', b'', b'', b'']
         self._dimension_labels = [dict(), dict(), dict(), dict()]
-        try:
-            # set units for pint.quantity._Quantity
-            self.set_datascale('{:~}'.format(array.units))
-        except (ValueError, AttributeError):
-            pass
-    
+
+        if isinstance(array, Series):
+            self.array = self._parse_Series(array)
+        elif isinstance(array, Quantity):
+            self.array = self._parse_Pint(array)
+        else:
+            self.array = np.asarray(array)
+
     def rename(self, name, on_errors='fix'):
         """
 
         :param name: new wavename.
         :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise exception.
         :return:
         """
-        bname = validator.check_and_encode(name, on_errors=on_errors)
+        bname = validator.check_and_encode(name, on_errors=on_errors, encoding=self._encoding)
         self._wave_header.bname = bname
 
     @property
     def name(self):
-        return self._wave_header.bname.decode(ENCODING)
+        return self._wave_header.bname.decode(self._encoding)
 
     def set_dimscale(self, dim, start, delta, units=None):
         """Set scale information of each axis.
 
         :param dim: dimensionality, 'x', 'y', 'z', or 't'
         :param start: start value (e.g. x[0])
         :param delta: "delta value" (e.g. x[1] - x[0])
         :param units: optional unit string
         :return:
         """
         dimint = {'x': 0, 'y': 1, 'z': 2, 't': 3}[dim]
         self._wave_header.sfB[dimint] = start
         self._wave_header.sfA[dimint] = delta
         if units is not None:
-            bunits = units.encode(ENCODING)
+            bunits = units.encode(self._encoding)
+            # if the units is short, they are written directly in the WaveHeader5 object.
+            # longer units are stored as dict, and encoded when saved.
             if len(bunits) <= MAX_UNIT_CHARS:
                 self._wave_header.dimUnits[dimint][:] = bunits + b'\x00' * (MAX_UNIT_CHARS + 1 - len(bunits))
                 self._bin_header.dimEUnitsSize[dimint] = 0
                 self._extended_dimension_units[dimint] = b''
             else:
                 self._wave_header.dimUnits[dimint][:] = b'\x00' * (MAX_UNIT_CHARS + 1)
                 self._bin_header.dimEUnitsSize[dimint] = len(bunits)
                 self._extended_dimension_units[dimint] = bunits
 
     def set_datascale(self, units):
         """Set units of the data.
 
         :param units: string representing units of the data.
         """
-        bunits = units.encode('ascii', errors='replace')
+        bunits = units.encode(self._encoding)
+        # if the units is short, they are written directly in the WaveHeader5 object.
+        # longer units are stored as python bytes object, and written when saved.
         if len(bunits) <= MAX_UNIT_CHARS:
             self._wave_header.dataUnits = bunits
             self._bin_header.dataEUnitsSize = 0
             self._extended_data_units = b''
         else:
             self._wave_header.dataUnits = b''
             self._bin_header.dataEUnitsSize = len(bunits)
@@ -217,16 +241,18 @@
         if dimNumber not in [0, 1, 2, 3]:
             raise ValueError('dimNumber must be 0, 1, 2, or 3.')
 
         # Dimension labels cannot contain illegal characters (", ', :, ; and control characters),
         # but they can conflict with built-in names.
         for s in validator.NG_LETTERS:
             if s in label:
-                raise igorwriter.errors.InvalidNameError('label contains illegal characters (", \', :, ;, and control characters)')
-        blabel = label.encode(ENCODING)
+                raise igorwriter.errors.InvalidNameError(
+                    'thelabel contains illegal characters (", \', :, ;, and control characters)'
+                )
+        blabel = label.encode(self._encoding)
         if len(blabel) > 31:
             raise ValueError('Dimension labels cannot be longer than 31 bytes.')
 
         if label == '':
             # if label is empty, remove the label.
             self._dimension_labels[dimNumber].pop(dimIndex, None)
         else:
@@ -249,16 +275,16 @@
 
         self._wave_header.npnts = len(a.ravel())
         self._wave_header.type = TYPES[a.dtype.type]
 
         self._wave_header.nDim = a.shape + (0,) * (MAXDIMS - a.ndim)
 
         if TYPES[a.dtype.type] == 0:
-            # text wave
-            wavesize = len(b''.join(a.ravel(order='F')))
+            # text wave (should be stored as numpy.bytes_)
+            wavesize = np.sum([len(x) for x in a.ravel()], dtype=int)
             self._bin_header.sIndicesSize = 4 * a.size
         else:
             wavesize = a.nbytes
             self._bin_header.sIndicesSize = 0
 
         self._bin_header.wfmSize = 320 + wavesize
 
@@ -267,66 +293,74 @@
         self._bin_header.checksum -= sum(struct.unpack('@192h', first384bytes))
 
         fp = file if hasattr(file, 'write') else open(file, mode='wb')
         fp.seek(0, os.SEEK_END)
         if fp.tell() > 0:
             raise ValueError('You can only save() into an empty file.')
         try:
+            # the binary header and wave header
             fp.write(self._bin_header)
             fp.write(self._wave_header)
-            if TYPES[a.dtype.type] == 0: # text waves
+
+            # wave data
+            if TYPES[a.dtype.type] == 0:  # text waves
                 fp.write(b''.join(a.ravel(order='F')))
             else:
                 fp.write(a.tobytes(order='F'))
 
+            # extended data units, dimension units
             fp.write(self._extended_data_units)
             for u in self._extended_dimension_units:
                 fp.write(u)
+
+            # dimension labels
             for dimlabeldict in self._dimension_labels:
                 if dimlabeldict:
                     for i in range(-1, max(dimlabeldict)+1):
                         b = dimlabeldict.get(i, b'\x00')
                         b += b'\x00' * (32-len(b))
                         assert len(b) == 32
                         fp.write(b)
-            if TYPES[a.dtype.type] == 0:  # text waves
+
+            # string indices if this is a text wave.
+            if TYPES[a.dtype.type] == 0:
                 sindices = np.zeros(a.size, dtype=np.int32)
                 pos = 0
                 for idx, s in enumerate(a.ravel(order='F')):
                     pos += len(s)
                     sindices[idx] = pos
-                fp.write(sindices.tobytes(order='F'))
+                fp.write(sindices.tobytes())
         finally:
             if fp is not file:
                 fp.close()
 
     def save_itx(self, file, image=False):
         """save data as igor text (.itx) format.
 
         :param file: file name or text-file object.
         :param image: if True, rows and columns are transposed."""
         array = self._check_array(image=image)
-        name = self._wave_header.bname.decode()
+        name = self._wave_header.bname.decode(self._encoding)
 
-        fp = file if hasattr(file, 'write') else open(file, mode='w')
+        fp = file if hasattr(file, 'write') else open(file, encoding=self._encoding, mode='w')
         try:
             if fp.tell() == 0:
                 fp.write('IGOR\n')
             fp.write("WAVES {typ} /N=({shape}) '{name}'\n".format(
                 typ=ITX_TYPES[array.dtype.type],
                 shape=','.join(str(x) for x in array.shape),
                 name=name
             ))
             fp.write('BEGIN\n')
             if np.iscomplexobj(array):
                 def str_(x):
                     return '%s\t%s' % (x.real, x.imag)
-            elif ITX_TYPES[array.dtype.type] == '/T':
+            elif array.dtype.type is np.bytes_:
                 def str_(x):
-                    return '"' + self._escape_specials(x).decode(ENCODING) + '"'
+                    return '"' + self._escape_specials(x.decode(self._encoding)) + '"'
             else:
                 str_ = str
             # write in column/row/layer/chunk order
             expanded = array
             while expanded.ndim < 4:
                 expanded = np.expand_dims(expanded, expanded.ndim)
             for chunk in range(expanded.shape[3]):
@@ -342,84 +376,144 @@
                 name=name
             ))
             for idx, dim in list(enumerate(('x', 'y', 'z', 't')))[:array.ndim]:
                 dimUnits = self._wave_header.dimUnits[idx][:]
                 bunits = dimUnits.replace(b'\x00', b'') or self._extended_dimension_units[idx]
                 fp.write('X SetScale /P {dim},{start},{delta},"{units}",\'{name}\'\n'.format(
                     dim=dim, start=self._wave_header.sfB[idx], delta=self._wave_header.sfA[idx],
-                    units=bunits.decode(ENCODING),
+                    units=bunits.decode(self._encoding),
                     name=name
                 ))
             for dimNumber, dimlabeldict in enumerate(self._dimension_labels):
                 for dimIndex, blabel in dimlabeldict.items():
                     fp.write('X SetDimLabel {dimNumber},{dimIndex},\'{label}\',\'{name}\'\n'.format(
-                        dimNumber=dimNumber, dimIndex=dimIndex, label=blabel.decode(ENCODING), name=name
+                        dimNumber=dimNumber, dimIndex=dimIndex, label=blabel.decode(self._encoding), name=name
                     ))
         finally:
             if fp is not file:
                 fp.close()
 
     def _check_array(self, image=False):
         if not isinstance(self.array, np.ndarray):
             raise ValueError('Please set an array before save')
         a = self._cast_array()
-        if a.dtype.type not in TYPES:
-            raise TypeError('Unsupported dtype: %r' % a.dtype.type)
         if a.ndim > 4:
             raise ValueError('Dimension of more than 4 is not supported.')
 
         if image and a.ndim >= 2:
             # transpose row and column
             a = np.transpose(a, (1, 0) + tuple(range(2, a.ndim)))
         return a
 
     def _cast_array(self):
         # check array dtype and try type casting if necessary
         type_ = self.array.dtype.type
-        if type_ is np.float16:
-            return self.array.astype(np.float32)
-        if type_ is np.datetime64:
+        if type_ is np.bytes_:
+            # 255 means binary data
+            self._wave_header.textWaveContentEncoding = 255
+            a = self.array
+        elif (not self._int64_support) and type_ in (np.int64, np.uint64):
+            # Convert to 32-bit integers
+            to_type = {np.int64: np.int32, np.uint64: np.uint32}[type_]
+            tinfo = np.iinfo(to_type)
+            if (tinfo.min <= np.min(self.array)) and (np.max(self.array) <= tinfo.max):
+                a = self.array.astype(to_type)
+            else:
+                msg = (f'Overflow detected when converting an array with type {type_!r}. '
+                    'If you are using Igor Pro 7 or later, try setting int64_support=True when calling IgorWave().')
+                raise OverflowError(msg)
+        elif type_ is np.bool_:
+            a = self.array.astype(np.int8)
+        elif type_ is np.float16:
+            a = self.array.astype(np.float32)
+        elif type_ is np.clongdouble:
+            a = self.array.astype(np.float64)
+        elif type_ is np.datetime64:
             self.set_datascale('dat')
-            return (self.array - np.datetime64('1904-01-01 00:00:00')) / np.timedelta64(1, 's')
-        if type_ is np.str_:
-            return np.array([e.encode(ENCODING) for e in self.array.ravel()]).reshape(self.array.shape)
-        for from_, to_ in {np.int64: np.int32, np.uint64: np.uint32}.items():
-            if type_ is from_:
-                type_info = np.iinfo(to_)
-                if np.all((self.array >= type_info.min) & (self.array <= type_info.max)):
-                    return self.array.astype(to_)
-                else:
-                    raise TypeError('Cast from %r to %r failed.' % (type_, to_))
-        if type_ is np.object_:
+            a = (self.array - np.datetime64('1904-01-01 00:00:00')) / np.timedelta64(1, 's')
+        elif type_ is np.str_:
+            a = np.char.encode(self.array, encoding=self._encoding)
+        elif type_ is np.object_:
             # infer data type
-            candidates = [np.float64, np.bytes_, np.str_]
+            candidates = [np.float64, np.str_, np.bytes_]
             for t in candidates:
                 try:
                     a = self.array.astype(t)
+                except (ValueError, UnicodeError):
+                    continue
+                else:
                     msg = ("Data will be converted from np.object_ to numpy.{}. "
                            "To avoid this warning, "
                            "you may manually convert the data before calling IgorWave().").format(t.__name__)
                     if t is np.str_:
-                        a = np.array([e.encode(ENCODING) for e in a.ravel()]).reshape(a.shape)
+                        a = np.char.encode(a, encoding=self._encoding)
+                    elif t is np.bytes_:
+                        # 255 means binary data
+                        self._wave_header.textWaveContentEncoding = 255
                     warnings.warn(msg, category=TypeConversionWarning)
-                    return a
-                except Exception:
-                    pass
-        return self.array
+                    break
+            else:
+                raise ValueError('The array could not be converted to Igor-compatible types.')
+        elif type_ in TYPES:
+            a = self.array
+        else:
+            raise TypeError('The array data type %r is not compatible with Igor.' % type_)
+        assert a.dtype.type in TYPES
+        return a
+
+    def _parse_Series(self, s):
+        import pandas as pd
+        start, step = None, None
+        # parse pandas.Series objects
+        if isinstance(s.index, pd.MultiIndex):
+            msg = 'pandas MultiIndex is stripped because it is not compatible with Igor waves.'
+            warnings.warn(msg, StrippedSeriesIndexWarning)
+        elif isinstance(s.index, pd.RangeIndex):
+            start, step = s.index.start, s.index.step
+        else:
+            i = s.index.to_numpy()
+            if issubclass(i.dtype.type, np.number):
+                diff = np.diff(i)
+                if np.all(np.isclose(diff, diff[0], atol=0)):
+                    start, step = i[0], diff[0]
+                else:
+                    msg = 'pandas Index is stripped because it is not evenly spaced.'
+                    warnings.warn(msg, StrippedSeriesIndexWarning)
+            else:
+                msg = 'pandas Index is stripped because non-numeric scaling is not supported in Igor'
+                warnings.warn(msg, StrippedSeriesIndexWarning)
+        if start is not None:
+            self.set_dimscale('x', start, step)
+            if s.index.name:
+                try:
+                    self.set_dimlabel(0, -1, s.index.name)
+                except (InvalidNameError, ValueError):
+                    msg = 'index name is ignored because "{}" is not a valid dimension label.'.format(
+                        s.index.name)
+                    warnings.warn(msg)
+        if issubclass(s.dtype.type, Quantity):
+            self.set_datascale('{:~}'.format(s.pint.units))
+            s = s.pint.magnitude
+        return s.to_numpy()
+
+    def _parse_Pint(self, q):
+        # set units for pint.quantity._Quantity
+        self.set_datascale('{:~}'.format(q.units))
+        return q.magnitude
 
     @staticmethod
-    def _escape_specials(b: bytes):
+    def _escape_specials(s: str):
         # escape special characters
-        b = b.replace(b'\\', b'\\\\')
-        b = b.replace(b'\t', b'\\t')
-        b = b.replace(b'\r', b'\\r')
-        b = b.replace(b'\n', b'\\n')
-        b = b.replace(b'\'', b'\\\'')
-        b = b.replace(b'"', b'\\"')
-        return b
+        s = s.replace('\\', '\\\\')
+        s = s.replace('\t', '\\t')
+        s = s.replace('\r', '\\r')
+        s = s.replace('\n', '\\n')
+        s = s.replace('\'', '\\\'')
+        s = s.replace('"', '\\"')
+        return s
 
     @staticmethod
     def load(self, file):
         raise NotImplementedError
 
     def __repr__(self):
         return '<IgorWave \'%s\' at %s>' % (self.name, hex(id(self)))
```

### Comparing `igorwriter-0.4.1/igorwriter/utils.py` & `igorwriter-0.5.0/igorwriter/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from io import open
-
-import igorwriter
-from igorwriter import IgorWave
-
-
-def dict_to_itx(dict_like, path_or_buf, on_errors='fix'):
-    """
-
-    :param dict_like: dictionary-like object ({name: array-like, ...})
-    :param path_or_buf: filename or file-like object
-    :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise an exception.
-    :return: dictionary of generated waves ({name: wave, ...})
-    """
-    fp = path_or_buf if hasattr(path_or_buf, 'write') else open(path_or_buf, 'w', encoding=igorwriter.ENCODING)
-    wavelist = [IgorWave(array, name, on_errors) for (name, array) in dict_like.items()]
-    try:
-        for wave in wavelist:
-            wave.save_itx(fp)
-    finally:
-        if fp is not path_or_buf:
-            fp.close()
-    return {wave.name: wave for wave in wavelist}
-
-
-def dict_to_ibw(dict_like, prefix, on_errors='fix'):
-    """
-
-    :param dict_like: dictionary-like object ({name: array-like, ...})
-    :param prefix: file name prefix (each wave is saved as <prefix>_<column>.ibw)
-    :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise an exception.
-    :return: dictionary of generated waves ({name: wave, ...})
-    """
-    wavelist = [IgorWave(array, name, on_errors) for (name, array) in dict_like.items()]
-    for wave in wavelist:
-        wave.save(str(prefix) + '_%s.ibw' % wave.name)
-    return {wave.name: wave for wave in wavelist}
-
-
-dataframe_to_itx = dict_to_itx
-dataframe_to_ibw = dict_to_ibw
+import igorwriter
+from igorwriter import IgorWave
+
+
+def dict_to_itx(dict_like, path_or_buf, on_errors='fix'):
+    """
+
+    :param dict_like: dictionary-like object ({name: array-like, ...})
+    :param path_or_buf: filename or file-like object
+    :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise an exception.
+    :return: dictionary of generated waves ({name: wave, ...})
+    """
+    fp = path_or_buf if hasattr(path_or_buf, 'write') else open(path_or_buf, 'w', encoding=igorwriter.ENCODING)
+    wavelist = [IgorWave(array, name, on_errors) for (name, array) in dict_like.items()]
+    try:
+        for wave in wavelist:
+            wave.save_itx(fp)
+    finally:
+        if fp is not path_or_buf:
+            fp.close()
+    return {wave.name: wave for wave in wavelist}
+
+
+def dict_to_ibw(dict_like, prefix, on_errors='fix'):
+    """
+
+    :param dict_like: dictionary-like object ({name: array-like, ...})
+    :param prefix: file name prefix (each wave is saved as <prefix>_<column>.ibw)
+    :param on_errors: behavior when invalid name is given. 'fix': fix errors. 'raise': raise an exception.
+    :return: dictionary of generated waves ({name: wave, ...})
+    """
+    wavelist = [IgorWave(array, name, on_errors) for (name, array) in dict_like.items()]
+    for wave in wavelist:
+        wave.save(str(prefix) + '_%s.ibw' % wave.name)
+    return {wave.name: wave for wave in wavelist}
+
+
+dataframe_to_itx = dict_to_itx
+dataframe_to_ibw = dict_to_ibw
```

### Comparing `igorwriter-0.4.1/igorwriter/validator.py` & `igorwriter-0.5.0/igorwriter/validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function, unicode_literals
 from functools import wraps
 import warnings
 import re
+from locale import getpreferredencoding as _getpreferredencoding
 
-import igorwriter
 from igorwriter import builtin_names
 from igorwriter.errors import InvalidNameError, RenameWarning
 
 NG_LETTERS = ['"', '\'', ':', ';'] + [chr(i) for i in range(32)]
 
 
 def _fix_or_raise(fn, on_errors='raise'):
@@ -20,20 +18,22 @@
                 raise InvalidNameError(msg)
             else:
                 warnings.warn('name %r is fixed as %r (reason: %s)' % (name, fixed_name, msg), RenameWarning)
         return fixed_name
     return inner
 
 
-def _fix_length(name, max_bytes):
-    bname = name.encode(igorwriter.ENCODING)
+def _fix_length(name, max_bytes, encoding=None):
+    if encoding is None:
+        encoding = _getpreferredencoding()
+    bname = name.encode(encoding)
     if len(bname) == 0:
         name = 'wave0'
     if len(bname) > max_bytes:
-        while len(name.encode(igorwriter.ENCODING)) > max_bytes:
+        while len(name.encode(encoding)) > max_bytes:
             name = name[:-1]
     return name, 'Size of name must be between 1 and %d' % max_bytes
 
 
 def _fix_ng_letters(name):
     for s in NG_LETTERS:
         name = name.replace(s, '_')
@@ -49,28 +49,31 @@
 
 def _fix_conflicts(name):
     if name.lower() in (builtin_names.operations + builtin_names.functions + builtin_names.keywords + builtin_names.variables):
         name = name + '_'
     return name, 'name must not conflict with built-in operations, functions, etc.'
 
 
-def check_and_encode(name, liberal=True, long=False, on_errors='raise'):
+def check_and_encode(name, liberal=True, long=False, on_errors='raise', encoding=None):
     """
 
     :param name: name of an object
     :param liberal: whether Liberal Object Names are allowed or not
     :param long: whether Long Object Names (introduced in Igor 8.00) are allowed or not
-    :param on_errors: If 'raise', raises InvalidNameError when name is invalid. Otherwise tries to fix errors.
+    :param on_errors: If 'raise', raises InvalidNameError when name is invalid, otherwise tries to fix errors.
+    :param encoding: text encoding. If None, it is set with getpreferredencoding()
     :return:
     """
+    if encoding is None:
+        encoding = _getpreferredencoding()
     MAX_BYTES = 255 if long else 31
     name_before = name
     name_after = None
     while name_before != name_after:
         name_before = name
-        name = _fix_or_raise(_fix_length, on_errors=on_errors)(name_before, MAX_BYTES)
+        name = _fix_or_raise(_fix_length, on_errors=on_errors)(name_before, MAX_BYTES, encoding=encoding)
         name = _fix_or_raise(_fix_ng_letters, on_errors=on_errors)(name)
         if not liberal:
             name = _fix_or_raise(_fix_standard, on_errors=on_errors)(name)
         name = _fix_or_raise(_fix_conflicts, on_errors=on_errors)(name)
         name_after = name
-    return name.encode(igorwriter.ENCODING)
+    return name.encode(encoding)
```

### Comparing `igorwriter-0.4.1/setup.py` & `igorwriter-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='igorwriter',
-    version='0.4.1',
+    version='0.5.0',
     description='Write IGOR binary (.ibw) or text (.itx) files from numpy array',
     long_description=long_description,
     url='https://github.com/t-onoz/igorwriter',
     author='t-onoz',
     license='MIT',
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `igorwriter-0.4.1/tests/test_names.py` & `igorwriter-0.5.0/tests/test_names.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import warnings
 
 import igorwriter.errors
 
-try:
-    import unittest2 as unittest
-except ImportError:
-    import unittest
+import unittest
 from itertools import product
 
 import igorwriter
 from igorwriter import validator as v
 
+encoding = "utf-8"
 
 class NameTestCase(unittest.TestCase):
     def setUp(self):
         warnings.simplefilter('ignore', category=igorwriter.errors.RenameWarning)
 
     def test_empty_name(self):
         # empty string is invalid regardless of the modes.
@@ -26,15 +24,15 @@
                 self.assertEqual(bname, b'wave0')  # empty name is fixed as 'wave0'
 
     def test_long_names(self):
         for liberal, long in product((True, False), (True, False)):
             with self.subTest('32-bit length name', liberal=liberal, long=long):
                 name = 'x' * 32
                 if long:
-                    self.assertEqual(v.check_and_encode(name, liberal, long), name.encode(igorwriter.ENCODING))
+                    self.assertEqual(v.check_and_encode(name, liberal, long), name.encode(encoding))
                 else:
                     self.assertRaises(igorwriter.errors.InvalidNameError, v.check_and_encode, name, liberal, long)
                     bname = v.check_and_encode(name, liberal, long, on_errors='fix')
                     desired = b'x'*31
                     self.assertEqual(bname, desired)
             with self.subTest('256-bit length name', liberal=liberal, long=long):
                 name = 'x' * 256
@@ -56,15 +54,15 @@
     def test_liberal_names(self):
         names = ('wave 0', '0 wave', 'Wave0-1', ' '*31, '0'*31)
         desired_std_short = (b'wave_0', b'X0_wave', b'Wave0_1', b'X'+b'_'*30, b'X'+b'0'*30)
         desired_std_long = (b'wave_0', b'X0_wave', b'Wave0_1', b'X'+b'_'*31, b'X'+b'0'*31)
         for (name, desired_s, desired_l), liberal, long in product(zip(names, desired_std_short, desired_std_long), (True, False), (True, False)):
             if liberal:
                 bname = v.check_and_encode(name, liberal, long)
-                self.assertEqual(bname, name.encode(igorwriter.ENCODING))
+                self.assertEqual(bname, name.encode(encoding))
             else:
                 self.assertRaises(igorwriter.errors.InvalidNameError, v.check_and_encode, name, liberal, long)
                 bname = v.check_and_encode(name, liberal, long, on_errors='fix')
                 desired = desired_l if long else desired_s
                 self.assertEqual(bname, desired)
 
     def test_conflicts(self):
@@ -73,13 +71,13 @@
             'abs', 'ABS',  # functions
             'do', 'DO',  # keywords
             'k1', 'K1',  # variables
         )
         for name, liberal, long in product(names, (True, False), (True, False)):
             self.assertRaises(igorwriter.errors.InvalidNameError, v.check_and_encode, name, liberal, long)
             bname = v.check_and_encode(name, liberal, long, on_errors='fix')
-            desired = (name + '_').encode(igorwriter.ENCODING)
+            desired = (name + '_').encode(encoding)
             self.assertEqual(bname, desired)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `igorwriter-0.4.1/tests/test_utils.py` & `igorwriter-0.5.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-try:
-    import unittest2 as unittest
-except ImportError:
-    import unittest
-try:
-    from tempfile import TemporaryFile, TemporaryDirectory
-except ImportError:
-    from tempfile import TemporaryFile
-    from backports.tempfile import TemporaryDirectory
-
-import numpy as np
-
-from igorwriter import utils
-
-
-class UtilsTestCase(unittest.TestCase):
-    def test_pandas(self):
-        import pandas as pd
-        df = pd.DataFrame(
-            data={
-                'time': np.arange(0, 100, dtype=np.float64),
-                'colInt32': np.random.randint(-100, 100, 100).astype(np.int32),
-                'colUint32': np.random.randint(0, 100, 100).astype(np.uint32),
-                'colSingle': np.random.randint(-100, 100, 100).astype(np.float32),
-                'colDouble': np.random.randint(-100, 100, 100).astype(np.float64),
-                'colComp': np.random.randint(0, 100, 100).astype(np.complex128),
-            }
-        )
-        with TemporaryDirectory() as datadir:
-            utils.dataframe_to_itx(df, datadir + 'df.itx')
-            with open(datadir + 'df_fp.itx', 'w') as fp:
-                utils.dataframe_to_itx(df, fp)
-            utils.dataframe_to_ibw(df, datadir + 'df_bin')
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from tempfile import TemporaryFile, TemporaryDirectory
+
+import numpy as np
+
+from igorwriter import utils
+
+
+class UtilsTestCase(unittest.TestCase):
+    def test_pandas(self):
+        import pandas as pd
+        df = pd.DataFrame(
+            data={
+                'time': np.arange(0, 100, dtype=np.float64),
+                'colInt32': np.random.randint(-100, 100, 100).astype(np.int32),
+                'colUint32': np.random.randint(0, 100, 100).astype(np.uint32),
+                'colSingle': np.random.randint(-100, 100, 100).astype(np.float32),
+                'colDouble': np.random.randint(-100, 100, 100).astype(np.float64),
+                'colComp': np.random.randint(0, 100, 100).astype(np.complex128),
+            }
+        )
+        with TemporaryDirectory() as datadir:
+            utils.dataframe_to_itx(df, datadir + 'df.itx')
+            with open(datadir + 'df_fp.itx', 'w') as fp:
+                utils.dataframe_to_itx(df, fp)
+            utils.dataframe_to_ibw(df, datadir + 'df_bin')
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `igorwriter-0.4.1/tests/test_wave.py` & `igorwriter-0.5.0/tests/test_wave.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import unittest
 import os
-from tempfile import TemporaryFile
 from pathlib import Path
 
 import numpy as np
 
 import igorwriter.errors
 from igorwriter import IgorWave
-from igorwriter.igorwave import ENCODING
-from igorwriter.errors import TypeConversionWarning
+from igorwriter.errors import TypeConversionWarning, StrippedSeriesIndexWarning
 
 OUTDIR = Path(os.path.dirname(os.path.abspath(__file__))) / 'out'
+ENCODING = "utf-8"
 
 
 class WaveTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         OUTDIR.mkdir(exist_ok=True)
         for f in OUTDIR.glob('*'):
@@ -69,23 +68,58 @@
             with open(ibw, 'ab') as fp:
                 self.assertRaises(ValueError, wave.save, fp)
         with self.subTest('save in a truncated binary file'):
             with open(ibw, 'wb') as fp:
                 wave.save(fp)
 
     def test_array_type(self):
-        valid_types = (np.bool_, np.float16, np.int32, np.uint32, np.int64, np.uint64, np.float32, np.float64, np.complex128, np.object_, np.str_, np.bytes_)
+        valid_types = (np.bool_, np.float16, np.int32, np.uint32, np.int64, np.uint64, np.float32, np.float64, np.complex128, np.object_, np.str_, np.bytes_, int, float)
         for vt in valid_types:
             with self.subTest('type: %r' % vt):
                 wave = IgorWave(np.random.randint(0, 100, 10).astype(vt))
                 with open(OUTDIR / 'array_type_{}.ibw'.format(vt.__name__), 'wb') as fp:
                     wave.save(fp)
                 with open(OUTDIR / 'array_type_{}.itx'.format(vt.__name__), 'w') as fp:
                     wave.save_itx(fp)
 
+    def test_bool_to_itx(self):
+        a = np.array([True, True, True, True, True], dtype=np.bool_)
+        w = IgorWave(a, 'boolwave')
+        with open(OUTDIR / 'bool_to_itx.itx', 'w+t') as fp:
+            w.save_itx(fp)
+            fp.seek(0)
+            self.assertRegex(fp.read(), r'BEGIN\n1')
+
+    def test_int64(self):
+        # int64 and uint64 overflow
+        a = np.array([2**63 - 1]*10, dtype=np.int64)
+        an = -a
+        au = np.array([2**63 - 1]*10, dtype=np.uint64)
+        self.assertRaises(OverflowError, IgorWave(a).save, OUTDIR/'int64_overflow.ibw')
+        self.assertRaises(OverflowError, IgorWave(an).save, OUTDIR/'int64_overflow.ibw')
+        self.assertRaises(OverflowError, IgorWave(au).save, OUTDIR/'int64_unsigned_overflow.ibw')
+        w = IgorWave(a, int64_support=True)
+        w.save(OUTDIR/'int64.ibw')
+        self.assertEqual(w._wave_header.type, 0x80)
+        com = 'WAVES /L'
+        with open(OUTDIR / 'int64.itx', 'w+t', encoding='utf-8') as fp:
+            w.save_itx(fp)
+            fp.seek(0)
+            content = fp.read()
+            self.assertRegex(content, com)
+        w = IgorWave(au, int64_support=True)
+        w.save(OUTDIR/'int64_unsigned.ibw')
+        self.assertEqual(w._wave_header.type, 0x80+0x40)
+        com = 'WAVES /U/L'
+        with open(OUTDIR / 'int64_unsigned.itx', 'w+t', encoding='utf-8') as fp:
+            w.save_itx(fp)
+            fp.seek(0)
+            content = fp.read()
+            self.assertRegex(content, com)
+
     def test_dimscale(self):
         array = np.random.randint(0, 100, 10, dtype=np.int32)
         wave = IgorWave(array)
         wave.set_dimscale('x', 0, 0.01, 's')
         with open(OUTDIR / 'dimscale.ibw', 'wb') as fp:
             wave.save(fp)
         with open(OUTDIR / 'dimscale.itx', 'w') as fp:
@@ -131,15 +165,14 @@
         name = '\'invalid_name\''  # wave cannot contain quotation marks
         array = np.random.randint(0, 100, 10, dtype=np.int32)
         wave = IgorWave(array)
         self.assertRaises(igorwriter.errors.InvalidNameError, wave.rename, name, on_errors='raise')
         self.assertWarns(igorwriter.errors.RenameWarning, wave.rename, name, on_errors='fix')
         self.assertEqual(wave.name, name.replace('\'', '_'))
 
-
     def test_multiwave_itx(self):
         a = np.random.random(size=2*3*4*2)
         w1 = IgorWave(a, 'w_1d')
         w2 = IgorWave(a.reshape((2, -1)), 'w_2d')
         w3 = IgorWave(a.reshape((2, 3, -1)), 'w_3d')
         w4 = IgorWave(a.reshape((2, 3, 4, -1)), 'w_4d')
         with open(OUTDIR / 'multiwave_itx.itx', 'w+t') as fp:
@@ -292,10 +325,77 @@
             w = IgorWave(a, 'numeric_object')
             with open(OUTDIR / 'object_array_numeric.itx', 'w+t') as fp:
                 self.assertWarns(TypeConversionWarning, w.save_itx, fp)
                 fp.seek(0)
                 text = fp.read()
                 self.assertTrue('WAVES /D' in text)
 
+    def test_unicode_wave(self):
+        a = np.array(['Hello', '你好', 'こんにちは', '안녕하세요'], dtype=np.str_)
+        w = IgorWave(a, 'H你こ안', unicode=True)
+        w.save(OUTDIR / 'unicode_wave.ibw')
+        self.assertEqual(w._wave_header.waveNameEncoding, 1)
+        self.assertEqual(w._wave_header.waveUnitsEncoding, 1)
+        self.assertEqual(w._wave_header.waveNoteEncoding, 1)
+        self.assertEqual(w._wave_header.waveDimLabelEncoding, 1)
+        self.assertEqual(w._wave_header.textWaveContentEncoding, 1)
+        w.save_itx(OUTDIR / 'unicode_wave.itx')
+        with open(OUTDIR / 'unicode_wave.itx', encoding='utf-8') as f:
+            f.read()
+
+    def test_pandas_series(self):
+        import pandas as pd
+        with self.subTest('simple Series object'):
+            s = pd.Series([1, 2, 3, 4, 5, 6])
+            w = IgorWave(s, 'serieswave')
+        with self.subTest('Series object with uniform Index'):
+            s = pd.Series([1, 2, 3, 4, 5, 6])
+            s.index = np.linspace(1, 2, 6)
+            w = IgorWave(s, 'series_uniformind')
+            self.assertAlmostEqual(w._wave_header.sfA[0], 0.2)
+            self.assertAlmostEqual(w._wave_header.sfB[0], 1.0)
+        with self.subTest('Series object with invalid Index names'):
+            s = pd.Series([1, 2, 3, 4, 5, 6])
+            s.index = np.linspace(1, 2, 6)
+            for n in ('\'', 'a'*32):
+                s.index.name = n
+                with self.assertWarns(UserWarning):
+                    w = IgorWave(s)
+                self.assertAlmostEqual(w._wave_header.sfA[0], 0.2)
+                self.assertAlmostEqual(w._wave_header.sfB[0], 1.0)
+                self.assertNotIn(-1, w._dimension_labels[0])
+        with self.subTest('Series object with uniform Index with a name'):
+            s.index.name = 'myindex'
+            w = IgorWave(s, 'series_uniformind')
+            self.assertEqual(w._dimension_labels[0][-1], b'myindex')
+        with self.subTest('Series object with nonuniform Index'):
+            s = pd.Series([1, 2, 3])
+            s.index = [1, 2, 3.05]
+            s.index.name = 'myindex'
+            with self.assertWarns(StrippedSeriesIndexWarning):
+                w = IgorWave(s, 'series_nonuniformind')
+            # when index is invalid, dimension labels should be empty
+            self.assertAlmostEqual(w._wave_header.sfA[0], 1)
+            self.assertAlmostEqual(w._wave_header.sfB[0], 0)
+            self.assertNotIn(-1, w._dimension_labels[0])
+        with self.subTest('Series object with incompatible dtype Index'):
+            s = pd.Series([1, 2, 3])
+            s.index = [1, 2, 'spam']
+            s.index.name = 'myindex'
+            with self.assertWarns(StrippedSeriesIndexWarning):
+                w = IgorWave(s, 'series_invalidind')
+            # when index is invalid, dimension labels should be empty
+            self.assertAlmostEqual(w._wave_header.sfA[0], 1)
+            self.assertAlmostEqual(w._wave_header.sfB[0], 0)
+            self.assertNotIn(-1, w._dimension_labels[0])
+        with self.subTest('pint-pandas extended types'):
+            import pint_pandas
+            u = "kg m / s**2"
+            s = pd.Series([1.0, 2.0, 2.0, 3.0], dtype=f"pint[{u}]")
+            expected = '{:~}'.format(s.pint.units).encode(ENCODING)
+            wave = IgorWave(s)
+            bunits = wave._extended_data_units
+            self.assertEqual(bunits, expected)
+
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

