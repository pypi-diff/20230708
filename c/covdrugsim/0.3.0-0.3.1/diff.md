# Comparing `tmp/covdrugsim-0.3.0.tar.gz` & `tmp/covdrugsim-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-0.3.0.tar", max compression
+gzip compressed data, was "covdrugsim-0.3.1.tar", max compression
```

## Comparing `covdrugsim-0.3.0.tar` & `covdrugsim-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-07-07 07:09:55.192971 covdrugsim-0.3.0/LICENSE
--rw-r--r--   0        0        0     6643 2023-07-07 07:09:55.192971 covdrugsim-0.3.0/README.md
--rw-r--r--   0        0        0     1956 2023-07-07 07:10:34.870719 covdrugsim-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      733 2023-07-07 07:10:34.870719 covdrugsim-0.3.0/setup.py
--rw-r--r--   0        0        0     1410 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/__init__.py
--rw-r--r--   0        0        0      170 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/chargesExample.txt
--rw-r--r--   0        0        0     4449 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/energyLevellerExample.inp
--rw-r--r--   0        0        0      619 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz
--rw-r--r--   0        0        0      621 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz
--rw-r--r--   0        0        0      619 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz
--rw-r--r--   0        0        0      866 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/datasets.py
--rw-r--r--   0        0        0      241 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/main.py
--rw-r--r--   0        0        0     3839 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/SCbondDist.py
--rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/__init__.py
--rw-r--r--   0        0        0     8141 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/baseID.py
--rw-r--r--   0        0        0     6071 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/bbRMSD.py
--rw-r--r--   0        0        0      331 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/config.py
--rw-r--r--   0        0        0     3084 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/hbondAnalysis.py
--rw-r--r--   0        0        0     3917 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/ligDihedral.py
--rw-r--r--   0        0        0      769 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/mdAnalyse.py
--rw-r--r--   0        0        0     5644 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/mdsim/prepMTB.py
--rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/admin.py
--rw-r--r--   0        0        0     1324 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/constants.py
--rw-r--r--   0        0        0     9228 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/genScripts.py
--rw-r--r--   0        0        0     1605 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/gsub.sh
--rw-r--r--   0        0        0     4844 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/tabulate.py
--rw-r--r--   0        0        0     4270 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/unitConv.py
--rw-r--r--   0        0        0        0 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/__init__.py
--rw-r--r--   0        0        0    17951 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rw-r--r--   0        0        0    11782 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rw-r--r--   0        0        0    13749 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     4017 2023-07-07 07:09:55.196971 covdrugsim-0.3.0/tests/test_covdrugsim.py
--rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-08 03:11:28.406364 covdrugsim-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6643 2023-07-08 03:11:28.406364 covdrugsim-0.3.1/README.md
+-rw-r--r--   0        0        0     1956 2023-07-08 03:12:10.061024 covdrugsim-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      733 2023-07-08 03:12:10.061024 covdrugsim-0.3.1/setup.py
+-rw-r--r--   0        0        0     1410 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0      619 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz
+-rw-r--r--   0        0        0      621 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz
+-rw-r--r--   0        0        0      619 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz
+-rw-r--r--   0        0        0      866 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/admin.py
+-rw-r--r--   0        0        0     1324 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/constants.py
+-rw-r--r--   0        0        0     9228 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/genScripts.py
+-rw-r--r--   0        0        0     1605 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/gsub.sh
+-rw-r--r--   0        0        0     4958 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/tabulate.py
+-rw-r--r--   0        0        0     4270 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/unitConv.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     4017 2023-07-08 03:11:28.410364 covdrugsim-0.3.1/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.3.1/PKG-INFO
```

### Comparing `covdrugsim-0.3.0/LICENSE` & `covdrugsim-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/README.md` & `covdrugsim-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/pyproject.toml` & `covdrugsim-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "covdrugsim"
-version = "0.3.0"
+version = "0.3.1"
 description = "Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/covdrugsim"
 repository = "https://github.com/Jon-Ting/covdrugsim"
 documentation = "https://covdrugsim.readthedocs.io/en/latest/"
