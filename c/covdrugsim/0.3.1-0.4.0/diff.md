# Comparing `tmp/covdrugsim-0.3.1.tar.gz` & `tmp/covdrugsim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-0.3.1.tar", max compression
+gzip compressed data, was "covdrugsim-0.4.0.tar", max compression
```

## Comparing `covdrugsim-0.3.1.tar` & `covdrugsim-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0     1082 2023-07-08 03:11:28.406364 covdrugsim-0.3.1/LICENSE
--rw-r--r--   0        0        0     6643 2023-07-08 03:11:28.406364 covdrugsim-0.3.1/README.md
--rw-r--r--   0        0        0     1956 2023-07-08 03:12:10.061024 covdrugsim-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      733 2023-07-08 03:12:10.061024 covdrugsim-0.3.1/setup.py
--rw-r--r--   0        0        0     1410 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/__init__.py
--rw-r--r--   0        0        0      170 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/chargesExample.txt
--rw-r--r--   0        0        0     4449 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/energyLevellerExample.inp
--rw-r--r--   0        0        0      619 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz
--rw-r--r--   0        0        0      621 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz
--rw-r--r--   0        0        0      619 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz
--rw-r--r--   0        0        0      866 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/datasets.py
--rw-r--r--   0        0        0      241 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/main.py
--rw-r--r--   0        0        0     3839 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/SCbondDist.py
--rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/__init__.py
--rw-r--r--   0        0        0     8141 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/baseID.py
--rw-r--r--   0        0        0     6071 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/bbRMSD.py
--rw-r--r--   0        0        0      331 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/config.py
--rw-r--r--   0        0        0     3084 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/hbondAnalysis.py
--rw-r--r--   0        0        0     3917 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/ligDihedral.py
--rw-r--r--   0        0        0      769 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/mdAnalyse.py
--rw-r--r--   0        0        0     5644 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/prepMTB.py
--rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/admin.py
--rw-r--r--   0        0        0     1324 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/constants.py
--rw-r--r--   0        0        0     9228 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/genScripts.py
--rw-r--r--   0        0        0     1605 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/gsub.sh
--rw-r--r--   0        0        0     4958 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/tabulate.py
--rw-r--r--   0        0        0     4270 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/unitConv.py
--rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/__init__.py
--rw-r--r--   0        0        0    17951 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rw-r--r--   0        0        0    11782 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rw-r--r--   0        0        0    13749 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     4017 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/tests/test_covdrugsim.py
--rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6643 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/README.md
+-rw-r--r--   0        0        0     1956 2023-07-08 08:02:59.773844 covdrugsim-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2023-07-08 08:02:59.773844 covdrugsim-0.4.0/setup.py
+-rw-r--r--   0        0        0     1410 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2023-07-08 08:02:16.425787 covdrugsim-0.4.0/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0   592600 2023-07-08 08:02:16.429787 covdrugsim-0.4.0/src/covdrugsim/data/exampleGaussianOutputs/example1.out
+-rw-r--r--   0        0        0   565812 2023-07-08 08:02:16.433786 covdrugsim-0.4.0/src/covdrugsim/data/exampleGaussianOutputs/example2.out
+-rw-r--r--   0        0        0  1069703 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/data/exampleGaussianOutputs/example3.out
+-rw-r--r--   0        0        0      984 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/data/exampleXYZs/example1.xyz
+-rw-r--r--   0        0        0      739 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/data/exampleXYZs/example2.xyz
+-rw-r--r--   0        0        0     1327 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/data/exampleXYZs/example3.xyz
+-rw-r--r--   0        0        0      866 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/admin.py
+-rw-r--r--   0        0        0     1324 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/constants.py
+-rw-r--r--   0        0        0    10364 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/genScripts.py
+-rw-r--r--   0        0        0     1605 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/gsub.sh
+-rw-r--r--   0        0        0     4958 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/tabulate.py
+-rw-r--r--   0        0        0     4280 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/unitConv.py
+-rw-r--r--   0        0        0        0 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     3882 2023-07-08 08:02:16.437787 covdrugsim-0.4.0/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.4.0/PKG-INFO
```

### Comparing `covdrugsim-0.3.1/LICENSE` & `covdrugsim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/README.md` & `covdrugsim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/pyproject.toml` & `covdrugsim-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "covdrugsim"
-version = "0.3.1"
+version = "0.4.0"
 description = "Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/covdrugsim"
 repository = "https://github.com/Jon-Ting/covdrugsim"
 documentation = "https://covdrugsim.readthedocs.io/en/latest/"
