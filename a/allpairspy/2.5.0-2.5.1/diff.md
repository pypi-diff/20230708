# Comparing `tmp/allpairspy-2.5.0.tar.gz` & `tmp/allpairspy-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allpairspy-2.5.0.tar", last modified: Sat May 11 08:50:15 2019, max compression
+gzip compressed data, was "allpairspy-2.5.1.tar", last modified: Sat Jul  8 09:07:20 2023, max compression
```

## Comparing `allpairspy-2.5.0.tar` & `allpairspy-2.5.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0 toor      (1000) toor      (1000)        0 2019-05-11 08:50:15.000000 allpairspy-2.5.0/
--rwxrwxrwx   0 toor      (1000) toor      (1000)      179 2019-05-11 08:50:09.000000 allpairspy-2.5.0/MANIFEST.in
--rwxrwxrwx   0 toor      (1000) toor      (1000)    14548 2019-05-11 08:50:15.000000 allpairspy-2.5.0/PKG-INFO
--rwxrwxrwx   0 toor      (1000) toor      (1000)    10598 2019-05-11 08:50:10.000000 allpairspy-2.5.0/README.rst
-drwxrwxrwx   0 toor      (1000) toor      (1000)        0 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy/
--rwxrwxrwx   0 toor      (1000) toor      (1000)      197 2019-05-11 08:50:10.000000 allpairspy-2.5.0/allpairspy/__init__.py
--rwxrwxrwx   0 toor      (1000) toor      (1000)      258 2019-05-11 08:50:11.000000 allpairspy-2.5.0/allpairspy/__version__.py
--rwxrwxrwx   0 toor      (1000) toor      (1000)     7748 2019-05-11 08:50:11.000000 allpairspy-2.5.0/allpairspy/allpairs.py
--rwxrwxrwx   0 toor      (1000) toor      (1000)     1779 2019-05-11 08:50:11.000000 allpairspy-2.5.0/allpairspy/pairs_storage.py
-drwxrwxrwx   0 toor      (1000) toor      (1000)        0 2019-05-11 08:50:15.000000 allpairspy-2.5.0/allpairspy.egg-info/
--rwxrwxrwx   0 toor      (1000) toor      (1000)    14548 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy.egg-info/PKG-INFO
--rwxrwxrwx   0 toor      (1000) toor      (1000)      405 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy.egg-info/SOURCES.txt
--rwxrwxrwx   0 toor      (1000) toor      (1000)        1 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy.egg-info/dependency_links.txt
--rwxrwxrwx   0 toor      (1000) toor      (1000)       92 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy.egg-info/requires.txt
--rwxrwxrwx   0 toor      (1000) toor      (1000)       11 2019-05-11 08:50:14.000000 allpairspy-2.5.0/allpairspy.egg-info/top_level.txt
-drwxrwxrwx   0 toor      (1000) toor      (1000)        0 2019-05-11 08:50:15.000000 allpairspy-2.5.0/requirements/
--rwxrwxrwx   0 toor      (1000) toor      (1000)       19 2019-05-11 08:50:11.000000 allpairspy-2.5.0/requirements/requirements.txt
--rwxrwxrwx   0 toor      (1000) toor      (1000)        7 2019-05-11 08:50:11.000000 allpairspy-2.5.0/requirements/test_requirements.txt
--rwxrwxrwx   0 toor      (1000) toor      (1000)       92 2019-05-11 08:50:15.000000 allpairspy-2.5.0/setup.cfg
--rwxrwxrwx   0 toor      (1000) toor      (1000)     2964 2019-05-11 08:50:11.000000 allpairspy-2.5.0/setup.py
-drwxrwxrwx   0 toor      (1000) toor      (1000)        0 2019-05-11 08:50:15.000000 allpairspy-2.5.0/test/
--rwxrwxrwx   0 toor      (1000) toor      (1000)    10499 2019-05-11 08:50:11.000000 allpairspy-2.5.0/test/test_allpairs.py
--rwxrwxrwx   0 toor      (1000) toor      (1000)      104 2019-05-11 08:50:11.000000 allpairspy-2.5.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 09:07:20.871602 allpairspy-2.5.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1073 2023-07-08 09:06:48.000000 allpairspy-2.5.1/LICENSE.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      184 2023-07-08 09:06:48.000000 allpairspy-2.5.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    13956 2023-07-08 09:07:20.871602 allpairspy-2.5.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    12250 2023-07-08 09:06:48.000000 allpairspy-2.5.1/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 09:07:20.871602 allpairspy-2.5.1/allpairspy/
+-rw-r--r--   0 toor      (1000) toor      (1000)      178 2023-07-08 09:06:48.000000 allpairspy-2.5.1/allpairspy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      238 2023-07-08 09:06:48.000000 allpairspy-2.5.1/allpairspy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7636 2023-07-08 09:06:48.000000 allpairspy-2.5.1/allpairspy/allpairs.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1715 2023-07-08 09:06:48.000000 allpairspy-2.5.1/allpairspy/pairs_storage.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 09:07:20.871602 allpairspy-2.5.1/allpairspy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    13956 2023-07-08 09:07:20.000000 allpairspy-2.5.1/allpairspy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      423 2023-07-08 09:07:20.000000 allpairspy-2.5.1/allpairspy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-08 09:07:20.000000 allpairspy-2.5.1/allpairspy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       44 2023-07-08 09:07:20.000000 allpairspy-2.5.1/allpairspy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       11 2023-07-08 09:07:20.000000 allpairspy-2.5.1/allpairspy.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      982 2023-07-08 09:06:48.000000 allpairspy-2.5.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 09:07:20.871602 allpairspy-2.5.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-08 09:06:48.000000 allpairspy-2.5.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-07-08 09:06:48.000000 allpairspy-2.5.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-08 09:07:20.871602 allpairspy-2.5.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2723 2023-07-08 09:06:48.000000 allpairspy-2.5.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 09:07:20.871602 allpairspy-2.5.1/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)    10439 2023-07-08 09:06:48.000000 allpairspy-2.5.1/tests/test_allpairs.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      924 2023-07-08 09:06:48.000000 allpairspy-2.5.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `allpairspy-2.5.0/PKG-INFO` & `allpairspy-2.5.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,330 +1,338 @@
-Metadata-Version: 2.1
-Name: allpairspy
-Version: 2.5.0
-Summary: Pairwise test combinations generator
-Home-page: https://github.com/thombashi/allpairspy
-Author: MetaCommunications Engineering
-Author-email: metacomm@users.sourceforge.net
-Maintainer: Tsuyoshi Hombashi
-Maintainer-email: tsuyoshi.hombashi@gmail.com
-License: MIT License
-Project-URL: Source, https://github.com/thombashi/allpairspy
-Project-URL: Tracker, https://github.com/thombashi/allpairspy/issues
-Description: .. contents:: **allpairspy** forked from `bayandin/allpairs <https://github.com/bayandin/allpairs>`__
-           :backlinks: top
-           :depth: 2
-        
-        .. image:: https://badge.fury.io/py/allpairspy.svg
-            :target: https://badge.fury.io/py/allpairspy
-            :alt: PyPI package version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/allpairspy.svg
-            :target: https://pypi.org/project/allpairspy
-            :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/travis/thombashi/allpairspy/master.svg?label=Linux/macOS%20CI
-            :target: https://travis-ci.org/thombashi/allpairspy
-            :alt: Linux/macOS CI status
-        
-        .. image:: https://img.shields.io/appveyor/ci/thombashi/allpairspy/master.svg?label=Windows%20CI
-            :target: https://ci.appveyor.com/project/thombashi/allpairspy
-            :alt: Windows CI status
-        
-        .. image:: https://coveralls.io/repos/github/thombashi/allpairspy/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/allpairspy?branch=master
-            :alt: Test coverage
-        
-        
-        AllPairs test combinations generator
-        ------------------------------------------------
-        AllPairs is an open source test combinations generator written in
-        Python, developed and maintained by MetaCommunications Engineering.
-        The generator allows one to create a set of tests using "pairwise
-        combinations" method, reducing a number of combinations of variables
-        into a lesser set that covers most situations.
-        
-        For more info on pairwise testing see http://www.pairwise.org.
-        
-        
-        Features
-        --------
-        * Produces good enough dataset.
-        * Pythonic, iterator-style enumeration interface.
-        * Allows to filter out "invalid" combinations during search for the next combination.
-        * Goes beyond pairs! If/when required can generate n-wise combinations.
-        
-        
-        Get Started
-        ---------------
-        
-        Basic Usage
-        ==================
-        :Sample Code:
-            .. code:: python
-        
-                from allpairspy import AllPairs
-        
-                parameters = [
+.. contents:: **allpairspy** forked from `bayandin/allpairs <https://github.com/bayandin/allpairs>`__
+   :backlinks: top
+   :depth: 2
+
+.. image:: https://badge.fury.io/py/allpairspy.svg
+    :target: https://badge.fury.io/py/allpairspy
+    :alt: PyPI package version
+
+.. image:: https://img.shields.io/pypi/pyversions/allpairspy.svg
+    :target: https://pypi.org/project/allpairspy
+    :alt: Supported Python versions
+
+.. image:: https://github.com/thombashi/allpairspy/workflows/Tests/badge.svg
+    :target: https://github.com/thombashi/allpairspy/actions?query=workflow%3ATests
+    :alt: Linux/macOS/Windows CI status
+
+.. image:: https://coveralls.io/repos/github/thombashi/allpairspy/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/allpairspy?branch=master
+    :alt: Test coverage
+
+
+AllPairs test combinations generator
+------------------------------------------------
+AllPairs is an open source test combinations generator written in
+Python, developed and maintained by MetaCommunications Engineering.
+The generator allows one to create a set of tests using "pairwise
+combinations" method, reducing a number of combinations of variables
+into a lesser set that covers most situations.
+
+For more info on pairwise testing see http://www.pairwise.org.
+
+
+Features
+--------
+* Produces good enough dataset.
+* Pythonic, iterator-style enumeration interface.
+* Allows to filter out "invalid" combinations during search for the next combination.
+* Goes beyond pairs! If/when required can generate n-wise combinations.
+
+
+Get Started
+---------------
+
+Basic Usage
+==================
+:Sample Code:
+    .. code:: python
+
+        from allpairspy import AllPairs
+
+        parameters = [
+            ["Brand X", "Brand Y"],
+            ["98", "NT", "2000", "XP"],
+            ["Internal", "Modem"],
+            ["Salaried", "Hourly", "Part-Time", "Contr."],
+            [6, 10, 15, 30, 60],
+        ]
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Output:
+    .. code::
+
+        PAIRWISE:
+         0: ['Brand X', '98', 'Internal', 'Salaried', 6]
+         1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
+         2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
+         3: ['Brand X', 'XP', 'Modem', 'Contr.', 10]
+         4: ['Brand X', '2000', 'Modem', 'Part-Time', 15]
+         5: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
+         6: ['Brand Y', '98', 'Modem', 'Salaried', 30]
+         7: ['Brand X', 'NT', 'Internal', 'Contr.', 30]
+         8: ['Brand X', '98', 'Internal', 'Hourly', 60]
+         9: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
+        10: ['Brand Y', 'NT', 'Modem', 'Salaried', 60]
+        11: ['Brand Y', 'XP', 'Modem', 'Part-Time', 60]
+        12: ['Brand Y', '2000', 'Modem', 'Hourly', 30]
+        13: ['Brand Y', '98', 'Modem', 'Contr.', 15]
+        14: ['Brand Y', 'XP', 'Modem', 'Salaried', 15]
+        15: ['Brand Y', 'NT', 'Modem', 'Part-Time', 15]
+        16: ['Brand Y', 'XP', 'Modem', 'Part-Time', 30]
+        17: ['Brand Y', '98', 'Modem', 'Part-Time', 6]
+        18: ['Brand Y', '2000', 'Modem', 'Salaried', 6]
+        19: ['Brand Y', '98', 'Modem', 'Salaried', 10]
+        20: ['Brand Y', 'XP', 'Modem', 'Contr.', 6]
+        21: ['Brand Y', 'NT', 'Modem', 'Hourly', 10]
+
+
+Filtering
+==================
+You can restrict pairs by setting a filtering function to ``filter_func`` at
+``AllPairs`` constructor.
+
+:Sample Code:
+    .. code:: python
+
+        from allpairspy import AllPairs
+
+        def is_valid_combination(row):
+            """
+            This is a filtering function. Filtering functions should return True
+            if combination is valid and False otherwise.
+
+            Test row that is passed here can be incomplete.
+            To prevent search for unnecessary items filtering function
+            is executed with found subset of data to validate it.
+            """
+
+            n = len(row)
+
+            if n > 1:
+                # Brand Y does not support Windows 98
+                if "98" == row[1] and "Brand Y" == row[0]:
+                    return False
+
+                # Brand X does not work with XP
+                if "XP" == row[1] and "Brand X" == row[0]:
+                    return False
+
+            if n > 4:
+                # Contractors are billed in 30 min increments
+                if "Contr." == row[3] and row[4] < 30:
+                    return False
+
+            return True
+
+        parameters = [
+            ["Brand X", "Brand Y"],
+            ["98", "NT", "2000", "XP"],
+            ["Internal", "Modem"],
+            ["Salaried", "Hourly", "Part-Time", "Contr."],
+            [6, 10, 15, 30, 60]
+        ]
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters, filter_func=is_valid_combination)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Output:
+    .. code::
+
+        PAIRWISE:
+         0: ['Brand X', '98', 'Internal', 'Salaried', 6]
+         1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
+         2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
+         3: ['Brand X', '2000', 'Modem', 'Contr.', 30]
+         4: ['Brand X', 'NT', 'Internal', 'Contr.', 60]
+         5: ['Brand Y', 'XP', 'Modem', 'Salaried', 60]
+         6: ['Brand X', '98', 'Modem', 'Part-Time', 15]
+         7: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
+         8: ['Brand Y', 'NT', 'Internal', 'Part-Time', 30]
+         9: ['Brand X', '2000', 'Modem', 'Hourly', 10]
+        10: ['Brand Y', 'XP', 'Modem', 'Contr.', 30]
+        11: ['Brand Y', '2000', 'Modem', 'Salaried', 15]
+        12: ['Brand Y', 'NT', 'Modem', 'Salaried', 10]
+        13: ['Brand Y', 'XP', 'Modem', 'Part-Time', 6]
+        14: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
+
+
+Data Source: OrderedDict
+====================================
+You can use ``collections.OrderedDict`` instance as an argument for ``AllPairs`` constructor.
+Pairs will be returned as ``collections.namedtuple`` instances.
+
+:Sample Code:
+    .. code:: python
+
+        from collections import OrderedDict
+        from allpairspy import AllPairs
+
+        parameters = OrderedDict({
+            "brand": ["Brand X", "Brand Y"],
+            "os": ["98", "NT", "2000", "XP"],
+            "minute": [15, 30, 60],
+        })
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Sample Code:
+    .. code::
+
+        PAIRWISE:
+         0: Pairs(brand='Brand X', os='98', minute=15)
+         1: Pairs(brand='Brand Y', os='NT', minute=15)
+         2: Pairs(brand='Brand Y', os='2000', minute=30)
+         3: Pairs(brand='Brand X', os='XP', minute=30)
+         4: Pairs(brand='Brand X', os='2000', minute=60)
+         5: Pairs(brand='Brand Y', os='XP', minute=60)
+         6: Pairs(brand='Brand Y', os='98', minute=60)
+         7: Pairs(brand='Brand X', os='NT', minute=60)
+         8: Pairs(brand='Brand X', os='NT', minute=30)
+         9: Pairs(brand='Brand X', os='98', minute=30)
+        10: Pairs(brand='Brand X', os='XP', minute=15)
+        11: Pairs(brand='Brand X', os='2000', minute=15)
+
+
+Parameterized testing pairwise by using pytest
+====================================================================
+
+Parameterized testing: value matrix
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+:Sample Code:
+    .. code:: python
+
+        import pytest
+        from allpairspy import AllPairs
+
+        def function_to_be_tested(brand, operating_system, minute) -> bool:
+            # do something
+            return True
+
+        class TestParameterized(object):
+            @pytest.mark.parametrize(["brand", "operating_system", "minute"], [
+                values for values in AllPairs([
                     ["Brand X", "Brand Y"],
                     ["98", "NT", "2000", "XP"],
-                    ["Internal", "Modem"],
-                    ["Salaried", "Hourly", "Part-Time", "Contr."],
-                    [6, 10, 15, 30, 60],
-                ]
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Output:
-            .. code::
-        
-                PAIRWISE:
-                 0: ['Brand X', '98', 'Internal', 'Salaried', 6]
-                 1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
-                 2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
-                 3: ['Brand X', 'XP', 'Modem', 'Contr.', 10]
-                 4: ['Brand X', '2000', 'Modem', 'Part-Time', 15]
-                 5: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
-                 6: ['Brand Y', '98', 'Modem', 'Salaried', 30]
-                 7: ['Brand X', 'NT', 'Internal', 'Contr.', 30]
-                 8: ['Brand X', '98', 'Internal', 'Hourly', 60]
-                 9: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
-                10: ['Brand Y', 'NT', 'Modem', 'Salaried', 60]
-                11: ['Brand Y', 'XP', 'Modem', 'Part-Time', 60]
-                12: ['Brand Y', '2000', 'Modem', 'Hourly', 30]
-                13: ['Brand Y', '98', 'Modem', 'Contr.', 15]
-                14: ['Brand Y', 'XP', 'Modem', 'Salaried', 15]
-                15: ['Brand Y', 'NT', 'Modem', 'Part-Time', 15]
-                16: ['Brand Y', 'XP', 'Modem', 'Part-Time', 30]
-                17: ['Brand Y', '98', 'Modem', 'Part-Time', 6]
-                18: ['Brand Y', '2000', 'Modem', 'Salaried', 6]
-                19: ['Brand Y', '98', 'Modem', 'Salaried', 10]
-                20: ['Brand Y', 'XP', 'Modem', 'Contr.', 6]
-                21: ['Brand Y', 'NT', 'Modem', 'Hourly', 10]
-        
-        
-        Filtering
-        ==================
-        You can restrict pairs by setting filtering function to ``filter_func`` at
-        ``AllPairs`` constructor.
-        
-        :Sample Code:
-            .. code:: python
-        
-                from allpairspy import AllPairs
-        
-                def is_valid_combination(row):
-                    """
-                    This is a filtering function. Filtering functions should return True
-                    if combination is valid and False otherwise.
-        
-                    Test row that is passed here can be incomplete.
-                    To prevent search for unnecessary items filtering function
-                    is executed with found subset of data to validate it.
-                    """
-        
-                    n = len(row)
-        
-                    if n > 1:
-                        # Brand Y does not support Windows 98
-                        if "98" == row[1] and "Brand Y" == row[0]:
-                            return False
-        
-                        # Brand X does not work with XP
-                        if "XP" == row[1] and "Brand X" == row[0]:
-                            return False
-        
-                    if n > 4:
-                        # Contractors are billed in 30 min increments
-                        if "Contr." == row[3] and row[4] < 30:
-                            return False
-        
-                    return True
-        
-                parameters = [
-                    ["Brand X", "Brand Y"],
-                    ["98", "NT", "2000", "XP"],
-                    ["Internal", "Modem"],
-                    ["Salaried", "Hourly", "Part-Time", "Contr."],
-                    [6, 10, 15, 30, 60]
-                ]
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters, filter_func=is_valid_combination)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Output:
-            .. code::
-        
-                PAIRWISE:
-                 0: ['Brand X', '98', 'Internal', 'Salaried', 6]
-                 1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
-                 2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
-                 3: ['Brand X', '2000', 'Modem', 'Contr.', 30]
-                 4: ['Brand X', 'NT', 'Internal', 'Contr.', 60]
-                 5: ['Brand Y', 'XP', 'Modem', 'Salaried', 60]
-                 6: ['Brand X', '98', 'Modem', 'Part-Time', 15]
-                 7: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
-                 8: ['Brand Y', 'NT', 'Internal', 'Part-Time', 30]
-                 9: ['Brand X', '2000', 'Modem', 'Hourly', 10]
-                10: ['Brand Y', 'XP', 'Modem', 'Contr.', 30]
-                11: ['Brand Y', '2000', 'Modem', 'Salaried', 15]
-                12: ['Brand Y', 'NT', 'Modem', 'Salaried', 10]
-                13: ['Brand Y', 'XP', 'Modem', 'Part-Time', 6]
-                14: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
-        
-        
-        OrderedDict
-        ==================
-        You can use ``collections.OrderedDict`` instance as an argument for ``AllPairs`` constructor.
-        Pairs returned as ``collections.namedtuple`` instances.
-        
-        :Sample Code:
-            .. code:: python
-        
-                from collections import OrderedDict
-                from allpairspy import AllPairs
-        
-                parameters = OrderedDict({
-                    "brand": ["Brand X", "Brand Y"],
-                    "os": ["98", "NT", "2000", "XP"],
-                    "minute": [15, 30, 60],
-                })
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Sample Code:
-            .. code::
-        
-                PAIRWISE:
-                 0: Pairs(brand='Brand X', os='98', minute=15)
-                 1: Pairs(brand='Brand Y', os='NT', minute=15)
-                 2: Pairs(brand='Brand Y', os='2000', minute=30)
-                 3: Pairs(brand='Brand X', os='XP', minute=30)
-                 4: Pairs(brand='Brand X', os='2000', minute=60)
-                 5: Pairs(brand='Brand Y', os='XP', minute=60)
-                 6: Pairs(brand='Brand Y', os='98', minute=60)
-                 7: Pairs(brand='Brand X', os='NT', minute=60)
-                 8: Pairs(brand='Brand X', os='NT', minute=30)
-                 9: Pairs(brand='Brand X', os='98', minute=30)
-                10: Pairs(brand='Brand X', os='XP', minute=15)
-                11: Pairs(brand='Brand X', os='2000', minute=15)
-        
-        
-        Parameterized testing with pairwise by using py.test
-        ====================================================================
-        :Sample Code:
-            .. code:: python
-        
-                import pytest
-                from allpairspy import AllPairs
-        
-                def function_to_be_tested(brand, operating_system, minute):
-                    # do something
-                    return True
-        
-                class TestParameterized(object):
-        
-                    @pytest.mark.parametrize(["brand", "operating_system", "minute"], [
-                        value_list for value_list in AllPairs([
-                            ["Brand X", "Brand Y"],
-                            ["98", "NT", "2000", "XP"],
-                            [10, 15, 30, 60]
-                        ])
-                    ])
-                    def test(self, brand, operating_system, minute):
-                        assert function_to_be_tested(brand, operating_system, minute)
-        
-        :Output:
-            .. code::
-        
-                $ py.test test_parameterize.py -v
-                ============================= test session starts ==============================
-                ...
-                collected 16 items
-        
-                test_parameterize.py::TestParameterized::test[Brand X-98-10] PASSED      [  6%]
-                test_parameterize.py::TestParameterized::test[Brand Y-NT-10] PASSED      [ 12%]
-                test_parameterize.py::TestParameterized::test[Brand Y-2000-15] PASSED    [ 18%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-15] PASSED      [ 25%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-30] PASSED    [ 31%]
-                test_parameterize.py::TestParameterized::test[Brand Y-XP-30] PASSED      [ 37%]
-                test_parameterize.py::TestParameterized::test[Brand Y-98-60] PASSED      [ 43%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-60] PASSED      [ 50%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-30] PASSED      [ 56%]
-                test_parameterize.py::TestParameterized::test[Brand X-98-30] PASSED      [ 62%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-60] PASSED      [ 68%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-60] PASSED    [ 75%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-10] PASSED    [ 81%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-10] PASSED      [ 87%]
-                test_parameterize.py::TestParameterized::test[Brand X-98-15] PASSED      [ 93%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-15] PASSED      [100%]
-        
-        
-        Other Examples
-        =================
-        Other examples could be found in `examples <https://github.com/thombashi/allpairspy/tree/master/examples>`__ directory.
-        
-        
-        Installation
-        ------------
-        
-        Install from PyPI
-        ==================================
-        ::
-        
-            pip install allpairspy
-        
-        Install from PPA (for Ubuntu)
-        ==================================
-        ::
-        
-            sudo add-apt-repository ppa:thombashi/ppa
-            sudo apt update
-            sudo apt install python3-allpairspy
-        
-        
-        Known issues
-        ------------
-        * Not optimal - there are tools that can create smaller set covering
-          all the pairs. However, they are missing some other important
-          features and/or do not integrate well with Python.
-        
-        * Lousy written filtering function may lead to full permutation of parameters.
-        
-        * Version 2.0 has become slower (a side-effect of introducing ability to produce n-wise combinations).
-        
-        Dependencies
-        ------------
-        Python 2.7+ or 3.5+
-        
-        - `six <https://pypi.org/project/six/>`__
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Provides-Extra: test
-Provides-Extra: release
-Provides-Extra: build
+                    [10, 15, 30, 60]
+                ])
+            ])
+            def test(self, brand, operating_system, minute):
+                assert function_to_be_tested(brand, operating_system, minute)
+
+:Output:
+    .. code::
+
+        $ py.test test_parameterize.py -v
+        ============================= test session starts ==============================
+        ...
+        collected 16 items
+
+        test_parameterize.py::TestParameterized::test[Brand X-98-10] PASSED      [  6%]
+        test_parameterize.py::TestParameterized::test[Brand Y-NT-10] PASSED      [ 12%]
+        test_parameterize.py::TestParameterized::test[Brand Y-2000-15] PASSED    [ 18%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-15] PASSED      [ 25%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-30] PASSED    [ 31%]
+        test_parameterize.py::TestParameterized::test[Brand Y-XP-30] PASSED      [ 37%]
+        test_parameterize.py::TestParameterized::test[Brand Y-98-60] PASSED      [ 43%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-60] PASSED      [ 50%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-30] PASSED      [ 56%]
+        test_parameterize.py::TestParameterized::test[Brand X-98-30] PASSED      [ 62%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-60] PASSED      [ 68%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-60] PASSED    [ 75%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-10] PASSED    [ 81%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-10] PASSED      [ 87%]
+        test_parameterize.py::TestParameterized::test[Brand X-98-15] PASSED      [ 93%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-15] PASSED      [100%]
+
+Parameterized testing: OrderedDict
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+:Sample Code:
+    .. code:: python
+
+        import pytest
+        from allpairspy import AllPairs
+
+        def function_to_be_tested(brand, operating_system, minute) -> bool:
+            # do something
+            return True
+
+        class TestParameterized(object):
+            @pytest.mark.parametrize(
+                ["pair"],
+                [
+                    [pair]
+                    for pair in AllPairs(
+                        OrderedDict(
+                            {
+                                "brand": ["Brand X", "Brand Y"],
+                                "operating_system": ["98", "NT", "2000", "XP"],
+                                "minute": [10, 15, 30, 60],
+                            }
+                        )
+                    )
+                ],
+            )
+            def test(self, pair):
+                assert function_to_be_tested(pair.brand, pair.operating_system, pair.minute)
+
+
+Other Examples
+=================
+Other examples could be found in `examples <https://github.com/thombashi/allpairspy/tree/master/examples>`__ directory.
+
+
+Installation
+------------
+
+Installation: pip
+==================================
+::
+
+    pip install allpairspy
+
+Installation: apt
+==================================
+You can install the package by ``apt`` via a Personal Package Archive (`PPA <https://launchpad.net/~thombashi/+archive/ubuntu/ppa>`__):
+
+::
+
+    sudo add-apt-repository ppa:thombashi/ppa
+    sudo apt update
+    sudo apt install python3-allpairspy
+
+
+Known issues
+------------
+* Not optimal - there are tools that can create smaller set covering
+  all the pairs. However, they are missing some other important
+  features and/or do not integrate well with Python.
+
+* Lousy written filtering function may lead to full permutation of parameters.
+
+* Version 2.0 has become slower (a side-effect of introducing ability to produce n-wise combinations).
+
+
+Dependencies
+------------
+Python 3.7+
+no external dependencies.
+
+
+Sponsors
+------------
+.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: Dmitry Belyaev (b4tman)
+.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+   :target: https://github.com/chasbecker
+   :alt: Charles Becker (chasbecker)
+.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: Arturi0
+
+`Become a sponsor <https://github.com/sponsors/thombashi>`__
```

### Comparing `allpairspy-2.5.0/allpairspy/allpairs.py` & `allpairspy-2.5.1/allpairspy/allpairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-# encoding: utf-8
-
 from collections import OrderedDict, namedtuple
