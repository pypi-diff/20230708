# Comparing `tmp/hypofuzz-23.6.1.tar.gz` & `tmp/hypofuzz-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-23.6.1.tar", last modified: Sat Jun  3 19:00:44 2023, max compression
+gzip compressed data, was "hypofuzz-23.7.1.tar", last modified: Sat Jul  8 08:49:51 2023, max compression
```

## Comparing `hypofuzz-23.6.1.tar` & `hypofuzz-23.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.003682 hypofuzz-23.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.011682 hypofuzz-23.6.1/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/patching.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.011682 hypofuzz-23.6.1/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 19:00:43.000000 hypofuzz-23.6.1/src/hypofuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:00:44.015682 hypofuzz-23.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_coverage_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_fuzz_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-03 19:00:31.000000 hypofuzz-23.6.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:51.584134 hypofuzz-23.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-08 08:49:51.584134 hypofuzz-23.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:49:51.584134 hypofuzz-23.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:51.580134 hypofuzz-23.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:51.580134 hypofuzz-23.7.1/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16737 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:51.580134 hypofuzz-23.7.1/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 08:49:51.000000 hypofuzz-23.7.1/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:49:51.584134 hypofuzz-23.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-08 08:49:42.000000 hypofuzz-23.7.1/tests/test_version.py
```

### Comparing `hypofuzz-23.6.1/LICENSE` & `hypofuzz-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/PKG-INFO` & `hypofuzz-23.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.6.1
+Version: 23.7.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.6.1/README.md` & `hypofuzz-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/setup.py` & `hypofuzz-23.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/src/hypofuzz/corpus.py` & `hypofuzz-23.7.1/src/hypofuzz/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             if origin not in self.interesting_examples or (
                 sort_key(result) < sort_key(self.interesting_examples[origin][0])
             ):
                 self._database.save(self._key, result.buffer)
                 self.interesting_examples[origin] = (
                     result,
                     [
-                        result.extra_information.call_repr,
+                        getattr(result.extra_information, "call_repr", "<unknown>"),
                         result.extra_information.reports,
                         reproduction_decorator(result.buffer),
                         result.extra_information.traceback,
                     ],
                 )
                 return True
