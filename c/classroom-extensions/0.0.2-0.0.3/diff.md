# Comparing `tmp/classroom_extensions-0.0.2.tar.gz` & `tmp/classroom_extensions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classroom_extensions-0.0.2.tar", last modified: Wed Jul  5 21:05:15 2023, max compression
+gzip compressed data, was "classroom_extensions-0.0.3.tar", last modified: Sat Jul  8 01:39:05 2023, max compression
```

## Comparing `classroom_extensions-0.0.2.tar` & `classroom_extensions-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/classroom_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/mariadb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/classroom_extensions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/classroom_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-05 21:05:15.000000 classroom_extensions-0.0.2/classroom_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 21:05:15.000000 classroom_extensions-0.0.2/classroom_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:05:15.000000 classroom_extensions-0.0.2/classroom_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-05 21:05:15.000000 classroom_extensions-0.0.2/classroom_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 21:05:15.000000 classroom_extensions-0.0.2/classroom_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:05:15.172186 classroom_extensions-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/tests/test_mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/tests/test_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-05 21:05:03.000000 classroom_extensions-0.0.2/tests/test_plantuml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:05.336245 classroom_extensions-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-08 01:39:05.336245 classroom_extensions-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:05.332245 classroom_extensions-0.0.3/classroom_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/mariadb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/classroom_extensions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:05.332245 classroom_extensions-0.0.3/classroom_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-08 01:39:05.000000 classroom_extensions-0.0.3/classroom_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-08 01:39:05.000000 classroom_extensions-0.0.3/classroom_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:39:05.000000 classroom_extensions-0.0.3/classroom_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-08 01:39:05.000000 classroom_extensions-0.0.3/classroom_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:39:05.000000 classroom_extensions-0.0.3/classroom_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:39:05.336245 classroom_extensions-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:05.336245 classroom_extensions-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/tests/test_mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/tests/test_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-08 01:38:56.000000 classroom_extensions-0.0.3/tests/test_plantuml.py
```

### Comparing `classroom_extensions-0.0.2/LICENSE` & `classroom_extensions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.2/PKG-INFO` & `classroom_extensions-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom_extensions
-Version: 0.0.2
+Version: 0.0.3
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
```

### Comparing `classroom_extensions-0.0.2/README.rst` & `classroom_extensions-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.2/classroom_extensions/mariadb.py` & `classroom_extensions-0.0.3/classroom_extensions/mariadb.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,53 +5,58 @@
 An extension to create the %%sql magic command using the MariaDB kernel to
 execute the commands using the CLI client. Although it uses the MariaDB kernel, using it as
 an extension does not limit the notebook to executing only SQL commands. This assumes you have
 
 Note: MariaDB server and client installed, and that you have created a MariaDB kernel
 configuration file before loading this extension.
 """
-from IPython.core.magic import (magics_class, cell_magic)
+from IPython.core.magic import magics_class, cell_magic
 from IPython.core.magics.display import DisplayMagics
-from IPython.core.getipython import get_ipython
 from IPython.display import display, HTML
 from mariadb_kernel.code_parser import CodeParser
 from mariadb_kernel.mariadb_client import MariaDBClient, ServerIsDownError
 from mariadb_kernel.client_config import ClientConfig
 
 
 @magics_class
 class MariaDBMagics(DisplayMagics):
+    """Implements the MariaDB magics using the database
+    client provided by the MariaDB kernel"""
+
     db_client: MariaDBClient
     in_notebook: bool
 
     def __init__(self, shell):
         super().__init__(shell=shell)
-        self.in_notebook = shell.has_trait('kernel')
+        self.in_notebook = shell.has_trait("kernel")
         self.log = shell.log
         config = ClientConfig(self.log)
         self.db_client = MariaDBClient(self.log, config)
         self.db_client.start()
 
     def __del__(self):
         self.db_client.stop()
 
     @cell_magic
-    def sql(self, line='', cell=None):
+    def sql(self, line: str = "", cell: str = None) -> None:
         """
         Code to intercept the SQL code and execute it using MariaDB iPython kernel.
 
-        :param line not used, included to avoid error
-        :param cell: The contents of the cell to execute
-        :return: None
+        Args:
+            line: Not used, included to avoid error
+            cell: The contents of the cell to execute
+
+        Returns:
+            None
         """
         parser: CodeParser
         try:
             parser = CodeParser(self.log, cell, ";")
-        except ValueError as e:
-            self.log.error(f"Error with SQL parser: {str(e)}")
+        except ValueError as value_error:
+            self.log.error(f"Error with SQL parser: {str(value_error)}")
             return
 
         result = ""
         for stmt in parser.get_sql():
             result += self.db_client.run_statement(stmt)
 
             if self.db_client.iserror():
@@ -61,21 +66,20 @@
         display_obj = HTML(result) if self.in_notebook else result
         display(display_obj)
 
 
 def load_ipython_extension(ipython):
     """
     Loads the ipython extension
