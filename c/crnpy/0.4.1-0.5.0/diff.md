# Comparing `tmp/crnpy-0.4.1.tar.gz` & `tmp/crnpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.4.1.tar", last modified: Mon Jul  3 22:20:08 2023, max compression
+gzip compressed data, was "crnpy-0.5.0.tar", last modified: Sat Jul  8 00:36:07 2023, max compression
```

## Comparing `crnpy-0.4.1.tar` & `crnpy-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 22:19:59.000000 crnpy-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 22:20:08.664037 crnpy-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 22:19:59.000000 crnpy-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:20:08.664037 crnpy-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 22:19:59.000000 crnpy-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 00:35:54.000000 crnpy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-08 00:36:07.013567 crnpy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 00:35:54.000000 crnpy-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:36:07.013567 crnpy-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-08 00:35:54.000000 crnpy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.009567 crnpy-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58403 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-08 00:35:54.000000 crnpy-0.5.0/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:36:07.013567 crnpy-0.5.0/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:36:07.000000 crnpy-0.5.0/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 00:36:06.000000 crnpy-0.5.0/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.4.1/LICENSE` & `crnpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.4.1/PKG-INFO` & `crnpy-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://github.com/soilwater/crnpy
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,36 +16,37 @@
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
-Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
+Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
-- Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
-- Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
-Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
+- Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
 ## Installation
 
-To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
+To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
+from the Jupyter notebook, type:
+
+```!pip install crnpy```
+
 ## Authors
 
-The CRNPy library was developed by:
+The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
+
 - Andres Patrignani
 
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University combines a range of experimental and computational approaches to tackle pressing issues in soil and water research. The development of the CRNPy library is a step forward to creating reproducible data processing workflows across the scientific community using cosmic-ray neutrons probes for soil moisture sensing.
```

### Comparing `crnpy-0.4.1/README.md` & `crnpy-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
-Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
+Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
-- Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
-- Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
-Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
+- Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
 ## Installation
 
-To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
+To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
+from the Jupyter notebook, type:
+
+```!pip install crnpy```
+
 ## Authors
 