```

### Comparing `covdrugsim-0.3.0/setup.py` & `covdrugsim-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covdrugsim",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `covdrugsim-0.3.0/src/covdrugsim/__init__.py` & `covdrugsim-0.3.1/src/covdrugsim/__init__.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/data/energyLevellerExample.inp` & `covdrugsim-0.3.1/src/covdrugsim/data/energyLevellerExample.inp`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz` & `covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneE/but2eneE.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz` & `covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneEd/but2eneEd.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz` & `covdrugsim-0.3.1/src/covdrugsim/data/exampleXYZs/but2eneZ/but2eneZ.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/datasets.py` & `covdrugsim-0.3.1/src/covdrugsim/datasets.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/baseID.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/mdAnalyse.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/mdAnalyse.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-0.3.1/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/admin.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/admin.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/constants.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/constants.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/genScripts.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/genScripts.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/gsub.sh` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/gsub.sh`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/tabulate.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/tabulate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from os import listdir
 from os.path import isdir
 import re
 
 import pandas as pd
 
 
-def sortHuman(alist):
-    """Sort a given alist in a more 'human' way"""
-    convert = lambda text: float(text) if text.isdigit() else text
-    alphanum = lambda key: [convert(c) for c in re.split('([-+]?[0-9]*\.?[0-9]*)', key)]
-    alist.sort(key=alphanum)
-    return alist
+def sortNatural(targetList):
+    """Sort a given list in a more natural way."""
+    tryConvertNumeric = lambda text: float(text) if text.isdigit() else text
+    alphanum = lambda key: [tryConvertNumeric(c) for c in re.split('([-+]?[0-9]*\.?[0-9]*)', key)]
+    targetList.sort(key=alphanum)
+    return targetList
 
 
-def replaceMultiple(mainStr, toBeReplaced, newStr):
-    """Replace multiple strings of mainStr"""
-    for elem in toBeReplaced:
-        if elem in mainStr:
-            mainStr = mainStr.replace(elem, newStr)
-    return mainStr
+def replaceMultiple(str1, strsToReplace, str2):
+    """Replace multiple strings of str1 by str2."""
+    for strToReplace in strsToReplace:
+        if strToReplace in str1:
+            str1 = str1.replace(strToReplace, str2)
+    return str1
 
 
 def findVal(lineList, targetStr):
-    """Find the values of interest from Gaussian output files"""
+    """Find the values of interest from Gaussian output files."""
     val, isEnergy, isMethod = None, 'Energies' in targetStr[0] or 'Enthalpies' in targetStr[0], '%chk' in targetStr[0]
-    for i, string in enumerate(targetStr):
+    for string in targetStr:
         for j, line in enumerate(lineList):
             if string in line:
                 if isMethod:
                     valueInc = lineList[j - 2]
                     val = valueInc.split(' ')[2]; break
                 else:
                     valueInc = line.split(string)[-1].strip()
@@ -47,59 +47,61 @@
                             continue
     if val is None:
         raise Exception('Target string {0} not found!'.format(targetStr))
     # print(targetStr, val, lineList[-3])  # For debugging
     return val
 
 
-def writeToExcel(dir_path):
-    """Write a new Excel file tabulating the quantities of interest"""
-    methodList, titleList, moleculeList, conformerList, NImagList, ZList, EList, HList, GList, MP2List = [], [], [], [], [], [], [], [], [], []
+def writeToExcel(inputDirPath, verbose=False):
+    """
+    Tabulate the quantities of interest to an Excel document.
+    """
+    groups = [f for f in listdir(inputDirPath) if isdir('{0}/{1}'.format(inputDirPath, f))]
+
+    if verbose:
+        print("\n# Tabulating values of interest from Gaussian .out files to an Excel sheet...")
+        print("\n# Input directory:\n", inputDirPath, "\n\n# Groups:\n", groups, "\n")
+
+    methodList, nameList, moleculeList, moleculeList, NImagList, ZList, EList, HList, GList, MP2List = [], [], [], [], [], [], [], [], [], []
     varFillList = [methodList, NImagList, ZList, EList, HList, GList]
     keywordList = [['%chk'], ['NI', 'Im'], ['zero-point Energies'], ['HF'], ['thermal Enthalpies'], ['thermal Free Energies']]
-    for j, title in enumerate(groups):
-        conformerDir = '{0}/{1}'.format(inputDir, title)
-        print("Conformer:", title)
+    for name in groups:
+        moleculeDir = '{0}/{1}'.format(inputDirPath, name)
+        print("Molecule:", name)
         try:
