# Comparing `tmp/astroid-3.0.0a6.tar.gz` & `tmp/astroid-3.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a6.tar", last modified: Tue Jul  4 20:09:59 2023, max compression
+gzip compressed data, was "astroid-3.0.0a7.tar", last modified: Sat Jul  8 18:21:24 2023, max compression
```

## Comparing `astroid-3.0.0a6.tar` & `astroid-3.0.0a7.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.811851 astroid-3.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-04 20:09:38.000000 astroid-3.0.0a6/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-04 20:09:38.000000 astroid-3.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 20:09:38.000000 astroid-3.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-04 20:09:59.811851 astroid-3.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-04 20:09:38.000000 astroid-3.0.0a6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.795851 astroid-3.0.0a6/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.803851 astroid-3.0.0a6/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   167768 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.807851 astroid-3.0.0a6/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   104648 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    72666 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-04 20:09:38.000000 astroid-3.0.0a6/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.795851 astroid-3.0.0a6/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:09:59.000000 astroid-3.0.0a6/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-04 20:09:38.000000 astroid-3.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 20:09:38.000000 astroid-3.0.0a6/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 20:09:59.811851 astroid-3.0.0a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:59.811851 astroid-3.0.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   223536 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    93424 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_type_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 20:09:38.000000 astroid-3.0.0a6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.028925 astroid-3.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-08 18:21:06.000000 astroid-3.0.0a7/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-08 18:21:06.000000 astroid-3.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 18:21:06.000000 astroid-3.0.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-08 18:21:24.028925 astroid-3.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-08 18:21:06.000000 astroid-3.0.0a7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:23.992925 astroid-3.0.0a7/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18185 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.020925 astroid-3.0.0a7/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166863 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.024925 astroid-3.0.0a7/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104617 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71204 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-08 18:21:06.000000 astroid-3.0.0a7/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:23.992925 astroid-3.0.0a7/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 18:21:23.000000 astroid-3.0.0a7/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-08 18:21:06.000000 astroid-3.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-08 18:21:06.000000 astroid-3.0.0a7/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-08 18:21:24.032925 astroid-3.0.0a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:24.028925 astroid-3.0.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223797 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55463 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93424 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 18:21:06.000000 astroid-3.0.0a7/tox.ini
```

### Comparing `astroid-3.0.0a6/CONTRIBUTORS.txt` & `astroid-3.0.0a7/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/LICENSE` & `astroid-3.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/PKG-INFO` & `astroid-3.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a6
+Version: 3.0.0a7
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a6/README.rst` & `astroid-3.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/__init__.py` & `astroid-3.0.0a7/astroid/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,26 +143,29 @@
     MatchStar,
     MatchValue,
     Module,
     Name,
     NamedExpr,
     NodeNG,
     Nonlocal,
+    ParamSpec,
     Pass,
     Raise,
     Return,
     Set,
     SetComp,
     Slice,
     Starred,
     Subscript,
-    TryExcept,
-    TryFinally,
+    Try,
     TryStar,
     Tuple,
+    TypeAlias,
+    TypeVar,
+    TypeVarTuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
     are_exclusive,
```

### Comparing `astroid-3.0.0a6/astroid/_ast.py` & `astroid-3.0.0a7/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a7/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/arguments.py` & `astroid-3.0.0a7/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/astroid_manager.py` & `astroid-3.0.0a7/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/bases.py` & `astroid-3.0.0a7/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_argparse.py` & `astroid-3.0.0a7/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_attrs.py` & `astroid-3.0.0a7/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_boto3.py` & `astroid-3.0.0a7/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a7/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_collections.py` & `astroid-3.0.0a7/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_crypt.py` & `astroid-3.0.0a7/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a7/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_curses.py` & `astroid-3.0.0a7/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a7/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_datetime.py` & `astroid-3.0.0a7/astroid/brain/brain_datetime.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a7/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a7/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_functools.py` & `astroid-3.0.0a7/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_gi.py` & `astroid-3.0.0a7/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a7/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_http.py` & `astroid-3.0.0a7/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a7/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_io.py` & `astroid-3.0.0a7/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a7/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a7/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a7/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_nose.py` & `astroid-3.0.0a7/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a7/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a7/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a7/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_pytest.py` & `astroid-3.0.0a7/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_qt.py` & `astroid-3.0.0a7/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_random.py` & `astroid-3.0.0a7/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_re.py` & `astroid-3.0.0a7/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_regex.py` & `astroid-3.0.0a7/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_responses.py` & `astroid-3.0.0a7/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a7/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_signal.py` & `astroid-3.0.0a7/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_six.py` & `astroid-3.0.0a7/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a7/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_ssl.py` & `astroid-3.0.0a7/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a7/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_threading.py` & `astroid-3.0.0a7/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_type.py` & `astroid-3.0.0a7/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_typing.py` & `astroid-3.0.0a7/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_unittest.py` & `astroid-3.0.0a7/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/brain_uuid.py` & `astroid-3.0.0a7/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/brain/helpers.py` & `astroid-3.0.0a7/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/builder.py` & `astroid-3.0.0a7/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/const.py` & `astroid-3.0.0a7/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/constraint.py` & `astroid-3.0.0a7/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/context.py` & `astroid-3.0.0a7/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/decorators.py` & `astroid-3.0.0a7/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/exceptions.py` & `astroid-3.0.0a7/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/filter_statements.py` & `astroid-3.0.0a7/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/helpers.py` & `astroid-3.0.0a7/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/inference_tip.py` & `astroid-3.0.0a7/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a7/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/interpreter/_import/util.py` & `astroid-3.0.0a7/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a7/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a7/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/manager.py` & `astroid-3.0.0a7/astroid/manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/mixins.py` & `astroid-3.0.0a7/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/modutils.py` & `astroid-3.0.0a7/astroid/modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/node_classes.py` & `astroid-3.0.0a7/astroid/node_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,26 +58,29 @@
     MatchSingleton,
     MatchStar,
     MatchValue,
     Name,
     NamedExpr,
     NodeNG,
     Nonlocal,
