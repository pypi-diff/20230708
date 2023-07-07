# Comparing `tmp/pyEDAA.ProjectModel-0.4.2.tar.gz` & `tmp/pyEDAA.ProjectModel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEDAA.ProjectModel-0.4.2.tar", last modified: Sun Jan 16 13:57:07 2022, max compression
+gzip compressed data, was "pyEDAA.ProjectModel-0.4.3.tar", last modified: Fri Jul  7 22:07:24 2023, max compression
```

## Comparing `pyEDAA.ProjectModel-0.4.2.tar` & `pyEDAA.ProjectModel-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     8914 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7567 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Altera/
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Altera/Quartus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Altera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3830 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/GHDL.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Intel/
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Intel/QuartusPrime.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Intel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/ModelSim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/QuestaSim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8420 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Verilog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/ISE.py
--rw-r--r--   0 runner    (1001) docker     (121)     8902 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/Vivado.py
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    45992 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8914 2022-01-16 13:57:07.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-01-16 13:57:07.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 13:57:07.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-01-16 13:57:07.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-16 13:57:07.000000 pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 13:57:07.637880 pyEDAA.ProjectModel-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-01-16 13:56:58.000000 pyEDAA.ProjectModel-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.488287 pyEDAA.ProjectModel-0.4.3/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Altera/
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Altera/Quartus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Altera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/GHDL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Intel/
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Intel/QuartusPrime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Intel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/ModelSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/QuestaSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/VHDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Verilog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/ISE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/Vivado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49365 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-07 22:07:24.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 22:07:24.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:07:24.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-07 22:07:24.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 22:07:24.000000 pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:07:24.492287 pyEDAA.ProjectModel-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-07 22:07:14.000000 pyEDAA.ProjectModel-0.4.3/setup.py
```

### Comparing `pyEDAA.ProjectModel-0.4.2/LICENSE.md` & `pyEDAA.ProjectModel-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/PKG-INFO` & `pyEDAA.ProjectModel-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pyEDAA.ProjectModel
-Version: 0.4.2
+Version: 0.4.3
 Summary: An abstract model of EDA tool projects.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.ProjectModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.ProjectModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.ProjectModel
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.ProjectModel/issues
 Keywords: eda project,model,abstract,xilinx,vivado,osvvm,file set,file group,test bench,test harness
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 <p align="center">
   <a title="edaa-org.github.io/pySVModel" href="https://edaa-org.github.io/pyEDAA.ProjectModel"><img height="80px" src="doc/_static/logo_on_dark.svg"/></a>
@@ -157,9 +156,7 @@
 # License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyEDAA.ProjectModel-0.4.2/README.md` & `pyEDAA.ProjectModel-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Altera/Quartus.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Altera/Quartus.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Altera/__init__.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Altera/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Attributes.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Attributes.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/GHDL.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/GHDL.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Intel/QuartusPrime.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Intel/QuartusPrime.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Intel/__init__.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Intel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/ModelSim.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/ModelSim.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/QuestaSim.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/QuestaSim.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/MentorGraphics/__init__.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/MentorGraphics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/OSVVM.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Verilog.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Verilog.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/ISE.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/ISE.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/Vivado.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/Vivado.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 # ==================================================================================================================== #
 #
 """Specific file types and attributes for Xilinx Vivado."""
 from pathlib import Path
 from typing import Iterable
 
 from xml.dom import minidom, Node
+
+from pyTooling.MetaClasses import ExtendedType
 from pyVHDLModel import VHDLVersion
 from pyTooling.Decorators import export
 
 from pyEDAA.ProjectModel import ProjectFile, XMLFile, XMLContent, SDCContent, Project, FileSet, Attribute, Design
 from pyEDAA.ProjectModel import File as Model_File
 from pyEDAA.ProjectModel import ConstraintFile as Model_ConstraintFile
 from pyEDAA.ProjectModel import VerilogSourceFile as Model_VerilogSourceFile