-    :param ipython: The currently active `InteractiveShell` instance.
-    :return: None
+
+    Args:
+        ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
+
+    Returns:
+        None
     """
     try:
         ipython.register_magics(MariaDBMagics(ipython))
-    except ServerIsDownError as se:
-        ipython.log.error(f"Error trying to access MariaDB Server: {se}")
-    except NameError as ne:
-        ipython.log.error(f"Error registering the magic command: {ne}")
-
-
-# Check if the module has not been loaded with %load_ext
-if '__IPYTHON__' not in globals():
-    load_ipython_extension(get_ipython())
+    except ServerIsDownError as server_error:
+        ipython.log.error(f"Error trying to access MariaDB Server: {server_error}")
+    except NameError as name_error:
+        ipython.log.error(f"Error registering the magic command: {name_error}")
```

### Comparing `classroom_extensions-0.0.2/classroom_extensions/mariadb_install.py` & `classroom_extensions-0.0.3/classroom_extensions/mariadb_install.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,66 +4,89 @@
 """
 An extension to install MariaDB, create the config file required by the
 MariaDB Jupyter to access it, and load a sample database.
 
 Note: This extension assumes that you are working in Google Colab
 running Ubuntu 20.04.
 """
+import time
+from os import path
+import json
+from argparse import ArgumentParser
 from IPython.core.magic import magics_class, line_magic, Magics
 from IPython.core.getipython import get_ipython
 from .util import exec_cmd, get_os_release, is_colab, get_user
-from argparse import ArgumentParser
 
 SAMPLE_DB = "https://www.mariadbtutorial.com/wp-content/uploads/2019/10/nation.zip"
 START_DB_TIMEOUT = 5  # Timeout for starting MariaDB
 
 
 @magics_class
 class MariaDBInstaller(Magics):
+    """
+    Implements the behaviour of the magic for installing MariaDB on Google Colab.
+    """
+
     in_notebook: bool
     _arg_parser: ArgumentParser
     _db_user: str
     _db_pass: str
 
     def __init__(self, shell):
         super().__init__(shell=shell)
         self._arg_parser = self._create_parser()
-        self.in_notebook = shell.has_trait('kernel')
+        self.in_notebook = shell.has_trait("kernel")
         self._db_user = get_user()
         self._db_pass = ""
 
     @classmethod
     def _create_parser(cls) -> ArgumentParser:
         parser = ArgumentParser()
-        parser.add_argument("-p", "--password", type=str, default=None,
-                            help="the password for the root user")
-        parser.add_argument("-s", "--sample_db", action='store_true',
-                            help="the password for the root user")
+        parser.add_argument(
+            "-p",
+            "--password",
+            type=str,
+            default=None,
+            help="the password for the root user",
+        )
+        parser.add_argument(
+            "-s",
+            "--sample_db",
+            action="store_true",
+            help="the password for the root user",
+        )
         return parser
 
     @classmethod
     def _meet_requirements(cls) -> bool:
-        """ Check if running on Colab with the right Ubuntu release """
-        return True if is_colab() and get_os_release().startswith('20.') else False
+        """
+        Check if running on Colab with the right Ubuntu release
+
+        Returns:
+            True if running on Google Colab on Ubuntu 20.xx container
+        """
+        return is_colab() and get_os_release().startswith("20.")
 
     @classmethod
     def _start_mariadb(cls) -> None:
-        """ Start MariaDB """
-        import time
-        get_ipython().system_raw('service mysql start &')
+        """Starts MariaDB"""
+
+        get_ipython().system_raw("service mysql start &")
         print("Waiting for a few seconds for MariaDB server to start...")
         time.sleep(START_DB_TIMEOUT)
 
     @line_magic
     def install_mariadb(self, line: str):
-        """ Install MariaDB, mariadb_kernel, sqlparse, etc """
+        """Install MariaDB, mariadb_kernel, sqlparse, etc"""
 
         if not self._meet_requirements():
-            print("Note: the magics for installing and configuring "
-                  "MariaDB may not work outside Google Colab")
+            print(
+                "Note: the magics for installing and configuring "
+                "MariaDB may not work outside Google Colab"
+            )
 
         args = self._arg_parser.parse_args(line.split() if line else "")
         if args.password is None:
             print("Error: you must provide a password using --password=password")
             return
 
         self._db_pass = args.password
@@ -71,58 +94,58 @@
         print("Running apt update...")
         exec_cmd("apt update -y")
         print("Installing MariaDB...")
         exec_cmd("apt install mariadb-server libmariadb-dev libmariadb3 -y")
         print("Installing required python packages...")
         exec_cmd("pip3 install mariadb==1.0.11 mariadb_kernel==0.2.0 sqlparse==0.4.4")
 
-        from os import path
-        import json
-
         self._start_mariadb()  # First start MariaDB
 
-        sql_stmt = f"ALTER USER '{self._db_user}'@'localhost' IDENTIFIED BY '{self._db_pass}'"
-        exec_cmd(f"mariadb -e \"{sql_stmt}\"")
+        sql_stmt = (
+            f"ALTER USER '{self._db_user}'@'localhost' IDENTIFIED BY '{self._db_pass}'"
+        )
+        exec_cmd(f'mariadb -e "{sql_stmt}"')
         exec_cmd("mkdir -p ~ /.jupyter")  # the config file must go in .jupyter
         config_path = path.join(path.expanduser("~"), ".jupyter/mariadb_config.json")
         client_conf = {
             "user": "root",
             "host": "localhost",
             "port": "3306",
             "password": self._db_pass,
             "start_server": "False",
             "client_bin": "/usr/bin/mariadb",
             "server_bin": "/usr/bin/mariadbd",
-            "socket": "/run/mysqld/mysqld.sock"
+            "socket": "/run/mysqld/mysqld.sock",
         }
-        with open(config_path, "w") as f:
-            f.write(json.dumps(client_conf, indent=4))
+        with open(config_path, "w", encoding="utf-8") as config_file:
+            config_file.write(json.dumps(client_conf, indent=4))
 
         # Load the sample database, if required
         if load_sample_db:
             self._load_sample_db()
         print("Done.")
 
     def _load_sample_db(self):
-        """ Configure a sample MariaDB database """
+        """Configure a sample MariaDB database"""
         exec_cmd(f"wget {SAMPLE_DB}")
         exec_cmd("unzip -o nation.zip")
         print("Importing nation database...")
-        exec_cmd(f"mariadb -e \"source nation.sql\" --user={self._db_user} --password={self._db_pass}")
+        exec_cmd(
+            f'mariadb -e "source nation.sql" --user={self._db_user} --password={self._db_pass}'
+        )
         exec_cmd("rm nation.zip")
 
 
 def load_ipython_extension(ipython):
     """
     Loads the ipython extension
