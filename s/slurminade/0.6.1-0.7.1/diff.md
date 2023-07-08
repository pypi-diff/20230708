# Comparing `tmp/slurminade-0.6.1.tar.gz` & `tmp/slurminade-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurminade-0.6.1.tar", last modified: Thu Jun  8 20:34:31 2023, max compression
+gzip compressed data, was "slurminade-0.7.1.tar", last modified: Sat Jul  8 17:22:51 2023, max compression
```

## Comparing `slurminade-0.6.1.tar` & `slurminade-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:34:31.899640 slurminade-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 20:34:12.000000 slurminade-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-08 20:34:31.895640 slurminade-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-08 20:34:12.000000 slurminade-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 20:34:12.000000 slurminade-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:34:31.899640 slurminade-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-08 20:34:12.000000 slurminade-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:34:31.895640 slurminade-0.6.1/slurminade/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/function_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 20:34:12.000000 slurminade-0.6.1/slurminade/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:34:31.895640 slurminade-0.6.1/slurminade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 20:34:31.000000 slurminade-0.6.1/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.036314 slurminade-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.032314 slurminade-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.032314 slurminade-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-08 17:22:37.000000 slurminade-0.7.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-08 17:22:37.000000 slurminade-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-08 17:22:37.000000 slurminade-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-08 17:22:37.000000 slurminade-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-08 17:22:37.000000 slurminade-0.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 17:22:37.000000 slurminade-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-08 17:22:51.036314 slurminade-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-08 17:22:37.000000 slurminade-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.032314 slurminade-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-08 17:22:37.000000 slurminade-0.7.1/docs/slurminade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.036314 slurminade-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-08 17:22:37.000000 slurminade-0.7.1/examples/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-08 17:22:37.000000 slurminade-0.7.1/examples/example_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 17:22:37.000000 slurminade-0.7.1/examples/example_2b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-08 17:22:37.000000 slurminade-0.7.1/examples/example_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-08 17:22:37.000000 slurminade-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 17:22:37.000000 slurminade-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:22:51.036314 slurminade-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.032314 slurminade-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.036314 slurminade-0.7.1/src/slurminade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-08 17:22:37.000000 slurminade-0.7.1/src/slurminade/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.036314 slurminade-0.7.1/src/slurminade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-08 17:22:51.000000 slurminade-0.7.1/src/slurminade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-08 17:22:51.000000 slurminade-0.7.1/src/slurminade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:22:51.000000 slurminade-0.7.1/src/slurminade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 17:22:51.000000 slurminade-0.7.1/src/slurminade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 17:22:51.000000 slurminade-0.7.1/src/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:51.036314 slurminade-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:22:37.000000 slurminade-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 17:22:37.000000 slurminade-0.7.1/tests/test_create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 17:22:37.000000 slurminade-0.7.1/tests/test_dispatch_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-08 17:22:37.000000 slurminade-0.7.1/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-08 17:22:37.000000 slurminade-0.7.1/tests/test_subprocess.py
```

### Comparing `slurminade-0.6.1/LICENSE` & `slurminade-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slurminade-0.6.1/PKG-INFO` & `slurminade-0.7.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,234 +1,385 @@
-Metadata-Version: 2.1
-Name: slurminade
-Version: 0.6.1
-Summary: A decorator-based slurm runner
-Home-page: https://github.com/d-krupke/slurminade
-Author: Dominik Krupke
-Author-email: krupke@ibr.cs.tu-bs.de
-License: MIT
-Keywords: slurm
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# slurminade
-
-*slurminade* makes using the workload manager [slurm](https://slurm.schedmd.com/documentation.html) with Python beautiful.
-It is based on [simple_slurm](https://github.com/amq92/simple_slurm), but instead of just allowing to comfortably execute shell commands in slurm, it allows to directly distribute Python-functions.
-A function decorated with `@slurminade.slurmify(partition="alg")` will automatically be executed by a node of the partition `alg` by just calling `.distribute(yes_also_args_are_allowed)`.
-The general idea is that the corresponding Python-code exists on both machines, thus, the slurm-node can also call the functions of the original code if you tell if which one and what arguments to use.
-This is similar to [celery](https://github.com/celery/celery) but you do not need to install anything, just make sure the same Python-environment is available the nodes (usually the case in a proper slurm setup).
+slurminade - A decorator-based slurm runner for Python-code.
+============================================================
 
-Please check the documentation of [simple_slurm](https://github.com/amq92/simple_slurm) to get to know more about the
-possible parameters. You can also call simple_slurm directly by `srun` and `sbatch` (automatically with the 
+|PyPI version| |CI status| |License|
+
+*slurminade* makes using the workload manager
+`slurm <https://slurm.schedmd.com/documentation.html>`__ with Python
+beautiful. It is based on
+`simple_slurm <https://github.com/amq92/simple_slurm>`__, but instead of
+just allowing to comfortably execute shell commands in slurm, it allows
+to directly distribute Python-functions. A function decorated with
+``@slurminade.slurmify(partition="alg")`` will automatically be executed
+by a node of the partition ``alg`` by just calling
+``.distribute(yes_also_args_are_allowed)``. The general idea is that the
+corresponding Python-code exists on both machines, thus, the slurm-node
+can also call the functions of the original code if you tell if which
+one and what arguments to use. This is similar to
+`celery <https://github.com/celery/celery>`__ but you do not need to
+install anything, just make sure the same Python-environment is
+available on the nodes (usually the case in a proper slurm setup).
+
+Please check the documentation of
+`simple_slurm <https://github.com/amq92/simple_slurm>`__ to get to know
+more about the possible parameters. You can also call simple_slurm
+directly by ``srun`` and ``sbatch`` (automatically with the
 configuration specified with slurminade).
 
 *slurminade* has two design goals:
-1. Pythonic slurm: Allowing to use slurm in a Pythonic-way, without any shell commands etc.
-2. Compatibility: Scripts can also run without slurm. You can share a script and also people without slurm can execute it without any changes.
+
+1. Pythonic slurm: Allowing to use slurm in a Pythonic-way, without any
+   shell commands etc.
+2. Compatibility: Scripts can also run without slurm. You can share a
+   script and also people without slurm can execute it without any
+   changes.
+
+We use it to empirically evaluate optimization algorithms for research
+papers on hundreds of instances that can require 15min each to solve.
+With slurminade, we can distribute the workload by just changing a few
+lines of code in our local Python scripts (those that you use for
+probing and development before running big experiments). An example of
+such a usage can be found here: `Example of an empirical algorithm
+performance study for graph coloring heuristics using slurminade and
+AlgBench <https://github.com/d-krupke/AlgBench/tree/main/examples/graph_coloring>`__.
+You will find the `original
+runner <https://github.com/d-krupke/AlgBench/blob/main/examples/graph_coloring/02_run_benchmark.py>`__
+and the `slurmified
+runner <https://github.com/d-krupke/AlgBench/blob/main/examples/graph_coloring/02b_run_benchmark_with_slurminade.py>`__,
+showing the simplicity of distributing your experiments with slurminade.
 
 A simple script could look like this:
-```python
-import slurminade
 
-slurminade.update_default_configuration(partition="alg")  # global options for slurm
+.. code:: python
 
-# If no slurm environment is found, the functions are called directly to make scripts
-# compatible with any environment.
-# You can enforce slurm with `slurminade.set_dispatcher(slurminade.SlurmDispatcher())`
+   import slurminade
 
-# use this decorator to make a function distributable with slurm
-@slurminade.slurmify(constraint="alggen02")  # function specific options can be specified
-def prepare():
-    print("Prepare")
+   slurminade.update_default_configuration(partition="alg")  # global options for slurm
 
-@slurminade.slurmify()
-def f(foobar):
-    print(f"f({foobar})")
+   # If no slurm environment is found, the functions are called directly to make scripts
+   # compatible with any environment.
+   # You can enforce slurm with `slurminade.set_dispatcher(slurminade.SlurmDispatcher())`
+
+
+   # use this decorator to make a function distributable with slurm
+   @slurminade.slurmify(
+       constraint="alggen02"
+   )  # function specific options can be specified
+   def prepare():
+       print("Prepare")
+
+
+   @slurminade.slurmify()
+   def f(foobar):
+       print(f"f({foobar})")
+
+
+   @slurminade.slurmify()
+   def clean_up():
+       print("Clean up")
+
+
+   if __name__ == "__main__":
+       jid = prepare.distribute()
+
+       with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
+           # run 100x f after `prepare` has finished
+           for i in range(100):
+               f.wait_for(jid).distribute(i)  # no job id while in batch!
+
+           # clean up after the previous jobs have finished
+           jids = batch.flush()  # flush returns a list with all job ids.
+           clean_up.wait_for(jids).distribute()
+
+If slurm is not available, ``distribute`` results in a local function
+call. Analogous for ``srun`` and ``sbatch`` (giving some extra value on
+top of just forwarding to *simple_slurm*).
+
+.. warning::
+   Always use ``Batch`` when distributing many tasks. Slurm
+   jobs have a certain overhead and you do not want to spam your
+   infrastructure with too many jobs.
+
+**What are the limitations of slurminade?** Slurminade reconstructs the
+environment by basically loading the code on the slurm node (without the
+``__main__``-part) and then calling the slurmified function with
+parameters serialized as JSONSs. This means that the code must be
+written in a common ``.py``-file and all (distributed) function
+arguments must be JSON-serializable. Also, the function must not use any
+global state (e.g., global variables, file or database connections)
+initialized in the ``__main__``-part. Additionally, the
+Python-environment must be available under the same path on the slurm
+node as slurminade will use the same paths on the slurm node to
+reconstruct the environment (allowing to use virtual environments).
+
+**Does slurminade work with Python 2?** No, it is a Python 3 project. We
+tested it with Python 3.7 and higher.
+
+**Does slurminade work with Windows?** Probably not, but I never saw a
+slurm cluster running on Windows. The (automatic) slurm-less mode should
+work on Windows. So your code will run, but all function calls will be
+local.
+
+**Are multi-file projects supported?** Yes, as long as the files are
+available on the slurm node.
+
+**Does slurminade work with virtual environments?** Yes. We recommend to
+use *slurminade* with `conda <https://docs.conda.io/en/latest/>`__. We
+have not tested it with other virtual environments.
+
+**Can I run my slurmified code outside a slurm environment?** Yes, if
+you do not have slurm, the distributed functions are run as normal
+Python function calls. This means that you can share the same code with
+people that do not have slurm. It was important to us that the
+experimental evaluations we run on our slurm cluster can also be run in
+a common Python environment by reviewers without any changes.
+
+**Can I receive the return value of a slurmified function?** No, the
+return value is not transmitted back to the caller. Note that the
+distribute-calls are non-blocking, i.e., the function returns
+immediately. Return values could be implemented via a *Promise*-object
+like for other distributed computing frameworks, but we did not see the
+need for it yet. We are usually saving the results in a database or
+files, e.g., using `AlgBench <https://github.com/d-krupke/AlgBench>`__.
+
+**Can I use command line arguments ``sys.argv`` in my scripts?** Yes,
+but only in your ``__main__``-part. The arguments are not transmitted to
+the slurm nodes as they are not part of the function call. You can add
+these as normal function arguments to your slurmified functions if
+needed. It is important that your global objects to not rely on these
+arguments for initialization, as the ``__main__``-part is not executed
+on the slurm node. It is theoretically possible to transmit the
+arguments to the slurm node, but we did not see the need for it. Let us
+know if you need it and we may implement it.
+
+The code is super simple and open source, don’t be afraid to create a
+fork that fits your own needs.
+
+.. note::
+   Talk with you system administrator or supervisor to get the
+   proper slurm configuration.
+
+Installation
+------------
+
+You can install *slurminade* with ``pip install slurminade``.
+
+Usage
+-----
+
+You can set task specific slurm arguments within the decorator, e.g.,
+``@slurminade.slurmify(constraint="alggen03")``. These arguments are
+directly passed to *simple_slurm*, such that all its arguments are
+supported.
+
+In order for *slurminade* to work, the code needs to be in a Python
+file/project shared by all slurm-nodes. Otherwise, *slurminade* will not
+find the corresponding function. The slurmified functions also must be
+importable, i.e., on the top level. Currently, all function names must
+be unique as *slurminade* will only transmit the function’s name.
+
+Don’t do:
+---------
+
+Bad: Non blocking system calls
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import slurminade
+   import os
+   import subprocess
+
+
+   @slurminade.slurmify()
+   def run_shell_command():
+       # non-blocking system call
+       subprocess.Popen("complex call")
+       # BAD! The system call will run outside of slurm! The slurm task directly terminates.
 
-@slurminade.slurmify()
-def clean_up():
-    print("Clean up")
+instead use
 
+.. code:: python
 
-if __name__ == "__main__":
-    jid = prepare.distribute()
+   import slurminade
 
-    with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
-        # run 100x f after `prepare` has finished
-        for i in range(100):
-            f.wait_for(jid).distribute(i)  # no job id while in batch!
+   if __name__ == "__main__":
+       slurminade.sbatch(
+           "complex call"
+       )  # forwards your call to simple_slurm that is better used for such things.
 
-        # clean up after the previous jobs have finished
-        jids = batch.flush()  # flush returns a list with all job ids.
-        clean_up.wait_for(jids).distribute()
-```
+Bad: Global variables in the ``__main__`` part
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-> :warning: Always use `Batch` when distributing many tasks. Otherwise, you DDoS your slurm.
+.. code:: python
 
-We recommend to use *slurminade* with [conda](https://docs.conda.io/en/latest/).
-We have not tested it with other virtual environments.
+   import slurminade
 
-The code is super simple and open source, don't be afraid to create a fork that fits your own needs.
+   FLAG = True
 
-If slurm is not available, `distribute` results in a local function call.
-Analogous for `srun` and `sbatch` (giving some extra value on top of just forwarding to
-*simple_slurm*).
 
-> :warning: Talk with you system administrator or supervisor to get the proper slurm configuration.
+   @slurminade.slurmify()
+   def bad_global(args):
+       if FLAG:  # BAD! Will be True because the __main__ Part is not executed on the node.
+           pass
+       else:
+           pass
 
-## Installation
 
-You can install *slurminade* with `pip install slurminade`.
+   if __name__ == "__main__":
+       FLAG = False
+       bad_global.distribute("args")
 
-## Usage
+instead do
 
-You can set task specific slurm arguments within the decorator, e.g., `@slurminade.slurmify(constraint="alggen03")`.
-These arguments are directly passed to *simple_slurm*, such that all its arguments are supported.
+.. code:: python
 
-In order for *slurminade* to work, the code needs to be in a Python file/project shared by all slurm-nodes.
-Otherwise, *slurminade* will not find the corresponding function.
-The slurmified functions also must be importable, i.e., on the top level.
-Currently, all function names must be unique as *slurminade* will only transmit the function's name.
+   import slurminade
 
-## Don't do:
 
-### Bad: System calls
-```python
-import slurminade
-import os
-@slurminade.slurmify()
-def run_shell_command():
-    os.system("complex call")
-    # BAD! The system call will run outside of slurm! The slurm task directly terminates.
-```
-instead use
-```python
-import slurminade
+   @slurminade.slurmify()
+   def bad_global(
+       args, FLAG
+   ):  # Now the flag is passed correctly as an argument. Note that only json-compatible arguments are possible.
+       if FLAG:
+           pass
+       else:
+           pass
+
+
+   # Without the `if`, the node would also execute this part (*slurminade* will abort automatically)
+   if __name__ == "__main__":
+       FLAG = False
+       bad_global.distribute("args", FLAG)
+
+..
+
+.. warning::
+   The same is true for any global state such as file or
+   database connections. You can use global variables, but be wary of
+   side effects.
+
+Error: Complex objects as arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   import slurminade
+
+
+   @slurminade.slurmify()
+   def sec_order_func(func):
+       func()
+
+
+   def f():
+       print("hello")
 
-if __name__=="__main__":
-    slurminade.sbatch("complex call")  # forwards your call to simple_slurm that is better used for such things.
-```
-
-### Bad: Global variables
-
-```python
-import slurminade
-
-FLAG = True
-
-@slurminade.slurmify()
-def bad_global(args):
-    if FLAG:  # BAD! Will be True because the __main__ Part is not executed on the node.
-        pass
-    else:
-        pass
-
-if __name__ == "__main__":
-    FLAG = False
-    bad_global.distribute("args")
-```
-instead do
-```python
-import slurminade
-@slurminade.slurmify()
-def bad_global(args, FLAG):  # Now the flag is passed correctly as an argument. Note that only json-compatible arguments are possible.
-    if FLAG: 
-        pass
-    else:
-        pass
-
-# Without the `if`, the node would also execute this part (*slurminade* will abort automatically)
-if __name__ == "__main__":
-    FLAG = False
-    bad_global.distribute("args", FLAG)
-```
-> :warning The same is true for any global state such as file or database connections.
-
-### Error: Complex objects as arguments
-
-```python
-import slurminade
-
-@slurminade.slurmify()
-def sec_order_func(func):  
-    func()  
-    
-def f():
-    print("hello")
-    
-def g():
-    print("world!")
-    
-if __name__=="__main__":
-    sec_order_func.distribute(f)  # will throw an exception 
-    sec_order_func.distribute(g)
-```
-Instead, create individual slurmified functions for each call or pass a simple identifier that lets the function
-deduce, what to do, e.g., a switch-case.
-If you really need to pass complex objects, you could also pickle the object and only pass the file name.
-
-## Default configuration
-
-You can set up a default configuration in `~/.slurminade_default.json`.
-This should simply be a dictionary of arguments for *simple_slurm*.
-For example
-```json
-{
-  "partition": "alg"
-}
-```
 
-## Debugging
+   def g():
+       print("world!")
+
+
+   if __name__ == "__main__":
+       sec_order_func.distribute(f)  # will throw an exception
+       sec_order_func.distribute(g)
+
+Instead, create individual slurmified functions for each call or pass a
+simple identifier that lets the function deduce, what to do, e.g., a
+switch-case. If you really need to pass complex objects, you could also
+pickle the object and only pass the file name.
+
+Default configuration
+---------------------
+
+You can set up a default configuration in
+``~/.slurminade_default.json``. This should simply be a dictionary of
+arguments for *simple_slurm*. For example
+
+.. code:: json
+
+   {
+     "partition": "alg"
+   }
+
+Debugging
+---------
 
 You can use
-```python
-import slurminade
 
-slurminade.set_dispatcher(slurminade.TestDispatcher())
-```
+.. code:: python
+
+   import slurminade
+
+   slurminade.set_dispatcher(slurminade.TestDispatcher())
+
 to see the serialization or
-```python
-import slurminade
-slurminade.set_dispatcher(slurminade.SubprocessDispatcher())
-```
-to distribute the tasks without slurm using subprocesses.
 
-If there is a bug, you will directly see it in the output (at least for most bugs).
+.. code:: python
+
+   import slurminade
+
+   slurminade.set_dispatcher(slurminade.SubprocessDispatcher())
+
+to distribute the tasks without slurm using subprocesses.
 
+If there is a bug, you will directly see it in the output (at least for
+most bugs).
 
-## Project structure
+Project structure
+-----------------
 
 The project is reasonably easy:
 
-- batch.py: Contains code for bundling tasks, so we don't spam slurm with too many.
-- conf.py: Contains code for managing the configuration of slurm.
-- dispatcher.py: Contains code for actually dispatching tasks to slurm.
-- execute.py: Contains code to execute the task on the slurm node.
-- function.py: Contains the code for making a function slurm-compatible.
-- function_map.py: Saves all the slurmified functions.
-- guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
-- options.py: Contains a simple data structure to save slurm options.
-
-## Changes
-
-* 0.6.1: Bugfixes in naming
-* 0.6.0: Autmatic naming of tasks.
-* 0.5.5: Fixing bug guard bug in subprocess dispatcher.
-* 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
-* 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
-* 0.5.2: Added pyproject.toml for PEP compliance
-* 0.5.1: `Batch` will now flush on delete, in case you forgot.
-* 0.5.0:
-  * Functions now have a `wait_for`-option and return job ids. 
-  * Braking changes: Batches have a new API.
-    * `add` is no longer needed.
-    * `AutoBatch` is now called `Batch`.
-  * Fundamental code changes under the hood.
-* <0.5.0:
-  * Lots of experiments on finding the right interface.
+-  batch.py: Contains code for bundling tasks, so we don’t spam slurm
+   with too many.
+-  conf.py: Contains code for managing the configuration of slurm.
+-  dispatcher.py: Contains code for actually dispatching tasks to slurm.
+-  execute.py: Contains code to execute the task on the slurm node.
+-  function.py: Contains the code for making a function
+   slurm-compatible.
+-  function_map.py: Saves all the slurmified functions.
+-  guard.py: Contains code to prevent you accidentally DDoSing your
+   infrastructure.
+-  options.py: Contains a simple data structure to save slurm options.
+
+Changes
+-------
+
+-  0.7.0: Warning if a Batch is flushed multiple times, as we noticed this to be a common indentation error.
+-  0.6.2: Fixes recursive distribution guard, which seemed to be broken.
+-  0.6.1: Bugfixes in naming
+-  0.6.0: Autmatic naming of tasks.
+-  0.5.5: Fixing bug guard bug in subprocess dispatcher.
+-  0.5.4: Dispatched function calls that are too long for the command
+   line now use a temporary file instead.
+-  0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
+-  0.5.2: Added pyproject.toml for PEP compliance
+-  0.5.1: ``Batch`` will now flush on delete, in case you forgot.
+-  0.5.0:
+
+   -  Functions now have a ``wait_for``-option and return job ids.
+   -  Braking changes: Batches have a new API.
+
+      -  ``add`` is no longer needed.
+      -  ``AutoBatch`` is now called ``Batch``.
+
+   -  Fundamental code changes under the hood.
+
+-  <0.5.0:
+
+   -  Lots of experiments on finding the right interface.
+
+Contributores
+-------------
+
+This project is developed at the Algorithms Group at TU Braunschweig,
+Germany. The lead developer is `Dominik Krupke <https://krupke.cc>`__.
+Further contributors are Matthias Konitzny and Patrick Blumenberg.
+
+.. |PyPI version| image:: https://badge.fury.io/py/slurminade.svg
+   :target: https://badge.fury.io/py/slurminade
+.. |CI status| image:: https://github.com/d-krupke/slurminade/actions/workflows/pytest.yml/badge.svg
+   :target: https://github.com/d-krupke/slurminade
 
+.. |License| image:: https://img.shields.io/github/license/d-krupke/slurminade
+   :target: https://github.com/d-krupke/slurminade
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slurminade-0.6.1/slurminade/__init__.py` & `slurminade-0.7.1/src/slurminade/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 """
 slurminade allows to distribute function calls to slurm using decorators.
 
-```
-import slurminade
+.. code-block:: python
 
-slurminade.update_default_configuration(partition="alg")  # global options for slurm
+    import slurminade
 
-# If no slurm environment is found, the functions are called directly to make scripts
-# compatible with any environment.
-# You can enforce slurm with `slurminade.set_dispatcher(slurminade.SlurmDispatcher())`
+    slurminade.update_default_configuration(partition="alg")  # global options for slurm
 
-# use this decorator to make a function distributable with slurm
-@slurminade.slurmify(constraint="alggen02")  # function specific options can be specified
-def prepare():
-    print("Prepare")
+    # If no slurm environment is found, the functions are called directly to make scripts
+    # compatible with any environment.
+    # You can enforce slurm with `slurminade.set_dispatcher(slurminade.SlurmDispatcher())`
 
-@slurminade.slurmify()
-def f(foobar):
-    print(f"f({foobar})")
+    # use this decorator to make a function distributable with slurm
+    @slurminade.slurmify(constraint="alggen02")  # function specific options can be specified
+    def prepare():
+        print("Prepare")
 
-@slurminade.slurmify()
-def clean_up():
-    print("Clean up")
+    @slurminade.slurmify()
+    def f(foobar):
+        print(f"f({foobar})")
 
+    @slurminade.slurmify()
+    def clean_up():
+        print("Clean up")
 
-if __name__ == "__main__":
-    jid = prepare.distribute()
 
-    with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
-        # run 100x f after `prepare` has finished
-        for i in range(100):
-            f.wait_for(jid).distribute(i)
+    if __name__ == "__main__":
+        jid = prepare.distribute()
+
+        with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
+            # run 100x f after `prepare` has finished
+            for i in range(100):
+                f.wait_for(jid).distribute(i)
+
+            # clean up after the previous jobs have finished
+            jids = batch.flush()
+            clean_up.wait_for(jids).distribute()
 
-        # clean up after the previous jobs have finished
-        jids = batch.flush()
-        clean_up.wait_for(jids).distribute()
-```
 
 Project structure:
 - batch.py: Contains code for bundling tasks, so we don't spam slurm with too many.
 - conf.py: Contains code for managing the configuration of slurm.
 - dispatcher.py: Contains code for actually dispatching tasks to slurm.
 - execute.py: Contains code to execute the task on the slurm node.
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 """
 
+# flake8: noqa F401
 from .function import slurmify
 from .conf import update_default_configuration, set_default_configuration
 from .guard import set_dispatch_limit, allow_recursive_distribution
 from .batch import Batch
 from .dispatcher import (
     srun,
     sbatch,
     SlurmDispatcher,
     set_dispatcher,
     get_dispatcher,
     TestDispatcher,
     SubprocessDispatcher,
 )
 from .function_map import set_entry_point
+
+__all__ = [
+    "slurmify",
+    "update_default_configuration",
+    "set_default_configuration",
+    "set_dispatch_limit",
+    "allow_recursive_distribution",
+    "Batch",
+    "srun",
+    "sbatch",
+    "SlurmDispatcher",
+    "set_dispatcher",
+    "get_dispatcher",
+    "TestDispatcher",
+    "SubprocessDispatcher",
+]
```

### Comparing `slurminade-0.6.1/slurminade/batch.py` & `slurminade-0.7.1/src/slurminade/batch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """
 Contains code for bundling function calls together.
 """
 import typing
 from collections import defaultdict
 
-from slurminade.dispatcher import Dispatcher
-from slurminade.dispatcher import get_dispatcher, FunctionCall, set_dispatcher
-from slurminade.function import SlurmFunction
-from slurminade.options import SlurmOptions
+from .dispatcher import (
+    Dispatcher,
+    FunctionCall,
+    get_dispatcher,
+    set_dispatcher,
+)
+from .function import SlurmFunction
+from .options import SlurmOptions
+from .guard import BatchGuard
 
 
 class TaskBuffer:
     """
     A simple container to buffer all the tasks by their options.
     We can only bundle tasks with the same slurm options.
     """
+
     def __init__(self):
         self._tasks = defaultdict(list)
 
     def add(self, task: FunctionCall, options: SlurmOptions) -> int:
         self._tasks[options].append(task)
         return len(self._tasks[options])
 
@@ -34,49 +40,56 @@
         self._tasks.clear()
 
 
 class Batch(Dispatcher):
     """
     The logic to buffer the function calls. It wraps the original dispatcher.
 
-    You can use
-    ```
-    with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
-        # run 100x f
-        for i in range(100):
-            f.distribute(i)
-    ```
+    You can use::
+
+        with slurminade.Batch(max_size=20) as batch:  # automatically bundles up to 20 tasks
+            # run 100x f
+            for i in range(100):
+                f.distribute(i)
+
+    to automatically bundle up to 20 tasks and distribute them.
     """
+
     def __init__(self, max_size: int):
         """
         :param max_size: Bundle up to this many calls.
         """
         super().__init__()
         self.max_size = max_size
         self.subdispatcher = get_dispatcher()
         self._tasks = TaskBuffer()
+        self._batch_guard = BatchGuard()
 
     def flush(
         self, options: typing.Optional[SlurmOptions] = None
-    ) -> typing.Iterable[int]:
+    ) -> typing.List[int]:
         """
         Distribute all buffered tasks. Return the job ids used.
+        This method is called automatically when the context is exited.
+        However, you may want to call it manually to get the job ids,
+        for example to use them for dependency management with ``wait_for``.
         :param options: Only flush tasks with specific options.
         :return: A list of job ids.
         """
         job_ids = []
         if options is None:
             for opt, tasks in self._tasks.items():
                 while tasks:
                     job_id = self.subdispatcher(tasks[: self.max_size], opt)
                     job_ids.append(job_id)
                     tasks = tasks[self.max_size :]
 
         else:
             tasks = self._tasks.get(options)
+            self._batch_guard.report_flush(len(tasks))
             while len(tasks) > self.max_size:
                 job_id = self.subdispatcher(tasks[: self.max_size], options)
                 job_ids.append(job_id)
                 tasks = tasks[: self.max_size]
         self._tasks.clear()
         return job_ids
```

### Comparing `slurminade-0.6.1/slurminade/conf.py` & `slurminade-0.7.1/src/slurminade/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from pathlib import Path
 
 
 def _load_default_conf():
     default_conf_file = os.path.join(Path.home(), ".slurminade_default.json")
     try:
         if os.path.isfile(default_conf_file):
-            with open(default_conf_file, "r") as f:
+            with open(default_conf_file) as f:
                 return json.load(f)
         else:
             return {}
     except Exception as e:
         print(
-            f"slurminade could not open default configuration {default_conf_file}!\n{str(e)}"
+            f"slurminade could not open default configuration {default_conf_file}!\n{e!s}"
         )
     return {}
 
 
 __default_conf = _load_default_conf()
```

### Comparing `slurminade-0.6.1/slurminade/dispatcher.py` & `slurminade-0.7.1/src/slurminade/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import simple_slurm
 
 from .conf import _get_conf
 from .function_map import FunctionMap, get_entry_point
 from .guard import dispatch_guard
 from .options import SlurmOptions
 
-
 # MAX_ARG_STRLEN on a Linux system with PAGE_SIZE 4096 is 131072
 DEFAULT_MAX_ARG_LENGTH = 100000
 
 
 class FunctionCall:
     """
     A function call to be dispatched.
@@ -58,15 +57,14 @@
     ) -> int:
         """
         Define how to dispatch a number of function calls.
         :param funcs: The function calls to be dispatched.
         :param options: The slurm options to be used.
         :return: The job id. Use -1 if not applicable (e.g., because buffered)
         """
-        pass
 
     @abc.abstractmethod
     def srun(
         self,
         command: str,
         conf: typing.Optional[SlurmOptions] = None,
         simple_slurm_kwargs: dict = None,
@@ -75,15 +73,14 @@
         Define how you want to execute an `srun` command. This command is directly
         executed and only terminates after completion.
         :param command: A system command, e.g. `echo hello world > foobar.txt`.
         :param conf: The slurm configuration.
         :param simple_slurm_kwargs: Additional options for simple_slurm.
         :return: Job id
         """
-        pass
 
     @abc.abstractmethod
     def sbatch(
         self,
         command: str,
         conf: typing.Optional[SlurmOptions] = None,
         simple_slurm_kwargs: dict = None,
@@ -92,15 +89,14 @@
         Define how you want to execute an `sbatch` command. The command is scheduled
         and the function return immediately.
         :param command: A system command, e.g. `echo hello world > foobar.txt`.
         :param conf: The slurm configuration.
         :param simple_slurm_kwargs: Additional options for simple_slurm.
         :return: Job id.
         """
-        pass
 
     def __call__(
         self,
         funcs: typing.Union[FunctionCall, typing.Iterable[FunctionCall]],
         options: SlurmOptions,
     ) -> int:
         """
@@ -114,15 +110,15 @@
         return self._dispatch(funcs, options)
 
     def is_sequential(self):
         """
         Return true if the dispatcher works sequential. In this case, the dependencies
         are trivially fulfilled. Slurm does not work sequentially, because this
         would destroy its purpose. In some cases however, you do not want to use
-        slurm for compatibility reasons, without chaning the script. In these cases,
+        slurm for compatibility reasons, without changing the script. In these cases,
         this function tells slurminade not to be too strict about dependencies.
         :return: True is tasks are executed sequentially, false if not.
         """
         return False
 
 
 class TestDispatcher(Dispatcher):
@@ -174,29 +170,29 @@
     """
     The most important dispatcher: Distributing function calls to slurm.
     """
 
     def __init__(self):
         super().__init__()
         if not shutil.which("sbatch"):
-            raise RuntimeError("Slurm could not be found.")
+            msg = "Slurm could not be found."
+            raise RuntimeError(msg)
         self.max_arg_length = DEFAULT_MAX_ARG_LENGTH
 
     def _create_slurm_api(self, special_slurm_opts):
         conf = _get_conf(special_slurm_opts)
         slurm = simple_slurm.Slurm(**conf)
         return slurm
-    
+
     def _job_name(self, funcs: typing.List[FunctionCall]) -> str:
-        func_names = list(set(FunctionMap.get_readable_name(f.func_id) for f in funcs))
+        func_names = list({FunctionMap.get_readable_name(f.func_id) for f in funcs})
         if len(funcs) == 1:
             return f"slurminade:{func_names[0]}"
         else:
             return f"slurminade[batch]:{func_names[0]}..."
-        
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
         dispatch_guard()
         if "job_name" not in options:
             funcs = list(funcs)
@@ -228,14 +224,15 @@
     """
     A dispatcher for debugging that distributes function calls using subprocesses.
     Thus, it uses the same serialization mechanisms, but without a slurm dependency.
     Completely useless for productive purposes. Use `DirectCallDispatcher` if you
     don't want to use slurm.
     Despite using subprocesses, it does not parallelize but works sequential.
     """
+
     def __init__(self):
         super().__init__()
         self.max_arg_length = DEFAULT_MAX_ARG_LENGTH
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
@@ -277,15 +274,17 @@
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
         self.srun(command)
 
     def is_sequential(self):
         return True
 
 
-def create_slurminade_command(funcs: typing.Iterable[FunctionCall], max_arg_length: int) -> str:
+def create_slurminade_command(
+    funcs: typing.Iterable[FunctionCall], max_arg_length: int
+) -> str:
     """
     Creates a terminal command that calls the Python module `slurminade.execute` with the
     provided function calls as an argument. If the total length of the function calls
     exceeds the maximum allowed length of a command line argument, a temporary file is
     created to pass the function calls instead.
     :param funcs: The function calls to be dispatched.
     :param max_arg_length: The maximum allowed length of a command line argument.
@@ -295,15 +294,15 @@
 
     # Serialize function calls as JSON
     serialized_calls = json.dumps([f.to_json() for f in funcs])
 
     if len(shlex.quote(serialized_calls)) > max_arg_length:
         # The argument is too long, create temporary file for the JSON
         fd, filename = mkstemp(prefix="slurminade_", suffix=".json", text=True, dir=".")
-        with os.fdopen(fd, 'w') as f:
+        with os.fdopen(fd, "w") as f:
             f.write(serialized_calls)
         command += f" temp {shlex.quote(filename)}"
     else:
         command += f" arg {shlex.quote(serialized_calls)}"
     return command
```

### Comparing `slurminade-0.6.1/slurminade/execute.py` & `slurminade-0.7.1/src/slurminade/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """
 This module provides the starting point for the slurm node. You do not have to call
 anything of this file yourself.
 """
+import json
 import os
+import sys
 
-from .guard import prevent_distribution
 from .function import SlurmFunction
 from .function_map import set_entry_point
-import json
-import sys
+from .guard import prevent_distribution
 
 
 def parse_args():
     batch_file_path = sys.argv[1]  # the file with the code (function definition)
     # determine whether function calls are provided as an argument or in a temp file.
     mode = sys.argv[2]
     if mode == "arg":
         function_calls = json.loads(sys.argv[3])
     elif mode == "temp":
         with open(sys.argv[3]) as f:
             function_calls = json.load(f)
         os.remove(sys.argv[3])  # delete the temp file
     else:
-        raise ValueError("Unknown function call mode. Expected 'arg' or 'temp'.")
+        msg = "Unknown function call mode. Expected 'arg' or 'temp'."
+        raise ValueError(msg)
     assert isinstance(function_calls, list), "Expected a list of dicts"
     return batch_file_path, function_calls
 
 
 def main():
     prevent_distribution()  # make sure, the code on the node does not distribute itself.
     batch_file, function_calls = parse_args()
 
     set_entry_point(batch_file)
-    with open(batch_file, "r") as f:
+    with open(batch_file) as f:
         code = "".join(f.readlines())
 
     # Workaround as otherwise __name__ is not defined
     global __name__
     __name__ = None
 
     glob = dict(globals())
```

### Comparing `slurminade-0.6.1/slurminade/function.py` & `slurminade-0.7.1/src/slurminade/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 from .guard import guard_recursive_distribution
 from .options import SlurmOptions
 
 
 class SlurmFunction:
     """
     A wrapper around a function that allows it to be distributed to slurm.
-    ```
-    @slurmify(...function specific slurm options...)
-    def f(foobar):
-        print(foobar)
-
-    if __name__=="__main__":
-        assert isinstance(f, SlurmFunction), "f has become a SlurmFunction"
-        jid = f.distribute("hello")
-        f.wait_for(jid).distribute("bye")
-    ```
+
+    .. code-block:: python
+
+        @slurmify(function specific slurm options)
+        def f(foobar):
+            print(foobar)
+
+        if __name__=="__main__":
+            assert isinstance(f, SlurmFunction), "f has become a SlurmFunction"
+            jid = f.distribute("hello")
+            f.wait_for(jid).distribute("bye")
+
     """
 
     def __init__(
         self, special_slurm_opts: typing.Dict, func: typing.Callable, func_id: str
     ):
         self.special_slurm_opts = SlurmOptions(**special_slurm_opts)
         self.func = func
@@ -44,15 +46,16 @@
                     )
                 else:
                     dependecy_dict[method] = ":".join(str(jid) for jid in job_ids)
             elif isinstance(self.special_slurm_opts["dependency"], str):
                 self.special_slurm_opts["dependency"] += "," + opt
             else:
                 # Could not extend dependencies because I have no idea what is going on.
-                raise RuntimeError("Key 'dependency' has unexpected type.")
+                msg = "Key 'dependency' has unexpected type."
+                raise RuntimeError(msg)
         else:
             self.special_slurm_opts["dependency"] = opt
 
     def wait_for(
         self, job_ids: typing.Union[int, typing.Iterable[int]], method: str = "afterany"
     ) -> "SlurmFunction":
         """
@@ -68,19 +71,16 @@
         :param method: 'after'|'afterany'|'afternotok'|'afterok'|'singleton'
         :return: Chainable slurm function object.
         """
         sfunc = SlurmFunction(self.special_slurm_opts, self.func, self.func_id)
         if isinstance(job_ids, int):
             job_ids = [job_ids]
         if any(jid < 0 for jid in job_ids) and not get_dispatcher().is_sequential():
-            raise RuntimeError(
-                "Invalid job id. Not every dispatcher can directly return"
-                " job ids, because it may not directly distribute them or"
-                " doesn't distribute them at all."
-            )
+            msg = "Invalid job id. Not every dispatcher can directly return job ids, because it may not directly distribute them or doesn't distribute them at all."
+            raise RuntimeError(msg)
         sfunc._add_dependencies(list(job_ids), method)
         return sfunc
 
     def _check(self, args, kwargs):
         """
         Check if the arguments match the function signature.
         """
@@ -104,32 +104,34 @@
         :return: Job id. Not necessarily valid (usually -1 in this case).
         """
         self._check(args, kwargs)
         guard_recursive_distribution()
         return dispatch(
             [FunctionCall(self.func_id, args, kwargs)], self.special_slurm_opts
         )
-    
+
     def __str__(self) -> str:
         return self.func.__name__
 
     @staticmethod
     def call(func_id, *args, **kwargs):
         return FunctionMap.call(func_id, args, kwargs)
 
 
 def slurmify(f=None, **args) -> typing.Callable[[typing.Callable], SlurmFunction]:
     """
     Decorator: Make a function distributable to slurm.
     Usage:
-    ```
-    @slurmify()
-    def func(a, b):
-        pass
-    ```
+
+    .. code-block:: python
+
+        @slurmify()
+        def func(a, b):
+            pass
+
     :param f: Function
     :param args: Special slurm options for this function.
     :return: A decorated function, callable with slurm.
     """
 
     if f:  # use default parameters
         func_id = FunctionMap.register(f)
```

### Comparing `slurminade-0.6.1/slurminade/function_map.py` & `slurminade-0.7.1/src/slurminade/function_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The internal datastructure to save all the slurmified functions.
 Not relevant for endusers.
 """
 
 import inspect
-import typing
 import os
+import typing
 
 
 class FunctionMap:
     """
     The function map assigns functions an id and stores them to be called later.
     This id is reproducible such that the slurm node can retrieve the function
     it is supposed to call just by the id.
@@ -31,49 +31,51 @@
         :param func: The function you want the id of.
         :return: The id as string.
         """
         file = inspect.getfile(func)
         if file == "<string>":  # on the slurm node, the functions in the entry point
             # are named `<string>`.
             if not FunctionMap.entry_point:
-                raise RuntimeError("No entry point known.")
+                msg = "No entry point known."
+                raise RuntimeError(msg)
             file = FunctionMap.entry_point
         path = os.path.normpath(os.path.abspath(file))
         return f"{path}:{func.__name__}"
-    
+
     @staticmethod
     def get_readable_name(func_id: str) -> str:
         return func_id.split(":")[-1]
 
-
     @staticmethod
     def check_compatibility(func: typing.Callable):
         """
         Throw if the function cannot be assigned an id.
         :param func: The function to be checked.
         :return: None
         """
         if (
             not func.__name__
             or func.__name__ == "<lambda>"
             or not inspect.getfile(func)
         ):
-            raise ValueError("Can only slurmify proper functions.")
+            msg = "Can only slurmify proper functions."
+            raise ValueError(msg)
 
     @staticmethod
     def register(func: typing.Callable) -> str:
         """
         Register a function, allowing it to be called just by its id.
         :param func: The function to be stored. Needs to be a proper function.
         :return: The function's id.
         """
         FunctionMap.check_compatibility(func)
         func_id = FunctionMap.get_id(func)
         if func_id in FunctionMap._data:
-            raise RuntimeError("Multiple function definitions!")
+            msg = "Multiple function definitions!"
+            raise RuntimeError(msg)
         FunctionMap._data[func_id] = func
         return func_id
 
     @staticmethod
     def call(
         func_id: str, args: typing.Iterable, kwargs: typing.Dict[str, typing.Any]
     ) -> typing.Any:
@@ -81,32 +83,36 @@
         Calls a function by its id.
         :param func_id: The id of the function to be called.
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
         :return: The return value of the function.
         """
         if func_id not in FunctionMap._data:
-            raise KeyError(f"Function '{func_id}' unknown!")
+            msg = f"Function '{func_id}' unknown!"
+            raise KeyError(msg)
         return FunctionMap._data[func_id](*args, **kwargs)
 
 
 def set_entry_point(entry_point: str) -> None:
     """
     This function usually is not necessary for endusers.
     Set a manual entry point. This can allow you to use slurmify from the interactive
     interpreter.
     :param entry_point: A path to the entry point file.
     :return: None
     """
     if not os.path.isfile(entry_point) or not entry_point.endswith(".py"):
-        raise ValueError(f"Illegal entry point ({entry_point}).")
+        msg = f"Illegal entry point ({entry_point})."
+        raise ValueError(msg)
     entry_point = os.path.abspath(entry_point)
     FunctionMap.entry_point = entry_point
     # SlurmFunction.dispatcher.entry_point = entry_point
 
+
 def get_entry_point() -> str:
     if FunctionMap.entry_point is None:
         import __main__
+
         entry_point = __main__.__file__
 
         set_entry_point(entry_point)
-    return FunctionMap.entry_point
+    return FunctionMap.entry_point
```

### Comparing `slurminade-0.6.1/slurminade/options.py` & `slurminade-0.7.1/src/slurminade/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import typing
-
-
 class SlurmOptions(dict):
     """
     Primarily just a wrapper to allow using the options in a dict as key.
     Necessary for batching function calls, because only function calls with the
     same options can be bundled.
     """
```

