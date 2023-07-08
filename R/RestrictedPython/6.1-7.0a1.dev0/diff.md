# Comparing `tmp/RestrictedPython-6.1.tar.gz` & `tmp/RestrictedPython-7.0a1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RestrictedPython-6.1.tar", last modified: Sat Jul  8 07:29:11 2023, max compression
+gzip compressed data, was "RestrictedPython-7.0a1.dev0.tar", last modified: Fri Mar 10 07:13:04 2023, max compression
```

## Comparing `RestrictedPython-6.1.tar` & `RestrictedPython-7.0a1.dev0.tar`

### file list

```diff
@@ -1,171 +1,133 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.604330 RestrictedPython-6.1/
--rw-r--r--   0 jens       (501) staff       (20)     7122 2023-07-08 07:25:49.000000 RestrictedPython-6.1/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2022-06-21 13:29:05.000000 RestrictedPython-6.1/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:20.000000 RestrictedPython-6.1/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:20.000000 RestrictedPython-6.1/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      431 2022-06-21 13:29:05.000000 RestrictedPython-6.1/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    11488 2023-07-08 07:29:11.604406 RestrictedPython-6.1/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     2960 2023-07-08 07:15:15.000000 RestrictedPython-6.1/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      148 2021-11-02 08:52:20.000000 RestrictedPython-6.1/buildout.cfg
--rw-r--r--   0 jens       (501) staff       (20)      155 2022-06-21 13:29:05.000000 RestrictedPython-6.1/constraints.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.591756 RestrictedPython-6.1/docs/
--rw-r--r--   0 jens       (501) staff       (20)     8119 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.588817 RestrictedPython-6.1/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.591853 RestrictedPython-6.1/docs/_build/doctest/
--rw-r--r--   0 jens       (501) staff       (20)      739 2023-07-08 07:01:45.000000 RestrictedPython-6.1/docs/_build/doctest/output.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.588905 RestrictedPython-6.1/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.591967 RestrictedPython-6.1/docs/_build/html/_images/
--rw-r--r--   0 jens       (501) staff       (20)   388310 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_images/logo.jpg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.592649 RestrictedPython-6.1/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/changes.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.594120 RestrictedPython-6.1/docs/_build/html/_sources/contributing/
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from26to27.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from30to31.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      147 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from310to311.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      149 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from311to312.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from31to32.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from32to33.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from33to34.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from34to35.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from35to36.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from36to37.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from37to38.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from38to39.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      145 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/changes_from39to310.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    14562 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/_build/html/_sources/contributing/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     4160 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/idea.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1151 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.594225 RestrictedPython-6.1/docs/_build/html/_sources/install/
--rw-r--r--   0 jens       (501) staff       (20)      346 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/install/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.594331 RestrictedPython-6.1/docs/_build/html/_sources/roadmap/
--rw-r--r--   0 jens       (501) staff       (20)     1204 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/_build/html/_sources/roadmap/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.594435 RestrictedPython-6.1/docs/_build/html/_sources/upgrade_dependencies/
--rw-r--r--   0 jens       (501) staff       (20)     1260 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/upgrade_dependencies/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.594919 RestrictedPython-6.1/docs/_build/html/_sources/usage/
--rw-r--r--   0 jens       (501) staff       (20)     5823 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/usage/api.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     3596 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/usage/basic_usage.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2914 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/usage/framework_usage.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      127 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/usage/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     6922 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/_build/html/_sources/usage/policy.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)    10475 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/conf.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.596232 RestrictedPython-6.1/docs/contributing/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.597642 RestrictedPython-6.1/docs/contributing/ast/
--rwxr-xr-x   0 jens       (501) staff       (20)     4572 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python2_6.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     4719 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python2_7.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5170 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_0.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5170 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_1.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     6756 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/contributing/ast/python3_10.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     6843 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/contributing/ast/python3_11.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     6843 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/contributing/ast/python3_12.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5171 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_2.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5135 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_3.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5107 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_4.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5402 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/ast/python3_5.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5828 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/ast/python3_6.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5828 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/ast/python3_7.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     6112 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/ast/python3_8.ast
--rwxr-xr-x   0 jens       (501) staff       (20)     5919 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/contributing/ast/python3_9.ast
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from26to27.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from30to31.rst
--rw-r--r--   0 jens       (501) staff       (20)      147 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from310to311.rst
--rw-r--r--   0 jens       (501) staff       (20)      149 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/contributing/changes_from311to312.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from31to32.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from32to33.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from33to34.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from34to35.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from35to36.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/changes_from36to37.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/changes_from37to38.rst
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/contributing/changes_from38to39.rst
--rw-r--r--   0 jens       (501) staff       (20)      145 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/contributing/changes_from39to310.rst
--rw-r--r--   0 jens       (501) staff       (20)    14711 2023-07-08 07:18:30.000000 RestrictedPython-6.1/docs/contributing/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     4160 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/idea.rst
--rw-r--r--   0 jens       (501) staff       (20)     1151 2023-07-08 07:15:15.000000 RestrictedPython-6.1/docs/index.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.597737 RestrictedPython-6.1/docs/install/
--rw-r--r--   0 jens       (501) staff       (20)      346 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/install/index.rst
--rw-r--r--   0 jens       (501) staff       (20)   388310 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/logo.jpg
--rw-r--r--   0 jens       (501) staff       (20)     7761 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/make.bat
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.597824 RestrictedPython-6.1/docs/roadmap/
--rw-r--r--   0 jens       (501) staff       (20)     1204 2022-11-01 15:05:11.000000 RestrictedPython-6.1/docs/roadmap/index.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.597919 RestrictedPython-6.1/docs/upgrade_dependencies/
--rw-r--r--   0 jens       (501) staff       (20)     1260 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/upgrade_dependencies/index.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.598370 RestrictedPython-6.1/docs/usage/
--rw-r--r--   0 jens       (501) staff       (20)     5823 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/usage/api.rst
--rw-r--r--   0 jens       (501) staff       (20)     3596 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/usage/basic_usage.rst
--rw-r--r--   0 jens       (501) staff       (20)     2914 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/usage/framework_usage.rst
--rw-r--r--   0 jens       (501) staff       (20)      127 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/usage/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     6922 2021-11-02 08:52:20.000000 RestrictedPython-6.1/docs/usage/policy.rst
--rw-r--r--   0 jens       (501) staff       (20)      716 2023-07-08 07:29:11.604674 RestrictedPython-6.1/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2732 2023-07-08 07:25:56.000000 RestrictedPython-6.1/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.589607 RestrictedPython-6.1/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.599191 RestrictedPython-6.1/src/RestrictedPython/
--rw-r--r--   0 jens       (501) staff       (20)     3201 2022-06-21 13:29:05.000000 RestrictedPython-6.1/src/RestrictedPython/Eval.py
--rw-r--r--   0 jens       (501) staff       (20)     7560 2022-11-02 08:18:05.000000 RestrictedPython-6.1/src/RestrictedPython/Guards.py
--rw-r--r--   0 jens       (501) staff       (20)     1866 2021-11-02 08:52:20.000000 RestrictedPython-6.1/src/RestrictedPython/Limits.py
--rw-r--r--   0 jens       (501) staff       (20)     1137 2022-06-21 13:29:05.000000 RestrictedPython-6.1/src/RestrictedPython/PrintCollector.py
--rw-r--r--   0 jens       (501) staff       (20)     2485 2022-06-21 13:29:05.000000 RestrictedPython-6.1/src/RestrictedPython/Utilities.py
--rw-r--r--   0 jens       (501) staff       (20)     1862 2021-11-02 08:52:20.000000 RestrictedPython-6.1/src/RestrictedPython/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      381 2023-07-08 07:15:15.000000 RestrictedPython-6.1/src/RestrictedPython/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)     6727 2022-06-21 13:29:05.000000 RestrictedPython-6.1/src/RestrictedPython/compile.py
--rw-r--r--   0 jens       (501) staff       (20)    41788 2023-07-08 07:18:30.000000 RestrictedPython-6.1/src/RestrictedPython/transformer.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.599785 RestrictedPython-6.1/src/RestrictedPython.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    11488 2023-07-08 07:29:11.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     5303 2023-07-08 07:29:11.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-07-08 07:29:11.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-01 15:05:52.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)       59 2023-07-08 07:29:11.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)       17 2023-07-08 07:29:11.000000 RestrictedPython-6.1/src/RestrictedPython.egg-info/top_level.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.600802 RestrictedPython-6.1/tests/
--rw-r--r--   0 jens       (501) staff       (20)       70 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.600995 RestrictedPython-6.1/tests/builtins/
--rw-r--r--   0 jens       (501) staff       (20)     1800 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/builtins/test_limits.py
--rw-r--r--   0 jens       (501) staff       (20)     4252 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/builtins/test_utilities.py
--rw-r--r--   0 jens       (501) staff       (20)     1156 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/helper.py
--rw-r--r--   0 jens       (501) staff       (20)     6835 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_Guards.py
--rw-r--r--   0 jens       (501) staff       (20)     1928 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_NamedExpr.py
--rw-r--r--   0 jens       (501) staff       (20)     1046 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/test_Utilities.py
--rw-r--r--   0 jens       (501) staff       (20)     7246 2023-07-08 07:23:09.000000 RestrictedPython-6.1/tests/test_compile.py
--rw-r--r--   0 jens       (501) staff       (20)     6297 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_compile_restricted_function.py
--rw-r--r--   0 jens       (501) staff       (20)     2758 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_eval.py
--rw-r--r--   0 jens       (501) staff       (20)     1536 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_imports.py
--rw-r--r--   0 jens       (501) staff       (20)     1010 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_iterating_over_dict_items.py
--rw-r--r--   0 jens       (501) staff       (20)     8262 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/test_print_function.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.603575 RestrictedPython-6.1/tests/transformer/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-08 07:29:11.604232 RestrictedPython-6.1/tests/transformer/operators/
--rw-r--r--   0 jens       (501) staff       (20)      752 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/operators/test_arithmetic_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      415 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_bit_wise_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      246 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_bool_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      408 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_comparison_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      181 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_identity_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      188 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_logical_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      184 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/operators/test_unary_operators.py
--rw-r--r--   0 jens       (501) staff       (20)      170 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_assert.py
--rw-r--r--   0 jens       (501) staff       (20)     1343 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_assign.py
--rw-r--r--   0 jens       (501) staff       (20)     2614 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_async.py
--rw-r--r--   0 jens       (501) staff       (20)     3871 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_attribute.py
--rw-r--r--   0 jens       (501) staff       (20)     1711 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_augassign.py
--rw-r--r--   0 jens       (501) staff       (20)      618 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_base_types.py
--rw-r--r--   0 jens       (501) staff       (20)      360 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_breakpoint.py
--rw-r--r--   0 jens       (501) staff       (20)     3339 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_call.py
--rw-r--r--   0 jens       (501) staff       (20)     4351 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_classdef.py
--rw-r--r--   0 jens       (501) staff       (20)     2157 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_comparators.py
--rw-r--r--   0 jens       (501) staff       (20)      974 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_conditional.py
--rw-r--r--   0 jens       (501) staff       (20)     1221 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_dict_comprehension.py
--rw-r--r--   0 jens       (501) staff       (20)      653 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_eval_exec.py
--rw-r--r--   0 jens       (501) staff       (20)     1641 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_fstring.py
--rw-r--r--   0 jens       (501) staff       (20)     1996 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_functiondef.py
--rw-r--r--   0 jens       (501) staff       (20)      535 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_generic.py
--rw-r--r--   0 jens       (501) staff       (20)      728 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_global_local.py
--rw-r--r--   0 jens       (501) staff       (20)     2872 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_import.py
--rw-r--r--   0 jens       (501) staff       (20)     1872 2023-07-08 07:18:30.000000 RestrictedPython-6.1/tests/transformer/test_inspect.py
--rw-r--r--   0 jens       (501) staff       (20)     3798 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_iterator.py
--rw-r--r--   0 jens       (501) staff       (20)     1970 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_lambda.py
--rw-r--r--   0 jens       (501) staff       (20)      754 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_loop.py
--rw-r--r--   0 jens       (501) staff       (20)     4600 2022-06-21 13:29:05.000000 RestrictedPython-6.1/tests/transformer/test_name.py
--rw-r--r--   0 jens       (501) staff       (20)      776 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_slice.py
--rw-r--r--   0 jens       (501) staff       (20)     4138 2021-11-02 08:52:20.000000 RestrictedPython-6.1/tests/transformer/test_subscript.py
--rw-r--r--   0 jens       (501) staff       (20)     4007 2022-11-02 08:18:05.000000 RestrictedPython-6.1/tests/transformer/test_try.py
--rw-r--r--   0 jens       (501) staff       (20)     3826 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_with_stmt.py
--rw-r--r--   0 jens       (501) staff       (20)     1894 2022-11-01 15:05:11.000000 RestrictedPython-6.1/tests/transformer/test_yield.py
--rw-r--r--   0 jens       (501) staff       (20)     2516 2023-07-08 07:15:15.000000 RestrictedPython-6.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.558254 RestrictedPython-7.0a1.dev0/
+-rw-r--r--   0 mac        (513) staff       (20)     7272 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      431 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    11632 2023-03-10 07:13:04.558421 RestrictedPython-7.0a1.dev0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2997 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      148 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      155 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/constraints.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.524788 RestrictedPython-7.0a1.dev0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     8119 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/changes.rst
+-rw-r--r--   0 mac        (513) staff       (20)    10475 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/conf.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.528874 RestrictedPython-7.0a1.dev0/docs/contributing/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.534442 RestrictedPython-7.0a1.dev0/docs/contributing/ast/
+-rwxr-xr-x   0 mac        (513) staff       (20)     4572 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python2_6.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     4719 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python2_7.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5170 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_0.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5170 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_1.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     6756 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_10.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     6843 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_11.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     6843 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_12.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5171 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_2.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5135 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_3.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5107 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_4.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5402 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_5.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5828 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_6.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5828 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_7.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     6112 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_8.ast
+-rwxr-xr-x   0 mac        (513) staff       (20)     5919 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_9.ast
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from26to27.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from30to31.rst
+-rw-r--r--   0 mac        (513) staff       (20)      147 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from310to311.rst
+-rw-r--r--   0 mac        (513) staff       (20)      149 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from311to312.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from31to32.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from32to33.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from33to34.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from34to35.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from35to36.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from36to37.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from37to38.rst
+-rw-r--r--   0 mac        (513) staff       (20)      143 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from38to39.rst
+-rw-r--r--   0 mac        (513) staff       (20)      145 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/changes_from39to310.rst
+-rw-r--r--   0 mac        (513) staff       (20)    14562 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/contributing/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4160 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/idea.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1139 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/index.rst
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.534944 RestrictedPython-7.0a1.dev0/docs/install/
+-rw-r--r--   0 mac        (513) staff       (20)      346 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/install/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)   388310 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/logo.jpg
+-rw-r--r--   0 mac        (513) staff       (20)     7761 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/make.bat
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.535247 RestrictedPython-7.0a1.dev0/docs/roadmap/
+-rw-r--r--   0 mac        (513) staff       (20)     1204 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/roadmap/index.rst
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.535554 RestrictedPython-7.0a1.dev0/docs/upgrade_dependencies/
+-rw-r--r--   0 mac        (513) staff       (20)     1260 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/upgrade_dependencies/index.rst
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.537129 RestrictedPython-7.0a1.dev0/docs/usage/
+-rw-r--r--   0 mac        (513) staff       (20)     5823 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/usage/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)     3596 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/usage/basic_usage.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2914 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/usage/framework_usage.rst
+-rw-r--r--   0 mac        (513) staff       (20)      127 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/usage/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     6922 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/docs/usage/policy.rst
+-rw-r--r--   0 mac        (513) staff       (20)      722 2023-03-10 07:13:04.559095 RestrictedPython-7.0a1.dev0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2690 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.515675 RestrictedPython-7.0a1.dev0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.540081 RestrictedPython-7.0a1.dev0/src/RestrictedPython/
+-rw-r--r--   0 mac        (513) staff       (20)     3201 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/Eval.py
+-rw-r--r--   0 mac        (513) staff       (20)     7560 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/Guards.py
+-rw-r--r--   0 mac        (513) staff       (20)     1866 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/Limits.py
+-rw-r--r--   0 mac        (513) staff       (20)     1137 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/PrintCollector.py
+-rw-r--r--   0 mac        (513) staff       (20)     2485 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/Utilities.py
+-rw-r--r--   0 mac        (513) staff       (20)     1862 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      383 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)     6727 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/compile.py
+-rw-r--r--   0 mac        (513) staff       (20)    41116 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython/transformer.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.542223 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    11632 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     3765 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       59 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)       17 2023-03-10 07:13:04.000000 RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.545916 RestrictedPython-7.0a1.dev0/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       70 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.546575 RestrictedPython-7.0a1.dev0/tests/builtins/
+-rw-r--r--   0 mac        (513) staff       (20)     1800 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/builtins/test_limits.py
+-rw-r--r--   0 mac        (513) staff       (20)     4252 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/builtins/test_utilities.py
+-rw-r--r--   0 mac        (513) staff       (20)     1156 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/helper.py
+-rw-r--r--   0 mac        (513) staff       (20)     6835 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_Guards.py
+-rw-r--r--   0 mac        (513) staff       (20)     1928 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_NamedExpr.py
+-rw-r--r--   0 mac        (513) staff       (20)     1046 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_Utilities.py
+-rw-r--r--   0 mac        (513) staff       (20)     7511 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_compile.py
+-rw-r--r--   0 mac        (513) staff       (20)     6297 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_compile_restricted_function.py
+-rw-r--r--   0 mac        (513) staff       (20)     2758 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_eval.py
+-rw-r--r--   0 mac        (513) staff       (20)     1536 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_imports.py
+-rw-r--r--   0 mac        (513) staff       (20)     1010 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_iterating_over_dict_items.py
+-rw-r--r--   0 mac        (513) staff       (20)     8262 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/test_print_function.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.555514 RestrictedPython-7.0a1.dev0/tests/transformer/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-10 07:13:04.557934 RestrictedPython-7.0a1.dev0/tests/transformer/operators/
+-rw-r--r--   0 mac        (513) staff       (20)      752 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_arithmetic_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      415 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_bit_wise_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      246 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_bool_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      408 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_comparison_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      181 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_identity_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      188 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_logical_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      184 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_unary_operators.py
+-rw-r--r--   0 mac        (513) staff       (20)      170 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_assert.py
+-rw-r--r--   0 mac        (513) staff       (20)     1343 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_assign.py
+-rw-r--r--   0 mac        (513) staff       (20)     2614 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_async.py
+-rw-r--r--   0 mac        (513) staff       (20)     3871 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_attribute.py
+-rw-r--r--   0 mac        (513) staff       (20)     1711 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_augassign.py
+-rw-r--r--   0 mac        (513) staff       (20)      618 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_base_types.py
+-rw-r--r--   0 mac        (513) staff       (20)      360 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_breakpoint.py
+-rw-r--r--   0 mac        (513) staff       (20)     3339 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_call.py
+-rw-r--r--   0 mac        (513) staff       (20)     4351 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_classdef.py
+-rw-r--r--   0 mac        (513) staff       (20)     2157 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_comparators.py
+-rw-r--r--   0 mac        (513) staff       (20)      974 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_conditional.py
+-rw-r--r--   0 mac        (513) staff       (20)     1221 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_dict_comprehension.py
+-rw-r--r--   0 mac        (513) staff       (20)      653 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_eval_exec.py
+-rw-r--r--   0 mac        (513) staff       (20)     1641 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_fstring.py
+-rw-r--r--   0 mac        (513) staff       (20)     1996 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_functiondef.py
+-rw-r--r--   0 mac        (513) staff       (20)      535 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_generic.py
+-rw-r--r--   0 mac        (513) staff       (20)      728 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_global_local.py
+-rw-r--r--   0 mac        (513) staff       (20)     2872 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_import.py
+-rw-r--r--   0 mac        (513) staff       (20)     3798 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_iterator.py
+-rw-r--r--   0 mac        (513) staff       (20)     1970 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_lambda.py
+-rw-r--r--   0 mac        (513) staff       (20)      754 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_loop.py
+-rw-r--r--   0 mac        (513) staff       (20)     4600 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_name.py
+-rw-r--r--   0 mac        (513) staff       (20)      776 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_slice.py
+-rw-r--r--   0 mac        (513) staff       (20)     4138 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_subscript.py
+-rw-r--r--   0 mac        (513) staff       (20)     4007 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_try.py
+-rw-r--r--   0 mac        (513) staff       (20)     3826 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_with_stmt.py
+-rw-r--r--   0 mac        (513) staff       (20)     1894 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tests/transformer/test_yield.py
+-rw-r--r--   0 mac        (513) staff       (20)     2548 2023-03-10 07:13:03.000000 RestrictedPython-7.0a1.dev0/tox.ini
```

### Comparing `RestrictedPython-6.1/CHANGES.rst` & `RestrictedPython-7.0a1.dev0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Changes
 =======
 