+    ParamSpec,
     Pass,
     Pattern,
     Raise,
     Return,
     Set,
     Slice,
     Starred,
     Subscript,
-    TryExcept,
-    TryFinally,
+    Try,
     TryStar,
     Tuple,
+    TypeAlias,
+    TypeVar,
+    TypeVarTuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
     are_exclusive,
```

### Comparing `astroid-3.0.0a6/astroid/nodes/__init__.py` & `astroid-3.0.0a7/astroid/nodes/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,16 +72,15 @@
     Pattern,
     Raise,
     Return,
     Set,
     Slice,
     Starred,
     Subscript,
-    TryExcept,
-    TryFinally,
+    Try,
     TryStar,
     Tuple,
     TypeAlias,
     TypeVar,
     TypeVarTuple,
     UnaryOp,
     Unknown,
@@ -174,30 +173,29 @@
     MatchValue,
     Module,
     Name,
     NamedExpr,
     NodeNG,
     Nonlocal,
     ParamSpec,
-    TypeVarTuple,
     Pass,
     Pattern,
     Raise,
     Return,
     Set,
     SetComp,
     Slice,
     Starred,
     Subscript,
-    TryExcept,
-    TryFinally,
+    Try,
     TryStar,
     Tuple,
     TypeAlias,
     TypeVar,
+    TypeVarTuple,
     UnaryOp,
     Unknown,
     While,
     With,
     Yield,
     YieldFrom,
 )
@@ -279,16 +277,15 @@
     "Raise",
     "Return",
     "Set",
     "SetComp",
     "Slice",
     "Starred",
     "Subscript",
-    "TryExcept",
-    "TryFinally",
+    "Try",
     "TryStar",
     "Tuple",
     "TypeAlias",
     "TypeVar",
     "TypeVarTuple",
     "UnaryOp",
     "Unknown",
```

### Comparing `astroid-3.0.0a6/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a7/astroid/nodes/_base_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/nodes/as_string.py` & `astroid-3.0.0a7/astroid/nodes/as_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,29 +487,25 @@
         idxstr = idx.accept(self)
         if idx.__class__.__name__.lower() == "tuple" and idx.elts:
             # Remove parenthesis in tuple and extended slice.
             # a[(::1, 1:)] is not valid syntax.
             idxstr = idxstr[1:-1]
         return f"{self._precedence_parens(node, node.value)}[{idxstr}]"
 
-    def visit_tryexcept(self, node) -> str:
-        """return an astroid.TryExcept node as string"""
+    def visit_try(self, node) -> str:
+        """return an astroid.Try node as string"""
         trys = [f"try:\n{self._stmt_list(node.body)}"]
         for handler in node.handlers:
             trys.append(handler.accept(self))
         if node.orelse:
             trys.append(f"else:\n{self._stmt_list(node.orelse)}")
+        if node.finalbody:
+            trys.append(f"finally:\n{self._stmt_list(node.finalbody)}")
         return "\n".join(trys)
 