-    :param ipython: The currently active `InteractiveShell` instance.
-    :return: None
+
+    Args:
+        ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
+
+    Returns:
+        None
     """
     try:
         ipython.register_magics(MariaDBInstaller(ipython))
     except NameError:
         print("IPython shell not available.")
-
-
-# Check if the module has not been loaded with %load_ext
-if '__IPYTHON__' not in globals():
-    load_ipython_extension(get_ipython())
```

### Comparing `classroom_extensions-0.0.2/classroom_extensions/node.py` & `classroom_extensions-0.0.3/classroom_extensions/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,110 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+"""
+The code customizes IPython's %%javascript magic by introducing line arguments
+that allow for executing the JavaScript code on the server side (via Node.js).
+When executed on the browser, the magic creates a section in the code cell that
+mimics the browser's console
+"""
 
-from IPython.core.magic import (magics_class, cell_magic)
-from IPython.core.magics.display import DisplayMagics
-from IPython.core.getipython import get_ipython
-from IPython.display import display, Javascript
 from argparse import ArgumentParser
 from functools import partial
-from typing import Any
+from typing import Any, Callable, AnyStr
 from os import path, environ
+from asyncio import streams
 import asyncio
 import contextlib
 import io
 import uuid
 import shutil
 import psutil
+from IPython.core.magic import magics_class, cell_magic
+from IPython.core.magics.display import DisplayMagics
+from IPython.display import display, Javascript
 
 
 # timeout to wait for a node server process to start (in seconds)
 START_SERVER_TIMEOUT = 5
 
 
 class NodeProcessManager:
-    """ Used to manage the execution of Node processes """
+    """Used to manage the execution of Node processes"""
+
     _node_cmd: str = "/usr/bin/node"
 
     def __init__(self):
         self._daemons: dict[int, Any] = {}
-        self._node_cmd = shutil.which('node')  # Try to discover full path of node command
+        self._node_cmd = shutil.which(
+            "node"
+        )  # Try to discover full path of node command
 
     @classmethod
-    async def read_stream(cls, proc, stream, callback) -> None:
+    async def read_stream(
+        cls,
+        proc,
+        stream: streams.StreamReader,
+        callback: Callable[[AnyStr], None],
+    ) -> None:
         """
         Reads the stout/stderr stream of a given process
-        :param proc: the process to read the output from
-        :param stream: the stdout stream
-        :param callback: a function to call on each line read from the stream
-        :return: None
+
+        Args:
+            proc: the process to read the output from
+            stream: the stream to read from
+            callback: the callback function to call when data is read
+
+        Returns:
+            None
         """
         while proc.returncode is None:
             data = await stream.readline()
             if not data:
                 break
             callback(data.decode().rstrip())
 
     @contextlib.asynccontextmanager
-    async def open_process(self, cmd: str, *cmd_args: dict, work_dir: str = None,
-                           env_vars: dict = None, daemon: bool = False,
-                           stdout_callback=print) -> None:
+    async def open_process(
+        self,
+        cmd: str,
+        *cmd_args: dict,
+        work_dir: str = None,
+        env_vars: dict = None,
+        daemon: bool = False,
+        stdout_callback: Callable[[AnyStr], None] = print,
+    ) -> None:
         """
         Creates a new Node process
 
