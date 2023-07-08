# Comparing `tmp/cellmachine-1.2.6.tar.gz` & `tmp/cellmachine-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-1.2.6.tar", max compression
+gzip compressed data, was "cellmachine-1.2.7.tar", max compression
```

## Comparing `cellmachine-1.2.6.tar` & `cellmachine-1.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35149 2023-07-08 08:18:49.253276 cellmachine-1.2.6/LICENSE
--rw-r--r--   0        0        0       60 2023-07-08 08:18:49.253276 cellmachine-1.2.6/README.md
--rw-r--r--   0        0        0      340 2023-07-08 08:18:49.253276 cellmachine-1.2.6/pyproject.toml
--rw-r--r--   0        0        0       84 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/__init__.py
--rw-r--r--   0        0        0      271 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__init__.py
--rw-r--r--   0        0        0      476 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      890 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
--rw-r--r--   0        0        0      885 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
--rw-r--r--   0        0        0     1229 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
--rw-r--r--   0        0        0      917 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
--rw-r--r--   0        0        0      561 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
--rw-r--r--   0        0        0      766 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
--rw-r--r--   0        0        0      719 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/ccw.py
--rw-r--r--   0        0        0     2081 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/cell.py
--rw-r--r--   0        0        0      536 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/cw.py
--rw-r--r--   0        0        0      341 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/enemy.py
--rw-r--r--   0        0        0     1266 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/generator.py
--rw-r--r--   0        0        0      294 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/immobile.py
--rw-r--r--   0        0        0      456 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/mover.py
--rw-r--r--   0        0        0      155 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/push.py
--rw-r--r--   0        0        0      354 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/slide.py
--rw-r--r--   0        0        0      277 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/cells/trash.py
--rw-r--r--   0        0        0     3656 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/level.py
--rw-r--r--   0        0        0      417 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__init__.py
--rw-r--r--   0        0        0      528 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2145 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
--rw-r--r--   0        0        0     2371 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
--rw-r--r--   0        0        0     2481 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v1.py
--rw-r--r--   0        0        0     4905 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v2.py
--rw-r--r--   0        0        0     6129 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/levelstring/v3.py
--rw-r--r--   0        0        0     6148 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/.DS_Store
--rwxr-xr-x   0        0        0      165 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/0.png
--rwxr-xr-x   0        0        0      127 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/BGDefault.png
--rwxr-xr-x   0        0        0      494 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/ccw.png
--rwxr-xr-x   0        0        0      437 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/cw.png
--rwxr-xr-x   0        0        0      429 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/enemy.png
--rwxr-xr-x   0        0        0      522 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/generator.png
--rwxr-xr-x   0        0        0      171 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/immobile.png
--rwxr-xr-x   0        0        0      467 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/mover.png
--rwxr-xr-x   0        0        0      527 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/push.png
--rwxr-xr-x   0        0        0      481 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/slide.png
--rwxr-xr-x   0        0        0      469 2023-07-08 08:18:49.253276 cellmachine-1.2.6/src/cellmachine/textures/trash.png
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 08:24:06.124586 cellmachine-1.2.7/LICENSE
+-rw-r--r--   0        0        0       60 2023-07-08 08:24:06.124586 cellmachine-1.2.7/README.md
+-rw-r--r--   0        0        0      340 2023-07-08 08:24:06.124586 cellmachine-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__init__.py
+-rw-r--r--   0        0        0      476 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      890 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc
+-rw-r--r--   0        0        0     1229 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc
+-rw-r--r--   0        0        0      917 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc
+-rw-r--r--   0        0        0      561 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/push.cpython-310.pyc
+-rw-r--r--   0        0        0      766 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc
+-rw-r--r--   0        0        0      719 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/ccw.py
+-rw-r--r--   0        0        0     2199 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/cell.py
+-rw-r--r--   0        0        0      536 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/cw.py
+-rw-r--r--   0        0        0      341 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/enemy.py
+-rw-r--r--   0        0        0     1266 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/generator.py
+-rw-r--r--   0        0        0      294 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/immobile.py
+-rw-r--r--   0        0        0      456 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/mover.py
+-rw-r--r--   0        0        0      155 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/push.py
+-rw-r--r--   0        0        0      354 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/slide.py
+-rw-r--r--   0        0        0      277 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/cells/trash.py
+-rw-r--r--   0        0        0     3656 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/level.py
+-rw-r--r--   0        0        0      417 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/__init__.py
+-rw-r--r--   0        0        0      528 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2145 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc
+-rw-r--r--   0        0        0     2371 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc
+-rw-r--r--   0        0        0     2481 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/v1.py
+-rw-r--r--   0        0        0     4905 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/v2.py
+-rw-r--r--   0        0        0     6129 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/levelstring/v3.py
+-rw-r--r--   0        0        0     6148 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/.DS_Store
+-rwxr-xr-x   0        0        0      165 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/0.png
+-rwxr-xr-x   0        0        0      127 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/BGDefault.png
+-rwxr-xr-x   0        0        0      494 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/ccw.png
+-rwxr-xr-x   0        0        0      437 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/cw.png
+-rwxr-xr-x   0        0        0      429 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/enemy.png
+-rwxr-xr-x   0        0        0      522 2023-07-08 08:24:06.124586 cellmachine-1.2.7/src/cellmachine/textures/generator.png
+-rwxr-xr-x   0        0        0      171 2023-07-08 08:24:06.128586 cellmachine-1.2.7/src/cellmachine/textures/immobile.png
+-rwxr-xr-x   0        0        0      467 2023-07-08 08:24:06.128586 cellmachine-1.2.7/src/cellmachine/textures/mover.png
+-rwxr-xr-x   0        0        0      527 2023-07-08 08:24:06.128586 cellmachine-1.2.7/src/cellmachine/textures/push.png
+-rwxr-xr-x   0        0        0      481 2023-07-08 08:24:06.128586 cellmachine-1.2.7/src/cellmachine/textures/slide.png
+-rwxr-xr-x   0        0        0      469 2023-07-08 08:24:06.128586 cellmachine-1.2.7/src/cellmachine/textures/trash.png
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-1.2.7/PKG-INFO
```

### Comparing `cellmachine-1.2.6/LICENSE` & `cellmachine-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/ccw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/cell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/cw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/enemy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/immobile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/mover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/push.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/push.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/slide.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/cells/__pycache__/trash.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/ccw.py` & `cellmachine-1.2.7/src/cellmachine/cells/ccw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/cell.py` & `cellmachine-1.2.7/src/cellmachine/cells/cell.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         if self.level.outside_bounds(target):
             return False, False
         
         if bias < 1:
             return False, False
         
         future_cell = self.level.cells.get(target)
