# Comparing `tmp/py_basic_commands-0.2.25b2.tar.gz` & `tmp/py_basic_commands-0.2.25b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.25b2.tar", last modified: Wed Jul  5 00:58:58 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.25b3.tar", last modified: Sat Jul  8 20:27:43 2023, max compression
```

## Comparing `py_basic_commands-0.2.25b2.tar` & `py_basic_commands-0.2.25b3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.182967 py_basic_commands-0.2.25b3/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.182967 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/other/basic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:27:43.182967 py_basic_commands-0.2.25b3/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-08 20:27:43.000000 py_basic_commands-0.2.25b3/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-08 20:27:43.000000 py_basic_commands-0.2.25b3/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:27:43.000000 py_basic_commands-0.2.25b3/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 20:27:43.000000 py_basic_commands-0.2.25b3/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-08 20:27:31.000000 py_basic_commands-0.2.25b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-08 20:27:43.186967 py_basic_commands-0.2.25b3/setup.cfg
```

### Comparing `py_basic_commands-0.2.25b2/LICENSE.md` & `py_basic_commands-0.2.25b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/PKG-INFO` & `py_basic_commands-0.2.25b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.25b2
+Version: 0.2.25b3
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.25b2/README.md` & `py_basic_commands-0.2.25b3/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/__init__.py` & `py_basic_commands-0.2.25b3/py_basic_commands/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 # From json_scripts
 from py_basic_commands.json_scripts import create_json, read_json, write_json
 from py_basic_commands.json_scripts import CreateJson, ReadJson, WriteJson
 from py_basic_commands.json_scripts import JsonEditor
 
 # From other
-from py_basic_commands.other import choose_from_list, chunker, enter_to_continue, flatten_list, func_timer, _func_timer, try_traceback, timer, try_listdir
+from py_basic_commands.other import choose_from_list, chunker, enter_to_continue, flatten_list, func_timer, _func_timer, try_traceback, timer, try_listdir, try_moving
 from py_basic_commands.other import ChooseFromList, FunctionTimer, Timer
```

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/base.py` & `py_basic_commands-0.2.25b3/py_basic_commands/base.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from py_basic_commands.file_dir_scripts.get_src_path  import get_src_path
 from py_basic_commands.fscripts   import Fprint
 from py_basic_commands.base   import Base
+from os.path import exists
 from os     import makedirs
 
 fprint = Fprint()
 
 
 class CreateDirs(Base):
     """Create all required directories for the given path"""
@@ -29,21 +30,30 @@
                 Whether to print information about the directory creation process. Default is True
 
             Returns
             -------
             bool
                 Whether the directories were created
             """
-
             # Check input values
             do_print = kwargs.get('do_print', self.do_print)
-
+            
             # Set print config
             fprint.config(do_print=do_print)
 
+            if not isinstance(dst_path, str):
+                raise TypeError(f'dst_path must be a string, not {type(dst_path)}')
+            
+            elif dst_path == '':
+                raise ValueError('dst_path cannot be an empty string')
+            
+            elif exists(dst_path):
+                fprint(f'dst_path already exists: {dst_path!r}')
+                return False
+
             if dst_path == '':
                 return False
 
             dir_path = get_src_path(dst_path, ret_val='d', do_print=do_print)
 
             if dir_path == '':
                 return False
```

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/file_editor.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/file_editor.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """Get the path for the given source.
         
         Parameters
         ----------
         src_path : str
             Source path to get path for
         ret_val : str, optional
-            Return value; 'a': (directory path, filename), 'd': directory path, 'f': filename, by default 'a'
+            Return value; 'a': (directory path, file name), 'd': directory path, 'f': file name, by default 'a'
         do_print : bool, optional
             Print output, by default True
         
         Returns
         -------
         Any
             The path for the given source
```

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/write_file.py` & `py_basic_commands-0.2.25b3/py_basic_commands/file_dir_scripts/write_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.25b3/py_basic_commands/fscripts/finput.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.25b3/py_basic_commands/fscripts/fprint.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.25b3/py_basic_commands/fscripts/fprint_array.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/create_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/json_editor.py` & `py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/json_editor.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/read_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.25b3/py_basic_commands/json_scripts/write_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.25b3/py_basic_commands/other/choose_from_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,14 @@
             user_input = finput(text=input_text)
 
             try:
                 value_indx_lst = self._check_input(user_input, array, choose_total, start_num)
             except InavlidInputError as e:
                 print(e)
                 continue
-
-            print('No errors')
             break
         
         chosen_value_lst = [array[indx] for indx in value_indx_lst]
 
         if choose_total == 1 and self.ret_single_as_str:
             return chosen_value_lst[0]
```

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.25b3/py_basic_commands/other/function_timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.25b3/py_basic_commands/other/timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.25b3/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.25b2
+Version: 0.2.25b3
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.25b2/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.25b3/py_basic_commands.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 py_basic_commands/fscripts/fprint_array.py
 py_basic_commands/json_scripts/__init__.py
 py_basic_commands/json_scripts/create_json.py
 py_basic_commands/json_scripts/json_editor.py
 py_basic_commands/json_scripts/read_json.py
 py_basic_commands/json_scripts/write_json.py
 py_basic_commands/other/__init__.py
-py_basic_commands/other/basic_commands.py
+py_basic_commands/other/basic_functions.py
 py_basic_commands/other/choose_from_list.py
 py_basic_commands/other/function_timer.py
 py_basic_commands/other/timer.py
```

### Comparing `py_basic_commands-0.2.25b2/pyproject.toml` & `py_basic_commands-0.2.25b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.25-beta.2"
+version = "0.2.25-beta.3"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.25b2/setup.cfg` & `py_basic_commands-0.2.25b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.25-beta.2
+version = 0.2.25-beta.3
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