-6.1 (2023-07-08)
-----------------
+7.0a1.dev0 (2023-03-10)
+-----------------------
+
+Backwards incompatible changes
+++++++++++++++++++++++++++++++
+
+- Drop support for Python 3.6.
+
+Features
+++++++++
 
-- Restrict access to some attributes accessible via the ``inspect`` module.
+- Allow to use the package with Python 3.12 -- Caution: No security audit has
+  been done so far.
 
 
 6.0 (2022-11-03)
 ----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
```

### Comparing `RestrictedPython-6.1/CONTRIBUTING.md` & `RestrictedPython-7.0a1.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/LICENSE.txt` & `RestrictedPython-7.0a1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/PKG-INFO` & `RestrictedPython-7.0a1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: RestrictedPython
-Version: 6.1
+Version: 7.0a1.dev0
 Summary: RestrictedPython is a defined subset of the Python language which allows to provide a program input into a trusted environment.
 Home-page: https://github.com/zopefoundation/RestrictedPython
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://restrictedpython.readthedocs.io/
 Project-URL: Source, https://github.com/zopefoundation/RestrictedPython
 Project-URL: Tracker, https://github.com/zopefoundation/RestrictedPython/issues
 Keywords: restricted execution security untrusted code
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
-.. image:: https://api.travis-ci.com/zopefoundation/RestrictedPython.svg?branch=master
-    :target: https://travis-ci.com/zopefoundation/RestrictedPython
+.. image:: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/RestrictedPython/badge.svg?branch=master
     :target: https://coveralls.io/github/zopefoundation/RestrictedPython?branch=master
 
 .. image:: https://readthedocs.org/projects/restrictedpython/badge/
     :target: https://restrictedpython.readthedocs.org/
     :alt: Documentation Status
