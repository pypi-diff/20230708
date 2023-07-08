# Comparing `tmp/alphacore-0.0.7.tar.gz` & `tmp/alphacore-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphacore-0.0.7.tar", last modified: Thu Jan  5 10:41:36 2023, max compression
+gzip compressed data, was "alphacore-0.0.8.tar", last modified: Sat Jul  8 05:38:25 2023, max compression
```

## Comparing `alphacore-0.0.7.tar` & `alphacore-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.852152 alphacore-0.0.7/
--rw-rw-rw-   0        0        0        6 2023-01-05 10:33:56.000000 alphacore-0.0.7/.gitignore
--rw-rw-rw-   0        0        0     7817 2020-04-27 03:35:53.000000 alphacore-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       90 2022-11-29 01:51:08.000000 alphacore-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      578 2023-01-05 10:41:36.852152 alphacore-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       51 2022-11-29 01:28:57.000000 alphacore-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.789654 alphacore-0.0.7/alphacore/
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.836531 alphacore-0.0.7/alphacore/.idea/
--rw-rw-rw-   0        0        0       50 2022-12-22 11:47:49.000000 alphacore-0.0.7/alphacore/.idea/.gitignore
--rw-rw-rw-   0        0        0      566 2022-12-22 11:47:48.000000 alphacore-0.0.7/alphacore/.idea/alphacore.iml
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.836531 alphacore-0.0.7/alphacore/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      174 2022-12-22 11:47:48.000000 alphacore-0.0.7/alphacore/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      188 2022-12-22 11:47:48.000000 alphacore-0.0.7/alphacore/.idea/misc.xml
--rw-rw-rw-   0        0        0      277 2022-12-22 11:47:48.000000 alphacore-0.0.7/alphacore/.idea/modules.xml
--rw-rw-rw-   0        0        0      188 2022-12-22 11:47:48.000000 alphacore-0.0.7/alphacore/.idea/vcs.xml
--rw-rw-rw-   0        0        0     9114 2022-12-23 02:13:43.000000 alphacore-0.0.7/alphacore/.idea/workspace.xml
--rw-rw-rw-   0        0        0      515 2023-01-05 10:12:27.000000 alphacore-0.0.7/alphacore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.836531 alphacore-0.0.7/alphacore/__pycache__/
--rw-rw-rw-   0        0        0    32531 2023-01-05 10:04:11.000000 alphacore-0.0.7/alphacore/__pycache__/distributions.cpython-39.pyc
--rw-rw-rw-   0        0        0    16381 2023-01-05 10:04:09.000000 alphacore-0.0.7/alphacore/__pycache__/fit_distribution.cpython-39.pyc
--rw-rw-rw-   0        0        0   110923 2023-01-05 10:04:09.000000 alphacore-0.0.7/alphacore/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0    43411 2023-01-05 10:04:05.000000 alphacore-0.0.7/alphacore/distributions.py
--rw-rw-rw-   0        0        0    25607 2023-01-05 10:04:05.000000 alphacore-0.0.7/alphacore/fit_distribution.py
--rw-rw-rw-   0        0        0     3308 2023-01-05 10:12:27.000000 alphacore-0.0.7/alphacore/fit_linear.py
--rw-rw-rw-   0        0        0      756 2023-01-05 10:06:02.000000 alphacore-0.0.7/alphacore/sandbox.py
--rw-rw-rw-   0        0        0        0 2023-01-05 10:12:27.000000 alphacore-0.0.7/alphacore/sandbox2.py
--rw-rw-rw-   0        0        0   193108 2023-01-05 10:18:21.000000 alphacore-0.0.7/alphacore/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-05 10:41:36.805276 alphacore-0.0.7/alphacore.egg-info/
--rw-rw-rw-   0        0        0      578 2023-01-05 10:41:35.000000 alphacore-0.0.7/alphacore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-01-05 10:41:36.000000 alphacore-0.0.7/alphacore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 10:41:35.000000 alphacore-0.0.7/alphacore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-01-05 10:41:35.000000 alphacore-0.0.7/alphacore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-05 10:41:35.000000 alphacore-0.0.7/alphacore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       65 2023-01-03 09:42:11.000000 alphacore-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-05 10:41:36.852152 alphacore-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-01-05 10:20:56.000000 alphacore-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:38:25.279810 alphacore-0.0.8/
+-rw-rw-rw-   0        0        0     7817 2020-04-27 03:35:53.000000 alphacore-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       90 2022-11-29 01:51:08.000000 alphacore-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      638 2023-07-08 05:38:25.264160 alphacore-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2022-11-29 01:28:57.000000 alphacore-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 05:38:25.248536 alphacore-0.0.8/alphacore/
+-rw-rw-rw-   0        0        0      515 2023-07-08 05:28:10.000000 alphacore-0.0.8/alphacore/__init__.py
+-rw-rw-rw-   0        0        0    43421 2023-01-13 11:40:46.000000 alphacore-0.0.8/alphacore/distributions.py
+-rw-rw-rw-   0        0        0    25627 2023-01-13 11:41:27.000000 alphacore-0.0.8/alphacore/fit_distribution.py
+-rw-rw-rw-   0        0        0     3308 2023-01-13 11:39:37.000000 alphacore-0.0.8/alphacore/fit_linear.py
+-rw-rw-rw-   0        0        0   193108 2023-01-05 10:43:57.000000 alphacore-0.0.8/alphacore/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:38:25.264160 alphacore-0.0.8/alphacore.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-07-08 05:38:25.000000 alphacore-0.0.8/alphacore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-08 05:38:25.000000 alphacore-0.0.8/alphacore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 05:38:25.000000 alphacore-0.0.8/alphacore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-08 05:38:25.000000 alphacore-0.0.8/alphacore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 05:38:25.000000 alphacore-0.0.8/alphacore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 05:38:25.279810 alphacore-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-07-08 05:37:26.000000 alphacore-0.0.8/setup.py
```

### Comparing `alphacore-0.0.7/LICENSE` & `alphacore-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alphacore-0.0.7/PKG-INFO` & `alphacore-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: alphacore
-Version: 0.0.7
+Version: 0.0.8
 Summary: Core statistical functions for alpha
 Home-page: https://pypi.org/project/alphacore/
 Author: Matthew Reid
 Author-email: alpha.reliability@gmail.com
 License: LGPLv3
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Core statistical functions for alpha
```

### Comparing `alphacore-0.0.7/alphacore/__init__.py` & `alphacore-0.0.8/alphacore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
 from alphacore import fit_linear
 from alphacore import fit_distribution
 from alphacore import utils
 from datetime import date
 
 __title__ = 'alphacore'
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __description__ = 'Core statistical functions for alpha'
 __url__ = 'https://pypi.org/project/alphacore/'
 __author__ = 'Matthew Reid'
 __author_email__ = 'alpha.reliability@gmail.com'
 __license__ = 'LGPLv3'
 __copyright__ = "Copyright 2022-{}, Matthew Reid".format(date.today().year)
