# Comparing `tmp/optical_dispersion_relations-0.2.0.tar.gz` & `tmp/optical_dispersion_relations-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optical_dispersion_relations-0.2.0.tar", last modified: Sat May  6 20:34:05 2023, max compression
+gzip compressed data, was "optical_dispersion_relations-0.3.0.tar", last modified: Sat Jul  8 00:13:40 2023, max compression
```

## Comparing `optical_dispersion_relations-0.2.0.tar` & `optical_dispersion_relations-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.825769 optical_dispersion_relations-0.2.0/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1071 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/LICENSE.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2100 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1565 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.817769 optical_dispersion_relations-0.2.0/optical_dispersion_relations/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4553 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/dielectric_waveguides.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5636 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/drude_lorentz.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3976 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/plasmon.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1342 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/utilities.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2100 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      623 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       14 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       29 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      714 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-06 20:34:05.825769 optical_dispersion_relations-0.2.0/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/test/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2185 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_dielectric_waveguide.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6848 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_drude_lorentz.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5902 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_plasmon.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2109 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_utilities.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-08 00:13:40.288656 optical_dispersion_relations-0.3.0/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1071 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/LICENSE.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2084 2023-07-08 00:13:40.284656 optical_dispersion_relations-0.3.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1549 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-08 00:13:40.280656 optical_dispersion_relations-0.3.0/optical_dispersion_relations/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4553 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations/dielectric_waveguides.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5615 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations/drude_lorentz.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7302 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations/plasmon.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1342 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations/utilities.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-08 00:13:40.284656 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2084 2023-07-08 00:13:40.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      623 2023-07-08 00:13:40.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-08 00:13:40.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       14 2023-07-08 00:13:40.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       29 2023-07-08 00:13:40.000000 optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      714 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-07-08 00:13:40.288656 optical_dispersion_relations-0.3.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-08 00:13:40.284656 optical_dispersion_relations-0.3.0/test/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2185 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/test/test_dielectric_waveguide.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6848 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/test/test_drude_lorentz.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9555 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/test/test_plasmon.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2109 2023-07-08 00:12:38.000000 optical_dispersion_relations-0.3.0/test/test_utilities.py
```

### Comparing `optical_dispersion_relations-0.2.0/LICENSE.txt` & `optical_dispersion_relations-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/optical_dispersion_relations/dielectric_waveguides.py` & `optical_dispersion_relations-0.3.0/optical_dispersion_relations/dielectric_waveguides.py`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/optical_dispersion_relations/drude_lorentz.py` & `optical_dispersion_relations-0.3.0/optical_dispersion_relations/drude_lorentz.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         'peak_position',
         'peak_strength',
     ])
 
     def __init__(self):
         self.poles = []
         self.dielectric_constant = 1
-        self.plasma_frequency = 0
+        self.plasma_frequency = 1
         self.angular_frequency = 0
 
     def with_dielectric_constant(self, dielectric_constant: float):
         """Paramerers
         ----------
         dielectric_constant: float, offset permittivity due to positive ion cores
 
@@ -72,15 +72,15 @@
         """
         self.angular_frequency = angular_frequency
         return self
 
     def permittivity(self):
         """Returns
         -------
-        The Drude-Lorentz dispersion relation as a function of angular frequency
+        Permittivity: float, the Drude-Lorentz permittivity
         """
         permittivity = self.dielectric_constant - self.plasma_frequency**2 * \
             sum(
                 pole.peak_strength *
                 lorentz_oscillator(self.angular_frequency,
                                    pole.peak_position, pole.damping_constant)
                 for pole in self.poles
```

### Comparing `optical_dispersion_relations-0.2.0/optical_dispersion_relations/utilities.py` & `optical_dispersion_relations-0.3.0/optical_dispersion_relations/utilities.py`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/SOURCES.txt` & `optical_dispersion_relations-0.3.0/optical_dispersion_relations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/pyproject.toml` & `optical_dispersion_relations-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["numpy>=1.23.4"]
 name = "optical_dispersion_relations"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="George Duffett" },
 ]
 description = "Optical Dispersion Relations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `optical_dispersion_relations-0.2.0/test/test_dielectric_waveguide.py` & `optical_dispersion_relations-0.3.0/test/test_dielectric_waveguide.py`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/test/test_drude_lorentz.py` & `optical_dispersion_relations-0.3.0/test/test_drude_lorentz.py`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.2.0/test/test_utilities.py` & `optical_dispersion_relations-0.3.0/test/test_utilities.py`

 * *Files identical despite different names*