-        :param cmd: the command to execute
-        :param cmd_args: the command arguments
-        :param work_dir: the path to the working directory
-        :param env_vars: the environment variables to set
-        :param daemon: True if the process will run as a daemon
-        :param stdout_callback: the callback function to call when reading the output stream
-        :return: None
+        Args:
+            cmd: the command to execute
+            *cmd_args: the command arguments
+            work_dir: the path to the working directory
+            env_vars: the environment variables to set
+            daemon: True if the process will run in background
+            stdout_callback: the callback function to call when reading the output stream
+
+        Returns:
+            None
         """
         proc = await asyncio.create_subprocess_exec(
-            cmd, *cmd_args,
+            cmd,
+            *cmd_args,
             stdin=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.STDOUT,
-            cwd=work_dir, env=env_vars
+            cwd=work_dir,
+            env=env_vars,
+        )
+        stream_task = asyncio.create_task(
+            self.read_stream(proc, proc.stdout, stdout_callback)
         )
-        stream_task = asyncio.create_task(self.read_stream(proc,
-                                                           proc.stdout,
-                                                           stdout_callback))
 
-        async def server_wait():
+        async def server_wait() -> None:
+            """Shields the execution and stream reader tasks for a background process"""
             server_task = asyncio.create_task(proc.wait())
             try:
                 await asyncio.shield(server_task)
                 await asyncio.shield(stream_task)
             except asyncio.CancelledError:
                 pass
 
@@ -86,83 +116,102 @@
                 await stream_task
             else:
                 try:
                     await asyncio.wait_for(server_wait(), START_SERVER_TIMEOUT)
                 except asyncio.TimeoutError:
                     pass
 
-    async def execute(self, js_file: str = None, port: int = None,
-                      stdout_callback=partial(print, flush=True)) -> None:
+    async def execute(
+        self,
+        js_file: str = None,
+        port: int = None,
+        stdout_callback: Callable[[AnyStr], None] = partial(print, flush=True),
+    ) -> None:
         """
         Use Node.js to run the provided script. If a port is given,
-        the script will be run as a daemon
-        :param js_file: the full path to the JavaScript file
-        :param port: the port number
-        :param stdout_callback: the callback function to call when reading the output stream
-        :return: None
+        the script will be run in background without blocking the cell
+
+        Args:
+            js_file: the full path to the JavaScript file
+            port: the port number for the server
+            stdout_callback: the callback function to call when reading the output stream
+
+        Returns:
+            None
         """
         server_env = environ.copy()
         if port:
-            self.kill_daemon(port)   # Kill any Node process using the port
+            self.kill_daemon(port)  # Kill any Node process using the port
             server_env["NODE_PORT"] = str(port)
 
         work_dir = path.dirname(path.realpath(js_file))
         daemon = port is not None
-        async with self.open_process(self._node_cmd, js_file,
-                                     work_dir=work_dir,
-                                     env_vars=server_env, daemon=daemon,
-                                     stdout_callback=stdout_callback) as proc:
+        async with self.open_process(
+            self._node_cmd,
+            js_file,
+            work_dir=work_dir,
+            env_vars=server_env,
+            daemon=daemon,
+            stdout_callback=stdout_callback,
+        ) as proc:
             if daemon:
                 self._daemons[port] = proc
 
     @classmethod
-    def _force_kill(cls, port):
-        """ To kill a Node.js process listening on a given port """
-        for proc in psutil.process_iter(['pid', 'name', 'connections']):
+    def _force_kill(cls, port: int) -> None:
+        """To kill a Node.js process listening on a given port"""
+        for proc in psutil.process_iter(["pid", "name", "connections"]):
             try:
                 for conn in proc.connections():
                     if conn.status == psutil.CONN_LISTEN and conn.laddr.port == port:
-                        print(f"Killing existing {proc.name()} process, id {proc.pid} "
-                              f"and listening on port {port}", flush=True)
+                        print(
+                            f"Killing existing {proc.name()} process, id {proc.pid} "
+                            f"and listening on port {port}",
+                            flush=True,
+                        )
                         proc.kill()
             except (psutil.AccessDenied, psutil.NoSuchProcess):
                 pass
 
-    def kill_daemon(self, port) -> None:
+    def kill_daemon(self, port: int) -> None:
         """
