# Comparing `tmp/readmet-0.7.1.tar.gz` & `tmp/readmet-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmet-0.7.1.tar", last modified: Thu Mar 16 15:35:14 2023, max compression
+gzip compressed data, was "readmet-0.7.3.tar", last modified: Fri Jul  7 22:57:03 2023, max compression
```

## Comparing `readmet-0.7.1.tar` & `readmet-0.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-03-16 15:35:14.990831 readmet-0.7.1/
--rw-r--r--   0 druee     (1015) users      (100)    13827 2020-03-06 09:08:59.000000 readmet-0.7.1/LICENSE
--rw-r--r--   0 druee     (1015) users      (100)      680 2023-03-16 15:35:14.990831 readmet-0.7.1/PKG-INFO
--rw-rw-r--   0 druee     (1015) users      (100)      399 2023-01-03 23:36:08.000000 readmet-0.7.1/README.md
--rw-r--r--   0 druee     (1015) users      (100)      110 2022-07-20 20:26:46.000000 readmet-0.7.1/pyproject.toml
-drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-03-16 15:35:14.990831 readmet-0.7.1/readmet/
--rw-r--r--   0 druee     (1015) users      (100)      685 2023-01-03 16:25:03.000000 readmet-0.7.1/readmet/__init__.py
--rw-r--r--   0 druee     (1015) users      (100)      364 2023-03-16 15:31:22.000000 readmet-0.7.1/readmet/_version.py
--rw-r--r--   0 druee     (1015) users      (100)    19032 2023-01-17 16:07:31.000000 readmet-0.7.1/readmet/akterm.py
--rw-r--r--   0 druee     (1015) users      (100)    55357 2023-03-16 15:31:22.000000 readmet-0.7.1/readmet/dmna.py
--rw-r--r--   0 druee     (1015) users      (100)    18071 2023-01-03 16:48:52.000000 readmet-0.7.1/readmet/scintec1.py
--rw-r--r--   0 druee     (1015) users      (100)     9181 2023-01-03 16:25:03.000000 readmet-0.7.1/readmet/toa5.py
-drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-03-16 15:35:14.990831 readmet-0.7.1/readmet.egg-info/
--rw-r--r--   0 druee     (1015) users      (100)      680 2023-03-16 15:35:14.000000 readmet-0.7.1/readmet.egg-info/PKG-INFO
--rw-r--r--   0 druee     (1015) users      (100)      315 2023-03-16 15:35:14.000000 readmet-0.7.1/readmet.egg-info/SOURCES.txt
--rw-r--r--   0 druee     (1015) users      (100)        1 2023-03-16 15:35:14.000000 readmet-0.7.1/readmet.egg-info/dependency_links.txt
--rw-r--r--   0 druee     (1015) users      (100)       13 2023-03-16 15:35:14.000000 readmet-0.7.1/readmet.egg-info/requires.txt
--rw-r--r--   0 druee     (1015) users      (100)        8 2023-03-16 15:35:14.000000 readmet-0.7.1/readmet.egg-info/top_level.txt
--rw-r--r--   0 druee     (1015) users      (100)      167 2023-03-16 15:35:14.990831 readmet-0.7.1/setup.cfg
--rw-r--r--   0 druee     (1015) users      (100)      659 2023-01-03 23:32:35.000000 readmet-0.7.1/setup.py
+drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-07-07 22:57:03.506307 readmet-0.7.3/
+-rw-r--r--   0 druee     (1015) users      (100)    13827 2020-03-06 09:08:59.000000 readmet-0.7.3/LICENSE
+-rw-r--r--   0 druee     (1015) users      (100)      680 2023-07-07 22:57:03.506307 readmet-0.7.3/PKG-INFO
+-rw-rw-r--   0 druee     (1015) users      (100)      399 2023-01-03 23:36:08.000000 readmet-0.7.3/README.md
+-rw-r--r--   0 druee     (1015) users      (100)      110 2022-07-20 20:26:46.000000 readmet-0.7.3/pyproject.toml
+drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-07-07 22:57:03.502308 readmet-0.7.3/readmet/
+-rw-r--r--   0 druee     (1015) users      (100)      685 2023-01-03 16:25:03.000000 readmet-0.7.3/readmet/__init__.py
+-rw-r--r--   0 druee     (1015) users      (100)      364 2023-07-07 22:53:21.000000 readmet-0.7.3/readmet/_version.py
+-rw-r--r--   0 druee     (1015) users      (100)    19032 2023-01-17 16:07:31.000000 readmet-0.7.3/readmet/akterm.py
+-rw-r--r--   0 druee     (1015) users      (100)    55590 2023-03-29 21:16:58.000000 readmet-0.7.3/readmet/dmna.py
+-rw-r--r--   0 druee     (1015) users      (100)    18071 2023-01-03 16:48:52.000000 readmet-0.7.3/readmet/scintec1.py
+-rw-r--r--   0 druee     (1015) users      (100)     9392 2023-07-07 14:53:57.000000 readmet-0.7.3/readmet/toa5.py
+drwxr-xr-x   0 druee     (1015) users      (100)        0 2023-07-07 22:57:03.506307 readmet-0.7.3/readmet.egg-info/
+-rw-r--r--   0 druee     (1015) users      (100)      680 2023-07-07 22:57:03.000000 readmet-0.7.3/readmet.egg-info/PKG-INFO
+-rw-r--r--   0 druee     (1015) users      (100)      315 2023-07-07 22:57:03.000000 readmet-0.7.3/readmet.egg-info/SOURCES.txt
+-rw-r--r--   0 druee     (1015) users      (100)        1 2023-07-07 22:57:03.000000 readmet-0.7.3/readmet.egg-info/dependency_links.txt
+-rw-r--r--   0 druee     (1015) users      (100)       13 2023-07-07 22:57:03.000000 readmet-0.7.3/readmet.egg-info/requires.txt
+-rw-r--r--   0 druee     (1015) users      (100)        8 2023-07-07 22:57:03.000000 readmet-0.7.3/readmet.egg-info/top_level.txt
+-rw-r--r--   0 druee     (1015) users      (100)      167 2023-07-07 22:57:03.506307 readmet-0.7.3/setup.cfg
+-rw-r--r--   0 druee     (1015) users      (100)      659 2023-01-03 23:32:35.000000 readmet-0.7.3/setup.py
```

### Comparing `readmet-0.7.1/LICENSE` & `readmet-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readmet-0.7.1/PKG-INFO` & `readmet-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmet
-Version: 0.7.1
+Version: 0.7.3
 Summary: Python library for reading and writing rare formats used in Meteorology.
 Home-page: 
 Author: Clemens Drüe
 Author-email: druee@uni-trier.de
 License: EUPL-1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readmet-0.7.1/readmet/__init__.py` & `readmet-0.7.3/readmet/__init__.py`

 * *Files identical despite different names*

### Comparing `readmet-0.7.1/readmet/akterm.py` & `readmet-0.7.3/readmet/akterm.py`

 * *Files identical despite different names*

### Comparing `readmet-0.7.1/readmet/dmna.py` & `readmet-0.7.3/readmet/dmna.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,26 @@
         res = arr[np.newaxis, :, :]
     elif dims == 3:
         res = arr
     else:
         raise ValueError('illegal number of dimensions: %d', dims)
     return res
 