@@ -110,24 +109,33 @@
     Traceback (most recent call last):
     ImportError: __import__ not found
 
 Contributing to RestrictedPython
 --------------------------------
 
 If you want to help maintain RestrictedPython and contribute, please refer to
-the documentation `Contributing page 
+the documentation `Contributing page
 <https://restrictedpython.readthedocs.io/en/latest/contributing/index.html>`_.
 
 Changes
 =======
 
-6.1 (2023-07-08)
-----------------
+7.0a1.dev0 (2023-03-10)
+-----------------------
+
+Backwards incompatible changes
+++++++++++++++++++++++++++++++
+
+- Drop support for Python 3.6.
+
+Features
+++++++++
 
-- Restrict access to some attributes accessible via the ``inspect`` module.
+- Allow to use the package with Python 3.12 -- Caution: No security audit has
+  been done so far.
 
 
 6.0 (2022-11-03)
 ----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
```

### Comparing `RestrictedPython-6.1/README.rst` & `RestrictedPython-7.0a1.dev0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. image:: https://api.travis-ci.com/zopefoundation/RestrictedPython.svg?branch=master
-    :target: https://travis-ci.com/zopefoundation/RestrictedPython
+.. image:: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/RestrictedPython/badge.svg?branch=master
     :target: https://coveralls.io/github/zopefoundation/RestrictedPython?branch=master
 
 .. image:: https://readthedocs.org/projects/restrictedpython/badge/
     :target: https://restrictedpython.readthedocs.org/
     :alt: Documentation Status