-        Kills a previously started daemon process
-        :param port: the port the daemon is likely listening to
-        :return: None
+        Kills a previously started background process
+
+        Args:
+            port: the port the daemon is likely listening to
+
+        Returns:
+            None
         """
         if port in self._daemons:
             process = self._daemons[port]
             try:
                 process.kill()
             except ProcessLookupError:
                 print(f"No node process on port {port}, ok to continue...")
         else:
             self._force_kill(port)
 
-    def cleanUp(self):
-        """ Some cleanup during testing and extension unloading """
+    def clean_up(self) -> None:
+        """Some cleanup during testing and extension unloading"""
         for proc in self._daemons.values():
             try:
                 proc.terminate()
-            except ProcessLookupError as e:
-                print(f"Error: process not found {e}")
+            except ProcessLookupError as process_error:
+                print(f"Error: process not found {process_error}")
         self._daemons.clear()
 
     def __del__(self):
-        self.cleanUp()
+        self.clean_up()
 
 
 # This code JavaScript will be included with the cell's code to
 # redirect the output of calls to console.[log, error, warn] to the
 # result section of the cell
-_cell_console = """
+_CELL_CONSOLE = """
 function c_msg(type, o_func, ...args) {
     let p = document.createElement("p");
     p.classList.add(`console-${type}`);
     p.textContent = args.join(" ");
     document.getElementById('console-box').appendChild(p);
     o_func(...args);
 }
@@ -249,98 +298,142 @@
 
 class JavascriptWithConsole(Javascript):
     """
     This class extends JavaScript to intercept calls to console.log
     and make a result section of the cell.
     """
 
-    CELL_CONSOLE: str = _cell_console
+    CELL_CONSOLE: str = _CELL_CONSOLE
 
-    def __init__(self, data=None, url=None, filename=None, lib=None, css=None):
-        super().__init__(data=data, url=url, filename=filename, lib=lib, css=None)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
     def _repr_javascript_(self):
+        """Creates the full JavaScript code to be delivered to the browser"""
         return self.CELL_CONSOLE + super()._repr_javascript_()
 
 
 @magics_class
 class NodeMagics(DisplayMagics):
+    """
+    Implements the customizations to the %%javascript magic
+    that enables JavaScript execution by Node.js
+    """
+
     _arg_parser: ArgumentParser
     _proc_mgmt: NodeProcessManager
     _in_notebook: bool
 
     def __init__(self, shell):
         super().__init__(shell=shell)
         self._arg_parser = self._create_parser()
         self._proc_mgmt = NodeProcessManager()
-        self._in_notebook = shell.has_trait('kernel')
+        self._in_notebook = shell.has_trait("kernel")
 
     @classmethod
     def _create_parser(cls) -> ArgumentParser:
+        """Creates a parser to the line arguments"""
         parser = ArgumentParser()
-        parser.add_argument("-t", "--target", type=str,
-                            choices=['browser', 'node', 'disk'], default="browser",
-                            help="the target for script execution")
-        parser.add_argument("-f", "--filename", type=str,
-                            help="filename when cell contents are saved to disk")
-        parser.add_argument("-p", "--port", type=int,
-                            help="a port number if the cell starts a Node server process")
+        parser.add_argument(
+            "-t",
+            "--target",
+            type=str,
+            choices=["browser", "node", "disk"],
+            default="browser",
+            help="the target for script execution",
+        )
+        parser.add_argument(
+            "-f",
+            "--filename",
+            type=str,
+            help="filename when cell contents are saved to disk",
+        )
+        parser.add_argument(
+            "-p",
+            "--port",
+            type=int,
+            help="a port number if the cell starts a Node server process",
+        )
         return parser
 
     @classmethod
     def _save_script(cls, filename: str, cell_content: str) -> str:
-        """ Create the JavaScript file for Node to run """
+        """
+        Creates the JavaScript file for Node to run
+
+        Args:
+            filename: the file name
+            cell_content: the cell contents to save into the file
+
+        Returns:
+            Name of the file created
+        """
         if not filename:
             filename = f"{uuid.uuid4().hex}.js"
-        with io.open(filename, 'w', encoding='utf-8') as f:
-            f.write(cell_content)
+        with io.open(filename, "w", encoding="utf-8") as script_file:
+            script_file.write(cell_content)
         return filename
 
     def _run_on_node(self, js_file: str, port: int = None) -> None:
+        """
+        Triggers the execution on Node.js
+
+        Args:
+            js_file: path to the file to execute
+            port: the port number to use, if the scripts launches a server
+
+        Returns:
+            None
+        """
         if self._in_notebook:
             loop = asyncio.get_event_loop()
             loop.create_task(self._proc_mgmt.execute(js_file, port))
         else:
             asyncio.run(self._proc_mgmt.execute(js_file, port))
 
     @cell_magic
-    def javascript(self, line=None, cell=None):
+    def javascript(self, line: str = None, cell: str = None) -> None:
+        """
+        Method called when executing %%javascript
+        Args:
+            line: line arguments (e.g. --target, --filename)
+            cell: the JavaScript code to execute
+
+        Returns:
+            None
+        """
         args = self._arg_parser.parse_args(line.split() if line else "")
 
-        if args.target == 'node':
+        if args.target == "node":
             if not args.filename:
-                raise ValueError(
-                    "--filename is required when using --target=node"
-                )
+                raise ValueError("--filename is required when using --target=node")
             js_file = self._save_script(args.filename, cell)
             self._run_on_node(js_file, args.port)
-        elif args.target == 'browser':
+        elif args.target == "browser":
             display(JavascriptWithConsole(cell))
-        elif args.target == 'disk':
+        elif args.target == "disk":
             if not args.filename:
-                raise ValueError(
-                    "--filename is required when using --target=disk"
-                )
+                raise ValueError("--filename is required when using --target=disk")
             self._save_script(args.filename, cell)
 
 
 def load_ipython_extension(ipython):
     """
     Loads the ipython extension
