# Comparing `tmp/PyTurboJPEG-1.7.1.tar.gz` & `tmp/PyTurboJPEG-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTurboJPEG-1.7.1.tar", last modified: Sat Apr 22 16:50:30 2023, max compression
+gzip compressed data, was "PyTurboJPEG-1.7.2.tar", last modified: Sat Jul  8 12:08:33 2023, max compression
```

## Comparing `PyTurboJPEG-1.7.1.tar` & `PyTurboJPEG-1.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-04-22 16:50:30.427491 PyTurboJPEG-1.7.1/
--rw-r--r--   0 lilohuang   (501) staff       (20)     1092 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/LICENSE
--rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-04-22 16:50:30.427231 PyTurboJPEG-1.7.1/PKG-INFO
-drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-04-22 16:50:30.426974 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/
--rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/PKG-INFO
--rw-r--r--   0 lilohuang   (501) staff       (20)      213 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/SOURCES.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)        1 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/dependency_links.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)        6 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/requires.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)       10 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/top_level.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)     6223 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/README.md
--rw-r--r--   0 lilohuang   (501) staff       (20)       38 2023-04-22 16:50:30.427539 PyTurboJPEG-1.7.1/setup.cfg
--rw-r--r--   0 lilohuang   (501) staff       (20)      543 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/setup.py
--rw-r--r--   0 lilohuang   (501) staff       (20)    37195 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/turbojpeg.py
+drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-07-08 12:08:33.302650 PyTurboJPEG-1.7.2/
+-rw-r--r--   0 lilohuang   (501) staff       (20)     1092 2023-07-08 12:08:23.000000 PyTurboJPEG-1.7.2/LICENSE
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-07-08 12:08:33.302496 PyTurboJPEG-1.7.2/PKG-INFO
+drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-07-08 12:08:33.302315 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-07-08 12:08:33.000000 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/PKG-INFO
+-rw-r--r--   0 lilohuang   (501) staff       (20)      213 2023-07-08 12:08:33.000000 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/SOURCES.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)        1 2023-07-08 12:08:33.000000 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/dependency_links.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)        6 2023-07-08 12:08:33.000000 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/requires.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)       10 2023-07-08 12:08:33.000000 PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/top_level.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6223 2023-07-08 12:08:23.000000 PyTurboJPEG-1.7.2/README.md
+-rw-r--r--   0 lilohuang   (501) staff       (20)       38 2023-07-08 12:08:33.302694 PyTurboJPEG-1.7.2/setup.cfg
+-rw-r--r--   0 lilohuang   (501) staff       (20)      543 2023-07-08 12:08:23.000000 PyTurboJPEG-1.7.2/setup.py
+-rw-r--r--   0 lilohuang   (501) staff       (20)    37210 2023-07-08 12:08:23.000000 PyTurboJPEG-1.7.2/turbojpeg.py
```

### Comparing `PyTurboJPEG-1.7.1/LICENSE` & `PyTurboJPEG-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTurboJPEG-1.7.1/PKG-INFO` & `PyTurboJPEG-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTurboJPEG
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.
 Home-page: https://github.com/lilohuang/PyTurboJPEG
 Author: Lilo Huang
 Author-email: kuso.cc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/PKG-INFO` & `PyTurboJPEG-1.7.2/PyTurboJPEG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTurboJPEG
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.
 Home-page: https://github.com/lilohuang/PyTurboJPEG
 Author: Lilo Huang
 Author-email: kuso.cc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTurboJPEG-1.7.1/README.md` & `PyTurboJPEG-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `PyTurboJPEG-1.7.1/setup.py` & `PyTurboJPEG-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 from setuptools import setup, find_packages
 setup(
     name='PyTurboJPEG',
-    version='1.7.1',
+    version='1.7.2',
     description='A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.',
     author='Lilo Huang',
     author_email='kuso.cc@gmail.com',
     url='https://github.com/lilohuang/PyTurboJPEG',
     license='MIT',
     install_requires=['numpy'],
     py_modules=['turbojpeg'],
```

### Comparing `PyTurboJPEG-1.7.1/turbojpeg.py` & `PyTurboJPEG-1.7.2/turbojpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 __author__ = 'Lilo Huang <kuso.cc@gmail.com>'
-__version__ = '1.7.1'
+__version__ = '1.7.2'
 
 from ctypes import *
 from ctypes.util import find_library
 import platform
 import numpy as np
 import math
 import warnings
@@ -89,14 +89,15 @@
 # see details in https://github.com/libjpeg-turbo/libjpeg-turbo/blob/master/turbojpeg.h
 TJSAMP_444 = 0
 TJSAMP_422 = 1
 TJSAMP_420 = 2
 TJSAMP_GRAY = 3
 TJSAMP_440 = 4
 TJSAMP_411 = 5
+TJSAMP_441 = 6
 
 # transform operations
 # see details in https://github.com/libjpeg-turbo/libjpeg-turbo/blob/master/turbojpeg.h
 TJXOP_NONE = 0
 TJXOP_HFLIP = 1
 TJXOP_VFLIP = 2
 TJXOP_TRANSPOSE = 3
```