@@ -79,9 +79,9 @@
     Traceback (most recent call last):
     ImportError: __import__ not found
 
 Contributing to RestrictedPython
 --------------------------------
 
 If you want to help maintain RestrictedPython and contribute, please refer to
-the documentation `Contributing page 
+the documentation `Contributing page
 <https://restrictedpython.readthedocs.io/en/latest/contributing/index.html>`_.
```

### Comparing `RestrictedPython-6.1/docs/Makefile` & `RestrictedPython-7.0a1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_images/logo.jpg` & `RestrictedPython-7.0a1.dev0/docs/logo.jpg`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/contributing/index.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/contributing/index.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/idea.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/idea.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/index.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 RestrictedPython is a tool that helps to define a subset of the Python language which allows to provide a program input into a trusted environment.
 RestrictedPython is not a sandbox system or a secured environment, but it helps to define a trusted environment and execute untrusted code inside of it.
 
 Supported Python versions
 =========================
 
-RestrictedPython supports CPython 2.7, 3.5, 3.6, 3.7 and 3.8.
+RestrictedPython supports CPython 3.7 up to 3.12.
 It does _not_ support PyPy or other alternative Python implementations.
 
 Contents
 ========
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/roadmap/index.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/roadmap/index.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/upgrade_dependencies/index.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/upgrade_dependencies/index.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/usage/api.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/usage/api.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/usage/basic_usage.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/usage/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/usage/framework_usage.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/usage/framework_usage.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/_build/html/_sources/usage/policy.rst.txt` & `RestrictedPython-7.0a1.dev0/docs/usage/policy.rst`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/conf.py` & `RestrictedPython-7.0a1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python2_6.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python2_6.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python2_7.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python2_7.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_0.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_0.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_1.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_1.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_10.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_10.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_11.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_11.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_12.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_12.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_2.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_2.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_3.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_3.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_4.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_4.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_5.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_5.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_6.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_6.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_7.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_7.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_8.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_8.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/contributing/ast/python3_9.ast` & `RestrictedPython-7.0a1.dev0/docs/contributing/ast/python3_9.ast`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/docs/make.bat` & `RestrictedPython-7.0a1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/setup.cfg` & `RestrictedPython-7.0a1.dev0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	docs/_build/html/_sources/upgrade_dependencies/*
 	docs/_build/html/_sources/usage/*
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
-known_third_party = six, docutils, pkg_resources
+known_third_party = six, docutils, pkg_resources, pytz
 known_zope = 
 known_first_party = 
 default_section = ZOPE
 line_length = 79
 lines_after_imports = 2
 
 [egg_info]
```