-    :param ipython: The currently active `InteractiveShell` instance.
-    :return: None
+
+    Args:
+        ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
+
+    Returns:
+        None
     """
     try:
         node_magic = NodeMagics(ipython)
         ipython.register_magics(node_magic)
         ipython.node_magic = node_magic
     except NameError:
         print("IPython shell not available.")
 
 
 def unload_ipython_extension(ipython):
+    """Unloads the extension"""
     del ipython.node_magic
-
-
-# Check if the module has not been loaded with %load_ext
-if '__IPYTHON__' not in globals():
-    load_ipython_extension(get_ipython())
```

### Comparing `classroom_extensions-0.0.2/classroom_extensions/plantuml.py` & `classroom_extensions-0.0.3/classroom_extensions/plantuml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """ Extension that uses PlantUML to draw multiple types of diagrams """
 
-from IPython.core.magic import (magics_class, cell_magic, line_magic)
-from IPython.core.magics.display import DisplayMagics, display
-from IPython.core.getipython import get_ipython
-from IPython.display import SVG, Image
 from argparse import ArgumentParser
 from copy import copy
 from os.path import expanduser, exists
-from plantweb.render import render
 import json
+from plantweb.render import render
+from IPython.core.magic import magics_class, cell_magic, line_magic
+from IPython.core.magics.display import DisplayMagics, display
+from IPython.display import SVG, Image
 
-__all__ = [
-    "load_ipython_extension",
-    "PlantUmlMagics"
-]
+__all__ = ["load_ipython_extension", "PlantUmlMagics"]
 
 
 DEFAULT_PLANTWEB_CONFIG = {
-    'engine': 'plantuml',
-    'format': 'svg',
-    'server': 'http://plantuml.com/plantuml/',
-    'use_cache': True,
-    'cache_dir': '~/.cache/plantweb'
+    "engine": "plantuml",
+    "format": "svg",
+    "server": "http://plantuml.com/plantuml/",
+    "use_cache": True,
+    "cache_dir": "~/.cache/plantweb",
 }
 
 
 @magics_class
 class PlantUmlMagics(DisplayMagics):
+    """
+    Implements magics for using PlantUML and enabling creating
+    several types of diagrams in Jupyter notebooks
+    """
+
     _config_path: str = expanduser("~/.plantwebrc")
+    """ The default path of the config file """
 
     def __init__(self, shell=None):
         super().__init__(shell=shell)
         self._plantweb_config = self._load_plantweb_config()
 
     @property
-    def plantweb_config(self):
+    def plantweb_config(self) -> dict:
+        """Returns the plantweb configuration"""
         return self._plantweb_config
 
     def _load_plantweb_config(self) -> dict:
         if not exists(self._config_path):
             return copy(DEFAULT_PLANTWEB_CONFIG)
-        with open(self._config_path, 'r') as fd:
-            return dict(json.loads(fd.read()))
+        with open(self._config_path, "r", encoding="utf-8") as config_file:
+            return dict(json.loads(config_file.read()))
 
     def _save_plantuml_config(self) -> None:
-        with open(self._config_path, 'w') as fd:
-            fd.write(json.dumps(self._plantweb_config))
+        with open(self._config_path, "w", encoding="utf-8") as config_file:
+            config_file.write(json.dumps(self._plantweb_config))
 
     @cell_magic
-    def plantuml(self, line=None, cell=None):
-        """ Cell magic responsible for rendering the SVG/PNG diagram """
-        output, out_format, _, _ = render(
-            cell,
-            engine='plantuml',
-            format='svg'
-        )
-        if out_format == 'svg':
+    def plantuml(self, line: str = None, cell: str = None):
+        """Cell magic responsible for rendering the SVG/PNG diagram"""
+        output, out_format, _, _ = render(cell, engine="plantuml", format="svg")
+        if out_format == "svg":
             svg = SVG(data=output)
             display(svg)
         else:
             img = Image(data=output)
             display(img)
 
     @line_magic
-    def plantuml_config(self, line=None):
-        """ Used to set the server address in case one wants to use its local PlatUML server """
+    def plantuml_config(self, line=None) -> None:
+        """Used to set the server address in case one wants to use its local PlatUML server"""
         parser = ArgumentParser()
-        parser.add_argument("-s", "--server", type=str, help="Address of the PlantUML server to use")
+        parser.add_argument(
+            "-s", "--server", type=str, help="Address of the PlantUML server to use"
+        )
         args = parser.parse_args(line.split() if line else "")
         if args.server:
-            self._plantweb_config['server'] = args.server
+            self._plantweb_config["server"] = args.server
             self._save_plantuml_config()
         else:
-            print("Use --server=address to provide the address of a valid PlantUML server")
+            print(
+                "Use --server=address to provide the address of a valid PlantUML server"
+            )
 
 
-def load_ipython_extension(ipython):
+def load_ipython_extension(ipython) -> None:
     """
