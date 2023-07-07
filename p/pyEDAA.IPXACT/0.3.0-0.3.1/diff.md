# Comparing `tmp/pyEDAA.IPXACT-0.3.0.tar.gz` & `tmp/pyEDAA.IPXACT-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEDAA.IPXACT-0.3.0.tar", last modified: Thu Mar 10 22:14:23 2022, max compression
+gzip compressed data, was "pyEDAA.IPXACT-0.3.1.tar", last modified: Fri Jul  7 23:09:10 2023, max compression
```

## Comparing `pyEDAA.IPXACT-0.3.0.tar` & `pyEDAA.IPXACT-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 22:14:23.633148 pyEDAA.IPXACT-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5356 2022-03-10 22:14:23.633148 pyEDAA.IPXACT-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4180 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 22:14:23.629148 pyEDAA.IPXACT-0.3.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 22:14:23.633148 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/
--rw-r--r--   0 runner    (1001) docker     (121)    10088 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)    12607 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Component.py
--rw-r--r--   0 runner    (1001) docker     (121)     7050 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Design.py
--rw-r--r--   0 runner    (1001) docker     (121)     6526 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/DesignConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/GeneratorChain.py
--rw-r--r--   0 runner    (1001) docker     (121)     8305 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 22:14:23.633148 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5356 2022-03-10 22:14:23.000000 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-03-10 22:14:23.000000 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 22:14:23.000000 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-03-10 22:14:23.000000 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-10 22:14:23.000000 pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-10 22:14:23.633148 pyEDAA.IPXACT-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-03-10 22:14:08.000000 pyEDAA.IPXACT-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:09:10.407868 pyEDAA.IPXACT-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-07 23:09:10.407868 pyEDAA.IPXACT-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:09:10.403868 pyEDAA.IPXACT-0.3.1/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:09:10.407868 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/DesignConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/GeneratorChain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:09:10.407868 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-07 23:09:10.000000 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 23:09:10.000000 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:09:10.000000 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-07 23:09:10.000000 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:09:10.000000 pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:09:10.407868 pyEDAA.IPXACT-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-07 23:09:01.000000 pyEDAA.IPXACT-0.3.1/setup.py
```

### Comparing `pyEDAA.IPXACT-0.3.0/LICENSE.md` & `pyEDAA.IPXACT-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.IPXACT-0.3.0/PKG-INFO` & `pyEDAA.IPXACT-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyEDAA.IPXACT
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Document-Object-Model (DOM) for IP-XACT files.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.IPXACT
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.IPXACT
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.IPXACT
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.IPXACT/issues
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
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
@@ -38,21 +38,18 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)  
 [![PyPI](https://img.shields.io/pypi/v/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyEDAA.IPXACT/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)  
 [![GitHub Workflow - Build and Test Status](https://img.shields.io/github/workflow/status/edaa-org/pyEDAA.IPXACT/Pipeline/main?longCache=true&style=flat-square&label=Build%20and%20Test&logo=GitHub%20Actions&logoColor=FFFFFF)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/actions/workflows/Pipeline.yml)
 [![Libraries.io status for latest release](https://img.shields.io/librariesio/release/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Libraries.io&logoColor=fff)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT)
 [![Codacy - Quality](https://img.shields.io/codacy/grade/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
-
-
-<!--
 [![Codacy - Coverage](https://img.shields.io/codacy/coverage/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
 [![Codecov - Branch Coverage](https://img.shields.io/codecov/c/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Codecov)](https://codecov.io/gh/edaa-org/pyEDAA.IPXACT)
 
-
+<!--
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=GitHub)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/network/dependents)
 [![Requires.io](https://img.shields.io/requires/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://requires.io/github/EDAA-ORG/pyEDAA.IPXACT/requirements/?branch=main)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT/sourcerank)
 -->
 
 An IP-XACT Document Object Model (DOM) for [IEEE 1685-2014][IEEE-1685-2014] written in Python.
 
@@ -85,9 +82,7 @@
 SPDX-License-Identifier: Apache-2.0
 
 
 [IEEE-1685-2009]: https://standards.ieee.org/findstds/standard/1685-2009.html
 [IEEE-1685-2014]: https://standards.ieee.org/findstds/standard/1685-2014.html
 [IPXACT]:         http://accellera.org/downloads/standards/ip-xact
 [Accellera]:      http://accellera.org
-
-
```

### Comparing `pyEDAA.IPXACT-0.3.0/README.md` & `pyEDAA.IPXACT-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,18 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)  
 [![PyPI](https://img.shields.io/pypi/v/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyEDAA.IPXACT/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)  
 [![GitHub Workflow - Build and Test Status](https://img.shields.io/github/workflow/status/edaa-org/pyEDAA.IPXACT/Pipeline/main?longCache=true&style=flat-square&label=Build%20and%20Test&logo=GitHub%20Actions&logoColor=FFFFFF)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/actions/workflows/Pipeline.yml)
 [![Libraries.io status for latest release](https://img.shields.io/librariesio/release/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Libraries.io&logoColor=fff)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT)
 [![Codacy - Quality](https://img.shields.io/codacy/grade/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
-
-
-<!--
 [![Codacy - Coverage](https://img.shields.io/codacy/coverage/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
 [![Codecov - Branch Coverage](https://img.shields.io/codecov/c/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Codecov)](https://codecov.io/gh/edaa-org/pyEDAA.IPXACT)
 
-
+<!--
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=GitHub)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/network/dependents)
 [![Requires.io](https://img.shields.io/requires/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://requires.io/github/EDAA-ORG/pyEDAA.IPXACT/requirements/?branch=main)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT/sourcerank)
 -->
 
 An IP-XACT Document Object Model (DOM) for [IEEE 1685-2014][IEEE-1685-2014] written in Python.
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Catalog.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Catalog.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
@@ -128,23 +128,23 @@
 	def FromFile(cls, filePath : Path):
 		"""Constructs an instance of ``Catalog`` from a file."""
 
 		if not filePath.exists():
 			raise PyIpxactException(f"File '{filePath}' not found.") from FileNotFoundError(str(filePath))
 
 		try:
-			with filePath.open(encoding="utf-8") as fileHandle:
+			with filePath.open("r", encoding="utf-8") as fileHandle:  # TODO: why not open in binary?
 				content = fileHandle.read()
 				content = bytes(bytearray(content, encoding='utf-8'))
 		except OSError as ex:
 			raise PyIpxactException("Couldn't open '{0!s}'.".format(filePath)) from ex
 
 		schemaPath = Path("../lib/schema/ieee-1685-2014/index.xsd")
 		try:
-			with schemaPath.open(encoding="utf-8") as fileHandle:
+			with schemaPath.open("r", encoding="utf-8") as fileHandle:  # TODO: why not opening as binary?
 				schema = fileHandle.read()
 				schema = bytes(bytearray(schema, encoding='utf-8'))
 		except OSError as ex:
 			raise PyIpxactException(f"Couldn't open '{schemaPath}'.") from ex
 
 		xmlParser = etree.XMLParser(remove_blank_text=True, encoding="utf-8")
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Component.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Component.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/Design.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/Design.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/DesignConfiguration.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/DesignConfiguration.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/GeneratorChain.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/GeneratorChain.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA/IPXACT/__init__.py` & `pyEDAA.IPXACT-0.3.1/pyEDAA/IPXACT/__init__.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
@@ -33,17 +33,17 @@
 from pathlib  import Path
 from textwrap import dedent
 
 from pyTooling.Decorators import export
 
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
-__copyright__ = "2016-2022, Patrick Lehmann"
+__copyright__ = "2016-2023, Patrick Lehmann"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.3.0"
+__version__ =   "0.3.1"
 
 
 @export
 class IpxactSchemaStruct:
 	"""Schema descriptor made of version, namespace prefix, URI, URL and local path."""
 
 	Version : str =         None    #: Schema version
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyEDAA.IPXACT.egg-info/PKG-INFO` & `pyEDAA.IPXACT-0.3.1/pyEDAA.IPXACT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyEDAA.IPXACT
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Document-Object-Model (DOM) for IP-XACT files.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.IPXACT
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.IPXACT
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.IPXACT
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.IPXACT/issues
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
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
@@ -38,21 +38,18 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)  
 [![PyPI](https://img.shields.io/pypi/v/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyEDAA.IPXACT/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)  
 [![GitHub Workflow - Build and Test Status](https://img.shields.io/github/workflow/status/edaa-org/pyEDAA.IPXACT/Pipeline/main?longCache=true&style=flat-square&label=Build%20and%20Test&logo=GitHub%20Actions&logoColor=FFFFFF)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/actions/workflows/Pipeline.yml)
 [![Libraries.io status for latest release](https://img.shields.io/librariesio/release/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Libraries.io&logoColor=fff)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT)
 [![Codacy - Quality](https://img.shields.io/codacy/grade/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
-
-
-<!--
 [![Codacy - Coverage](https://img.shields.io/codacy/coverage/c924eeffd4cc49ed9ebbbe3a89b6fa76?longCache=true&style=flat-square&logo=Codacy)](https://app.codacy.com/gh/edaa-org/pyEDAA.IPXACT)
 [![Codecov - Branch Coverage](https://img.shields.io/codecov/c/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=Codecov)](https://codecov.io/gh/edaa-org/pyEDAA.IPXACT)
 
-
+<!--
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square&logo=GitHub)](https://GitHub.com/edaa-org/pyEDAA.IPXACT/network/dependents)
 [![Requires.io](https://img.shields.io/requires/github/edaa-org/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://requires.io/github/EDAA-ORG/pyEDAA.IPXACT/requirements/?branch=main)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyEDAA.IPXACT?longCache=true&style=flat-square)](https://libraries.io/github/edaa-org/pyEDAA.IPXACT/sourcerank)
 -->
 
 An IP-XACT Document Object Model (DOM) for [IEEE 1685-2014][IEEE-1685-2014] written in Python.
 
@@ -85,9 +82,7 @@
 SPDX-License-Identifier: Apache-2.0
 
 
 [IEEE-1685-2009]: https://standards.ieee.org/findstds/standard/1685-2009.html
 [IEEE-1685-2014]: https://standards.ieee.org/findstds/standard/1685-2014.html
 [IPXACT]:         http://accellera.org/downloads/standards/ip-xact
 [Accellera]:      http://accellera.org
-
-
```

### Comparing `pyEDAA.IPXACT-0.3.0/pyproject.toml` & `pyEDAA.IPXACT-0.3.1/pyproject.toml`

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

### Comparing `pyEDAA.IPXACT-0.3.0/setup.py` & `pyEDAA.IPXACT-0.3.1/setup.py`

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
-# Copyright 2017-2022 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 # Copyright 2016-2016 Patrick Lehmann - Dresden, Germany                                                               #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
```