```

### Comparing `hypofuzz-23.6.1/src/hypofuzz/cov.py` & `hypofuzz-23.7.1/src/hypofuzz/cov.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/src/hypofuzz/dashboard.py` & `hypofuzz-23.7.1/src/hypofuzz/dashboard.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/src/hypofuzz/debugger.py` & `hypofuzz-23.7.1/src/hypofuzz/debugger.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/src/hypofuzz/entrypoint.py` & `hypofuzz-23.7.1/src/hypofuzz/entrypoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,109 @@
-"""CLI and Python API for the fuzzer."""
-
-import sys
-from multiprocessing import Process
-from typing import NoReturn, Tuple
-
-import click
-import hypothesis.extra.cli
-import psutil
-
-
-@hypothesis.extra.cli.main.command()  # type: ignore
-@click.option(
-    "-n",
-    "--numprocesses",
-    type=click.IntRange(1, None),
-    metavar="NUM",
-    # we match the -n auto behaviour of pytest-xdist by default
-    default=psutil.cpu_count(logical=False) or psutil.cpu_count() or 1,
-    help="default: all available cores",
-)
-@click.option(
-    "--dashboard/--no-dashboard",
-    default=True,
-    help="serve / don't serve a live dashboard page",
-)
-@click.option(
-    "--port",
-    type=click.IntRange(1, 65535),
-    default=9999,
-    metavar="PORT",
-    help="Optional port for the dashboard (if any)",
-)
-@click.option(
-    "--unsafe",
-    is_flag=True,
-    help="Allow concurrent execution of each test (dashboard may report wrong results)",
-)
-@click.argument(
-    "pytest_args",
-    nargs=-1,
-    metavar="[-- PYTEST_ARGS]",
-)
-def fuzz(
-    numprocesses: int,
-    dashboard: bool,
-    port: int,
-    unsafe: bool,
-    pytest_args: Tuple[str, ...],
-) -> NoReturn:
-    """[hypofuzz] runs tests with an adaptive coverage-guided fuzzer.
-
-    Unrecognised arguments are passed through to `pytest` to select the tests
-    to run, with the additional constraint that only tests using Hypothesis
-    but not any pytest fixtures can be fuzzed.
-
-    This process will run forever unless stopped with e.g. ctrl-C.
-    """
-    # Before doing anything with our arguments, we'll check that none
-    # of HypoFuzz's arguments will be passed on to pytest instead.
-    misplaced: set = set(pytest_args) & set().union(*(p.opts for p in fuzz.params))
-    if misplaced:
-        plural = "s" * (len(misplaced) > 1)
-        names = ", ".join(map(repr, misplaced))
-        raise click.UsageError(
-            f"fuzzer option{plural} {names} would be passed to pytest instead"
-        )
-
-    from .interface import _fuzz_several, _get_hypothesis_tests_with_pytest
-
-    # With our arguments validated, it's time to actually do the work.
-    tests = _get_hypothesis_tests_with_pytest(pytest_args)
-    if not tests:
-        raise click.UsageError("No property-based tests were collected")
-    if numprocesses > len(tests) and not unsafe:
-        numprocesses = len(tests)
-
-    testnames = "\n    ".join(t.nodeid for t in tests)
-    print(f"using up to {numprocesses} processes to fuzz:\n    {testnames}\n")  # noqa
-
-    if dashboard:
-        from .dashboard import start_dashboard_process
-
-        Process(
-            target=start_dashboard_process,
-            kwargs={"port": port, "pytest_args": pytest_args},
-        ).start()
-
-    processes = []
-    for i in range(numprocesses):
-        nodes = {t.nodeid for t in (tests if unsafe else tests[i::numprocesses])}
-        p = Process(
-            target=_fuzz_several,
-            kwargs={"pytest_args": pytest_args, "nodeids": nodes, "port": port},
-        )
-        p.start()
-        processes.append(p)
-    for p in processes:
-        p.join()
-    print("Found a failing input for every test!", file=sys.stderr)  # noqa: T201
-    sys.exit(1)
-    raise NotImplementedError("unreachable")
+"""CLI and Python API for the fuzzer."""
+
+import sys
+from multiprocessing import Process
+from typing import NoReturn, Optional, Tuple
+
+import click
+import hypothesis.extra.cli
+import psutil
+
+
+@hypothesis.extra.cli.main.command()  # type: ignore
+@click.option(
+    "-n",
+    "--numprocesses",
+    type=click.IntRange(1, None),
+    metavar="NUM",
+    # we match the -n auto behaviour of pytest-xdist by default
+    default=psutil.cpu_count(logical=False) or psutil.cpu_count() or 1,
+    help="default: all available cores",
+)
+@click.option(
+    "--dashboard/--no-dashboard",
+    default=True,
+    help="serve / don't serve a live dashboard page",
+)
+@click.option(
+    "--port",
+    type=click.IntRange(1, 65535),
+    default=9999,
+    metavar="PORT",
+    help="Optional port for the dashboard (if any)",
+)
+@click.option(
+    "--unsafe",
+    is_flag=True,
+    help="Allow concurrent execution of each test (dashboard may report wrong results)",
+)
+@click.argument(
+    "pytest_args",
+    nargs=-1,
+    metavar="[-- PYTEST_ARGS]",
+)
+def fuzz(
+    numprocesses: int,
+    dashboard: bool,
+    port: Optional[int],
+    unsafe: bool,
+    pytest_args: Tuple[str, ...],
+) -> NoReturn:
+    """[hypofuzz] runs tests with an adaptive coverage-guided fuzzer.
+
+    Unrecognised arguments are passed through to `pytest` to select the tests
+    to run, with the additional constraint that only tests using Hypothesis
+    but not any pytest fixtures can be fuzzed.
+
+    This process will run forever unless stopped with e.g. ctrl-C.
+    """
+    # Before doing anything with our arguments, we'll check that none
+    # of HypoFuzz's arguments will be passed on to pytest instead.
+    misplaced: set = set(pytest_args) & set().union(*(p.opts for p in fuzz.params))
+    if misplaced:
+        plural = "s" * (len(misplaced) > 1)
+        names = ", ".join(map(repr, misplaced))
+        raise click.UsageError(
+            f"fuzzer option{plural} {names} would be passed to pytest instead"
+        )
+
+    from .interface import _fuzz_several, _get_hypothesis_tests_with_pytest
+
+    # With our arguments validated, it's time to actually do the work.
+    tests = _get_hypothesis_tests_with_pytest(pytest_args)
+    if not tests:
+        raise click.UsageError("No property-based tests were collected")
+    if numprocesses > len(tests) and not unsafe:
+        numprocesses = len(tests)
+
+    testnames = "\n    ".join(t.nodeid for t in tests)
+    print(f"using up to {numprocesses} processes to fuzz:\n    {testnames}\n")  # noqa
+
+    if dashboard:
+        from .dashboard import start_dashboard_process
+
+        Process(
+            target=start_dashboard_process,
+            kwargs={"port": port, "pytest_args": pytest_args},
+        ).start()
+    else:
+        port = None
+
+    if numprocesses <= 1:
+        _fuzz_several(
+            pytest_args=pytest_args, nodeids=[t.nodeid for t in tests], port=port
+        )
+    else:
+        processes = []
+        for i in range(numprocesses):
+            nodes = {t.nodeid for t in (tests if unsafe else tests[i::numprocesses])}
+            p = Process(
+                target=_fuzz_several,
+                kwargs={"pytest_args": pytest_args, "nodeids": nodes, "port": port},
+            )
+            p.start()
+            processes.append(p)
+        for p in processes:
+            p.join()
+    print("Found a failing input for every test!", file=sys.stderr)  # noqa: T201
+    sys.exit(1)
+    raise NotImplementedError("unreachable")
```

### Comparing `hypofuzz-23.6.1/src/hypofuzz/hy.py` & `hypofuzz-23.7.1/src/hypofuzz/hy.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,17 @@
             params=get_signature(wrapped_test).parameters,
         )
         return cls(
             test_fn=wrapped_test.hypothesis.inner_test,
             stuff=stuff,
             nodeid=nodeid,
             database_key=function_digest(wrapped_test.hypothesis.inner_test),
-            hypothesis_database=wrapped_test._hypothesis_internal_use_settings.database
+            hypothesis_database=getattr(
+                wrapped_test, "_hypothesis_internal_use_settings", settings.default
+            ).database
             or settings.default.database,
         )
 
     def __init__(
         self,
         test_fn: Callable,
         stuff: Stuff,
@@ -302,14 +304,18 @@
             data.status = Status.INTERESTING
             tb = get_trimmed_traceback()
             filename, lineno, *_ = traceback.extract_tb(tb)[-1]
             data.interesting_origin = (type(e), filename, lineno)
             data.extra_information.traceback = "".join(
                 traceback.format_exception(type(e), value=e, tb=tb)
             )
+        except KeyboardInterrupt:
+            # If you have a test function which raises KI, this is pretty useful.
+            print(f"Got a KeyboardInterrupt in {self.nodeid}, exiting...")  # noqa
+            raise
         finally:
             data.extra_information.reports = "\n".join(map(str, reports))
 
         # In addition to coverage branches, use psudeo-coverage information provided via
         # the `hypothesis.event()` function - exploiting user-defined partitions
         # designed for diagnostic output to guide generation.  See
         # https://hypothesis.readthedocs.io/en/latest/details.html#hypothesis.event
```

### Comparing `hypofuzz-23.6.1/src/hypofuzz/patching.py` & `hypofuzz-23.7.1/src/hypofuzz/patching.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.7.1/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.6.1
+Version: 23.7.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.6.1/src/hypofuzz.egg-info/SOURCES.txt` & `hypofuzz-23.7.1/src/hypofuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/tests/test_corpus.py` & `hypofuzz-23.7.1/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/tests/test_fuzz_process.py` & `hypofuzz-23.7.1/tests/test_fuzz_process.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.6.1/tests/test_version.py` & `hypofuzz-23.7.1/tests/test_version.py`

 * *Files identical despite different names*