-from functools import cmp_to_key
+from functools import cmp_to_key, reduce
 from itertools import combinations
 
-import six
-from six.moves import range, reduce
-
 from .pairs_storage import PairsStorage, key
 
 
-class Item(object):
+class Item:
     @property
     def id(self):
         return self.__item_id
 
     @property
     def value(self):
         return self.__value
@@ -44,15 +39,15 @@
 def cmp_item(lhs, rhs):
     if lhs.weights == rhs.weights:
         return 0
 
     return -1 if lhs.weights < rhs.weights else 1
 
 
-class AllPairs(object):
+class AllPairs:
     def __init__(self, parameters, filter_func=lambda x: True, previously_tested=None, n=2):
         """
         TODO: check that input arrays are:
             - (optional) has no duplicated values inside single array / or compress such values
         """
 
         if not previously_tested:
@@ -131,15 +126,15 @@
                     direction = -1
                     if i == 0:
                         raise StopIteration()
                     i += direction
                     continue
                 direction = 0
             else:
-                raise ValueError("next(): unknown 'direction' code '{}'".format(direction))
+                raise ValueError(f"next(): unknown 'direction' code '{direction}'")
 
             chosen_item_list[i] = self.__working_item_matrix[i][indexes[i]]
 
             if self.__filter_func(self.__get_values(chosen_item_list[: i + 1])):
                 assert direction > -1
                 direction = 1
             else:
