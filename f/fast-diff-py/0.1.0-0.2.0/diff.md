# Comparing `tmp/fast_diff_py-0.1.0.tar.gz` & `tmp/fast_diff_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_diff_py-0.1.0.tar", last modified: Thu Jul  6 22:20:40 2023, max compression
+gzip compressed data, was "fast_diff_py-0.2.0.tar", last modified: Sat Jul  8 16:58:08 2023, max compression
```

## Comparing `fast_diff_py-0.1.0.tar` & `fast_diff_py-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 22:20:40.321152 fast_diff_py-0.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2023-02-17 16:03:58.000000 fast_diff_py-0.1.0/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      838 2023-07-06 22:20:40.334186 fast_diff_py-0.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7894 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 22:20:40.280417 fast_diff_py-0.1.0/fast_diff_py/
--rwxrwxrwx   0 root         (0) root         (0)      203 2023-07-06 21:49:36.000000 fast_diff_py-0.1.0/fast_diff_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16775 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/child_processes.py
--rwxrwxrwx   0 root         (0) root         (0)    13144 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/config.py
--rwxrwxrwx   0 root         (0) root         (0)    23157 2023-04-18 11:56:24.000000 fast_diff_py-0.1.0/fast_diff_py/cpu_image_processor.py
--rwxrwxrwx   0 root         (0) root         (0)    16005 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/database.py
--rwxrwxrwx   0 root         (0) root         (0)    12143 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/datatransfer.py
--rwxrwxrwx   0 root         (0) root         (0)     6682 2023-07-06 21:51:41.000000 fast_diff_py-0.1.0/fast_diff_py/dif.py
--rwxrwxrwx   0 root         (0) root         (0)    62751 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/fastDif.py
--rwxrwxrwx   0 root         (0) root         (0)    31049 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/fast_diff_base.py
--rwxrwxrwx   0 root         (0) root         (0)     2585 2023-03-07 18:36:06.000000 fast_diff_py-0.1.0/fast_diff_py/gpu_image_processor.py
--rwxrwxrwx   0 root         (0) root         (0)    39101 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/mariadb_database.py
--rwxrwxrwx   0 root         (0) root         (0)    38244 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/sql_database.py
--rwxrwxrwx   0 root         (0) root         (0)     4727 2023-07-06 21:38:13.000000 fast_diff_py-0.1.0/fast_diff_py/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 22:20:40.320740 fast_diff_py-0.1.0/fast_diff_py.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      838 2023-07-06 22:20:40.000000 fast_diff_py-0.1.0/fast_diff_py.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      584 2023-07-06 22:20:40.000000 fast_diff_py-0.1.0/fast_diff_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-06 22:20:40.000000 fast_diff_py-0.1.0/fast_diff_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-07-06 22:20:40.000000 fast_diff_py-0.1.0/fast_diff_py.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-06 22:20:40.000000 fast_diff_py-0.1.0/fast_diff_py.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-06 22:20:40.334741 fast_diff_py-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1599 2023-07-06 22:20:13.000000 fast_diff_py-0.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 16:58:08.928633 fast_diff_py-0.2.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1070 2023-02-17 16:03:58.000000 fast_diff_py-0.2.0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-08 16:58:08.928879 fast_diff_py-0.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7894 2023-07-06 21:38:13.000000 fast_diff_py-0.2.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1059 2023-07-08 16:33:59.000000 fast_diff_py-0.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      977 2023-07-08 16:58:08.929609 fast_diff_py-0.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      579 2023-07-08 16:52:40.000000 fast_diff_py-0.2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 16:58:08.902020 fast_diff_py-0.2.0/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 16:58:08.922357 fast_diff_py-0.2.0/src/fast_diff_py/
+-rwxrwxrwx   0 root         (0) root         (0)      114 2023-07-08 11:57:20.000000 fast_diff_py-0.2.0/src/fast_diff_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17697 2023-07-08 13:11:54.000000 fast_diff_py-0.2.0/src/fast_diff_py/child_processes.py
+-rwxrwxrwx   0 root         (0) root         (0)    13893 2023-07-07 14:48:21.000000 fast_diff_py-0.2.0/src/fast_diff_py/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    23138 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/cpu_image_processor.py
+-rwxrwxrwx   0 root         (0) root         (0)    16005 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/database.py
+-rwxrwxrwx   0 root         (0) root         (0)    12143 2023-07-06 21:38:13.000000 fast_diff_py-0.2.0/src/fast_diff_py/datatransfer.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2023-07-08 13:43:56.000000 fast_diff_py-0.2.0/src/fast_diff_py/dif.py
+-rwxrwxrwx   0 root         (0) root         (0)    67447 2023-07-08 13:42:47.000000 fast_diff_py-0.2.0/src/fast_diff_py/fastDif.py
+-rwxrwxrwx   0 root         (0) root         (0)    31323 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/fast_diff_base.py
+-rwxrwxrwx   0 root         (0) root         (0)     2585 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/gpu_image_processor.py
+-rwxrwxrwx   0 root         (0) root         (0)    39101 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/mariadb_database.py
+-rwxrwxrwx   0 root         (0) root         (0)    38244 2023-07-08 05:26:18.000000 fast_diff_py-0.2.0/src/fast_diff_py/sql_database.py
+-rwxrwxrwx   0 root         (0) root         (0)     4727 2023-07-06 21:38:13.000000 fast_diff_py-0.2.0/src/fast_diff_py/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 16:58:08.928259 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-08 16:58:08.000000 fast_diff_py-0.2.0/src/fast_diff_py.egg-info/top_level.txt
```

### Comparing `fast_diff_py-0.1.0/LICENSE.txt` & `fast_diff_py-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/README.md` & `fast_diff_py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/child_processes.py` & `fast_diff_py-0.2.0/src/fast_diff_py/child_processes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,47 @@
 from fast_diff_py.cpu_image_processor import CPUImageProcessing