-The CRNPy library was developed by:
+The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
+
 - Andres Patrignani
 
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University combines a range of experimental and computational approaches to tackle pressing issues in soil and water research. The development of the CRNPy library is a step forward to creating reproducible data processing workflows across the scientific community using cosmic-ray neutrons probes for soil moisture sensing.
```

### Comparing `crnpy-0.4.1/setup.py` & `crnpy-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # contents of setup.py
 import setuptools
 
 setuptools.setup(
     name="crnpy",
-    version="0.4.1",
+    version="0.5.0",
     packages=['crnpy'],
     package_dir = {"": "src"},
     description="A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.",
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/soilwater/crnpy",
```

### Comparing `crnpy-0.4.1/src/crnpy/crnpy.py` & `crnpy-0.5.0/src/crnpy/crnpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,170 +70,170 @@
             source = pd.concat([df,new_line])
 
     df.sort_values(by=col, inplace=True)
     df.reset_index(drop=True, inplace=True)
     df.set_index(col, inplace=True)
     return df
 
-def count_time(counts=None, timestamp_col=None):
+def get_integration_time(counts=None, timestamp_col=None):
     """Approximate counting time.
     The function will calculate the approximate counting time for each observation by taking the difference between
     consecutive timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
 
     Args:
         counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
         timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
 
     Returns:
         (pandas.Series): Series with the approximate counting time for each observation.
 
     Examples:
-        Using `count_time` in a console environment:
+        Using `get_integration_time` in a console environment:
 
         >>> df = pd.DataFrame(...)
-        >>> count_time(timestamp_col=df['timestamp'])
+        >>> get_integration_time(timestamp_col=df['timestamp'])
         0   3600.0
         1   3600.0
         2   3600.0
     """
     if timestamp_col is not None:
         if not isinstance(timestamp_col, pd.Series):
             raise TypeError('timestamp_col must be a pandas Series.')
         if timestamp_col.dtype != 'datetime64[ns]':
             raise TypeError('timestamp_col must be a pandas Series with datetime64[ns] dtype.')
 
-        count_time = timestamp_col.diff().dt.total_seconds()
-        return count_time
+        integration_time = timestamp_col.diff().dt.total_seconds()
+        return integration_time
 
     if counts is not None:
         if not isinstance(counts, pd.DataFrame):
             raise TypeError('counts must be a pandas DataFrame.')
 
         if not counts.index.dtype == 'datetime64[ns]':
             raise TypeError('counts must have a DateTimeIndex.')
 
-        count_time = counts.index.to_series().diff().dt.total_seconds()
-        return count_time
+        integration_time = counts.index.to_series().diff().dt.total_seconds()
+        return integration_time
 
     raise TypeError('Either counts or timestamp_col must be provided.')
 
-def fill_counts(counts, count_times=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
+def fill_counts(counts, actual_integration_time=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
     """Fill missing neutron counts. Observation periods shorter than threshold are discarded (replaced with NaN).
-    
+
     Args:
         counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
+        actual_integration_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
         timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
-        expected_time (int): Expected counting time in seconds. If not provided, it is calculated as the median of the counting times.
+        expected_time (int): Expected integration time in seconds. If not provided, it is calculated as the median of the counting times.
         threshold (float): Minimum fraction of the neutron integration time. Default is 0.25.
 
     Returns:
         (pandas.DataFrame): DataFrame with linearly interpolated neutron counts.
 
     Examples:
         Using `fill_counts` in a console environment:
 
         >>> counts = pd.DataFrame({'counts':[100,105,98,102], count_time:[3600,200,3600,3600]})
-        >>> fill_counts(counts, count_time=count_time, expected_time=3600, threshold=0.25)
+        >>> fill_counts(counts, actual_integration_time=counts['actual_integration_time'], expected_time=3600, threshold=0.25)
         0   100.0
         1   NaN
         2   98.0
         3   102.0
     """
 
     counts=counts.copy()
 
-    if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
+    if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(actual_integration_time, type(None)):
         print("No count time columns provided. Using timestamp index to compute count time.")
-        count_times = count_time(timestamp_col=counts.index.to_series())
+        actual_integration_time = get_integration_time(timestamp_col=counts.index.to_series())
 
-    elif not isinstance(timestamp_col, type(None)) and isinstance(count_times, type(None)):
+    elif not isinstance(timestamp_col, type(None)) and isinstance(actual_integration_time, type(None)):
         if timestamp_col.dtype != 'datetime64[ns]':
             if len(timestamp_col) != len(counts):
                 raise ValueError('Timestamp column length does not match number of readings.')
             print("No count time columns provided. Using timestamp column to compute count time.")
-            count_times = count_time(timestamp_col=timestamp_col)
+            actual_integration_time = get_integration_time(timestamp_col=timestamp_col)
         else:
             raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
 
-    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)) and isinstance(timestamp_col, type(None)):
+    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(actual_integration_time, type(None)) and isinstance(timestamp_col, type(None)):
         raise ValueError('Count_times must be provided, or timestamp_col must be provided, or counts must have a DatetimeIndex.')
 
-    if len(counts) != len(count_times):
+    if len(counts) != len(actual_integration_time):
         raise ValueError('Count times length does not match number of readings.')
 
     if expected_time is False:
-        expected_time = count_times.median()
+        expected_time = actual_integration_time.median()
         print('Using median count time as expected count time:', expected_time)
 
     # Replace values below threshold with NaN
     time_threshold = round(expected_time * threshold)
 
-    if type(count_times) == pd.core.frame.DataFrame:
-        if len(count_times.columns) == 1:
-            idx_nan = count_times[count_times < time_threshold].index
+    if type(actual_integration_time) == pd.core.frame.DataFrame:
+        if len(actual_integration_time.columns) == 1:
+            idx_nan = actual_integration_time[actual_integration_time < time_threshold].index
             counts.loc[idx_nan] = np.nan
         else:
-            for i in range(len(count_times.columns)):
-                idx_nan = count_times[count_times.iloc[:,i] < time_threshold].index
+            for i in range(len(actual_integration_time.columns)):
+                idx_nan = actual_integration_time[actual_integration_time.iloc[:, i] < time_threshold].index
                 counts.iloc[:,i].loc[idx_nan] = np.nan
-    elif type(count_times) == pd.core.series.Series:
-        idx_nan = count_times[count_times < time_threshold].index
+    elif type(actual_integration_time) == pd.core.series.Series:
+        idx_nan = actual_integration_time[actual_integration_time < time_threshold].index
         counts.loc[idx_nan] = np.nan
-    elif type(count_times) == np.ndarray:
-        idx_nan = np.where(count_times < time_threshold)
+    elif type(actual_integration_time) == np.ndarray:
+        idx_nan = np.where(actual_integration_time < time_threshold)
         counts.loc[idx_nan] = np.nan
 
     # Fill missing values with linear interpolation and round to nearest integer
     counts = counts.interpolate(method='linear', limit=limit, limit_direction='both').round()
     return counts
 
-def adjust_temporal_counts(counts, count_time=None, count_times=None, timestamp_col=None):
-    """Normalize neutron counts to the desired counting time.
-    
+def adjust_temporal_counts(counts, nominal_integration_time=None, actual_integration_time=None, timestamp_col=None):
+    """Adjust neutron counts for the desired integration time.
+
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
-        count_time (int): Count time in seconds for normalization. Default is 3600 seconds.
-        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
-        timestamp_col (pandas.Series): Timestamp column, used to calculate count time if count_times is not provided, it must have the same number of rows as counts.
-        
+        nominal_integration_time (int): Nominal intgration time in seconds.
+        actual_integration_time (pandas.Series or pandas.DataFrame): Actual integration time of each measurement in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
+        timestamp_col (pandas.Series): Timestamp column, used to calculate integration time if actual_integration_time is not provided, it must have the same number of rows as counts.
+
     Returns:
-        (pandas.DataFrame): Normalized neutron counts.
+        (pandas.DataFrame): Neutron counts adjusted for the desired integration time.
 
     """
 
-    if count_times is None and type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex:
+    if actual_integration_time is None and type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex:
         print("No count_times columns provided. Using timestamp index to compute count time.")
-        count_times = counts.index.to_series().diff().dt.total_seconds()
+        actual_integration_time = counts.index.to_series().diff().dt.total_seconds()
 
-    elif count_times is None and not isinstance(timestamp_col, type(None)):
+    elif actual_integration_time is None and not isinstance(timestamp_col, type(None)):
         if len(timestamp_col) != len(counts):
             raise ValueError('Timestamp column length does not match number of readings.')
         print("No count_times columns provided. Using timestamp column to compute count time.")
         if timestamp_col.dtype != 'datetime64[ns]':
             raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-        count_times = count_time(timestamp_col=timestamp_col)
+        actual_integration_time = get_integration_time(timestamp_col=timestamp_col)
 
 
-    if isinstance(count_times, type(None)):
-        raise ValueError('Count time must be provided, or `timestamp_col` must be provided, or counts must have a DatetimeIndex.')
+    if isinstance(actual_integration_time, type(None)):
+        raise ValueError('Actual integration time must be provided, or `timestamp_col` must be provided, or counts must have a DatetimeIndex.')
 
-    if len(counts) != len(count_times):
+    if len(counts) != len(actual_integration_time):
         raise ValueError('Count times length does not match number of readings.')
 
     #Normalize counts rounded to integer
-    if type(count_times) == pd.core.series.Series or len(count_times.columns) == 1:
-        normalized_counts = counts.div(count_times, axis=0).mul(count_time).round()
-        return normalized_counts
+    if type(actual_integration_time) == pd.core.series.Series or len(actual_integration_time.columns) == 1:
+        adjusted_counts = counts.div(actual_integration_time, axis=0).mul(nominal_integration_time).round()
+        return adjusted_counts
     else:
-        normalized_counts = counts.copy()
-        count_times = count_times.copy()
+        adjusted_counts = counts.copy()
+        count_times = actual_integration_time.copy()
         for i in range(len(count_times.columns)):
-            normalized_counts[normalized_counts.columns[i]] = normalized_counts.iloc[:,i].div(count_times.iloc[:,i], axis=0).mul(count_time).round()
-        return normalized_counts
+            adjusted_counts[adjusted_counts.columns[i]] = adjusted_counts.iloc[:,i].div(count_times.iloc[:,i], axis=0).mul(nominal_integration_time).round()
+        return adjusted_counts
 
 
 def compute_total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
     """Compute the sum of uncorrected neutron counts for all detectors.
 
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
@@ -271,15 +271,15 @@
     # Replace zeros with NaN
     total_raw_counts = total_raw_counts.replace(0, np.nan)
     return total_raw_counts
 
 
 def drop_outliers(raw_counts, window=5, store_outliers=False, min_counts=None, max_counts=None):
     """Computation of a moving modified Z-score based on the median absolute difference.
-    
+
     Args:
         raw_counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         window (int): Window size for the moving median. Default is 11.
         store_outliers (bool): If True, store the outliers in a new column. Default is False.
         min_counts (int): Minimum number of counts for a reading to be considered valid. Default is None.
         max_counts (int): Maximum number of counts for a reading to be considered valid. Default is None.
 
@@ -338,16 +338,16 @@
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.interpolate.html
     """
 
     # Fill missing values in atmospheric variables
     return cols_atm.interpolate(method='pchip', limit=limit, limit_direction='both')
 
 
-def pressure_correction(raw_counts, pressure, Pref, L):
-    r"""Correct neutron counts for atmospheric pressure.
+def pressure_correction(pressure, Pref, L):
+    r"""Correction factor for atmospheric pressure.
 
     This function corrects neutron counts for atmospheric pressure using the method described in Andreasen et al. (2017).
     The correction is performed using the following equation:
 
     $$
     C_{corrected} = \frac{C_{raw}}{fp}
     $$
@@ -366,35 +366,33 @@
 
     - P: atmospheric pressure
     - Pref: reference atmospheric pressure
     - L: Atmospheric attenuation coefficient.
 
 
     Args:
-        raw_counts (list or array): Neutron counts to correct.
-        pressure (list or array): Atmospheric pressure readings. Long-term average pressure is recommended.
+        atm_pressure (list or array): Atmospheric pressure readings. Long-term average pressure is recommended.
         Pref (float): Reference atmospheric pressure.
         L (float): Atmospheric attenuation coefficient.
 
     Returns:
-        (list): Corrected neutron counts.
+        (list): fp pressure correction factor.
 
     References:
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
 
     # Compute pressure correction factor
     fp = np.exp((Pref - pressure) / L) # Zreda et al. 2017 Eq 5.
-    # Compute corrected neutron counts
-    corrected_counts = raw_counts / fp
-    return np.round(corrected_counts)
+
+    return fp
 
 
-def humidity_correction(raw_counts, humidity, temp, Aref):
-    r"""Correct neutron counts for absolute humidity.
+def humidity_correction(abs_humidity, Aref):
+    r"""Correction factor for absolute humidity.
 
     This function corrects neutron counts for absolute humidity using the method described in Rosolem et al. (2013) and Anderson et al. (2017). The correction is performed using the following equation:
 
     $$
     C_{corrected} = C_{raw} \cdot f_w
     $$
 
@@ -410,33 +408,30 @@
 
     where:
 
     - A: absolute humidity
     - Aref: reference absolute humidity
 
     Args:
-        raw_counts (list or array): Neutron counts to correct.
-        humidity (list or array): Relative humidity readings.
+        abs_humidity (list or array): Relative humidity readings.
         temp (list or array): Temperature readings (Celsius).
         Aref (float): Reference absolute humidity (g/m^3). The day of the instrument calibration is recommended.
 
     Returns:
-        (list): Corrected neutron counts.
+        (list): fw correction factor.
 
     References:
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
     """
-
-    A = estimate_abs_humidity(humidity, temp)
+    A = abs_humidity
     fw = 1 + 0.0054*(A - Aref) # Zreda et al. 2017 Eq 6.
-    corrected_counts = raw_counts * fw
-    return np.round(corrected_counts)
+    return fw
 
-def incoming_flux_correction(raw_counts, incoming_neutrons, incoming_Ref=None):
-    r"""Correct neutron counts for incoming neutron flux.
+def incoming_flux_correction(incoming_neutrons, incoming_Ref=None):
+    r"""Correction factor for incoming neutron flux.
 
     This function corrects neutron counts for incoming neutron flux using the method described in Anderson et al. (2017). The correction is performed using the following equation:
 
     $$
     C_{corrected} = \frac{C_{raw}}{f_i}
     $$
 
@@ -452,34 +447,32 @@
 
     where:
 
     - I: incoming neutron flux
     - Iref: reference incoming neutron flux
 
     Args:
-        raw_counts (list or array): Neutron counts to correct.
         incoming_neutrons (list or array): Incoming neutron flux readings.
         incoming_Ref (float): Reference incoming neutron flux. Baseline incoming neutron flux.
 
     Returns:
-        (list): Corrected neutron counts.
+        (list): fi correction factor.
 
     References:
         M. Andreasen, K.H. Jensen, D. Desilets, T.E. Franz, M. Zreda, H.R. Bogena, and M.C. Looms. 2017. Status and perspectives on the cosmic-ray neutron method for soil moisture estimation and other environmental science applications. Vadose Zone J. 16(8). doi:10.2136/vzj2017.04.0086
 
 
     """
     if incoming_Ref is None and not isinstance(incoming_neutrons, type(None)):
         incoming_Ref = incoming_neutrons[0]
         warnings.warn('Reference incoming neutron flux not provided. Using first value of incoming neutron flux.')
     fi = incoming_neutrons / incoming_Ref
     fi.fillna(1.0, inplace=True)  # Use a value of 1 for days without data
 
-    # Apply correction factors
-    return np.round(raw_counts / fi)
+    return fi
 
 
 def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window = 0,  verbose=False):
     """Function to retrieve neutron flux from the Neutron Monitor Database.
 
     Args:
         start_date (datetime): Start date of the time series.
@@ -716,18 +709,18 @@
         N0 (float): Device-specific neutron calibration constant.
         Wlat (float): Lattice water content.
         Wsoc (float): Soil organic carbon content.
         bulk_density (float): Soil bulk density.
         a0 (float): Parameter given in Zreda et al., 2012. Default is 0.0808.
         a1 (float): Parameter given in Zreda et al., 2012. Default is 0.372.
         a2 (float): Parameter given in Zreda et al., 2012. Default is 0.115.
-        
+
     Returns:
         (array or pd.Series or pd.DataFrame): Volumetric water content in m3 m-3.
-        
+
     References:
         Desilets, D., M. Zreda, and T.P.A. Ferré. 2010. Nature’s neutron probe:
         Land surface hydrology at an elusive scale with cosmic rays. Water Resour. Res. 46:W11505.
         doi.org/10.1029/2009WR008726
     """
 
     # Convert neutron counts into vwc
