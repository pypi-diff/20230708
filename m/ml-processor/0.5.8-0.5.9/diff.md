# Comparing `tmp/ml_processor-0.5.8.tar.gz` & `tmp/ml_processor-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_processor-0.5.8.tar", last modified: Tue Feb 14 17:07:28 2023, max compression
+gzip compressed data, was "ml_processor-0.5.9.tar", last modified: Tue Feb 14 17:31:38 2023, max compression
```

## Comparing `ml_processor-0.5.8.tar` & `ml_processor-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:07:28.019945 ml_processor-0.5.8/
--rw-r--r--   0 gsp        (501) staff       (20)     1075 2023-02-11 08:06:28.000000 ml_processor-0.5.8/LICENSE.txt
--rw-r--r--   0 gsp        (501) staff       (20)    18907 2023-02-14 17:07:28.019497 ml_processor-0.5.8/PKG-INFO
--rw-r--r--   0 gsp        (501) staff       (20)    18562 2023-02-13 13:39:55.000000 ml_processor-0.5.8/README.rst
--rw-r--r--   0 gsp        (501) staff       (20)       38 2023-02-14 17:07:28.020168 ml_processor-0.5.8/setup.cfg
--rw-r--r--   0 gsp        (501) staff       (20)     1670 2023-02-14 17:06:47.000000 ml_processor-0.5.8/setup.py
-drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:07:28.007614 ml_processor-0.5.8/src/
-drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:07:28.015393 ml_processor-0.5.8/src/ml_processor/
--rw-r--r--   0 gsp        (501) staff       (20)        0 2023-02-11 08:06:28.000000 ml_processor-0.5.8/src/ml_processor/__init__.py
--rw-r--r--   0 gsp        (501) staff       (20)     2393 2023-02-11 12:35:48.000000 ml_processor-0.5.8/src/ml_processor/configuration.py
--rw-r--r--   0 gsp        (501) staff       (20)    13137 2023-02-14 16:15:03.000000 ml_processor-0.5.8/src/ml_processor/data_prep.py
--rw-r--r--   0 gsp        (501) staff       (20)    13308 2023-02-13 20:15:43.000000 ml_processor-0.5.8/src/ml_processor/eda_analysis.py
--rw-r--r--   0 gsp        (501) staff       (20)     5017 2023-02-11 08:06:28.000000 ml_processor-0.5.8/src/ml_processor/etl_processor.py
--rw-r--r--   0 gsp        (501) staff       (20)      359 2023-02-11 08:06:28.000000 ml_processor-0.5.8/src/ml_processor/jsonSerializer.py
--rw-r--r--   0 gsp        (501) staff       (20)    41068 2023-02-14 16:28:19.000000 ml_processor-0.5.8/src/ml_processor/model_training.py
--rw-r--r--   0 gsp        (501) staff       (20)    11656 2023-02-11 08:06:28.000000 ml_processor-0.5.8/src/ml_processor/outliers.py
-drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:07:28.018728 ml_processor-0.5.8/src/ml_processor.egg-info/
--rw-r--r--   0 gsp        (501) staff       (20)    18907 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/PKG-INFO
--rw-r--r--   0 gsp        (501) staff       (20)      528 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/SOURCES.txt
--rw-r--r--   0 gsp        (501) staff       (20)        1 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/dependency_links.txt
--rw-r--r--   0 gsp        (501) staff       (20)        1 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/not-zip-safe
--rw-r--r--   0 gsp        (501) staff       (20)      191 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/requires.txt
--rw-r--r--   0 gsp        (501) staff       (20)       13 2023-02-14 17:07:27.000000 ml_processor-0.5.8/src/ml_processor.egg-info/top_level.txt
+drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:31:38.246608 ml_processor-0.5.9/
+-rw-r--r--   0 gsp        (501) staff       (20)     1075 2023-02-11 08:06:28.000000 ml_processor-0.5.9/LICENSE.txt
+-rw-r--r--   0 gsp        (501) staff       (20)    18907 2023-02-14 17:31:38.246181 ml_processor-0.5.9/PKG-INFO
+-rw-r--r--   0 gsp        (501) staff       (20)    18562 2023-02-13 13:39:55.000000 ml_processor-0.5.9/README.rst
+-rw-r--r--   0 gsp        (501) staff       (20)       38 2023-02-14 17:31:38.246777 ml_processor-0.5.9/setup.cfg
+-rw-r--r--   0 gsp        (501) staff       (20)     1670 2023-02-14 17:30:34.000000 ml_processor-0.5.9/setup.py
+drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:31:38.233723 ml_processor-0.5.9/src/
+drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:31:38.242466 ml_processor-0.5.9/src/ml_processor/
+-rw-r--r--   0 gsp        (501) staff       (20)        0 2023-02-11 08:06:28.000000 ml_processor-0.5.9/src/ml_processor/__init__.py
+-rw-r--r--   0 gsp        (501) staff       (20)     2393 2023-02-11 12:35:48.000000 ml_processor-0.5.9/src/ml_processor/configuration.py
+-rw-r--r--   0 gsp        (501) staff       (20)    13137 2023-02-14 16:15:03.000000 ml_processor-0.5.9/src/ml_processor/data_prep.py
+-rw-r--r--   0 gsp        (501) staff       (20)    13308 2023-02-13 20:15:43.000000 ml_processor-0.5.9/src/ml_processor/eda_analysis.py
+-rw-r--r--   0 gsp        (501) staff       (20)     5017 2023-02-11 08:06:28.000000 ml_processor-0.5.9/src/ml_processor/etl_processor.py
+-rw-r--r--   0 gsp        (501) staff       (20)      359 2023-02-11 08:06:28.000000 ml_processor-0.5.9/src/ml_processor/jsonSerializer.py
+-rw-r--r--   0 gsp        (501) staff       (20)    40506 2023-02-14 17:29:33.000000 ml_processor-0.5.9/src/ml_processor/model_training.py
+-rw-r--r--   0 gsp        (501) staff       (20)    11656 2023-02-11 08:06:28.000000 ml_processor-0.5.9/src/ml_processor/outliers.py
+drwxr-xr-x   0 gsp        (501) staff       (20)        0 2023-02-14 17:31:38.245563 ml_processor-0.5.9/src/ml_processor.egg-info/
+-rw-r--r--   0 gsp        (501) staff       (20)    18907 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/PKG-INFO
+-rw-r--r--   0 gsp        (501) staff       (20)      528 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/SOURCES.txt
+-rw-r--r--   0 gsp        (501) staff       (20)        1 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/dependency_links.txt
+-rw-r--r--   0 gsp        (501) staff       (20)        1 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/not-zip-safe
+-rw-r--r--   0 gsp        (501) staff       (20)      191 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/requires.txt
+-rw-r--r--   0 gsp        (501) staff       (20)       13 2023-02-14 17:31:37.000000 ml_processor-0.5.9/src/ml_processor.egg-info/top_level.txt
```

### Comparing `ml_processor-0.5.8/LICENSE.txt` & `ml_processor-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/PKG-INFO` & `ml_processor-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_processor
-Version: 0.5.8
+Version: 0.5.9
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/package_dev/tree/master/ml
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `ml_processor-0.5.8/README.rst` & `ml_processor-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/setup.py` & `ml_processor-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(path, "r") as fh:
     long_description = fh.read()
 
 setup(
     # name that will be imported, can be different from code file name
     name='ml_processor',
 
-    version='0.5.8',
+    version='0.5.9',
 
     description='Includes functions for performing econometrics tasks',
 
     # code file name without file extension
     # py_modules=['configuration', 'eda_analysis', 'encoders', 'jsonSerializer', 'model_training' 'outliers' 'snowflake_processor'],
 
     packages=['ml_processor'],
```

