# Comparing `tmp/ElliptiCBn-1.0.4.tar.gz` & `tmp/ElliptiCBn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElliptiCBn-1.0.4.tar", last modified: Fri Jul  7 21:50:46 2023, max compression
+gzip compressed data, was "ElliptiCBn-1.0.5.tar", last modified: Fri Jul  7 22:25:06 2023, max compression
```

## Comparing `ElliptiCBn-1.0.4.tar` & `ElliptiCBn-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.789797 ElliptiCBn-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.774150 ElliptiCBn-1.0.4/ElliptiC/
--rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.4/ElliptiC/ElliptiC.py
--rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.4/ElliptiC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.786804 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/
--rw-rw-rw-   0        0        0     5393 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 21:50:46.000000 ElliptiCBn-1.0.4/ElliptiCBn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     5393 2023-07-07 21:50:46.789797 ElliptiCBn-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4621 2023-07-07 21:49:44.000000 ElliptiCBn-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 21:50:46.788798 ElliptiCBn-1.0.4/bin/
--rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.4/bin/ElliptiC
--rw-rw-rw-   0        0        0      780 2023-07-07 21:50:19.000000 ElliptiCBn-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 21:50:46.790799 ElliptiCBn-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-07-07 21:50:08.000000 ElliptiCBn-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:25:06.781208 ElliptiCBn-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-07 22:25:06.768208 ElliptiCBn-1.0.5/ElliptiC/
+-rw-rw-rw-   0        0        0    27466 2023-06-28 19:43:33.000000 ElliptiCBn-1.0.5/ElliptiC/ElliptiC.py
+-rw-rw-rw-   0        0        0       30 2023-06-28 19:22:14.000000 ElliptiCBn-1.0.5/ElliptiC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 22:25:06.778210 ElliptiCBn-1.0.5/ElliptiCBn.egg-info/
+-rw-rw-rw-   0        0        0     4719 2023-07-07 22:25:06.000000 ElliptiCBn-1.0.5/ElliptiCBn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-07 22:25:06.000000 ElliptiCBn-1.0.5/ElliptiCBn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 22:25:06.000000 ElliptiCBn-1.0.5/ElliptiCBn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 22:25:06.000000 ElliptiCBn-1.0.5/ElliptiCBn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-06-23 18:27:33.000000 ElliptiCBn-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4719 2023-07-07 22:25:06.781208 ElliptiCBn-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-07-07 22:24:48.000000 ElliptiCBn-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 22:25:06.779208 ElliptiCBn-1.0.5/bin/
+-rw-rw-rw-   0        0        0      899 2023-07-07 18:41:14.000000 ElliptiCBn-1.0.5/bin/ElliptiC
+-rw-rw-rw-   0        0        0      780 2023-07-07 22:22:28.000000 ElliptiCBn-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 22:25:06.781208 ElliptiCBn-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-07-07 22:22:48.000000 ElliptiCBn-1.0.5/setup.py
```

### Comparing `ElliptiCBn-1.0.4/ElliptiC/ElliptiC.py` & `ElliptiCBn-1.0.5/ElliptiC/ElliptiC.py`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.4/LICENSE` & `ElliptiCBn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.4/README.md` & `ElliptiCBn-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 <br />
 
 ## How to run the analysis
 ### The ElliptiC package takes a single command line argument: an xyz file containing atom coordinates, or a folder of xyz files containing atom coordinates
 
 **To run the analysis package on a single file, navigate to the directory with the ElliptiC script and execute it:**
 (NOTE: if there are spaces in your file name, you will need quotes around the file name)
-![](https://github.com/tensorbored/kds/raw/master/docs/_static/readme_lift.png)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/single_file.png)
 
 
 **The same convention can be used to execute the package on a folder of xyz files**
-![](https://raw.githubusercontent.com/mshavlik/ElliptiC/862682bad75f3521ff466b526dcaef7738487db8/images/folder_test.png?token=GHSAT0AAAAAACEFKZS2QDGUHV7PEO7TBJTYZFIQXHQ)
-
+![](https://github.com/harmslab/ElliptiC/raw/main/images/folder_test.png)
+    
 <br />
 
 ## How the package works
 ### Below is a diagram of the analysis steps the software completes on any given file
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/pipeline_image.svg?token=GHSAT0AAAAAACEFKZS2ML7WH5EZDFOIUJR4ZFIQYJQ)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/pipeline_image.svg)
 
 ### 1. In a given XYZ file, extract the coordinates of all carbon atoms (and oxygen atoms used later on in the analysis).
 ### 2. Identify strongly connected components to differentiate between host and guest structures.
 ### 3. Remove the guest structure since we only care about calculating ellipticity of the host.
 ### 4. Using proximity to oxygen atoms, remove the top and bottom rings of the hosts for accurate ellipticity calculation.
 ### 5 & 6. Using a Principal Components Analysis, calculate the variance along both major axes of the host ring. The ellipticity is thus (Vax1-Vax2)/Vax1 where Vax1 is the variance on the longest axis (length) and Vax2 is the variance on the second-longest axis (width). 
 ### 7. Output graphs of both the single ring hosts and the full host-guest structures, as well as a spreadsheet with the calculated ellipticity for each structure.
@@ -47,26 +47,26 @@
 ### Each xyz file analyzed with this package will produce at least 3 pieces of data: 
 * 1 interactive 3D scatter plot with all carbons in the CBn structures visualized 
 * 1 interactive 3D scatter plot with only the central carbon ring of the CBn structures visualized
 * 1 spreadsheet with all of the carbons, their positions, distance to the centroid of the structure, and the measured ellipticity
 
 **In the case of host CBn structures with an internally situated guest structure, an additional 3D graph will be produced with the guests visualized in the structures (see below)**
 
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/testing_cbn_interactive.png?token=GHSAT0AAAAAACEFKZS37M4B4NDDM6EVOAVSZFIQYTQ)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/testing_cbn_interactive.png)
 
 To see the interactive version of this plot that gets generated from the script, [Click Here](https://plotly.com/~Mshavlik/63/)
 
 **The user can visually see the ellipticity in the structues and compare them to the measured values in the spreadsheets:**                 
 _CB7 structures from above with guests removed_
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/CB7_circular.png?token=GHSAT0AAAAAACEFKZS36BNU4REKZRP5LHSWZFIQY3Q)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/CB7_circular.png)
 
 Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/circular_ellipticity.png?token=GHSAT0AAAAAACEFKZS3GCNVG7FRSYCCECIEZFIQZCA)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/circular_ellipticity.png)
 
 
 _CB10 wide structures with guests removed_
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/ellipsoid_example.png?token=GHSAT0AAAAAACEFKZS3LKCINOU2ZIQHSQE4ZFIQZKQ)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipsoid_example.png)
 
 Calculated ellipticity for each structure on a scale of circular (0) to linear (1)  
-![](https://raw.githubusercontent.com/harmslab/ElliptiC/4c68867b573e185b3b5dbf53601352d34d4580f1/images/ellipse_ellipticity.png?token=GHSAT0AAAAAACEFKZS2K7TV7B62MKVP35AGZFIQZRA)
+![](https://github.com/harmslab/ElliptiC/raw/main/images/ellipse_ellipticity.png)
```

