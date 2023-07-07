# Comparing `tmp/motion_python-0.1.77.tar.gz` & `tmp/motion_python-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.77.tar", max compression
+gzip compressed data, was "motion_python-0.1.78.tar", max compression
```

## Comparing `motion_python-0.1.77.tar` & `motion_python-0.1.78.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-07 21:31:24.442276 motion_python-0.1.77/README.md
--rw-r--r--   0        0        0      344 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/cli.py
--rw-r--r--   0        0        0    23355 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/dicts.py
--rw-r--r--   0        0        0    17016 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/execute.py
--rw-r--r--   0        0        0    13900 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/route.py
--rw-r--r--   0        0        0     5018 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/server/update_task.py
--rw-r--r--   0        0        0     8661 2023-07-07 21:31:24.446276 motion_python-0.1.77/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-07 21:31:45.274232 motion_python-0.1.77/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.77/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-07 22:31:48.218689 motion_python-0.1.78/README.md
+-rw-r--r--   0        0        0      344 2023-07-07 22:31:48.218689 motion_python-0.1.78/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-07 22:31:48.218689 motion_python-0.1.78/motion/cli.py
+-rw-r--r--   0        0        0    23355 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/dicts.py
+-rw-r--r--   0        0        0    17213 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/execute.py
+-rw-r--r--   0        0        0    13900 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/instance.py
+-rw-r--r--   0        0        0     4882 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/route.py
+-rw-r--r--   0        0        0     5018 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/server/update_task.py
+-rw-r--r--   0        0        0     8661 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-07 22:32:12.142738 motion_python-0.1.78/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.78/PKG-INFO
```

### Comparing `motion_python-0.1.77/README.md` & `motion_python-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/cli.py` & `motion_python-0.1.78/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/component.py` & `motion_python-0.1.78/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/dicts.py` & `motion_python-0.1.78/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/execute.py` & `motion_python-0.1.78/motion/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,37 +132,42 @@
                 queue_id = self._get_queue_identifier(rkey, udf_name)
                 self.queue_ids_for_fit.append(queue_id)
                 self.route_dict_for_fit[queue_id] = route
                 self.channel_dict_for_fit[queue_id] = self._get_channel_identifier(
                     rkey, udf_name
                 )
 
-        self.worker_task = UpdateTask(
-            self._instance_name,
-            routes=self.route_dict_for_fit,
-            save_state_func=self._save_state_func,
-            load_state_func=self._load_state_func,
-            queue_identifiers=self.queue_ids_for_fit,
-            channel_identifiers=self.channel_dict_for_fit,
-            redis_host=rp.host,
-            redis_port=rp.port,
-            redis_db=rp.db,
-            redis_password=rp.password,  # type: ignore
-            running=self.running,
-        )
-        self.worker_task.start()
+        self.worker_task = None
+        if self.queue_ids_for_fit:
+            self.worker_task = UpdateTask(
+                self._instance_name,
+                routes=self.route_dict_for_fit,
+                save_state_func=self._save_state_func,
+                load_state_func=self._load_state_func,
+                queue_identifiers=self.queue_ids_for_fit,
+                channel_identifiers=self.channel_dict_for_fit,
+                redis_host=rp.host,
+                redis_port=rp.port,
+                redis_db=rp.db,
+                redis_password=rp.password,  # type: ignore
+                running=self.running,
+            )
+            self.worker_task.start()
 
         # Set up a monitor thread
         self.stop_event = threading.Event()
         self.monitor_thread = threading.Thread(
             target=self._monitor_process, daemon=True
         )
         self.monitor_thread.start()
 
     def _monitor_process(self) -> None:
+        if not self.worker_task:
+            return
+
         rp = RedisParams()
         while not self.stop_event.is_set():
             # See if the update task is alive
             if not self.worker_task.is_alive():
                 logger.debug(
                     f"Failed to detect heartbeat for {self.worker_task.name}."
                     + " Restarting the task in the background."
@@ -208,15 +213,15 @@
         if is_open:
             logger.info("Running update operations on remaining data...")
 
         # Set shutdown event
         self.stop_event.set()
         self.running.value = False
 
-        if psutil.pid_exists(self.worker_task.pid):
+        if self.worker_task and psutil.pid_exists(self.worker_task.pid):
             self.worker_task.join()
 
         self._redis_con.close()
 
         self.monitor_thread.join()
 
     def _updateState(self, new_state: Dict[str, Any]) -> None:
```

### Comparing `motion_python-0.1.77/motion/instance.py` & `motion_python-0.1.78/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/migrate.py` & `motion_python-0.1.78/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.78/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/route.py` & `motion_python-0.1.78/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/server/update_task.py` & `motion_python-0.1.78/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/motion/utils.py` & `motion_python-0.1.78/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.77/pyproject.toml` & `motion_python-0.1.78/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.77"
+version = "0.1.78"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.77/PKG-INFO` & `motion_python-0.1.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.77
+Version: 0.1.78
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