@@ -156,15 +151,15 @@
             raise StopIteration()
 
         # replace returned array elements with real values and return it
         return self.__get_iteration_value(chosen_item_list)
 
     def __validate_parameter(self, value):
         if isinstance(value, OrderedDict):
-            for parameter_list in six.itervalues(value):
+            for parameter_list in value.values():
                 if not parameter_list:
                     raise ValueError("each parameter arrays must have at least one item")
 
             return
 
         if len(value) < 2:
             raise ValueError("must provide more than one option")
@@ -176,15 +171,15 @@
     def __resort_working_array(self, chosen_item_list, num):
         for item in self.__working_item_matrix[num]:
             data_node = self.__pairs.get_node_info(item)
 
             new_combs = [
                 # numbers of new combinations to be created if this item is
                 # appended to array
-                set([key(z) for z in combinations(chosen_item_list + [item], i + 1)])
+                {key(z) for z in combinations(chosen_item_list + [item], i + 1)}
                 - self.__pairs.get_combs()[i]
                 for i in range(0, self.__n)
             ]
 
             # weighting the node node that creates most of new pairs is the best
             weights = [-len(new_combs[-1])]
 
@@ -203,15 +198,15 @@
             item.set_weights(weights)
 
         self.__working_item_matrix[num].sort(key=cmp_to_key(cmp_item))
 
     def __get_working_item_matrix(self, parameter_matrix):
         return [
             [
-                Item("a{:d}v{:d}".format(param_idx, value_idx), value)
+                Item(f"a{param_idx:d}v{value_idx:d}", value)
                 for value_idx, value in enumerate(value_list)
             ]
             for param_idx, value_list in enumerate(parameter_matrix)
         ]
 
     @staticmethod
     def __get_values(item_list):