-from fast_diff_py.mariadb_database import MariaDBDatabase
 from fast_diff_py.fast_diff_base import FastDiffPyBase
 from fast_diff_py.datatransfer import PreprocessArguments, PreprocessResults, CompareImageArguments, CompareImageResults
 from fast_diff_py.datatransfer import Messages
 import multiprocessing as mp
 from multiprocessing.connection import Connection
 import warnings
 import queue
 import os
 from typing import Tuple, Union, List
 from types import FunctionType
+import signal
+
+
+class GracefulWorker:
+    interrupts: int = 0
+    interrupt_threshold: int = 2
+    identifier: int
+
+    def __init__(self, identifier: int):
+        """
+        Attach handlers for interrupts
+        :param identifier: identifier of this class
+        """
+        self.identifier = identifier
+        signal.signal(signal.SIGINT, self.handle_interrupt)
+        signal.signal(signal.SIGTERM, self.handle_interrupt)
+
+    def handle_interrupt(self):
+        """
+        Handle the interrupt if more than `interrupt_threshold` interrupts are received, exit immediately, otherwise
+        wait for the stop to come through the parent process.
+        :return:
+        """
+        print(f"{self.identifier} - Interrupt")
+        if self.interrupts >= self.interrupt_threshold:
+            print(f"{self.identifier:03} - Exiting immediately")
+            exit(1)
+
+        self.interrupts += 1
 
 def process_image(proc: CPUImageProcessing, args: PreprocessArguments) -> PreprocessResults:
     """
     Function to execute preprocessing with the ImageProcessing Class
     # TODO WARNING in docs that an error in the course of processing if it was not fatal, will be treated as fatal.
 
     :param proc: the ImageProcessing class to retain information (not really necessary currently)
@@ -77,15 +105,15 @@
         try:
             import cupy as cp
             cupy_avail = True
         except ImportError:
             warnings.warn(f"{identifier:03}: Cupy not available. Using CPU instead.")
 
     if cupy_avail:
-        from fast_diff_py.gpu_image_processor import GPUImageProcessing
+        from src.fast_diff_py.gpu_image_processor import GPUImageProcessing
         img_proc = GPUImageProcessing(identifier=identifier)
     else:
         img_proc = CPUImageProcessing(identifier=identifier)
 
     # stay awake for 60s, otherwise kill
     while timeout < 60:
         try:
@@ -136,15 +164,15 @@
         try:
             import cupy as cp
             cupy_avail = True
         except ImportError:
             warnings.warn(f"{identifier:03}: Cupy not available. Using CPU instead.")
 
     if cupy_avail:
-        from fast_diff_py.gpu_image_processor import GPUImageProcessing
+        from src.fast_diff_py.gpu_image_processor import GPUImageProcessing
         processor = GPUImageProcessing(identifier=identifier)
     else:
         processor = CPUImageProcessing(identifier=identifier)
 
     # stay awake for 60s, otherwise kill
     while timeout < 60:
         try:
@@ -239,14 +267,15 @@
 
     :param config: config for the FastDiffPyBase class
     :param db_config: config required for database.
     :return:
     """
     fdb = FastDiffPyBase(cfg=config)
     if db_config["type"] == "mariadb":