-            with open('{0}/{1}.out'.format(conformerDir, title), 'r') as f:
+            with open('{0}/{1}.out'.format(moleculeDir, name), 'r') as f:
                 lineList = f.readlines()
                 lineList.reverse()
                 for i, varList in enumerate(varFillList):
                     val = findVal(lineList, keywordList[i])
                     varList.append(val)
-                titleList.append(title)
-                moleculeList.append(replace_multiple(title.split('c')[0].replace('_', ''), ['TR', 'TSS', 'TP'], ''))
-                conformerList.append('c' + title.split('c')[-1])
+                nameList.append(name)
+                moleculeList.append(replaceMultiple(name.split('c')[0].replace('_', ''), ['TR', 'TSS', 'TP'], ''))
+                moleculeList.append('c' + name.split('c')[-1])
         except FileNotFoundError:
-            print("{0}/{1}.out not found!".format(conformerDir, title))
+            print("{0}/{1}.out not found!".format(moleculeDir, name))
             continue
-    data = {'Method': methodList, 'Title': titleList, 'Molecule': moleculeList, 'Conformer': conformerList, 'NImag': NImagList,
+    data = {'Method': methodList, 'Name': nameList, 'Molecule': moleculeList, 'Molecule': moleculeList, 'NImag': NImagList,
            'Z (Hartree)': ZList, 'E (Hartree)': EList, 'H (Hartree)': HList, 'G (Hartree)': GList}
-    df = pd.DataFrame(data, columns=['Method', 'Title', 'Molecule', 'Conformer', 'NImag', 'Z (Hartree)', 'E (Hartree)', 'H (Hartree)', 'G (Hartree)'])
-    titleList = sortHuman(titleList)
-    sortedDF = df.set_index('Title').reindex(titleList).reset_index()
+    df = pd.DataFrame(data, columns=['Method', 'Name', 'Molecule', 'Molecule', 'NImag', 'Z (Hartree)', 'E (Hartree)', 'H (Hartree)', 'G (Hartree)'])
+    nameList = sortNatural(nameList)
+    sortedDF = df.set_index('Name').reindex(nameList).reset_index()
     print("# Sorted data frame:\n", sortedDF)
 
     print("# Writing to Excel sheet...")
-    # sortedDF.to_excel('{0}/Energies.xlsx'.format(inputDir), sheet_name='Sheet1')
-    writer = pd.ExcelWriter('{0}/Energies.xlsx'.format(inputDir), engine='xlsxwriter')
+    # sortedDF.to_excel('{0}/Energies.xlsx'.format(inputDirPath), sheet_name='Sheet1')
+    writer = pd.ExcelWriter('{0}/Energies.xlsx'.format(inputDirPath), engine='xlsxwriter')
     sortedDF.to_excel(writer, startrow=1, sheet_name='Sheet1', index=False)
     workbook = writer.book
     worksheet = writer.sheets['Sheet1']
     for i, col in enumerate(sortedDF.columns):
         column_len = sortedDF[col].astype(str).str.len().max()
         column_len = max(column_len, len(col)) + 2
         worksheet.set_column(i, i, column_len)
     writer.save()
     return workbook
 
 
 if __name__ == "__main__":
-
-    # Change this!
-    inputDir = "/User/kahochow/Desktop/Li_mechanism/Li_work/Reactant"
-
-    groups = [f for f in listdir(inputDir) if isdir('{0}/{1}'.format(inputDir, f))]
-    print("\n# Tabulating values of interest from Gaussian .out files to an Excel sheet...")
-    print("\n# Input directory:\n", inputDir, "\n\n# Groups:\n", groups, "\n")
-    workbook = writeToExcel(inputDir)
+    inputDirPath = '/mnt/c/Users/ASUS/Documents/covdrugsim/src/covdrugsim/data/exampleXYZs'  # To be modified!
+    workbook = writeToExcel(inputDirPath, verbose=True)
```

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/unitConv.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/unitConv.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-0.3.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/tests/test_covdrugsim.py` & `covdrugsim-0.3.1/tests/test_covdrugsim.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.3.0/PKG-INFO` & `covdrugsim-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
 Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