@@ -229,8 +224,8 @@
 
         return list(parameters)
 
     def __extract_value_matrix(self, parameters):
         if not self.__is_ordered_dict_param:
             return parameters
 
-        return [v for v in six.itervalues(parameters)]
+        return [v for v in parameters.values()]
```

### Comparing `allpairspy-2.5.0/allpairspy/pairs_storage.py` & `allpairspy-2.5.1/allpairspy/pairs_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# encoding: utf-8
-
 from itertools import combinations
 
-from six.moves import range
-
 
-class Node(object):
+class Node:
     @property
     def id(self):
         return self.__node_id
 
     @property
     def counter(self):
         return self.__counter
@@ -36,15 +32,15 @@
 
     key_value = tuple([x.id for x in items])
     key_cache[items] = key_value
 
     return key_value
 
 
-class PairsStorage(object):
+class PairsStorage:
     def __init__(self, n):
         self.__n = n
         self.__nodes = {}
         self.__combs_arr = [set() for _i in range(n)]
 
     def __len__(self):
         return len(self.__combs_arr[-1])
```

### Comparing `allpairspy-2.5.0/allpairspy.egg-info/PKG-INFO` & `allpairspy-2.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,330 +1,377 @@
 Metadata-Version: 2.1
 Name: allpairspy