-
+def _count_digits(arr: np.ndarray) -> int:
+    # this code produces Warnings for 0.0 in arr
+    # np.max(np.ceil(np.log10(np.abs(arr))))
+    #
+    # this code counts actual digits
+    bb = arr.copy()
+    bb[~np.isfinite(bb)] = 0
+
+    lx = len(str(int(np.max(bb))))
+    ln = len(str(int(np.min(bb))))
+    res = max(lx, ln)
+    return res
 #
 #
 #
 # ------------------------------------------------------------------------
 #
 
 
@@ -589,29 +600,27 @@
                 elif self.filetype == 'timeseries' and '.' in var:
                     # prefer exp form for source strengths in timeseries
                     self._variable_type[var] = "e"
                 elif np.all((self.data[var] - np.floor(self.data[var]))
                             == 0):
                     self._variable_type[var] = "d"
                 else:
-                    digits = np.max(np.ceil(np.log10(np.abs(
-                        self.data[var]))))
+                    digits = _count_digits(self.data[var])
                     if digits > 7 or digits < 0:
                         self._variable_type[var] = "e"
                     else:
                         self._variable_type[var] = "f"
             #
             # determine variable format
             #
             if self._variable_type[var] == "d":
-                digits = np.max(np.ceil(np.log10(np.abs(self.data[var]))))
-                digits = max(digits, 4)
+                digits = max(_count_digits(self.data[var]), 4)
                 fmt = '%%%dhd' % digits
             elif self._variable_type[var] == "f":