### Comparing `RestrictedPython-6.1/setup.py` & `RestrictedPython-7.0a1.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,29 @@
     'pytest',
     'pytest-mock',
 ]
 
 
 setup(
     name='RestrictedPython',
-    version='6.1',
+    version='7.0a1.dev0',
     url='https://github.com/zopefoundation/RestrictedPython',
     license='ZPL 2.1',
     description=(
         'RestrictedPython is a defined subset of the Python language which '
         'allows to provide a program input into a trusted environment.'
     ),
     long_description=read('README.rst') + '\n' + read('CHANGES.rst'),
     long_description_content_type='text/x-rst',
     classifiers=[
         'Development Status :: 6 - Mature',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Security',
@@ -64,15 +63,15 @@
         "Source": "https://github.com/zopefoundation/RestrictedPython",
         "Tracker": "https://github.com/zopefoundation/RestrictedPython/issues",
     },
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
     ],
-    python_requires=">=3.6, <3.12",
+    python_requires=">=3.7, <3.13",
     tests_require=tests_require,
     extras_require={
         'test': tests_require,
         'docs': ['Sphinx', 'sphinx_rtd_theme'],
     },
     include_package_data=True,
     zip_safe=False
```

### Comparing `RestrictedPython-6.1/src/RestrictedPython/Eval.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/Eval.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/Guards.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/Guards.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/Limits.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/Limits.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/PrintCollector.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/PrintCollector.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/Utilities.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/Utilities.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/__init__.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/__init__.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/compile.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/compile.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/src/RestrictedPython/transformer.py` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,40 +59,14 @@
 FORBIDDEN_FUNC_NAMES = frozenset([
     'print',
     'printed',
     'builtins',
     'breakpoint',
 ])
 
-# inspect attributes. See also
-# https://docs.python.org/3/library/inspect.html
-INSPECT_ATTRIBUTES = frozenset([
-    # traceback
-    "tb_frame",
-    "tb_next",
-    # code
-    "co_code",
-    # frame
-    "f_back",
-    "f_builtins",
-    "f_code",
-    "f_globals",
-    "f_locals",
-    "f_trace",
-    # generator
-    "gi_frame",
-    "gi_code",
-    "gi_yieldfrom",
-    # coroutine
-    "cr_await",
-    "cr_frame",
-    "cr_code",
-    "cr_origin",
-])
-
 
 # When new ast nodes are generated they have no 'lineno', 'end_lineno',
 # 'col_offset' and 'end_col_offset'. This function copies these fields from the
 # incoming node:
 def copy_locations(new_node, old_node):
     assert 'lineno' in new_node._attributes
     new_node.lineno = old_node.lineno
@@ -866,21 +840,14 @@
 
         if node.attr.endswith('__roles__'):
             self.error(
                 node,
                 '"{name}" is an invalid attribute name because it ends '
                 'with "__roles__".'.format(name=node.attr))
 
-        if node.attr in INSPECT_ATTRIBUTES:
-            self.error(
-                node,
-                f'"{node.attr}" is a restricted name,'
-                ' that is forbidden to access in RestrictedPython.',
-            )
-
         if isinstance(node.ctx, ast.Load):
             node = self.node_contents_visit(node)
             new_node = ast.Call(
                 func=ast.Name('_getattr_', ast.Load()),
                 args=[node.value, ast.Str(node.attr)],
                 keywords=[])
```

