# Comparing `tmp/pyEDAA.CLITool-0.2.0.tar.gz` & `tmp/pyEDAA.CLITool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEDAA.CLITool-0.2.0.tar", last modified: Thu Mar 10 21:47:44 2022, max compression
+gzip compressed data, was "pyEDAA.CLITool-0.2.1.tar", last modified: Fri Jul  7 22:46:29 2023, max compression
```

## Comparing `pyEDAA.CLITool-0.2.0.tar` & `pyEDAA.CLITool-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.327055 pyEDAA.CLITool-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8033 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.319055 pyEDAA.CLITool-0.2.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/ActiveHDL.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/RivieraPRO.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Docker.py
--rw-r--r--   0 runner    (1001) docker     (121)    13208 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/GHDL.py
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/GTKWave.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/IntelFPGA/
--rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/IntelFPGA/Quartus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/IntelFPGA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Lattice/
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Lattice/Diamond.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Lattice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Mentor/
--rw-r--r--   0 runner    (1001) docker     (121)    10774 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Mentor/ModelSim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Mentor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/
--rw-r--r--   0 runner    (1001) docker     (121)     5841 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/ISE.py
--rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/Vivado.py
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 21:47:44.323055 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-03-10 21:47:44.000000 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-03-10 21:47:44.000000 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 21:47:44.000000 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-03-10 21:47:44.000000 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-10 21:47:44.000000 pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-10 21:47:44.327055 pyEDAA.CLITool-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-03-10 21:47:29.000000 pyEDAA.CLITool-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.469429 pyEDAA.CLITool-0.2.1/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/ActiveHDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/RivieraPRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/GHDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/GTKWave.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/IntelFPGA/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/IntelFPGA/Quartus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/IntelFPGA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Lattice/Diamond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Lattice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Mentor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Mentor/ModelSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Mentor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/ISE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/Vivado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:46:29.469429 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-07 22:46:29.000000 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 22:46:29.000000 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:46:29.000000 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 22:46:29.000000 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 22:46:29.000000 pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:46:29.473429 pyEDAA.CLITool-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-07 22:46:18.000000 pyEDAA.CLITool-0.2.1/setup.py
```

### Comparing `pyEDAA.CLITool-0.2.0/LICENSE.md` & `pyEDAA.CLITool-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.CLITool-0.2.0/PKG-INFO` & `pyEDAA.CLITool-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyEDAA.CLITool
-Version: 0.2.0
+Version: 0.2.1
 Summary: An abstraction layer of EDA CLI tools.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.CLITool
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.CLITool
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.CLITool
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.CLITool/issues
 Keywords: cli,abstraction layer,eda
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
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
 
@@ -168,9 +168,7 @@
 # License
 
 This Python package (source code) is licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 ---
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyEDAA.CLITool-0.2.0/README.md` & `pyEDAA.CLITool-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/ActiveHDL.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/ActiveHDL.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/RivieraPRO.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/RivieraPRO.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Aldec/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Aldec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Docker.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2021-2022 Patrick Lehmann - Boetzingen, Germany                                                            #
+# Copyright 2021-2023 Patrick Lehmann - Boetzingen, Germany                                                            #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
```

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/GHDL.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/GHDL.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/GTKWave.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/GTKWave.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/IntelFPGA/Quartus.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/IntelFPGA/Quartus.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/IntelFPGA/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/IntelFPGA/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Lattice/Diamond.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Lattice/Diamond.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Lattice/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Lattice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Mentor/ModelSim.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Mentor/ModelSim.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Mentor/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Mentor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/ISE.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/ISE.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/Vivado.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/Vivado.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/Xilinx/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/Xilinx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA/CLITool/__init__.py` & `pyEDAA.CLITool-0.2.1/pyEDAA/CLITool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2017-2022 Patrick Lehmann - Boetzingen, Germany                                                            #
+# Copyright 2017-2023 Patrick Lehmann - Boetzingen, Germany                                                            #
 # Copyright 2014-2016 Technische Universitaet Dresden - Germany, Chair of VLSI-Design, Diagnostics and Architecture    #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
@@ -28,11 +28,11 @@
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """An abstraction layer of EDA CLI tools."""
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
-__copyright__ = "2014-2022, Patrick Lehmann, Unai Martinez-Corral"
+__copyright__ = "2014-2023, Patrick Lehmann, Unai Martinez-Corral"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.2.0"
+__version__ =   "0.2.1"
 __keywords__ =  ["cli", "abstraction layer", "eda"]
```

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/PKG-INFO` & `pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyEDAA.CLITool
-Version: 0.2.0
+Version: 0.2.1
 Summary: An abstraction layer of EDA CLI tools.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.CLITool
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.CLITool
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.CLITool
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.CLITool/issues
 Keywords: cli,abstraction layer,eda
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
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
 
@@ -168,9 +168,7 @@
 # License
 
 This Python package (source code) is licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 ---
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyEDAA.CLITool-0.2.0/pyEDAA.CLITool.egg-info/SOURCES.txt` & `pyEDAA.CLITool-0.2.1/pyEDAA.CLITool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyEDAA.CLITool-0.2.0/pyproject.toml` & `pyEDAA.CLITool-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pyTooling >= 1.9.5",
+    "pyTooling >= 5.0.0",
     "setuptools >= 59.6.0",
-    "wheel >= 0.37.0"
+    "wheel >= 0.38.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.pytest.ini_options]
```

### Comparing `pyEDAA.CLITool-0.2.0/setup.py` & `pyEDAA.CLITool-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
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

