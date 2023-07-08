# Comparing `tmp/dequeai-0.800.tar.gz` & `tmp/dequeai-0.802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.800.tar", last modified: Fri Jun 23 20:57:38 2023, max compression
+gzip compressed data, was "dequeai-0.802.tar", last modified: Sat Jul  8 00:17:28 2023, max compression
```

## Comparing `dequeai-0.800.tar` & `dequeai-0.802.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:57:38.472236 dequeai-0.800/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-23 20:57:38.472236 dequeai-0.800/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:57:38.472236 dequeai-0.800/dequeai/
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.800/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.800/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.800/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.800/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.800/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    32570 2023-06-23 20:57:08.000000 dequeai-0.800/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.800/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.800/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.800/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.800/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:57:38.472236 dequeai-0.800/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-23 20:57:38.000000 dequeai-0.800/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-23 20:57:38.000000 dequeai-0.800/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:57:38.000000 dequeai-0.800/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-23 20:57:38.000000 dequeai-0.800/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-23 20:57:38.000000 dequeai-0.800/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:57:38.472236 dequeai-0.800/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-23 20:57:24.000000 dequeai-0.800/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.146827 dequeai-0.802/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 00:17:28.142827 dequeai-0.802/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.142827 dequeai-0.802/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-05 17:59:58.000000 dequeai-0.802/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.802/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.802/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.802/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-07-05 18:59:08.000000 dequeai-0.802/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    12748 2023-07-08 00:09:40.000000 dequeai-0.802/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32571 2023-06-23 20:59:39.000000 dequeai-0.802/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.802/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.802/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.802/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.802/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.142827 dequeai-0.802/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-08 00:17:28.000000 dequeai-0.802/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-08 00:17:28.000000 dequeai-0.802/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 00:17:28.146827 dequeai-0.802/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-08 00:17:14.000000 dequeai-0.802/setup.py
```

### Comparing `dequeai-0.800/dequeai/datatypes.py` & `dequeai-0.802/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.800/dequeai/dequeai.py` & `dequeai-0.802/dequeai/dequeai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from dequeai.dequeai_run import Run
+from dequeai.dequeai_model import Model
 
 run = Run()
-
+model = Model()
 
 def init( user_name, api_key, project_name):
     run.init(user_name=user_name, api_key=api_key, project_name=project_name)
+    #model.init(user_name=user_name, api_key=api_key, project_name=project_name)
+
 
 def finish():
     run.finish()
 
 def log( data, step=None, commit=True):
     run.log(data=data, step=step, commit=commit)
 
 def log_hyperparams( hyperparams):
     run.log_hyperparams(hyperparams=hyperparams)
 
-def log_gradients( model, logging_frequency=1, layers_to_log="all"):
+def log_gradients( model, logging_frequency=10, layers_to_log="all"):
     run.log_gradients(model=model, logging_frequency=logging_frequency,layers_to_log=layers_to_log)
 
 def log_artifact(artifact_type, path):
     run.log_artifact(artifact_type=artifact_type, path=path)
 
 def load_artifact(artifact_type, run_id):
     run.load_artifact(artifact_type=artifact_type, run_id=run_id)
@@ -31,7 +34,8 @@
     run.compare_runs(project_name=project_name, metric_key=metric_key)
 
 def read_best_run(project_name, metric_key):
     run.read_best_run(project_name=project_name, metric_key=metric_key)
 
 
 
+
```

### Comparing `dequeai-0.800/dequeai/dequeai_run.py` & `dequeai-0.802/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,15 @@
         #print(f"Sending gradients to server {AGENT_API_SERVICE_URL}/fex/project/run/log/gradients/")
         pickled_data = pickle.dumps(full_data)
         self._rest.post_binary(url=AGENT_API_SERVICE_URL+ "/fex/project/run/log/gradients/", data=pickled_data)
         #resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/log/gradients/", json=full_data)
         #print(resp.json())
 
 
-    def log_gradients(self, model, logging_frequency=1, layers_to_log="all"):
+    def log_gradients(self, model, logging_frequency=10, layers_to_log="all"):
         if self.user_name is None:
             raise Exception("Please call dequeai.init(user_name, api_key, project_name) before logging")
 
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for logging gradients.")
```

### Comparing `dequeai-0.800/dequeai/parsing_service.py` & `dequeai-0.802/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.800/dequeai/rest_connect.py` & `dequeai-0.802/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.800/dequeai/util.py` & `dequeai-0.802/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.800/setup.py` & `dequeai-0.802/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000800',
+    version='0.00000802',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