-    def visit_tryfinally(self, node) -> str:
-        """return an astroid.TryFinally node as string"""
-        return "try:\n{}\nfinally:\n{}".format(
-            self._stmt_list(node.body), self._stmt_list(node.finalbody)
-        )
-
     def visit_trystar(self, node) -> str:
         """return an astroid.TryStar node as string"""
         trys = [f"try:\n{self._stmt_list(node.body)}"]
         for handler in node.handlers:
             trys.append(handler.accept(self))
         if node.orelse:
             trys.append(f"else:\n{self._stmt_list(node.orelse)}")
```

### Comparing `astroid-3.0.0a6/astroid/nodes/const.py` & `astroid-3.0.0a7/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/nodes/node_classes.py` & `astroid-3.0.0a7/astroid/nodes/node_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,27 +139,27 @@
         stmt1_parents[node] = 1
         children[node] = previous
         previous = node
     # climb among stmt2's parents until we find a common parent
     previous = stmt2
     for node in stmt2.node_ancestors():
         if node in stmt1_parents:
-            # if the common parent is a If or TryExcept statement, look if
+            # if the common parent is a If or Try statement, look if
             # nodes are in exclusive branches
             if isinstance(node, If) and exceptions is None:
                 c2attr, c2node = node.locate_child(previous)
                 c1attr, c1node = node.locate_child(children[node])
                 if "test" in (c1attr, c2attr):
                     # If any node is `If.test`, then it must be inclusive with
                     # the other node (`If.body` and `If.orelse`)
                     return False
                 if c1attr != c2attr:
                     # different `If` branches (`If.body` and `If.orelse`)
                     return True