@@ -781,33 +774,33 @@
     elif method == 'Franz_2012':
         results = 5.8/(bulk_density*Wlat+vwc+0.0829)
     else:
         raise ValueError('Method not recognized. Please select either "Schron_2017" or "Franz_2012".')
 
     return results
 
-def estimate_abs_humidity(RH, temp):
+def estimate_abs_humidity(relative_humidity, temp):
     """
     Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
 
     Args:
-        RH (float): relative humidity (%)
+        relative_humidity (float): relative humidity (%)
         temp (float): temperature (Celsius)
 
     Returns:
         float: actual vapor pressure (g m^-3)
     """
 
     ### Atmospheric water vapor factor
     # Saturation vapor pressure
     e_sat = 0.611 * np.exp(17.502 * temp / (
                 temp + 240.97)) * 1000  # in Pascals Eq. 3.8 p.41 Environmental Biophysics (Campbell and Norman)
 
     # Vapor pressure Pascals
-    Pw = e_sat * RH / 100
+    Pw = e_sat * relative_humidity / 100
 
     # Absolute humidity (g/m^3)
     C = 2.16679  # g K/J;
     abs_h = C * Pw / (temp + 273.15)
     return abs_h
 
 
@@ -985,24 +978,24 @@
     zq = griddata(points, values, (xq,yq))
 
     return np.round(zq,2)
 
 
 def find_neutron_monitor(Rc, start_date=None, end_date=None):
     """Search for potential reference neutron monitoring stations based on cutoff rigidity.
-    
+
     Args:
         Rc (float): Cutoff rigidity in GV. Values in range 1.0 to 3.0 GV.
-        start_date (datetime): Start date for the period of interest.   
+        start_date (datetime): Start date for the period of interest.
         end_date (datetime): End date for the period of interest.
-        
+
     Returns:
         (list): List of top five stations with closes cutoff rigidity.
             User needs to select station according to site altitude.
-            
+
     Examples:
         >>> from crnpy import crnpy
         >>> Rc = 2.40 # 2.40 Newark, NJ, US
         >>> crnpy.find_neutron_monitor(Rc)
         Select a station with an altitude similar to that of your location. For more information go to: 'https://www.nmdb.eu/nest/help.php#helpstations
 
         Your cutoff rigidity is 2.4 GV
```

### Comparing `crnpy-0.4.1/src/crnpy/data.py` & `crnpy-0.5.0/src/crnpy/data.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.4.1/src/crnpy.egg-info/PKG-INFO` & `crnpy-0.5.0/src/crnpy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://github.com/soilwater/crnpy
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,36 +16,37 @@
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
-Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
+Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
-- Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
-- Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Versatile and instrument agnostic: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
-Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
+- Modular: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
 
 
 ## Installation
 
-To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
+To install the CRNPy library, you can use Python's package manager. Open a terminal and type:
 
 ```pip install crnpy```
 
+from the Jupyter notebook, type:
+
+```!pip install crnpy```
+
 ## Authors
 
-The CRNPy library was developed by:
+The CRNPy library was developed at the Kansas State University Soil Water Processes Lab by:
 
 - Joaquin Peraza
+
 - Andres Patrignani
 
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University combines a range of experimental and computational approaches to tackle pressing issues in soil and water research. The development of the CRNPy library is a step forward to creating reproducible data processing workflows across the scientific community using cosmic-ray neutrons probes for soil moisture sensing.
```