-                digits = np.max(np.ceil(np.log10(np.abs(self.data[var]))))
+                digits = _count_digits(self.data[var])
                 if np.all(self.data[var] - np.floor(self.data[var]) == 0):
                     precision = 0
                     digits = max(digits, 5)
                 else:
                     precision = 1
                     digits = max(digits + 2, 7)
                 fmt = '%%%d.%df' % (digits, precision)
@@ -993,15 +1002,15 @@
         if len(delta) > 1:
             raise ValueError('horizontal grid spacing not unique')
         if dims == 2 and 'sk' in axes.keys():
             dims = 3
             sk = axes['sk']
         elif 'z' in axes.keys():
             dims = 3
-            sk = axes['Z']
+            sk = axes['z']
         else:
             sk = None
         #
         #  look for conflicts
         #
         if self._att1('dims', None) not in [None, dims]:
             raise ValueError('dims is already set to %d' %
@@ -1414,18 +1423,18 @@
                    If missing or `None`, all axes are returned.
 
         :return: `dict` with axis names as keys, containing\
                  list(s) of positions as values.
         """
         axes = self._att1('axes', None)
         dims = self._att1('dims', -1)
-        print('axes : %s' % format(axes))
+        logging.debug('axes : %s' % format(axes))
         if axes == 'ti' or dims == 1:
             return self.data['te'].values
-        elif axes in ['xy', 'xyz', 'xyzs']:
+        elif axes in ['xy', 'xyz', 'xyzs', None]:
             return self._get_axes(ax)
 
     # ----------------------------------------------------------------------
     #
     # calculate  in Gauss-Krueger coordinates
     #
     def grid(self, what=None):
```

### Comparing `readmet-0.7.1/readmet/scintec1.py` & `readmet-0.7.3/readmet/scintec1.py`

 * *Files identical despite different names*

### Comparing `readmet-0.7.1/readmet/toa5.py` & `readmet-0.7.3/readmet/toa5.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,20 @@
     :returns: data from the file given
     :rtype: ``pandas.DataFrame``
     '''
     header = get_header(filename)
     data = pd.read_csv(filename, header=None, skiprows=4, sep=',',
                        quotechar='"', na_values=['NAN', '+INF', '-INF'])
     data.columns = header['column_names']
-    data.index = pd.to_datetime(data['TIMESTAMP'])
+    # if there are fractional seconds, make all timestamps have them
+    if any("." in x for x in data['TIMESTAMP']):
+        fmt = '%Y-%m-%d %H:%M:%S.%f'
+    else:
+        fmt = '%Y-%m-%d %H:%M:%S'
+    data.index = pd.to_datetime(data['TIMESTAMP'], format=fmt)
     return data
 
 
 def verify_header(header):
     H = Header()
     for f in H.keys():
         if f not in header.keys():
```

### Comparing `readmet-0.7.1/readmet.egg-info/PKG-INFO` & `readmet-0.7.3/readmet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmet
-Version: 0.7.1
+Version: 0.7.3
 Summary: Python library for reading and writing rare formats used in Meteorology.
 Home-page: 
 Author: Clemens Drüe
 Author-email: druee@uni-trier.de
 License: EUPL-1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `readmet-0.7.1/setup.py` & `readmet-0.7.3/setup.py`

 * *Files identical despite different names*