### Comparing `ElliptiCBn-1.0.4/bin/ElliptiC` & `ElliptiCBn-1.0.5/bin/ElliptiC`

 * *Files identical despite different names*

### Comparing `ElliptiCBn-1.0.4/pyproject.toml` & `ElliptiCBn-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ElliptiCBn"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{name="Michael Shavlik", email="mshavlik@uoregon.edu"}]
 description = "Python package for analyzing Cucurbituril crystal structures automatically"
 readme = "README.md"
 requires-python = ">=3.7.0"
 classifiers = [
                   "Development Status :: 3 - Alpha",
                   "Intended Audience :: Science/Research",
```

### Comparing `ElliptiCBn-1.0.4/setup.py` & `ElliptiCBn-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 #Package meta-data
 DESCRIPTION= \
 """ Python package for analyzing CBn crystal structures automatically. """
 URL = "https://github.com/harmslab/ElliptiC"  # temp URL
 EMAIL = "mshavlik@uoregon.edu"
 AUTHOR = "Michael Shavlik"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import README for description
 with io.open(os.path.join(here,'README.md'),encoding='utf-8') as f:
     full_description = '\n' + f.read()
 
     
 # Now the part where we do setup
 setup(
     name='ElliptiCBn',
-    version='1.0.4',
+    version='1.0.5',
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=full_description,
     url=URL,
     license='MIT',
     packages=['ElliptiC'],
```