```

### Comparing `alphacore-0.0.7/alphacore/distributions.py` & `alphacore-0.0.8/alphacore/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import scipy.stats as ss
-from utils import (
+from alphacore.utils import (
     round_to_decimals,
     distributions_input_checking,
     unpack_single_arrays,
     zeroise_below_gamma,
     extract_CI,
     colorprint,
 )
```

### Comparing `alphacore-0.0.7/alphacore/fit_distribution.py` & `alphacore-0.0.8/alphacore/fit_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from utils import (
+from alphacore.utils import (
     fitters_input_checking,
     LS_optimization,
     MLE_optimization,
     plotting_positions,
     anderson_darling,
     colorprint,
 )
-from distributions import Weibull_Distribution, Normal_Distribution
+from alphacore.distributions import Weibull_Distribution, Normal_Distribution
 from autograd.differential_operators import hessian
 import scipy.stats as ss
 import numpy as np
 from numpy.linalg import LinAlgError
 import autograd.numpy as anp
 from autograd.scipy.special import erf
```

### Comparing `alphacore-0.0.7/alphacore/fit_linear.py` & `alphacore-0.0.8/alphacore/fit_linear.py`

 * *Files identical despite different names*

### Comparing `alphacore-0.0.7/alphacore/utils.py` & `alphacore-0.0.8/alphacore/utils.py`

 * *Files identical despite different names*

### Comparing `alphacore-0.0.7/alphacore.egg-info/PKG-INFO` & `alphacore-0.0.8/alphacore.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: alphacore
-Version: 0.0.7
+Version: 0.0.8
 Summary: Core statistical functions for alpha
 Home-page: https://pypi.org/project/alphacore/
 Author: Matthew Reid
 Author-email: alpha.reliability@gmail.com
 License: LGPLv3
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Core statistical functions for alpha
```

### Comparing `alphacore-0.0.7/setup.py` & `alphacore-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name="alphacore",
-    version="0.0.7",
+    version="0.0.8",
     description="Core statistical functions for alpha",
     author="Matthew Reid",
     author_email="alpha.reliability@gmail.com",
     license="LGPLv3",
     url="https://pypi.org/project/alphacore/",
+    long_description="Core statistical functions for alpha",
+    long_description_content_type="text/x-rst",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Programming Language :: Python :: 3",
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     ],
     install_requires=[
-        "scipy>=1.7.0",
-        "numpy>=1.19.2",
-        "autograd>=1.3",
+        "scipy>=1.10.1",
+        "numpy>=1.24.2",
+        "autograd>=1.5",
         "autograd-gamma>=0.5.0"
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*"]
     ),
 )
```

