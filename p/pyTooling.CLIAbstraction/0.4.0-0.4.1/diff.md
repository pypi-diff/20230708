# Comparing `tmp/pyTooling.CLIAbstraction-0.4.0.tar.gz` & `tmp/pyTooling.CLIAbstraction-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTooling.CLIAbstraction-0.4.0.tar", last modified: Wed Mar  2 10:49:10 2022, max compression
+gzip compressed data, was "pyTooling.CLIAbstraction-0.4.1.tar", last modified: Fri Jul  7 22:18:23 2023, max compression
```

## Comparing `pyTooling.CLIAbstraction-0.4.0.tar` & `pyTooling.CLIAbstraction-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6334 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/pyTooling/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/
--rw-r--r--   0 runner    (1001) docker     (121)    22619 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Argument.py
--rw-r--r--   0 runner    (1001) docker     (121)     9175 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6806 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Command.py
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Flag.py
--rw-r--r--   0 runner    (1001) docker     (121)     8527 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (121)     7392 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (121)     8679 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedFlagList.py
--rw-r--r--   0 runner    (1001) docker     (121)     5593 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
--rw-r--r--   0 runner    (1001) docker     (121)    13673 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-03-02 10:49:09.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-02 10:49:10.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 10:49:09.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-02 10:49:10.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-02 10:49:10.000000 pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-02 10:49:10.072716 pyTooling.CLIAbstraction-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-03-02 10:48:59.000000 pyTooling.CLIAbstraction-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:18:23.331824 pyTooling.CLIAbstraction-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-07 22:18:23.331824 pyTooling.CLIAbstraction-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:18:23.327824 pyTooling.CLIAbstraction-0.4.1/pyTooling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:18:23.331824 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/
+-rw-r--r--   0 runner    (1001) docker     (123)    22619 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedFlagList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedTupleFlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:18:23.327824 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-07 22:18:23.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 22:18:23.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:18:23.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 22:18:23.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 22:18:23.000000 pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:18:23.331824 pyTooling.CLIAbstraction-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-07 22:18:14.000000 pyTooling.CLIAbstraction-0.4.1/setup.py
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/LICENSE.md` & `pyTooling.CLIAbstraction-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyTooling.CLIAbstraction-0.4.0/PKG-INFO` & `pyTooling.CLIAbstraction-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyTooling.CLIAbstraction
-Version: 0.4.0
+Version: 0.4.1
 Summary: Basic abstraction layer for executables.
 Home-page: https://GitHub.com/pyTooling/pyTooling.CLIAbstraction
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.CLIAbstraction
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.CLIAbstraction
 Project-URL: Issue Tracker, https://GitHub.com/pyTooling/pyTooling.CLIAbstraction/issues
 Keywords: abstract,executable,cli,cli arguments
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
@@ -138,9 +138,7 @@
 ## License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/README.md` & `pyTooling.CLIAbstraction-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Argument.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Argument.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/BooleanFlag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/BooleanFlag.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Command.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Command.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/Flag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/Flag.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/KeyValueFlag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/KeyValueFlag.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/OptionalValuedFlag.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedFlag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedFlag.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedFlagList.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedFlagList.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/ValuedTupleFlag.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling/CLIAbstraction/__init__.py` & `pyTooling.CLIAbstraction-0.4.1/pyTooling/CLIAbstraction/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2007-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
@@ -28,17 +28,17 @@
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Basic abstraction layer for executables."""
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
-__copyright__ = "2014-2022, Patrick Lehmann"
+__copyright__ = "2014-2023, Patrick Lehmann"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.4.0"
+__version__ =   "0.4.1"
 __keywords__ =  ["abstract", "executable", "cli", "cli arguments"]
 
 from pathlib              import Path
 from platform             import system
 from shutil               import which as shutil_which
 from subprocess           import (
 	Popen		as Subprocess_Popen,
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/PKG-INFO` & `pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyTooling.CLIAbstraction
-Version: 0.4.0
+Version: 0.4.1
 Summary: Basic abstraction layer for executables.
 Home-page: https://GitHub.com/pyTooling/pyTooling.CLIAbstraction
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.CLIAbstraction
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.CLIAbstraction
 Project-URL: Issue Tracker, https://GitHub.com/pyTooling/pyTooling.CLIAbstraction/issues
 Keywords: abstract,executable,cli,cli arguments
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
@@ -138,9 +138,7 @@
 ## License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyTooling.CLIAbstraction.egg-info/SOURCES.txt` & `pyTooling.CLIAbstraction-0.4.1/pyTooling.CLIAbstraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTooling.CLIAbstraction-0.4.0/pyproject.toml` & `pyTooling.CLIAbstraction-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pyTooling >= 1.9.5",
+    "pyTooling >= 5.0.0",
     "setuptools >= 60.9.3",
-    "wheel >= 0.37.1"
+    "wheel >= 0.38.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.pytest.ini_options]
```

### Comparing `pyTooling.CLIAbstraction-0.4.0/setup.py` & `pyTooling.CLIAbstraction-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Boetzingen, Germany                                                            #
+# Copyright 2017-2023 Patrick Lehmann - Boetzingen, Germany                                                            #
 # Copyright 2014-2016 Technische Universität Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture     #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