-    Loads the ipython extension
-    :param ipython: The currently active `InteractiveShell` instance.
-    :return: None
+    To unload the extension
+    Args:
+        ipython: the current interactive shell
+
+    Returns:
+        None
     """
     try:
         uml_magics = PlantUmlMagics(ipython)
         ipython.register_magics(uml_magics)
         ipython.node_magic = uml_magics
     except NameError:
         print("IPython shell not available.")
-
-
-# Check if the module has not been loaded with %load_ext
-if '__IPYTHON__' not in globals():
-    load_ipython_extension(get_ipython())
```

### Comparing `classroom_extensions-0.0.2/classroom_extensions.egg-info/PKG-INFO` & `classroom_extensions-0.0.3/classroom_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom-extensions
-Version: 0.0.2
+Version: 0.0.3
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
```

### Comparing `classroom_extensions-0.0.2/classroom_extensions.egg-info/SOURCES.txt` & `classroom_extensions-0.0.3/classroom_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.2/pyproject.toml` & `classroom_extensions-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.2/tests/test_html.py` & `classroom_extensions-0.0.3/tests/test_html.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+""" Tests the HTML magics """
 
 import unittest
+from classroom_extensions.html import HTMLWithConsole
 from .base import BaseTestCase
 
 
 class TestHTML(BaseTestCase):
-    """ Testcase for the HTML extension """
+    """Testcase for the HTML extension"""
 
     def setUp(self) -> None:
-        self.ipython.extension_manager.load_extension('classroom_extensions.html')
+        self.ipython.extension_manager.load_extension("classroom_extensions.html")
 
     def tearDown(self):
-        self.ipython.extension_manager.unload_extension('classroom_extensions.html')
+        self.ipython.extension_manager.unload_extension("classroom_extensions.html")
 
     def test_javascript(self):
+        """Test HTML with JavaScript"""
         print("Testing HTML with JavaScript")
-        from classroom_extensions.html import HTMLWithConsole
-        self.ipython.extension_manager.load_extension('classroom_extensions.html')
-        expected_dir = {"text/plain": f"<{HTMLWithConsole.__module__}."
-                                      f"{HTMLWithConsole.__qualname__} object>"}
-        cell_content = f"console.log('----');"
+        self.ipython.extension_manager.load_extension("classroom_extensions.html")
+        expected_dir = {
+            "text/plain": f"<{HTMLWithConsole.__module__}."
+            f"{HTMLWithConsole.__qualname__} object>"
+        }
+        cell_content = "console.log('----');"
         self.ipython.run_cell_magic("html", line="--console", cell=f"{cell_content}")
         self.assertEqual(expected_dir, self.publisher.display_output.pop())
-        self.ipython.extension_manager.unload_extension('classroom_extensions.html')
+        self.ipython.extension_manager.unload_extension("classroom_extensions.html")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `classroom_extensions-0.0.2/tests/test_mariadb.py` & `classroom_extensions-0.0.3/tests/test_mariadb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+""" Tests the MariaDB magics """
 
 import unittest
+import json
+from os import path
 from .base import BaseTestCase
 
-
-MARIADB_USER = 'testuser'
-MARIADB_PASSWORD = 'testpassword'
+MARIADB_USER = "testuser"
+MARIADB_PASSWORD = "testpassword"
 
 
 class TestMariaDB(BaseTestCase):
-    """ Testcase for the MariaDB extension """
+    """Testcase for the MariaDB extension"""
 
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
 
         # Create the MariaDB kernel config file
         cls._create_mariadb_config()
 
     def setUp(self):
         # Custom path to MariaDB kernel config
-        self.ipython.run_line_magic('env', 'JUPYTER_CONFIG_DIR /tmp/')
+        self.ipython.run_line_magic("env", "JUPYTER_CONFIG_DIR /tmp/")
 
         # Load the mariadb extension
-        self.ipython.extension_manager.load_extension('classroom_extensions.mariadb')
+        self.ipython.extension_manager.load_extension("classroom_extensions.mariadb")
 
     def tearDown(self):
-        self.ipython.extension_manager.unload_extension('classroom_extensions.mariadb')
+        self.ipython.extension_manager.unload_extension("classroom_extensions.mariadb")
 
     def test_show_databases(self):
+        """ Tests the execution of SQL command """
         print("Testing SHOW DATABASES command.")
-        self.ipython.run_cell_magic('sql', line='', cell="SHOW DATABASES;")
+        self.ipython.run_cell_magic("sql", line="", cell="SHOW DATABASES;")
         pattern = r"<TABLE BORDER=1><TR><TH>Database</TH></TR><TR><TD>(.*?)</TD></TR>.+</TABLE>"
-        self.assertRegex(text=str(self.publisher.display_output.pop()),
-                         expected_regex=pattern)
+        self.assertRegex(
+            text=str(self.publisher.display_output.pop()), expected_regex=pattern
+        )
 
     @classmethod
     def _create_mariadb_config(cls):
         """
         Create the MariaDB kernel config file required by the MariaDB extension.
         The file contains information on how to access the MariaDB server
         """
-        from os import path
-        import json
+
         config_path = path.join("/tmp", "mariadb_config.json")
         client_conf = {
             "user": f"{MARIADB_USER}",
             "host": "localhost",
             "port": 3306,
             "password": f"{MARIADB_PASSWORD}",
             "start_server": "False",
             "client_bin": "/usr/bin/mariadb",
-            "socket": "/var/run/mysqld/mysqld.sock"
+            "socket": "/var/run/mysqld/mysqld.sock",
         }
-        with open(config_path, "w") as f:
-            f.write(json.dumps(client_conf, indent=4))
-            f.flush()
+        with open(config_path, "w", encoding="utf-8") as config_file:
+            config_file.write(json.dumps(client_conf, indent=4))
+            config_file.flush()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `classroom_extensions-0.0.2/tests/test_nodejs.py` & `classroom_extensions-0.0.3/tests/test_nodejs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+""" Tests the JavaScript magics """
 
 import unittest
+import asyncio
 from IPython.utils import io
+from classroom_extensions.node import NodeProcessManager
+from classroom_extensions.node import JavascriptWithConsole
 from .base import BaseTestCase
-import asyncio
 
 
 class TestNodeJs(BaseTestCase):
-    """ Testcase for the NodeJs extension """
+    """Testcase for the NodeJs extension"""
 
     def setUp(self) -> None:
         # Loads the extension
-        self.ipython.extension_manager.load_extension('classroom_extensions.node')
+        self.ipython.extension_manager.load_extension("classroom_extensions.node")
 
     def tearDown(self) -> None:
-        self.ipython.extension_manager.unload_extension('classroom_extensions.node')
+        self.ipython.extension_manager.unload_extension("classroom_extensions.node")
 
     def test_process_manager(self):
+        """Tests the process manager"""
         print("Test process manager.")
-        from classroom_extensions.node import NodeProcessManager
         proc_manager = NodeProcessManager()
         where_ls = ""
 
         def stdout_callback(data):
             nonlocal where_ls
             where_ls += data
 
         async def run_cmd():
-            async with proc_manager.open_process('which', 'uname', stdout_callback=stdout_callback):
+            async with proc_manager.open_process(
+                "which", "uname", stdout_callback=stdout_callback
+            ):
                 pass
 
         asyncio.run(run_cmd())
         self.assertRegex(text=where_ls, expected_regex=r"uname")
 
     def test_node_script(self):
+        """Tests executing server-side JavaScript"""
         print("Test executing Node.js script.")
         cell_output: str
         console_content = "------"
         with io.capture_output() as captured:
-            self.ipython.run_cell_magic("javascript",
-                                        line="--target=node --filename=/tmp/test.js",
-                                        cell=f"console.log('{console_content}');\n")
+            self.ipython.run_cell_magic(
+                "javascript",
+                line="--target=node --filename=/tmp/test.js",
+                cell=f"console.log('{console_content}');\n",
+            )
             cell_output = captured.stdout
         self.assertEqual(cell_output.strip(), console_content)
 
     def test_node_server(self):
+        """Tests the creation of a Node.js server"""
         print("Testing executing Node.js server...")
         cell_output: str
         expected_output = "Server listening at http://localhost:3000/"
         cell_content = """
             const http = require('http')
 
             const hostname = 'localhost'