### Comparing `RestrictedPython-6.1/src/RestrictedPython.egg-info/PKG-INFO` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: RestrictedPython
-Version: 6.1
+Version: 7.0a1.dev0
 Summary: RestrictedPython is a defined subset of the Python language which allows to provide a program input into a trusted environment.
 Home-page: https://github.com/zopefoundation/RestrictedPython
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://restrictedpython.readthedocs.io/
 Project-URL: Source, https://github.com/zopefoundation/RestrictedPython
 Project-URL: Tracker, https://github.com/zopefoundation/RestrictedPython/issues
 Keywords: restricted execution security untrusted code
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
-.. image:: https://api.travis-ci.com/zopefoundation/RestrictedPython.svg?branch=master
-    :target: https://travis-ci.com/zopefoundation/RestrictedPython
+.. image:: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/zopefoundation/RestrictedPython/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/RestrictedPython/badge.svg?branch=master
     :target: https://coveralls.io/github/zopefoundation/RestrictedPython?branch=master
 
 .. image:: https://readthedocs.org/projects/restrictedpython/badge/
     :target: https://restrictedpython.readthedocs.org/
     :alt: Documentation Status
@@ -110,24 +109,33 @@
     Traceback (most recent call last):
     ImportError: __import__ not found
 
 Contributing to RestrictedPython
 --------------------------------
 
 If you want to help maintain RestrictedPython and contribute, please refer to