-Version: 2.5.0
+Version: 2.5.1
 Summary: Pairwise test combinations generator
 Home-page: https://github.com/thombashi/allpairspy
 Author: MetaCommunications Engineering
 Author-email: metacomm@users.sourceforge.net
 Maintainer: Tsuyoshi Hombashi
 Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/allpairspy
 Project-URL: Tracker, https://github.com/thombashi/allpairspy/issues
-Description: .. contents:: **allpairspy** forked from `bayandin/allpairs <https://github.com/bayandin/allpairs>`__
-           :backlinks: top
-           :depth: 2
-        
-        .. image:: https://badge.fury.io/py/allpairspy.svg
-            :target: https://badge.fury.io/py/allpairspy
-            :alt: PyPI package version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/allpairspy.svg
-            :target: https://pypi.org/project/allpairspy
-            :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/travis/thombashi/allpairspy/master.svg?label=Linux/macOS%20CI
-            :target: https://travis-ci.org/thombashi/allpairspy
-            :alt: Linux/macOS CI status
-        
-        .. image:: https://img.shields.io/appveyor/ci/thombashi/allpairspy/master.svg?label=Windows%20CI
-            :target: https://ci.appveyor.com/project/thombashi/allpairspy
-            :alt: Windows CI status
-        
-        .. image:: https://coveralls.io/repos/github/thombashi/allpairspy/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/allpairspy?branch=master
-            :alt: Test coverage
-        
-        
-        AllPairs test combinations generator
-        ------------------------------------------------
-        AllPairs is an open source test combinations generator written in
-        Python, developed and maintained by MetaCommunications Engineering.
-        The generator allows one to create a set of tests using "pairwise
-        combinations" method, reducing a number of combinations of variables
-        into a lesser set that covers most situations.
-        
-        For more info on pairwise testing see http://www.pairwise.org.
-        
-        
-        Features
-        --------
-        * Produces good enough dataset.
-        * Pythonic, iterator-style enumeration interface.
-        * Allows to filter out "invalid" combinations during search for the next combination.
-        * Goes beyond pairs! If/when required can generate n-wise combinations.
-        
-        
-        Get Started
-        ---------------
-        
-        Basic Usage
-        ==================
-        :Sample Code:
-            .. code:: python
-        
-                from allpairspy import AllPairs
-        
-                parameters = [
-                    ["Brand X", "Brand Y"],
-                    ["98", "NT", "2000", "XP"],
-                    ["Internal", "Modem"],
-                    ["Salaried", "Hourly", "Part-Time", "Contr."],
-                    [6, 10, 15, 30, 60],
-                ]
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Output:
-            .. code::
-        
-                PAIRWISE:
-                 0: ['Brand X', '98', 'Internal', 'Salaried', 6]
-                 1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
-                 2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
-                 3: ['Brand X', 'XP', 'Modem', 'Contr.', 10]
-                 4: ['Brand X', '2000', 'Modem', 'Part-Time', 15]
-                 5: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
-                 6: ['Brand Y', '98', 'Modem', 'Salaried', 30]
-                 7: ['Brand X', 'NT', 'Internal', 'Contr.', 30]
-                 8: ['Brand X', '98', 'Internal', 'Hourly', 60]
-                 9: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
-                10: ['Brand Y', 'NT', 'Modem', 'Salaried', 60]
-                11: ['Brand Y', 'XP', 'Modem', 'Part-Time', 60]
-                12: ['Brand Y', '2000', 'Modem', 'Hourly', 30]
-                13: ['Brand Y', '98', 'Modem', 'Contr.', 15]
-                14: ['Brand Y', 'XP', 'Modem', 'Salaried', 15]
-                15: ['Brand Y', 'NT', 'Modem', 'Part-Time', 15]
-                16: ['Brand Y', 'XP', 'Modem', 'Part-Time', 30]
-                17: ['Brand Y', '98', 'Modem', 'Part-Time', 6]
-                18: ['Brand Y', '2000', 'Modem', 'Salaried', 6]
-                19: ['Brand Y', '98', 'Modem', 'Salaried', 10]
-                20: ['Brand Y', 'XP', 'Modem', 'Contr.', 6]
-                21: ['Brand Y', 'NT', 'Modem', 'Hourly', 10]
-        
-        
-        Filtering
-        ==================
-        You can restrict pairs by setting filtering function to ``filter_func`` at
-        ``AllPairs`` constructor.
-        
-        :Sample Code:
-            .. code:: python
-        
-                from allpairspy import AllPairs
-        
-                def is_valid_combination(row):
-                    """
-                    This is a filtering function. Filtering functions should return True
-                    if combination is valid and False otherwise.
-        
-                    Test row that is passed here can be incomplete.
-                    To prevent search for unnecessary items filtering function
-                    is executed with found subset of data to validate it.
-                    """
-        
-                    n = len(row)
-        
-                    if n > 1:
-                        # Brand Y does not support Windows 98
-                        if "98" == row[1] and "Brand Y" == row[0]:
-                            return False
-        
-                        # Brand X does not work with XP
-                        if "XP" == row[1] and "Brand X" == row[0]:
-                            return False
-        
-                    if n > 4:
-                        # Contractors are billed in 30 min increments
-                        if "Contr." == row[3] and row[4] < 30:
-                            return False
-        
-                    return True
-        
-                parameters = [
-                    ["Brand X", "Brand Y"],
-                    ["98", "NT", "2000", "XP"],
-                    ["Internal", "Modem"],
-                    ["Salaried", "Hourly", "Part-Time", "Contr."],
-                    [6, 10, 15, 30, 60]
-                ]
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters, filter_func=is_valid_combination)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Output:
-            .. code::
-        
-                PAIRWISE:
-                 0: ['Brand X', '98', 'Internal', 'Salaried', 6]
-                 1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
-                 2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
-                 3: ['Brand X', '2000', 'Modem', 'Contr.', 30]
-                 4: ['Brand X', 'NT', 'Internal', 'Contr.', 60]
-                 5: ['Brand Y', 'XP', 'Modem', 'Salaried', 60]
-                 6: ['Brand X', '98', 'Modem', 'Part-Time', 15]
-                 7: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
-                 8: ['Brand Y', 'NT', 'Internal', 'Part-Time', 30]
-                 9: ['Brand X', '2000', 'Modem', 'Hourly', 10]
-                10: ['Brand Y', 'XP', 'Modem', 'Contr.', 30]
-                11: ['Brand Y', '2000', 'Modem', 'Salaried', 15]
-                12: ['Brand Y', 'NT', 'Modem', 'Salaried', 10]
-                13: ['Brand Y', 'XP', 'Modem', 'Part-Time', 6]
-                14: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
-        
-        
-        OrderedDict
-        ==================
-        You can use ``collections.OrderedDict`` instance as an argument for ``AllPairs`` constructor.
-        Pairs returned as ``collections.namedtuple`` instances.
-        
-        :Sample Code:
-            .. code:: python
-        
-                from collections import OrderedDict
-                from allpairspy import AllPairs
-        
-                parameters = OrderedDict({
-                    "brand": ["Brand X", "Brand Y"],
-                    "os": ["98", "NT", "2000", "XP"],
-                    "minute": [15, 30, 60],
-                })
-        
-                print("PAIRWISE:")
-                for i, pairs in enumerate(AllPairs(parameters)):
-                    print("{:2d}: {}".format(i, pairs))
-        
-        :Sample Code:
-            .. code::
-        
-                PAIRWISE:
-                 0: Pairs(brand='Brand X', os='98', minute=15)
-                 1: Pairs(brand='Brand Y', os='NT', minute=15)
-                 2: Pairs(brand='Brand Y', os='2000', minute=30)
-                 3: Pairs(brand='Brand X', os='XP', minute=30)
-                 4: Pairs(brand='Brand X', os='2000', minute=60)
-                 5: Pairs(brand='Brand Y', os='XP', minute=60)
-                 6: Pairs(brand='Brand Y', os='98', minute=60)
-                 7: Pairs(brand='Brand X', os='NT', minute=60)
-                 8: Pairs(brand='Brand X', os='NT', minute=30)
-                 9: Pairs(brand='Brand X', os='98', minute=30)
-                10: Pairs(brand='Brand X', os='XP', minute=15)
-                11: Pairs(brand='Brand X', os='2000', minute=15)
-        
-        
-        Parameterized testing with pairwise by using py.test
-        ====================================================================
-        :Sample Code:
-            .. code:: python
-        
-                import pytest
-                from allpairspy import AllPairs
-        
-                def function_to_be_tested(brand, operating_system, minute):
-                    # do something
-                    return True
-        
-                class TestParameterized(object):
-        
-                    @pytest.mark.parametrize(["brand", "operating_system", "minute"], [
-                        value_list for value_list in AllPairs([
-                            ["Brand X", "Brand Y"],
-                            ["98", "NT", "2000", "XP"],
-                            [10, 15, 30, 60]
-                        ])
-                    ])
-                    def test(self, brand, operating_system, minute):
-                        assert function_to_be_tested(brand, operating_system, minute)
-        
-        :Output:
-            .. code::
-        
-                $ py.test test_parameterize.py -v
-                ============================= test session starts ==============================
-                ...
-                collected 16 items
-        
-                test_parameterize.py::TestParameterized::test[Brand X-98-10] PASSED      [  6%]
-                test_parameterize.py::TestParameterized::test[Brand Y-NT-10] PASSED      [ 12%]
-                test_parameterize.py::TestParameterized::test[Brand Y-2000-15] PASSED    [ 18%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-15] PASSED      [ 25%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-30] PASSED    [ 31%]
-                test_parameterize.py::TestParameterized::test[Brand Y-XP-30] PASSED      [ 37%]
-                test_parameterize.py::TestParameterized::test[Brand Y-98-60] PASSED      [ 43%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-60] PASSED      [ 50%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-30] PASSED      [ 56%]
-                test_parameterize.py::TestParameterized::test[Brand X-98-30] PASSED      [ 62%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-60] PASSED      [ 68%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-60] PASSED    [ 75%]
-                test_parameterize.py::TestParameterized::test[Brand X-2000-10] PASSED    [ 81%]
-                test_parameterize.py::TestParameterized::test[Brand X-XP-10] PASSED      [ 87%]
-                test_parameterize.py::TestParameterized::test[Brand X-98-15] PASSED      [ 93%]
-                test_parameterize.py::TestParameterized::test[Brand X-NT-15] PASSED      [100%]
-        
-        
-        Other Examples
-        =================
-        Other examples could be found in `examples <https://github.com/thombashi/allpairspy/tree/master/examples>`__ directory.
-        
-        
-        Installation
-        ------------
-        
-        Install from PyPI
-        ==================================
-        ::
-        
-            pip install allpairspy
-        
-        Install from PPA (for Ubuntu)
-        ==================================
-        ::
-        
-            sudo add-apt-repository ppa:thombashi/ppa
-            sudo apt update
-            sudo apt install python3-allpairspy
-        
-        
-        Known issues
-        ------------
-        * Not optimal - there are tools that can create smaller set covering
-          all the pairs. However, they are missing some other important
-          features and/or do not integrate well with Python.
-        
-        * Lousy written filtering function may lead to full permutation of parameters.
-        
-        * Version 2.0 has become slower (a side-effect of introducing ability to produce n-wise combinations).
-        
-        Dependencies
-        ------------
-        Python 2.7+ or 3.5+
-        
-        - `six <https://pypi.org/project/six/>`__
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: release
-Provides-Extra: build
+License-File: LICENSE.txt
+
+.. contents:: **allpairspy** forked from `bayandin/allpairs <https://github.com/bayandin/allpairs>`__
+   :backlinks: top
+   :depth: 2
+
+.. image:: https://badge.fury.io/py/allpairspy.svg
+    :target: https://badge.fury.io/py/allpairspy
+    :alt: PyPI package version
+
+.. image:: https://img.shields.io/pypi/pyversions/allpairspy.svg
+    :target: https://pypi.org/project/allpairspy
+    :alt: Supported Python versions
+
+.. image:: https://github.com/thombashi/allpairspy/workflows/Tests/badge.svg
+    :target: https://github.com/thombashi/allpairspy/actions?query=workflow%3ATests
+    :alt: Linux/macOS/Windows CI status
+
+.. image:: https://coveralls.io/repos/github/thombashi/allpairspy/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/allpairspy?branch=master
+    :alt: Test coverage
+
+
+AllPairs test combinations generator
+------------------------------------------------
+AllPairs is an open source test combinations generator written in
+Python, developed and maintained by MetaCommunications Engineering.
+The generator allows one to create a set of tests using "pairwise
+combinations" method, reducing a number of combinations of variables
+into a lesser set that covers most situations.
+
+For more info on pairwise testing see http://www.pairwise.org.
+
+
+Features
+--------
+* Produces good enough dataset.
+* Pythonic, iterator-style enumeration interface.
+* Allows to filter out "invalid" combinations during search for the next combination.
+* Goes beyond pairs! If/when required can generate n-wise combinations.
+
+
+Get Started
+---------------
+
+Basic Usage
+==================
+:Sample Code:
+    .. code:: python
+
+        from allpairspy import AllPairs
+
+        parameters = [
+            ["Brand X", "Brand Y"],
+            ["98", "NT", "2000", "XP"],
+            ["Internal", "Modem"],
+            ["Salaried", "Hourly", "Part-Time", "Contr."],
+            [6, 10, 15, 30, 60],
+        ]
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Output:
+    .. code::
+
+        PAIRWISE:
+         0: ['Brand X', '98', 'Internal', 'Salaried', 6]
+         1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
+         2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
+         3: ['Brand X', 'XP', 'Modem', 'Contr.', 10]
+         4: ['Brand X', '2000', 'Modem', 'Part-Time', 15]
+         5: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
+         6: ['Brand Y', '98', 'Modem', 'Salaried', 30]
+         7: ['Brand X', 'NT', 'Internal', 'Contr.', 30]
+         8: ['Brand X', '98', 'Internal', 'Hourly', 60]
+         9: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
+        10: ['Brand Y', 'NT', 'Modem', 'Salaried', 60]
+        11: ['Brand Y', 'XP', 'Modem', 'Part-Time', 60]
+        12: ['Brand Y', '2000', 'Modem', 'Hourly', 30]
+        13: ['Brand Y', '98', 'Modem', 'Contr.', 15]
+        14: ['Brand Y', 'XP', 'Modem', 'Salaried', 15]
+        15: ['Brand Y', 'NT', 'Modem', 'Part-Time', 15]
+        16: ['Brand Y', 'XP', 'Modem', 'Part-Time', 30]
+        17: ['Brand Y', '98', 'Modem', 'Part-Time', 6]
+        18: ['Brand Y', '2000', 'Modem', 'Salaried', 6]
+        19: ['Brand Y', '98', 'Modem', 'Salaried', 10]
+        20: ['Brand Y', 'XP', 'Modem', 'Contr.', 6]
+        21: ['Brand Y', 'NT', 'Modem', 'Hourly', 10]
+
+
+Filtering
+==================
+You can restrict pairs by setting a filtering function to ``filter_func`` at
+``AllPairs`` constructor.
+
+:Sample Code:
+    .. code:: python
+
+        from allpairspy import AllPairs
+
+        def is_valid_combination(row):
+            """
+            This is a filtering function. Filtering functions should return True
+            if combination is valid and False otherwise.
+
+            Test row that is passed here can be incomplete.
+            To prevent search for unnecessary items filtering function
+            is executed with found subset of data to validate it.
+            """
+
+            n = len(row)
+
+            if n > 1:
+                # Brand Y does not support Windows 98
+                if "98" == row[1] and "Brand Y" == row[0]:
+                    return False
+
+                # Brand X does not work with XP
+                if "XP" == row[1] and "Brand X" == row[0]:
+                    return False
+
+            if n > 4:
+                # Contractors are billed in 30 min increments
+                if "Contr." == row[3] and row[4] < 30:
+                    return False
+
+            return True
+
+        parameters = [
+            ["Brand X", "Brand Y"],
+            ["98", "NT", "2000", "XP"],
+            ["Internal", "Modem"],
+            ["Salaried", "Hourly", "Part-Time", "Contr."],
+            [6, 10, 15, 30, 60]
+        ]
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters, filter_func=is_valid_combination)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Output:
+    .. code::
+
+        PAIRWISE:
+         0: ['Brand X', '98', 'Internal', 'Salaried', 6]
+         1: ['Brand Y', 'NT', 'Modem', 'Hourly', 6]
+         2: ['Brand Y', '2000', 'Internal', 'Part-Time', 10]
+         3: ['Brand X', '2000', 'Modem', 'Contr.', 30]
+         4: ['Brand X', 'NT', 'Internal', 'Contr.', 60]
+         5: ['Brand Y', 'XP', 'Modem', 'Salaried', 60]
+         6: ['Brand X', '98', 'Modem', 'Part-Time', 15]
+         7: ['Brand Y', 'XP', 'Internal', 'Hourly', 15]
+         8: ['Brand Y', 'NT', 'Internal', 'Part-Time', 30]
+         9: ['Brand X', '2000', 'Modem', 'Hourly', 10]
+        10: ['Brand Y', 'XP', 'Modem', 'Contr.', 30]
+        11: ['Brand Y', '2000', 'Modem', 'Salaried', 15]
+        12: ['Brand Y', 'NT', 'Modem', 'Salaried', 10]
+        13: ['Brand Y', 'XP', 'Modem', 'Part-Time', 6]
+        14: ['Brand Y', '2000', 'Modem', 'Contr.', 60]
+
+
+Data Source: OrderedDict
+====================================
+You can use ``collections.OrderedDict`` instance as an argument for ``AllPairs`` constructor.
+Pairs will be returned as ``collections.namedtuple`` instances.
+
+:Sample Code:
+    .. code:: python
+
+        from collections import OrderedDict
+        from allpairspy import AllPairs
+
+        parameters = OrderedDict({
+            "brand": ["Brand X", "Brand Y"],
+            "os": ["98", "NT", "2000", "XP"],
+            "minute": [15, 30, 60],
+        })
+
+        print("PAIRWISE:")
+        for i, pairs in enumerate(AllPairs(parameters)):
+            print("{:2d}: {}".format(i, pairs))
+
+:Sample Code:
+    .. code::
+
+        PAIRWISE:
+         0: Pairs(brand='Brand X', os='98', minute=15)
+         1: Pairs(brand='Brand Y', os='NT', minute=15)
+         2: Pairs(brand='Brand Y', os='2000', minute=30)
+         3: Pairs(brand='Brand X', os='XP', minute=30)
+         4: Pairs(brand='Brand X', os='2000', minute=60)
+         5: Pairs(brand='Brand Y', os='XP', minute=60)
+         6: Pairs(brand='Brand Y', os='98', minute=60)
+         7: Pairs(brand='Brand X', os='NT', minute=60)
+         8: Pairs(brand='Brand X', os='NT', minute=30)
+         9: Pairs(brand='Brand X', os='98', minute=30)
+        10: Pairs(brand='Brand X', os='XP', minute=15)
+        11: Pairs(brand='Brand X', os='2000', minute=15)
+
+
+Parameterized testing pairwise by using pytest
+====================================================================
+
+Parameterized testing: value matrix
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+:Sample Code:
+    .. code:: python
+
+        import pytest
+        from allpairspy import AllPairs
+
+        def function_to_be_tested(brand, operating_system, minute) -> bool:
+            # do something
+            return True
+
+        class TestParameterized(object):
+            @pytest.mark.parametrize(["brand", "operating_system", "minute"], [
+                values for values in AllPairs([
+                    ["Brand X", "Brand Y"],
+                    ["98", "NT", "2000", "XP"],
+                    [10, 15, 30, 60]
+                ])
+            ])
+            def test(self, brand, operating_system, minute):
+                assert function_to_be_tested(brand, operating_system, minute)
+
+:Output:
+    .. code::
+
+        $ py.test test_parameterize.py -v
+        ============================= test session starts ==============================
+        ...
+        collected 16 items
+
+        test_parameterize.py::TestParameterized::test[Brand X-98-10] PASSED      [  6%]
+        test_parameterize.py::TestParameterized::test[Brand Y-NT-10] PASSED      [ 12%]
+        test_parameterize.py::TestParameterized::test[Brand Y-2000-15] PASSED    [ 18%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-15] PASSED      [ 25%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-30] PASSED    [ 31%]
+        test_parameterize.py::TestParameterized::test[Brand Y-XP-30] PASSED      [ 37%]
+        test_parameterize.py::TestParameterized::test[Brand Y-98-60] PASSED      [ 43%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-60] PASSED      [ 50%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-30] PASSED      [ 56%]
+        test_parameterize.py::TestParameterized::test[Brand X-98-30] PASSED      [ 62%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-60] PASSED      [ 68%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-60] PASSED    [ 75%]
+        test_parameterize.py::TestParameterized::test[Brand X-2000-10] PASSED    [ 81%]
+        test_parameterize.py::TestParameterized::test[Brand X-XP-10] PASSED      [ 87%]
+        test_parameterize.py::TestParameterized::test[Brand X-98-15] PASSED      [ 93%]
+        test_parameterize.py::TestParameterized::test[Brand X-NT-15] PASSED      [100%]
+
+Parameterized testing: OrderedDict
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+:Sample Code:
+    .. code:: python
+
+        import pytest
+        from allpairspy import AllPairs
+
+        def function_to_be_tested(brand, operating_system, minute) -> bool:
+            # do something
+            return True
+
+        class TestParameterized(object):
+            @pytest.mark.parametrize(
+                ["pair"],
+                [
+                    [pair]
+                    for pair in AllPairs(
+                        OrderedDict(
+                            {
+                                "brand": ["Brand X", "Brand Y"],
+                                "operating_system": ["98", "NT", "2000", "XP"],
+                                "minute": [10, 15, 30, 60],
+                            }
+                        )
+                    )
+                ],
+            )
+            def test(self, pair):
+                assert function_to_be_tested(pair.brand, pair.operating_system, pair.minute)
+
+
+Other Examples
+=================
+Other examples could be found in `examples <https://github.com/thombashi/allpairspy/tree/master/examples>`__ directory.
+
+
+Installation
+------------
+
+Installation: pip
+==================================
+::
+
+    pip install allpairspy
+
+Installation: apt
+==================================
+You can install the package by ``apt`` via a Personal Package Archive (`PPA <https://launchpad.net/~thombashi/+archive/ubuntu/ppa>`__):
+
+::
+
+    sudo add-apt-repository ppa:thombashi/ppa
+    sudo apt update
+    sudo apt install python3-allpairspy
+
+
+Known issues
+------------
+* Not optimal - there are tools that can create smaller set covering
+  all the pairs. However, they are missing some other important
+  features and/or do not integrate well with Python.
+
+* Lousy written filtering function may lead to full permutation of parameters.
+
+* Version 2.0 has become slower (a side-effect of introducing ability to produce n-wise combinations).
+
+
+Dependencies
+------------
+Python 3.7+
+no external dependencies.
+
+
+Sponsors
+------------
+.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: Dmitry Belyaev (b4tman)
+.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+   :target: https://github.com/chasbecker
+   :alt: Charles Becker (chasbecker)
+.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: Arturi0
+
+`Become a sponsor <https://github.com/sponsors/thombashi>`__
```

### Comparing `allpairspy-2.5.0/setup.py` & `allpairspy-2.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,79 @@
-# encoding: utf-8
-
-import io
 import os.path