```

### Comparing `covdrugsim-0.3.1/setup.py` & `covdrugsim-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.3.1'
+__version__ = '0.4.0'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covdrugsim",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `covdrugsim-0.3.1/src/covdrugsim/__init__.py` & `covdrugsim-0.4.0/src/covdrugsim/__init__.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/data/energyLevellerExample.inp` & `covdrugsim-0.4.0/src/covdrugsim/data/energyLevellerExample.inp`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz` & `covdrugsim-0.4.0/src/covdrugsim/data/exampleXYZs/example2.xyz`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-12
-2-Butene, (E)-, ID: C624646
-C          1.07554        0.07724        0.08103
-C          0.34595        0.76890        0.96973
-C         -1.14733        0.78432        0.98955
-C          2.56882        0.06181        0.06122
-H          0.57785       -0.51698       -0.68246
-H          0.84364        1.36311        1.73322
-H         -1.57791        0.16627        0.19545
-H         -1.51078        1.80832        0.86043
-H         -1.51077        0.40770        1.95051
-H          2.99940        0.67985        0.85533
-H          2.93228        0.43841       -0.89973
-H          2.93226       -0.96220        0.19034
+15
+
+O         -2.79950        0.48220        0.15150
+N         -1.60800        0.39500        0.22230
+O         -0.86220        1.49300        0.51860
+O         -0.99980       -0.80220        0.00650
+C          0.30370       -0.58300       -0.53920
+C          1.14170        0.24740        0.45070
+C          2.54540        0.48340       -0.13690
+O          3.18500       -0.77540       -0.36380
+H          0.21840       -0.05420       -1.46540
+H          0.78230       -1.52490       -0.70900
+H          1.22700       -0.28140        1.37700
+H          0.66310        1.18920        0.62050
+H          3.12760        1.06040        0.55090
+H          2.46010        1.01220       -1.06320
+H          4.06010       -0.62820       -0.73010
```

### Comparing `covdrugsim-0.3.1/src/covdrugsim/datasets.py` & `covdrugsim-0.4.0/src/covdrugsim/datasets.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/baseID.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/mdAnalyse.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/mdAnalyse.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-0.4.0/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/constants.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 keywordDict = {
-    'GOVF': {'type': ' opt int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(8000), 'jobfs': int(2400), 'time': '10:00:00'},  # geometry optimization with vibrational frequency calculation
-    'TSGOVF': {'type': ' opt=(ts,calcfc,noeigentest,maxcyc=200) int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(4000), 'jobfs': int(4000), 'time': '10:00:00'},  # transition state GOVF
+    'GOVF': {'grid': ' opt int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(8000), 'jobfs': int(2400), 'time': '10:00:00'},  # geometry optimization with vibrational frequency calculation
+    'TSGOVF': {'grid': ' opt=(ts,calcfc,noeigentest,maxcyc=200) int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'mem': int(4000), 'jobfs': int(4000), 'time': '10:00:00'},  # transition state GOVF
 
-    'SPEXGO': {'type': '', 'time': '48:00:00', 'vmem': int(10000), 'ncpus': int(16)},  # single-point energy calculation without geometry optimization
-    'IRC': {'type': ' irc=(maxpoints=6,stepsize=10,calcfc,maxcyc=200)', 'time': '10:00:00'},  # intrinsic reaction coordinate calculation
-    'SPEiS': {'type': ' int(grid=ultrafine) scf=tight', 'freq': '', 'time': '07:00:00', 'mem': int(70000), 'jobfs': int(100000)},  # single-point energy calculation in solvent
-    'MO': {'type': ' gfinput iop(6/7=3)', 'time': '10:00:00'},  # print molecular orbitals for Molden display
-    'FBRGO': {'type': ' opt=modredundant int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'edit_charge': int(-1), 'time': '18:00:00', 'mem': int(4000), 'jobfs': int(4000)},  # freeze a bond, optimize the rest
-    'SBGO': {'type': ' opt=(z-matrix)'},  # stretch a bond, optimize for each point
+    'SPEXGO': {'grid': '', 'time': '48:00:00', 'vmem': int(10000), 'ncpus': int(16)},  # single-point energy calculation without geometry optimization
+    'IRC': {'grid': ' irc=(maxpoints=6,stepsize=10,calcfc,maxcyc=200)', 'time': '10:00:00'},  # intrinsic reaction coordinate calculation
+    'SPEiS': {'grid': ' int(grid=ultrafine) scf=tight', 'freq': '', 'time': '07:00:00', 'mem': int(70000), 'jobfs': int(100000)},  # single-point energy calculation in solvent
+    'MO': {'grid': ' gfinput iop(6/7=3)', 'time': '10:00:00'},  # print molecular orbitals for Molden display
+    'FBRGO': {'grid': ' opt=modredundant int(grid=ultrafine) scf=tight', 'freq': ' freq=noraman', 'edit_charge': int(-1), 'time': '18:00:00', 'mem': int(4000), 'jobfs': int(4000)},  # freeze a bond, optimize the rest
+    'SBGO': {'grid': ' opt=(z-matrix)'},  # stretch a bond, optimize for each point
     }
```

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/genScripts.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/genScripts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,137 +1,152 @@
 import os
 from os.path import isdir
 
 from covdrugsim.qmcalc.constants import keywordDict
+from covdrugsim.qmcalc.admin import groupFilesIntoDir
 
 
-def writeGaussInpFile(name, dirPath, 
-                      mem=8000, ncpus=8, 
-                      combination='B3LYP/6-31+G(d)', scrf=' scrf=(water,solvent=smd)', freq=' freq=noraman', 
-                      calcType='GOVF', charge=0, spin=1,
+def writeGaussInpFile(name, inpDirPath, 
+                      keywordLine=None, 
+                      mem=4000, ncpus=8, 
+                      combination=' m062x/6-311+g(d,p)', scrf=' scrf=(cpcm,solvent=water)', freq=' freq', grid=' opt=calcfc int(grid=ultrafine)', 
+                      charge=0, spin=1,
                       verbose=False):
     """
     Generate a Gaussian input file based on specified inputs.
 
     Parameters
     ----------
     name : str
         Name of the jobscript, also used for input and output file of the software to run.
-    dirPath : str
+    inpDirPath : str
         Directory path to store the jobscript.
     mem : Union[int,str]
         Amount of memory to request for the Gaussian job.
     ncpus : Union[int,str]
         Number of CPUs to request for the job.
     combination : str
         Keyword for DFT method and basis set specification in Gaussian.
     scrf : str
         Keyword for solvent specification in Gaussian.
     freq : str
         Keyword for force constant and resulting vibrational frequencies computation in Gaussian.
-    calcType : str
-        Type of calculation (e.g. 'GOVF' for normal geometry optimisation; 'TSGOVF' for transition state geometry optimisation, 
-        'SPEiS' for single point energy calculation, refer to 'keywordDict' for other options).
+    grid : str
+        Keyword for grid specification in Gaussian.
     charge : int
         Charge of the molecule (pay special attention if you have a transition state).
     spin : int
         Spin of the molecule.
+    verbose : bool
+        Whether to display details of the process.
     """
-    with open(f"{dirPath}/{name}.inp", 'w') as inpFile:
-        inpFile.write(f"%mem={mem}mb\n%nproc={ncpus}\n%chk={name}.chk\n")
-        inpFile.write(f"# {combination}{scrf}{calcType}{freq}")
+    with open(f"{inpDirPath}/{name}.inp", 'w') as inpFile:
+        inpFile.write(f"%mem={mem}mb\n%nprocshared={ncpus}\n%chk={name}.chk\n")
+        if keywordLine:
+            inpFile.write(keywordLine)
+        else:
+            inpFile.write(f"#{combination}{scrf}{grid}{freq}")
         inpFile.write(f"\n\n{name}\n\n{charge} {spin}\n")
-        with open(f"{dirPath}/{name}.xyz", 'r') as xyzFile:
+        with open(f"{inpDirPath}/{name}.xyz", 'r') as xyzFile:
             lineList = xyzFile.readlines()
-            hasEnergyName = 'Energy' in lineList[1] or 'TI' in lineList[1] or 'Name' in lineList[1]  # Potential bugs
+
+            # Couldn't recount why this was implemented, to be looked into
+            hasEnergyName = 'Energy' in lineList[1] or 'TI' in lineList[1] or 'Name' in lineList[1]
             hasPath = ':' in lineList[1]
             hasBlank = '\n' in lineList[1]
             for (i, line) in enumerate(lineList):
                 if hasEnergyName and (i > 1):
                     inpFile.write(line)
                 elif hasPath and (i > 1):
                     inpFile.write(f"\n{line}") if i == 2 else inpFile.write(line)
                 elif hasBlank and (i > 1):
                     inpFile.write(line)
-                elif not(hasEnergyName) and not(hasPath) and not(has_blank) and (i > 0):
+                elif not(hasEnergyName) and not(hasPath) and not(hasBlank) and (i > 0):
                     inpFile.write(line)
             inpFile.write('\n')
     if verbose:
-        print(f"    Generated Gaussian input file...")
+        print(f"    Generated Gaussian input file for {name}!")
 
 
-def writeHPCJobScript(name, dirPath='.', 
+def writeHPCJobScript(name, inpDirPath='.', 
                       scheduler='pbs', cluster='gadi', 
-                      ncpus=8, walltime='10:00:00', vmem=8000, jobfs=2400, software='g16', version='c01',
+                      ncpus=8, walltime='24:00:00', vmem=8000, jobfs=9000, project='p39', software='g16', version='c01',
                       verbose=False):
     """
     Generate a HPC jobscript based on specified inputs. 
 
     Parameters
     ----------
     name : str
         Name of the jobscript, also used for input and output file of the software to run.
-    dirPath : str
+    inpDirPath : str
         Directory path to store the jobscript.
     scheduler : str
         Scheduler to submit the job to.
     cluster : {'gadi', 'uq-rcc'}
         Cluster to run the job on.
     ncpus : Union[int,str]
         Number of CPUs to request for the job.
     walltime : str
         Wall time to request for the job.
     vmem : Union[int,str]
         Amount of memory to request for the HPC job.
     jobfs : Union[int,str]
         Amount of Jobfs memory to request for the job.
+    project : str
+        Project ID on NCI Gadi, only used if 'cluster' = 'gadi'.
     software : str
         Gaussian software name to use for the job.
     version : str
         Version of the Gaussian software.
+    verbose : bool
+        Whether to display details of the process.
     
     Notes
     -----
-    - If your HPC system does not use PBS jobscript modifications will be needed for the function.
+    - If your HPC system does not use PBS jobscript modifications will be needed for the function (open an issue on GitHub!).
     - Feel free to change the default values according to your most commonly used settings.
     """
-    with open(f"{dirPath}/{name}.sh", 'w') as f:
+    with open(f"{inpDirPath}/{name}.sh", 'w') as f:
         if scheduler == 'pbs':
             if cluster == 'gadi':
                 f.write('#!/bin/bash\n#PBS -l wd\n#PBS -q normal\n')
-                f.write(f"#PBS -l walltime={walltime},mem={vmem}mb,ncpus={ncpus},software={software},jobfs={jobfs}mb")
+                f.write(f"#PBS -l walltime={walltime},mem={vmem}mb,ncpus={ncpus},software={software},jobfs={jobfs}mb,storage=scratch/{project}")
                 f.write(f"\n\nmodule load gaussian/{software}{version}")
                 f.write(f"\n{software} < {name}.inp > {name}.out 2>&1")
             elif cluster == 'uq-rcc':
                 f.write(f"#!/bin/bash\n#PBS -S /bin/bash\n#PBS -l walltime={walltime}\n#PBS -A UQ-SCI-SCMB\n")
                 f.write(f"#PBS -l select=1:ncpus={ncpus}:mem={vmem}MB")
                 f.write('\n\ncd $PBS_O_WORKDIR')
                 f.write(f"\n\nmodule load gaussian/{software}-{version.upper()}-bash")
                 f.write(f"\n{software} < {name}.inp > {name}.out")
             else:
                 raise Exception(f"Cluster {cluster} not recognised/accommodated for yet!")
         else: 
             raise Exception(f"Scheduler {scheduler} not recognised/accommodated for yet!")
     if verbose:
-        print(f"    Generated HPC job script...")
+        print(f"    Generated HPC job script for {name}!")
 
 
-def genAllScripts(inputDirPath, 
-                  method='B3LYP', basisSet='6-31+G(d)', solvent='water', solventModel='smd',
-                  mem=8000, ncpus=8, calcType='GOVF', charge=0, spin=1, 
-                  scheduler='pbs', cluster='gadi', 
-                  walltime='10:00:00', vmem=8000, jobfs=2400, software='g16', version='c01',
+def genAllScripts(inpDirPath,
+                  keywordLine=None,
+                  method='m062x', basisSet='6-311+g(d,p)', solvent='water', solventModel='cpcm',
+                  mem=4000, ncpus=8, calcType='GOVF', charge=0, spin=1,
+                  scheduler='pbs', cluster='gadi',
+                  walltime='24:00:00', vmem=8000, jobfs=9000, project='p39', software='g16', version='c01',
                   verbose=False):
     """
-    Generate Gaussian input job files and submission files for molecules under all directories under a specified directory ('inputDirPath').
+    Generate Gaussian input job files and submission files for molecules under all directories under a specified directory ('inpDirPath').
 
     Parameters
     ----------
-    inputDirPath : str
+    inpDirPath : str
         Directory path to the input directories.
+    keywordLine : Union[str,None]
+        The line of keywords specification for Gaussian job, the other input arguments will be used to compose the line if it is not provided.
     method : str
         Keyword for DFT method specification in Gaussian.
     basisSet : str
         Keyword for basis set specification in Gaussian.
     solvent : str
         Keyword for solvent specification in Gaussian.
     solventModel : str
@@ -157,52 +172,68 @@
         Amount of memory to request for the HPC job.
     jobfs : Union[int,str]
         Amount of Jobfs memory to request for the job.
     software : str
         Gaussian software name to use for the job.
     version : str
         Version of the software.
+    verbose : bool
+        Whether to display details of the process.
 
     Notes
     -----
-    - Users should organise their directories such that a directory is created for each molecule to be calculated, and all of these directories should be placed under the specified directory that this function takes in ('inputDirPath')
+    - Users should organise their directories such that a directory is created for each molecule to be calculated, and all of these directories should be placed under the specified directory that this function takes in ('inpDirPath')
     """
     if verbose:
-        print(f"\nGenerating all job scripts for molecules under directories under {inputDirPath}...")
+        print(f"\nGenerating all job scripts for molecules under directories under {inpDirPath}...")
     assert calcType in keywordDict.keys(), 'Calculation type not known!'
-    molecules = [g for g in os.listdir(inputDirPath) if isdir(f"{inputDirPath}/{g}")]
+
+    molecules = [g for g in os.listdir(inpDirPath) if isdir(f"{inpDirPath}/{g}")]
+    if len(molecules) == 0:
+        groupFilesIntoDir(inpDirPath, verbose=verbose)
+        molecules = [g for g in os.listdir(inpDirPath) if isdir(f"{inpDirPath}/{g}")]
+
     for name in molecules:
         if verbose:
             print(f"  Processing {name}...")
-        moleculeDir = f"{inputDirPath}/{name}"
-        combination = f"{method}/{basisSet}"
-        scrf = f" scrf=({solvent},solvent={solventModel})"
+        moleculeDir = f"{inpDirPath}/{name}"
+        combination = f" {method}/{basisSet}"
+        scrf = f" scrf=({solventModel},solvent={solvent})"
+        freq = keywordDict[calcType]['freq']
+        grid = keywordDict[calcType]['grid']
         writeGaussInpFile(name, moleculeDir, 
-                          mem, ncpus, combination, keywordDict[calcType]['freq'], 
-                          scrf, keywordDict[calcType]['type'], charge, spin, 
+                          keywordLine, 
+                          mem, ncpus, 
+                          combination, freq, scrf, grid, charge, spin, 
                           verbose)
         writeHPCJobScript(name, moleculeDir, 
                           scheduler, cluster, 
-                          ncpus, walltime, vmem, jobfs, software, version,
+                          ncpus, walltime, vmem, jobfs, project, software, version,
                           verbose)
     if verbose:
-        print('  Generated all scripts.')
+        print('DONE -- Generated all scripts!\n')
 
 
 if __name__ == "__main__":
-    inputDirPath = '/mnt/c/Users/ASUS/Documents/covdrugsim/src/covdrugsim/data/exampleXYZs'  # To be modified!
-    method, basisSet = 'B3LYP', '6-31+G(d)'
-    solvent, solventModel = 'water', 'smd'
-    mem, ncpus = 8000, 8
+    # Test case
+    inpDirPath = '/mnt/c/Users/ASUS/Documents/covdrugsim/src/covdrugsim/data/exampleXYZs'
+
+    keywordLine = '# m062x/6-311+g(d,p) opt=calcfc freq scrf=(cpcm,solvent=water) int(grid=ultrafine)'
+
+    method, basisSet = 'm062x', '6-311+g(d,p)'
+    solvent, solventModel = 'water', 'cpcm'
+    mem, ncpus = 4000, 8
     calcType = 'GOVF'
     charge, spin = 0, 1
+
     scheduler, cluster = 'pbs', 'gadi'
-    walltime, vmem, jobfs = '12:00:00', 8000, 2400
+    walltime, vmem, jobfs, project = '24:00:00', 8000, 9000, 'p39'
     software, version = 'g16', 'c01'
-    verbose = True
 
-    genAllScripts(inputDirPath, 
+    genAllScripts(inpDirPath, 
+                  keywordLine,
                   method, basisSet, solvent, solventModel,
                   mem, ncpus, calcType, charge, spin,
                   scheduler, cluster,
-                  walltime, vmem, jobfs, software, version,
-                  verbose)
+                  walltime, vmem, jobfs, project, software, version,
+                  verbose=True)
+
```

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/gsub.sh` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/gsub.sh`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/tabulate.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/tabulate.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/unitConv.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/unitConv.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     E_kcal : float
         Energy (kcal).
     E_kJ : float
         Energy (kJ).
 
     Examples
     --------
-    >>> E_unit_conv(100, False, True)
+    >>> energyUnitsConversion(100, False, True)
     """
     if not(E_kcal):  # If no value is provided
         E_kcal = E_kJ/cal2J
     elif not(E_kJ):
         E_kJ = E_kcal*cal2J
     else:
         raise Exception("Both E_kcal & E_kJ are missing! Provide one.")
```

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-0.4.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.1/tests/test_covdrugsim.py` & `covdrugsim-0.4.0/tests/test_covdrugsim.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,62 +10,64 @@
 from covdrugsim.qmcalc.genScripts import genAllScripts
 from covdrugsim.qmcalc.admin import groupFilesIntoDir
 from covdrugsim.qmcalc.tabulate import writeToExcel
 from covdrugsim.qmcalc.unitConv import energyUnitsConversion, eyringEquation, timeUnitsConversion
 from covdrugsim.mdsim import mdAnalyse
 
 targetDirPath = 'tests/exampleXYZs'
-exampleXYZname = 'but2eneZ'
+exampleXYZname = 'example1'
 exampleXYZdirPath = f"{targetDirPath}/{exampleXYZname}"
 
 
 def test_genExampleXYZs():
+    """Unit test for genExampleXYZs()."""
     genExampleXYZs(targetDirPath)
     assert exists(targetDirPath), f"{targetDirPath} not found"
     assert isdir(targetDirPath), f"{targetDirPath} not a directory"
     assert len(listdir(targetDirPath)) == 3, f"Incorrect number of xyz files in {targetDirPath}"
 
 
 def test_getExampleEnergyLevellerInputPath():
+    """Unit test for genExampleEnergyLevellerInputPath()."""
     energyLevellerInputPathAct = getExampleEnergyLevellerInputPath()
     assert isinstance(energyLevellerInputPathAct, str), 'Path not a string'
 
 
 def test_getExampleChargePath():
+    """Unit test for genExampleChargePath()."""
     chargePathAct = getExampleChargePath()
     assert isinstance(chargePathAct, str), 'Path not a string'
 
 
-def test_genAllScripts():
-    genExampleXYZs(targetDirPath)
+def test_groupFilesIntoDir():
+    """Unit test for groupFilesIntoDir()."""
     groupFilesIntoDir(targetDirPath)
-    genAllScripts(targetDirPath, verbose=True)
+
+    assert exists(exampleXYZdirPath), f"{exampleXYZdirPath} not found"
+    assert isdir(exampleXYZdirPath), f"{exampleXYZdirPath} not a directory"
+
     assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.xyz"), f"{exampleXYZname}.xyz not found"
     assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.xyz"), f"{exampleXYZname}.xyz not a file"
-    assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.inp"), f"{exampleXYZname}.inp not found"
-    assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.inp"), f"{exampleXYZname}.inp not a file"
-    assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.sh"), f"{exampleXYZname}.sh not found"
-    assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.sh"), f"{exampleXYZname}.sh not a file"
 
+    assert len(listdir(targetDirPath)) == 3, f"Incorrect number of files in {exampleXYZdirPath}"
 
-def test_groupFilesIntoDir():
-    groupFilesIntoDir(targetDirPath)
+    if isdir(targetDirPath):
+        rmtree(targetDirPath)
 
-    assert exists(exampleXYZdirPath), f"{exampleXYZdirPath} not found"
-    assert isdir(exampleXYZdirPath), f"{exampleXYZdirPath} not a directory"
 
+def test_genAllScripts():
+    """Unit test for genAllScripts()."""
+    genExampleXYZs(targetDirPath)
+    genAllScripts(targetDirPath, verbose=True)
     assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.xyz"), f"{exampleXYZname}.xyz not found"
     assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.xyz"), f"{exampleXYZname}.xyz not a file"
     assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.inp"), f"{exampleXYZname}.inp not found"
     assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.inp"), f"{exampleXYZname}.inp not a file"
     assert exists(f"{exampleXYZdirPath}/{exampleXYZname}.sh"), f"{exampleXYZname}.sh not found"
     assert isfile(f"{exampleXYZdirPath}/{exampleXYZname}.sh"), f"{exampleXYZname}.sh not a file"
-
-    assert len(listdir(exampleXYZdirPath)) == 3, f"Incorrect number of files in {exampleXYZdirPath}"
-
     if isdir(targetDirPath):
         rmtree(targetDirPath)
 
 
 def test_energyUnitsConversion():
     assert energyUnitsConversion(100, None) == approx((100, 418.40000000000003))
```

### Comparing `covdrugsim-0.3.1/PKG-INFO` & `covdrugsim-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 0.3.1
+Version: 0.4.0
 Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
 Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