-            elif isinstance(node, TryExcept):
+            elif isinstance(node, Try):
                 c2attr, c2node = node.locate_child(previous)
                 c1attr, c1node = node.locate_child(children[node])
                 if c1node is not c2node:
                     first_in_body_caught_by_handlers = (
                         c2attr == "handlers"
                         and c1attr == "body"
                         and previous.catch(exceptions)
@@ -566,14 +566,15 @@
 
     def _get_name_nodes(self):
         yield self
 
         for child_node in self.get_children():
             yield from child_node._get_name_nodes()
 
+    @decorators.raise_if_nothing_inferred
     @decorators.path_wrapper
     def _infer(
         self, context: InferenceContext | None = None, **kwargs: Any
     ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
         """Infer a Name: use name lookup rules
 
         Same implementation as AssignName._infer_lhs."""
@@ -3715,169 +3716,129 @@
         return self._infer_subscript(context, **kwargs)
 
     @decorators.raise_if_nothing_inferred
     def infer_lhs(self, context: InferenceContext | None = None, **kwargs: Any):
         return self._infer_subscript(context, **kwargs)
 
 
-class TryExcept(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
-    """Class representing an :class:`ast.TryExcept` node.
+class Try(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
+    """Class representing a :class:`ast.Try` node.
 
     >>> import astroid
     >>> node = astroid.extract_node('''
         try:
             do_something()
         except Exception as error:
             print("Error!")
+        finally:
+            print("Cleanup!")
         ''')
     >>> node
-    <TryExcept l.2 at 0x7f23b2e9d908>
+    <Try l.2 at 0x7f23b2e41d68>
     """
 
-    _astroid_fields = ("body", "handlers", "orelse")
-    _multi_line_block_fields = ("body", "handlers", "orelse")
-
-    body: list[NodeNG]
-    """The contents of the block to catch exceptions from."""
-
-    handlers: list[ExceptHandler]
-    """The exception handlers."""
-
-    orelse: list[NodeNG]
-    """The contents of the ``else`` block."""
-
-    def postinit(
-        self,
-        body: list[NodeNG],
-        handlers: list[ExceptHandler],
-        orelse: list[NodeNG],
-    ) -> None:
-        self.body = body
-        self.handlers = handlers
-        self.orelse = orelse
-
-    def _infer_name(self, frame, name):
-        return name
-
-    def block_range(self, lineno: int) -> tuple[int, int]:
-        """Get a range from the given line number to where this node ends.
-
-        :param lineno: The line number to start the range at.
-
-        :returns: The range of line numbers that this node belongs to,
-            starting at the given line number.
-        """
-        last = None
-        for exhandler in self.handlers:
-            if exhandler.type and lineno == exhandler.type.fromlineno:
-                return lineno, lineno
-            if exhandler.body[0].fromlineno <= lineno <= exhandler.body[-1].tolineno:
-                return lineno, exhandler.body[-1].tolineno
-            if last is None:
-                last = exhandler.body[0].fromlineno - 1
-        return self._elsed_block_range(lineno, self.orelse, last)
-
-    def get_children(self):
-        yield from self.body
-
-        yield from self.handlers or ()
-        yield from self.orelse or ()
-
-
-class TryFinally(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
-    """Class representing an :class:`ast.TryFinally` node.
-
-    >>> import astroid
-    >>> node = astroid.extract_node('''
-    try:
-        do_something()
-    except Exception as error:
-        print("Error!")
-    finally:
-        print("Cleanup!")
-    ''')
-    >>> node
-    <TryFinally l.2 at 0x7f23b2e41d68>
-    """
-
-    _astroid_fields = ("body", "finalbody")
-    _multi_line_block_fields = ("body", "finalbody")
+    _astroid_fields = ("body", "handlers", "orelse", "finalbody")
+    _multi_line_block_fields = ("body", "handlers", "orelse", "finalbody")
 
     def __init__(
         self,
-        lineno: int | None = None,
-        col_offset: int | None = None,
-        parent: NodeNG | None = None,
         *,
-        end_lineno: int | None = None,
-        end_col_offset: int | None = None,
+        lineno: int,
+        col_offset: int,
+        end_lineno: int,
+        end_col_offset: int,
+        parent: NodeNG,
     ) -> None:
         """
         :param lineno: The line that this node appears on in the source code.
 
         :param col_offset: The column that this node appears on in the
             source code.
 
         :param parent: The parent node in the syntax tree.
 
         :param end_lineno: The last line this node appears on in the source code.
 
         :param end_col_offset: The end column this node appears on in the
             source code. Note: This is after the last symbol.
         """
-        self.body: list[NodeNG | TryExcept] = []
-        """The try-except that the finally is attached to."""
+        self.body: list[NodeNG] = []
+        """The contents of the block to catch exceptions from."""
+
+        self.handlers: list[ExceptHandler] = []
+        """The exception handlers."""
+
+        self.orelse: list[NodeNG] = []
+        """The contents of the ``else`` block."""
 
         self.finalbody: list[NodeNG] = []
         """The contents of the ``finally`` block."""
 
         super().__init__(
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
             parent=parent,
         )
 
     def postinit(
         self,
-        body: list[NodeNG | TryExcept] | None = None,
-        finalbody: list[NodeNG] | None = None,
+        *,
+        body: list[NodeNG],
+        handlers: list[ExceptHandler],
+        orelse: list[NodeNG],
+        finalbody: list[NodeNG],
     ) -> None:
         """Do some setup after initialisation.
 
-        :param body: The try-except that the finally is attached to.
+        :param body: The contents of the block to catch exceptions from.
+
+        :param handlers: The exception handlers.
+
+        :param orelse: The contents of the ``else`` block.
 
         :param finalbody: The contents of the ``finally`` block.
         """
-        if body is not None:
-            self.body = body
-        if finalbody is not None:
-            self.finalbody = finalbody
-
-    def block_range(self, lineno: int) -> tuple[int, int]:
-        """Get a range from the given line number to where this node ends.
+        self.body = body
+        self.handlers = handlers
+        self.orelse = orelse
+        self.finalbody = finalbody
 
-        :param lineno: The line number to start the range at.
+    def _infer_name(self, frame, name):
+        return name
 
-        :returns: The range of line numbers that this node belongs to,
-            starting at the given line number.
-        """
-        child = self.body[0]
-        # py2.5 try: except: finally:
-        if (
-            isinstance(child, TryExcept)
-            and child.fromlineno == self.fromlineno
-            and child.tolineno >= lineno > self.fromlineno
-        ):
-            return child.block_range(lineno)
-        return self._elsed_block_range(lineno, self.finalbody)
+    def block_range(self, lineno: int) -> tuple[int, int]:
+        """Get a range from a given line number to where this node ends."""
+        if lineno == self.fromlineno:
+            return lineno, lineno
+        if self.body and self.body[0].fromlineno <= lineno <= self.body[-1].tolineno:
+            # Inside try body - return from lineno till end of try body
+            return lineno, self.body[-1].tolineno
+        for exhandler in self.handlers:
+            if exhandler.type and lineno == exhandler.type.fromlineno:
+                return lineno, lineno
+            if exhandler.body[0].fromlineno <= lineno <= exhandler.body[-1].tolineno:
+                return lineno, exhandler.body[-1].tolineno
+        if self.orelse:
+            if self.orelse[0].fromlineno - 1 == lineno:
+                return lineno, lineno
+            if self.orelse[0].fromlineno <= lineno <= self.orelse[-1].tolineno:
+                return lineno, self.orelse[-1].tolineno
+        if self.finalbody:
+            if self.finalbody[0].fromlineno - 1 == lineno:
+                return lineno, lineno
+            if self.finalbody[0].fromlineno <= lineno <= self.finalbody[-1].tolineno:
+                return lineno, self.finalbody[-1].tolineno
+        return lineno, self.tolineno
 
     def get_children(self):
         yield from self.body
+        yield from self.handlers
+        yield from self.orelse
         yield from self.finalbody
 
 
 class TryStar(_base_nodes.MultiLineWithElseBlockNode, _base_nodes.Statement):
     """Class representing an :class:`ast.TryStar` node."""
 
     _astroid_fields = ("body", "handlers", "orelse", "finalbody")
```

### Comparing `astroid-3.0.0a6/astroid/nodes/node_ng.py` & `astroid-3.0.0a7/astroid/nodes/node_ng.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,15 @@
     def _get_yield_nodes_skip_functions(self):
         yield from ()
 
     def _get_yield_nodes_skip_lambdas(self):
         yield from ()
 
     def _infer_name(self, frame, name):
-        # overridden for ImportFrom, Import, Global, TryExcept, TryStar and Arguments
+        # overridden for ImportFrom, Import, Global, Try, TryStar and Arguments
         pass
 
     def _infer(
         self, context: InferenceContext | None = None, **kwargs: Any
     ) -> Generator[InferenceResult, None, InferenceErrorInfo | None]:
         """We don't know how to resolve a statement by default."""
         # this method is overridden by most concrete classes
```

### Comparing `astroid-3.0.0a6/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a7/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a7/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a7/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1527,15 +1527,15 @@
         parent_frame = self.parent.frame()
         property_already_in_parent_locals = self.name in parent_frame.locals and any(
             isinstance(val, objects.Property) for val in parent_frame.locals[self.name]
         )
         # We also don't want to pass parent if the definition is within a Try node
         if isinstance(
             self.parent,
-            (node_classes.TryExcept, node_classes.TryFinally, node_classes.If),
+            (node_classes.Try, node_classes.If),
         ):
             property_already_in_parent_locals = True
 
         prop_func = objects.Property(
             function=self,
             name=self.name,
             lineno=self.lineno,
```

### Comparing `astroid-3.0.0a6/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a7/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/objects.py` & `astroid-3.0.0a7/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/protocols.py` & `astroid-3.0.0a7/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/raw_building.py` & `astroid-3.0.0a7/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/rebuilder.py` & `astroid-3.0.0a7/astroid/rebuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,16 @@
         To keep consistency across astroid and pylint, reset all.
 
         This has been fixed in PyPy 3.9.
         For reference, an (incomplete) list of nodes with issues:
             - ClassDef          - For
             - FunctionDef       - While
             - Call              - If
-            - Decorators        - TryExcept
-            - With              - TryFinally
-            - Assign
+            - Decorators        - Try
+            - With              - Assign
         """
         newnode.end_lineno = None
         newnode.end_col_offset = None
         for child_node in newnode.get_children():
             self._reset_end_lineno(child_node)
 
     def visit_module(
@@ -419,17 +418,15 @@
             ...
 
         @overload
         def visit(self, node: ast.Starred, parent: NodeNG) -> nodes.Starred:
             ...
 
         @overload
-        def visit(
-            self, node: ast.Try, parent: NodeNG
-        ) -> nodes.TryExcept | nodes.TryFinally:
+        def visit(self, node: ast.Try, parent: NodeNG) -> nodes.Try:
             ...
 
         if sys.version_info >= (3, 11):
 
             @overload
             def visit(self, node: ast.TryStar, parent: NodeNG) -> nodes.TryStar:
                 ...
@@ -1627,64 +1624,31 @@
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
             parent=parent,
         )
         newnode.postinit(self.visit(node.value, newnode))
         return newnode
 
-    def visit_tryexcept(self, node: ast.Try, parent: NodeNG) -> nodes.TryExcept:
-        """Visit a TryExcept node by returning a fresh instance of it."""
-        # TryExcept excludes the 'finally' but that will be included in the
-        # end_lineno from 'node'. Therefore, we check all non 'finally'
-        # children to find the correct end_lineno and column.
-        end_lineno = node.end_lineno
-        end_col_offset = node.end_col_offset
-        all_children: list[ast.AST] = [*node.body, *node.handlers, *node.orelse]
-        for child in reversed(all_children):
-            end_lineno = child.end_lineno
-            end_col_offset = child.end_col_offset
-            break
-        newnode = nodes.TryExcept(
+    def visit_try(self, node: ast.Try, parent: NodeNG) -> nodes.Try:
+        """Visit a Try node by returning a fresh instance of it"""
+        newnode = nodes.Try(
             lineno=node.lineno,
             col_offset=node.col_offset,
-            end_lineno=end_lineno,
-            end_col_offset=end_col_offset,
+            end_lineno=node.end_lineno,
+            end_col_offset=node.end_col_offset,
             parent=parent,
         )
         newnode.postinit(
-            [self.visit(child, newnode) for child in node.body],
-            [self.visit(child, newnode) for child in node.handlers],
-            [self.visit(child, newnode) for child in node.orelse],
+            body=[self.visit(child, newnode) for child in node.body],
+            handlers=[self.visit(child, newnode) for child in node.handlers],
+            orelse=[self.visit(child, newnode) for child in node.orelse],
+            finalbody=[self.visit(child, newnode) for child in node.finalbody],
         )
         return newnode
 
-    def visit_try(
-        self, node: ast.Try, parent: NodeNG
-    ) -> nodes.TryExcept | nodes.TryFinally | None:
-        # python 3.3 introduce a new Try node replacing
-        # TryFinally/TryExcept nodes
-        if node.finalbody:
-            newnode = nodes.TryFinally(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                end_lineno=node.end_lineno,
-                end_col_offset=node.end_col_offset,
-                parent=parent,
-            )
-            body: list[NodeNG | nodes.TryExcept]
-            if node.handlers:
-                body = [self.visit_tryexcept(node, newnode)]
-            else:
-                body = [self.visit(child, newnode) for child in node.body]
-            newnode.postinit(body, [self.visit(n, newnode) for n in node.finalbody])
-            return newnode
-        if node.handlers:
-            return self.visit_tryexcept(node, parent)
-        return None
-
     def visit_trystar(self, node: ast.TryStar, parent: NodeNG) -> nodes.TryStar:
         newnode = nodes.TryStar(
             lineno=node.lineno,
             col_offset=node.col_offset,
             end_lineno=node.end_lineno,
             end_col_offset=node.end_col_offset,
             parent=parent,
```

### Comparing `astroid-3.0.0a6/astroid/scoped_nodes.py` & `astroid-3.0.0a7/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/test_utils.py` & `astroid-3.0.0a7/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/transforms.py` & `astroid-3.0.0a7/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/typing.py` & `astroid-3.0.0a7/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid/util.py` & `astroid-3.0.0a7/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a7/astroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a6
+Version: 3.0.0a7
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a6/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a7/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/pyproject.toml` & `astroid-3.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/resources.py` & `astroid-3.0.0a7/tests/resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_builder.py` & `astroid-3.0.0a7/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_constraint.py` & `astroid-3.0.0a7/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_decorators.py` & `astroid-3.0.0a7/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_filter_statements.py` & `astroid-3.0.0a7/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_group_exceptions.py` & `astroid-3.0.0a7/tests/test_group_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 
 from astroid import (
     AssignName,
     ExceptHandler,
     For,
     Name,
-    TryExcept,
+    Try,
     Uninferable,
     bases,
     extract_node,
 )
 from astroid.const import PY311_PLUS
 from astroid.context import InferenceContext
 from astroid.nodes import Expr, Raise, TryStar
@@ -31,27 +31,26 @@
             for err in eg.exceptions:
                 if isinstance(err, ValueError):
                     print("Handling ValueError")
                 elif isinstance(err, TypeError):
                     print("Handling TypeError")"""
         )
     )
-    assert isinstance(node, TryExcept)
+    assert isinstance(node, Try)
     handler = node.handlers[0]
-    exception_group_block_range = (1, 4)
-    assert node.block_range(lineno=1) == exception_group_block_range
+    assert node.block_range(lineno=1) == (1, 9)
     assert node.block_range(lineno=2) == (2, 2)
     assert node.block_range(lineno=5) == (5, 9)
     assert isinstance(handler, ExceptHandler)
     assert handler.type.name == "ExceptionGroup"
     children = list(handler.get_children())
     assert len(children) == 3
     exception_group, short_name, for_loop = children
     assert isinstance(exception_group, Name)
-    assert exception_group.block_range(1) == exception_group_block_range
+    assert exception_group.block_range(1) == (1, 4)
     assert isinstance(short_name, AssignName)
     assert isinstance(for_loop, For)
 
 
 @pytest.mark.skipif(not PY311_PLUS, reason="Requires Python 3.11 or higher")
 def test_star_exceptions() -> None:
     code = textwrap.dedent(
```

### Comparing `astroid-3.0.0a6/tests/test_helpers.py` & `astroid-3.0.0a7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_inference.py` & `astroid-3.0.0a7/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1466,14 +1466,21 @@
         """
         node = extract_node(code)
         assert isinstance(node, nodes.NodeNG)
         results = node.inferred()
         assert len(results) == 2
         assert all(isinstance(result, nodes.Dict) for result in results)
 
+    def test_name_repeat_inference(self) -> None:
+        node = extract_node("print")
+        context = InferenceContext()
+        _ = next(node.infer(context=context))
+        with pytest.raises(InferenceError):
+            next(node.infer(context=context))
+
     def test_python25_no_relative_import(self) -> None:
         ast = resources.build_file("data/package/absimport.py")
         self.assertTrue(ast.absolute_import_activated(), True)
         inferred = next(
             test_utils.get_name_node(ast, "import_package_subpackage_module").infer()
         )
         # failed to import since absolute_import is activated
```

### Comparing `astroid-3.0.0a6/tests/test_inference_calls.py` & `astroid-3.0.0a7/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_lookup.py` & `astroid-3.0.0a7/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_manager.py` & `astroid-3.0.0a7/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_modutils.py` & `astroid-3.0.0a7/tests/test_modutils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_nodes.py` & `astroid-3.0.0a7/tests/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,72 +364,104 @@
         self.assertEqual(self.astroid.block_range(10), (0, 22))  # XXX (10, 22) ?
         self.assertEqual(self.astroid.body[1].block_range(5), (5, 6))
         self.assertEqual(self.astroid.body[1].block_range(6), (6, 6))
         self.assertEqual(self.astroid.body[1].orelse[0].block_range(7), (7, 8))
         self.assertEqual(self.astroid.body[1].orelse[0].block_range(8), (8, 8))
 
 
+class TryNodeTest(_NodeTest):
+    CODE = """
+        try:  # L2
+            print("Hello")
+        except IOError:
+            pass
+        except UnicodeError:
+            pass
+        else:
+            print()
+        finally:
+            print()
+    """
+
+    def test_block_range(self) -> None:
+        try_node = self.astroid.body[0]
+        assert try_node.block_range(1) == (1, 11)
+        assert try_node.block_range(2) == (2, 2)
+        assert try_node.block_range(3) == (3, 3)
+        assert try_node.block_range(4) == (4, 4)
+        assert try_node.block_range(5) == (5, 5)
+        assert try_node.block_range(6) == (6, 6)
+        assert try_node.block_range(7) == (7, 7)
+        assert try_node.block_range(8) == (8, 8)
+        assert try_node.block_range(9) == (9, 9)
+        assert try_node.block_range(10) == (10, 10)
+        assert try_node.block_range(11) == (11, 11)
+
+
 class TryExceptNodeTest(_NodeTest):
     CODE = """
         try:
             print ('pouet')
         except IOError:
             pass
         except UnicodeError:
             print()
         else:
             print()
     """
 
     def test_block_range(self) -> None:
         # XXX ensure expected values
-        self.assertEqual(self.astroid.body[0].block_range(1), (1, 8))
+        self.assertEqual(self.astroid.body[0].block_range(1), (1, 9))
         self.assertEqual(self.astroid.body[0].block_range(2), (2, 2))
-        self.assertEqual(self.astroid.body[0].block_range(3), (3, 8))
+        self.assertEqual(self.astroid.body[0].block_range(3), (3, 3))
         self.assertEqual(self.astroid.body[0].block_range(4), (4, 4))
         self.assertEqual(self.astroid.body[0].block_range(5), (5, 5))
         self.assertEqual(self.astroid.body[0].block_range(6), (6, 6))
         self.assertEqual(self.astroid.body[0].block_range(7), (7, 7))
         self.assertEqual(self.astroid.body[0].block_range(8), (8, 8))
+        self.assertEqual(self.astroid.body[0].block_range(9), (9, 9))
 
 
 class TryFinallyNodeTest(_NodeTest):
     CODE = """
         try:
             print ('pouet')
         finally:
             print ('pouet')
     """
 
     def test_block_range(self) -> None:
         # XXX ensure expected values
-        self.assertEqual(self.astroid.body[0].block_range(1), (1, 4))
+        self.assertEqual(self.astroid.body[0].block_range(1), (1, 5))
         self.assertEqual(self.astroid.body[0].block_range(2), (2, 2))
-        self.assertEqual(self.astroid.body[0].block_range(3), (3, 4))
+        self.assertEqual(self.astroid.body[0].block_range(3), (3, 3))
         self.assertEqual(self.astroid.body[0].block_range(4), (4, 4))
+        self.assertEqual(self.astroid.body[0].block_range(5), (5, 5))
 
 
 class TryExceptFinallyNodeTest(_NodeTest):
     CODE = """
         try:
             print('pouet')
         except Exception:
             print ('oops')
         finally:
             print ('pouet')
     """
 
     def test_block_range(self) -> None:
         # XXX ensure expected values
-        self.assertEqual(self.astroid.body[0].block_range(1), (1, 6))
+        self.assertEqual(self.astroid.body[0].block_range(1), (1, 7))
         self.assertEqual(self.astroid.body[0].block_range(2), (2, 2))
-        self.assertEqual(self.astroid.body[0].block_range(3), (3, 4))
+        self.assertEqual(self.astroid.body[0].block_range(3), (3, 3))
         self.assertEqual(self.astroid.body[0].block_range(4), (4, 4))
         self.assertEqual(self.astroid.body[0].block_range(5), (5, 5))
         self.assertEqual(self.astroid.body[0].block_range(6), (6, 6))
+        self.assertEqual(self.astroid.body[0].block_range(7), (7, 7))
 
 
 class ImportNodeTest(resources.SysPathSetup, unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         self.module = resources.build_file("data/module.py", "data.module")
         self.module2 = resources.build_file("data/module2.py", "data.module2")
```

### Comparing `astroid-3.0.0a6/tests/test_nodes_lineno.py` & `astroid-3.0.0a7/tests/test_nodes_lineno.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,15 +759,15 @@
             pass
         """
         ).strip()
         ast_nodes = builder.extract_node(code)
         assert isinstance(ast_nodes, list) and len(ast_nodes) == 2
 
         t1 = ast_nodes[0]
-        assert isinstance(t1, nodes.TryExcept)
+        assert isinstance(t1, nodes.Try)
         assert isinstance(t1.body[0], nodes.Pass)
         assert isinstance(t1.orelse[0], nodes.Pass)
         assert (t1.lineno, t1.col_offset) == (1, 0)
         assert (t1.end_lineno, t1.end_col_offset) == (8, 8)
         assert (t1.body[0].lineno, t1.body[0].col_offset) == (2, 4)
         assert (t1.body[0].end_lineno, t1.body[0].end_col_offset) == (2, 8)
         assert (t1.orelse[0].lineno, t1.orelse[0].col_offset) == (8, 4)
@@ -785,21 +785,20 @@
         # TODO fix column offset: ExceptHandler -> name (AssignName)
         assert (t2.name.lineno, t2.name.col_offset) == (3, 0)
         assert (t2.name.end_lineno, t2.name.end_col_offset) == (4, 8)
         assert (t2.body[0].lineno, t2.body[0].col_offset) == (4, 4)
         assert (t2.body[0].end_lineno, t2.body[0].end_col_offset) == (4, 8)
 
         t3 = ast_nodes[1]
-        assert isinstance(t3, nodes.TryFinally)
-        assert isinstance(t3.body[0], nodes.TryExcept)
+        assert isinstance(t3, nodes.Try)
         assert isinstance(t3.finalbody[0], nodes.Pass)
         assert (t3.lineno, t3.col_offset) == (10, 0)
         assert (t3.end_lineno, t3.end_col_offset) == (17, 8)
-        assert (t3.body[0].lineno, t3.body[0].col_offset) == (10, 0)
-        assert (t3.body[0].end_lineno, t3.body[0].end_col_offset) == (15, 8)
+        assert (t3.body[0].lineno, t3.body[0].col_offset) == (11, 4)
+        assert (t3.body[0].end_lineno, t3.body[0].end_col_offset) == (11, 8)
         assert (t3.finalbody[0].lineno, t3.finalbody[0].col_offset) == (17, 4)
         assert (t3.finalbody[0].end_lineno, t3.finalbody[0].end_col_offset) == (17, 8)
 
     @staticmethod
     def test_end_lineno_subscript() -> None:
         """Subscript, Slice, (ExtSlice, Index)."""
         code = textwrap.dedent(
```

### Comparing `astroid-3.0.0a6/tests/test_nodes_position.py` & `astroid-3.0.0a7/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_object_model.py` & `astroid-3.0.0a7/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_objects.py` & `astroid-3.0.0a7/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_protocols.py` & `astroid-3.0.0a7/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_python3.py` & `astroid-3.0.0a7/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_raw_building.py` & `astroid-3.0.0a7/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_regrtest.py` & `astroid-3.0.0a7/tests/test_regrtest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_scoped_nodes.py` & `astroid-3.0.0a7/tests/test_scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_stdlib.py` & `astroid-3.0.0a7/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_transforms.py` & `astroid-3.0.0a7/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_type_params.py` & `astroid-3.0.0a7/tests/test_type_params.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a6/tests/test_utils.py` & `astroid-3.0.0a7/tests/test_utils.py`

 * *Files identical despite different names*