-import sys
 
 import setuptools
 
 
 MODULE_NAME = "allpairspy"
-REPOSITORY_URL = "https://github.com/thombashi/{:s}".format(MODULE_NAME)
+REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 
 pkg_info = {}
 
 
-def need_pytest():
-    return set(["pytest", "test", "ptr"]).intersection(sys.argv)
-
-
 def get_release_command_class():
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
 
 with open(os.path.join(MODULE_NAME, "__version__.py")) as f:
     exec(f.read(), pkg_info)
 
-with io.open("README.rst", encoding="utf8") as fp:
+with open("README.rst", encoding="utf8") as fp:
     long_description = fp.read()
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     install_requires = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     tests_requires = [line.strip() for line in f if line.strip()]
 
-PYTEST_RUNNER_REQUIRES = ["pytest-runner"] if need_pytest() else []
-
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
-
     author=pkg_info["__author__"],
     author_email=pkg_info["__author_email__"],
     description="Pairwise test combinations generator",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     license=pkg_info["__license__"],
     maintainer=pkg_info["__maintainer__"],
     maintainer_email=pkg_info["__maintainer_email__"],
-    packages=setuptools.find_packages(exclude=["test*"]),
+    packages=setuptools.find_packages(exclude=["tests*"]),
     project_urls={
         "Source": REPOSITORY_URL,
-        "Tracker": "{:s}/issues".format(REPOSITORY_URL),
+        "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
+    python_requires=">=3.7",
     install_requires=install_requires,
-    setup_requires=PYTEST_RUNNER_REQUIRES,
-    tests_require=tests_requires,
-    extras_require={
-        "build": ["twine", "wheel"],
-        "release": ["releasecmd>=0.0.18,<0.1.0"],
-        "test": tests_requires,
-    },
-
+    extras_require={"test": tests_requires},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
-    cmdclass=get_release_command_class())
+    cmdclass=get_release_command_class(),
+)
```

### Comparing `allpairspy-2.5.0/test/test_allpairs.py` & `allpairspy-2.5.1/tests/test_allpairs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# encoding: utf-8
-
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 from collections import OrderedDict
 
 from allpairspy import AllPairs
 
 