+        if future_cell == self:
+            print('\033[91m[!] \033[0mPushing self!')
+            return False, False
     
         if future_cell is None:
             self.position = target
             return True, False
 
         push_result = future_cell.push(direction, bias)
```

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/cw.py` & `cellmachine-1.2.7/src/cellmachine/cells/cw.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/cells/generator.py` & `cellmachine-1.2.7/src/cellmachine/cells/generator.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/level.py` & `cellmachine-1.2.7/src/cellmachine/level.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc` & `cellmachine-1.2.7/src/cellmachine/levelstring/__pycache__/v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/v1.py` & `cellmachine-1.2.7/src/cellmachine/levelstring/v1.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/v2.py` & `cellmachine-1.2.7/src/cellmachine/levelstring/v2.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/levelstring/v3.py` & `cellmachine-1.2.7/src/cellmachine/levelstring/v3.py`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/textures/.DS_Store` & `cellmachine-1.2.7/src/cellmachine/textures/.DS_Store`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/textures/generator.png` & `cellmachine-1.2.7/src/cellmachine/textures/generator.png`

 * *Files identical despite different names*

### Comparing `cellmachine-1.2.6/src/cellmachine/textures/push.png` & `cellmachine-1.2.7/src/cellmachine/textures/push.png`

 * *Files identical despite different names*

