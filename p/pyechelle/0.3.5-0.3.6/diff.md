# Comparing `tmp/pyechelle-0.3.5.tar.gz` & `tmp/pyechelle-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechelle-0.3.5.tar", max compression
+gzip compressed data, was "pyechelle-0.3.6.tar", max compression
```

## Comparing `pyechelle-0.3.5.tar` & `pyechelle-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1065 2022-11-19 15:42:42.016064 pyechelle-0.3.5/LICENSE
--rw-r--r--   0        0        0     3435 2022-11-19 15:42:42.016064 pyechelle-0.3.5/README.md
--rw-r--r--   0        0        0     2261 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/CCD.py
--rw-r--r--   0        0        0       81 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/__init__.py
--rw-r--r--   0        0        0     3325 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/benchmark.py
--rw-r--r--   0        0        0     6555 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/efficiency.py
--rw-r--r--   0        0        0     5522 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/model_viewer.py
--rw-r--r--   0        0        0       83 2022-11-30 15:21:31.680420 pyechelle-0.3.5/pyechelle/models/available_models.txt
--rw-r--r--   0        0        0     9351 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/optics.py
--rw-r--r--   0        0        0     2235 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/randomgen.py
--rw-r--r--   0        0        0     9582 2022-11-24 19:40:48.608404 pyechelle-0.3.5/pyechelle/raytrace_cuda.py
--rw-r--r--   0        0        0     8377 2022-11-24 19:40:48.608404 pyechelle-0.3.5/pyechelle/raytracing.py
--rwxr-xr-x   0        0        0    30886 2022-11-30 11:50:26.500584 pyechelle-0.3.5/pyechelle/simulator.py
--rw-r--r--   0        0        0     4700 2022-11-24 19:40:48.608404 pyechelle-0.3.5/pyechelle/slit.py
--rw-r--r--   0        0        0    15968 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/sources.py
--rw-r--r--   0        0        0    23213 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/spectrograph.py
--rw-r--r--   0        0        0      822 2022-11-19 15:42:42.172064 pyechelle-0.3.5/pyechelle/telescope.py
--rw-r--r--   0        0        0     1348 2022-11-30 15:02:26.161186 pyechelle-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4615 2022-11-30 15:27:38.255150 pyechelle-0.3.5/setup.py
--rw-r--r--   0        0        0     4496 2022-11-30 15:27:38.255477 pyechelle-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-11 10:17:14.118690 pyechelle-0.3.6/LICENSE
+-rw-r--r--   0        0        0       84 2023-06-06 12:23:50.718422 pyechelle-0.3.6/pyechelle/__init__.py
+-rw-r--r--   0        0        0     3422 2023-07-08 10:14:07.560615 pyechelle-0.3.6/pyechelle/benchmark.py
+-rw-r--r--   0        0        0     2335 2023-05-11 10:17:14.333485 pyechelle-0.3.6/pyechelle/CCD.py
+-rw-r--r--   0        0        0     7239 2023-06-06 12:23:50.718422 pyechelle-0.3.6/pyechelle/efficiency.py
+-rw-r--r--   0        0        0     5675 2023-05-11 10:17:14.334635 pyechelle-0.3.6/pyechelle/model_viewer.py
+-rw-r--r--   0        0        0       99 2023-07-08 10:14:07.561660 pyechelle-0.3.6/pyechelle/models/available_models.txt
+-rw-r--r--   0        0        0     9593 2023-05-11 10:17:14.336183 pyechelle-0.3.6/pyechelle/optics.py
+-rw-r--r--   0        0        0     2305 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/randomgen.py
+-rw-r--r--   0        0        0     9794 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/raytrace_cuda.py
+-rw-r--r--   0        0        0     8551 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/raytracing.py
+-rw-r--r--   0        0        0    31886 2023-06-06 12:23:50.722422 pyechelle-0.3.6/pyechelle/simulator.py
+-rw-r--r--   0        0        0     4854 2023-05-11 10:17:14.337422 pyechelle-0.3.6/pyechelle/slit.py
+-rw-r--r--   0        0        0    19711 2023-06-06 12:23:50.722422 pyechelle-0.3.6/pyechelle/sources.py
+-rw-r--r--   0        0        0    30781 2023-07-08 14:06:17.904478 pyechelle-0.3.6/pyechelle/spectrograph.py
+-rw-r--r--   0        0        0      853 2023-05-11 10:17:14.337993 pyechelle-0.3.6/pyechelle/telescope.py
+-rw-r--r--   0        0        0     1593 2023-07-08 13:18:29.945660 pyechelle-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3528 2023-05-11 10:17:14.118690 pyechelle-0.3.6/README.md
+-rw-r--r--   0        0        0     4639 1970-01-01 00:00:00.000000 pyechelle-0.3.6/PKG-INFO
```

### Comparing `pyechelle-0.3.5/README.md` & `pyechelle-0.3.6/README.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# PyEchelle
-
-PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
-However, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit
-spectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include
-photon and read-out noise.
-
-PyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major
-speed improvements.
-
-### Example usage
-
-You can use PyEchelle directly from the console:
-
-```bash
-pyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit
-```
-
-If you rather script in python, you can do the same as above with the following python script:
-
-```python
-
-from pyechelle.simulator import Simulator
-from pyechelle.sources import Phoenix
-from pyechelle.spectrograph import ZEMAX
-
-sim = Simulator(ZEMAX("MaroonX"))
-sim.set_ccd(1)
-sim.set_fibers([2, 3, 4])
-sim.set_sources(Phoenix(t_eff=3500))
-sim.set_exposure_time(10.)
-sim.set_radial_velocities(100.)
-sim.set_output('mdwarf.fits', overwrite=True)
-sim.run()
-
-```
-
-Both times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X
-spectrograph is simulated.
-
-The output is a 2D raw frame (.fits) and will look similar to:
-
-![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")
-
-Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
-
-Pyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar
-functionality but was written in C++. This package was rewritten in python for better maintainability, easier package
-distribution and for smoother cross-platform development.
-
-# Installation
-
-As simple as
-
-```bash
-pip install pyechelle
-```
-
-Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.
-
-# Usage
-
-See
-
-```bash
-pyechelle -h
-```
-
-for all available command line options.
-
-See [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
-
-# Concept:
-
-The basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and
-point spread functions which describe the spectrographs' optics:
-
-First, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.
-As the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle
-order, these matrices can be interpolated for any intermediate wavelength.
-
-Second, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly
-account for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for
-interpolation at intermediate wavelength.
-
-![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")
-
-**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate
-spectra without access to ZEMAX**
-
-# Citation
-
-Please cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.
+# PyEchelle
+
+PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
+However, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit
+spectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include
+photon and read-out noise.
+
+PyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major
+speed improvements.
+
+### Example usage
+
+You can use PyEchelle directly from the console:
+
+```bash
+pyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit
+```
+
+If you rather script in python, you can do the same as above with the following python script:
+
+```python
+
+from pyechelle.simulator import Simulator
+from pyechelle.sources import Phoenix
+from pyechelle.spectrograph import ZEMAX
+
+sim = Simulator(ZEMAX("MaroonX"))
+sim.set_ccd(1)
+sim.set_fibers([2, 3, 4])
+sim.set_sources(Phoenix(t_eff=3500))
+sim.set_exposure_time(10.)
+sim.set_radial_velocities(100.)
+sim.set_output('mdwarf.fits', overwrite=True)
+sim.run()
+
+```
+
+Both times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X
+spectrograph is simulated.
+
+The output is a 2D raw frame (.fits) and will look similar to:
+
+![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+Pyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar
+functionality but was written in C++. This package was rewritten in python for better maintainability, easier package
+distribution and for smoother cross-platform development.
+
+# Installation
+
+As simple as
+
+```bash
+pip install pyechelle
+```
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.
+
+# Usage
+
+See
+
+```bash
+pyechelle -h
+```
+
+for all available command line options.
+
+See [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+# Concept:
+
+The basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and
+point spread functions which describe the spectrographs' optics:
+
+First, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.
+As the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle
+order, these matrices can be interpolated for any intermediate wavelength.
+
+Second, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly
+account for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for
+interpolation at intermediate wavelength.
+
+![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")
+
+**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate
+spectra without access to ZEMAX**
+
+# Citation
+
+Please cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.
```

### Comparing `pyechelle-0.3.5/pyechelle/CCD.py` & `pyechelle-0.3.6/pyechelle/CCD.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-""" Detector module
-
-Implementing handling of CCDs/detectors for PyEchelle. It is recommended to use a dedicated detector simulation
-framework such as pyxel for including CCD effects such as cosmics, CTI or the brighter-fatter effect.
-
-Therefore, this module is kept rather simple.
-"""
-import logging
-from dataclasses import dataclass, field
-
-import numpy as np
-
-logger = logging.getLogger('CCD')
-
-
-@dataclass
-class CCD:
-    """ A CCD detector
-
-    Attributes:
-        data (np.ndarray): data array (uint) that will be filled by the simulator
-        n_pix_x (int): number of pixels in x-direction
-        n_pix_y (int): number of pixels in y-direction
-        maxval (int): maximum pixel value before clipping
-        pixelsize (float): physical size of an individual pixel [microns]
-        identifier (str): identifier of the CCD. This will also end up in the .fits header.
-
-    """
-    n_pix_x: int = 4096
-    n_pix_y: int = 4096
-    maxval: int = 65536
-    pixelsize: float = 9.
-    identifier: str = 'detector'
-    data: np.ndarray = field(init=False)
-
-    def __post_init__(self):
-        self.data = np.zeros((self.n_pix_y, self.n_pix_x), dtype=np.uint32)
-
-    def add_readnoise(self, std: float = 3.):
-        """ Adds readnoise to the detector counts
-
-        Args:
-            std: standard deviation of readnoise in counts
-
-        Returns:
-            None
-        """
-        self.data = self.data + np.asarray(np.random.normal(0., std, self.data.shape).round(0), dtype=np.int32)
-
-    def add_bias(self, value: int = 1000):
-        """Adds a bias value to the detector counts
-
-        Args:
-            value: bias value to be added. If float will get rounded to next integer
-
-        Returns:
-            None
-        """
-        self.data += value
-
-    def clip(self):
-        """ Clips CCD data
-
-        Clips data if any count value is larger than self.maxval
-
-        Returns:
-            None
-        """
-        if np.any(self.data < 0):
-            logger.warning('There is data <0 which will be clipped. Make sure you e.g. apply the bias before the '
-                           'readnoise.')
-            self.data[self.data < 0] = 0
-        if np.any(self.data > self.maxval):
-            self.data[self.data > self.maxval] = self.maxval
+""" Detector module
+
+Implementing handling of CCDs/detectors for PyEchelle. It is recommended to use a dedicated detector simulation
+framework such as pyxel for including CCD effects such as cosmics, CTI or the brighter-fatter effect.
+
+Therefore, this module is kept rather simple.
+"""
+import logging
+from dataclasses import dataclass, field
+
+import numpy as np
+
+logger = logging.getLogger('CCD')
+
+
+@dataclass
+class CCD:
+    """ A CCD detector
+
+    Attributes:
+        data (np.ndarray): data array (uint) that will be filled by the simulator
+        n_pix_x (int): number of pixels in x-direction
+        n_pix_y (int): number of pixels in y-direction
+        maxval (int): maximum pixel value before clipping
+        pixelsize (float): physical size of an individual pixel [microns]
+        identifier (str): identifier of the CCD. This will also end up in the .fits header.
+
+    """
+    n_pix_x: int = 4096
+    n_pix_y: int = 4096
+    maxval: int = 65536
+    pixelsize: float = 9.
+    identifier: str = 'detector'
+    data: np.ndarray = field(init=False)
+
+    def __post_init__(self):
+        self.data = np.zeros((self.n_pix_y, self.n_pix_x), dtype=np.uint32)
+
+    def add_readnoise(self, std: float = 3.):
+        """ Adds readnoise to the detector counts
+
+        Args:
+            std: standard deviation of readnoise in counts
+
+        Returns:
+            None
+        """
+        self.data = self.data + np.asarray(np.random.normal(0., std, self.data.shape).round(0), dtype=np.int32)
+
+    def add_bias(self, value: int = 1000):
+        """Adds a bias value to the detector counts
+
+        Args:
+            value: bias value to be added. If float will get rounded to next integer
+
+        Returns:
+            None
+        """
+        self.data += value
+
+    def clip(self):
+        """ Clips CCD data
+
+        Clips data if any count value is larger than self.maxval
+
+        Returns:
+            None
+        """
+        if np.any(self.data < 0):
+            logger.warning('There is data <0 which will be clipped. Make sure you e.g. apply the bias before the '
+                           'readnoise.')
+            self.data[self.data < 0] = 0
+        if np.any(self.data > self.maxval):
+            self.data[self.data > self.maxval] = self.maxval
```

### Comparing `pyechelle-0.3.5/pyechelle/efficiency.py` & `pyechelle-0.3.6/pyechelle/efficiency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,197 @@
-from __future__ import annotations
-
-import pathlib
-
-import numpy as np
-import skycalc_ipy
-from joblib import Memory
-from numpy import deg2rad
-from numpy import sin, cos, tan, arcsin
-from scipy.interpolate import interp1d
-
-path = pathlib.Path(__file__).parent.resolve()
-cache_path = path.joinpath('.cache')
-# create data directory if it doesn't exist:
-pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
-memory = Memory(cache_path, verbose=0)
-
-
-class Efficiency:
-    def __init__(self, name):
-        self.name = name
-
-    def get_efficiency(self, wavelength):
-        raise NotImplementedError
-
-    def get_efficiency_per_order(self, wavelength, order):
-        raise NotImplementedError
-
-
-class ConstantEfficiency(Efficiency):
-    def __init__(self, name, eff=1.):
-        super().__init__(name)
-        self.eff = eff
-
-    def get_efficiency(self, wavelength):
-        return np.ones_like(wavelength) * self.eff
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.get_efficiency(wavelength)
-
-
-class SystemEfficiency(Efficiency):
-    def __init__(self, efficiencies: list[Efficiency], name: str):
-        super().__init__(name)
-        self.efficiencies = efficiencies
-
-    def get_efficiency(self, wavelength):
-        e = np.ones_like(wavelength)
-        for ef in self.efficiencies:
-            e *= ef.get_efficiency(wavelength)
-        return e
-
-    def get_efficiency_per_order(self, wavelength, order):
-        e = np.ones_like(wavelength)
-        for ef in self.efficiencies:
-            e *= ef.get_efficiency_per_order(wavelength, order)
-        return e
-
-    def add_efficiency(self, efficiency):
-        self.efficiencies.append(efficiency)
-
-
-class GratingEfficiency(Efficiency):
-    def __init__(self, alpha, blaze, gpmm, peak_efficiency=1.0, name="Grating"):
-        super().__init__(name)
-        self.alpha = deg2rad(alpha)
-        self.blaze = deg2rad(blaze)
-        self.gpmm = gpmm
-        self.peak_efficiency = peak_efficiency
-
-    def calc_efficiency(self, order, wl):
-        bb = np.nan_to_num(
-            arcsin(-sin(self.alpha) + order * wl * 1e-6 / (1.0 / self.gpmm / 1000.0))
-        )
-        # blaze_wavelength = 2.*self.gpmm * sin(self.blaze) / order
-        # fsr = blaze_wavelength / order
-
-        x = (
-                order
-                * (cos(self.alpha) / cos(self.alpha - self.blaze))
-                * (cos(self.blaze) - sin(self.blaze) / tan((self.alpha + bb) / 2.0))
-        )
-        sinc = np.sinc(x)
-
-        return self.peak_efficiency * sinc * sinc
-
-    def get_efficiency(self, wavelength):
-        e = np.zeros_like(wavelength)
-        for o in range(50, 150):
-            e += self.calc_efficiency(o, wavelength)
-        return e
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.calc_efficiency(order, wavelength)
-
-
-class TabulatedEfficiency(Efficiency):
-    def __init__(self, name, wavelength, efficiency, orders=None):
-        super().__init__(name)
-        wavelength = np.atleast_1d(wavelength)
-        efficiency = np.atleast_1d(efficiency)
-        assert len(wavelength) == len(efficiency)
-        if orders is None:
-            # do constant extrapolation if only 1 point
-            if len(wavelength) == 1:
-                self.ip = lambda x: efficiency
-            # do linear interpolation if only 2 points
-            elif len(wavelength) == 2:
-                self.ip = interp1d(wavelength, efficiency, kind="linear", fill_value=0., bounds_error=False)
-            # do linear interpolation if only 2 points
-            elif len(wavelength) == 3:
-                self.ip = interp1d(wavelength, efficiency, kind="quadratic", fill_value=0., bounds_error=False)
-            # do cubic interpolation if >= 4 points
-            else:
-                self.ip = interp1d(wavelength, efficiency, kind="cubic", fill_value=0., bounds_error=False)
-            self.ip_per_order = self.ip
-        else:
-            self.ip_per_order = {}
-
-            for o in np.unique(orders):
-                idx = orders == o
-                self.ip_per_order[o] = interp1d(wavelength[idx], efficiency[idx], kind="cubic", fill_value=0.0,
-                                                bounds_error=False)
-
-            y = np.zeros_like(wavelength)
-            for o in np.unique(orders):
-                y += self.ip_per_order[o](wavelength)
-
-            self.ip = interp1d(wavelength, y)
-
-    def get_efficiency(self, wavelength):
-        return self.ip(wavelength)
-
-    def get_efficiency_per_order(self, wavelength, order):
-        if isinstance(self.ip_per_order, dict):
-            return self.ip_per_order[order](wavelength)
-        else:
-            return self.ip_per_order(wavelength)
-
-
-class CSVEfficiency(TabulatedEfficiency):
-    def __init__(self, name, path, delimiter=","):
-        data = np.genfromtxt(path, delimiter=delimiter)
-        if data.shape[1] == 2:  # file contains wavelength, efficiency
-            super().__init__(name, data[:, 0], data[:, 1])
-        if data.shape[1] == 3:  # file contains order, wavelength, efficiency
-            super().__init__(name, data[:, 1], data[:, 2], data[:, 0])
-
-
-class Atmosphere(Efficiency):
-    def __init__(self, name, sky_calc_kwargs=None):
-        super().__init__(name)
-        # set default atmosphere arguments to high-resolution
-        self.kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
-        if sky_calc_kwargs is not None:
-            self.kwargs.update(sky_calc_kwargs)
-
-    def get_efficiency(self, wavelength):
-        return self.get_atmosphere_data(wavelength, self.kwargs)
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.get_atmosphere_data(wavelength, self.kwargs)
-
-    @staticmethod
-    @memory.cache
-    def get_atmosphere_data(wavelength, sky_calc_kwargs=None):
-        kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
-        if sky_calc_kwargs is not None:
-            kwargs.update(sky_calc_kwargs)
-        sky = skycalc_ipy.SkyCalc()
-        sky.update(kwargs)  # set sky arguments
-        wmin = np.min(wavelength) * 1000.
-        wmax = np.max(wavelength) * 1000.
-        sky.update({'wmin': wmin, 'wmax': wmax})
-
-        tbl = sky.get_sky_spectrum()
-        # extrapolate is needed because tbl['lam'].data might not contain exact wavelength limits,
-        # since we are in constant resolution mode ("wgrid_mode": "fixed_spectral_resolution")
-        ip = interp1d(tbl['lam'].data, tbl['trans'].data, assume_sorted=True, fill_value="extrapolate")
-
-        return ip(wavelength)
+from __future__ import annotations
+
+import pathlib
+
+import numpy as np
+import skycalc_ipy
+from joblib import Memory
+from numpy import deg2rad
+from numpy import sin, cos, tan, arcsin
+from scipy.interpolate import interp1d
+
+path = pathlib.Path(__file__).parent.resolve()
+cache_path = path.joinpath('.cache')
+# create data directory if it doesn't exist:
+pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
+memory = Memory(cache_path, verbose=0)
+
+
+class Efficiency:
+    def __init__(self, name):
+        self.name = name
+
+    def get_efficiency(self, wavelength):
+        raise NotImplementedError
+
+    def get_efficiency_per_order(self, wavelength, order):
+        raise NotImplementedError
+
+
+class ConstantEfficiency(Efficiency):
+    def __init__(self, name, eff=1.):
+        super().__init__(name)
+        self.eff = eff
+
+    def get_efficiency(self, wavelength):
+        return np.ones_like(wavelength) * self.eff
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_efficiency(wavelength)
+
+
+class BandpassFilter(Efficiency):
+    def __init__(self, minwl, maxwl, name='bandpass'):
+        super().__init__(name=name)
+        self.minwl = minwl
+        self.maxwl = maxwl
+
+    def get_efficiency(self, wavelength):
+        e = np.ones_like(wavelength)
+        idx = np.logical_or((wavelength < self.minwl), (wavelength > self.maxwl))
+        e[idx] = 0.
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_efficiency(wavelength)
+
+
+class SystemEfficiency(Efficiency):
+    def __init__(self, efficiencies: list[Efficiency], name: str):
+        super().__init__(name)
+        self.efficiencies = efficiencies
+
+    def get_efficiency(self, wavelength):
+        e = np.ones_like(wavelength)
+        for ef in self.efficiencies:
+            e *= ef.get_efficiency(wavelength)
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        e = np.ones_like(wavelength)
+        for ef in self.efficiencies:
+            e *= ef.get_efficiency_per_order(wavelength, order)
+        return e
+
+    def add_efficiency(self, efficiency):
+        self.efficiencies.append(efficiency)
+
+
+class GratingEfficiency(Efficiency):
+    def __init__(self, alpha, blaze, gpmm, peak_efficiency=1.0, name="Grating"):
+        super().__init__(name)
+        self.alpha = deg2rad(alpha)
+        self.blaze = deg2rad(blaze)
+        self.gpmm = gpmm
+        self.peak_efficiency = peak_efficiency
+
+    def calc_efficiency(self, order, wl):
+        bb = np.nan_to_num(
+            arcsin(-sin(self.alpha) + order * wl * 1e-6 / (1.0 / self.gpmm / 1000.0))
+        )
+        # blaze_wavelength = 2.*self.gpmm * sin(self.blaze) / order
+        # fsr = blaze_wavelength / order
+
+        x = (
+                order
+                * (cos(self.alpha) / cos(self.alpha - self.blaze))
+                * (cos(self.blaze) - sin(self.blaze) / tan((self.alpha + bb) / 2.0))
+        )
+        sinc = np.sinc(x)
+
+        return self.peak_efficiency * sinc * sinc
+
+    def get_efficiency(self, wavelength):
+        e = np.zeros_like(wavelength)
+        for o in range(50, 150):
+            e += self.calc_efficiency(o, wavelength)
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.calc_efficiency(order, wavelength)
+
+
+class TabulatedEfficiency(Efficiency):
+    def __init__(self, name, wavelength, efficiency, orders=None):
+        super().__init__(name)
+        wavelength = np.atleast_1d(wavelength)
+        efficiency = np.atleast_1d(efficiency)
+        assert len(wavelength) == len(efficiency)
+        if orders is None:
+            # do constant extrapolation if only 1 point
+            if len(wavelength) == 1:
+                self.ip = lambda x: efficiency
+            # do linear interpolation if only 2 points
+            elif len(wavelength) == 2:
+                self.ip = interp1d(wavelength, efficiency, kind="linear", fill_value=0., bounds_error=False)
+            # do linear interpolation if only 2 points
+            elif len(wavelength) == 3:
+                self.ip = interp1d(wavelength, efficiency, kind="quadratic", fill_value=0., bounds_error=False)
+            # do cubic interpolation if >= 4 points
+            else:
+                self.ip = interp1d(wavelength, efficiency, kind="cubic", fill_value=0., bounds_error=False)
+            self.ip_per_order = self.ip
+        else:
+            self.ip_per_order = {}
+
+            for o in np.unique(orders):
+                idx = orders == o
+                self.ip_per_order[o] = interp1d(wavelength[idx], efficiency[idx], kind="cubic", fill_value=0.0,
+                                                bounds_error=False)
+
+            y = np.zeros_like(wavelength)
+            for o in np.unique(orders):
+                y += self.ip_per_order[o](wavelength)
+
+            self.ip = interp1d(wavelength, y)
+
+    def get_efficiency(self, wavelength):
+        return self.ip(wavelength)
+
+    def get_efficiency_per_order(self, wavelength, order):
+        if isinstance(self.ip_per_order, dict):
+            return self.ip_per_order[order](wavelength)
+        else:
+            return self.ip_per_order(wavelength)
+
+
+class CSVEfficiency(TabulatedEfficiency):
+    def __init__(self, name, path, delimiter=","):
+        data = np.genfromtxt(path, delimiter=delimiter)
+        if data.shape[1] == 2:  # file contains wavelength, efficiency
+            super().__init__(name, data[:, 0], data[:, 1])
+        if data.shape[1] == 3:  # file contains order, wavelength, efficiency
+            super().__init__(name, data[:, 1], data[:, 2], data[:, 0])
+
+
+class Atmosphere(Efficiency):
+    def __init__(self, name, sky_calc_kwargs=None):
+        super().__init__(name)
+        # set default atmosphere arguments to high-resolution
+        self.kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
+        if sky_calc_kwargs is not None:
+            self.kwargs.update(sky_calc_kwargs)
+
+    def get_efficiency(self, wavelength):
+        return self.get_atmosphere_data(wavelength, self.kwargs)
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_atmosphere_data(wavelength, self.kwargs)
+
+    @staticmethod
+    @memory.cache
+    def get_atmosphere_data(wavelength, sky_calc_kwargs=None):
+        kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
+        if sky_calc_kwargs is not None:
+            kwargs.update(sky_calc_kwargs)
+        sky = skycalc_ipy.SkyCalc()
+        sky.update(kwargs)  # set sky arguments
+        wmin = np.min(wavelength) * 1000.
+        wmax = np.max(wavelength) * 1000.
+        sky.update({'wmin': wmin, 'wmax': wmax})
+
+        tbl = sky.get_sky_spectrum()
+        # extrapolate is needed because tbl['lam'].data might not contain exact wavelength limits,
+        # since we are in constant resolution mode ("wgrid_mode": "fixed_spectral_resolution")
+        ip = interp1d(tbl['lam'].data, tbl['trans'].data, assume_sorted=True, fill_value="extrapolate")
+
+        return ip(wavelength)
```

### Comparing `pyechelle-0.3.5/pyechelle/model_viewer.py` & `pyechelle-0.3.6/pyechelle/model_viewer.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import argparse
-import sys
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from pyechelle.optics import convert_matrix
-from pyechelle.simulator import available_models
-from pyechelle.spectrograph import Spectrograph, ZEMAX
-
-
-def plot_transformations(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot affine transformation matrices
-
-    Args:
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-    fig, ax = plt.subplots(2, 3, sharex=True)
-    fig.suptitle(f"Affine transformations of {spectrograph.name}")
-    if isinstance(spectrograph, ZEMAX):
-        for o in spectrograph.get_orders(fiber, ccd_index):
-            ax[0, 0].set_title("sx")
-            ax[0, 0].plot([af.sx for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[0, 1].set_title("sy")
-            ax[0, 1].plot([af.sy for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[0, 2].set_title("shear")
-            ax[0, 2].plot([af.shear for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 0].set_title("rot")
-            ax[1, 0].plot([af.rot for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 1].set_title("tx")
-            ax[1, 1].plot([af.tx for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 2].set_title("ty")
-            ax[1, 2].plot([af.ty for af in spectrograph.transformations(o, fiber, ccd_index)])
-    else:
-        raise NotImplementedError
-    return fig
-
-
-def plot_transformation_matrices(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot affine transformation matrices
-
-    Args:
-        fiber: fiber index
-        ccd_index: ccd index
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-    fig, ax = plt.subplots(2, 3, sharex=True)
-    fig.suptitle(f"Affine transformation matrices of {spectrograph.name}")
-    for o in spectrograph.get_orders(fiber, ccd_index):
-        if isinstance(spectrograph, ZEMAX):
-            transformations = convert_matrix(
-                np.array([tm.as_matrix() for tm in spectrograph.transformations(o, fiber, ccd_index)]).T)
-            ax[0, 0].set_title("m0")
-            ax[0, 0].plot(transformations[0])
-            ax[0, 1].set_title("m1")
-            ax[0, 1].plot(transformations[1])
-            ax[0, 2].set_title("m2")
-            ax[0, 2].plot(transformations[2])
-            ax[1, 0].set_title("m3")
-            ax[1, 0].plot(transformations[3])
-            ax[1, 1].set_title("m4")
-            ax[1, 1].plot(transformations[4])
-            ax[1, 2].set_title("m5")
-            ax[1, 2].plot(transformations[5])
-        else:
-            raise NotImplementedError
-    return fig
-
-
-def plot_psfs(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot PSFs as one big map
-    Args:
-        fiber: fiber index
-        ccd_index: ccd index
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-
-    fig, ax = plt.subplots()
-    orders = spectrograph.get_orders(fiber, ccd_index)
-    n_orders = len(orders)
-    if isinstance(spectrograph, ZEMAX):
-        n_psfs = len(spectrograph.psfs(orders[0], fiber, ccd_index))
-    else:
-        n_psfs = 10
-
-    shape_psfs = spectrograph.get_psf(sum(spectrograph.get_wavelength_range(orders[0], fiber, ccd_index)) / 2.,
-                                      orders[0], fiber, ccd_index).data.shape
-
-    # shape_psfs = spectrograph.psfs[next(spectrograph.psfs.keys().__iter__())].psfs[0].data.shape
-    img = np.empty((n_psfs * shape_psfs[0], n_orders * shape_psfs[1]))
-
-    for oo, o in enumerate(np.sort(orders)):
-        if isinstance(spectrograph, ZEMAX):
-            psfs = spectrograph.psfs(o, fiber, ccd_index)
-        else:
-            wl = np.linspace(*spectrograph.get_wavelength_range(o, fiber, ccd_index), num=n_psfs)
-            psfs = [spectrograph.get_psf(w, o, fiber, ccd_index) for w in wl]
-
-        for i, p in enumerate(psfs):
-            if p.data.shape == shape_psfs:
-                img[int(i * shape_psfs[0]):int((i + 1) * shape_psfs[0]),
-                int(oo * shape_psfs[1]):int((oo + 1) * shape_psfs[1])] = p.data
-    ax.imshow(img, vmin=0, vmax=np.mean(img) * 10.0)
-    return fig
-
-
-# def plot_fields(spec: ZEMAX, show=True):
-#     plt.figure()
-#     with h5py.File(spec.modelpath, 'r') as h5f:
-#         for k in h5f.keys():
-#             if 'fiber_' in k:
-#                 a = h5f[k].attrs['norm_field'].decode('utf-8').split('\n')
-#
-#                 for b in a:
-#                     if 'aF' in b:
-#                         print(b[2:])
-
-
-def main(args):
-    if not args:
-        args = sys.argv[1:]
-
-    parser = argparse.ArgumentParser(description='PyEchelle Simulator Model Viewer')
-    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
-                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
-    parser.add_argument('--fiber', type=int, default=1, required=False)
-    parser.add_argument('--show', action='store_true')
-
-    args = parser.parse_args(args)
-    spec = ZEMAX(args.spectrograph)
-    # if args.plot_transformations:
-    plot_transformations(spec, args.fiber)
-    # if args.plot_transformation_matrices:
-    plot_transformation_matrices(spec, args.fiber)
-    # if args.plot_field:
-    # plot_fields(spec)
-    # if args.plot_psfs:
-    plot_psfs(spec)
-    if args.show:
-        plt.show()
-
-
-if __name__ == "__main__":
-    main(sys.argv[1:])
+import argparse
+import sys
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from pyechelle.optics import convert_matrix
+from pyechelle.simulator import available_models
+from pyechelle.spectrograph import Spectrograph, ZEMAX
+
+
+def plot_transformations(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
+    """ Plot affine transformation matrices
+
+    Args:
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+    fig, ax = plt.subplots(2, 3, sharex=True)
+    fig.suptitle(f"Affine transformations of {spectrograph.name}")
+    if isinstance(spectrograph, ZEMAX):
+        for o in spectrograph.get_orders(fiber, ccd_index):
+            ax[0, 0].set_title("sx")
+            ax[0, 0].plot([af.sx for af in spectrograph.transformations(o, fiber, ccd_index)])
+            ax[0, 1].set_title("sy")
+            ax[0, 1].plot([af.sy for af in spectrograph.transformations(o, fiber, ccd_index)])
+            ax[0, 2].set_title("shear")
+            ax[0, 2].plot([af.shear for af in spectrograph.transformations(o, fiber, ccd_index)])
+            ax[1, 0].set_title("rot")
+            ax[1, 0].plot([af.rot for af in spectrograph.transformations(o, fiber, ccd_index)])
+            ax[1, 1].set_title("tx")
+            ax[1, 1].plot([af.tx for af in spectrograph.transformations(o, fiber, ccd_index)])
+            ax[1, 2].set_title("ty")
+            ax[1, 2].plot([af.ty for af in spectrograph.transformations(o, fiber, ccd_index)])
+    else:
+        raise NotImplementedError
+    return fig
+
+
+def plot_transformation_matrices(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
+    """ Plot affine transformation matrices
+
+    Args:
+        fiber: fiber index
+        ccd_index: ccd index
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+    fig, ax = plt.subplots(2, 3, sharex=True)
+    fig.suptitle(f"Affine transformation matrices of {spectrograph.name}")
+    for o in spectrograph.get_orders(fiber, ccd_index):
+        if isinstance(spectrograph, ZEMAX):
+            transformations = convert_matrix(
+                np.array([tm.as_matrix() for tm in spectrograph.transformations(o, fiber, ccd_index)]).T)
+            ax[0, 0].set_title("m0")
+            ax[0, 0].plot(transformations[0])
+            ax[0, 1].set_title("m1")
+            ax[0, 1].plot(transformations[1])
+            ax[0, 2].set_title("m2")
+            ax[0, 2].plot(transformations[2])
+            ax[1, 0].set_title("m3")
+            ax[1, 0].plot(transformations[3])
+            ax[1, 1].set_title("m4")
+            ax[1, 1].plot(transformations[4])
+            ax[1, 2].set_title("m5")
+            ax[1, 2].plot(transformations[5])
+        else:
+            raise NotImplementedError
+    return fig
+
+
+def plot_psfs(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
+    """ Plot PSFs as one big map
+    Args:
+        fiber: fiber index
+        ccd_index: ccd index
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+
+    fig, ax = plt.subplots()
+    orders = spectrograph.get_orders(fiber, ccd_index)
+    n_orders = len(orders)
+    if isinstance(spectrograph, ZEMAX):
+        n_psfs = len(spectrograph.psfs(orders[0], fiber, ccd_index))
+    else:
+        n_psfs = 10
+
+    shape_psfs = spectrograph.get_psf(sum(spectrograph.get_wavelength_range(orders[0], fiber, ccd_index)) / 2.,
+                                      orders[0], fiber, ccd_index).data.shape
+
+    # shape_psfs = spectrograph.psfs[next(spectrograph.psfs.keys().__iter__())].psfs[0].data.shape
+    img = np.empty((n_psfs * shape_psfs[0], n_orders * shape_psfs[1]))
+
+    for oo, o in enumerate(np.sort(orders)):
+        if isinstance(spectrograph, ZEMAX):
+            psfs = spectrograph.psfs(o, fiber, ccd_index)
+        else:
+            wl = np.linspace(*spectrograph.get_wavelength_range(o, fiber, ccd_index), num=n_psfs)
+            psfs = [spectrograph.get_psf(w, o, fiber, ccd_index) for w in wl]
+
+        for i, p in enumerate(psfs):
+            if p.data.shape == shape_psfs:
+                img[int(i * shape_psfs[0]):int((i + 1) * shape_psfs[0]),
+                int(oo * shape_psfs[1]):int((oo + 1) * shape_psfs[1])] = p.data
+    ax.imshow(img, vmin=0, vmax=np.mean(img) * 10.0)
+    return fig
+
+
+# def plot_fields(spec: ZEMAX, show=True):
+#     plt.figure()
+#     with h5py.File(spec.modelpath, 'r') as h5f:
+#         for k in h5f.keys():
+#             if 'fiber_' in k:
+#                 a = h5f[k].attrs['norm_field'].decode('utf-8').split('\n')
+#
+#                 for b in a:
+#                     if 'aF' in b:
+#                         print(b[2:])
+
+
+def main(args):
+    if not args:
+        args = sys.argv[1:]
+
+    parser = argparse.ArgumentParser(description='PyEchelle Simulator Model Viewer')
+    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
+                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
+    parser.add_argument('--fiber', type=int, default=1, required=False)
+    parser.add_argument('--show', action='store_true')
+
+    args = parser.parse_args(args)
+    spec = ZEMAX(args.spectrograph)
+    # if args.plot_transformations:
+    plot_transformations(spec, args.fiber)
+    # if args.plot_transformation_matrices:
+    plot_transformation_matrices(spec, args.fiber)
+    # if args.plot_field:
+    # plot_fields(spec)
+    # if args.plot_psfs:
+    plot_psfs(spec)
+    if args.show:
+        plt.show()
+
+
+if __name__ == "__main__":
+    main(sys.argv[1:])
```

### Comparing `pyechelle-0.3.5/pyechelle/optics.py` & `pyechelle-0.3.6/pyechelle/optics.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-""" Optics module
-
-PyEchelle concept is to describe the optics of an instrument by applying a wavelength dependent affine transformation
- to the input plane and applying a PSF. This module implements the two basic classes that are needed to do so.
-"""
-from __future__ import annotations
-
-import math
-from dataclasses import dataclass, field
-
-import numba
-import numpy as np
-import scipy.interpolate
-
-
-@dataclass
-class AffineTransformation:
-    r""" Affine transformation matrix
-
-    This class represents an affine transformation matrix.
-
-    PyEchelle uses affine transformations (which are represented by affine transformation matrices) to describe the
-    mapping of a monochromatic image from the input focal plane of the spectrograph to the detector plane.
-
-    See `wikipedia <https://en.wikipedia.org/wiki/Affine_transformation>`_ for more details about affine transformations.
-
-    In two dimensions an affine transformation matrix can be written as:
-
-    .. math::
-        M = \begin{bmatrix}
-        m0 & m1 & m2 \\
-        m3 & m4 & m4 \\
-        0 & 0 & 1
-        \end{bmatrix}
-
-    The last row is constant and is therefore be omitted. This is the form that is returned (as a flat array) by
-    :meth:`pyechelle.AffineTransformation.as_matrix`
-
-    There is another more intuitive representation of an affine transformation matrix in terms of the parameters:
-    rotation, scaling in x- and y-direction, shear and translation in x- and y-direction.
-    See :meth:`pyechelle.AffineTransformation.__post_init__` for how those representations are connected.
-
-    Instances of this class can be sorted by wavelength.
-
-    Attributes:
-        rot (float): rotation [radians]
-        sx (float): scaling factor in x-direction
-        sy (float): scaling factor in y-direction
-        shear (float): shearing factor
-        tx (float): translation in x-direction
-        ty (float): translation in y-direction
-        wavelength (float | None): wavelength [micron] of affine transformation matrix
-    """
-    rot: float
-    sx: float
-    sy: float
-    shear: float
-    tx: float
-    ty: float
-    wavelength: float | None
-
-    def __le__(self, other):
-        return self.wavelength <= other.wavelength
-
-    def __lt__(self, other):
-        return self.wavelength < other.wavelength
-
-    def __add__(self, other):
-        wl = None
-        if other.wavelength and self.wavelength:
-            assert np.isclose(other.wavelength, self.wavelength)
-            wl = self.wavelength
-        if other.wavelength and self.wavelength is None:
-            wl = other.wavelength
-        if self.wavelength and other.wavelength is None:
-            wl = self.wavelength
-        return AffineTransformation(self.rot + other.rot,
-                                    self.sx + other.sx,
-                                    self.sy + other.sy,
-                                    self.shear + other.shear,
-                                    self.tx + other.tx,
-                                    self.ty + other.ty,
-                                    wl)
-
-    def __sub__(self, other):
-        wl = None
-        if other.wavelength and self.wavelength:
-            assert np.isclose(other.wavelength, self.wavelength)
-            wl = self.wavelength
-        if other.wavelength and self.wavelength is None:
-            wl = other.wavelength
-        if self.wavelength and other.wavelength is None:
-            wl = self.wavelength
-        return AffineTransformation(self.rot - other.rot,
-                                    self.sx - other.sx,
-                                    self.sy - other.sy,
-                                    self.shear - other.shear,
-                                    self.tx - other.tx,
-                                    self.ty - other.ty,
-                                    wl)
-
-    def __iadd__(self, other):
-        assert np.isclose(other.wavelength, self.wavelength)
-        self.sx += other.sx
-        self.sy += other.sy
-        self.shear += other.shear
-        self.tx += other.tx
-        self.ty += other.ty
-        return self
-
-    def __isub__(self, other):
-        assert np.isclose(other.wavelength, self.wavelength)
-        self.sx -= other.sx
-        self.sy -= other.sy
-        self.shear -= other.shear
-        self.tx -= other.tx
-        self.ty -= other.ty
-        return self
-
-    def __mul__(self, other):
-        assert isinstance(other, tuple), "You can only multiply an affine matrix with a tuple of length 2 (x," \
-                                         "y coordinate) "
-        assert len(other) == 2, "You can only multiply an affine matrix with a tuple of length 2  (x,y coordinate)"
-        x_new = self.sx * math.cos(self.rot) * other[0] - self.sy * math.sin(self.rot + self.shear) * other[1] + self.tx
-        y_new = self.sx * math.sin(self.rot) * other[0] + self.sy * math.cos(self.rot + self.shear) * other[1] + self.ty
-        return x_new, y_new
-
-    def as_matrix(self) -> tuple:
-        """flat affine matrix
-
-        Returns:
-            flat affine transformation matrix
-        """
-        return self.rot, self.sx, self.sy, self.shear, self.tx, self.ty
-
-
-@dataclass
-class TransformationSet:
-    affine_transformations: list[AffineTransformation]
-    rot: np.ndarray = field(init=False)
-    sx: np.ndarray = field(init=False)
-    sy: np.ndarray = field(init=False)
-    shear: np.ndarray = field(init=False)
-    tx: np.ndarray = field(init=False)
-    ty: np.ndarray = field(init=False)
-    wl: np.ndarray = field(init=False)
-
-    _spline_affine: list = field(init=False, default=None)
-
-    def __post_init__(self):
-        self.affine_transformations.sort()
-
-        self.rot = np.array([at.rot for at in self.affine_transformations])
-        self.sx = np.array([at.sx for at in self.affine_transformations])
-        self.sy = np.array([at.sy for at in self.affine_transformations])
-        self.shear = np.array([at.shear for at in self.affine_transformations])
-        self.tx = np.array([at.tx for at in self.affine_transformations])
-        self.ty = np.array([at.ty for at in self.affine_transformations])
-
-        # correct for possible jumps in rot and shear
-        # assert max(abs(np.ediff1d(self.shear))) < 4, 'There is a jump in the shear parameter of the model file. ' \
-        #                                              'Please correct the jump, by wrapping shear to e.g. to (-pi, pi) or (0, 2.*pi)'
-
-        # self.shear = np.mod(self.shear, np.pi * 2.)
-
-        self.wl = np.array([at.wavelength for at in self.affine_transformations])
-
-    def get_affine_transformations(self, wl: float | np.ndarray) -> AffineTransformation | np.ndarray:
-        if self._spline_affine is None:
-            self._spline_affine = [scipy.interpolate.CubicSpline(self.wl, self.rot),
-                                   scipy.interpolate.CubicSpline(self.wl, self.sx),
-                                   scipy.interpolate.CubicSpline(self.wl, self.sy),
-                                   scipy.interpolate.CubicSpline(self.wl, self.shear),
-                                   scipy.interpolate.CubicSpline(self.wl, self.tx),
-                                   scipy.interpolate.CubicSpline(self.wl, self.ty)
-                                   ]
-        if isinstance(wl, float):
-            return AffineTransformation(*[af(wl) for af in self._spline_affine], wl)
-        else:
-            return np.array([af(wl) for af in self._spline_affine])
-
-
-def convert_matrix(input: AffineTransformation | np.ndarray) -> np.ndarray:
-    if isinstance(input, AffineTransformation):
-        return np.array([input.sx * math.cos(input.rot),
-                         -input.sy * math.sin(input.rot + input.shear),
-                         input.tx,
-                         input.sx * math.sin(input.rot),
-                         input.sy * math.cos(input.rot + input.shear),
-                         input.ty])
-    else:
-        assert isinstance(input, np.ndarray)
-        return np.array([
-            input[1] * np.cos(input[0]),
-            -input[2] * np.sin(input[0] + input[3]),
-            input[4],
-            input[1] * np.sin(input[0]),
-            input[2] * np.cos(input[0] + input[3]),
-            input[5]])
-
-
-@numba.njit
-def apply_matrix(matrix, coords):
-    return matrix[0] * coords[0] + matrix[1] * coords[1] + matrix[2], \
-           matrix[3] * coords[0] + matrix[4] * coords[1] + matrix[5]
-
-
-@dataclass
-class PSF:
-    """Point spread function
-
-    The point spread function describes how an optical system responds to a point source.
-
-    Attributes:
-        wavelength (float): wavelength [micron]
-        data (np.ndarray): PSF data as 2D array
-        sampling (float): physical size of the sampling of data [micron]
-
-    """
-    wavelength: float
-    data: np.ndarray
-    sampling: float
-
-    def __post_init__(self):
-        self.data /= np.sum(self.data)
-
-    def __le__(self, other):
-        return self.wavelength <= other.wavelength
-
-    def __lt__(self, other):
-        return self.wavelength < other.wavelength
-
-    def __str__(self):
-        res = f'PSF@\n{self.wavelength:.4f}micron\n'
-        letters = ['.', ':', 'o', 'x', '#', '@']
-        norm = np.max(self.data)
-        for d in self.data:
-            for dd in d:
-                i = int(math.floor(dd / norm / 0.2))
-                res += letters[i]
-            res += '\n'
-        return res
+""" Optics module
+
+PyEchelle concept is to describe the optics of an instrument by applying a wavelength dependent affine transformation
+ to the input plane and applying a PSF. This module implements the two basic classes that are needed to do so.
+"""
+from __future__ import annotations
+
+import math
+from dataclasses import dataclass, field
+
+import numba
+import numpy as np
+import scipy.interpolate
+
+
+@dataclass
+class AffineTransformation:
+    r""" Affine transformation matrix
+
+    This class represents an affine transformation matrix.
+
+    PyEchelle uses affine transformations (which are represented by affine transformation matrices) to describe the
+    mapping of a monochromatic image from the input focal plane of the spectrograph to the detector plane.
+
+    See `wikipedia <https://en.wikipedia.org/wiki/Affine_transformation>`_ for more details about affine transformations.
+
+    In two dimensions an affine transformation matrix can be written as:
+
+    .. math::
+        M = \begin{bmatrix}
+        m0 & m1 & m2 \\
+        m3 & m4 & m4 \\
+        0 & 0 & 1
+        \end{bmatrix}
+
+    The last row is constant and is therefore be omitted. This is the form that is returned (as a flat array) by
+    :meth:`pyechelle.AffineTransformation.as_matrix`
+
+    There is another more intuitive representation of an affine transformation matrix in terms of the parameters:
+    rotation, scaling in x- and y-direction, shear and translation in x- and y-direction.
+    See :meth:`pyechelle.AffineTransformation.__post_init__` for how those representations are connected.
+
+    Instances of this class can be sorted by wavelength.
+
+    Attributes:
+        rot (float): rotation [radians]
+        sx (float): scaling factor in x-direction
+        sy (float): scaling factor in y-direction
+        shear (float): shearing factor
+        tx (float): translation in x-direction
+        ty (float): translation in y-direction
+        wavelength (float | None): wavelength [micron] of affine transformation matrix
+    """
+    rot: float
+    sx: float
+    sy: float
+    shear: float
+    tx: float
+    ty: float
+    wavelength: float | None
+
+    def __le__(self, other):
+        return self.wavelength <= other.wavelength
+
+    def __lt__(self, other):
+        return self.wavelength < other.wavelength
+
+    def __add__(self, other):
+        wl = None
+        if other.wavelength and self.wavelength:
+            assert np.isclose(other.wavelength, self.wavelength)
+            wl = self.wavelength
+        if other.wavelength and self.wavelength is None:
+            wl = other.wavelength
+        if self.wavelength and other.wavelength is None:
+            wl = self.wavelength
+        return AffineTransformation(self.rot + other.rot,
+                                    self.sx + other.sx,
+                                    self.sy + other.sy,
+                                    self.shear + other.shear,
+                                    self.tx + other.tx,
+                                    self.ty + other.ty,
+                                    wl)
+
+    def __sub__(self, other):
+        wl = None
+        if other.wavelength and self.wavelength:
+            assert np.isclose(other.wavelength, self.wavelength)
+            wl = self.wavelength
+        if other.wavelength and self.wavelength is None:
+            wl = other.wavelength
+        if self.wavelength and other.wavelength is None:
+            wl = self.wavelength
+        return AffineTransformation(self.rot - other.rot,
+                                    self.sx - other.sx,
+                                    self.sy - other.sy,
+                                    self.shear - other.shear,
+                                    self.tx - other.tx,
+                                    self.ty - other.ty,
+                                    wl)
+
+    def __iadd__(self, other):
+        assert np.isclose(other.wavelength, self.wavelength)
+        self.sx += other.sx
+        self.sy += other.sy
+        self.shear += other.shear
+        self.tx += other.tx
+        self.ty += other.ty
+        return self
+
+    def __isub__(self, other):
+        assert np.isclose(other.wavelength, self.wavelength)
+        self.sx -= other.sx
+        self.sy -= other.sy
+        self.shear -= other.shear
+        self.tx -= other.tx
+        self.ty -= other.ty
+        return self
+
+    def __mul__(self, other):
+        assert isinstance(other, tuple), "You can only multiply an affine matrix with a tuple of length 2 (x," \
+                                         "y coordinate) "
+        assert len(other) == 2, "You can only multiply an affine matrix with a tuple of length 2  (x,y coordinate)"
+        x_new = self.sx * math.cos(self.rot) * other[0] - self.sy * math.sin(self.rot + self.shear) * other[1] + self.tx
+        y_new = self.sx * math.sin(self.rot) * other[0] + self.sy * math.cos(self.rot + self.shear) * other[1] + self.ty
+        return x_new, y_new
+
+    def as_matrix(self) -> tuple:
+        """flat affine matrix
+
+        Returns:
+            flat affine transformation matrix
+        """
+        return self.rot, self.sx, self.sy, self.shear, self.tx, self.ty
+
+
+@dataclass
+class TransformationSet:
+    affine_transformations: list[AffineTransformation]
+    rot: np.ndarray = field(init=False)
+    sx: np.ndarray = field(init=False)
+    sy: np.ndarray = field(init=False)
+    shear: np.ndarray = field(init=False)
+    tx: np.ndarray = field(init=False)
+    ty: np.ndarray = field(init=False)
+    wl: np.ndarray = field(init=False)
+
+    _spline_affine: list = field(init=False, default=None)
+
+    def __post_init__(self):
+        self.affine_transformations.sort()
+
+        self.rot = np.array([at.rot for at in self.affine_transformations])
+        self.sx = np.array([at.sx for at in self.affine_transformations])
+        self.sy = np.array([at.sy for at in self.affine_transformations])
+        self.shear = np.array([at.shear for at in self.affine_transformations])
+        self.tx = np.array([at.tx for at in self.affine_transformations])
+        self.ty = np.array([at.ty for at in self.affine_transformations])
+
+        # correct for possible jumps in rot and shear
+        # assert max(abs(np.ediff1d(self.shear))) < 4, 'There is a jump in the shear parameter of the model file. ' \
+        #                                              'Please correct the jump, by wrapping shear to e.g. to (-pi, pi) or (0, 2.*pi)'
+
+        # self.shear = np.mod(self.shear, np.pi * 2.)
+
+        self.wl = np.array([at.wavelength for at in self.affine_transformations])
+
+    def get_affine_transformations(self, wl: float | np.ndarray) -> AffineTransformation | np.ndarray:
+        if self._spline_affine is None:
+            self._spline_affine = [scipy.interpolate.CubicSpline(self.wl, self.rot),
+                                   scipy.interpolate.CubicSpline(self.wl, self.sx),
+                                   scipy.interpolate.CubicSpline(self.wl, self.sy),
+                                   scipy.interpolate.CubicSpline(self.wl, self.shear),
+                                   scipy.interpolate.CubicSpline(self.wl, self.tx),
+                                   scipy.interpolate.CubicSpline(self.wl, self.ty)
+                                   ]
+        if isinstance(wl, float):
+            return AffineTransformation(*[af(wl) for af in self._spline_affine], wl)
+        else:
+            return np.array([af(wl) for af in self._spline_affine])
+
+
+def convert_matrix(input: AffineTransformation | np.ndarray) -> np.ndarray:
+    if isinstance(input, AffineTransformation):
+        return np.array([input.sx * math.cos(input.rot),
+                         -input.sy * math.sin(input.rot + input.shear),
+                         input.tx,
+                         input.sx * math.sin(input.rot),
+                         input.sy * math.cos(input.rot + input.shear),
+                         input.ty])
+    else:
+        assert isinstance(input, np.ndarray)
+        return np.array([
+            input[1] * np.cos(input[0]),
+            -input[2] * np.sin(input[0] + input[3]),
+            input[4],
+            input[1] * np.sin(input[0]),
+            input[2] * np.cos(input[0] + input[3]),
+            input[5]])
+
+
+@numba.njit
+def apply_matrix(matrix, coords):
+    return matrix[0] * coords[0] + matrix[1] * coords[1] + matrix[2], \
+           matrix[3] * coords[0] + matrix[4] * coords[1] + matrix[5]
+
+
+@dataclass
+class PSF:
+    """Point spread function
+
+    The point spread function describes how an optical system responds to a point source.
+
+    Attributes:
+        wavelength (float): wavelength [micron]
+        data (np.ndarray): PSF data as 2D array
+        sampling (float): physical size of the sampling of data [micron]
+
+    """
+    wavelength: float
+    data: np.ndarray
+    sampling: float
+
+    def __post_init__(self):
+        self.data /= np.sum(self.data)
+
+    def __le__(self, other):
+        return self.wavelength <= other.wavelength
+
+    def __lt__(self, other):
+        return self.wavelength < other.wavelength
+
+    def __str__(self):
+        res = f'PSF@\n{self.wavelength:.4f}micron\n'
+        letters = ['.', ':', 'o', 'x', '#', '@']
+        norm = np.max(self.data)
+        for d in self.data:
+            for dd in d:
+                i = int(math.floor(dd / norm / 0.2))
+                res += letters[i]
+            res += '\n'
+        return res
```

### Comparing `pyechelle-0.3.5/pyechelle/raytrace_cuda.py` & `pyechelle-0.3.6/pyechelle/raytrace_cuda.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-import math
-import pathlib
-
-import numba
-import numba.cuda
-import numpy as np
-from joblib import Memory
-from numba import cuda
-from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float64
-
-from pyechelle.optics import convert_matrix
-from pyechelle.randomgen import make_alias_sampling_arrays
-from pyechelle.sources import Source
-from pyechelle.spectrograph import Spectrograph
-from pyechelle.telescope import Telescope
-
-path = pathlib.Path(__file__).parent.resolve()
-cache_path = path.joinpath('.cache')
-# create data directory if it doesn't exist:
-pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
-memory = Memory(cache_path, verbose=0)
-
-
-@memory.cache
-def make_cuda_kernel(slitfun):
-    @cuda.jit()
-    def cuda_kernel(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld,
-                    transf_deriv, psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd,
-                    pixelsize, rng_states, nphotons):
-        max_y, max_x = ccd.shape
-        thread_id = cuda.grid(1)
-
-        for _ in range(thread_id, nphotons, cuda.gridDim.x * cuda.blockDim.x):
-            # sample from spectrum
-            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(spectrum_j)))
-            wl = spectrum_wl[k] if xoroshiro128p_uniform_float64(rng_states, thread_id) < spectrum_q[k] \
-                else spectrum_wl[spectrum_j[k]]
-
-            # find index for transformation
-            idx_trans_float = (wl - trans_wl[0]) / trans_wld
-            idx_trans = int(math.floor(idx_trans_float))
-            r = (idx_trans_float - idx_trans)
-
-            # do linear interpolation of transformation matrices
-            # m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans] + r * transf_deriv[:, idx_trans]
-            m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans]
-            dm0, dm1, dm2, dm3, dm4, dm5 = transf_deriv[:, idx_trans]
-            m0 += r * dm0
-            m1 += r * dm1
-            m2 += r * dm2
-            m3 += r * dm3
-            m4 += r * dm4
-            m5 += r * dm5
-
-            # random start points in slit
-            x = xoroshiro128p_uniform_float64(rng_states, thread_id)
-            y = xoroshiro128p_uniform_float64(rng_states, thread_id)
-            x, y = slitfun(x, y, rng_states, thread_id)
-
-            # transform
-            xt = m0 * x + m1 * y + m2
-            yt = m3 * x + m4 * y + m5
-
-            # apply PSF
-            idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
-            # next 3 lines implement drawing random number via alias sampling
-            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(psfs_j[idx_psf])))
-            if not xoroshiro128p_uniform_float64(rng_states, thread_id) < psfs_q[idx_psf][k]:
-                k = psfs_j[idx_psf][k]
-
-            # unravel 2d index
-            dy = k % psf_shape[1]
-            k = k // psf_shape[1]
-            dx = k % psf_shape[0]
-
-            # dx, dy = unravel_index(k, psf_shape)
-            xt += (dx - psf_shape[1] / 2.) * psf_sampling / pixelsize
-            yt += (dy - psf_shape[0] / 2.) * psf_sampling / pixelsize
-            x_int = int(math.floor(xt))
-            y_int = int(math.floor(yt))
-
-            if (0 <= x_int < max_x) and (0 <= y_int < max_y):
-                numba.cuda.atomic.inc(ccd, (y_int, x_int), 4294967295)
-
-    return cuda_kernel
-
-@memory.cache
-def make_cuda_kernel_singlemode():
-    @cuda.jit()
-    def cuda_kernel(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld,
-                    transf_deriv, psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd,
-                    pixelsize, rng_states, nphotons):
-        max_y, max_x = ccd.shape
-        thread_id = cuda.grid(1)
-
-        for _ in range(thread_id, nphotons, cuda.gridDim.x * cuda.blockDim.x):
-            # sample from spectrum
-            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(spectrum_j)))
-            wl = spectrum_wl[k] if xoroshiro128p_uniform_float64(rng_states, thread_id) < spectrum_q[k] \
-                else spectrum_wl[spectrum_j[k]]
-
-            # find index for transformation
-            idx_trans_float = (wl - trans_wl[0]) / trans_wld
-            idx_trans = int(math.floor(idx_trans_float))
-            r = (idx_trans_float - idx_trans)
-
-            # do linear interpolation of transformation matrices
-            xt = transformations[2, idx_trans]
-            yt = transformations[5, idx_trans]
-            dm2 = transf_deriv[2, idx_trans]
-            dm5 = transf_deriv[5, idx_trans]
-
-            xt += r * dm2
-            yt += r * dm5
-
-
-
-            # apply PSF
-            idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
-            # next 3 lines implement drawing random number via alias sampling
-            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(psfs_j[idx_psf])))
-            if not xoroshiro128p_uniform_float64(rng_states, thread_id) < psfs_q[idx_psf][k]:
-                k = psfs_j[idx_psf][k]
-
-            # unravel 2d index
-            dy = k % psf_shape[1]
-            k = k // psf_shape[1]
-            dx = k % psf_shape[0]
-
-            # dx, dy = unravel_index(k, psf_shape)
-            # random point within sampling element of PSF
-            dx_psf = xoroshiro128p_uniform_float64(rng_states, thread_id)
-            dy_psf = xoroshiro128p_uniform_float64(rng_states, thread_id)
-
-            xt += (dx - psf_shape[1] / 2. + dx_psf - 0.5) * psf_sampling / pixelsize
-            yt += (dy - psf_shape[0] / 2. + dy_psf - 0.5) * psf_sampling / pixelsize
-            x_int = int(math.floor(xt))
-            y_int = int(math.floor(yt))
-
-            if (0 <= x_int < max_x) and (0 <= y_int < max_y):
-                numba.cuda.atomic.inc(ccd, (y_int, x_int), 4294967295)
-
-    return cuda_kernel
-
-def raytrace_order_cuda(o, spec: Spectrograph, source: Source, telescope: Telescope, rv: float, t, ccd, ps, fiber: int,
-                        ccd_index: int, efficiency=None,
-                        seed=-1, cuda_kernel=None):
-    wavelength = np.linspace(*spec.get_wavelength_range(o, fiber, ccd_index), num=100000)
-
-    # get spectral density per order
-    spectral_density = source.get_spectral_density_rv(wavelength, rv)
-    # if source returns own wavelength vector, use that for further calculations instead of default grid
-    if isinstance(spectral_density, tuple):
-        wavelength, spectral_density = spectral_density
-
-    # for stellar targets calculate collected flux by telescope area
-    if source.stellar_target:
-        spectral_density *= telescope.area
-
-    # get efficiency per order
-    if efficiency is not None:
-        eff = efficiency.get_efficiency_per_order(wavelength=wavelength, order=o)
-        effective_density = eff * spectral_density
-    else:
-        effective_density = spectral_density
-
-    # calculate photon flux
-    if source.flux_in_photons:
-        flux = effective_density
-    else:
-        ch_factor = 5.03E12  # convert microwatts / micrometer to photons / s per wavelength interval
-        wl_diffs = np.ediff1d(wavelength, wavelength[-1] - wavelength[-2])
-        flux = effective_density * wavelength * wl_diffs * ch_factor
-
-    flux_photons = flux * t
-    total_photons = int(np.sum(flux_photons))
-    print(f'Order {o:3d}:    {(np.min(wavelength) * 1000.):7.1f} - {(np.max(wavelength) * 1000.):7.1f} nm.     '
-          f'Number of photons: {total_photons}')
-
-    minwl, maxwl = spec.get_wavelength_range(o, fiber, ccd_index)
-    trans_wl, trans_wld = np.linspace(minwl, maxwl, 10000, retstep=True)
-    transformations = convert_matrix(np.array(spec.get_transformation(trans_wl, o, fiber, ccd_index)))
-    # derivatives for simple linear interpolation
-    trans_deriv = np.array([np.ediff1d(t, t[-1] - t[-2]) for t in transformations])
-
-    psf_sampler_qj = np.array(
-        [make_alias_sampling_arrays(p.data.T.ravel()) for p in spec.get_psf(None, o, fiber, ccd_index)])
-
-    psfs_wl = np.array([p.wavelength for p in spec.get_psf(None, o, fiber, ccd_index)])
-    psfs_wld = np.ediff1d(psfs_wl, psfs_wl[-1] - psfs_wl[-2])
-    psf_shape = spec.get_psf(None, o, fiber, ccd_index)[0].data.shape
-
-    spectrum_sampler_q, spectrum_sampler_j = make_alias_sampling_arrays(np.asarray(flux_photons / np.sum(flux_photons),
-                                                                                   dtype=np.float32))
-
-    psf_sampling = spec.get_psf(None, o, fiber, ccd_index)[0].sampling
-
-    threads_per_block = 128
-    blocks = 64
-    rng_states = create_xoroshiro128p_states(threads_per_block * blocks, seed=seed)
-
-    cuda_kernel[threads_per_block, blocks](np.ascontiguousarray(wavelength), np.ascontiguousarray(spectrum_sampler_q),
-                                           np.ascontiguousarray(spectrum_sampler_j),
-                                           np.ascontiguousarray(transformations), np.ascontiguousarray(trans_wl),
-                                           trans_wld, np.ascontiguousarray(trans_deriv),
-                                           np.ascontiguousarray(psf_sampler_qj[:, 0]),
-                                           np.ascontiguousarray(psf_sampler_qj[:, 1]), np.ascontiguousarray(psfs_wl),
-                                           psfs_wld[0],
-                                           np.ascontiguousarray(psf_shape), psf_sampling,
-                                           ccd, float(ps), rng_states,
-                                           total_photons)
-    return total_photons
+import math
+import pathlib
+
+import numba
+import numba.cuda
+import numpy as np
+from joblib import Memory
+from numba import cuda
+from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float64
+
+from pyechelle.optics import convert_matrix
+from pyechelle.randomgen import make_alias_sampling_arrays
+from pyechelle.sources import Source
+from pyechelle.spectrograph import Spectrograph
+from pyechelle.telescope import Telescope
+
+path = pathlib.Path(__file__).parent.resolve()
+cache_path = path.joinpath('.cache')
+# create data directory if it doesn't exist:
+pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
+memory = Memory(cache_path, verbose=0)
+
+
+@memory.cache
+def make_cuda_kernel(slitfun):
+    @cuda.jit()
+    def cuda_kernel(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld,
+                    transf_deriv, psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd,
+                    pixelsize, rng_states, nphotons):
+        max_y, max_x = ccd.shape
+        thread_id = cuda.grid(1)
+
+        for _ in range(thread_id, nphotons, cuda.gridDim.x * cuda.blockDim.x):
+            # sample from spectrum
+            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(spectrum_j)))
+            wl = spectrum_wl[k] if xoroshiro128p_uniform_float64(rng_states, thread_id) < spectrum_q[k] \
+                else spectrum_wl[spectrum_j[k]]
+
+            # find index for transformation
+            idx_trans_float = (wl - trans_wl[0]) / trans_wld
+            idx_trans = int(math.floor(idx_trans_float))
+            r = (idx_trans_float - idx_trans)
+
+            # do linear interpolation of transformation matrices
+            # m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans] + r * transf_deriv[:, idx_trans]
+            m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans]
+            dm0, dm1, dm2, dm3, dm4, dm5 = transf_deriv[:, idx_trans]
+            m0 += r * dm0
+            m1 += r * dm1
+            m2 += r * dm2
+            m3 += r * dm3
+            m4 += r * dm4
+            m5 += r * dm5
+
+            # random start points in slit
+            x = xoroshiro128p_uniform_float64(rng_states, thread_id)
+            y = xoroshiro128p_uniform_float64(rng_states, thread_id)
+            x, y = slitfun(x, y, rng_states, thread_id)
+
+            # transform
+            xt = m0 * x + m1 * y + m2
+            yt = m3 * x + m4 * y + m5
+
+            # apply PSF
+            idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
+            # next 3 lines implement drawing random number via alias sampling
+            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(psfs_j[idx_psf])))
+            if not xoroshiro128p_uniform_float64(rng_states, thread_id) < psfs_q[idx_psf][k]:
+                k = psfs_j[idx_psf][k]
+
+            # unravel 2d index
+            dy = k % psf_shape[1]
+            k = k // psf_shape[1]
+            dx = k % psf_shape[0]
+
+            # dx, dy = unravel_index(k, psf_shape)
+            xt += (dx - psf_shape[1] / 2.) * psf_sampling / pixelsize
+            yt += (dy - psf_shape[0] / 2.) * psf_sampling / pixelsize
+            x_int = int(math.floor(xt))
+            y_int = int(math.floor(yt))
+
+            if (0 <= x_int < max_x) and (0 <= y_int < max_y):
+                numba.cuda.atomic.inc(ccd, (y_int, x_int), 4294967295)
+
+    return cuda_kernel
+
+
+@memory.cache
+def make_cuda_kernel_singlemode():
+    @cuda.jit()
+    def cuda_kernel(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld,
+                    transf_deriv, psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd,
+                    pixelsize, rng_states, nphotons):
+        max_y, max_x = ccd.shape
+        thread_id = cuda.grid(1)
+
+        for _ in range(thread_id, nphotons, cuda.gridDim.x * cuda.blockDim.x):
+            # sample from spectrum
+            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(spectrum_j)))
+            wl = spectrum_wl[k] if xoroshiro128p_uniform_float64(rng_states, thread_id) < spectrum_q[k] \
+                else spectrum_wl[spectrum_j[k]]
+
+            # find index for transformation
+            idx_trans_float = (wl - trans_wl[0]) / trans_wld
+            idx_trans = int(math.floor(idx_trans_float))
+            r = (idx_trans_float - idx_trans)
+
+            # do linear interpolation of transformation matrices
+            xt = transformations[2, idx_trans]
+            yt = transformations[5, idx_trans]
+            dm2 = transf_deriv[2, idx_trans]
+            dm5 = transf_deriv[5, idx_trans]
+
+            xt += r * dm2
+            yt += r * dm5
+
+            # apply PSF
+            idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
+            # next 3 lines implement drawing random number via alias sampling
+            k = int(math.floor(xoroshiro128p_uniform_float64(rng_states, thread_id) * len(psfs_j[idx_psf])))
+            if not xoroshiro128p_uniform_float64(rng_states, thread_id) < psfs_q[idx_psf][k]:
+                k = psfs_j[idx_psf][k]
+
+            # unravel 2d index
+            dy = k % psf_shape[1]
+            k = k // psf_shape[1]
+            dx = k % psf_shape[0]
+
+            # dx, dy = unravel_index(k, psf_shape)
+            # random point within sampling element of PSF
+            dx_psf = xoroshiro128p_uniform_float64(rng_states, thread_id)
+            dy_psf = xoroshiro128p_uniform_float64(rng_states, thread_id)
+
+            xt += (dx - psf_shape[1] / 2. + dx_psf - 0.5) * psf_sampling / pixelsize
+            yt += (dy - psf_shape[0] / 2. + dy_psf - 0.5) * psf_sampling / pixelsize
+            x_int = int(math.floor(xt))
+            y_int = int(math.floor(yt))
+
+            if (0 <= x_int < max_x) and (0 <= y_int < max_y):
+                numba.cuda.atomic.inc(ccd, (y_int, x_int), 4294967295)
+
+    return cuda_kernel
+
+
+def raytrace_order_cuda(o, spec: Spectrograph, source: Source, telescope: Telescope, rv: float, t, ccd, ps, fiber: int,
+                        ccd_index: int, efficiency=None,
+                        seed=-1, cuda_kernel=None):
+    wavelength = np.linspace(*spec.get_wavelength_range(o, fiber, ccd_index), num=100000)
+
+    # get spectral density per order
+    spectral_density = source.get_spectral_density_rv(wavelength, rv)
+    # if source returns own wavelength vector, use that for further calculations instead of default grid
+    if isinstance(spectral_density, tuple):
+        wavelength, spectral_density = spectral_density
+
+    # for stellar targets calculate collected flux by telescope area
+    if source.stellar_target:
+        spectral_density *= telescope.area
+
+    # get efficiency per order
+    if efficiency is not None:
+        eff = efficiency.get_efficiency_per_order(wavelength=wavelength, order=o)
+        effective_density = eff * spectral_density
+    else:
+        effective_density = spectral_density
+
+    # calculate photon flux
+    if source.flux_in_photons:
+        flux = effective_density
+    else:
+        ch_factor = 5.03E12  # convert microwatts / micrometer to photons / s per wavelength interval
+        wl_diffs = np.ediff1d(wavelength, wavelength[-1] - wavelength[-2])
+        flux = effective_density * wavelength * wl_diffs * ch_factor
+
+    flux_photons = flux * t
+    total_photons = int(np.sum(flux_photons))
+    print(f'Order {o:3d}:    {(np.min(wavelength) * 1000.):7.1f} - {(np.max(wavelength) * 1000.):7.1f} nm.     '
+          f'Number of photons: {total_photons}')
+
+    minwl, maxwl = spec.get_wavelength_range(o, fiber, ccd_index)
+    trans_wl, trans_wld = np.linspace(minwl, maxwl, 10000, retstep=True)
+    transformations = convert_matrix(np.array(spec.get_transformation(trans_wl, o, fiber, ccd_index)))
+    # derivatives for simple linear interpolation
+    trans_deriv = np.array([np.ediff1d(t, t[-1] - t[-2]) for t in transformations])
+
+    psf_sampler_qj = np.array(
+        [make_alias_sampling_arrays(p.data.T.ravel()) for p in spec.get_psf(None, o, fiber, ccd_index)])
+
+    psfs_wl = np.array([p.wavelength for p in spec.get_psf(None, o, fiber, ccd_index)])
+    psfs_wld = np.ediff1d(psfs_wl, psfs_wl[-1] - psfs_wl[-2])
+    psf_shape = spec.get_psf(None, o, fiber, ccd_index)[0].data.shape
+
+    spectrum_sampler_q, spectrum_sampler_j = make_alias_sampling_arrays(np.asarray(flux_photons / np.sum(flux_photons),
+                                                                                   dtype=np.float32))
+
+    psf_sampling = spec.get_psf(None, o, fiber, ccd_index)[0].sampling
+
+    threads_per_block = 128
+    blocks = 64
+    rng_states = create_xoroshiro128p_states(threads_per_block * blocks, seed=seed)
+
+    cuda_kernel[threads_per_block, blocks](np.ascontiguousarray(wavelength), np.ascontiguousarray(spectrum_sampler_q),
+                                           np.ascontiguousarray(spectrum_sampler_j),
+                                           np.ascontiguousarray(transformations), np.ascontiguousarray(trans_wl),
+                                           trans_wld, np.ascontiguousarray(trans_deriv),
+                                           np.ascontiguousarray(psf_sampler_qj[:, 0]),
+                                           np.ascontiguousarray(psf_sampler_qj[:, 1]), np.ascontiguousarray(psfs_wl),
+                                           psfs_wld[0],
+                                           np.ascontiguousarray(psf_shape), psf_sampling,
+                                           ccd, float(ps), rng_states,
+                                           total_photons)
+    return total_photons
```

### Comparing `pyechelle-0.3.5/pyechelle/raytracing.py` & `pyechelle-0.3.6/pyechelle/raytracing.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import math
-import random
-
-import numba.cuda
-import numpy as np
-
-from pyechelle.CCD import CCD
-from pyechelle.optics import convert_matrix
-from pyechelle.randomgen import make_alias_sampling_arrays, unravel_index
-from pyechelle.sources import Source
-from pyechelle.spectrograph import Spectrograph
-from pyechelle.telescope import Telescope
-
-
-@numba.njit(cache=True, parallel=False, nogil=True)
-def raytrace(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld, transf_deriv,
-             psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd, pixelsize, slitfun, nphotons):
-    max_y, max_x = ccd.shape
-
-    for _ in range(nphotons):
-        # sample from spectrum
-        k = int(math.floor(random.random() * len(spectrum_j)))
-        wl = spectrum_wl[k] if random.random() < spectrum_q[k] else spectrum_wl[spectrum_j[k]]
-
-        # find index for transformation
-        idx_trans_float = (wl - trans_wl[0]) / trans_wld
-        idx_trans = math.floor(idx_trans_float)
-        r = (idx_trans_float - idx_trans)
-
-        # do linear interpolation of transformation matrices
-        m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans] + r * transf_deriv[:, idx_trans]
-
-        # random start points in slit
-        x, y = slitfun(random.random(), random.random())
-        # transform
-        xt = m0 * x + m1 * y + m2
-        yt = m3 * x + m4 * y + m5
-
-        # apply PSF
-        idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
-        # next 3 lines implement drawing random number via alias sampling
-        k = int(math.floor(random.random() * len(psfs_j[idx_psf])))
-        if not random.random() < psfs_q[idx_psf][k]:
-            k = psfs_j[idx_psf][k]
-
-        dx, dy = unravel_index(k, psf_shape)
-        xt += (dx - psf_shape[1] / 2.) * psf_sampling / pixelsize
-        yt += (dy - psf_shape[0] / 2.) * psf_sampling / pixelsize
-        x_int = math.floor(xt)
-        y_int = math.floor(yt)
-
-        if (0 <= x_int < max_x) and (0 <= y_int < max_y):
-            ccd[y_int, x_int] += 1
-
-
-@numba.njit(cache=True, parallel=False, nogil=True)
-def raytrace_singlemode(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld, transf_deriv,
-                        psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd, pixelsize, nphotons):
-    max_y, max_x = ccd.shape
-
-    for _ in range(nphotons):
-        # sample from spectrum
-        k = int(math.floor(random.random() * len(spectrum_j)))
-        wl = spectrum_wl[k] if random.random() < spectrum_q[k] else spectrum_wl[spectrum_j[k]]
-
-        # find index for transformation
-        idx_trans_float = (wl - trans_wl[0]) / trans_wld
-        idx_trans = math.floor(idx_trans_float)
-        r = (idx_trans_float - idx_trans)
-
-        # do linear interpolation of transformation matrices (for SM this is not a full matrix, but just the
-        # translation coordinates for the chief ray
-        xt = transformations[2, idx_trans] + r * transf_deriv[2, idx_trans]
-        yt = transformations[5, idx_trans] + r * transf_deriv[5, idx_trans]
-
-        # apply PSF
-        idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
-        # next 3 lines implement drawing random number via alias sampling
-        k = int(math.floor(random.random() * len(psfs_j[idx_psf])))
-        if not random.random() < psfs_q[idx_psf][k]:
-            k = psfs_j[idx_psf][k]
-
-        dx, dy = unravel_index(k, psf_shape)
-        # here we add random.random()-0.5, so a uniform random number in [-0.5,0.5) that is applied to the 'integer' offset dx,dy
-        # this should be equivalent of drawing from a 'piecewise constant' distribution
-        xt += (dx - psf_shape[1] / 2. + random.random() - 0.5) * psf_sampling / pixelsize
-        yt += (dy - psf_shape[0] / 2. + random.random() - 0.5) * psf_sampling / pixelsize
-        x_int = math.floor(xt)
-        y_int = math.floor(yt)
-
-        if (0 <= x_int < max_x) and (0 <= y_int < max_y):
-            ccd[y_int, x_int] += 1
-
-
-def raytrace_order_cpu(o, spec: Spectrograph, source: Source, slit_fun: callable,
-                       telescope: Telescope, rv: float, t, ccd: CCD, fiber: int, ccd_index: int, efficiency=None,
-                       n_cpu=1):
-    wavelength = np.linspace(*spec.get_wavelength_range(o, fiber, ccd_index), num=100000)
-
-    # get spectral density per order
-    spectral_density = source.get_spectral_density_rv(wavelength, rv)
-    # if source returns own wavelength vector, use that for further calculations instead of default grid
-    if isinstance(spectral_density, tuple):
-        wavelength, spectral_density = spectral_density
-
-    # for stellar targets calculate collected flux by telescope area
-    if source.stellar_target:
-        spectral_density *= telescope.area
-
-    # get efficiency per order
-    if efficiency is not None:
-        eff = efficiency.get_efficiency_per_order(wavelength=wavelength, order=o)
-        effective_density = eff * spectral_density
-    else:
-        effective_density = spectral_density
-
-    # calculate photon flux
-    if source.flux_in_photons:
-        flux = effective_density
-    else:
-        ch_factor = 5.03E12  # convert microwatts / micrometer to photons / s per wavelength interval
-        wl_diffs = np.ediff1d(wavelength, wavelength[-1] - wavelength[-2])
-        flux = effective_density * wavelength * wl_diffs * ch_factor
-
-    flux_photons = flux * t
-    total_photons = int(np.sum(flux_photons))
-    print(f'Order {o:3d}:    {(np.min(wavelength) * 1000.):7.1f} - {(np.max(wavelength) * 1000.):7.1f} nm.     '
-          f'Number of photons: {total_photons}')
-
-    minwl, maxwl = spec.get_wavelength_range(o, fiber, ccd_index)
-    trans_wl, trans_wld = np.linspace(minwl, maxwl, 10000, retstep=True)
-    transformations = convert_matrix(np.array(spec.get_transformation(trans_wl, o, fiber, ccd_index)))
-
-    # transformations = np.array(spec.transformations[f'order{o}'].get_matrices_spline(trans_wl))
-    # derivatives for simple linear interpolation
-    trans_deriv = np.array([np.ediff1d(t, t[-1] - t[-2]) for t in transformations])
-
-    psf_sampler_qj = np.array(
-        [make_alias_sampling_arrays(p.data.T.ravel()) for p in spec.get_psf(None, o, fiber, ccd_index)])
-
-    psfs_wl = np.array([p.wavelength for p in spec.get_psf(None, o, fiber, ccd_index)])
-    psfs_wld = np.ediff1d(psfs_wl, psfs_wl[-1] - psfs_wl[-2])
-    psf_shape = spec.get_psf(None, o, fiber, ccd_index)[0].data.shape
-
-    spectrum_sampler_q, spectrum_sampler_j = make_alias_sampling_arrays(np.asarray(flux_photons / np.sum(flux_photons),
-                                                                                   dtype=np.float32))
-
-    psf_sampling = spec.get_psf(None, o, fiber, ccd_index)[0].sampling
-    if n_cpu > 1:
-        ccd_new = np.zeros_like(ccd.data, dtype=np.uint32)
-        if slit_fun is not None:
-            raytrace(wavelength, spectrum_sampler_q, spectrum_sampler_j,
-                     transformations, trans_wl, trans_wld, trans_deriv,
-                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
-                     ccd_new, float(ccd.pixelsize), slit_fun, total_photons)
-        else:
-            raytrace_singlemode(wavelength, spectrum_sampler_q, spectrum_sampler_j,
-                                transformations, trans_wl, trans_wld, trans_deriv,
-                                psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape,
-                                psf_sampling,
-                                ccd_new, float(ccd.pixelsize), total_photons)
-        return ccd_new, total_photons
-    else:
-        if slit_fun is not None:
-            raytrace(wavelength, spectrum_sampler_q, spectrum_sampler_j,
-                     transformations, trans_wl, trans_wld, trans_deriv,
-                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
-                     ccd.data, float(ccd.pixelsize), slit_fun, total_photons)
-        else:
-            raytrace_singlemode(wavelength, spectrum_sampler_q, spectrum_sampler_j,
-                     transformations, trans_wl, trans_wld, trans_deriv,
-                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
-                     ccd.data, float(ccd.pixelsize), total_photons)
-        return total_photons
+import math
+import random
+
+import numba.cuda
+import numpy as np
+
+from pyechelle.CCD import CCD
+from pyechelle.optics import convert_matrix
+from pyechelle.randomgen import make_alias_sampling_arrays, unravel_index
+from pyechelle.sources import Source
+from pyechelle.spectrograph import Spectrograph
+from pyechelle.telescope import Telescope
+
+
+@numba.njit(cache=True, parallel=False, nogil=True)
+def raytrace(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld, transf_deriv,
+             psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd, pixelsize, slitfun, nphotons):
+    max_y, max_x = ccd.shape
+
+    for _ in range(nphotons):
+        # sample from spectrum
+        k = int(math.floor(random.random() * len(spectrum_j)))
+        wl = spectrum_wl[k] if random.random() < spectrum_q[k] else spectrum_wl[spectrum_j[k]]
+
+        # find index for transformation
+        idx_trans_float = (wl - trans_wl[0]) / trans_wld
+        idx_trans = math.floor(idx_trans_float)
+        r = (idx_trans_float - idx_trans)
+
+        # do linear interpolation of transformation matrices
+        m0, m1, m2, m3, m4, m5 = transformations[:, idx_trans] + r * transf_deriv[:, idx_trans]
+
+        # random start points in slit
+        x, y = slitfun(random.random(), random.random())
+        # transform
+        xt = m0 * x + m1 * y + m2
+        yt = m3 * x + m4 * y + m5
+
+        # apply PSF
+        idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
+        # next 3 lines implement drawing random number via alias sampling
+        k = int(math.floor(random.random() * len(psfs_j[idx_psf])))
+        if not random.random() < psfs_q[idx_psf][k]:
+            k = psfs_j[idx_psf][k]
+
+        dx, dy = unravel_index(k, psf_shape)
+        xt += (dx - psf_shape[1] / 2.) * psf_sampling / pixelsize
+        yt += (dy - psf_shape[0] / 2.) * psf_sampling / pixelsize
+        x_int = math.floor(xt)
+        y_int = math.floor(yt)
+
+        if (0 <= x_int < max_x) and (0 <= y_int < max_y):
+            ccd[y_int, x_int] += 1
+
+
+@numba.njit(cache=True, parallel=False, nogil=True)
+def raytrace_singlemode(spectrum_wl, spectrum_q, spectrum_j, transformations, trans_wl, trans_wld, transf_deriv,
+                        psfs_q, psfs_j, psf_wl, psf_wld, psf_shape, psf_sampling, ccd, pixelsize, nphotons):
+    max_y, max_x = ccd.shape
+
+    for _ in range(nphotons):
+        # sample from spectrum
+        k = int(math.floor(random.random() * len(spectrum_j)))
+        wl = spectrum_wl[k] if random.random() < spectrum_q[k] else spectrum_wl[spectrum_j[k]]
+
+        # find index for transformation
+        idx_trans_float = (wl - trans_wl[0]) / trans_wld
+        idx_trans = math.floor(idx_trans_float)
+        r = (idx_trans_float - idx_trans)
+
+        # do linear interpolation of transformation matrices (for SM this is not a full matrix, but just the
+        # translation coordinates for the chief ray
+        xt = transformations[2, idx_trans] + r * transf_deriv[2, idx_trans]
+        yt = transformations[5, idx_trans] + r * transf_deriv[5, idx_trans]
+
+        # apply PSF
+        idx_psf = int((wl - psf_wl[0]) / psf_wld)  # find psf index
+        # next 3 lines implement drawing random number via alias sampling
+        k = int(math.floor(random.random() * len(psfs_j[idx_psf])))
+        if not random.random() < psfs_q[idx_psf][k]:
+            k = psfs_j[idx_psf][k]
+
+        dx, dy = unravel_index(k, psf_shape)
+        # here we add random.random()-0.5, so a uniform random number in [-0.5,0.5) that is applied to the 'integer' offset dx,dy
+        # this should be equivalent of drawing from a 'piecewise constant' distribution
+        xt += (dx - psf_shape[1] / 2. + random.random() - 0.5) * psf_sampling / pixelsize
+        yt += (dy - psf_shape[0] / 2. + random.random() - 0.5) * psf_sampling / pixelsize
+        x_int = math.floor(xt)
+        y_int = math.floor(yt)
+
+        if (0 <= x_int < max_x) and (0 <= y_int < max_y):
+            ccd[y_int, x_int] += 1
+
+
+def raytrace_order_cpu(o, spec: Spectrograph, source: Source, slit_fun: callable,
+                       telescope: Telescope, rv: float, t, ccd: CCD, fiber: int, ccd_index: int, efficiency=None,
+                       n_cpu=1):
+    wavelength = np.linspace(*spec.get_wavelength_range(o, fiber, ccd_index), num=100000)
+
+    # get spectral density per order
+    spectral_density = source.get_spectral_density_rv(wavelength, rv)
+    # if source returns own wavelength vector, use that for further calculations instead of default grid
+    if isinstance(spectral_density, tuple):
+        wavelength, spectral_density = spectral_density
+
+    # for stellar targets calculate collected flux by telescope area
+    if source.stellar_target:
+        spectral_density *= telescope.area
+
+    # get efficiency per order
+    if efficiency is not None:
+        eff = efficiency.get_efficiency_per_order(wavelength=wavelength, order=o)
+        effective_density = eff * spectral_density
+    else:
+        effective_density = spectral_density
+
+    # calculate photon flux
+    if source.flux_in_photons:
+        flux = effective_density
+    else:
+        ch_factor = 5.03E12  # convert microwatts / micrometer to photons / s per wavelength interval
+        wl_diffs = np.ediff1d(wavelength, wavelength[-1] - wavelength[-2])
+        flux = effective_density * wavelength * wl_diffs * ch_factor
+
+    flux_photons = flux * t
+    total_photons = int(np.sum(flux_photons))
+    print(f'Order {o:3d}:    {(np.min(wavelength) * 1000.):7.1f} - {(np.max(wavelength) * 1000.):7.1f} nm.     '
+          f'Number of photons: {total_photons}')
+
+    minwl, maxwl = spec.get_wavelength_range(o, fiber, ccd_index)
+    trans_wl, trans_wld = np.linspace(minwl, maxwl, 10000, retstep=True)
+    transformations = convert_matrix(np.array(spec.get_transformation(trans_wl, o, fiber, ccd_index)))
+
+    # transformations = np.array(spec.transformations[f'order{o}'].get_matrices_spline(trans_wl))
+    # derivatives for simple linear interpolation
+    trans_deriv = np.array([np.ediff1d(t, t[-1] - t[-2]) for t in transformations])
+
+    psf_sampler_qj = np.array(
+        [make_alias_sampling_arrays(p.data.T.ravel()) for p in spec.get_psf(None, o, fiber, ccd_index)])
+
+    psfs_wl = np.array([p.wavelength for p in spec.get_psf(None, o, fiber, ccd_index)])
+    psfs_wld = np.ediff1d(psfs_wl, psfs_wl[-1] - psfs_wl[-2])
+    psf_shape = spec.get_psf(None, o, fiber, ccd_index)[0].data.shape
+
+    spectrum_sampler_q, spectrum_sampler_j = make_alias_sampling_arrays(np.asarray(flux_photons / np.sum(flux_photons),
+                                                                                   dtype=np.float32))
+
+    psf_sampling = spec.get_psf(None, o, fiber, ccd_index)[0].sampling
+    if n_cpu > 1:
+        ccd_new = np.zeros_like(ccd.data, dtype=np.uint32)
+        if slit_fun is not None:
+            raytrace(wavelength, spectrum_sampler_q, spectrum_sampler_j,
+                     transformations, trans_wl, trans_wld, trans_deriv,
+                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
+                     ccd_new, float(ccd.pixelsize), slit_fun, total_photons)
+        else:
+            raytrace_singlemode(wavelength, spectrum_sampler_q, spectrum_sampler_j,
+                                transformations, trans_wl, trans_wld, trans_deriv,
+                                psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape,
+                                psf_sampling,
+                                ccd_new, float(ccd.pixelsize), total_photons)
+        return ccd_new, total_photons
+    else:
+        if slit_fun is not None:
+            raytrace(wavelength, spectrum_sampler_q, spectrum_sampler_j,
+                     transformations, trans_wl, trans_wld, trans_deriv,
+                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
+                     ccd.data, float(ccd.pixelsize), slit_fun, total_photons)
+        else:
+            raytrace_singlemode(wavelength, spectrum_sampler_q, spectrum_sampler_j,
+                     transformations, trans_wl, trans_wld, trans_deriv,
+                     psf_sampler_qj[:, 0], psf_sampler_qj[:, 1], psfs_wl, psfs_wld[0], psf_shape, psf_sampling,
+                     ccd.data, float(ccd.pixelsize), total_photons)
+        return total_photons
```

### Comparing `pyechelle-0.3.5/pyechelle/simulator.py` & `pyechelle-0.3.6/pyechelle/simulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,588 +1,591 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
-import argparse
-import distutils.util
-import inspect
-import logging
-import pathlib
-import re
-import sys
-import time
-from dataclasses import field, dataclass
-from pathlib import Path
-
-import numpy as np
-from astropy.io import fits
-from joblib import Parallel, delayed
-from numba import cuda
-
-import pyechelle
-import pyechelle.slit
-from pyechelle import sources
-from pyechelle.CCD import CCD
-from pyechelle.efficiency import Efficiency, CSVEfficiency, SystemEfficiency, Atmosphere
-from pyechelle.raytrace_cuda import make_cuda_kernel, raytrace_order_cuda, make_cuda_kernel_singlemode
-from pyechelle.raytracing import raytrace_order_cpu
-from pyechelle.sources import CSV
-from pyechelle.sources import Phoenix, Source
-from pyechelle.spectrograph import Spectrograph, ZEMAX
-from pyechelle.telescope import Telescope
-
-logger = logging.getLogger('Simulator')
-logger.setLevel(level=logging.INFO)
-
-# get list of available spectrograph models
-dir_path = Path(__file__).resolve().parent.joinpath("models").joinpath("available_models.txt")
-with open(dir_path, 'r') as am:
-    available_models = [line.strip() for line in am.readlines() if line.strip() != '']
-
-# get list of available sources
-available_sources = [m[0] for m in inspect.getmembers(pyechelle.sources, inspect.isclass) if
-                     issubclass(m[1], pyechelle.sources.Source) and m[0] != "Source"]
-
-
-def parse_num_list(string_list: str) -> list:
-    """
-    Converts a string specifying a range of numbers (e.g. '1-3') into a list of these numbers ([1,2,3])
-    Args:
-        string_list: string like "[start value]-[end value]"
-
-    Returns:
-        List of integers
-    """
-
-    m = re.match(r'(\d+)(?:-(\d+))?$', string_list)
-    if not m:
-        raise argparse.ArgumentTypeError(
-            "'" + string_list + "' is not a range of number. Expected forms like '0-5' or '2'.")
-    start = m.group(1)
-    end = m.group(2) or start
-    return list(range(int(start, 10), int(end, 10) + 1))
-
-
-def export_to_html(data, filename, include_plotlyjs=False):
-    """
-    Exports a 2D image into a 'standalone' HTML file. This is used e.g. for some examples in the documentation.
-    Args:
-        data: 2d numpy array
-        filename: output filename
-        include_plotlyjs: whether plotlyjs is included in html file or not
-
-    Returns:
-        None
-    """
-    import plotly.express as px
-    fig = px.imshow(data, binary_string=True, aspect='equal')
-
-    fig.update_traces(
-        hovertemplate=None,
-        hoverinfo='skip'
-    )
-    w = 1000
-    h = 300
-    fig.update_layout(autosize=True, width=w, height=h, margin=dict(l=0, r=0, b=0, t=0))
-    fig.update_yaxes(range=[2000, 3000])
-    fig.write_html(filename, include_plotlyjs=include_plotlyjs)
-
-
-def log_elapsed_time(msg: str, t0: float) -> float:
-    t1 = time.time()
-    logger.info(msg + f' (took {t1 - t0:2f} s )')
-    return t1
-
-
-def write_to_fits(c: CCD, filename: str | Path, overwrite: bool = True, append: bool = False):
-    """ Saves CCD image to disk
-
-    Args:
-        c: CCD object
-        filename: filepath
-        overwrite: if True, file will be overwritten if existing
-        append: if True, CCD data will be added to data in fits file
-
-    Returns:
-        None
-    """
-    old_file_data = np.zeros_like(c.data)
-    if append:
-        if pathlib.Path(filename).is_file():
-            old_file_data = fits.getdata(filename)
-            assert old_file_data.shape == c.data.shape, f"You tried to append data to {filename}, " \
-                                                        f"but the fits file contains" \
-                                                        f"data with a different shape ({old_file_data.shape})."
-    hdu = fits.PrimaryHDU(data=np.array(c.data + old_file_data, dtype=int))
-    hdu_list = fits.HDUList([hdu])
-    hdu_list.writeto(filename, overwrite=overwrite or append)
-
-
-@dataclass
-class Simulator:
-    """ PyEchelle simulator
-
-    Simulator class that contains everything needed to generate spectra.
-
-    Attributes:
-        spectrograph (Spectrograph): spectrograph used for simulations
-        fibers (list[int]): fiber / list of fibers to be simulated
-        orders (list[int]): order / list of diffraction orders to be simulated
-        sources (list[Source]): spectral source / list of spectral sources per fiber (same length as fibers)
-        atmosphere (list[bool]): whether to include atmospheric transmission per fiber (same length as fibers)
-        atmosphere_conditions (list[dict | None]): skycalc arguments for atmospheric conditions (same length as sources)
-        rvs (list[float]): radial velocity shifts in [m/s] for sources (same length as fibers)
-        telescope (Telescope): Telescope used for simulations (relevant for 'on-sky' sources)
-        random_seed (int): random seed for the number generator
-        cuda (bool): flat if CUDA is to be used
-        max_cpu (int): number of CPUs used for simulation (if -1, max_cpu is number of available cores)
-        exp_time (float): exposure time to be simulated
-        output (Path): path to output fits file
-        append (bool): flag if simulated counts should be appended to existing image
-        overwrite (bool): flat if output file should be overwritten if existing
-        global_efficiency (Efficiency): overall efficiency curve to be considered
-         (on top of spectrograph efficiency curve and potentially atmosphere)
-
-    """
-    spectrograph: Spectrograph
-    fibers: list[int] = field(init=False, default=None)
-    orders: list[int] = field(init=False, default=None)
-    ccd: int = field(init=False, default=None)
-    sources: list[Source] = field(init=False, default=None)
-    atmosphere: list[bool] = field(init=False, default=None)
-    atmosphere_conditions: list[dict | None] = field(init=False, default=None)
-    rvs: list[float] = field(init=False, default=None)
-    telescope: Telescope = field(init=False, default=None)
-    random_seed: int = field(init=False, default=-1)
-    cuda: bool = field(init=False, default=False)
-    max_cpu: int = field(init=False, default=1)
-    exp_time: float = field(init=False, default=1.)
-    output: Path = field(init=False, default=None)
-    append: bool = field(init=False, default=False)
-    overwrite: bool = field(init=False, default=False)
-    bias: int = field(init=False, default=0)
-    read_noise: float = field(init=False, default=0.)
-    global_efficiency: Efficiency = field(init=False, default=None)
-
-    def set_sources(self, source: Source | list[Source]):
-        assert self.fibers is not None, 'Please set first the fields that you want to simulate.'
-        self.sources = source if isinstance(source, list) else [source] * len(self.fibers)
-        assert len(self.fibers) == len(self.sources), \
-            'Number of sources needs to match the number of fields/fibers (or be 1)'
-
-    def set_atmospheres(self, atmosphere: bool | list[bool], sky_calc_kwargs: dict | list[dict] = None):
-        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
-        self.atmosphere = [atmosphere] * len(self.sources) if isinstance(atmosphere, bool) else atmosphere
-        self.atmosphere_conditions = [sky_calc_kwargs] * len(self.sources) if (
-                isinstance(sky_calc_kwargs, dict) or sky_calc_kwargs is None) else sky_calc_kwargs
-        assert len(self.atmosphere) == len(self.sources), \
-            'Number of atmosphere flags needs to match the number of sources (or be 1)'
-        assert len(self.atmosphere_conditions) == len(self.sources), \
-            'Number of atmosphere condition arguments needs to match the number of sources (or be 1)'
-
-    def set_radial_velocities(self, rvs: float | list[float]):
-        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
-        self.rvs = [rvs] * len(self.sources) if isinstance(rvs, float) else rvs
-        assert len(self.rvs) == len(self.sources), \
-            'Number of radial velocity values needs to match the number of sources (or be 1)'
-
-    def set_telescope(self, telescope: Telescope):
-        self.telescope = telescope
-
-    def set_ccd(self, ccd: int):
-        self.ccd = ccd
-        assert self.ccd in self.spectrograph.get_ccd().keys(), f'You requested simulation of CCD {ccd}, ' \
-                                                               f'which is not available.'
-
-    def set_efficiency(self, eff: Efficiency):
-        assert isinstance(eff, Efficiency)
-        self.global_efficiency = eff
-
-    def set_bias(self, bias_value: int = 0):
-        self.bias = bias_value
-
-    def set_read_noise(self, read_noise: float = 0.):
-        if read_noise > 0.0:
-            assert self.bias > 0, "read noise was specified, but no bias value is set, yet. " \
-                                  "Do so before setting the read noise."
-        self.read_noise = read_noise
-
-    def set_fibers(self, fiber: int | list[int]):
-        assert self.ccd is not None, 'Please set CCD index first.'
-        self.fibers = [fiber] if isinstance(fiber, int) else fiber
-        for f in self.fibers:
-            assert f in self.spectrograph.get_fibers(self.ccd), f'You requested simulation of fiber {f}, which is ' \
-                                                                f'not available for ccd with index {self.ccd}'
-
-    def set_cuda(self, activate: bool = True, seed: int = -1):
-        self.cuda = activate
-        self.random_seed = seed
-
-    def _get_valid_orders(self, fiber: int):
-        valid_orders = []
-
-        requested_orders = self.spectrograph.get_orders(fiber, self.ccd) if self.orders is None else self.orders
-        for o in requested_orders:
-            if o in self.spectrograph.get_orders(fiber, self.ccd):
-                valid_orders.append(o)
-            else:
-                logger.warning(f'Order {o} is requested, but it is not in the Spectrograph model.')
-        return valid_orders
-
-    def _get_slit_function(self, fiber: int):
-        try:
-            if self.cuda:
-                slit_fun = getattr(pyechelle.slit, f"cuda_{self.spectrograph.get_field_shape(fiber, self.ccd)}")
-            else:
-                slit_fun = getattr(pyechelle.slit, self.spectrograph.get_field_shape(fiber, self.ccd))
-        except AttributeError:
-            raise NotImplementedError(
-                f"Field shape {self.spectrograph.get_field_shape(fiber, self.ccd)} is not implemented.")
-        return slit_fun
-
-    def _simulate_multi_cpu(self, orders, fiber, ccd_index, slit_fun, s, rv, integration_time, c, efficiency):
-        simulated_photons = []
-        t0 = time.time()
-        results = Parallel(n_jobs=min(self.max_cpu, len(orders)), backend="threading")(
-            delayed(raytrace_order_cpu)(o, self.spectrograph, s, slit_fun, self.telescope, rv,
-                                        integration_time,
-                                        c, fiber, ccd_index,
-                                        efficiency, self.max_cpu) for o in np.sort(orders))
-        logger.info('Add up orders...')
-        ccd_results = [r[0] for r in results]
-        simulated_photons.extend([r[1] for r in results])
-        c.data = np.sum(ccd_results, axis=0)
-        log_elapsed_time('done.', t0)
-        return simulated_photons
-
-    def _simulate_single_cpu(self, orders, fiber, ccd_index, s, slit_fun, rv, integration_time, c, efficiency):
-        simulated_photons = []
-        for o in np.sort(orders):
-            nphot = raytrace_order_cpu(o, self.spectrograph, s, slit_fun, self.telescope, rv,
-                                       integration_time,
-                                       c, fiber, ccd_index,
-                                       efficiency,
-                                       1)
-            simulated_photons.append(nphot)
-        return simulated_photons
-
-    def _simulate_cuda(self, orders, slit_fun, rv, integration_time, dccd, efficiency, s, c, fiber, ccd_index):
-        if slit_fun is not None:  # multimode
-            cuda_kernel = make_cuda_kernel(slit_fun)
-        else:  # singlemode
-            cuda_kernel = make_cuda_kernel_singlemode()
-        simulated_photons = []
-        for o in np.sort(orders):
-            nphot = raytrace_order_cuda(o, self.spectrograph, s, self.telescope, rv, integration_time, dccd,
-                                        float(c.pixelsize), fiber, ccd_index, efficiency, seed=self.random_seed,
-                                        cuda_kernel=cuda_kernel)
-            simulated_photons.append(nphot)
-        return simulated_photons
-
-    def validate(self):
-        assert self.fibers is not None, 'Please set fibers for simulation'
-        assert self.ccd is not None, 'Please set ccd index/indices for simulation'
-        assert self.output is not None, 'Please set output path for simulation'
-        if self.atmosphere is None:
-            logger.info('It was not explicitly specified whether to consider atmospheric transmission. '
-                        'It is set to False')
-            self.atmosphere = [False] * len(self.sources)
-
-        if self.atmosphere_conditions is None:
-            if self.atmosphere:
-                logger.info('Atmospheric conditions were not specified. The default atmospheric conditions apply. '
-                            '(e.g. airmass 1)')
-            self.atmosphere_conditions = [None] * len(self.sources)
-
-        if self.rvs is None:
-            logger.info('Radial velocities are not specified explicitly. They are therefore set to 0.0')
-            self.rvs = [0.0] * len(self.sources)
-        if self.output.is_file():
-            assert self.overwrite or self.append, f'You specified to save the simulation at {self.output}, ' \
-                                                  f'but this file exists. If you want to overwrite, ' \
-                                                  f'please set the overwrite flag. Or in case you want to append to ' \
-                                                  f'the file: please set the append flag'
-        return True
-
-    def run(self):
-        self.validate()
-        c = self.spectrograph.get_ccd(self.ccd)
-        total_simulated_photons = []
-        t1 = time.time()
-        # copy empty array to CUDA device
-        if self.cuda:
-            dccd = cuda.to_device(np.zeros_like(c.data, dtype=np.uint32))
-
-        for f, s, atm, atm_cond, rv in zip(self.fibers, self.sources, self.atmosphere, self.atmosphere_conditions,
-                                           self.rvs):
-            orders = self.orders if self.orders is not None else self._get_valid_orders(f)
-            slit_fun = self._get_slit_function(f)
-            if self.global_efficiency is None:
-                if atm:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd),
-                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
-                                         'Combined Efficiency')
-                else:
-                    e = self.spectrograph.get_efficiency(f, self.ccd)
-            else:
-                if atm:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency,
-                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
-                                         'Combined Efficiency')
-                else:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency],
-                                         'Combined Efficiency')
-
-            if not self.cuda:
-                if self.max_cpu > 1:
-                    total_simulated_photons.extend(
-                        self._simulate_multi_cpu(orders, f, self.ccd, slit_fun, s, rv, self.exp_time, c, e))
-                else:
-                    total_simulated_photons.extend(
-                        self._simulate_single_cpu(orders, f, self.ccd, s, slit_fun, rv, self.exp_time, c, e))
-            else:
-                total_simulated_photons.extend(
-                    self._simulate_cuda(orders, slit_fun, rv, self.exp_time, dccd, e, s, c, f, self.ccd))
-
-        if self.cuda:
-            dccd.copy_to_host(c.data)
-        logger.info('Finish up simulation and save...')
-        c.clip()
-
-        # add bias / global ccd effects
-        if self.bias > 0:
-            c.add_bias(self.bias)
-        if self.read_noise > 0.:
-            c.add_readnoise(self.read_noise)
-        t2 = time.time()
-
-        write_to_fits(c, self.output, self.overwrite, self.append)
-        logger.info(f"Total time for simulation: {t2 - t1:.3f}s.")
-        logger.info(f"Total simulated photons: {sum(total_simulated_photons)}")
-        return sum(total_simulated_photons)
-
-    def set_exposure_time(self, exp_time: float = 1):
-        self.exp_time = exp_time
-
-    def set_output(self, path: str | Path = Path().cwd().joinpath('test.fits'),
-                   append: bool = False, overwrite: bool = False):
-
-        self.output = path if isinstance(path, Path) else Path(path)
-        self.append = append
-        self.overwrite = overwrite
-        if append and not self.output.is_file():
-            logger.warning(f'You specified that the simulation should be appended to {self.output}, but there is no '
-                           f'such file. It will be created.')
-
-    def set_orders(self, orders: int | list[int] | None):
-        if isinstance(orders, int):
-            self.orders = [orders]
-        self.orders = orders
-        if self.orders is not None:
-            for f in self.fibers:
-                valid_orders = self._get_valid_orders(f)
-                for o in self.orders:
-                    assert o in valid_orders, f'You requested to simulate order {o}, but this order is not available' \
-                                              f'on CCD {self.ccd} and fiber/field {f}'
-
-
-def generate_parser():
-    parser = argparse.ArgumentParser(description='PyEchelle Simulator',
-                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
-                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
-    parser.add_argument('--ccd', type=int, default=1, required=False, help='Sets CCD index to be simulated.')
-    parser.add_argument('-t', '--integration_time', type=float, default=1.0, required=False,
-                        help=f"Integration time for the simulation in seconds [s].")
-    parser.add_argument('--fiber', type=parse_num_list, required=False,
-                        help='Fiber/Field number(s) to be simulated. Can either be a single integer, or an integer'
-                             'range (e.g. 1-3) ')
-    parser.add_argument('--no_blaze', action='store_true',
-                        help='If set, the blaze efficiency per order will be ignored.')
-    parser.add_argument('--no_efficiency', action='store_true',
-                        help='If set, all instrument/atmosphere efficiencies will be ignored.')
-
-    parser.add_argument('--cuda', action='store_true',
-                        help='If set, CUDA will be used for raytracing. Note: the max_cpu flag is then obsolete.')
-
-    parser.add_argument('--cuda_seed', type=int, default=-1,
-                        help='Random seed for generating CUDA RNG states. If <0, then the seed is choosen randomly.')
-
-    parser.add_argument('--max_cpu', type=int, default=1,
-                        help="Maximum number of CPU cores used. Note: The parallelization happens 'per order'."
-                             " Order-wise images are added up. This requires a large amount of memory at the moment."
-                             "If planning on simulating multiple images, consider using only 1 CPU per simulation "
-                             "and starting multiple simulations instead.")
-
-    atmosphere_group = parser.add_argument_group('Atmosphere')
-    atmosphere_group.add_argument('--atmosphere', nargs='+', required=False,
-                                  help='Add telluric lines to spectrum. For adding tellurics to all spectra just use'
-                                       '--atmosphere Y, for specifying per fiber user e.g. --atmosphere Y N Y',
-                                  type=lambda x: bool(distutils.util.strtobool(x)), default=[False])
-
-    atmosphere_group.add_argument('--airmass', default=1.0, type=float, required=False,
-                                  help='airmass for atmospheric model')
-
-    telescope_group = parser.add_argument_group('Telescope settings')
-    telescope_group.add_argument('--d_primary', type=float, required=False, default=1.0,
-                                 help='Diameter of the primary telescope mirror.')
-    telescope_group.add_argument('--d_secondary', type=float, required=False, default=0,
-                                 help='Diameter of the secondary telescope mirror.')
-
-    parser.add_argument('--orders', type=parse_num_list, nargs='+', required=False,
-                        help='Echelle/Grating order numbers to simulate... '
-                             'if not specified, all orders of the spectrograph are simulated.'
-                             'Can either be a single integer, or a range (e.g. 80-90)')
-
-    parser.add_argument('--sources', nargs='+', choices=available_sources, required=True,
-                        help='Spectral source for the simulation. Can either be a single string, e.g. "Etalon",'
-                             ' or a comma separated list of sources (e.g. "Etalon, Constant, Etalon") which length must'
-                             'match the number of fields/fibers.')
-    parser.add_argument('--rv', nargs='+', type=float, required=False, default=[0.],
-                        help="radial velocity shift of source")
-    const_source_group = parser.add_argument_group('Constant source')
-    const_source_group.add_argument('--constant_intensity', type=float, default=0.0001, required=False,
-                                    help="Flux in microWatts / nanometer for constant flux spectral source")
-    arclamps_group = parser.add_argument_group('Arc Lamps')
-    arclamps_group.add_argument('--scale', default=10.0, required=False,
-                                help='Intensity scale of gas lines (e.g. Ag or Ne) vs metal (Th)')
-
-    csv_group = parser.add_argument_group('CSV')
-    csv_group.add_argument('--csv_filepath', type=argparse.FileType('r'), required=False,
-                           help="Path to .csv file that contains two columns: wavelength and flux. The flux is expected"
-                                "to be in ergs/s/cm^2/cm (like Phoenix spectra) or photons (then set it via "
-                                "--csv_flux_in_photons). The wavelength unit is expected to "
-                                "be angstroms, but it can be changed via --csv_wavelength_unit")
-    csv_group.add_argument('--csv_wavelength_unit', choices=list(CSV.wavelength_scaling.keys()), default='a', type=str,
-                           help=f"Unit of the wavelength column in the .csv file. Options are "
-                                f"{list(CSV.wavelength_scaling.keys())}")
-    csv_group.add_argument('--csv_list_like', type=bool, default=False, help='Set to True if spectrum is discrete.')
-    csv_group.add_argument('--csv_flux_in_photons', type=bool, default=False,
-                           help='Set to True if flux is given in Photons/s rather than ergs')
-    csv_group.add_argument('--csv_stellar_target', type=bool, default=True,
-                           help='Set to True if Source is a stellar target.')
-    csv_group.add_argument('--csv_magnitude', type=float, default=10., required=False,
-                           help='If stellar target, the magnitude value i considered as V magnitude of the object and '
-                                'the flux is scaled accordingly. Ignored if --flux_in_photons is true.')
-    csv_group.add_argument('--csv_delimiter', type=str, required=False, default=',', help='Delimiter of the CSV file')
-
-    csv_eff_group = parser.add_argument_group('CSVEfficiency')
-    csv_eff_group.add_argument('--eff_csv_filepath', type=argparse.FileType('r'), required=False,
-                               help="Path to .csv file that contains two columns: wavelength and efficiency."
-                                    "The wavelength is expected to be in microns, "
-                                    "the efficiency is a real number in [0,1]."
-                                    "PyEchelle will interpolate the given values "
-                                    "for intermediate wavelength positions.")
-    csv_eff_group.add_argument('--eff_csv_delimiter', type=str, required=False, default=',',
-                               help='Delimiter of the CSV file')
-
-    phoenix_group = parser.add_argument_group('Phoenix')
-    phoenix_group.add_argument('--phoenix_t_eff', default=3600,
-                               choices=Phoenix.valid_t,
-                               type=int, required=False,
-                               help="Effective temperature in Kelvins [K].")
-    phoenix_group.add_argument('--phoenix_log_g', default=5.,
-                               choices=Phoenix.valid_g,
-                               type=float, required=False,
-                               help="Surface gravity log g.")
-    phoenix_group.add_argument('--phoenix_z',
-                               choices=Phoenix.valid_z,
-                               type=float, required=False, default=0.,
-                               help="Overall metallicity.")
-    phoenix_group.add_argument('--phoenix_alpha',
-                               choices=Phoenix.valid_a,
-                               type=float, required=False, default=0.,
-                               help="Alpha element abundance.")
-    phoenix_group.add_argument('--phoenix_magnitude', default=10., required=False, type=float,
-                               help='V Magnitude of stellar object.')
-
-    etalon_group = parser.add_argument_group('Etalon')
-    etalon_group.add_argument('--etalon_d', type=float, default=5., required=False,
-                              help='Mirror distance of Fabry Perot etalon in [mm].')
-    etalon_group.add_argument('--etalon_n', type=float, default=1.0, required=False,
-                              help='Refractive index of medium between etalon mirrors.')
-    etalon_group.add_argument('--etalon_theta', type=float, default=0., required=False,
-                              help='angle of incidence of light in radians.')
-    etalon_group.add_argument('--etalon_n_photons', default=1000, required=False,
-                              help='Number of photons per seconds per peak of the etalon spectrum.')
-
-    ccd_group = parser.add_argument_group('CCD')
-    ccd_group.add_argument('--bias', type=int, required=False, default=0)
-    ccd_group.add_argument('--read_noise', type=float, required=False, default=0.)
-
-    parser.add_argument('--show', default=False, action='store_true',
-                        help='If set, the simulated frame will be shown in a matplotlib imshow frame at the end.')
-    parser.add_argument('-o', '--output', type=lambda p: Path(p).absolute(), required=False,
-                        default=Path(__file__).absolute().parent / "test.fits",
-                        help='A .fits file where the simulation is saved.')
-    parser.add_argument('--overwrite', default=False, action='store_true',
-                        help='If set, the output file will be overwritten if it exists already.')
-    parser.add_argument('--append', default=False, action='store_true',
-                        help='If set, the simulated photons will be added to the output file rather than overwriting '
-                             'the content of the output file. If the output file does not exist yet, '
-                             'it will be created.This flag can be used to do more complex multi-fiber simulations as a'
-                             ' sequential manner of simpler simulations.')
-
-    parser.add_argument('--html_export', type=str, default='',
-                        help="If given, the spectrum will be exported to an interactive image using plotly. It's not a"
-                             "standalone html file, but requires plotly.js to be loaded.")
-    return parser
-
-
-def main(args=None):
-    if not args:
-        args = sys.argv[1:]
-    parser = generate_parser()
-    args = parser.parse_args(args)
-    t1 = time.time()
-    sim = Simulator(ZEMAX(args.spectrograph))
-    sim.set_ccd(args.ccd)
-
-    # generate flat list for all fields to simulate
-    if args.fiber is not None:
-        if any(isinstance(el, list) for el in args.fiber):
-            fibers = [item for sublist in args.fiber for item in sublist]
-        else:
-            fibers = args.fiber
-    else:
-        fibers = sim.spectrograph.get_fibers(args.ccd)
-    sim.set_fibers(fibers)
-
-    if args.orders is not None:
-        if any(isinstance(el, list) for el in args.orders):
-            requested_orders = [item for sublist in args.orders for item in sublist]
-        else:
-            requested_orders = args.orders
-        sim.set_orders(requested_orders)
-    # generate flat list of all sources to simulate
-    source_names = args.sources
-    if len(source_names) == 1:
-        source_names = [source_names[0]] * len(
-            fibers)  # generate list of same length as 'fields' if only one source given
-
-    source_kwargs = []
-    # extract kwords specific to selected source
-    for s in source_names:
-        source_args = [ss for ss in vars(args) if ss.startswith(s.lower())]
-        # create dict consisting of kword arguments and values specific to selected source
-        source_kwargs.append(dict(zip([ss.replace(f"{s.lower()}_", "") for ss in source_args],
-                                      [getattr(args, ss) for ss in source_args])))
-
-    sim.set_sources([getattr(sources, source)(**s_args) for source, s_args in zip(source_names, source_kwargs)])
-
-    if args.eff_csv_filepath:
-        sim.set_efficiency(CSVEfficiency('global', args.eff_csv_filepath, args.eff_csv_delimiter))
-    # generate flat list of whether atmosphere is added
-    sim.set_atmospheres(args.atmosphere[0] if len(args.atmosphere) == 1 else args.atmosphere)
-    sim.set_radial_velocities(args.rv[0] if len(args.rv) == 1 else args.rv)
-    sim.set_cuda(args.cuda, args.cuda_seed)
-    sim.set_exposure_time(args.integration_time)
-    sim.set_telescope(Telescope(args.d_primary, args.d_secondary))
-    sim.set_output(args.output, args.append, args.overwrite)
-    sim.set_bias(args.bias)
-    sim.set_read_noise(args.read_noise)
-    sim.run()
-    t2 = time.time()
-    print(f"Simulation took {t2 - t1:.3f} s")
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+from __future__ import annotations
+
+import argparse
+import distutils.util
+import inspect
+import logging
+import pathlib
+import re
+import sys
+import time
+from dataclasses import field, dataclass
+from pathlib import Path
+
+import numpy as np
+from astropy.io import fits
+from joblib import Parallel, delayed
+from numba import cuda
+
+import pyechelle
+import pyechelle.slit
+from pyechelle import sources
+from pyechelle.CCD import CCD
+from pyechelle.efficiency import Efficiency, CSVEfficiency, SystemEfficiency, Atmosphere
+from pyechelle.raytrace_cuda import make_cuda_kernel, raytrace_order_cuda, make_cuda_kernel_singlemode
+from pyechelle.raytracing import raytrace_order_cpu
+from pyechelle.sources import CSV
+from pyechelle.sources import Phoenix, Source
+from pyechelle.spectrograph import Spectrograph, ZEMAX
+from pyechelle.telescope import Telescope
+
+logger = logging.getLogger('Simulator')
+logger.setLevel(level=logging.INFO)
+
+# get list of available spectrograph models
+dir_path = Path(__file__).resolve().parent.joinpath("models").joinpath("available_models.txt")
+with open(dir_path, 'r') as am:
+    available_models = [line.strip() for line in am.readlines() if line.strip() != '']
+
+# get list of available sources
+available_sources = [m[0] for m in inspect.getmembers(pyechelle.sources, inspect.isclass) if
+                     issubclass(m[1], pyechelle.sources.Source) and m[0] != "Source"]
+
+
+def parse_num_list(string_list: str) -> list:
+    """
+    Converts a string specifying a range of numbers (e.g. '1-3') into a list of these numbers ([1,2,3])
+    Args:
+        string_list: string like "[start value]-[end value]"
+
+    Returns:
+        List of integers
+    """
+
+    m = re.match(r'(\d+)(?:-(\d+))?$', string_list)
+    if not m:
+        raise argparse.ArgumentTypeError(
+            "'" + string_list + "' is not a range of number. Expected forms like '0-5' or '2'.")
+    start = m.group(1)
+    end = m.group(2) or start
+    return list(range(int(start, 10), int(end, 10) + 1))
+
+
+def export_to_html(data, filename, include_plotlyjs=False, width=1000, height=300, y_range_min=2000, y_range_max=3000):
+    """
+    Exports a 2D image into a 'standalone' HTML file. This is used e.g. for some examples in the documentation.
+    Args:
+        data: 2d numpy array
+        filename: output filename
+        include_plotlyjs: whether plotlyjs is included in html file or not
+        width: width of the plot in pixel
+        height: height of the plot in pixel
+        y_range_min: minimum y coordinate shown in image
+        y_range_max: maximum y coordinate shown in image
+
+    Returns:
+        None
+    """
+    import plotly.express as px
+    fig = px.imshow(data, binary_string=True, aspect='equal')
+
+    fig.update_traces(
+        hovertemplate=None,
+        hoverinfo='skip'
+    )
+    fig.update_layout(autosize=True, width=width, height=height, margin=dict(l=0, r=0, b=0, t=0))
+    fig.update_yaxes(range=[y_range_min, y_range_max])
+    fig.write_html(filename, include_plotlyjs=include_plotlyjs)
+
+
+def log_elapsed_time(msg: str, t0: float) -> float:
+    t1 = time.time()
+    logger.info(msg + f' (took {t1 - t0:2f} s )')
+    return t1
+
+
+def write_to_fits(c: CCD, filename: str | Path, overwrite: bool = True, append: bool = False, dtype: np.dtype = np.uint16):
+    """ Saves CCD image to disk
+
+    Args:
+        c: CCD object
+        filename: filepath
+        overwrite: if True, file will be overwritten if existing
+        append: if True, CCD data will be added to data in fits file
+        dtype: numpy.dtype object defining the data type of the saved FITS file, defaulting to unsigned 16-bit integers
+
+    Returns:
+        None
+    """
+    old_file_data = np.zeros_like(c.data)
+    if append:
+        if pathlib.Path(filename).is_file():
+            old_file_data = fits.getdata(filename)
+            assert old_file_data.shape == c.data.shape, f"You tried to append data to {filename}, " \
+                                                        f"but the fits file contains" \
+                                                        f"data with a different shape ({old_file_data.shape})."
+    hdu = fits.PrimaryHDU(data=np.array(c.data + old_file_data, dtype=dtype))
+    hdu_list = fits.HDUList([hdu])
+    hdu_list.writeto(filename, overwrite=overwrite or append)
+
+
+@dataclass
+class Simulator:
+    """ PyEchelle simulator
+
+    Simulator class that contains everything needed to generate spectra.
+
+    Attributes:
+        spectrograph (Spectrograph): spectrograph used for simulations
+        fibers (list[int]): fiber / list of fibers to be simulated
+        orders (list[int]): order / list of diffraction orders to be simulated
+        sources (list[Source]): spectral source / list of spectral sources per fiber (same length as fibers)
+        atmosphere (list[bool]): whether to include atmospheric transmission per fiber (same length as fibers)
+        atmosphere_conditions (list[dict | None]): skycalc arguments for atmospheric conditions (same length as sources)
+        rvs (list[float]): radial velocity shifts in [m/s] for sources (same length as fibers)
+        telescope (Telescope): Telescope used for simulations (relevant for 'on-sky' sources)
+        random_seed (int): random seed for the number generator
+        cuda (bool): flat if CUDA is to be used
+        max_cpu (int): number of CPUs used for simulation (if -1, max_cpu is number of available cores)
+        exp_time (float): exposure time to be simulated
+        output (Path): path to output fits file
+        append (bool): flag if simulated counts should be appended to existing image
+        overwrite (bool): flat if output file should be overwritten if existing
+        global_efficiency (Efficiency): overall efficiency curve to be considered
+         (on top of spectrograph efficiency curve and potentially atmosphere)
+
+    """
+    spectrograph: Spectrograph
+    fibers: list[int] = field(init=False, default=None)
+    orders: list[int] = field(init=False, default=None)
+    ccd: int = field(init=False, default=None)
+    sources: list[Source] = field(init=False, default=None)
+    atmosphere: list[bool] = field(init=False, default=None)
+    atmosphere_conditions: list[dict | None] = field(init=False, default=None)
+    rvs: list[float] = field(init=False, default=None)
+    telescope: Telescope = field(init=False, default=None)
+    random_seed: int = field(init=False, default=-1)
+    cuda: bool = field(init=False, default=False)
+    max_cpu: int = field(init=False, default=1)
+    exp_time: float = field(init=False, default=1.)
+    output: Path = field(init=False, default=None)
+    append: bool = field(init=False, default=False)
+    overwrite: bool = field(init=False, default=False)
+    bias: int = field(init=False, default=0)
+    read_noise: float = field(init=False, default=0.)
+    global_efficiency: Efficiency = field(init=False, default=None)
+
+    def set_sources(self, source: Source | list[Source]):
+        assert self.fibers is not None, 'Please set first the fields that you want to simulate.'
+        self.sources = source if isinstance(source, list) else [source] * len(self.fibers)
+        assert len(self.fibers) == len(self.sources), \
+            'Number of sources needs to match the number of fields/fibers (or be 1)'
+
+    def set_atmospheres(self, atmosphere: bool | list[bool], sky_calc_kwargs: dict | list[dict] = None):
+        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
+        self.atmosphere = [atmosphere] * len(self.sources) if isinstance(atmosphere, bool) else atmosphere
+        self.atmosphere_conditions = [sky_calc_kwargs] * len(self.sources) if (
+                isinstance(sky_calc_kwargs, dict) or sky_calc_kwargs is None) else sky_calc_kwargs
+        assert len(self.atmosphere) == len(self.sources), \
+            'Number of atmosphere flags needs to match the number of sources (or be 1)'
+        assert len(self.atmosphere_conditions) == len(self.sources), \
+            'Number of atmosphere condition arguments needs to match the number of sources (or be 1)'
+
+    def set_radial_velocities(self, rvs: float | list[float]):
+        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
+        self.rvs = [rvs] * len(self.sources) if isinstance(rvs, float) else rvs
+        assert len(self.rvs) == len(self.sources), \
+            'Number of radial velocity values needs to match the number of sources (or be 1)'
+
+    def set_telescope(self, telescope: Telescope):
+        self.telescope = telescope
+
+    def set_ccd(self, ccd: int):
+        self.ccd = ccd
+        assert self.ccd in self.spectrograph.get_ccd().keys(), f'You requested simulation of CCD {ccd}, ' \
+                                                               f'which is not available.'
+
+    def set_efficiency(self, eff: Efficiency):
+        assert isinstance(eff, Efficiency)
+        self.global_efficiency = eff
+
+    def set_bias(self, bias_value: int = 0):
+        self.bias = bias_value
+
+    def set_read_noise(self, read_noise: float = 0.):
+        if read_noise > 0.0:
+            assert self.bias > 0, "read noise was specified, but no bias value is set, yet. " \
+                                  "Do so before setting the read noise."
+        self.read_noise = read_noise
+
+    def set_fibers(self, fiber: int | list[int]):
+        assert self.ccd is not None, 'Please set CCD index first.'
+        self.fibers = [fiber] if isinstance(fiber, int) else fiber
+        for f in self.fibers:
+            assert f in self.spectrograph.get_fibers(self.ccd), f'You requested simulation of fiber {f}, which is ' \
+                                                                f'not available for ccd with index {self.ccd}'
+
+    def set_cuda(self, activate: bool = True, seed: int = -1):
+        self.cuda = activate
+        self.random_seed = seed
+
+    def _get_valid_orders(self, fiber: int):
+        valid_orders = []
+
+        requested_orders = self.spectrograph.get_orders(fiber, self.ccd) if self.orders is None else self.orders
+        for o in requested_orders:
+            if o in self.spectrograph.get_orders(fiber, self.ccd):
+                valid_orders.append(o)
+            else:
+                logger.warning(f'Order {o} is requested, but it is not in the Spectrograph model.')
+        return valid_orders
+
+    def _get_slit_function(self, fiber: int):
+        try:
+            if self.cuda:
+                slit_fun = getattr(pyechelle.slit, f"cuda_{self.spectrograph.get_field_shape(fiber, self.ccd)}")
+            else:
+                slit_fun = getattr(pyechelle.slit, self.spectrograph.get_field_shape(fiber, self.ccd))
+        except AttributeError:
+            raise NotImplementedError(
+                f"Field shape {self.spectrograph.get_field_shape(fiber, self.ccd)} is not implemented.")
+        return slit_fun
+
+    def _simulate_multi_cpu(self, orders, fiber, ccd_index, slit_fun, s, rv, integration_time, c, efficiency):
+        simulated_photons = []
+        t0 = time.time()
+        results = Parallel(n_jobs=min(self.max_cpu, len(orders)), backend="threading")(
+            delayed(raytrace_order_cpu)(o, self.spectrograph, s, slit_fun, self.telescope, rv,
+                                        integration_time,
+                                        c, fiber, ccd_index,
+                                        efficiency, self.max_cpu) for o in np.sort(orders))
+        logger.info('Add up orders...')
+        ccd_results = [r[0] for r in results]
+        simulated_photons.extend([r[1] for r in results])
+        c.data = np.sum(ccd_results, axis=0)
+        log_elapsed_time('done.', t0)
+        return simulated_photons
+
+    def _simulate_single_cpu(self, orders, fiber, ccd_index, s, slit_fun, rv, integration_time, c, efficiency):
+        simulated_photons = []
+        for o in np.sort(orders):
+            nphot = raytrace_order_cpu(o, self.spectrograph, s, slit_fun, self.telescope, rv,
+                                       integration_time,
+                                       c, fiber, ccd_index,
+                                       efficiency,
+                                       1)
+            simulated_photons.append(nphot)
+        return simulated_photons
+
+    def _simulate_cuda(self, orders, slit_fun, rv, integration_time, dccd, efficiency, s, c, fiber, ccd_index):
+        if slit_fun is not None:  # multimode
+            cuda_kernel = make_cuda_kernel(slit_fun)
+        else:  # singlemode
+            cuda_kernel = make_cuda_kernel_singlemode()
+        simulated_photons = []
+        for o in np.sort(orders):
+            nphot = raytrace_order_cuda(o, self.spectrograph, s, self.telescope, rv, integration_time, dccd,
+                                        float(c.pixelsize), fiber, ccd_index, efficiency, seed=self.random_seed,
+                                        cuda_kernel=cuda_kernel)
+            simulated_photons.append(nphot)
+        return simulated_photons
+
+    def validate(self):
+        assert self.fibers is not None, 'Please set fibers for simulation'
+        assert self.ccd is not None, 'Please set ccd index/indices for simulation'
+        assert self.output is not None, 'Please set output path for simulation'
+        if self.atmosphere is None:
+            logger.info('It was not explicitly specified whether to consider atmospheric transmission. '
+                        'It is set to False')
+            self.atmosphere = [False] * len(self.sources)
+
+        if self.atmosphere_conditions is None:
+            if self.atmosphere:
+                logger.info('Atmospheric conditions were not specified. The default atmospheric conditions apply. '
+                            '(e.g. airmass 1)')
+            self.atmosphere_conditions = [None] * len(self.sources)
+
+        if self.rvs is None:
+            logger.info('Radial velocities are not specified explicitly. They are therefore set to 0.0')
+            self.rvs = [0.0] * len(self.sources)
+        if self.output.is_file():
+            assert self.overwrite or self.append, f'You specified to save the simulation at {self.output}, ' \
+                                                  f'but this file exists. If you want to overwrite, ' \
+                                                  f'please set the overwrite flag. Or in case you want to append to ' \
+                                                  f'the file: please set the append flag'
+        return True
+
+    def run(self):
+        self.validate()
+        c = self.spectrograph.get_ccd(self.ccd)
+        total_simulated_photons = []
+        t1 = time.time()
+        # copy empty array to CUDA device
+        if self.cuda:
+            dccd = cuda.to_device(np.zeros_like(c.data, dtype=np.uint32))
+
+        for f, s, atm, atm_cond, rv in zip(self.fibers, self.sources, self.atmosphere, self.atmosphere_conditions,
+                                           self.rvs):
+            orders = self.orders if self.orders is not None else self._get_valid_orders(f)
+            slit_fun = self._get_slit_function(f)
+            if self.global_efficiency is None:
+                if atm:
+                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd),
+                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
+                                         'Combined Efficiency')
+                else:
+                    e = self.spectrograph.get_efficiency(f, self.ccd)
+            else:
+                if atm:
+                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency,
+                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
+                                         'Combined Efficiency')
+                else:
+                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency],
+                                         'Combined Efficiency')
+
+            if not self.cuda:
+                if self.max_cpu > 1:
+                    total_simulated_photons.extend(
+                        self._simulate_multi_cpu(orders, f, self.ccd, slit_fun, s, rv, self.exp_time, c, e))
+                else:
+                    total_simulated_photons.extend(
+                        self._simulate_single_cpu(orders, f, self.ccd, s, slit_fun, rv, self.exp_time, c, e))
+            else:
+                total_simulated_photons.extend(
+                    self._simulate_cuda(orders, slit_fun, rv, self.exp_time, dccd, e, s, c, f, self.ccd))
+
+        if self.cuda:
+            dccd.copy_to_host(c.data)
+        logger.info('Finish up simulation and save...')
+        c.clip()
+
+        # add bias / global ccd effects
+        if self.bias > 0:
+            c.add_bias(self.bias)
+        if self.read_noise > 0.:
+            c.add_readnoise(self.read_noise)
+        t2 = time.time()
+
+        write_to_fits(c, self.output, self.overwrite, self.append)
+        logger.info(f"Total time for simulation: {t2 - t1:.3f}s.")
+        logger.info(f"Total simulated photons: {sum(total_simulated_photons)}")
+        return sum(total_simulated_photons)
+
+    def set_exposure_time(self, exp_time: float = 1):
+        self.exp_time = exp_time
+
+    def set_output(self, path: str | Path = Path().cwd().joinpath('test.fits'),
+                   append: bool = False, overwrite: bool = False):
+
+        self.output = path if isinstance(path, Path) else Path(path)
+        self.append = append
+        self.overwrite = overwrite
+        if append and not self.output.is_file():
+            logger.warning(f'You specified that the simulation should be appended to {self.output}, but there is no '
+                           f'such file. It will be created.')
+
+    def set_orders(self, orders: int | list[int] | None):
+        if isinstance(orders, int):
+            self.orders = [orders]
+        self.orders = orders
+        if self.orders is not None:
+            for f in self.fibers:
+                valid_orders = self._get_valid_orders(f)
+                for o in self.orders:
+                    assert o in valid_orders, f'You requested to simulate order {o}, but this order is not available' \
+                                              f'on CCD {self.ccd} and fiber/field {f}'
+
+
+def generate_parser():
+    parser = argparse.ArgumentParser(description='PyEchelle Simulator',
+                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
+                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
+    parser.add_argument('--ccd', type=int, default=1, required=False, help='Sets CCD index to be simulated.')
+    parser.add_argument('-t', '--integration_time', type=float, default=1.0, required=False,
+                        help=f"Integration time for the simulation in seconds [s].")
+    parser.add_argument('--fiber', type=parse_num_list, required=False,
+                        help='Fiber/Field number(s) to be simulated. Can either be a single integer, or an integer'
+                             'range (e.g. 1-3) ')
+    parser.add_argument('--no_blaze', action='store_true',
+                        help='If set, the blaze efficiency per order will be ignored.')
+    parser.add_argument('--no_efficiency', action='store_true',
+                        help='If set, all instrument/atmosphere efficiencies will be ignored.')
+
+    parser.add_argument('--cuda', action='store_true',
+                        help='If set, CUDA will be used for raytracing. Note: the max_cpu flag is then obsolete.')
+
+    parser.add_argument('--cuda_seed', type=int, default=-1,
+                        help='Random seed for generating CUDA RNG states. If <0, then the seed is choosen randomly.')
+
+    parser.add_argument('--max_cpu', type=int, default=1,
+                        help="Maximum number of CPU cores used. Note: The parallelization happens 'per order'."
+                             " Order-wise images are added up. This requires a large amount of memory at the moment."
+                             "If planning on simulating multiple images, consider using only 1 CPU per simulation "
+                             "and starting multiple simulations instead.")
+
+    atmosphere_group = parser.add_argument_group('Atmosphere')
+    atmosphere_group.add_argument('--atmosphere', nargs='+', required=False,
+                                  help='Add telluric lines to spectrum. For adding tellurics to all spectra just use'
+                                       '--atmosphere Y, for specifying per fiber user e.g. --atmosphere Y N Y',
+                                  type=lambda x: bool(distutils.util.strtobool(x)), default=[False])
+
+    atmosphere_group.add_argument('--airmass', default=1.0, type=float, required=False,
+                                  help='airmass for atmospheric model')
+
+    telescope_group = parser.add_argument_group('Telescope settings')
+    telescope_group.add_argument('--d_primary', type=float, required=False, default=1.0,
+                                 help='Diameter of the primary telescope mirror.')
+    telescope_group.add_argument('--d_secondary', type=float, required=False, default=0,
+                                 help='Diameter of the secondary telescope mirror.')
+
+    parser.add_argument('--orders', type=parse_num_list, nargs='+', required=False,
+                        help='Echelle/Grating order numbers to simulate... '
+                             'if not specified, all orders of the spectrograph are simulated.'
+                             'Can either be a single integer, or a range (e.g. 80-90)')
+
+    parser.add_argument('--sources', nargs='+', choices=available_sources, required=True,
+                        help='Spectral source for the simulation. Can either be a single string, e.g. "Etalon",'
+                             ' or a comma separated list of sources (e.g. "Etalon, Constant, Etalon") which length must'
+                             'match the number of fields/fibers.')
+    parser.add_argument('--rv', nargs='+', type=float, required=False, default=[0.],
+                        help="radial velocity shift of source")
+    const_source_group = parser.add_argument_group('Constant source')
+    const_source_group.add_argument('--constant_intensity', type=float, default=0.0001, required=False,
+                                    help="Flux in microWatts / nanometer for constant flux spectral source")
+    arclamps_group = parser.add_argument_group('Arc Lamps')
+    arclamps_group.add_argument('--scale', default=10.0, required=False,
+                                help='Intensity scale of gas lines (e.g. Ag or Ne) vs metal (Th)')
+
+    csv_group = parser.add_argument_group('CSV')
+    csv_group.add_argument('--csv_filepath', type=argparse.FileType('r'), required=False,
+                           help="Path to .csv file that contains two columns: wavelength and flux. The flux is expected"
+                                "to be in ergs/s/cm^2/cm (like Phoenix spectra) or photons (then set it via "
+                                "--csv_flux_in_photons). The wavelength unit is expected to "
+                                "be angstroms, but it can be changed via --csv_wavelength_unit")
+    csv_group.add_argument('--csv_wavelength_unit', choices=list(CSV.wavelength_scaling.keys()), default='a', type=str,
+                           help=f"Unit of the wavelength column in the .csv file. Options are "
+                                f"{list(CSV.wavelength_scaling.keys())}")
+    csv_group.add_argument('--csv_list_like', type=bool, default=False, help='Set to True if spectrum is discrete.')
+    csv_group.add_argument('--csv_flux_in_photons', type=bool, default=False,
+                           help='Set to True if flux is given in Photons/s rather than ergs')
+    csv_group.add_argument('--csv_stellar_target', type=bool, default=True,
+                           help='Set to True if Source is a stellar target.')
+    csv_group.add_argument('--csv_magnitude', type=float, default=10., required=False,
+                           help='If stellar target, the magnitude value i considered as V magnitude of the object and '
+                                'the flux is scaled accordingly. Ignored if --flux_in_photons is true.')
+    csv_group.add_argument('--csv_delimiter', type=str, required=False, default=',', help='Delimiter of the CSV file')
+
+    csv_eff_group = parser.add_argument_group('CSVEfficiency')
+    csv_eff_group.add_argument('--eff_csv_filepath', type=argparse.FileType('r'), required=False,
+                               help="Path to .csv file that contains two columns: wavelength and efficiency."
+                                    "The wavelength is expected to be in microns, "
+                                    "the efficiency is a real number in [0,1]."
+                                    "PyEchelle will interpolate the given values "
+                                    "for intermediate wavelength positions.")
+    csv_eff_group.add_argument('--eff_csv_delimiter', type=str, required=False, default=',',
+                               help='Delimiter of the CSV file')
+
+    phoenix_group = parser.add_argument_group('Phoenix')
+    phoenix_group.add_argument('--phoenix_t_eff', default=3600,
+                               choices=Phoenix.valid_t,
+                               type=int, required=False,
+                               help="Effective temperature in Kelvins [K].")
+    phoenix_group.add_argument('--phoenix_log_g', default=5.,
+                               choices=Phoenix.valid_g,
+                               type=float, required=False,
+                               help="Surface gravity log g.")
+    phoenix_group.add_argument('--phoenix_z',
+                               choices=Phoenix.valid_z,
+                               type=float, required=False, default=0.,
+                               help="Overall metallicity.")
+    phoenix_group.add_argument('--phoenix_alpha',
+                               choices=Phoenix.valid_a,
+                               type=float, required=False, default=0.,
+                               help="Alpha element abundance.")
+    phoenix_group.add_argument('--phoenix_magnitude', default=10., required=False, type=float,
+                               help='V Magnitude of stellar object.')
+
+    etalon_group = parser.add_argument_group('Etalon')
+    etalon_group.add_argument('--etalon_d', type=float, default=5., required=False,
+                              help='Mirror distance of Fabry Perot etalon in [mm].')
+    etalon_group.add_argument('--etalon_n', type=float, default=1.0, required=False,
+                              help='Refractive index of medium between etalon mirrors.')
+    etalon_group.add_argument('--etalon_theta', type=float, default=0., required=False,
+                              help='angle of incidence of light in radians.')
+    etalon_group.add_argument('--etalon_n_photons', default=1000, required=False,
+                              help='Number of photons per seconds per peak of the etalon spectrum.')
+
+    ccd_group = parser.add_argument_group('CCD')
+    ccd_group.add_argument('--bias', type=int, required=False, default=0)
+    ccd_group.add_argument('--read_noise', type=float, required=False, default=0.)
+
+    parser.add_argument('--show', default=False, action='store_true',
+                        help='If set, the simulated frame will be shown in a matplotlib imshow frame at the end.')
+    parser.add_argument('-o', '--output', type=lambda p: Path(p).absolute(), required=False,
+                        default=Path(__file__).absolute().parent / "test.fits",
+                        help='A .fits file where the simulation is saved.')
+    parser.add_argument('--overwrite', default=False, action='store_true',
+                        help='If set, the output file will be overwritten if it exists already.')
+    parser.add_argument('--append', default=False, action='store_true',
+                        help='If set, the simulated photons will be added to the output file rather than overwriting '
+                             'the content of the output file. If the output file does not exist yet, '
+                             'it will be created.This flag can be used to do more complex multi-fiber simulations as a'
+                             ' sequential manner of simpler simulations.')
+
+    parser.add_argument('--html_export', type=str, default='',
+                        help="If given, the spectrum will be exported to an interactive image using plotly. It's not a"
+                             "standalone html file, but requires plotly.js to be loaded.")
+    return parser
+
+
+def main(args=None):
+    if not args:
+        args = sys.argv[1:]
+    parser = generate_parser()
+    args = parser.parse_args(args)
+    t1 = time.time()
+    sim = Simulator(ZEMAX(args.spectrograph))
+    sim.set_ccd(args.ccd)
+
+    # generate flat list for all fields to simulate
+    if args.fiber is not None:
+        if any(isinstance(el, list) for el in args.fiber):
+            fibers = [item for sublist in args.fiber for item in sublist]
+        else:
+            fibers = args.fiber
+    else:
+        fibers = sim.spectrograph.get_fibers(args.ccd)
+    sim.set_fibers(fibers)
+
+    if args.orders is not None:
+        if any(isinstance(el, list) for el in args.orders):
+            requested_orders = [item for sublist in args.orders for item in sublist]
+        else:
+            requested_orders = args.orders
+        sim.set_orders(requested_orders)
+    # generate flat list of all sources to simulate
+    source_names = args.sources
+    if len(source_names) == 1:
+        source_names = [source_names[0]] * len(
+            fibers)  # generate list of same length as 'fields' if only one source given
+
+    source_kwargs = []
+    # extract kwords specific to selected source
+    for s in source_names:
+        source_args = [ss for ss in vars(args) if ss.startswith(s.lower())]
+        # create dict consisting of kword arguments and values specific to selected source
+        source_kwargs.append(dict(zip([ss.replace(f"{s.lower()}_", "") for ss in source_args],
+                                      [getattr(args, ss) for ss in source_args])))
+
+    sim.set_sources([getattr(sources, source)(**s_args) for source, s_args in zip(source_names, source_kwargs)])
+
+    if args.eff_csv_filepath:
+        sim.set_efficiency(CSVEfficiency('global', args.eff_csv_filepath, args.eff_csv_delimiter))
+    # generate flat list of whether atmosphere is added
+    sim.set_atmospheres(args.atmosphere[0] if len(args.atmosphere) == 1 else args.atmosphere)
+    sim.set_radial_velocities(args.rv[0] if len(args.rv) == 1 else args.rv)
+    sim.set_cuda(args.cuda, args.cuda_seed)
+    sim.set_exposure_time(args.integration_time)
+    sim.set_telescope(Telescope(args.d_primary, args.d_secondary))
+    sim.set_output(args.output, args.append, args.overwrite)
+    sim.set_bias(args.bias)
+    sim.set_read_noise(args.read_noise)
+    sim.run()
+    t2 = time.time()
+    print(f"Simulation took {t2 - t1:.3f} s")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyechelle-0.3.5/pyechelle/slit.py` & `pyechelle-0.3.6/pyechelle/slit.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-""" Slit transformation functions
-
-This module implements various coordinate transformations for implementing different slit shapes such as circular,
-octagonal etc.
-Both, numba compiled functions and cuda device functions are implemented.
-
-In general, a slit function transforms a random coordinate x, y (both from the interval [0, 1]) to a random coordinate
-x', y'
-
-A special case is the 'singlemode' slit, since here, no transformation is required.
-
-
-.. plot::
-
-    import matplotlib.pyplot as plt
-    import random
-    import numpy
-    import pyechelle.slit
-    import inspect
-    from numba.core.registry import CPUDispatcher
-
-    available_slits = [m[0] for m in inspect.getmembers(pyechelle.slit) if isinstance(m[1], CPUDispatcher)]
-
-
-    fig, ax = plt.subplots(1, len(available_slits), sharey=True, sharex=True,figsize=(len(available_slits)*3, 3))
-    fig.suptitle('Supported slit functions')
-    for i, slit in enumerate(available_slits):
-        s = getattr(pyechelle.slit, slit)
-        xy = [s(random.random(), random.random()) for _ in range(2000)]
-        ax[i].scatter(*numpy.array(xy).T, s=1)
-        ax[i].set_aspect('equal', 'box')
-        ax[i].set_title(slit)
-    plt.tight_layout()
-    plt.show()
-
-"""
-import math
-import random
-
-import numba.cuda.random
-from numba import njit, float64, cuda
-from numba.types import UniTuple
-
-# single mode slit just return 'None'
-singlemode = None
-cuda_singlemode = None
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def rectangular(xx, yy):
-    """ Rectangular transformation
-    """
-    return xx, yy
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def circular(xx, yy):
-    """ Circular transformation
-    """
-    r = math.sqrt(xx) / 2.
-    phi = yy * math.pi * 2
-    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def octagonal(r1, r2):
-    """ Octagonal transformation
-    """
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 8
-
-    b = [1., 0.]
-    c = [math.cos(phi_segment), math.sin(phi_segment)]
-    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = random.randint(0, 7)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    x_new = x * cos_values - y * sin_values
-    y_new = x * sin_values + y * cos_values
-    return x_new / 2. + 0.5, y_new / 2. + 0.5
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def hexagonal(r1, r2):
-    """ Hexagonal transformation
-    """
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 6
-
-    b = [1., 0.]
-    c = [math.cos(phi_segment), math.sin(phi_segment)]
-    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = random.randint(0, 5)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    xnew = x * cos_values - y * sin_values
-    ynew = x * sin_values + y * cos_values
-    return xnew / 2. + 0.5, ynew / 2. + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_rectangular(x, y, rng_states, thread_id):
-    return x, y
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_circular(x, y, rng_states, thread_id):
-    r = math.sqrt(x) / 2.
-    phi = y * math.pi * 2
-    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_octagonal(r1, r2, rng_states, thread_id):
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 8.
-
-    b = (1., 0.)
-    c = (math.cos(phi_segment), math.sin(phi_segment))
-    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 8.)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_hexagonal(r1, r2, rng_states, thread_id):
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 6.
-
-    b = (1., 0.)
-    c = (math.cos(phi_segment), math.sin(phi_segment))
-    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 6.)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
+""" Slit transformation functions
+
+This module implements various coordinate transformations for implementing different slit shapes such as circular,
+octagonal etc.
+Both, numba compiled functions and cuda device functions are implemented.
+
+In general, a slit function transforms a random coordinate x, y (both from the interval [0, 1]) to a random coordinate
+x', y'
+
+A special case is the 'singlemode' slit, since here, no transformation is required.
+
+
+.. plot::
+
+    import matplotlib.pyplot as plt
+    import random
+    import numpy
+    import pyechelle.slit
+    import inspect
+    from numba.core.registry import CPUDispatcher
+
+    available_slits = [m[0] for m in inspect.getmembers(pyechelle.slit) if isinstance(m[1], CPUDispatcher)]
+
+
+    fig, ax = plt.subplots(1, len(available_slits), sharey=True, sharex=True,figsize=(len(available_slits)*3, 3))
+    fig.suptitle('Supported slit functions')
+    for i, slit in enumerate(available_slits):
+        s = getattr(pyechelle.slit, slit)
+        xy = [s(random.random(), random.random()) for _ in range(2000)]
+        ax[i].scatter(*numpy.array(xy).T, s=1)
+        ax[i].set_aspect('equal', 'box')
+        ax[i].set_title(slit)
+    plt.tight_layout()
+    plt.show()
+
+"""
+import math
+import random
+
+import numba.cuda.random
+from numba import njit, float64, cuda
+from numba.types import UniTuple
+
+# single mode slit just return 'None'
+singlemode = None
+cuda_singlemode = None
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def rectangular(xx, yy):
+    """ Rectangular transformation
+    """
+    return xx, yy
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def circular(xx, yy):
+    """ Circular transformation
+    """
+    r = math.sqrt(xx) / 2.
+    phi = yy * math.pi * 2
+    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def octagonal(r1, r2):
+    """ Octagonal transformation
+    """
+    phi = 0.
+    s1 = math.sqrt(r1)
+    phi_segment = 2. * math.pi / 8
+
+    b = [1., 0.]
+    c = [math.cos(phi_segment), math.sin(phi_segment)]
+    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = random.randint(0, 7)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    x_new = x * cos_values - y * sin_values
+    y_new = x * sin_values + y * cos_values
+    return x_new / 2. + 0.5, y_new / 2. + 0.5
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def hexagonal(r1, r2):
+    """ Hexagonal transformation
+    """
+    phi = 0.
+    s1 = math.sqrt(r1)
+    phi_segment = 2. * math.pi / 6
+
+    b = [1., 0.]
+    c = [math.cos(phi_segment), math.sin(phi_segment)]
+    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = random.randint(0, 5)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    xnew = x * cos_values - y * sin_values
+    ynew = x * sin_values + y * cos_values
+    return xnew / 2. + 0.5, ynew / 2. + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_rectangular(x, y, rng_states, thread_id):
+    return x, y
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_circular(x, y, rng_states, thread_id):
+    r = math.sqrt(x) / 2.
+    phi = y * math.pi * 2
+    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_octagonal(r1, r2, rng_states, thread_id):
+    phi = 0.
+    s1 = math.sqrt(r1)
+    phi_segment = 2. * math.pi / 8.
+
+    b = (1., 0.)
+    c = (math.cos(phi_segment), math.sin(phi_segment))
+    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 8.)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_hexagonal(r1, r2, rng_states, thread_id):
+    phi = 0.
+    s1 = math.sqrt(r1)
+    phi_segment = 2. * math.pi / 6.
+
+    b = (1., 0.)
+    c = (math.cos(phi_segment), math.sin(phi_segment))
+    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 6.)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
```

### Comparing `pyechelle-0.3.5/pyechelle/spectrograph.py` & `pyechelle-0.3.6/pyechelle/spectrograph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,564 +1,735 @@
-from __future__ import annotations
-
-import logging
-import urllib.request
-from dataclasses import dataclass
-from pathlib import Path
-from urllib.error import URLError
-
-import h5py
-import numpy as np
-
-from pyechelle.CCD import CCD
-from pyechelle.efficiency import SystemEfficiency, GratingEfficiency, TabulatedEfficiency, ConstantEfficiency
-from pyechelle.optics import AffineTransformation, PSF, TransformationSet, convert_matrix, apply_matrix
-
-
-def check_url_exists(url: str) -> bool:
-    """
-    Check if URL exists.
-    Args:
-        url: url to be tested
-
-    Returns:
-        if URL exists
-    """
-    try:
-        with urllib.request.urlopen(url) as response:
-            return float(response.headers['Content-length']) > 0
-    except URLError:
-        return False
-
-
-def check_for_spectrograph_model(model_name: str, download=True):
-    """
-    Check if spectrograph model exists locally. Otherwise: Download if download is true (default) or check if URL to
-    spectrograph model is valid (this is mainly for testing purpose).
-
-    Args:
-        model_name: name of spectrograph model. See models/available_models.txt for valid names
-        download: download flag
-
-    Returns:
-
-    """
-    file_path = Path(__file__).resolve().parent.joinpath("models").joinpath(f"{model_name}.hdf")
-    if not file_path.is_file():
-        url = f"https://stuermer.science/nextcloud/index.php/s/ps5Pk379LgcpLwN/download?path=/&files={model_name}.hdf"
-        if download:
-            print(f"Spectrograph model {model_name} not found locally. Trying to download from {url}...")
-            Path(Path(__file__).resolve().parent.joinpath("models")).mkdir(parents=False, exist_ok=True)
-            with urllib.request.urlopen(url) as response, open(file_path, "wb") as out_file:
-                data = response.read()
-                out_file.write(data)
-        else:
-            check_url_exists(url)
-    return file_path
-
-
-@dataclass
-class Spectrograph:
-    """ Abstract spectrograph model
-
-    Describes all methods that a spectrograph model must have to be used in a simulation. \n
-    When subclassing, all methods need to be implemented in the subclass.
-
-    A spectrograph model as at least one CCD (with CCD_index 1), at least one field/fiber (with fiber index 1),
-    and at least one diffraction order.
-    """
-    name: str = 'Spectrograph'
-
-    def get_fibers(self, ccd_index: int = 1) -> list[int]:
-        """ Fields/fiber indices
-
-        Args:
-            ccd_index: CCD index
-
-        Returns:
-            available fields/fiber indices
-        """
-        raise NotImplementedError
-
-    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
-        """ Diffraction orders
-
-        Args:
-            fiber: fiber/field index
-            ccd_index: CCD index
-
-        Returns:
-            available diffraction order(s) for given indices
-        """
-        raise NotImplementedError
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
-        """ Transformation matrix/matrices
-
-        Args:
-            wavelength: wavelength(s) [micron]
-            order: diffraction order
-            fiber: fiber index
-            ccd_index: CCD index
-
-        Returns:
-            transformation matrix/matrices
-        """
-        raise NotImplementedError
-
-    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
-        """ PSF
-
-        PSFs are tabulated. When wavelength is provided, the closest available PSF of the model is returned.
-
-        When wavelength is None, all PSFs for that particular order (and fiber and CCD index) are returned.
-
-        Args:
-            wavelength: wavelength [micron] or None
-            order: diffraction order
-            fiber: fiber index
-            ccd_index: ccd index
-
-        Returns:
-            PSF(s)
-        """
-        raise NotImplementedError
-
-    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
-            -> tuple[float, float]:
-        """ Wavelength range
-
-        Returns minimum and maximum wavelength of the entire spectrograph unit or an individual order if specified.
-
-        Args:
-            ccd_index: CCD index
-            fiber: fiber index
-            order: diffraction order
-
-        Returns:
-            minimum and maximum wavelength [microns]
-        """
-        raise NotImplementedError
-
-    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
-        """ Get CCD object(s)
-
-        When index is provided the corresponding CCD object is returned.\n
-        If no index is provided, all available CCDs are return as a dict with the index as key.
-
-        Args:
-            ccd_index: CCD index
-
-        Returns:
-            CCD object(s)
-        """
-        raise NotImplementedError
-
-    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
-        """ Shape of field/fiber
-
-        Returning the field/fiber shape for the given indices as a string.
-        See slit.py for currently implemented shapes.
-
-        Args:
-            fiber: fiber index
-            ccd_index: ccd index
-
-        Returns:
-            field/fiber shape as string (e.g. rectangular, octagonal)
-        """
-        raise NotImplementedError
-
-    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
-        """ Spectrograph efficiency
-
-        Args:
-            fiber: fiber/field index
-            ccd_index: CCD index
-
-        Returns:
-            System efficiency for given indices
-        """
-        raise NotImplementedError
-
-
-class SimpleSpectrograph(Spectrograph):
-    def __init__(self):
-        self._ccd = {1: CCD()}
-        self._fibers = {}
-        self._orders = {}
-        self._transformations = {}
-        for c in self._ccd.keys():
-            self._fibers[c] = [1]
-            self._orders[c] = {}
-            for f in self._fibers.keys():
-                self._orders[c][f] = [1]
-
-    def get_fibers(self, ccd_index: int = 1) -> list[int]:
-        return self._fibers[ccd_index]
-
-    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
-        return self._orders[ccd_index][fiber]
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation]:
-        if isinstance(wavelength, float):
-            return AffineTransformation(0.0, 1.0, 10., 0., (wavelength - 0.5) * wavelength * 100000. + 2000.,
-                                        fiber * 10. + 2000., wavelength)
-        else:
-            ts = TransformationSet([AffineTransformation(0.0, 1.0, 10., 0., (w - 0.5) * w * 100000. + 2000.,
-                                                         fiber * 10. + 2000., w) for w in wavelength])
-            return ts.get_affine_transformations(wavelength)
-
-    @staticmethod
-    def gauss_map(size_x, size_y=None, sigma_x=5., sigma_y=None):
-        if size_y is None:
-            size_y = size_x
-        if sigma_y is None:
-            sigma_y = sigma_x
-
-        assert isinstance(size_x, int)
-        assert isinstance(size_y, int)
-
-        x0 = size_x // 2
-        y0 = size_y // 2
-
-        x = np.arange(0, size_x, dtype=float)
-        y = np.arange(0, size_y, dtype=float)[:, np.newaxis]
-
-        x -= x0
-        y -= y0
-
-        exp_part = x ** 2 / (2 * sigma_x ** 2) + y ** 2 / (2 * sigma_y ** 2)
-        return 1 / (2 * np.pi * sigma_x * sigma_y) * np.exp(-exp_part)
-
-    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
-        if wavelength is None:
-            wl = np.linspace(*self.get_wavelength_range(order, fiber, ccd_index), 20)
-            return [PSF(w, self.gauss_map(11, sigma_x=3., sigma_y=10.), 1.5) for w in wl]
-        else:
-            return PSF(wavelength, self.gauss_map(11, sigma_x=3., sigma_y=10.), 1.5)
-
-    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
-            -> tuple[float, float]:
-        return 0.4, 0.6
-
-    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
-        if ccd_index is None:
-            return self._ccd
-        else:
-            return self._ccd[ccd_index]
-
-    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
-        return 'rectangular'
-
-    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
-        return SystemEfficiency([ConstantEfficiency(1.0)], 'System')
-
-
-class ZEMAX(Spectrograph):
-    def __init__(self, path: str | Path):
-        self.path = check_for_spectrograph_model(path)
-        self._CCDs = {}
-        self._ccd_keys = []
-        self._h5f = None
-
-        self._transformations = {}
-        self._spline_transformations = {}
-        self._psfs = {}
-        self._efficiency = {}
-
-        # self.name = self.h5f[f"Spectrograph"].attrs['name']
-        self._field_shape = {}
-
-        self._orders = {}
-
-        self.CCD = [self._read_ccd_from_hdf]
-
-    @property
-    def h5f(self):
-        if self._h5f is None:
-            self._h5f = h5py.File(self.path, "r")
-        return self._h5f
-
-    def _read_ccd_from_hdf(self, k) -> CCD:
-        # read in CCD information
-        nx = self.h5f[f"CCD_{k}"].attrs['Nx']
-        ny = self.h5f[f"CCD_{k}"].attrs['Ny']
-        ps = self.h5f[f"CCD_{k}"].attrs['pixelsize']
-        return CCD(n_pix_x=nx, n_pix_y=ny, pixelsize=ps)
-
-    def get_fibers(self, ccd_index: int = 1) -> list[int]:
-        return [int(k[6:]) for k in self.h5f[f"CCD_{ccd_index}"].keys() if "fiber" in k]
-
-    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
-        if ccd_index not in self._field_shape.keys():
-            self._field_shape[ccd_index] = {}
-        if fiber not in self._field_shape[ccd_index].keys():
-            fs = self.h5f[f"CCD_{ccd_index}/fiber_{fiber}"].attrs["field_shape"]
-            self._field_shape[ccd_index][fiber] = fs.decode("utf-8") if isinstance(fs, bytes) else fs
-        return self._field_shape[ccd_index][fiber]
-
-    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
-        if ccd_index not in self._orders.keys():
-            self._orders[ccd_index] = {}
-        if fiber not in self._orders[ccd_index].keys():
-            self._orders[ccd_index][fiber] = [int(k[5:]) for k
-                                              in self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/"].keys() if "psf" not in k]
-            self._orders[ccd_index][fiber].sort()
-        return self._orders[ccd_index][fiber]
-
-    def transformations(self, order: int, fiber: int = 1, ccd_index: int = 1) -> list[AffineTransformation]:
-        if ccd_index not in self._transformations.keys():
-            self._transformations[ccd_index] = {}
-        if fiber not in self._transformations[ccd_index].keys():
-            self._transformations[ccd_index][fiber] = {}
-        if order not in self._transformations[ccd_index][fiber].keys():
-            try:
-                self._transformations[ccd_index][fiber][order] = [AffineTransformation(*af)
-                                                                  for af in
-                                                                  self.h5f[
-                                                                      f"CCD_{ccd_index}/fiber_{fiber}/order{order}"][
-                                                                      ()]]
-                self._transformations[ccd_index][fiber][order].sort()
-
-            except KeyError:
-                raise KeyError(
-                    f"You asked for the affine transformation matrices in diffraction order {order}. "
-                    f"But this data is not available")
-
-        return self._transformations[ccd_index][fiber][order]
-
-    def spline_transformations(self, order: int, fiber: int = 1, ccd_index: int = 1) -> TransformationSet:
-        if ccd_index not in self._spline_transformations.keys():
-            self._spline_transformations[ccd_index] = {}
-        if fiber not in self._spline_transformations[ccd_index].keys():
-            self._spline_transformations[ccd_index][fiber] = {}
-        if order not in self._spline_transformations[ccd_index][fiber].keys():
-            tfs = self.transformations(order, fiber, ccd_index)
-            self._spline_transformations[ccd_index][fiber][order] = TransformationSet(tfs)
-        return self._spline_transformations[ccd_index][fiber][order]
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation] | np.ndarray:
-        return self.spline_transformations(order, fiber, ccd_index).get_affine_transformations(wavelength)
-
-    def psfs(self, order: int, fiber: int = 1, ccd_index: int = 1) -> list[PSF]:
-        if ccd_index not in self._psfs.keys():
-            self._psfs[ccd_index] = {}
-        if order not in self._psfs[ccd_index].keys():
-            try:
-                self._psfs[ccd_index][order] = \
-                    [PSF(self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"].attrs['wavelength'],
-                         self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"][()],
-                         self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"].attrs[
-                             'dataSpacing'])
-                     for wl in self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}"]]
-
-            except KeyError:
-                raise KeyError(f"You asked for the PSFs in diffraction order {order}. But this data is not available")
-            self._psfs[ccd_index][order].sort()
-        return self._psfs[ccd_index][order]
-
-    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
-        if wavelength is None:
-            return self.psfs(order, fiber, ccd_index)
-        else:
-            # find the nearest PSF:
-            idx = min(range(len(self.psfs(order, fiber, ccd_index))),
-                      key=lambda i: abs(self.psfs(order, fiber, ccd_index)[i].wavelength - wavelength))
-            return self.psfs(order, fiber, ccd_index)[idx]
-
-    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
-            -> tuple[float, float]:
-        min_w = []
-        max_w = []
-
-        if ccd_index is None:
-            new_ccd_index = self.available_ccd_keys()
-        else:
-            new_ccd_index = [ccd_index]
-
-        for ci in new_ccd_index:
-            if fiber is None:
-                new_fiber = self.get_fibers(ci)
-            else:
-                new_fiber = [fiber]
-
-            for f in new_fiber:
-                if order is None:
-                    new_order = self.get_orders(f, ci)
-                else:
-                    new_order = [order]
-                for o in new_order:
-                    min_w.append(self.transformations(o, f, ci)[0].wavelength)
-                    max_w.append(self.transformations(o, f, ci)[-1].wavelength)
-        return min(min_w), max(max_w)
-
-    def available_ccd_keys(self) -> list[int]:
-        if not self._ccd_keys:
-            self._ccd_keys = [int(k[4:]) for k in self.h5f[f"/"].keys() if "CCD" in k]
-        return self._ccd_keys
-
-    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
-        if ccd_index is None:
-            return dict(zip(self.available_ccd_keys(), [self._read_ccd_from_hdf(k) for k in self.available_ccd_keys()]))
-
-        if ccd_index not in self._CCDs:
-            self._CCDs[ccd_index] = self._read_ccd_from_hdf(ccd_index)
-        return self._CCDs[ccd_index]
-
-    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
-        ge = GratingEfficiency(self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['blaze'],
-                               self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['blaze'],
-                               self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['gpmm'])
-
-        if ccd_index not in self._efficiency.keys():
-            self._efficiency[ccd_index] = {}
-        if fiber not in self._efficiency[ccd_index].keys():
-            try:
-                self._efficiency[ccd_index][fiber] = \
-                    SystemEfficiency([ge,
-                                      TabulatedEfficiency('System', *self.h5f[f"CCD_{ccd_index}/fiber_{fiber}"].attrs[
-                                          "efficiency"])], 'System')
-
-            except KeyError:
-                logging.warning(f'No spectrograph efficiency data found for fiber {fiber}.')
-                self._efficiency[ccd_index][fiber] = SystemEfficiency([ge], 'System')
-        return self._efficiency[ccd_index][fiber]
-
-    def __exit__(self):
-        if self._h5f:
-            self._h5f.close()
-
-
-class InteractiveZEMAX(Spectrograph):
-
-    def get_fibers(self, ccd_index: int = 1) -> list[int]:
-        pass
-
-    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
-        pass
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation]:
-        pass
-
-    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
-        pass
-
-    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) -> \
-            tuple[float, float]:
-        pass
-
-    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
-        pass
-
-    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
-        pass
-
-    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
-        pass
-
-
-class LocalDisturber(Spectrograph):
-
-    def __init__(self, spec: Spectrograph, d_tx=0., d_ty=0., d_rot=0., d_shear=0., d_sx=0., d_sy=0.):
-        self.spec = spec
-        for method in dir(Spectrograph):
-            if method.startswith('get_') and method != 'get_transformation':
-                setattr(self, method, getattr(self.spec, method))
-        self.disturber_matrix = AffineTransformation(d_rot, d_sx, d_sy, d_shear, d_tx, d_ty, None)
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
-        if isinstance(wavelength, float):
-            return self.spec.get_transformation(wavelength, order, fiber, ccd_index) + self.disturber_matrix
-        else:
-            return self.spec.get_transformation(wavelength, order, fiber, ccd_index) + \
-                   np.expand_dims(self.disturber_matrix.as_matrix(), axis=-1)
-
-
-class GlobalDisturber(Spectrograph):
-    def __init__(self, spec: Spectrograph, tx: float = 0., ty: float = 0., rot: float = 0., shear: float = 0.,
-                 sx: float = 1., sy: float = 1., reference_x: float = None, reference_y: float = None):
-        self.spec = spec
-        for method in dir(Spectrograph):
-            if method.startswith('get_') and method != 'get_transformation':
-                setattr(self, method, getattr(self.spec, method))
-        self.disturber_matrix = AffineTransformation(rot, sx, sy, shear, tx, ty, None)
-        self.ref_x = reference_x
-        self.ref_y = reference_y
-
-    def _get_transformation_matrix(self, dx, dy, wavelength):
-        if isinstance(wavelength, float):
-            return AffineTransformation(0., 1., 1., 0., dx, dy, wavelength)
-        else:
-            assert isinstance(wavelength, np.ndarray) or isinstance(wavelength, list)
-            n_wavelength = len(wavelength)
-            return np.array([[0.] * n_wavelength,
-                             [1.] * n_wavelength,
-                             [1.] * n_wavelength,
-                             [0.] * n_wavelength,
-                             [dx] * n_wavelength,
-                             [dy] * n_wavelength])
-
-    def _get_disturbance_matrix(self, wavelength):
-        if isinstance(wavelength, float):
-            return AffineTransformation(self.disturber_matrix.rot, self.disturber_matrix.sx,
-                                        self.disturber_matrix.sy, self.disturber_matrix.shear,
-                                        0., 0., wavelength)
-        else:
-            assert isinstance(wavelength, np.ndarray) or isinstance(wavelength, list)
-            n_wavelength = len(wavelength)
-            return np.array([[self.disturber_matrix.rot] * n_wavelength,
-                             [self.disturber_matrix.sx] * n_wavelength,
-                             [self.disturber_matrix.sy] * n_wavelength,
-                             [self.disturber_matrix.shear] * n_wavelength,
-                             [0.] * n_wavelength,
-                             [0.] * n_wavelength])
-
-    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
-                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
-        # by default take center of CCD as reference point
-        w, h = self.spec.get_ccd(ccd_index).data.shape
-        w /= 2.
-        h /= 2.
-
-        if self.ref_x is not None:
-            w = self.ref_x
-        if self.ref_y is not None:
-            h = self.ref_y
-
-        if isinstance(wavelength, float):
-            tm = self.spec.get_transformation(wavelength, order, fiber, ccd_index)
-            xy = tm.tx, tm.ty
-            # affine transformation to shift origin to center of image
-            tm_trans = self._get_transformation_matrix(-w / 2., -h / 2., tm.wavelength)
-            xy = tm_trans * xy
-            # affine transformation to rotate/shear/scale
-            tm_trans = self._get_disturbance_matrix(wavelength)
-            xy = tm_trans * xy
-            # affine transformation to shift origin back
-            tm_trans = AffineTransformation(0., 1., 1., 0., w / 2., h / 2., tm.wavelength)
-            xy = tm_trans * xy
-            tm.tx = xy[0] + self.disturber_matrix.tx
-            tm.ty = xy[1] + self.disturber_matrix.ty
-            return tm
-        else:
-            tm = self.spec.get_transformation(wavelength, order, fiber, ccd_index)
-            xy = tm[4:6].T
-            # affine transformation to shift origin to center of image
-            tm_trans = convert_matrix(self._get_transformation_matrix(-w / 2., -h / 2., wavelength))
-            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
-
-            tm_trans = convert_matrix(self._get_disturbance_matrix(wavelength))
-            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
-
-            # affine transformation to shift origin back
-            tm_trans = convert_matrix(self._get_transformation_matrix(w / 2., h / 2., wavelength))
-            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
-            tm[4:6] = xy.T
-            tm[4] += self.disturber_matrix.tx
-            tm[5] += self.disturber_matrix.ty
-            return tm
+from __future__ import annotations
+
+import logging
+import urllib.request
+from dataclasses import dataclass
+from pathlib import Path
+from urllib.error import URLError
+
+import h5py
+import numpy as np
+
+from pyechelle.CCD import CCD
+from pyechelle.efficiency import SystemEfficiency, GratingEfficiency, TabulatedEfficiency, ConstantEfficiency
+from pyechelle.optics import AffineTransformation, PSF, TransformationSet, convert_matrix, apply_matrix
+
+from ftplib import FTP
+
+def check_FTP_url_exists(url):
+    assert url.lower().startswith('ftp://')
+    url = url[6:]
+    ftp_host = url.split('/')[0]
+    file_path = '/'.join(url.split('/')[1:])
+
+    try:
+        ftp = FTP(ftp_host)
+        ftp.login()
+        file_list = ftp.nlst(file_path)
+        ftp.quit()
+        return file_path in file_list
+    except Exception as e:
+        print(f"An error occurred: {str(e)}")
+        return False
+
+def check_url_exists(url: str) -> bool:
+    """
+    Check if URL exists.
+    Args:
+        url: url to be tested
+
+    Returns:
+        if URL exists
+    """
+    if url.lower().startswith('ftp:'):
+        return check_FTP_url_exists(url)
+    try:
+        with urllib.request.urlopen(url, timeout=3) as response:
+            return float(response.headers['Content-length']) > 0
+    except URLError:
+        return False
+
+
+def check_for_spectrograph_model(model_name: str, download=True):
+    """
+    Check if spectrograph model exists locally. Otherwise: Download if download is true (default) or check if URL to
+    spectrograph model is valid (this is mainly for testing purpose).
+
+    Args:
+        model_name: name of spectrograph model. See models/available_models.txt for valid names
+        download: download flag
+
+    Returns:
+
+    """
+    file_path = Path(__file__).resolve().parent.joinpath("models").joinpath(f"{model_name}.hdf")
+    if not file_path.is_file():
+        url = f"https://stuermer.science/nextcloud/index.php/s/ps5Pk379LgcpLwN/download?path=/&files={model_name}.hdf"
+        if download:
+            print(f"Spectrograph model {model_name} not found locally. Trying to download from {url}...")
+            Path(Path(__file__).resolve().parent.joinpath("models")).mkdir(parents=False, exist_ok=True)
+            with urllib.request.urlopen(url) as response, open(file_path, "wb") as out_file:
+                data = response.read()
+                out_file.write(data)
+        else:
+            check_url_exists(url)
+    return file_path
+
+
+@dataclass
+class Spectrograph:
+    """ Abstract spectrograph model
+
+    Describes all methods that a spectrograph model must have to be used in a simulation. \n
+    When subclassing, all methods need to be implemented in the subclass.
+
+    A spectrograph model as at least one CCD (with CCD_index 1), at least one field/fiber (with fiber index 1),
+    and at least one diffraction order.
+    """
+    name: str = 'Spectrograph'
+
+    def get_fibers(self, ccd_index: int = 1) -> list[int]:
+        """ Fields/fiber indices
+
+        Args:
+            ccd_index: CCD index
+
+        Returns:
+            available fields/fiber indices
+        """
+        raise NotImplementedError
+
+    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
+        """ Diffraction orders
+
+        Args:
+            fiber: fiber/field index
+            ccd_index: CCD index
+
+        Returns:
+            available diffraction order(s) for given indices
+        """
+        raise NotImplementedError
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
+        """ Transformation matrix/matrices
+
+        Args:
+            wavelength: wavelength(s) [micron]
+            order: diffraction order
+            fiber: fiber index
+            ccd_index: CCD index
+
+        Returns:
+            transformation matrix/matrices
+        """
+        raise NotImplementedError
+
+    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
+        """ PSF
+
+        PSFs are tabulated. When wavelength is provided, the closest available PSF of the model is returned.
+
+        When wavelength is None, all PSFs for that particular order (and fiber and CCD index) are returned.
+
+        Args:
+            wavelength: wavelength [micron] or None
+            order: diffraction order
+            fiber: fiber index
+            ccd_index: ccd index
+
+        Returns:
+            PSF(s)
+        """
+        raise NotImplementedError
+
+    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
+            -> tuple[float, float]:
+        """ Wavelength range
+
+        Returns minimum and maximum wavelength of the entire spectrograph unit or an individual order if specified.
+
+        Args:
+            ccd_index: CCD index
+            fiber: fiber index
+            order: diffraction order
+
+        Returns:
+            minimum and maximum wavelength [microns]
+        """
+        raise NotImplementedError
+
+    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
+        """ Get CCD object(s)
+
+        When index is provided the corresponding CCD object is returned.\n
+        If no index is provided, all available CCDs are return as a dict with the index as key.
+
+        Args:
+            ccd_index: CCD index
+
+        Returns:
+            CCD object(s)
+        """
+        raise NotImplementedError
+
+    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
+        """ Shape of field/fiber
+
+        Returning the field/fiber shape for the given indices as a string.
+        See slit.py for currently implemented shapes.
+
+        Args:
+            fiber: fiber index
+            ccd_index: ccd index
+
+        Returns:
+            field/fiber shape as string (e.g. rectangular, octagonal)
+        """
+        raise NotImplementedError
+
+    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
+        """ Spectrograph efficiency
+
+        Args:
+            fiber: fiber/field index
+            ccd_index: CCD index
+
+        Returns:
+            System efficiency for given indices
+        """
+        raise NotImplementedError
+
+
+class SimpleSpectrograph(Spectrograph):
+    def __init__(self):
+        self._ccd = {1: CCD()}
+        self._fibers = {}
+        self._orders = {}
+        self._transformations = {}
+        for c in self._ccd.keys():
+            self._fibers[c] = [1]
+            self._orders[c] = {}
+            for f in self._fibers.keys():
+                self._orders[c][f] = [1]
+
+    def get_fibers(self, ccd_index: int = 1) -> list[int]:
+        return self._fibers[ccd_index]
+
+    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
+        return self._orders[ccd_index][fiber]
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation]:
+        if isinstance(wavelength, float):
+            return AffineTransformation(0.0, 1.0, 10., 0., (wavelength - 0.5) * wavelength * 100000. + 2000.,
+                                        fiber * 10. + 2000., wavelength)
+        else:
+            ts = TransformationSet([AffineTransformation(0.0, 1.0, 10., 0., (w - 0.5) * w * 100000. + 2000.,
+                                                         fiber * 10. + 2000., w) for w in wavelength])
+            return ts.get_affine_transformations(wavelength)
+
+    @staticmethod
+    def gauss_map(size_x, size_y=None, sigma_x=5., sigma_y=None):
+        if size_y is None:
+            size_y = size_x
+        if sigma_y is None:
+            sigma_y = sigma_x
+
+        assert isinstance(size_x, int)
+        assert isinstance(size_y, int)
+
+        x0 = size_x // 2
+        y0 = size_y // 2
+
+        x = np.arange(0, size_x, dtype=float)
+        y = np.arange(0, size_y, dtype=float)[:, np.newaxis]
+
+        x -= x0
+        y -= y0
+
+        exp_part = x ** 2 / (2 * sigma_x ** 2) + y ** 2 / (2 * sigma_y ** 2)
+        return 1 / (2 * np.pi * sigma_x * sigma_y) * np.exp(-exp_part)
+
+    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
+        if wavelength is None:
+            wl = np.linspace(*self.get_wavelength_range(order, fiber, ccd_index), 20)
+            return [PSF(w, self.gauss_map(11, sigma_x=3., sigma_y=10.), 1.5) for w in wl]
+        else:
+            return PSF(wavelength, self.gauss_map(11, sigma_x=3., sigma_y=10.), 1.5)
+
+    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
+            -> tuple[float, float]:
+        return 0.4, 0.6
+
+    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
+        if ccd_index is None:
+            return self._ccd
+        else:
+            return self._ccd[ccd_index]
+
+    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
+        return 'rectangular'
+
+    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
+        return SystemEfficiency([ConstantEfficiency(1.0)], 'System')
+
+
+class AtmosphericDispersion(Spectrograph):
+    """
+    Atmospheric Dispersion
+
+    Simulates atmospheric dispersion from 300nm to 2microns.
+    The model does not include atmospheric transmission as an efficiency model.
+    In case you want to use this, please explicitly add the atmospheric model via the simulator.
+
+    Attributes:
+        zd: zenith distance [deg]
+        pressure: air pressure [Pa]
+        temperature: air temperature [K]
+        r_wl: undisturbed wavelength [micron]
+        pixel_scale: arcsec per pixel [arcsec]
+        seeing: seeing at reference_wavelength [arcsec]
+        ccd_size: number of pixels in X and Y direction
+    """
+
+    def __init__(self, zd: float, pressure=775E2, temperature=283.15, reference_wavelength: float = 0.35,
+                 pixel_scale: float = 0.1, seeing: float = 1.0, ccd_size: int = 80):
+        """ Constructor
+
+        Args:
+            zd: zenith distance [deg]
+            pressure: air pressue [Pa]
+            temperature: air temperature [K]
+            reference_wavelength: undisturbed wavelength [micron]
+            pixel_scale: arcsec per pixel [arcsec]
+            seeing: seeing at reference_wavelength [arcsec]
+            ccd_size: number of pixels in X and Y direction for simulated output
+        """
+        self.ccd_size = ccd_size
+        self._ccd = {1: CCD(self.ccd_size, self.ccd_size, pixelsize=1)}
+        self._fibers = {}
+        self._orders = {}
+        self._transformations = {}
+        self.pressure = pressure
+        self.temperature = temperature
+        self.r_wl = reference_wavelength
+        self.pixel_scale = pixel_scale
+        self.zd = zd
+        self.seeing = seeing
+        for c in self._ccd.keys():
+            self._fibers[c] = [1]
+            self._orders[c] = {}
+            for f in self._fibers.keys():
+                self._orders[c][f] = [1]
+
+    def refractive_index(self, wl: float | np.ndarray) -> float | np.ndarray:
+        """ Calculates the refractive index depending on atmospheric condition and ZD
+
+        reference:
+        http://www.ls.eso.org/sci/facilities/lasilla/instruments/feros/Projects/ADC/references/refraction/index.html
+
+        Args:
+            wl: wavelength(s) [micron]
+
+        Returns:
+            refractive index at given wavelength for given conditions
+        """
+        P0 = 1013.25E2
+        T0 = 288.15
+        return (64.328 + 29498.1E-6 / (146E-6 - (1 / (wl * 1000.)) ** 2) + 255.4E-6 / (
+                    41E-4 - (1 / (wl * 1000.)) ** 2)) * \
+            self.pressure / self.temperature * T0 / P0
+
+    def delta_R(self, wl: np.ndarray | float) -> float | np.ndarray:
+        """ Differential refraction
+
+        Returns difference in refraction for given wavelength(s)
+        Args:
+            wl: wavelength(s) [micron]
+
+        Returns:
+            refraction [arcsec]
+        """
+        return 206264.80625 / 1E6 * ((self.refractive_index(wl) - 1) - (self.refractive_index(self.r_wl) - 1)) \
+            * np.tan(np.deg2rad(self.zd))
+
+    def get_fibers(self, ccd_index: int = 1) -> list[int]:
+        return self._fibers[ccd_index]
+
+    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
+        return self._orders[ccd_index][fiber]
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation]:
+        if isinstance(wavelength, float):
+            return AffineTransformation(0.0, 1.0, 1., 0., self._ccd[1].n_pix_x / 2.,
+                                        self._ccd[1].n_pix_y / 2. - self.delta_R(
+                                            wavelength) / self.pixel_scale,
+                                        wavelength)
+        else:
+            ts = TransformationSet([AffineTransformation(0.0, 1.0, 1., 0., self._ccd[1].n_pix_x / 2.,
+                                                         self._ccd[1].n_pix_y / 2. - self.delta_R(
+                                                             w) / self.pixel_scale,
+                                                         w) for w in wavelength])
+            return ts.get_affine_transformations(wavelength)
+
+    @staticmethod
+    def gauss_map(size_x, size_y=None, sigma_x=5., sigma_y=None):
+        if size_y is None:
+            size_y = size_x
+        if sigma_y is None:
+            sigma_y = sigma_x
+
+        assert isinstance(size_x, int)
+        assert isinstance(size_y, int)
+
+        x0 = size_x // 2
+        y0 = size_y // 2
+
+        x = np.arange(0, size_x, dtype=float)
+        y = np.arange(0, size_y, dtype=float)[:, np.newaxis]
+
+        x -= x0
+        y -= y0
+
+        exp_part = x ** 2 / (2 * sigma_x ** 2) + y ** 2 / (2 * sigma_y ** 2)
+        return 1 / (2 * np.pi * sigma_x * sigma_y) * np.exp(-exp_part)
+
+    def seeing_disc_diameter(self, wl):
+        """ Returns seeing disc diameter in pixel for given pixel scale and seeing"""
+        seeing_wl = self.seeing * (wl/self.r_wl)**(-1./5.)
+        return (seeing_wl / self.pixel_scale) / 2.
+
+    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
+        if wavelength is None:
+            wl = np.linspace(*self.get_wavelength_range(order, fiber, ccd_index), 20)
+            return [PSF(w, self.gauss_map(50, sigma_x=self.seeing_disc_diameter(w),
+                                          sigma_y=self.seeing_disc_diameter(w)), 1.) for w in wl]
+        else:
+            return PSF(wavelength, self.gauss_map(50, sigma_x=self.seeing_disc_diameter(wavelength),
+                                                  sigma_y=self.seeing_disc_diameter(wavelength)), 1.)
+
+    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
+            -> tuple[float, float]:
+        return 0.3, 2.0
+
+    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
+        if ccd_index is None:
+            return self._ccd
+        else:
+            return self._ccd[ccd_index]
+
+    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
+        return 'singlemode'
+
+    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
+        return SystemEfficiency([ConstantEfficiency(1.0)], 'System')
+
+
+class ZEMAX(Spectrograph):
+    def __init__(self, path: str | Path):
+        self.path = check_for_spectrograph_model(path)
+        self._CCDs = {}
+        self._ccd_keys = []
+        self._h5f = None
+
+        self._transformations = {}
+        self._spline_transformations = {}
+        self._psfs = {}
+        self._efficiency = {}
+
+        # self.name = self.h5f[f"Spectrograph"].attrs['name']
+        self._field_shape = {}
+
+        self._orders = {}
+
+        self.CCD = [self._read_ccd_from_hdf]
+
+    @property
+    def h5f(self):
+        if self._h5f is None:
+            self._h5f = h5py.File(self.path, "r")
+        return self._h5f
+
+    def _read_ccd_from_hdf(self, k) -> CCD:
+        # read in CCD information
+        nx = self.h5f[f"CCD_{k}"].attrs['Nx']
+        ny = self.h5f[f"CCD_{k}"].attrs['Ny']
+        ps = self.h5f[f"CCD_{k}"].attrs['pixelsize']
+        return CCD(n_pix_x=nx, n_pix_y=ny, pixelsize=ps)
+
+    def get_fibers(self, ccd_index: int = 1) -> list[int]:
+        return [int(k[6:]) for k in self.h5f[f"CCD_{ccd_index}"].keys() if "fiber" in k]
+
+    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
+        if ccd_index not in self._field_shape.keys():
+            self._field_shape[ccd_index] = {}
+        if fiber not in self._field_shape[ccd_index].keys():
+            fs = self.h5f[f"CCD_{ccd_index}/fiber_{fiber}"].attrs["field_shape"]
+            self._field_shape[ccd_index][fiber] = fs.decode("utf-8") if isinstance(fs, bytes) else fs
+        return self._field_shape[ccd_index][fiber]
+
+    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
+        if ccd_index not in self._orders.keys():
+            self._orders[ccd_index] = {}
+        if fiber not in self._orders[ccd_index].keys():
+            self._orders[ccd_index][fiber] = [int(k[5:]) for k
+                                              in self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/"].keys() if "psf" not in k]
+            self._orders[ccd_index][fiber].sort()
+        return self._orders[ccd_index][fiber]
+
+    def transformations(self, order: int, fiber: int = 1, ccd_index: int = 1) -> list[AffineTransformation]:
+        if ccd_index not in self._transformations.keys():
+            self._transformations[ccd_index] = {}
+        if fiber not in self._transformations[ccd_index].keys():
+            self._transformations[ccd_index][fiber] = {}
+        if order not in self._transformations[ccd_index][fiber].keys():
+            try:
+                self._transformations[ccd_index][fiber][order] = [AffineTransformation(*af)
+                                                                  for af in
+                                                                  self.h5f[
+                                                                      f"CCD_{ccd_index}/fiber_{fiber}/order{order}"][
+                                                                      ()]]
+                self._transformations[ccd_index][fiber][order].sort()
+
+            except KeyError:
+                raise KeyError(
+                    f"You asked for the affine transformation matrices in diffraction order {order}. "
+                    f"But this data is not available")
+
+        return self._transformations[ccd_index][fiber][order]
+
+    def spline_transformations(self, order: int, fiber: int = 1, ccd_index: int = 1) -> TransformationSet:
+        if ccd_index not in self._spline_transformations.keys():
+            self._spline_transformations[ccd_index] = {}
+        if fiber not in self._spline_transformations[ccd_index].keys():
+            self._spline_transformations[ccd_index][fiber] = {}
+        if order not in self._spline_transformations[ccd_index][fiber].keys():
+            tfs = self.transformations(order, fiber, ccd_index)
+            self._spline_transformations[ccd_index][fiber][order] = TransformationSet(tfs)
+        return self._spline_transformations[ccd_index][fiber][order]
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation] | np.ndarray:
+        return self.spline_transformations(order, fiber, ccd_index).get_affine_transformations(wavelength)
+
+    def psfs(self, order: int, fiber: int = 1, ccd_index: int = 1) -> list[PSF]:
+        if ccd_index not in self._psfs.keys():
+            self._psfs[ccd_index] = {}
+        if order not in self._psfs[ccd_index].keys():
+            try:
+                self._psfs[ccd_index][order] = \
+                    [PSF(self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"].attrs['wavelength'],
+                         self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"][()],
+                         self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}/{wl}"].attrs[
+                             'dataSpacing'])
+                     for wl in self.h5f[f"CCD_{ccd_index}/fiber_{fiber}/psf_order_{order}"]]
+
+            except KeyError:
+                raise KeyError(f"You asked for the PSFs in diffraction order {order}. But this data is not available")
+            self._psfs[ccd_index][order].sort()
+        return self._psfs[ccd_index][order]
+
+    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
+        if wavelength is None:
+            return self.psfs(order, fiber, ccd_index)
+        else:
+            # find the nearest PSF:
+            idx = min(range(len(self.psfs(order, fiber, ccd_index))),
+                      key=lambda i: abs(self.psfs(order, fiber, ccd_index)[i].wavelength - wavelength))
+            return self.psfs(order, fiber, ccd_index)[idx]
+
+    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) \
+            -> tuple[float, float]:
+        min_w = []
+        max_w = []
+
+        if ccd_index is None:
+            new_ccd_index = self.available_ccd_keys()
+        else:
+            new_ccd_index = [ccd_index]
+
+        for ci in new_ccd_index:
+            if fiber is None:
+                new_fiber = self.get_fibers(ci)
+            else:
+                new_fiber = [fiber]
+
+            for f in new_fiber:
+                if order is None:
+                    new_order = self.get_orders(f, ci)
+                else:
+                    new_order = [order]
+                for o in new_order:
+                    min_w.append(self.transformations(o, f, ci)[0].wavelength)
+                    max_w.append(self.transformations(o, f, ci)[-1].wavelength)
+        return min(min_w), max(max_w)
+
+    def available_ccd_keys(self) -> list[int]:
+        if not self._ccd_keys:
+            self._ccd_keys = [int(k[4:]) for k in self.h5f[f"/"].keys() if "CCD" in k]
+        return self._ccd_keys
+
+    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
+        if ccd_index is None:
+            return dict(zip(self.available_ccd_keys(), [self._read_ccd_from_hdf(k) for k in self.available_ccd_keys()]))
+
+        if ccd_index not in self._CCDs:
+            self._CCDs[ccd_index] = self._read_ccd_from_hdf(ccd_index)
+        return self._CCDs[ccd_index]
+
+    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
+        ge = GratingEfficiency(self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['blaze'],
+                               self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['blaze'],
+                               self.h5f[f"CCD_{ccd_index}/Spectrograph"].attrs['gpmm'])
+
+        if ccd_index not in self._efficiency.keys():
+            self._efficiency[ccd_index] = {}
+        if fiber not in self._efficiency[ccd_index].keys():
+            try:
+                self._efficiency[ccd_index][fiber] = \
+                    SystemEfficiency([ge,
+                                      TabulatedEfficiency('System', *self.h5f[f"CCD_{ccd_index}/fiber_{fiber}"].attrs[
+                                          "efficiency"])], 'System')
+
+            except KeyError:
+                logging.warning(f'No spectrograph efficiency data found for fiber {fiber}.')
+                self._efficiency[ccd_index][fiber] = SystemEfficiency([ge], 'System')
+        return self._efficiency[ccd_index][fiber]
+
+    def __exit__(self):
+        if self._h5f:
+            self._h5f.close()
+
+
+class InteractiveZEMAX(Spectrograph):
+
+    def get_fibers(self, ccd_index: int = 1) -> list[int]:
+        pass
+
+    def get_orders(self, fiber: int = 1, ccd_index: int = 1) -> list[int]:
+        pass
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | list[AffineTransformation]:
+        pass
+
+    def get_psf(self, wavelength: float | None, order: int, fiber: int = 1, ccd_index: int = 1) -> PSF | list[PSF]:
+        pass
+
+    def get_wavelength_range(self, order: int | None = None, fiber: int | None = None, ccd_index: int | None = None) -> \
+            tuple[float, float]:
+        pass
+
+    def get_ccd(self, ccd_index: int | None = None) -> CCD | dict[int, CCD]:
+        pass
+
+    def get_field_shape(self, fiber: int, ccd_index: int) -> str:
+        pass
+
+    def get_efficiency(self, fiber: int, ccd_index: int) -> SystemEfficiency:
+        pass
+
+
+class LocalDisturber(Spectrograph):
+
+    def __init__(self, spec: Spectrograph, d_tx=0., d_ty=0., d_rot=0., d_shear=0., d_sx=0., d_sy=0.):
+        self.spec = spec
+        for method in dir(Spectrograph):
+            if method.startswith('get_') and method != 'get_transformation':
+                setattr(self, method, getattr(self.spec, method))
+        self.disturber_matrix = AffineTransformation(d_rot, d_sx, d_sy, d_shear, d_tx, d_ty, None)
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
+        if isinstance(wavelength, float):
+            return self.spec.get_transformation(wavelength, order, fiber, ccd_index) + self.disturber_matrix
+        else:
+            return self.spec.get_transformation(wavelength, order, fiber, ccd_index) + \
+                np.expand_dims(self.disturber_matrix.as_matrix(), axis=-1)
+
+
+class GlobalDisturber(Spectrograph):
+    def __init__(self, spec: Spectrograph, tx: float = 0., ty: float = 0., rot: float = 0., shear: float = 0.,
+                 sx: float = 1., sy: float = 1., reference_x: float = None, reference_y: float = None):
+        self.spec = spec
+        for method in dir(Spectrograph):
+            if method.startswith('get_') and method != 'get_transformation':
+                setattr(self, method, getattr(self.spec, method))
+        self.disturber_matrix = AffineTransformation(rot, sx, sy, shear, tx, ty, None)
+        self.ref_x = reference_x
+        self.ref_y = reference_y
+
+    def _get_transformation_matrix(self, dx, dy, wavelength):
+        if isinstance(wavelength, float):
+            return AffineTransformation(0., 1., 1., 0., dx, dy, wavelength)
+        else:
+            assert isinstance(wavelength, np.ndarray) or isinstance(wavelength, list)
+            n_wavelength = len(wavelength)
+            return np.array([[0.] * n_wavelength,
+                             [1.] * n_wavelength,
+                             [1.] * n_wavelength,
+                             [0.] * n_wavelength,
+                             [dx] * n_wavelength,
+                             [dy] * n_wavelength])
+
+    def _get_disturbance_matrix(self, wavelength):
+        if isinstance(wavelength, float):
+            return AffineTransformation(self.disturber_matrix.rot, self.disturber_matrix.sx,
+                                        self.disturber_matrix.sy, self.disturber_matrix.shear,
+                                        0., 0., wavelength)
+        else:
+            assert isinstance(wavelength, np.ndarray) or isinstance(wavelength, list)
+            n_wavelength = len(wavelength)
+            return np.array([[self.disturber_matrix.rot] * n_wavelength,
+                             [self.disturber_matrix.sx] * n_wavelength,
+                             [self.disturber_matrix.sy] * n_wavelength,
+                             [self.disturber_matrix.shear] * n_wavelength,
+                             [0.] * n_wavelength,
+                             [0.] * n_wavelength])
+
+    def get_transformation(self, wavelength: float | np.ndarray, order: int, fiber: int = 1,
+                           ccd_index: int = 1) -> AffineTransformation | np.ndarray:
+        # by default take center of CCD as reference point
+        w, h = self.spec.get_ccd(ccd_index).data.shape
+        w /= 2.
+        h /= 2.
+
+        if self.ref_x is not None:
+            w = self.ref_x
+        if self.ref_y is not None:
+            h = self.ref_y
+
+        if isinstance(wavelength, float):
+            tm = self.spec.get_transformation(wavelength, order, fiber, ccd_index)
+            xy = tm.tx, tm.ty
+            # affine transformation to shift origin to center of image
+            tm_trans = self._get_transformation_matrix(-w / 2., -h / 2., tm.wavelength)
+            xy = tm_trans * xy
+            # affine transformation to rotate/shear/scale
+            tm_trans = self._get_disturbance_matrix(wavelength)
+            xy = tm_trans * xy
+            # affine transformation to shift origin back
+            tm_trans = AffineTransformation(0., 1., 1., 0., w / 2., h / 2., tm.wavelength)
+            xy = tm_trans * xy
+            tm.tx = xy[0] + self.disturber_matrix.tx
+            tm.ty = xy[1] + self.disturber_matrix.ty
+            return tm
+        else:
+            tm = self.spec.get_transformation(wavelength, order, fiber, ccd_index)
+            xy = tm[4:6].T
+            # affine transformation to shift origin to center of image
+            tm_trans = convert_matrix(self._get_transformation_matrix(-w / 2., -h / 2., wavelength))
+            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
+
+            tm_trans = convert_matrix(self._get_disturbance_matrix(wavelength))
+            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
+
+            # affine transformation to shift origin back
+            tm_trans = convert_matrix(self._get_transformation_matrix(w / 2., h / 2., wavelength))
+            xy = np.array([apply_matrix(c, p) for c, p in zip(tm_trans.T, xy)])
+            tm[4:6] = xy.T
+            tm[4] += self.disturber_matrix.tx
+            tm[5] += self.disturber_matrix.ty
+            return tm
```

### Comparing `pyechelle-0.3.5/pyproject.toml` & `pyechelle-0.3.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,68 @@
-[tool.poetry]
-name = "pyechelle"
-version = "0.3.5"
-description = "A fast generic spectrum simulator"
-authors = ["Julian Stuermer <julian@stuermer.science>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://gitlab.com/Stuermer/pyechelle"
-repository = "https://gitlab.com/Stuermer/pyechelle"
-documentation = "https://stuermer.gitlab.io/pyechelle/"
-include = ["models/available_models.txt"]
-
-[tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-astropy = "^5.1.1"
-h5py = "^3.7.0"
-scipy = "^1.9.3"
-parmap = "^1.6.0"
-numba = "^0.56.4"
-plotly = "^5.11.0"
-pandas = "^1.5.2"
-skycalc-ipy = "^0.1.3"
-astroquery = "^0.4.6"
-joblib = "^1.2.0"
-matplotlib = "^3.6.2"
-
-[tool.poetry.dev-dependencies]
-hypothesis = "^6.58.2"
-pytest = "^7.2.0"
-coverage = { extras = ["toml"], version = "^6.5.0" }
-sphinx-argparse = "^0.4.0"
-sphinx-rtd-theme = "^1.1.1"
-pytest-benchmark = "^4.0.0"
-pytest-cov = "^4.0.0"
-sphinx-autodoc-annotation = "^1.0-1"
-sphinx-copybutton = "^0.5.1"
-Sphinx = "^5.3.0"
-poetryup = "^0.12.5"
-
-[tool.coverage.paths]
-source = ["pyechelle"]
-
-[tool.coverage.run]
-branch = true
-source = ["pyechelle"]
-
-[tool.coverage.report]
-show_missing = true
-
-[tool.coverage.html]
-directory = "tests/coverage"
-
-[tool.poetry.scripts]
-pyechelle = "pyechelle.simulator:main"
-
-[build-system]
-requires = ["poetry-core>=1.0.0a5"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "pyechelle"
+version = "0.3.6"
+description = "A fast generic spectrum simulator"
+authors = ["Julian Stuermer <julian@stuermer.science>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://gitlab.com/Stuermer/pyechelle"
+repository = "https://gitlab.com/Stuermer/pyechelle"
+documentation = "https://stuermer.gitlab.io/pyechelle/"
+include = ["models/available_models.txt"]
+
+[tool.poetry.dependencies]
+python = ">=3.8,<3.12"
+astropy = "^5.2.2"
+h5py = "^3.9.0"
+scipy = "^1.10.1"
+parmap = "^1.6.0"
+plotly = "^5.15.0"
+pandas = "^1.5.3"
+skycalc-ipy = "^0.1.3"
+astroquery = "^0.4.6"
+joblib = "^1.3.1"
+matplotlib = "^3.7.2"
+synphot = "^1.2.1"
+numba = "^0.57.1"
+
+[tool.poetry.group.dev.dependencies]
+hypothesis = "^6.80.1"
+pytest = "^7.4.0"
+coverage = { extras = ["toml"], version = "^6.5.0" }
+sphinx-argparse = "^0.4.0"
+sphinx-rtd-theme = "^1.2.2"
+pytest-benchmark = "^4.0.0"
+pytest-cov = "^4.1.0"
+sphinx-autodoc-annotation = "^1.0-1"
+sphinx-copybutton = "^0.5.2"
+Sphinx = "^5.3.0"
+poetryup = "^0.12.7"
+pytest-env = "^0.8.2"
+setuptools = "^68.0.0"
+pytest-timeout = "^2.1.0"
+
+[tool.pytest.ini_options]
+timeout = "300"
+env = [
+    "NUMBA_DISABLE_JIT=4",
+]
+
+[tool.coverage.paths]
+source = ["pyechelle"]
+
+[tool.coverage.run]
+branch = true
+source = ["pyechelle"]
+
+[tool.coverage.report]
+show_missing = true
+
+[tool.coverage.html]
+directory = "tests/coverage"
+
+[tool.poetry.scripts]
+pyechelle = "pyechelle.simulator:main"
+
+[build-system]
+requires = ["poetry-core>=1.0.0a5"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pyechelle-0.3.5/setup.py` & `pyechelle-0.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyechelle
+Version: 0.3.6
+Summary: A fast generic spectrum simulator
+Home-page: https://gitlab.com/Stuermer/pyechelle
+License: MIT
+Author: Julian Stuermer
+Author-email: julian@stuermer.science
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Requires-Dist: astroquery (>=0.4.6,<0.5.0)
+Requires-Dist: h5py (>=3.9.0,<4.0.0)
+Requires-Dist: joblib (>=1.3.1,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: numba (>=0.57.1,<0.58.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: parmap (>=1.6.0,<2.0.0)
+Requires-Dist: plotly (>=5.15.0,<6.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: skycalc-ipy (>=0.1.3,<0.2.0)
+Requires-Dist: synphot (>=1.2.1,<2.0.0)
+Project-URL: Documentation, https://stuermer.gitlab.io/pyechelle/
+Project-URL: Repository, https://gitlab.com/Stuermer/pyechelle
+Description-Content-Type: text/markdown
 
-packages = \
-['pyechelle']
+# PyEchelle
 
-package_data = \
-{'': ['*'], 'pyechelle': ['models/available_models.txt']}
+PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
+However, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit
+spectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include
+photon and read-out noise.
 
-install_requires = \
-['astropy>=5.1.1,<6.0.0',
- 'astroquery>=0.4.6,<0.5.0',
- 'h5py>=3.7.0,<4.0.0',
- 'joblib>=1.2.0,<2.0.0',
- 'matplotlib>=3.6.2,<4.0.0',
- 'numba>=0.56.4,<0.57.0',
- 'pandas>=1.5.2,<2.0.0',
- 'parmap>=1.6.0,<2.0.0',
- 'plotly>=5.11.0,<6.0.0',
- 'scipy>=1.9.3,<2.0.0',
- 'skycalc-ipy>=0.1.3,<0.2.0']
-
-entry_points = \
-{'console_scripts': ['pyechelle = pyechelle.simulator:main']}
-
-setup_kwargs = {
-    'name': 'pyechelle',
-    'version': '0.3.5',
-    'description': 'A fast generic spectrum simulator',
-    'long_description': '# PyEchelle\n\nPyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.\nHowever, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit\nspectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include\nphoton and read-out noise.\n\nPyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major\nspeed improvements.\n\n### Example usage\n\nYou can use PyEchelle directly from the console:\n\n```bash\npyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit\n```\n\nIf you rather script in python, you can do the same as above with the following python script:\n\n```python\n\nfrom pyechelle.simulator import Simulator\nfrom pyechelle.sources import Phoenix\nfrom pyechelle.spectrograph import ZEMAX\n\nsim = Simulator(ZEMAX("MaroonX"))\nsim.set_ccd(1)\nsim.set_fibers([2, 3, 4])\nsim.set_sources(Phoenix(t_eff=3500))\nsim.set_exposure_time(10.)\nsim.set_radial_velocities(100.)\nsim.set_output(\'mdwarf.fits\', overwrite=True)\nsim.run()\n\n```\n\nBoth times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X\nspectrograph is simulated.\n\nThe output is a 2D raw frame (.fits) and will look similar to:\n\n![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")\n\nCheck out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.\n\nPyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar\nfunctionality but was written in C++. This package was rewritten in python for better maintainability, easier package\ndistribution and for smoother cross-platform development.\n\n# Installation\n\nAs simple as\n\n```bash\npip install pyechelle\n```\n\nCheck out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.\n\n# Usage\n\nSee\n\n```bash\npyechelle -h\n```\n\nfor all available command line options.\n\nSee [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.\n\n# Concept:\n\nThe basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and\npoint spread functions which describe the spectrographs\' optics:\n\nFirst, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.\nAs the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle\norder, these matrices can be interpolated for any intermediate wavelength.\n\nSecond, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly\naccount for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for\ninterpolation at intermediate wavelength.\n\n![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")\n\n**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate\nspectra without access to ZEMAX**\n\n# Citation\n\nPlease cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.\n',
-    'author': 'Julian Stuermer',
-    'author_email': 'julian@stuermer.science',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.com/Stuermer/pyechelle',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+PyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major
+speed improvements.
 
+### Example usage
+
+You can use PyEchelle directly from the console:
+
+```bash
+pyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit
+```
+
+If you rather script in python, you can do the same as above with the following python script:
+
+```python
+
+from pyechelle.simulator import Simulator
+from pyechelle.sources import Phoenix
+from pyechelle.spectrograph import ZEMAX
+
+sim = Simulator(ZEMAX("MaroonX"))
+sim.set_ccd(1)
+sim.set_fibers([2, 3, 4])
+sim.set_sources(Phoenix(t_eff=3500))
+sim.set_exposure_time(10.)
+sim.set_radial_velocities(100.)
+sim.set_output('mdwarf.fits', overwrite=True)
+sim.run()
+
+```
+
+Both times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X
+spectrograph is simulated.
+
+The output is a 2D raw frame (.fits) and will look similar to:
+
+![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+Pyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar
+functionality but was written in C++. This package was rewritten in python for better maintainability, easier package
+distribution and for smoother cross-platform development.
+
+# Installation
+
+As simple as
+
+```bash
+pip install pyechelle
+```
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.
+
+# Usage
+
+See
+
+```bash
+pyechelle -h
+```
+
+for all available command line options.
+
+See [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+# Concept:
+
+The basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and
+point spread functions which describe the spectrographs' optics:
+
+First, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.
+As the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle
+order, these matrices can be interpolated for any intermediate wavelength.
+
+Second, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly
+account for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for
+interpolation at intermediate wavelength.
+
+![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")
+
+**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate
+spectra without access to ZEMAX**
+
+# Citation
+
+Please cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.
 
-setup(**setup_kwargs)
```

