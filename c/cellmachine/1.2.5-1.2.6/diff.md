# Comparing `tmp/cellmachine-1.2.5.tar.gz` & `tmp/cellmachine-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-1.2.5.tar", max compression
+gzip compressed data, was "cellmachine-1.2.6.tar", max compression
```

## Comparing `cellmachine-1.2.5.tar` & `cellmachine-1.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35149 2023-07-08 08:13:35.228448 cellmachine-1.2.5/LICENSE
--rw-r--r--   0        0        0       60 2023-07-08 08:13:35.228448 cellmachine-1.2.5/README.md
--rw-r--r--   0        0        0      340 2023-07-08 08:13:35.228448 cellmachine-1.2.5/pyproject.toml
--rw-r--r--   0        0        0       84 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/__init__.py
--rw-r--r--   0        0        0      271 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__init__.py
--rw-r--r--   0        0        0      476 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      890 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
--rw-r--r--   0        0        0      885 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
--rw-r--r--   0        0        0     1229 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
--rw-r--r--   0        0        0      917 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
--rw-r--r--   0        0        0      561 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
--rw-r--r--   0        0        0      766 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
--rw-r--r--   0        0        0      719 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/ccw.py
--rw-r--r--   0        0        0     2091 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/cell.py
--rw-r--r--   0        0        0      536 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/cw.py
--rw-r--r--   0        0        0      341 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/enemy.py
--rw-r--r--   0        0        0     1266 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/generator.py
--rw-r--r--   0        0        0      294 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/immobile.py
--rw-r--r--   0        0        0      456 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/mover.py
--rw-r--r--   0        0        0      155 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/push.py
--rw-r--r--   0        0        0      354 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/slide.py
--rw-r--r--   0        0        0      277 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/cells/trash.py
--rw-r--r--   0        0        0     3656 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/level.py
--rw-r--r--   0        0        0      417 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/__init__.py
--rw-r--r--   0        0        0      528 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2145 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
--rw-r--r--   0        0        0     2371 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
--rw-r--r--   0        0        0     2481 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/v1.py
--rw-r--r--   0        0        0     4905 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/v2.py
--rw-r--r--   0        0        0     6129 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/levelstring/v3.py
--rw-r--r--   0        0        0     6148 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/textures/.DS_Store
--rwxr-xr-x   0        0        0      165 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/textures/0.png
--rwxr-xr-x   0        0        0      127 2023-07-08 08:13:35.228448 cellmachine-1.2.5/src/cellmachine/textures/BGDefault.png
--rwxr-xr-x   0        0        0      494 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/ccw.png
--rwxr-xr-x   0        0        0      437 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/cw.png
--rwxr-xr-x   0        0        0      429 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/enemy.png
--rwxr-xr-x   0        0        0      522 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/generator.png
--rwxr-xr-x   0        0        0      171 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/immobile.png
--rwxr-xr-x   0        0        0      467 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/mover.png
--rwxr-xr-x   0        0        0      527 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/push.png
--rwxr-xr-x   0        0        0      481 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/slide.png
--rwxr-xr-x   0        0        0      469 2023-07-08 08:13:35.232448 cellmachine-1.2.5/src/cellmachine/textures/trash.png
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 08:18:49.253276 cellmachine-1.2.6/LICENSE
+-rw-r--r--   0        0        0       60 2023-07-08 08:18:49.253276 cellmachine-1.2.6/README.md
+-rw-r--r--   0        0        0      340 2023-07-08 08:18:49.253276 cellmachine-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__init__.py
+-rw-r--r--   0        0        0      476 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      890 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
+-rw-r--r--   0        0        0     1229 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
+-rw-r--r--   0        0        0      917 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
+-rw-r--r--   0        0        0      561 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
+-rw-r--r--   0        0        0      766 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
+-rw-r--r--   0        0        0      719 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/ccw.py
+-rw-r--r--   0        0        0     2081 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/cell.py
+-rw-r--r--   0        0        0      536 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/cw.py
+-rw-r--r--   0        0        0      341 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/enemy.py
+-rw-r--r--   0        0        0     1266 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/generator.py
+-rw-r--r--   0        0        0      294 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/immobile.py
+-rw-r--r--   0        0        0      456 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/mover.py
+-rw-r--r--   0        0        0      155 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/push.py
+-rw-r--r--   0        0        0      354 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/slide.py
+-rw-r--r--   0        0        0      277 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/trash.py
+-rw-r--r--   0        0        0     3656 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/level.py
+-rw-r--r--   0        0        0      417 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__init__.py
+-rw-r--r--   0        0        0      528 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2145 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
+-rw-r--r--   0        0        0     2371 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
+-rw-r--r--   0        0        0     2481 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v1.py
+-rw-r--r--   0        0        0     4905 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v2.py
+-rw-r--r--   0        0        0     6129 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v3.py
+-rw-r--r--   0        0        0     6148 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/.DS_Store
+-rwxr-xr-x   0        0        0      165 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/0.png
+-rwxr-xr-x   0        0        0      127 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/BGDefault.png
+-rwxr-xr-x   0        0        0      494 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/ccw.png
+-rwxr-xr-x   0        0        0      437 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/cw.png
+-rwxr-xr-x   0        0        0      429 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/enemy.png
+-rwxr-xr-x   0        0        0      522 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/generator.png
+-rwxr-xr-x   0        0        0      171 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/immobile.png
+-rwxr-xr-x   0        0        0      467 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/mover.png
+-rwxr-xr-x   0        0        0      527 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/push.png
+-rwxr-xr-x   0        0        0      481 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/slide.png
+-rwxr-xr-x   0        0        0      469 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/trash.png
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.2.6/PKG-INFO
```

### Comparing `cellmachine-1.2.5/LICENSE` & `cellmachine-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/push.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/push.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/ccw.py` & `cellmachine-1.2.6/src/cellmachine/cells/ccw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/cell.py` & `cellmachine-1.2.6/src/cellmachine/cells/cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 class Cell:
     def __init__(self, level, celltype, position, rotation=0):
         self.level    = level
         self.celltype = celltype
         self._rotation = rotation
 