+        from src.fast_diff_py.mariadb_database import MariaDBDatabase
         mdb = MariaDBDatabase(user=db_config["user"],
                               password=db_config["password"],
                               host=db_config["host"],
                               port=db_config["port"],
                               database=db_config["database"],
                               table_suffix=db_config["table_suffix"],
                               **db_config["kwargs"],
```

### Comparing `fast_diff_py-0.1.0/fast_diff_py/config.py` & `fast_diff_py-0.2.0/src/fast_diff_py/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,42 @@
     """
     Tests the default config path if it exists.
     :return: True if there's a config.
     """
     return os.path.exists(os.path.join(os.path.dirname(__file__), "task.json"))
 
 
+def remove_existing_config():
+    """
+    Removes a preexisting config. Needed because config path is relative to file.
+    :return:
+    """
+    if test_existing_config():
+        os.remove(os.path.join(os.path.dirname(__file__), "task.json"))
+
 class FastDiffPyConfig:
     cfg_path: str
     update_timeout: int = 30
     retain_config: bool = False
 
     __task_dict: dict
     __last_update: datetime.datetime = datetime.datetime.now()
 
     # ------------------------------------------------------------------------------------------------------------------
     # Class Config Storage
     # ------------------------------------------------------------------------------------------------------------------
 
     def __init__(self, task_path: str = None, task_purge: bool = False, cfg: dict = None):
+        """
+        Create config object
+
+        :param task_path: path to where config is stored.
+        :param task_purge: If a config exists at the specified path, the config will be removed if it exists
+        :param cfg: an initial state of the config - used for config created in child processes.
+        """
         # set the config_path
         if task_path is None:
             self.cfg_path = os.path.join(os.path.dirname(__file__), "task.json")
 
         self._task_dict = {
             "thumbnail_size_x": 64,
             "thumbnail_size_y": 64,
@@ -58,33 +73,33 @@
                 "gpu_proc": 0,
                 "queue_status": None ,
                 "loop_base_a": True ,
                 "use_workers": True,
                 "use_special_b_algo": True
             },
             "database":{
-                "type": "sqlite",
+                "type": None,
                 "path": ""
             },
             "supported_file_types" : [".jpg", ".jpeg", ".png", ".bmp", ".tiff", ".tif", ".gif", ".webp"],
             "less_optimized": False,
             "retry_limit": 1000,
             "verbose": False,
             "state": None,
             "retain_db": True,
+            "cli_args": None
         }
 
-        if os.path.exists(self.cfg_path):
+        if os.path.exists(self.cfg_path) and cfg is None:
             if task_purge:
                 os.remove(self.cfg_path)
             else:
-                if cfg is not None:
-                    self.__task_dict = cfg
-                else:
-                    self.load_config()
+                self.load_config()
+        elif cfg is not None:
+            self.__task_dict = cfg
 
     def load_config(self):
         """
         Load config from file
         :return:
         """
         with open(self.cfg_path, "r") as file:
@@ -413,8 +428,16 @@
 
     @property
     def max_queue_size(self) -> int:
         return self._task_dict["max_queue_size"]
 
     @max_queue_size.setter
     def max_queue_size(self, value: int):
-        self._task_dict["max_queue_size"] = value
+        self._task_dict["max_queue_size"] = value
+
+    @property
+    def cli_args(self):
+        return self._task_dict["cli_args"]
+
+    @cli_args.setter
+    def cli_args(self, value: dict):
+        self._task_dict["cli_args"] = value
```

### Comparing `fast_diff_py-0.1.0/fast_diff_py/cpu_image_processor.py` & `fast_diff_py-0.2.0/src/fast_diff_py/cpu_image_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from types import FunctionType
 from fast_diff_py.datatransfer import *
 import os
 from typing import Tuple, Union
 import cv2
 from matplotlib import pyplot as plt
 import skimage
```

### Comparing `fast_diff_py-0.1.0/fast_diff_py/database.py` & `fast_diff_py-0.2.0/src/fast_diff_py/database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/datatransfer.py` & `fast_diff_py-0.2.0/src/fast_diff_py/datatransfer.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/fastDif.py` & `fast_diff_py-0.2.0/src/fast_diff_py/fastDif.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 from fast_diff_py.utils import *
 import multiprocessing as mp
 import multiprocessing.connection as con
 import threading as th
 from fast_diff_py.datatransfer import *
 from concurrent.futures import ProcessPoolExecutor
 from fast_diff_py.sql_database import SQLiteDatabase
-from fast_diff_py.config import FastDiffPyConfig
+from fast_diff_py.config import FastDiffPyConfig, test_existing_config, remove_existing_config
 from fast_diff_py.fast_diff_base import FastDiffPyBase
 from fast_diff_py.child_processes import parallel_resize, parallel_compare, find_best_image
 from fast_diff_py.child_processes import first_loop_dequeue_worker, first_loop_enqueue_worker
 from fast_diff_py.child_processes import second_loop_dequeue_worker, second_loop_enqueue_worker
-from fast_diff_py.mariadb_database import MariaDBDatabase
 import logging
 import signal
 
 
 """
 Fast implementation of the DifPy Library.
 Features:
@@ -72,143 +71,237 @@
     # logger / CLI Output
     logger: logging.Logger = None
     file_handler: logging.FileHandler = None
     stream_handler: logging.StreamHandler = None
     debug_logger: logging.FileHandler = None
 
     loop_run: bool = False
+    stop_received: bool = False
     en_com_1: Union[None, con.Connection] = None
     de_com_1: Union[None, con.Connection] = None
 
-    def __init__(self, directory_a: str, directory_b: str = None, default_db: bool = True, **kwargs):
+    @classmethod
+    def init_new(cls, directory_a: str, directory_b: str = None, default_db: bool = True, progress: bool = True,
+                 **kwargs):
         """
-        Provide the directories to be searched. If a different implementation of the database is used,
-        set the test_db to false.
+        Creates a fresh instance of the FastDiffPy class.
 
+        A Config will be generated, if the config exists, it will be purged (with warning, that can be disabled)
+        If default_db is True, an instance of the SQLiteDatabase will be created located in the default location.
+
+        If the debug option is passed as a kwarg, more verbose printing in the console is enabled.
+
+        :param progress: Responsible for setting the filter in the logger - if true allows info messages to be
+                            propagated, giving you more information about the state of the process.
         :param directory_a: first directory to search for differentiation.
         :param directory_b: second directory to compare against. Otherwise, comparison will be done against directory
         :param default_db: create a sqlite database in the a_directory.
-        itself.
+        :param kwargs:  - debug: bool - Enable Debug File in the logs. Default False
+                        - disable_config_timeout: bool - if a config exists at the default location, a timeout of 10s is
+                                                         given to the user to halt the process. Turn this off if you are
+                                                         not using the script or use different init method.
+                                                         Default False
+                        - config_path: str - Path to the config that stores the progress of the program
+                                             (for progress recovery on stop) Default None
+                        - retain_config: bool - Default True, You can disable the retention of the config. Default True
 
