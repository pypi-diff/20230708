# Comparing `tmp/turnt-1.8.0.tar.gz` & `tmp/turnt-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turnt-1.8.0.tar", last modified: Tue Jun  7 11:47:47 2022, max compression
+gzip compressed data, was "turnt-1.9.0.tar", last modified: Wed Nov  2 13:19:18 2022, max compression
```

## Comparing `turnt-1.8.0.tar` & `turnt-1.9.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0      751 2022-06-02 20:17:32.000000 turnt-1.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       32 2022-06-01 13:38:09.872930 turnt-1.8.0/.gitignore
--rw-r--r--   0        0        0     1902 2022-06-07 11:47:27.513683 turnt-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2020-09-16 16:15:25.000000 turnt-1.8.0/LICENSE
--rw-r--r--   0        0        0       37 2022-06-04 11:53:43.667318 turnt-1.8.0/Makefile
--rw-r--r--   0        0        0    10098 2022-06-05 22:48:11.673972 turnt-1.8.0/README.md
--rw-r--r--   0        0        0      488 2022-06-04 00:52:06.055041 turnt-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       56 2020-06-23 23:42:49.000000 turnt-1.8.0/test/basic/args.out
--rw-r--r--   0        0        0       35 2019-06-05 15:46:34.000000 turnt-1.8.0/test/basic/args.t
--rw-r--r--   0        0        0        8 2022-06-02 20:17:32.000000 turnt-1.8.0/test/basic/bad.err
--rw-r--r--   0        0        0       63 2022-06-02 20:17:32.000000 turnt-1.8.0/test/basic/bad.t
--rw-r--r--   0        0        0       18 2019-06-05 15:46:49.000000 turnt-1.8.0/test/basic/cmd.out
--rw-r--r--   0        0        0       54 2019-06-05 15:45:52.000000 turnt-1.8.0/test/basic/cmd.t
--rw-r--r--   0        0        0        9 2019-06-05 15:56:21.000000 turnt-1.8.0/test/basic/hello.out
--rw-r--r--   0        0        0        3 2019-06-05 15:56:17.000000 turnt-1.8.0/test/basic/hello.t
--rw-r--r--   0        0        0        4 2019-06-07 02:14:48.000000 turnt-1.8.0/test/basic/multi-output.out
--rw-r--r--   0        0        0      107 2019-06-07 02:14:48.000000 turnt-1.8.0/test/basic/multi-output.t
--rw-r--r--   0        0        0        4 2019-06-07 02:14:48.000000 turnt-1.8.0/test/basic/multi-output.txt
--rw-r--r--   0        0        0      105 2020-06-30 12:56:14.000000 turnt-1.8.0/test/basic/turnt.toml
--rw-r--r--   0        0        0       21 2022-06-04 11:56:25.693593 turnt-1.8.0/test/dirtest/bar.t/opts.txt
--rw-r--r--   0        0        0       35 2022-06-04 11:56:42.499589 turnt-1.8.0/test/dirtest/bar.t/out.out
--rw-r--r--   0        0        0       16 2022-06-04 11:56:00.011030 turnt-1.8.0/test/dirtest/bar.t/test.in
--rw-r--r--   0        0        0       18 2022-06-04 11:53:09.302723 turnt-1.8.0/test/dirtest/foo.t/out.out
--rw-r--r--   0        0        0       14 2022-06-04 11:52:42.764283 turnt-1.8.0/test/dirtest/foo.t/test.in
--rw-r--r--   0        0        0       79 2022-06-04 11:55:40.893426 turnt-1.8.0/test/dirtest/turnt.toml
--rw-r--r--   0        0        0        8 2022-06-02 20:17:32.000000 turnt-1.8.0/test/errors/bad.out
--rw-r--r--   0        0        0       35 2022-06-02 20:17:32.000000 turnt-1.8.0/test/errors/bad.t
--rw-r--r--   0        0        0       34 2022-06-02 20:17:32.000000 turnt-1.8.0/test/errors/turnt.toml
--rw-r--r--   0        0        0        8 2022-06-02 20:17:32.000000 turnt-1.8.0/test/multi-output/bad.err
--rw-r--r--   0        0        0       63 2022-06-02 20:17:32.000000 turnt-1.8.0/test/multi-output/bad.t
--rw-r--r--   0        0        0        4 2019-09-24 14:26:25.000000 turnt-1.8.0/test/multi-output/multi-output.out
--rw-r--r--   0        0        0      107 2019-09-24 14:26:25.000000 turnt-1.8.0/test/multi-output/multi-output.t
--rw-r--r--   0        0        0        4 2019-09-24 14:26:25.000000 turnt-1.8.0/test/multi-output/multi-output.txt
--rw-r--r--   0        0        0        4 2022-06-05 13:45:44.291157 turnt-1.8.0/test/multi-output/other_file.txt
--rw-r--r--   0        0        0       95 2019-09-24 14:26:25.000000 turnt-1.8.0/test/multi-output/turnt.toml
--rw-r--r--   0        0        0       21 2022-06-05 22:48:11.674340 turnt-1.8.0/test/multienv/something.out
--rw-r--r--   0        0        0       22 2022-06-05 22:48:11.674552 turnt-1.8.0/test/multienv/something.out3
--rw-r--r--   0        0        0       18 2022-06-05 22:48:11.674694 turnt-1.8.0/test/multienv/something.t
--rw-r--r--   0        0        0      482 2022-06-05 22:48:11.674920 turnt-1.8.0/test/multienv/turnt.toml
--rw-r--r--   0        0        0       31 2022-06-02 20:17:32.000000 turnt-1.8.0/test/subdir/example.out
--rw-r--r--   0        0        0       14 2022-06-02 20:17:32.000000 turnt-1.8.0/test/subdir/example.t
--rw-r--r--   0        0        0      185 2022-06-02 20:17:32.000000 turnt-1.8.0/test/turnt.toml
--rw-r--r--   0        0        0      137 2022-06-04 01:03:27.855833 turnt-1.8.0/turnt/__init__.py
--rw-r--r--   0        0        0     1621 2022-06-05 22:48:34.008371 turnt-1.8.0/turnt/__main__.py
--rw-r--r--   0        0        0     9901 2022-06-05 22:48:11.675592 turnt-1.8.0/turnt/config.py
--rw-r--r--   0        0        0     5550 2022-06-05 22:48:11.675863 turnt-1.8.0/turnt/run.py
--rw-r--r--   0        0        0    10464 1970-01-01 00:00:00.000000 turnt-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2022-11-02 13:14:06.256449 turnt-1.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       32 2022-11-02 13:14:06.256519 turnt-1.9.0/.gitignore
+-rw-r--r--   0        0        0     2420 2022-11-02 13:14:32.766556 turnt-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2022-11-02 13:14:06.256695 turnt-1.9.0/LICENSE
+-rw-r--r--   0        0        0       37 2022-11-02 13:14:06.256768 turnt-1.9.0/Makefile
+-rw-r--r--   0        0        0    10369 2022-11-02 13:14:06.256879 turnt-1.9.0/README.md
+-rw-r--r--   0        0        0      488 2022-11-02 13:14:06.256955 turnt-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2022-11-02 13:14:06.257100 turnt-1.9.0/test/basic/args.out
+-rw-r--r--   0        0        0       35 2022-11-02 13:14:06.257163 turnt-1.9.0/test/basic/args.t
+-rw-r--r--   0        0        0        8 2022-11-02 13:14:06.257220 turnt-1.9.0/test/basic/bad.err
+-rw-r--r--   0        0        0       63 2022-11-02 13:14:06.257281 turnt-1.9.0/test/basic/bad.t
+-rw-r--r--   0        0        0       18 2022-11-02 13:14:06.257343 turnt-1.9.0/test/basic/cmd.out
+-rw-r--r--   0        0        0       54 2022-11-02 13:14:06.257409 turnt-1.9.0/test/basic/cmd.t
+-rw-r--r--   0        0        0        9 2022-11-02 13:14:06.257482 turnt-1.9.0/test/basic/hello.out
+-rw-r--r--   0        0        0        3 2022-11-02 13:14:06.257541 turnt-1.9.0/test/basic/hello.t
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.257609 turnt-1.9.0/test/basic/multi-output.out
+-rw-r--r--   0        0        0      107 2022-11-02 13:14:06.257697 turnt-1.9.0/test/basic/multi-output.t
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.257780 turnt-1.9.0/test/basic/multi-output.txt
+-rw-r--r--   0        0        0      105 2022-11-02 13:14:06.257856 turnt-1.9.0/test/basic/turnt.toml
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.257978 turnt-1.9.0/test/binary/bin.out
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.258061 turnt-1.9.0/test/binary/bin.t
+-rw-r--r--   0        0        0       45 2022-11-02 13:14:06.258129 turnt-1.9.0/test/binary/turnt.toml
+-rw-r--r--   0        0        0       21 2022-11-02 13:14:06.258284 turnt-1.9.0/test/dirtest/bar.t/opts.txt
+-rw-r--r--   0        0        0       35 2022-11-02 13:14:06.258343 turnt-1.9.0/test/dirtest/bar.t/out.out
+-rw-r--r--   0        0        0       16 2022-11-02 13:14:06.258401 turnt-1.9.0/test/dirtest/bar.t/test.in
+-rw-r--r--   0        0        0       18 2022-11-02 13:14:06.258507 turnt-1.9.0/test/dirtest/foo.t/out.out
+-rw-r--r--   0        0        0       14 2022-11-02 13:14:06.258609 turnt-1.9.0/test/dirtest/foo.t/test.in
+-rw-r--r--   0        0        0       79 2022-11-02 13:14:06.258694 turnt-1.9.0/test/dirtest/turnt.toml
+-rw-r--r--   0        0        0        8 2022-11-02 13:14:06.258958 turnt-1.9.0/test/errors/bad.out
+-rw-r--r--   0        0        0       35 2022-11-02 13:14:06.259022 turnt-1.9.0/test/errors/bad.t
+-rw-r--r--   0        0        0       34 2022-11-02 13:14:06.259114 turnt-1.9.0/test/errors/turnt.toml
+-rw-r--r--   0        0        0        8 2022-11-02 13:14:06.259222 turnt-1.9.0/test/multi-output/bad.err
+-rw-r--r--   0        0        0       63 2022-11-02 13:14:06.259288 turnt-1.9.0/test/multi-output/bad.t
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.259391 turnt-1.9.0/test/multi-output/multi-output.out
+-rw-r--r--   0        0        0      107 2022-11-02 13:14:06.259538 turnt-1.9.0/test/multi-output/multi-output.t
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.259658 turnt-1.9.0/test/multi-output/multi-output.txt
+-rw-r--r--   0        0        0        4 2022-11-02 13:14:06.259806 turnt-1.9.0/test/multi-output/other_file.txt
+-rw-r--r--   0        0        0       95 2022-11-02 13:14:06.259924 turnt-1.9.0/test/multi-output/turnt.toml
+-rw-r--r--   0        0        0       21 2022-11-02 13:14:06.260154 turnt-1.9.0/test/multienv/something.out
+-rw-r--r--   0        0        0       22 2022-11-02 13:14:06.260261 turnt-1.9.0/test/multienv/something.out3
+-rw-r--r--   0        0        0       18 2022-11-02 13:14:06.260328 turnt-1.9.0/test/multienv/something.t
+-rw-r--r--   0        0        0      482 2022-11-02 13:14:06.260429 turnt-1.9.0/test/multienv/turnt.toml
+-rw-r--r--   0        0        0       31 2022-11-02 13:14:06.260545 turnt-1.9.0/test/subdir/example.out
+-rw-r--r--   0        0        0       14 2022-11-02 13:14:06.260645 turnt-1.9.0/test/subdir/example.t
+-rw-r--r--   0        0        0      185 2022-11-02 13:14:06.260718 turnt-1.9.0/test/turnt.toml
+-rw-r--r--   0        0        0      137 2022-11-02 13:14:06.260856 turnt-1.9.0/turnt/__init__.py
+-rw-r--r--   0        0        0     1714 2022-11-02 13:14:06.260944 turnt-1.9.0/turnt/__main__.py
+-rw-r--r--   0        0        0    10198 2022-11-02 13:14:06.261062 turnt-1.9.0/turnt/config.py
+-rw-r--r--   0        0        0     5633 2022-11-02 13:14:06.261169 turnt-1.9.0/turnt/run.py
+-rw-r--r--   0        0        0    10735 1970-01-01 00:00:00.000000 turnt-1.9.0/PKG-INFO
```

### Comparing `turnt-1.8.0/.github/workflows/ci.yml` & `turnt-1.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `turnt-1.8.0/CHANGELOG.md` & `turnt-1.9.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Turnt Changelog
 ===============
 
+1.9.0 (2022-11-02)
+------------------
+
+- `-h` is now an alias for `--help`.
+- `differing` and `missing` notes are now printed on the same line as the test itself, as TAP directives. This should both be easier to read when looking at the TAP output directly, and it should make life a bit simpler for TAP consumers.
+- A new `binary` config option that disables looking with test files for (text) overrides. Even without this flag, binary files no longer crash Turnt altogether and instead merely log an error message.
+
 1.8.0 (2022-06-07)
 ------------------
 
 - Add support for multiple *test environments* that run different commands on the same file. This is especially useful for differential testing, when multiple commands have the same expected output.
 - Flush the output buffer after every line, which makes streaming TAP consumers more useful.
 
 1.7.0 (2022-06-03)
```