-class Test_pairewise_OrderedDict(object):
+class Test_pairewise_OrderedDict:
     def test_normal(self):
         parameters = OrderedDict(
             {"brand": ["Brand X", "Brand Y"], "os": ["NT", "2000", "XP"], "minute": [15, 30, 60]}
         )
 
         for pairs in AllPairs(parameters):
             assert pairs.brand == "Brand X"
             assert pairs.os == "NT"
             assert pairs.minute == 15
             break
 
         assert len(list(AllPairs(parameters))) == 9
 
 
-class Test_pairewise_list(object):
+class Test_pairewise_list:
     # example1.1.py
 
     def test_normal(self):
         parameters = [
             ["Brand X", "Brand Y"],
             ["98", "NT", "2000", "XP"],
             ["Internal", "Modem"],
@@ -58,15 +56,15 @@
             ["Brand Y", "2000", "Modem", "Salaried", 6],
             ["Brand Y", "98", "Modem", "Salaried", 10],
             ["Brand Y", "XP", "Modem", "Contr.", 6],
             ["Brand Y", "NT", "Modem", "Hourly", 10],
         ]
 
 
-class Test_triplewise(object):
+class Test_triplewise:
     # example1.2.py
 
     def test_normal(self):
         parameters = [
             ["Brand X", "Brand Y"],
             ["98", "NT", "2000", "XP"],
             ["Internal", "Modem"],
@@ -101,15 +99,15 @@
             ["Brand Y", "NT", "Modem", "Hourly", 15],
             ["Brand Y", "NT", "Modem", "Hourly", 30],
             ["Brand Y", "NT", "Modem", "Hourly", 60],
             ["Brand Y", "NT", "Modem", "Hourly", 10],
         ]
 
 
