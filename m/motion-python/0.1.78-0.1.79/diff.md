# Comparing `tmp/motion_python-0.1.78.tar.gz` & `tmp/motion_python-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.78.tar", max compression
+gzip compressed data, was "motion_python-0.1.79.tar", max compression
```

## Comparing `motion_python-0.1.78.tar` & `motion_python-0.1.79.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-07 22:31:48.218689 motion_python-0.1.78/README.md
--rw-r--r--   0        0        0      344 2023-07-07 22:31:48.218689 motion_python-0.1.78/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-07 22:31:48.218689 motion_python-0.1.78/motion/cli.py
--rw-r--r--   0        0        0    23355 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/dicts.py
--rw-r--r--   0        0        0    17213 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/execute.py
--rw-r--r--   0        0        0    13900 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/route.py
--rw-r--r--   0        0        0     5018 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/server/update_task.py
--rw-r--r--   0        0        0     8661 2023-07-07 22:31:48.222689 motion_python-0.1.78/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-07 22:32:12.142738 motion_python-0.1.78/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.78/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-08 00:46:41.015336 motion_python-0.1.79/README.md
+-rw-r--r--   0        0        0      344 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/cli.py
+-rw-r--r--   0        0        0    23355 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/dicts.py
+-rw-r--r--   0        0        0    17213 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/execute.py
+-rw-r--r--   0        0        0    13900 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/instance.py
+-rw-r--r--   0        0        0     4882 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/route.py
+-rw-r--r--   0        0        0     4953 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/server/update_task.py
+-rw-r--r--   0        0        0     8661 2023-07-08 00:46:41.015336 motion_python-0.1.79/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-08 00:47:00.723385 motion_python-0.1.79/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.79/PKG-INFO
```

### Comparing `motion_python-0.1.78/README.md` & `motion_python-0.1.79/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/cli.py` & `motion_python-0.1.79/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/component.py` & `motion_python-0.1.79/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/dicts.py` & `motion_python-0.1.79/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/execute.py` & `motion_python-0.1.79/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/instance.py` & `motion_python-0.1.79/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/migrate.py` & `motion_python-0.1.79/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.79/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/route.py` & `motion_python-0.1.79/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/motion/server/update_task.py` & `motion_python-0.1.79/motion/server/update_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,18 +122,17 @@
                         old_state.update(state_update)
                         saveState(
                             old_state,
                             redis_con,
                             self.instance_name,
                             self.save_state_func,
                         )
-                except Exception as e:
-                    # logger.error(f"Error in {self.queue_identifier} fit: {e}")
+                except Exception:
                     logger.error(traceback.format_exc())
-                    exception_str = str(e)
+                    exception_str = str(traceback.format_exc())
                 finally:
                     logger.info("Releasing lock.")
                     lock.release()
             else:
                 logger.error("Lock not acquired; item lost.")
 
             redis_con.publish(
```

### Comparing `motion_python-0.1.78/motion/utils.py` & `motion_python-0.1.79/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.78/pyproject.toml` & `motion_python-0.1.79/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.78"
+version = "0.1.79"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.78/PKG-INFO` & `motion_python-0.1.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.78
+Version: 0.1.79
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

