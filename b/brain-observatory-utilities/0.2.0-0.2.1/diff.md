# Comparing `tmp/brain_observatory_utilities-0.2.0.tar.gz` & `tmp/brain_observatory_utilities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain_observatory_utilities-0.2.0.tar", last modified: Sat Jul  8 02:58:37 2023, max compression
+gzip compressed data, was "brain_observatory_utilities-0.2.1.tar", last modified: Sat Jul  8 03:29:43 2023, max compression
```

## Comparing `brain_observatory_utilities-0.2.0.tar` & `brain_observatory_utilities-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.596506 brain_observatory_utilities-0.2.0/
--rw-rw-rw-   0        0        0     1987 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1840 2023-07-08 02:58:37.597505 brain_observatory_utilities-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1049 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.286683 brain_observatory_utilities-0.2.0/brain_observatory_utilities/
--rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.326660 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/
--rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.350646 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/
--rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/__init__.py
--rw-rw-rw-   0        0        0    10837 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/data_access.py
--rw-rw-rw-   0        0        0    36394 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/data_formatting.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.434600 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/
--rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/__init__.py
--rw-rw-rw-   0        0        0     4487 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/ccf_tools.py
--rw-rw-rw-   0        0        0    24816 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/receptive_field_mapping.py
--rw-rw-rw-   0        0        0     5560 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.506577 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/
--rw-rw-rw-   0        0        0       98 2022-08-23 17:41:24.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/__init__.py
--rw-rw-rw-   0        0        0     3432 2022-08-23 19:27:14.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/data_access.py
--rw-rw-rw-   0        0        0    29218 2023-04-19 02:08:06.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/data_formatting.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.570520 brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/__init__.py
--rw-rw-rw-   0        0        0     7991 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/behavior_plots.py
--rw-rw-rw-   0        0        0     5607 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/ophys_plots.py
--rw-rw-rw-   0        0        0     4109 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/plot_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.595506 brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/
--rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/__init__.py
--rw-rw-rw-   0        0        0    20104 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/general_utilities.py
--rw-rw-rw-   0        0        0     8632 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/trial_utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:58:37.324661 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/
--rw-rw-rw-   0        0        0     1840 2023-07-08 02:58:36.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1435 2023-07-08 02:58:36.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:58:36.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-08 02:58:36.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-08 02:58:36.000000 brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      169 2023-07-08 02:58:37.599504 brain_observatory_utilities-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-07-08 02:48:25.000000 brain_observatory_utilities-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.712648 brain_observatory_utilities-0.2.1/
+-rw-rw-rw-   0        0        0     1987 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1840 2023-07-08 03:29:43.712648 brain_observatory_utilities-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.550720 brain_observatory_utilities-0.2.1/brain_observatory_utilities/
+-rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.575706 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/
+-rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.587699 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/
+-rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/__init__.py
+-rw-rw-rw-   0        0        0    10837 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/data_access.py
+-rw-rw-rw-   0        0        0    37947 2023-07-08 03:18:25.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/data_formatting.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.618701 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/
+-rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/__init__.py
+-rw-rw-rw-   0        0        0     4487 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/ccf_tools.py
+-rw-rw-rw-   0        0        0    24816 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/receptive_field_mapping.py
+-rw-rw-rw-   0        0        0     5560 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.650671 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/
+-rw-rw-rw-   0        0        0       98 2022-08-23 17:41:24.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/__init__.py
+-rw-rw-rw-   0        0        0     3432 2022-08-23 19:27:14.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/data_access.py
+-rw-rw-rw-   0        0        0    29218 2023-04-19 02:08:06.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/data_formatting.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.687642 brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:15:24.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/__init__.py
+-rw-rw-rw-   0        0        0     7991 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/behavior_plots.py
+-rw-rw-rw-   0        0        0     5607 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/ophys_plots.py
+-rw-rw-rw-   0        0        0     4109 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/plot_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.710629 brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/
+-rw-rw-rw-   0        0        0        0 2022-08-22 23:26:12.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/__init__.py
+-rw-rw-rw-   0        0        0    20104 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/general_utilities.py
+-rw-rw-rw-   0        0        0     8632 2023-07-08 02:48:17.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/trial_utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:29:43.573708 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1840 2023-07-08 03:29:43.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2023-07-08 03:29:43.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:29:43.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-08 03:29:43.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-08 03:29:43.000000 brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      169 2023-07-08 03:29:43.714628 brain_observatory_utilities-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-07-08 03:25:11.000000 brain_observatory_utilities-0.2.1/setup.py
```

### Comparing `brain_observatory_utilities-0.2.0/LICENSE` & `brain_observatory_utilities-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/PKG-INFO` & `brain_observatory_utilities-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain_observatory_utilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for analyzing, manipulating and visualizing data for Brain Observatory projects
 Home-page: https://github.com/AllenInstitute/mindscope_utilities
 Author: Allen Institute
 Author-email: corbettb@alleninstitute.org, michaelbu@alleninstitute.org, marinag@alleninstitute.org, clark.roll@alleninstitute.org
 License: Allen Institute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `brain_observatory_utilities-0.2.0/README.md` & `brain_observatory_utilities-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/data_access.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/data_access.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/behavior/data_formatting.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/behavior/data_formatting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import numpy as np
-from allensdk.brain_observatory.behavior.trials_processing import calculate_reward_rate
 from brain_observatory_utilities.utilities.general_utilities import get_trace_average
 import brain_observatory_utilities.datasets.behavior.data_access as data_access
 from brain_observatory_utilities.utilities import general_utilities
 
 
 def add_mean_running_speed_to_stimulus_presentations(stimulus_presentations,
                                                      running_speed,
@@ -199,14 +198,56 @@
             ((lick_times > row["start_time"] + time_window[0]) & (lick_times < row["start_time"] + time_window[1]))],
         axis=1,
     )
     stimulus_presentations["licks"] = licks_each_stim
     return stimulus_presentations
 
 
+def calculate_reward_rate(response_latency=None,
+                          starttime=None,
+                          window=0.75,
+                          trial_window=25,
+                          initial_trials=10):
+
+    assert len(response_latency) == len(starttime)
+
+    df = pd.DataFrame({'response_latency': response_latency,
+                       'starttime': starttime})
+
+    # adds a column called reward_rate to the input dataframe
+    # the reward_rate column contains a rolling average of rewards/min
+    # window sets the window in which a response is considered correct,
+    # so a window of 1.0 means licks before 1.0 second are considered correct
+    #
+    # Reorganized into this unit-testable form by Nick Cain April 25 2019
+
+    reward_rate = np.zeros(len(df))
+    # make the initial reward rate infinite,
+    # so that you include the first trials automatically.
+    reward_rate[:initial_trials] = np.inf
+
+    for trial_number in range(initial_trials, len(df)):
+
+        min_index = np.max((0, trial_number - trial_window))
+        max_index = np.min((trial_number + trial_window, len(df)))
+        df_roll = df.iloc[min_index:max_index]
+
+        # get a rolling number of correct trials
+        correct = len(df_roll[df_roll.response_latency < window])
+
+        # get the time elapsed over the trials
+        time_elapsed = df_roll.starttime.iloc[-1] - df_roll.starttime.iloc[0]
+
+        # calculate the reward rate, rewards/min
+        reward_rate_on_this_lap = correct / time_elapsed * 60
+
+        reward_rate[trial_number] = reward_rate_on_this_lap
+    return reward_rate
+
+
 def add_reward_rate_to_stimulus_presentations(stimulus_presentations,
                                               trials):
     '''
     Parameters:
     ____________
     trials: Pandas.DataFrame
         ophys_experiment.trials
```

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/ccf_tools.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/ccf_tools.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/receptive_field_mapping.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/receptive_field_mapping.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/electrophysiology/utilities.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/electrophysiology/utilities.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/data_access.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/data_access.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/datasets/optical_physiology/data_formatting.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/datasets/optical_physiology/data_formatting.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/behavior_plots.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/behavior_plots.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/ophys_plots.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/ophys_plots.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/plotting/plot_utils.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/plotting/plot_utils.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/general_utilities.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/general_utilities.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities/utilities/trial_utilities.py` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities/utilities/trial_utilities.py`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/PKG-INFO` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-observatory-utilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utilities for analyzing, manipulating and visualizing data for Brain Observatory projects
 Home-page: https://github.com/AllenInstitute/mindscope_utilities
 Author: Allen Institute
 Author-email: corbettb@alleninstitute.org, michaelbu@alleninstitute.org, marinag@alleninstitute.org, clark.roll@alleninstitute.org
 License: Allen Institute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `brain_observatory_utilities-0.2.0/brain_observatory_utilities.egg-info/SOURCES.txt` & `brain_observatory_utilities-0.2.1/brain_observatory_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain_observatory_utilities-0.2.0/setup.py` & `brain_observatory_utilities-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="brain_observatory_utilities",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     description="Utilities for analyzing, manipulating and visualizing data for Brain Observatory projects",
     dowload_url='https://github.com/AllenInstitute/brain_observatory_utilities/archive/refs/tags/v0.2.0.tar.gz',
     url="https://github.com/AllenInstitute/mindscope_utilities",
     author="Allen Institute",
     author_email="corbettb@alleninstitute.org, michaelbu@alleninstitute.org, marinag@alleninstitute.org, clark.roll@alleninstitute.org",
```