### Comparing `turnt-1.8.0/LICENSE` & `turnt-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turnt-1.8.0/README.md` & `turnt-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 The default behaves like this configuration:
 
     output.out = "-"
 
 which captures stdout and saves it in `<test-name>.out`.
 Defining `output` in `turnt.toml` disables this default behavior; you can include it explicitly if you want it alongside other outputs.
 
+### `binary`
+
+By default, Turnt looks inside test files for overrides (see below).
+This won't work if your test inputs are binary (non-text) files (Turnt will warn you and proceed with no overrides).
+Set `binary = true` to suppress this search for overrides altogether.
+
 
 Per-Test Overrides
 ------------------
 
 Sometimes you need to alter the setup for a specific test file.
 Turnt looks for some overrides embedded in the test file itself: for example, you might put them in a comment at the top of a test program.
```

### Comparing `turnt-1.8.0/turnt/__main__.py` & `turnt-1.9.0/turnt/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List, Optional
 import click
 import sys
 from .config import Config
 from .run import run_tests
 
 CONFIG_NAME = 'turnt.toml'
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
-@click.command()
+@click.command(context_settings=CONTEXT_SETTINGS)
 @click.option('--save', is_flag=True, default=False,
               help='Save new outputs (overwriting old).')
 @click.option('--diff', is_flag=True, default=False,
               help='Show a diff between the actual and expected output.')
 @click.option('-p', '--print', 'dump', is_flag=True, default=False,
               help="Just show the command output (don't check anything).")
 @click.option('-v', '--verbose', is_flag=True, default=False,
```

### Comparing `turnt-1.8.0/turnt/config.py` & `turnt-1.9.0/turnt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     command: Optional[str]  # Here, a template to be filled in.
     out_files: Dict[str, str]
     return_code: int
     out_base: str
     opts_file: Optional[str]
     diff_cmd: List[str]
     args: str
+    binary: bool
 
 
 class Test(NamedTuple):
     """The configuration for running a specific test.
     """
     env_name: Optional[str]
 
@@ -190,14 +191,15 @@
         command=config_data.get('command'),
         out_files=config_data.get('output', {"out": STDOUT}),
         return_code=config_data.get('return_code', 0),
         diff_cmd=shlex.split(config_data.get('diff', DIFF_DEFAULT)),
         out_base=config_data.get("out_base", "out"),
         opts_file=config_data.get("opts_file"),
         args='',
+        binary=config_data.get('binary', False),
     )
 
 
 def get_envs(config_base: dict, names: List[str]) -> Iterator[TestEnv]:
     """List the test environments described in a TOML config file.
 
     If `names` is empty, include all the environments where `default` is
@@ -270,16 +272,22 @@
     """
     # Load base options from the configuration file.
     config, config_dir = load_config(path, cfg.config_name)
 
     # Configure each environment.
     for env in get_envs(config, names=cfg.envs):
         # Load the contents and extract overrides.