-the documentation `Contributing page 
+the documentation `Contributing page
 <https://restrictedpython.readthedocs.io/en/latest/contributing/index.html>`_.
 
 Changes
 =======
 
-6.1 (2023-07-08)
-----------------
+7.0a1.dev0 (2023-03-10)
+-----------------------
+
+Backwards incompatible changes
+++++++++++++++++++++++++++++++
+
+- Drop support for Python 3.6.
+
+Features
+++++++++
 
-- Restrict access to some attributes accessible via the ``inspect`` module.
+- Allow to use the package with Python 3.12 -- Caution: No security audit has
+  been done so far.
 
 
 6.0 (2022-11-03)
 ----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
```

### Comparing `RestrictedPython-6.1/src/RestrictedPython.egg-info/SOURCES.txt` & `RestrictedPython-7.0a1.dev0/src/RestrictedPython.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -12,41 +12,14 @@
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/idea.rst
 docs/index.rst
 docs/logo.jpg
 docs/make.bat
-docs/_build/doctest/output.txt
-docs/_build/html/_images/logo.jpg
-docs/_build/html/_sources/changes.rst.txt
-docs/_build/html/_sources/idea.rst.txt
-docs/_build/html/_sources/index.rst.txt
-docs/_build/html/_sources/contributing/changes_from26to27.rst.txt
-docs/_build/html/_sources/contributing/changes_from30to31.rst.txt
-docs/_build/html/_sources/contributing/changes_from310to311.rst.txt
-docs/_build/html/_sources/contributing/changes_from311to312.rst.txt
-docs/_build/html/_sources/contributing/changes_from31to32.rst.txt
-docs/_build/html/_sources/contributing/changes_from32to33.rst.txt
-docs/_build/html/_sources/contributing/changes_from33to34.rst.txt
-docs/_build/html/_sources/contributing/changes_from34to35.rst.txt
-docs/_build/html/_sources/contributing/changes_from35to36.rst.txt
-docs/_build/html/_sources/contributing/changes_from36to37.rst.txt
-docs/_build/html/_sources/contributing/changes_from37to38.rst.txt
-docs/_build/html/_sources/contributing/changes_from38to39.rst.txt
-docs/_build/html/_sources/contributing/changes_from39to310.rst.txt
-docs/_build/html/_sources/contributing/index.rst.txt
-docs/_build/html/_sources/install/index.rst.txt
-docs/_build/html/_sources/roadmap/index.rst.txt
-docs/_build/html/_sources/upgrade_dependencies/index.rst.txt
-docs/_build/html/_sources/usage/api.rst.txt
-docs/_build/html/_sources/usage/basic_usage.rst.txt
-docs/_build/html/_sources/usage/framework_usage.rst.txt
-docs/_build/html/_sources/usage/index.rst.txt
-docs/_build/html/_sources/usage/policy.rst.txt
 docs/contributing/changes_from26to27.rst
 docs/contributing/changes_from30to31.rst
 docs/contributing/changes_from310to311.rst
 docs/contributing/changes_from311to312.rst
 docs/contributing/changes_from31to32.rst
 docs/contributing/changes_from32to33.rst
 docs/contributing/changes_from33to34.rst
@@ -122,15 +95,14 @@
 tests/transformer/test_dict_comprehension.py
 tests/transformer/test_eval_exec.py
 tests/transformer/test_fstring.py
 tests/transformer/test_functiondef.py
 tests/transformer/test_generic.py
 tests/transformer/test_global_local.py
 tests/transformer/test_import.py
-tests/transformer/test_inspect.py
 tests/transformer/test_iterator.py
 tests/transformer/test_lambda.py
 tests/transformer/test_loop.py
 tests/transformer/test_name.py
 tests/transformer/test_slice.py
 tests/transformer/test_subscript.py
 tests/transformer/test_try.py