@@ -62,26 +71,30 @@
             })
 
             server.listen(port, hostname, () => {
                 console.log(`Server listening at http://${hostname}:${port}/`)
             })
         """
         with io.capture_output() as captured:
-            self.ipython.run_cell_magic("javascript",
-                                        line="--target=node --filename=/tmp/server.js --port=3000",
-                                        cell=f"{cell_content}")
+            self.ipython.run_cell_magic(
+                "javascript",
+                line="--target=node --filename=/tmp/server.js --port=3000",
+                cell=f"{cell_content}",
+            )
             cell_output = captured.stdout
-        # TODO: Change this test. If the test case is run twice, it fails as another process is still running
         self.assertEqual(cell_output.strip(), expected_output)
 
     def test_javascript(self):
+        """Tests normal JavaScript code"""
         print("Testing JavaScript with console...")
-        from classroom_extensions.node import JavascriptWithConsole
-        expected_dir = {"text/plain": f"<{JavascriptWithConsole.__module__}."
-                                      f"{JavascriptWithConsole.__qualname__} object>"}
-        cell_content = f"console.log('----');"
+
+        expected_dir = {
+            "text/plain": f"<{JavascriptWithConsole.__module__}."
+            f"{JavascriptWithConsole.__qualname__} object>"
+        }
+        cell_content = "console.log('----');"
         self.ipython.run_cell_magic("javascript", line="", cell=f"{cell_content}")
         self.assertEqual(expected_dir, self.publisher.display_output.pop())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `classroom_extensions-0.0.2/tests/test_plantuml.py` & `classroom_extensions-0.0.3/tests/test_plantuml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+""" Tests the PlantUML magics """
 
 import unittest
+from classroom_extensions.plantuml import PlantUmlMagics
 from .base import BaseTestCase
 
 
 class TestPlantUML(BaseTestCase):
-    """ Testcase for the PlantUML extension """
+    """Testcase for the PlantUML extension"""
 
     def test_config(self):
+        """ Tests creating a config file """
         print("Testing PlantUML config...")
-        from classroom_extensions.plantuml import PlantUmlMagics
         magics1 = PlantUmlMagics(shell=self.ipython)
-        previous_server = magics1.plantweb_config['server']
+        previous_server = magics1.plantweb_config["server"]
         magics1.plantuml_config("--server=http://localhost:8080/plantuml/")
         magics2 = PlantUmlMagics(shell=self.ipython)
-        self.assertEqual("http://localhost:8080/plantuml/", magics2.plantweb_config['server'])
+        self.assertEqual(
+            "http://localhost:8080/plantuml/", magics2.plantweb_config["server"]
+        )
         magics2.plantuml_config(f"--server={previous_server}")
 
     def test_render(self):
+        """ Tests rendering a graph """
         print("Testing PlantUML rendering...")
-        from classroom_extensions.plantuml import PlantUmlMagics
         content = """
         actor Foo1
         boundary Foo2
         control Foo3
         entity Foo4
         database Foo5
         Foo1 -> Foo2 : To boundary
@@ -30,17 +36,22 @@
         Foo1 -> Foo4 : To entity
         Foo1 -> Foo5 : To database
         """
         magics = PlantUmlMagics(shell=self.ipython)
         magics.plantuml(cell=content)
 
     def test_load_extension(self):
+        """ Tests loading and unloading the extension """
         print("Testing loading/unloading extension...")
-        self.ipython.extension_manager.load_extension('classroom_extensions.plantuml')
-        second_load = self.ipython.extension_manager.load_extension('classroom_extensions.plantuml')
+        self.ipython.extension_manager.load_extension("classroom_extensions.plantuml")
+        second_load = self.ipython.extension_manager.load_extension(
+            "classroom_extensions.plantuml"
+        )
         self.assertEqual(second_load, "already loaded")
-        unload = self.ipython.extension_manager.unload_extension('classroom_extensions.plantuml')
+        unload = self.ipython.extension_manager.unload_extension(
+            "classroom_extensions.plantuml"
+        )
         self.assertEqual(unload, "no unload function")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