-
-        self.position = position
+        self._position = position
+        if self.level is not None:
+            self.position = position
     
     @property
     def rotation(self):
         return self._rotation
     
     @rotation.setter
     def rotation(self, value: int):
@@ -17,20 +18,18 @@
     
     @property
     def position(self):
         return self._position
     
     @position.setter
     def position(self, value: tuple):
-        if self.level is not None:
-            if self._position in self.level.cells:
-                del self.level.cells[self._position]
+        if self._position in self.level.cells:
+            del self.level.cells[self._position]
         self._position = value
-        if self.level is not None:
-            self.level.cells[self._position] = self
+        self.level.cells[self._position] = self
 
     def push(self, direction, bias):
         """
         Returns
         -------
             - (bool) Can the cell move?
             - (bool) Does the previous cell, the one pushing this one, get deleted?
```

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/cw.py` & `cellmachine-1.2.6/src/cellmachine/cells/cw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/cells/generator.py` & `cellmachine-1.2.6/src/cellmachine/cells/generator.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/level.py` & `cellmachine-1.2.6/src/cellmachine/level.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc` & `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/v1.py` & `cellmachine-1.2.6/src/cellmachine/levelstring/v1.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/v2.py` & `cellmachine-1.2.6/src/cellmachine/levelstring/v2.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/levelstring/v3.py` & `cellmachine-1.2.6/src/cellmachine/levelstring/v3.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/textures/.DS_Store` & `cellmachine-1.2.6/src/cellmachine/textures/.DS_Store`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/textures/generator.png` & `cellmachine-1.2.6/src/cellmachine/textures/generator.png`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.5/src/cellmachine/textures/push.png` & `cellmachine-1.2.6/src/cellmachine/textures/push.png`

 * *Files identical despite different names*