```

### Comparing `RestrictedPython-6.1/tests/builtins/test_limits.py` & `RestrictedPython-7.0a1.dev0/tests/builtins/test_limits.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/builtins/test_utilities.py` & `RestrictedPython-7.0a1.dev0/tests/builtins/test_utilities.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/helper.py` & `RestrictedPython-7.0a1.dev0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_Guards.py` & `RestrictedPython-7.0a1.dev0/tests/test_Guards.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_NamedExpr.py` & `RestrictedPython-7.0a1.dev0/tests/test_NamedExpr.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_Utilities.py` & `RestrictedPython-7.0a1.dev0/tests/test_Utilities.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_compile.py` & `RestrictedPython-7.0a1.dev0/tests/test_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from RestrictedPython import CompileResult
 from RestrictedPython import compile_restricted
 from RestrictedPython import compile_restricted_eval
 from RestrictedPython import compile_restricted_exec
 from RestrictedPython import compile_restricted_single
 from RestrictedPython._compat import IS_PY38_OR_GREATER
 from RestrictedPython._compat import IS_PY310_OR_GREATER
+from RestrictedPython._compat import IS_PY312_OR_GREATER
 from tests.helper import restricted_eval
 
 
 def test_compile__compile_restricted_invalid_code_input():
     with pytest.raises(TypeError):
         compile_restricted(object(), '<string>', 'exec')
     with pytest.raises(TypeError):
@@ -98,15 +99,21 @@
 
 def test_compile__compile_restricted_exec__5():
     """It does not return code if the code contains a NULL byte."""
     result = compile_restricted_exec('a = 5\x00')
     assert result.code is None
     assert result.warnings == []
     assert result.used_names == {}
-    assert 'source code string cannot contain null bytes' in result.errors[0]
+    if IS_PY312_OR_GREATER:
+        assert result.errors == (
+            'Line None: SyntaxError: source code string cannot contain null'
+            ' bytes at statement: None',)
+    else:
+        assert result.errors == (
+            'source code string cannot contain null bytes',)
 
 
 EXEC_STATEMENT = """\
 def no_exec():
     exec 'q = 1'
 """
```

### Comparing `RestrictedPython-6.1/tests/test_compile_restricted_function.py` & `RestrictedPython-7.0a1.dev0/tests/test_compile_restricted_function.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_eval.py` & `RestrictedPython-7.0a1.dev0/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_imports.py` & `RestrictedPython-7.0a1.dev0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_iterating_over_dict_items.py` & `RestrictedPython-7.0a1.dev0/tests/test_iterating_over_dict_items.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/test_print_function.py` & `RestrictedPython-7.0a1.dev0/tests/test_print_function.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/operators/test_arithmetic_operators.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/operators/test_arithmetic_operators.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_assign.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_assign.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_async.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_async.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_attribute.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_attribute.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_augassign.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_augassign.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_base_types.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_base_types.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_call.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_call.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_classdef.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_classdef.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_comparators.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_comparators.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_conditional.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_conditional.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_dict_comprehension.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_dict_comprehension.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_eval_exec.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_eval_exec.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_fstring.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_fstring.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_functiondef.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_functiondef.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_generic.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_generic.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_global_local.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_global_local.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_import.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_import.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_iterator.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_iterator.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_lambda.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_lambda.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_loop.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_loop.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_name.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_name.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_slice.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_slice.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_subscript.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_subscript.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_try.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_try.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_with_stmt.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_with_stmt.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tests/transformer/test_yield.py` & `RestrictedPython-7.0a1.dev0/tests/transformer/test_yield.py`

 * *Files identical despite different names*

### Comparing `RestrictedPython-6.1/tox.ini` & `RestrictedPython-7.0a1.dev0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py36
     py37
     py38
     py39
     py310
     py311
+    py312
     docs
     coverage
     py39-datetime
     combined-coverage
 
 [testenv]
 usedevelop = true
+pip_pre = py312: true
 deps =
     datetime: DateTime
     -cconstraints.txt
     pytest-cov
+    Sphinx
 setenv =
     COVERAGE_FILE=.coverage.{envname}
 commands =
     python -V
-    pip list
     pytest --cov=src --cov=tests --cov-report= {posargs}
     sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:combined-coverage]
@@ -43,15 +44,15 @@
     COVERAGE_FILE=.coverage
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage erase
     coverage combine
     coverage html
     coverage report -m --fail-under=100
-depends = py36,py37,py38,py39,py39-datetime,py310,py311,coverage
+depends = py37,py38,py39,py39-datetime,py310,py311,py312coverage
 
 [testenv:lint]
 basepython = python3
 skip_install = true
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py {toxinidir}/tests
     flake8 src setup.py tests
@@ -86,22 +87,23 @@
 allowlist_externals =
     mkdir
 deps =
     coverage
     datetime: DateTime
     -cconstraints.txt
     pytest-cov
+    Sphinx
 setenv =
     COVERAGE_FILE=.coverage
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     pytest --cov=src --cov=tests --cov-report= {posargs}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
     coverage html --ignore-errors
-    coverage report --ignore-errors --show-missing --fail-under=98.5
+    coverage report --ignore-errors --show-missing --fail-under=98.4
 
 [coverage:run]
 branch = True
 source = RestrictedPython
 
 [coverage:report]
 precision = 2
```