@@ -50,15 +52,15 @@
 
 
 @export
 class File(Model_File):
 	pass
 
 
-class VivadoFileMixIn:
+class VivadoFileMixIn(metaclass=ExtendedType, mixin=True):
 	def _registerAttributes(self):
 		self._attributes[UsedInAttribute] = []
 
 
 @export
 class ConstraintFile(Model_ConstraintFile, VivadoFileMixIn):
 	def _registerAttributes(self):
```

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/Xilinx/__init__.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/Xilinx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA/ProjectModel/__init__.py` & `pyEDAA.ProjectModel-0.4.3/pyEDAA/ProjectModel/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,24 +30,26 @@
 # ==================================================================================================================== #
 #
 """An abstract model of EDA tool projects."""
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2014-2022, Patrick Lehmann, Unai Martinez-Corral"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.4.2"
+__version__ =   "0.4.3"
 __keywords__ =  ["eda project", "model", "abstract", "xilinx", "vivado", "osvvm", "file set", "file group", "test bench", "test harness"]
 
 from os.path import relpath as path_relpath
 from pathlib import Path as pathlib_Path
 from typing  import Dict, Union, Optional as Nullable, List, Iterable, Generator, Tuple, Any as typing_Any, Type
 
-from pyTooling.Decorators import export
-from pySVModel            import VerilogVersion, SystemVerilogVersion
-from pyVHDLModel          import VHDLVersion
+from pyTooling.Decorators  import export
+from pyTooling.MetaClasses import ExtendedType
+from pyTooling.Graph       import Graph, Vertex
+from pySVModel             import VerilogVersion, SystemVerilogVersion
+from pyVHDLModel           import VHDLVersion
 
 
 @export
 class Attribute:
 	KEY: str
 	VALUE_TYPE: typing_Any
 
@@ -60,46 +62,46 @@
 		elif isinstance(obj, Design):
 			return obj._project[key]
 		else:
 			raise Exception("Resolution error")
 
 
 @export
-class FileType(type):
+class FileType(ExtendedType):
 	"""
 	A :term:`meta-class` to construct *FileType* classes.
 
 	Modifications done by this meta-class:
 	* Register all classes of type :class:`FileType` or derived variants in a class field :attr:`FileType.FileTypes` in this meta-class.
 	"""
 
 	FileTypes: Dict[str, 'FileType'] = {}     #: Dictionary of all classes of type :class:`FileType` or derived variants
 	Any: 'FileType'
 
 	def __init__(cls, name: str, bases: Tuple[type, ...], dictionary: Dict[str, typing_Any], **kwargs):
 		super().__init__(name, bases, dictionary, **kwargs)
 		cls.Any = cls
 
-	def __new__(cls, className, baseClasses, classMembers: Dict):
-		fileType = super().__new__(cls, className, baseClasses, classMembers)
+	def __new__(cls, className, baseClasses, classMembers: Dict, *args, **kwargs):
+		fileType = super().__new__(cls, className, baseClasses, classMembers, *args, **kwargs)
 		cls.FileTypes[className] = fileType
 		return fileType
 
 	def __getattr__(cls, item) -> 'FileType':
 		if item[:2] != "__" and item[-2:] != "__":
 			return cls.FileTypes[item]
 		else:
 			return super().__getattribute__(item)
 
 	def __contains__(cls, item) -> bool:
 		return issubclass(item, cls)
 
 
 @export
-class File(metaclass=FileType):
+class File(metaclass=FileType, slots=True):
 	"""
 	A :term:`File` represents a file in a design. This :term:`base-class` is used
 	for all derived file classes.
 
 	A file can be created standalone and later associated to a fileset, design and
 	project. Or a fileset, design and/or project can be associated immediately
 	while creating a file.
@@ -260,15 +262,15 @@
 		self._attributes[key] = value
 
 
 FileTypes = File
 
 
 @export
-class HumanReadableContent:
+class HumanReadableContent(metaclass=ExtendedType, mixin=True):
 	"""A file type representing human-readable contents."""
 
 
 @export
 class XMLContent(HumanReadableContent):
 	"""A file type representing XML contents."""
 
@@ -363,16 +365,35 @@
 
 	_vhdlLibrary: 'VHDLLibrary'
 	_vhdlVersion: VHDLVersion
 
 	def __init__(self, path: pathlib_Path, vhdlLibrary: Union[str, 'VHDLLibrary'] = None, vhdlVersion: VHDLVersion = None, project: 'Project' = None, design: 'Design' = None, fileSet: 'FileSet' = None):
 		super().__init__(path, project, design, fileSet)
 
-		# TODO: handle if vhdlLibrary is a string
-		self._vhdlLibrary = vhdlLibrary
+		if isinstance(vhdlLibrary, str):
+			if design is not None:
+				try:
+					vhdlLibrary = design.VHDLLibraries[vhdlLibrary]
+				except KeyError as ex:
+					raise Exception(f"VHDL library '{vhdlLibrary}' not found in design '{design.Name}'.") from ex
+			elif project is not None:
+				try:
+					vhdlLibrary = project.DefaultDesign.VHDLLibraries[vhdlLibrary]
+				except KeyError as ex:
+					raise Exception(f"VHDL library '{vhdlLibrary}' not found in default design '{project.DefaultDesign.Name}'.") from ex
+			else:
+				raise Exception(f"Can't lookup VHDL library because neither 'project' nor 'design' is given as a parameter.")
+		elif isinstance(vhdlLibrary, VHDLLibrary):
+			self._vhdlLibrary = vhdlLibrary
+			vhdlLibrary.AddFile(self)
+		elif vhdlLibrary is None:
+			self._vhdlLibrary = None
+		else:
+			raise TypeError(f"Parameter 'vhdlLibrary' is neither a 'str' nor 'VHDLibrary'.")
+
 		self._vhdlVersion = vhdlVersion
 
 	def Validate(self):
 		"""Validate this VHDL source file."""
 		super().Validate()
 
 		try:
@@ -409,14 +430,17 @@
 		else:
 			raise Exception("VHDLVersion was neither set locally nor globally.")
 
 	@VHDLVersion.setter
 	def VHDLVersion(self, value: VHDLVersion) -> None:
 		self._vhdlVersion = value
 
+	def __repr__(self) -> str:
+		return f"<VHDL file: '{self.ResolvedPath}'; lib: '{self.VHDLLibrary}'; version: {self.VHDLVersion}>"
+
 
 @export
 class VerilogSourceFile(HDLSourceFile, HumanReadableContent):
 	"""A Verilog source file (of any language version)."""
 
 	_verilogVersion: VerilogVersion
 
@@ -534,15 +558,15 @@
 
 @export
 class WaveformExchangeFile(File):
 	"""Base-class of all tool-independent waveform exchange files."""
 
 
 @export
-class FileSet:
+class FileSet(metaclass=ExtendedType, slots=True):
 	"""
 	A :term:`FileSet` represents a group of files. Filesets can have sub-filesets.
 
 	The order of insertion is preserved. A fileset can be created standalone and
 	later associated to another fileset, design and/or project. Or a fileset,
 	design and/or project can be associated immediately while creating the
 	fileset.
@@ -587,15 +611,16 @@
 		verilogVersion: VerilogVersion = None,
 		svVersion: SystemVerilogVersion = None
 	):
 		self._name =      name
 		self._topLevel =  topLevel
 		if project is not None:
 			self._project = project
-			self._design =  design
+			self._design =  design if design is not None else project.DefaultDesign
+
 		elif design is not None:
 			self._project = design._project
 			self._design =  design
 		else:
 			self._project = None
 			self._design =  None
 		self._directory = directory
@@ -731,15 +756,15 @@
 					yield file
 		else:
 			if isinstance(fileSet, str):
 				fileSetName = fileSet
 				try:
 					fileSet = self._fileSets[fileSetName]
 				except KeyError as ex:
-					raise Exception("Fileset {name} not bound to fileset {fileset}.".format(name=fileSetName, fileset=self.Name)) from ex
+					raise Exception(f"Fileset {fileSetName} not bound to fileset {self.Name}.") from ex
 			elif not isinstance(fileSet, FileSet):
 				raise TypeError("Parameter 'fileSet' is not of type 'str' or 'FileSet' nor value 'None'.")
 
 			for file in fileSet.Files(fileType):
 				yield file
 
 	def AddFile(self, file: File) -> None:
@@ -808,14 +833,18 @@
 	def __setitem__(self, key: Type[Attribute], value: typing_Any):
 		"""Index access for setting attributes on this file."""
 		self._attributes[key] = value
 
 	def GetOrCreateVHDLLibrary(self, name):
 		if name in self._vhdlLibraries:
 			return self._vhdlLibraries[name]
+		elif name in self._design._vhdlLibraries:
+			library = self._design._vhdlLibraries[name]
+			self._vhdlLibraries[name] = library
+			return library
 		else:
 			library = VHDLLibrary(name, design=self._design, vhdlVersion=self._vhdlVersion)
 			self._vhdlLibraries[name] = library
 			return library
 
 	@property
 	def VHDLLibrary(self) -> 'VHDLLibrary':
@@ -883,15 +912,15 @@
 
 	def __str__(self):
 		"""Returns the fileset's name."""
 		return self._name
 
 
 @export
-class VHDLLibrary:
+class VHDLLibrary(metaclass=ExtendedType, slots=True):
 	"""
 	A :term:`VHDLLibrary` represents a group of VHDL source files compiled into the same VHDL library.
 
 	:arg name:        The VHDL libraries' name.
 	:arg project:     Project the VHDL library is associated with.
 	:arg design:      Design the VHDL library is associated with.
 	:arg vhdlVersion: Default VHDL version for files in this VHDL library, if not specified for the file itself.
@@ -899,62 +928,102 @@
 
 	_name:        str
 	_project:     Nullable['Project']
 	_design:      Nullable['Design']
 	_files:       List[File]
 	_vhdlVersion: VHDLVersion
 
+	_dependencyNode: Vertex
+
 	def __init__(
 		self,
 		name: str,
 		project: 'Project' = None,
 		design: 'Design' = None,
 		vhdlVersion: VHDLVersion = None
 	):
 		self._name =    name
 		if project is not None:
 			self._project = project
-			self._design =  design
+			self._design = project._defaultDesign if design is None else design
+			self._dependencyNode = Vertex(value=self, graph=self._design._vhdlLibraryDependencyGraph)
+
+			if name in self._design._vhdlLibraries:
+				raise Exception(f"Library '{name}' already in design '{self._design.Name}'.")
+			else:
+				self._design._vhdlLibraries[name] = self
+
 		elif design is not None:
 			self._project = design._project
-			self._design =  design
+			self._design = design
+			self._dependencyNode = Vertex(value=self, graph=design._vhdlLibraryDependencyGraph)
+
+			if name in design._vhdlLibraries:
+				raise Exception(f"Library '{name}' already in design '{design.Name}'.")
+			else:
+				design._vhdlLibraries[name] = self
+
 		else:
 			self._project = None
 			self._design =  None
+			self._dependencyNode = None
+
 		self._files =     []
 		self._vhdlVersion = vhdlVersion
 
 	@property
 	def Name(self) -> str:
 		return self._name
 
 	@property
 	def Project(self) -> Nullable['Project']:
 		"""Property setting or returning the project this VHDL library is used in."""
 		return self._project
 
 	@Project.setter
 	def Project(self, value: 'Project'):
-		self._project = value
+		if not isinstance(value, Project):
+			raise TypeError("Parameter 'value' is not of type 'Project'.")
+
+		if value is None:
+			# TODO: unlink VHDLLibrary from project
+			self._project = None
+		else:
+			self._project = value
+			if self._design is None:
+				self._design = value._defaultDesign
 
 	@property
 	def Design(self) -> Nullable['Design']:
 		"""Property setting or returning the design this VHDL library is used in."""
 		return self._design
 
 	@Design.setter
 	def Design(self, value: 'Design'):
 		if not isinstance(value, Design):
-			raise TypeError("Parameter 'value' is not of type 'DesignModel.Design'.")
+			raise TypeError("Parameter 'value' is not of type 'Design'.")
 
-		self._design = value
-		if self._project is None:
-			self._project = value._project
-		elif self._project is not value._project:
-			raise Exception("The design's project is not identical to the already assigned project.")
+		if value is None:
+			# TODO: unlink VHDLLibrary from design
+			self._design = None
+		else:
+			if self._design is None:
+				self._design = value
+				self._dependencyNode = Vertex(value=self, graph=self._design._vhdlLibraryDependencyGraph)
+			elif self._design is not value:
+				# TODO: move VHDLLibrary to other design
+				# TODO: create new vertex in dependency graph and remove vertex from old graph
+				self._design = value
+			else:
+				pass
+
+			if self._project is None:
+				self._project = value._project
+			elif self._project is not value._project:
+				raise Exception("The design's project is not identical to the already assigned project.")
 
 	@property
 	def Files(self) -> Generator[File, None, None]:
 		"""Read-only property to return all files in this VHDL library."""
 		for file in self._files:
 			yield file
 
@@ -968,21 +1037,37 @@
 		else:
 			raise Exception("VHDLVersion is not set on VHDLLibrary nor parent object.")
 
 	@VHDLVersion.setter
 	def VHDLVersion(self, value: VHDLVersion) -> None:
 		self._vhdlVersion = value
 
+	def AddDependency(self, library: 'VHDLLibrary'):
+		library.parent = self
+
+	def AddFile(self, vhdlFile: VHDLSourceFile) -> None:
+		if not isinstance(vhdlFile, VHDLSourceFile):
+			raise TypeError(f"Parameter 'vhdlFile' is not a 'VHDLSourceFile'.")
+
+		self._files.append(vhdlFile)
+
+	def AddFiles(self, vhdlFiles: Iterable[VHDLSourceFile]) -> None:
+		for vhdlFile in vhdlFiles:
+			if not isinstance(vhdlFile, VHDLSourceFile):
+				raise TypeError(f"Item '{vhdlFile}' in parameter 'vhdlFiles' is not a 'VHDLSourceFile'.")
+
+			self._files.append(vhdlFile)
+
 	def __str__(self):
 		"""Returns the VHDL library's name."""
 		return self._name
 
 
 @export
-class Design:
+class Design(metaclass=ExtendedType, slots=True):
 	"""
 	A :term:`Design` represents a group of filesets and the source files therein.
 
 	Each design contains at least one fileset - the :term:`default fileset`. For
 	designs with VHDL source files, a independent `VHDLLibraries` overlay structure
 	exists.
 
@@ -1005,14 +1090,17 @@
 
 	_vhdlLibraries:         Dict[str, VHDLLibrary]
 	_vhdlVersion:           VHDLVersion
 	_verilogVersion:        VerilogVersion
 	_svVersion:             SystemVerilogVersion
 	_externalVHDLLibraries: List
 
+	_vhdlLibraryDependencyGraph: Graph
+	_fileDependencyGraph:        Graph
+
 	def __init__(
 		self,
 		name: str,
 		topLevel: str = None,
 		directory: pathlib_Path = pathlib_Path("."),
 		project: 'Project' = None,
 		vhdlVersion: VHDLVersion = None,
@@ -1030,14 +1118,17 @@
 		self._attributes =            {}
 		self._vhdlLibraries =         {}
 		self._vhdlVersion =           vhdlVersion
 		self._verilogVersion =        verilogVersion
 		self._svVersion =             svVersion
 		self._externalVHDLLibraries = []
 
+		self._vhdlLibraryDependencyGraph = Graph()
+		self._fileDependencyGraph = Graph()
+
 	@property
 	def Name(self) -> str:
 		"""Property setting or returning the design's name."""
 		return self._name
 
 	@Name.setter
 	def Name(self, value: str) -> None:
@@ -1092,20 +1183,20 @@
 		"""Property setting or returning the default fileset of this design."""
 		return self._defaultFileSet
 
 	@DefaultFileSet.setter
 	def DefaultFileSet(self, value: Union[str, FileSet]) -> None:
 		if isinstance(value, str):
 			if (value not in self._fileSets.keys()):
-				raise Exception("Fileset '{0}' is not in this design.".format(value))
+				raise Exception(f"Fileset '{value}' is not in this design.")
 
 			self._defaultFileSet = self._fileSets[value]
 		elif isinstance(value, FileSet):
 			if (value not in self.FileSets):
-				raise Exception("Fileset '{0}' is not associated to this design.".format(value))
+				raise Exception(f"Fileset '{value}' is not associated to this design.")
 
 			self._defaultFileSet = value
 		else:
 			raise ValueError("Unsupported parameter type for 'value'.")
 
 	# TODO: return generator with another method
 	@property
@@ -1125,15 +1216,15 @@
 				for file in fileSet.Files(fileType):
 					yield file
 		else:
 			if isinstance(fileSet, str):
 				try:
 					fileSet = self._fileSets[fileSet]
 				except KeyError as ex:
-					raise Exception("Fileset {name} not bound to design {design}.".format(name=fileSet.Name, design=self.Name)) from ex
+					raise Exception(f"Fileset {fileSet.Name} not bound to design {self.Name}.") from ex
 			elif not isinstance(fileSet, FileSet):
 				raise TypeError("Parameter 'fileSet' is not of type 'str' or 'FileSet' nor value 'None'.")
 
 			for file in fileSet.Files(fileType):
 				yield file
 
 	def Validate(self):
@@ -1177,16 +1268,16 @@
 		except KeyError:
 			return key.resolve(self, key)
 
 	def __setitem__(self, key: Type[Attribute], value: typing_Any):
 		self._attributes[key] = value
 
 	@property
-	def VHDLLibraries(self) -> List[VHDLLibrary]:
-		return self._vhdlLibraries.values()
+	def VHDLLibraries(self) -> Dict[str, VHDLLibrary]:
+		return self._vhdlLibraries
 
 	@property
 	def VHDLVersion(self) -> VHDLVersion:
 		if self._vhdlVersion is not None:
 			return self._vhdlVersion
 		elif self._project is not None:
 			return self._project.VHDLVersion
@@ -1229,28 +1320,28 @@
 
 	def AddFileSet(self, fileSet: FileSet) -> None:
 		if (not isinstance(fileSet, FileSet)):
 			raise ValueError("Parameter 'fileSet' is not of type ProjectModel.FileSet.")
 		elif (fileSet in self.FileSets):
 			raise Exception("Design already contains this fileSet.")
 		elif (fileSet.Name in self._fileSets.keys()):
-			raise Exception("Design already contains a fileset named '{0}'.".format(fileSet.Name))
+			raise Exception(f"Design already contains a fileset named '{fileSet.Name}'.")
 
 		fileSet.Design = self
 		self._fileSets[fileSet.Name] = fileSet
 
 	def AddFileSets(self, fileSets: Iterable[FileSet]) -> None:
 		for fileSet in fileSets:
 			self.AddFileSet(fileSet)
 
 	def AddFile(self, file: File) -> None:
 		if file.FileSet is None:
 			self._defaultFileSet.AddFile(file)
 		else:
-			raise ValueError("File '{file.Path!s}' is already part of fileset '{file.FileSet.Name}' and can't be assigned via Design to a default fileset.".format(file=file))
+			raise ValueError(f"File '{file.Path!s}' is already part of fileset '{file.FileSet.Name}' and can't be assigned via Design to a default fileset.")
 
 	def AddFiles(self, files: Iterable[File]) -> None:
 		for file in files:
 			self.AddFile(file)
 
 	def AddVHDLLibrary(self, vhdlLibrary: VHDLLibrary):
 		if vhdlLibrary.Name in self._vhdlLibraries:
@@ -1260,15 +1351,15 @@
 				raise Exception(f"A VHDLLibrary with same name ('{vhdlLibrary.Name}') already exists for this design.")
 
 	def __str__(self):
 		return self._name
 
 
 @export
-class Project:
+class Project(metaclass=ExtendedType, slots=True):
 	"""
 	A :term:`Project` represents a group of designs and the source files therein.
 
 	:arg name:            The project's name.
 	:arg rootDirectory:   Base-path to the project.
 	:arg vhdlVersion:     Default VHDL version for files in this project, if not specified for the file itself.
 	:arg verilogVersion:  Default Verilog version for files in this project, if not specified for the file itself.
```

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/PKG-INFO` & `pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pyEDAA.ProjectModel
-Version: 0.4.2
+Version: 0.4.3
 Summary: An abstract model of EDA tool projects.
 Home-page: https://GitHub.com/edaa-org/pyEDAA.ProjectModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pyEDAA.ProjectModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pyEDAA.ProjectModel
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pyEDAA.ProjectModel/issues
 Keywords: eda project,model,abstract,xilinx,vivado,osvvm,file set,file group,test bench,test harness
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 <p align="center">
   <a title="edaa-org.github.io/pySVModel" href="https://edaa-org.github.io/pyEDAA.ProjectModel"><img height="80px" src="doc/_static/logo_on_dark.svg"/></a>