-        contents = read_contents(env, path)
-        env = override_env(env, contents)
+        if not env.binary:
+            try:
+                contents = read_contents(env, path)
+            except UnicodeDecodeError:
+                print(f'{path}: Could not decode text. '
+                      'Consider setting `binary=true`.')
+            else:
+                env = override_env(env, contents)
 
         # Further override using the global configuration.
         if cfg.args is not None:
             env = env._replace(args=cfg.args)
 
         yield Test(
             env_name=env.name,
```

### Comparing `turnt-1.8.0/turnt/run.py` & `turnt-1.9.0/turnt/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,21 @@
     # Show TAP success line and annotations.
     line = tap_line(not differing, idx, test)
     if update:
         line += ' # skip: updated {}'.format(', '.join(test.out_files.keys()))
 
     diff_exist = [fn for fn in differing if fn not in missing]
     if diff_exist:
-        line += '\n# differing: {}'.format(', '.join(diff_exist))
+        line += ' # differing: {}'.format(', '.join(diff_exist))
     if missing:
-        line += '\n# missing: {}'.format(', '.join(missing))
+        if diff_exist:
+            line += '; '
+        else:
+            line += ' # '
+        line += 'missing: {}'.format(', '.join(missing))
 
     return not differing, [line]
 
 
 def run_test(cfg: Config, test: Test, idx: int) -> Tuple[bool, List[str]]:
     """Run a single test.
```

### Comparing `turnt-1.8.0/PKG-INFO` & `turnt-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turnt
-Version: 1.8.0
+Version: 1.9.0
 Summary: Turnt is a simple expect-style testing tool for command-line
 Home-page: https://github.com/cucapra/turnt
 Author: Adrian Sampson
 Author-email: asampson@cs.cornell.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
@@ -109,14 +109,20 @@
 The default behaves like this configuration:
 
     output.out = "-"
 
 which captures stdout and saves it in `<test-name>.out`.
 Defining `output` in `turnt.toml` disables this default behavior; you can include it explicitly if you want it alongside other outputs.
 
+### `binary`
+
+By default, Turnt looks inside test files for overrides (see below).
+This won't work if your test inputs are binary (non-text) files (Turnt will warn you and proceed with no overrides).
+Set `binary = true` to suppress this search for overrides altogether.
+
 
 Per-Test Overrides
 ------------------
 
 Sometimes you need to alter the setup for a specific test file.
 Turnt looks for some overrides embedded in the test file itself: for example, you might put them in a comment at the top of a test program.
```

