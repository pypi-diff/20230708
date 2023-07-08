# Comparing `tmp/voltcraft-1.3.0.tar.gz` & `tmp/voltcraft-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltcraft-1.3.0.tar", last modified: Wed Dec 29 10:25:49 2021, max compression
+gzip compressed data, was "voltcraft-1.3.1.tar", last modified: Sat Jul  8 08:52:35 2023, max compression
```

## Comparing `voltcraft-1.3.0.tar` & `voltcraft-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-12-29 10:25:49.208344 voltcraft-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-12-29 10:25:49.204343 voltcraft-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       95 2021-12-29 10:25:41.000000 voltcraft-1.3.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-12-29 10:25:49.204343 voltcraft-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      720 2021-12-29 10:25:41.000000 voltcraft-1.3.0/.github/workflows/build_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1091 2021-12-29 10:25:41.000000 voltcraft-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-12-29 10:25:41.000000 voltcraft-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2038 2021-12-29 10:25:49.208344 voltcraft-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1129 2021-12-29 10:25:41.000000 voltcraft-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      224 2021-12-29 10:25:41.000000 voltcraft-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      918 2021-12-29 10:25:49.208344 voltcraft-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-12-29 10:25:49.204343 voltcraft-1.3.0/voltcraft/
--rw-r--r--   0 runner    (1001) docker     (116)      181 2021-12-29 10:25:41.000000 voltcraft-1.3.0/voltcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     6598 2021-12-29 10:25:41.000000 voltcraft-1.3.0/voltcraft/pps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-12-29 10:25:49.208344 voltcraft-1.3.0/voltcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2038 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      339 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-12-29 10:25:49.000000 voltcraft-1.3.0/voltcraft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.github/workflows/build_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-08 08:52:25.000000 voltcraft-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-08 08:52:25.000000 voltcraft-1.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 08:52:25.000000 voltcraft-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:52:35.155655 voltcraft-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 08:52:25.000000 voltcraft-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-08 08:52:25.000000 voltcraft-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 08:52:35.155655 voltcraft-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/voltcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 08:52:25.000000 voltcraft-1.3.1/voltcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-08 08:52:25.000000 voltcraft-1.3.1/voltcraft/pps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:35.155655 voltcraft-1.3.1/voltcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 08:52:35.000000 voltcraft-1.3.1/voltcraft.egg-info/top_level.txt
```

### Comparing `voltcraft-1.3.0/.github/workflows/build_publish.yaml` & `voltcraft-1.3.1/.github/workflows/build_publish.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: build and publish voltcraft
 
 on: [push]
 
 jobs:
   build:
     name: build and publish voltcraft
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.8
-    - name: Install pep517
-      run: python -m pip install pep517 --user
+        python-version: 3.11
+    - name: Install build
+      run: python -m pip install build
     - name: Build a binary wheel and a source tarball
-      run: python -m pep517.build --source --binary --out-dir dist/ .
+      run: python -m build --sdist --wheel .
     - name: Publish distribution 📦 to PyPI
       if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.pypi_password }}
```

### Comparing `voltcraft-1.3.0/LICENSE.md` & `voltcraft-1.3.1/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `voltcraft-1.3.0/PKG-INFO` & `voltcraft-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.0
+Version: 1.3.1
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
+Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
-Download-URL: https://github.com/ap--/voltcraft
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
@@ -47,9 +46,7 @@
 
 Install via:
 ```console
 pip install voltcraft
 ```
 
 There's no documentation, but the module is tiny, so please just read the [voltcraft/pps.py](voltcraft/pps.py) :sparkling_heart:
-
-
```

### Comparing `voltcraft-1.3.0/README.md` & `voltcraft-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.0/setup.cfg` & `voltcraft-1.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [metadata]
 name = voltcraft
 url = https://github.com/ap--/voltcraft.git
 download_url = https://github.com/ap--/voltcraft
 license = MIT
-license_file = LICENSE.md
+license_files = 
+	LICENSE.md
 description = library for controlling Voltcraft PPS power supplies
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Poehlmann
 author_email = andreas@poehlmann.io
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -27,11 +28,16 @@
 packages = find:
 install_requires = 
 	pyserial
 
 [bdist_wheel]
 universal = 1
 
+[flake8]
+max-line-length = 88
+extend-ignore = 
+	E203,
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `voltcraft-1.3.0/voltcraft/pps.py` & `voltcraft-1.3.1/voltcraft/pps.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         sys.stdout.flush()
 
 
 # noinspection PyPep8Naming
 class PPS(object):
     def __init__(self, port="/dev/ttyUSB0", reset=True, prom=None, debug=False):
         """PPS(port, reset, prom)
-        
+
         Parameters
         ----------
         port : str
             default '/dev/ttyUSB0'
         reset : bool
             reset the voltage and current limit to 0, and disable the output
         prom : int
@@ -101,15 +101,15 @@
         self._debug("PPS <- %s<CR>\n" % cmd)
         self._serial.write((cmd + "\r").encode())
         b = []
         self._debug("PPS -> ")
         while True:
             b.append(self._serial.read(1))
             self._debug(b[-1].replace(b"\r", b"<CR>").decode())
-            if b[-1] == "":
+            if b[-1] in {b"", b"\x00"}:
                 raise serial.SerialTimeoutException()
             if b"".join(b[-3:]) == b"OK\r":
                 break
         self._debug("\n")
         return (b"".join(b[:-4])).decode()
 
     def limits(self):
```

### Comparing `voltcraft-1.3.0/voltcraft.egg-info/PKG-INFO` & `voltcraft-1.3.1/voltcraft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.0
+Version: 1.3.1
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
+Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
-Download-URL: https://github.com/ap--/voltcraft
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
@@ -47,9 +46,7 @@
 
 Install via:
 ```console
 pip install voltcraft
 ```
 
 There's no documentation, but the module is tiny, so please just read the [voltcraft/pps.py](voltcraft/pps.py) :sparkling_heart:
-
-
```