@@ -157,9 +156,7 @@
 # License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pyEDAA.ProjectModel-0.4.2/pyEDAA.ProjectModel.egg-info/SOURCES.txt` & `pyEDAA.ProjectModel-0.4.3/pyEDAA.ProjectModel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyEDAA.ProjectModel.egg-info/SOURCES.txt
 pyEDAA.ProjectModel.egg-info/dependency_links.txt
 pyEDAA.ProjectModel.egg-info/requires.txt
 pyEDAA.ProjectModel.egg-info/top_level.txt
 pyEDAA/ProjectModel/Attributes.py
 pyEDAA/ProjectModel/GHDL.py
 pyEDAA/ProjectModel/OSVVM.py
+pyEDAA/ProjectModel/VHDL.py
 pyEDAA/ProjectModel/Verilog.py
 pyEDAA/ProjectModel/__init__.py
 pyEDAA/ProjectModel/Altera/Quartus.py
 pyEDAA/ProjectModel/Altera/__init__.py
 pyEDAA/ProjectModel/Intel/QuartusPrime.py
 pyEDAA/ProjectModel/Intel/__init__.py
 pyEDAA/ProjectModel/MentorGraphics/ModelSim.py
```

### Comparing `pyEDAA.ProjectModel-0.4.2/pyproject.toml` & `pyEDAA.ProjectModel-0.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pyTooling >= 1.9.2",
-    "setuptools >= 35.0.2",
-    "wheel >= 0.29.0"
+    "pyTooling >= 5.0.0",
+    "setuptools >= 60.9.3",
+    "wheel >= 0.38.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.pytest.ini_options]
```

### Comparing `pyEDAA.ProjectModel-0.4.2/setup.py` & `pyEDAA.ProjectModel-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,9 +40,11 @@
 
 DescribePythonPackageHostedOnGitHub(
 	packageName=packageName,
 	description="An abstract model of EDA tool projects.",
 	gitHubNamespace=gitHubNamespace,
 	sourceFileWithVersion=packageInformationFile,
 	developmentStatus="beta",
-	classifiers=list(DEFAULT_CLASSIFIERS) + ["Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)"]
+	classifiers=list(DEFAULT_CLASSIFIERS) + [
+		"Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)"
+	]
 )
```