-        kwarg:
-        ------
-        - debug: bool - Enable Debug File in the logs.
-        - config_path: str - Path to the config that stores the progress of the program (for progress recovery on stop)
-        - config_purge: str - Ignore preexisting config and overwrite it.
-        - config: FastDiffPyConfig - Pass a preexisting config. (process recovery)
-                                      Ignores config_path, config_purge kwarg!!!
+        :return: FastDiffPy
         """
-        super().__init__()
+        # fetch debug information
+        debug = False
+        if "debug" in kwargs.keys():
+            debug = kwargs.get("debug")
 
-        if "config" in kwargs.keys():
-            if type(kwargs.get("config")) is not FastDiffPyConfig:
-                raise ValueError(f"Unsupported type for config: {kwargs.get('config').__name__}, "
-                                 f"only FastDiffPyConfig allowed")
-            self.config = kwargs.get("config")
-
-            if self.config.database["type"] == "sqlite":
-                self.db = SQLiteDatabase(path=self.config.database["path"])
-            elif self.config.database["type"] == "mariadb":
-                self.db = MariaDBDatabase(
-                    user=self.config.database["user"],
-                    password=self.config.database["password"],
-                    host=self.config.database["host"],
-                    port=self.config.database["port"],
-                    database=self.config.database["database"],
-                    table_suffix=self.config.database["table_suffix"]
-                )
+        obj = cls(debug=debug, progress=progress)
 
-            return
+        config_path = None
+        if "config_path" in kwargs.keys():
+            config_path = kwargs.get("config_path")
+
+        disable_config_timeout = False
+        if "disable_config_timeout" in kwargs.keys():
+            disable_config_timeout = kwargs.get("disable_config_timeout")
+
+        # Testing for config existence
+        if not disable_config_timeout:
+            if (config_path is not None and os.path.exists(config_path)) or test_existing_config():
+                obj.logger.warning("Preexisting config will be overwritten!!!")
+                obj.logger.warning("You have 10s to stop the process if this is an error.")
+                time.sleep(10)
+
+        config = FastDiffPyConfig(task_path=config_path, task_purge=True)
+        config.retain_config = kwargs.get("retain_config") if "retain_config" in kwargs.keys() else True
+
+        if not os.path.isdir(directory_a):
+            raise NotADirectoryError(f"{directory_a} is not a directory")
+
+        if directory_b is not None and not os.path.isdir(directory_b):
+            raise NotADirectoryError(f"{directory_b} is not a directory")
+
+        directory_a = os.path.abspath(directory_a)
+        directory_b = os.path.abspath(directory_b) if directory_b is not None else None
+
+        # make sure the paths aren't sub-dirs of each other.
+        if directory_b is not None:
+            temp_a = directory_a + os.sep
+            temp_b = directory_b + os.sep
+            if temp_a.startswith(temp_b):
+                raise ValueError(f"{directory_a} is a subdirectory of {directory_b}")
+            elif temp_b.startswith(temp_a):
+                raise ValueError(f"{directory_b} is a subdirectory of {directory_a}")
+
+        config.p_root_dir_b = directory_b
+        config.p_root_dir_a = directory_a
+        obj.config = config
+
+        # Creating default database if desired.
+        if default_db:
+            obj.db = SQLiteDatabase(path=os.path.join(config.p_root_dir_a, "diff.db"), purge=True)
+
+        config.ignore_paths = []
+        config.ignore_names = []
+
+        obj.init_completed()
+        return obj
+
+    @classmethod
+    def init_preexisting_config(cls, config: FastDiffPyConfig = None, config_path: str = None, progress: bool = True,
+                                retain_config: bool = True, db = None, integrity_check: bool = False):
+        """
+        Create FastDiffPy object from preexisting config. The config can either be at the default path
+        (config_path is None), at a user defined path (config_path is not None) or a config object can be passed in as
+        an argument (config is not None).
+
+        The config argument has higher priority than config_path, i.e. if you provide a config, the config_path argument
+        is ignored since it is assumed, that you set the config path already when instantiating the FastDiffPyConfig
+        object.
+
+        You can pass in a database. This is required, if you have a config that has an empty database type.
+        You can have an empty database type in the case where you don't retain the database in the config since you
+        don't want the password of you mariadb to be in plain text.
+
+        You can set the database to not be retained by setting the `retain_db` attribute of the config to False.
+
+        :param progress: Responsible for setting the filter in the logger - if true allows info messages to be
+                            propagated, giving you more information about the state of the process.
+        :param config: Provide a Config Object that is already instantiated.
+        :param config_path: Load config from user specified path otherwise use default path.
+        :param retain_config: if config should be written to file in regular intervals
+        :param db: database to use for object. Otherwise, try to reconstruct db from config.
+        :param integrity_check: Performs check that all images in database are also present on file system.
+        :return: FastDiffPy
+        """
+
+        obj = cls(debug=False, progress=progress)
+
+        if config is not None:
+            fdc = config
+            obj.logger.info("Adding config provided as argument.")
+        else:
+            fdc = FastDiffPyConfig(task_path=config_path)
+            if config_path is not None:
+                obj.logger.info("Creating config object and using given path.")
+            else:
+                obj.logger.info("Creating config object and using default path.")
 
-        if not self.verify_config():
-            # Only set the directory_a and directory_b when the config is not set.
-            if not os.path.isdir(directory_a):
-                raise NotADirectoryError(f"{directory_a} is not a directory")
-
-            if directory_b is not None and not os.path.isdir(directory_b):
-                raise NotADirectoryError(f"{directory_b} is not a directory")
-
-            directory_a = os.path.abspath(directory_a)
-            directory_b = os.path.abspath(directory_b) if directory_b is not None else None
-
-            # make sure the paths aren't sub-dirs of each other.
-            if directory_b is not None:
-                temp_a = directory_a + os.sep
-                temp_b = directory_b + os.sep
-                if temp_a.startswith(temp_b):
-                    raise ValueError(f"{directory_a} is a subdirectory of {directory_b}")
-                elif temp_b.startswith(temp_a):
-                    raise ValueError(f"{directory_b} is a subdirectory of {directory_a}")
-
-            self.config.p_root_dir_b = directory_b
-            self.config.p_root_dir_a = directory_a
-
-            # Creating default database if desired.
-            if default_db:
-                self.db = SQLiteDatabase(path=os.path.join(self.config.p_root_dir_a, "diff.db"))
+        fdc.retain_config = retain_config
 
-            self.config.ignore_paths = []
-            self.config.ignore_names = []
+        # Need to pass in verbose from top to set the verbose settings in the parent class as well.
+        obj.config = fdc
 
+        # Only set the verbose if it is True. Otherwise, the show_progress setting with console level = info will be
+        # overwritten.
+        if fdc.verbose:
+            obj.verbose = fdc.verbose
+
+        # reconnecting database
+        if fdc.database["type"] == "sqlite":
+            obj.db = SQLiteDatabase(path=fdc.database["path"])
+        elif fdc.database["type"] == "mariadb":
+            from fast_diff_py.mariadb_database import MariaDBDatabase
+            obj.db = MariaDBDatabase(
+                user=fdc.database["user"],
+                password=fdc.database["password"],
+                host=fdc.database["host"],
+                port=fdc.database["port"],
+                database=fdc.database["database"],
+                table_suffix=fdc.database["table_suffix"]
+            )
+        elif fdc.database["type"] is None:
+            if db is not None:
+                obj.db = db
+            else:
+                raise ValueError("Couldn't reconnect database - "
+                                 "No database specified in config and no database provided as argument")
+        if integrity_check:
+            obj.verify_dir_content()
+        return obj
 
-        debug = False
-        if "debug" in kwargs.keys():
-            debug = kwargs.get("debug")
+    def __init__(self, debug: bool = False, progress: bool = True):
+        """
+        Skeleton init function. Main logic of init function is supposed to happen in `init_new` and
+        `init_preexisting_config`
+
+        :param debug: used for loggers and preparation of logging.
+        """
 
-        self.prepare_logging(debug=debug)
+        super().__init__()
+
+        if debug:
+            csl_lvl = logging.DEBUG
+        elif progress:
+            csl_lvl = logging.INFO
+        else:
+            csl_lvl = logging.WARNING
+
+        self.prepare_logging(console_level=csl_lvl, debug=debug)
 
-        # Setting the first stuff in the config
+
+    def init_completed(self):
+        """
+        Updates the config object to indicate that the initialisation of the object has been completed
+        """
         self.config.state = "init"
         self.config.write_to_file()
 
     def interrupt_handler(self):
         """
         Adds handlers for sigint and sigterm
         :return:
         """
+        self.logger.info("Added handling for Interrupts")
         signal.signal(signal.SIGINT, self.sig_int)
         signal.signal(signal.SIGTERM, self.sig_int)
 
-    def sig_int(self):
+    def sig_int(self, *args, **kwargs):
         """
         Handler to trigger the stopping of the loop functions.
         :return:
         """
         self.loop_run = False
 
+        if self.stop_received:
+            exit(100)
+
+        self.stop_received = True
+
         if self.en_com_1 is not None:
             self.en_com_1.send(Messages.Stop)
 
         if self.de_com_1 is not None:
             self.de_com_1.send(Messages.Stop)
 
         self.logger.info("Stop signal received, shutting down...")
 
-    def verify_config(self, full_depth: bool = False):
-        """
-        Load the config and verify that the folders match and the content if the directories too.
-
-        :param full_depth: Check that every file in the database exists.
-
-        :return: returns False if no Config is found. otherwise returns true.
-        """
-        # Empty dict, we have nothing.
-        if not os.path.exists(self.config.cfg_path):
-            return False
-
-        if full_depth:
-            self.verify_dir_content()
-        return True
-
     def verify_dir_content(self):
         """
         Function should go through dir table and make sure every file exists. If a file doesn't exist, raises ValueError.
         :return:
         """
-        pass
+        self.logger.warning("Integrity check not implemented !!!")
 
     def index_the_dirs(self):
         """
         List all the files in directory_a and possibly directory_b and store the paths and filenames in the temporary
         database.
 
         :return:
@@ -674,15 +767,14 @@
         :param cpu_proc: number of cpu processes. Default number of cpus on the system.
         :param diff_location: Where the plots should be stored (needs to be provided if make_diff_plots is true)
         :return:
         """
         # TODO check the number of images with self.db.get_dir_count() -> set the less optimized flag there and then
         #   make the adjustment fro there.
         # Writing to config.
-        self.config.state = "second_loop_in_progress"
         self.config.sl_gpu_proc = gpu_proc
         self.config.sl_cpu_proc = cpu_proc
         self.config.sl_matching_aspect = only_matching_aspect
         self.config.sl_make_diff_plots = make_diff_plots
         self.config.sl_matching_hash = only_matching_hash
         self.config.similarity_threshold = float(similarity_threshold)
         self.config.state = "second_loop_in_progress"
@@ -1136,15 +1228,15 @@
         :return:
         """
         if not self.config.enough_images_to_compare:
             return {}, []
 
         if not dif_based:
             raise NotImplementedError("hash_based is in todos.")
-        clusters = self.build_loose_duplicate_cluster(similarity)
+        clusters = self._build_loose_duplicate_cluster(similarity)
         return self.find_best_image(clusters)
 
     def spawn_duplicate_pair_worker(self, queue_size: int = 1000, start_id: int = None, threshold: float = 200) \
             -> Tuple[mp.Queue, th.Thread]:
         """
         Function creates a worker thread which continuously enqueues dicts of each matching pair into the returned
         transfer queue.
@@ -1297,15 +1389,15 @@
     def continuous_preprocessing_error_worker(self):
         """
         TODO docstring
         :return:
         """
         raise NotImplementedError("Need to implement that one")
 
-    def build_loose_duplicate_cluster(self, similarity: float = None):
+    def _build_loose_duplicate_cluster(self, similarity: float = None):
         """
         Function generates a list of dicts containing duplicates. Each dict in the list satisfies that there exists at
         least **one** path between each two images. It is **not** guaranteed that within a cluster each pair of images
         matches the similarity threshold.
 
         This function is implemented in **RAM** only. If the dataset to deduplicate is too large, it is possible that
         this function fails due to insufficient memory. A Database driven solution might exist in the future.