### Comparing `ml_processor-0.5.8/src/ml_processor/configuration.py` & `ml_processor-0.5.9/src/ml_processor/configuration.py`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/src/ml_processor/data_prep.py` & `ml_processor-0.5.9/src/ml_processor/data_prep.py`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/src/ml_processor/eda_analysis.py` & `ml_processor-0.5.9/src/ml_processor/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/src/ml_processor/etl_processor.py` & `ml_processor-0.5.9/src/ml_processor/etl_processor.py`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/src/ml_processor/model_training.py` & `ml_processor-0.5.9/src/ml_processor/model_training.py`

 * *Files 4% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         Returns
         -------
         
         None
         
         """
 
-        self._split_tunning_data()
+        self._reduce_data()
         
 
         self.hyperparams = hyper_parameter_tunning(
             features = self.X_train_param[self.features], 
             labels = self.y_train_param, 
             method = self.method,
             classifier = self.classifier,
@@ -535,53 +535,34 @@
         Returns
         -------
         
         pandas.DataFrame:
             Dataset for hyperparameter tuning
         
         """
-        
-        tunning_data_size = int(self.data.shape[0] * self.params_prop)
-        
-        self.log.info('Hyper parameter tuning data set created')
-    
-        self.log.info(f'Hyper parameter tuning data set:{tunning_data_size} rows')
-        
-        return self.data.sample(tunning_data_size)
 
 
-    def _split_tunning_data(self):
-        
-        """
+        if self.X_train.empty:
+            self._split_data()
 
-        Split data into training and test sets
 
-        Parameters
-        ----------
-        
-        None
-        
-        Returns
-        -------
-        
-        None
-        
-        """
-        
-        tunning_data = self._reduce_data()
+        train_set = pd.concat([self.X_train, self.y_train], axis=1)
 
-        self.X_train_param, self.X_test_param, self.y_train_param, self.y_test_param = split_data(data=tunning_data, target=self.target, test_size=self.test_size)
-        
-        self.log.info('Splitting hyperparameter tuning data into training and testing sets completed')
-        
-        self.log.info(f'Hyperparameter tuning training data set:{self.X_train_param.shape[0]} rows')
-        
-        self.log.info(f'Hyperparameter tuning testing data set:{self.X_test_param.shape[0]} rows')
+        tunning_data_size = int(self.X_train.shape[0] * self.params_prop)
+
+        hyp_tune_data = self.data.sample(tunning_data_size)
 
+        self.log.info('Hyper parameter tuning data set created')
 
+        self.log.info(f'Hyper parameter tuning data set:{tunning_data_size} rows')
+
+        self.X_train_param = hyp_tune_data[self.features]
+
+        self.y_train_param =  hyp_tune_data[self.target]
+        
 
 # <<<<<<<<<<<<<<<<<<<<<<<<>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 class plot_model_perf:
 
     """
 
     Generate model diagnostics plots
```

### Comparing `ml_processor-0.5.8/src/ml_processor/outliers.py` & `ml_processor-0.5.9/src/ml_processor/outliers.py`

 * *Files identical despite different names*

### Comparing `ml_processor-0.5.8/src/ml_processor.egg-info/PKG-INFO` & `ml_processor-0.5.9/src/ml_processor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-processor
-Version: 0.5.8
+Version: 0.5.9
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/package_dev/tree/master/ml
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
```

### Comparing `ml_processor-0.5.8/src/ml_processor.egg-info/SOURCES.txt` & `ml_processor-0.5.9/src/ml_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

