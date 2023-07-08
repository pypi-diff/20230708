# Comparing `tmp/screwhashesset-0.11.tar.gz` & `tmp/screwhashesset-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwhashesset-0.11.tar", last modified: Tue Jul  4 06:12:50 2023, max compression
+gzip compressed data, was "screwhashesset-0.12.tar", last modified: Sat Jul  8 20:12:57 2023, max compression
```

## Comparing `screwhashesset-0.11.tar` & `screwhashesset-0.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.981678 screwhashesset-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-04 06:12:46.000000 screwhashesset-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      113 2023-07-04 06:12:43.000000 screwhashesset-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0    25580 2023-07-04 06:12:50.981678 screwhashesset-0.11/PKG-INFO
--rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.978686 screwhashesset-0.11/screwhashesset/
--rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.11/screwhashesset/README.MD
--rw-rw-rw-   0        0        0    12813 2023-07-04 06:02:27.000000 screwhashesset-0.11/screwhashesset/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.980681 screwhashesset-0.11/screwhashesset.egg-info/
--rw-rw-rw-   0        0        0    25580 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-04 06:12:50.982675 screwhashesset-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-07-04 06:12:50.000000 screwhashesset-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 20:12:57.226568 screwhashesset-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-08 20:12:52.000000 screwhashesset-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      113 2023-07-08 20:12:51.000000 screwhashesset-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    25580 2023-07-08 20:12:57.226568 screwhashesset-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 20:12:57.224573 screwhashesset-0.12/screwhashesset/
+-rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.12/screwhashesset/README.MD
+-rw-rw-rw-   0        0        0    12813 2023-07-08 20:11:40.000000 screwhashesset-0.12/screwhashesset/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 20:12:55.000000 screwhashesset-0.12/screwhashesset/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-08 20:12:55.000000 screwhashesset-0.12/screwhashesset/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-08 20:12:57.226568 screwhashesset-0.12/screwhashesset.egg-info/
+-rw-rw-rw-   0        0        0    25580 2023-07-08 20:12:56.000000 screwhashesset-0.12/screwhashesset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-08 20:12:56.000000 screwhashesset-0.12/screwhashesset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 20:12:56.000000 screwhashesset-0.12/screwhashesset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-08 20:12:56.000000 screwhashesset-0.12/screwhashesset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-08 20:12:57.227566 screwhashesset-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-07-08 20:12:55.000000 screwhashesset-0.12/setup.py
```

### Comparing `screwhashesset-0.11/LICENSE.rst` & `screwhashesset-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `screwhashesset-0.11/PKG-INFO` & `screwhashesset-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screwhashesset
-Version: 0.11
+Version: 0.12
 Summary: A set that handles all kinds of objects (hashable or not) and preserves the order of the elements
 Home-page: https://github.com/hansalemaos/screwhashesset
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: set,hash,collections
 Classifier: Development Status :: 4 - Beta
```

### Comparing `screwhashesset-0.11/README.md` & `screwhashesset-0.12/README.md`

 * *Files identical despite different names*

### Comparing `screwhashesset-0.11/screwhashesset/README.MD` & `screwhashesset-0.12/screwhashesset/README.MD`

 * *Files identical despite different names*

### Comparing `screwhashesset-0.11/screwhashesset/__init__.py` & `screwhashesset-0.12/screwhashesset/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Returns:
             ScrewHashesSet: A new ScrewHashesSet that is the union of this set and the other set or iterable.
         """
         tmpelements = deque([])
         for o in other:
             if not self._isin(o):
                 tmpelements.append(o)
-        return ScrewHashesSet(tmpelements + self.elements.copy())
+        return self.__class__(tmpelements + self.elements.copy())
 
     def _isin(self, o):
         """
         Check if an element is present in the ScrewHashesSet.
 
         Args:
             o: The element to check for presence.
@@ -116,32 +116,32 @@
         """
         Create a shallow copy of the ScrewHashesSet.
 
         Returns:
             ScrewHashesSet: A shallow copy of the ScrewHashesSet.
         """
         try:
-            return ScrewHashesSet(deepcopy(self.elements))
+            return self.__class__(deepcopy(self.elements))
         except Exception:
-            return ScrewHashesSet(copy(self.elements))
+            return self.__class__(copy(self.elements))
 
     def _convert_all_iters(self, *others):
         """
         Convert all input arguments to instances of ScrewHashesSet if they are not already one.
 
         Args:
             *others: Variable number of input arguments to convert.
 
         Returns:
             deque: A deque containing all the converted ScrewHashesSet instances.
         """
         allothers = deque([])
         for other in others:
-            if not isinstance(other, ScrewHashesSet):
-                other = ScrewHashesSet(other)
+            if not isinstance(other, self.__class__):
+                other = self.__class__(other)
             allothers.append(other)
         return allothers
 
     def difference(self, *others):
         """
         Return a new ScrewHashesSet with elements that are in the current set but not in any of the other sets.
```

### Comparing `screwhashesset-0.11/screwhashesset.egg-info/PKG-INFO` & `screwhashesset-0.12/screwhashesset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screwhashesset
-Version: 0.11
+Version: 0.12
 Summary: A set that handles all kinds of objects (hashable or not) and preserves the order of the elements
 Home-page: https://github.com/hansalemaos/screwhashesset
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: set,hash,collections
 Classifier: Development Status :: 4 - Beta
```

### Comparing `screwhashesset-0.11/setup.py` & `screwhashesset-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''A set that handles all kinds of objects (hashable or not) and preserves the order of the elements'''
 
 # Setting up
 setup(
     name="screwhashesset",
     version=VERSION,
     license='MIT',
```

