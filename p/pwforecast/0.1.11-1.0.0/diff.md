# Comparing `tmp/pwforecast-0.1.11.tar.gz` & `tmp/pwforecast-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-0.1.11.tar", last modified: Sat Jul  8 10:46:51 2023, max compression
+gzip compressed data, was "pwforecast-1.0.0.tar", last modified: Sat Jul  8 21:34:40 2023, max compression
```

## Comparing `pwforecast-0.1.11.tar` & `pwforecast-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:46:51.641744 pwforecast-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 10:46:40.000000 pwforecast-0.1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 10:46:51.641744 pwforecast-0.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-08 10:46:40.000000 pwforecast-0.1.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:46:51.641744 pwforecast-0.1.11/pwforecast/
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-08 10:46:40.000000 pwforecast-0.1.11/pwforecast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:46:51.641744 pwforecast-0.1.11/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 10:46:51.000000 pwforecast-0.1.11/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 10:46:51.000000 pwforecast-0.1.11/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:46:51.000000 pwforecast-0.1.11/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 10:46:51.000000 pwforecast-0.1.11/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 10:46:51.000000 pwforecast-0.1.11/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:46:51.645744 pwforecast-0.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-08 10:46:40.000000 pwforecast-0.1.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 21:34:29.000000 pwforecast-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-08 21:34:40.954244 pwforecast-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-08 21:34:29.000000 pwforecast-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/pwforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-07-08 21:34:29.000000 pwforecast-1.0.0/pwforecast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:34:40.954244 pwforecast-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 21:34:29.000000 pwforecast-1.0.0/setup.py
```

### Comparing `pwforecast-0.1.11/LICENSE` & `pwforecast-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-0.1.11/PKG-INFO` & `pwforecast-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 0.1.11
+Version: 1.0.0
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
 Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
-more flexible control for those with more complex tariffs, please let me know. 
+more flexible control for those with more complex tariffs, please let me know.
 
 [![Version](https://img.shields.io/pypi/v/pwforecast)](https://pypi.org/project/pwforecast)
 
 
 ## Getting Started
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
-[free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 calls per day. 
+[free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
-[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two factor
-enabled.
+[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
+authentication enabled.
 
 Rather than wrap [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed to 
 it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
+When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
+faster than 1.7kW per Powerwall, but results may be unpredictable. 
+
 
 ## Overview 
 
 PwForecast has two main methods, `set_peak_mode` and `set_off_peak_mode`. Both can be configured using a PwForecast
 instance. 
 
 Here is an example showing how to configure teslapy and PwForecast:
@@ -55,34 +58,53 @@
 ```
 
 
 
 ## Setting Peak Mode
 
 Use this method when your peak rate starts. You can configure what backup reserve the Powerwall can discharge down
-to by setting the `min_reserve_peak_rate` value. 
+to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
 pw_forecast.set_peak_mode()
 ```
 
 
 ## Setting Off-Peak Mode
 
 Use this method when your off-peak rate starts. This requires a little more configuration.
  * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
  * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
  * Configure the amount of energy you require during the peak-rate. 
 
+TODO: ADD BIT ABOUT TAKING 20 SECONDS, SHOW OUTPUT
+
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
 
 
+## Retry Logic
+
+When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
+figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
+issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
+Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command. 
+Please do let me know if you have any ideas. 
+
+Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site power 
+flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry up to the 
+`reserve_retry` limit. If the `retry_limit` is reached, an exception will be raised. PwForecast will then attempt to 
+apply the setting up to the `global_retry` limit, eventually raising an exception. 
+
+Both `reserve_retry` and `global_retry` can be configured on the PwForecast instance. The `reserve_retry` has been 
+split from the `global_retry` to try and avoid exhausting Solcast API calls. 
+
+
 ## Advanced Configuration
 
 PwForecast has a few advanced configuration options. Please check the class docstring for more info.
```

### Comparing `pwforecast-0.1.11/pwforecast/__init__.py` & `pwforecast-1.0.0/pwforecast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import tzlocal
 import datetime
 import requests
 import pprint
 from dateutil import parser
 
 
-
 # TODO: Calculate required energy by looking at average historic usage during peak-rate between certain time period.
 
 
 class PwForecast(object):
     """
     A tool that dynamically sets Powerwall backup reserve percent based on solar forecast.
```

### Comparing `pwforecast-0.1.11/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.0.0/pwforecast.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 0.1.11
+Version: 1.0.0
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
 Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
-more flexible control for those with more complex tariffs, please let me know. 
+more flexible control for those with more complex tariffs, please let me know.
 
 [![Version](https://img.shields.io/pypi/v/pwforecast)](https://pypi.org/project/pwforecast)
 
 
 ## Getting Started
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
-[free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 calls per day. 
+[free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
-[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two factor
-enabled.
+[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
+authentication enabled.
 
 Rather than wrap [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed to 
 it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
+When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
+faster than 1.7kW per Powerwall, but results may be unpredictable. 
+
 
 ## Overview 
 
 PwForecast has two main methods, `set_peak_mode` and `set_off_peak_mode`. Both can be configured using a PwForecast
 instance. 
 
 Here is an example showing how to configure teslapy and PwForecast:
@@ -55,34 +58,53 @@
 ```
 
 
 
 ## Setting Peak Mode
 
 Use this method when your peak rate starts. You can configure what backup reserve the Powerwall can discharge down
-to by setting the `min_reserve_peak_rate` value. 
+to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
 pw_forecast.set_peak_mode()
 ```
 
 
 ## Setting Off-Peak Mode
 
 Use this method when your off-peak rate starts. This requires a little more configuration.
  * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
  * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
  * Configure the amount of energy you require during the peak-rate. 
 
+TODO: ADD BIT ABOUT TAKING 20 SECONDS, SHOW OUTPUT
+
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
 
 
+## Retry Logic
+
+When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
+figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
+issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
+Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command. 
+Please do let me know if you have any ideas. 
+
+Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site power 
+flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry up to the 
+`reserve_retry` limit. If the `retry_limit` is reached, an exception will be raised. PwForecast will then attempt to 
+apply the setting up to the `global_retry` limit, eventually raising an exception. 
+
+Both `reserve_retry` and `global_retry` can be configured on the PwForecast instance. The `reserve_retry` has been 
+split from the `global_retry` to try and avoid exhausting Solcast API calls. 
+
+
 ## Advanced Configuration
 
 PwForecast has a few advanced configuration options. Please check the class docstring for more info.
```

### Comparing `pwforecast-0.1.11/setup.py` & `pwforecast-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 
 # read the contents of README file
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='0.1.11',
+    version='1.0.0',
     author='Tim Hawker',
     description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     url='https://github.com/timhawker/pwforecast',
     long_description_content_type='text/markdown',
     long_description=readme,
     packages=['pwforecast'],
     install_requires=['tzlocal', 'requests', 'python-dateutil', 'TeslaPy']
```