```

### Comparing `fast_diff_py-0.1.0/fast_diff_py/fast_diff_base.py` & `fast_diff_py-0.2.0/src/fast_diff_py/fast_diff_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,26 +18,30 @@
 
         Provided the base class is instantiated itself and not just called as the parent for FastDiffPy, the config
         from the main class is copied into this one and stored.
 
         :param cfg: config dict form parent class.
         """
         if cfg is not None:
+            # Instantiate config and ignore any existing config that is already there (done with cfg option)
             self.config = FastDiffPyConfig(cfg=cfg)
+
+            # Retention of config explicitly set to False since this class is intended to be instantiated in child
+            # workers.
             self.config.retain_config = False
 
 
     @property
     def db(self):
         return self.__db
 
     @db.setter
     def db(self, value):
         self.__db = value
-        if self.config.retain_db:
+        if self.config.retain_db and self.__db is not None:
             self.config.database = self.__db.create_config_dump()
             self.config.write_to_file()
 
     # ------------------------------------------------------------------------------------------------------------------
     # FIRST LOOP COMMON FUNCTIONS
     # ------------------------------------------------------------------------------------------------------------------
```

### Comparing `fast_diff_py-0.1.0/fast_diff_py/gpu_image_processor.py` & `fast_diff_py-0.2.0/src/fast_diff_py/gpu_image_processor.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/mariadb_database.py` & `fast_diff_py-0.2.0/src/fast_diff_py/mariadb_database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/sql_database.py` & `fast_diff_py-0.2.0/src/fast_diff_py/sql_database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py/utils.py` & `fast_diff_py-0.2.0/src/fast_diff_py/utils.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.1.0/fast_diff_py.egg-info/SOURCES.txt` & `fast_diff_py-0.2.0/src/fast_diff_py.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE.txt
 README.md
+pyproject.toml
 setup.cfg
 setup.py
-fast_diff_py/__init__.py
-fast_diff_py/child_processes.py
-fast_diff_py/config.py
-fast_diff_py/cpu_image_processor.py
-fast_diff_py/database.py
-fast_diff_py/datatransfer.py
-fast_diff_py/dif.py
-fast_diff_py/fastDif.py
-fast_diff_py/fast_diff_base.py
-fast_diff_py/gpu_image_processor.py
-fast_diff_py/mariadb_database.py
-fast_diff_py/sql_database.py
-fast_diff_py/utils.py
-fast_diff_py.egg-info/PKG-INFO
-fast_diff_py.egg-info/SOURCES.txt
-fast_diff_py.egg-info/dependency_links.txt
-fast_diff_py.egg-info/requires.txt
-fast_diff_py.egg-info/top_level.txt
+src/fast_diff_py/__init__.py
+src/fast_diff_py/child_processes.py
+src/fast_diff_py/config.py
+src/fast_diff_py/cpu_image_processor.py
+src/fast_diff_py/database.py
+src/fast_diff_py/datatransfer.py
+src/fast_diff_py/dif.py
+src/fast_diff_py/fastDif.py
+src/fast_diff_py/fast_diff_base.py
+src/fast_diff_py/gpu_image_processor.py
+src/fast_diff_py/mariadb_database.py
+src/fast_diff_py/sql_database.py
+src/fast_diff_py/utils.py
+src/fast_diff_py.egg-info/PKG-INFO
+src/fast_diff_py.egg-info/SOURCES.txt
+src/fast_diff_py.egg-info/dependency_links.txt
+src/fast_diff_py.egg-info/not-zip-safe
+src/fast_diff_py.egg-info/requires.txt
+src/fast_diff_py.egg-info/top_level.txt
```