-class Test_pairewise_w_tested(object):
+class Test_pairewise_w_tested:
     # example1.3.py
 
     def test_normal(self):
         parameters = [
             ["Brand X", "Brand Y"],
             ["98", "NT", "2000", "XP"],
             ["Internal", "Modem"],
@@ -142,15 +140,15 @@
             ["Brand Y", "NT", "Modem", "Salaried", 30],
             ["Brand Y", "NT", "Modem", "Salaried", 15],
             ["Brand Y", "NT", "Modem", "Hourly", 6],
             ["Brand Y", "NT", "Modem", "Contr.", 60],
         ]
 
 
-class Test_pairewise_filter(object):
+class Test_pairewise_filter:
     def test_normal_example21(self):
         # example2.1.py
 
         parameters = [
             ["Brand X", "Brand Y"],
             ["98", "NT", "2000", "XP"],
             ["Internal", "Modem"],
@@ -208,15 +206,14 @@
             ("os", ["98", "NT", "2000", "XP"]),
             ("network", ["Internal", "Modem"]),
             ("employee", ["Salaried", "Hourly", "Part-Time", "Contr."]),
             ("increment", [6, 10, 15, 30, 60]),
         ]
 
         def is_valid_combination(values, names):
-
             dictionary = dict(zip(names, values))
 
             """
             Should return True if combination is valid and False otherwise.
 
             Dictionary that is passed here can be incomplete.
             To prevent search for unnecessary items filtering function
```

