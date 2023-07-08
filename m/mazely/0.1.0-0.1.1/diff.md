# Comparing `tmp/mazely-0.1.0.tar.gz` & `tmp/mazely-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazely-0.1.0.tar", last modified: Thu Jul  6 14:32:55 2023, max compression
+gzip compressed data, was "mazely-0.1.1.tar", last modified: Sat Jul  8 10:10:25 2023, max compression
```

## Comparing `mazely-0.1.0.tar` & `mazely-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 14:32:55.007800 mazely-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-21 09:11:43.000000 mazely-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3656 2023-07-06 14:32:55.007800 mazely-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2852 2023-07-06 14:28:44.000000 mazely-0.1.0/README.md
--rw-rw-rw-   0        0        0       50 2023-07-06 11:43:41.000000 mazely-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-07-03 09:38:28.000000 mazely-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      962 2023-07-06 14:32:55.009783 mazely-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-07-06 11:43:41.000000 mazely-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:32:54.963958 mazely-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 14:32:54.981569 mazely-0.1.0/src/mazely/
--rw-rw-rw-   0        0        0      189 2023-07-06 14:18:01.000000 mazely-0.1.0/src/mazely/__about__.py
--rw-rw-rw-   0        0        0      160 2023-07-06 11:43:41.000000 mazely-0.1.0/src/mazely/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:32:55.007800 mazely-0.1.0/src/mazely/algorithms/
--rw-rw-rw-   0        0        0      180 2023-07-03 03:29:15.000000 mazely-0.1.0/src/mazely/algorithms/__init__.py
--rw-rw-rw-   0        0        0     2806 2023-07-06 14:22:49.000000 mazely-0.1.0/src/mazely/algorithms/maze_generator.py
--rw-rw-rw-   0        0        0      812 2023-07-03 07:22:25.000000 mazely-0.1.0/src/mazely/algorithms/maze_solver.py
--rw-rw-rw-   0        0        0     2351 2023-07-06 11:43:41.000000 mazely-0.1.0/src/mazely/algorithms/recursive_backtracking.py
--rw-rw-rw-   0        0        0     2546 2023-07-06 11:43:41.000000 mazely-0.1.0/src/mazely/algorithms/shortest_path.py
--rw-rw-rw-   0        0        0     7367 2023-07-06 11:43:41.000000 mazely-0.1.0/src/mazely/maze.py
--rw-rw-rw-   0        0        0     8466 2023-07-06 11:43:41.000000 mazely-0.1.0/src/mazely/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:32:55.000657 mazely-0.1.0/src/mazely.egg-info/
--rw-rw-rw-   0        0        0     3656 2023-07-06 14:32:54.000000 mazely-0.1.0/src/mazely.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-07-06 14:32:54.000000 mazely-0.1.0/src/mazely.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 14:32:54.000000 mazely-0.1.0/src/mazely.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-06 14:32:54.000000 mazely-0.1.0/src/mazely.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 14:32:54.000000 mazely-0.1.0/src/mazely.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.436617 mazely-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-21 09:11:43.000000 mazely-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3684 2023-07-08 10:10:25.437618 mazely-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2858 2023-07-08 09:33:51.000000 mazely-0.1.1/README.md
+-rw-rw-rw-   0        0        0       50 2023-07-08 09:33:50.000000 mazely-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-07-03 09:38:28.000000 mazely-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0     1036 2023-07-08 10:10:25.438617 mazely-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-07-08 09:33:50.000000 mazely-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.404159 mazely-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.415212 mazely-0.1.1/src/mazely/
+-rw-rw-rw-   0        0        0      189 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/__about__.py
+-rw-rw-rw-   0        0        0      160 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.436617 mazely-0.1.1/src/mazely/algorithms/
+-rw-rw-rw-   0        0        0      180 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2806 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/maze_generator.py
+-rw-rw-rw-   0        0        0      812 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/maze_solver.py
+-rw-rw-rw-   0        0        0     2351 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/recursive_backtracking.py
+-rw-rw-rw-   0        0        0     2546 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/shortest_path.py
+-rw-rw-rw-   0        0        0     7367 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/maze.py
+-rw-rw-rw-   0        0        0     8466 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.432618 mazely-0.1.1/src/mazely.egg-info/
+-rw-rw-rw-   0        0        0     3684 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/top_level.txt
```

### Comparing `mazely-0.1.0/LICENSE` & `mazely-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/PKG-INFO` & `mazely-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazely
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implementation of maze-related algorithms
 Author: Kenneth C.
 License: MIT
 Project-URL: Documentation, https://mazely.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Munckenh/mazely
 Keywords: mazely,maze,algorithms
 Classifier: Development Status :: 1 - Planning
@@ -13,14 +13,15 @@
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
 </p>
 
 # mazely
@@ -41,15 +42,15 @@
 Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
 
 ### Load and display a maze
 
 Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2015apec.maze")
 utils = Utilities()
 utils.show_grid(maze.grid)
 ```
 
 <p align="center">
@@ -57,15 +58,15 @@
 </p>
 
 ### Solve a maze and display its solution
 
 A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2019japan.maze")
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
@@ -73,15 +74,15 @@
 </p>
 
 ### Generate a maze and display its solution
 
 To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(32, 32)
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
```

### Comparing `mazely-0.1.0/README.md` & `mazely-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
 
 ### Load and display a maze
 
 Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2015apec.maze")
 utils = Utilities()
 utils.show_grid(maze.grid)
 ```
 
 <p align="center">
@@ -36,15 +36,15 @@
 </p>
 
 ### Solve a maze and display its solution
 
 A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2019japan.maze")
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
@@ -52,15 +52,15 @@
 </p>
 
 ### Generate a maze and display its solution
 
 To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(32, 32)
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
```

### Comparing `mazely-0.1.0/setup.cfg` & `mazely-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 617a 656c 790d 0a76 6572 7369   = mazely..versi
-00000020: 6f6e 203d 2030 2e31 2e30 0d0a 6175 7468  on = 0.1.0..auth
+00000020: 6f6e 203d 2030 2e31 2e31 0d0a 6175 7468  on = 0.1.1..auth
 00000030: 6f72 203d 204b 656e 6e65 7468 2043 2e0d  or = Kenneth C..
 00000040: 0a64 6573 6372 6970 7469 6f6e 203d 2049  .description = I
 00000050: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
 00000060: 206d 617a 652d 7265 6c61 7465 6420 616c   maze-related al
 00000070: 676f 7269 7468 6d73 0d0a 6c6f 6e67 5f64  gorithms..long_d
 00000080: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000090: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
@@ -51,11 +51,15 @@
 00000320: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
 00000330: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
 00000340: 310d 0a69 6e73 7461 6c6c 5f72 6571 7569  1..install_requi
 00000350: 7265 7320 3d20 6669 6c65 3a20 7265 7175  res = file: requ
 00000360: 6972 656d 656e 7473 2e74 7874 0d0a 0d0a  irements.txt....
 00000370: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
 00000380: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000390: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-000003a0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000003b0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000003c0: 0d0a                                     ..
+00000390: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
+000003a0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+000003b0: 0d0a 646f 6373 203d 200d 0a09 7370 6869  ..docs = ...sphi
+000003c0: 6e78 3e3d 362e 302c 3c38 2e30 0d0a 0966  nx>=6.0,<8.0...f
+000003d0: 7572 6f3d 3d32 3032 332e 352e 3230 0d0a  uro==2023.5.20..
+000003e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000003f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000400: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `mazely-0.1.0/src/mazely/algorithms/maze_generator.py` & `mazely-0.1.1/src/mazely/algorithms/maze_generator.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely/algorithms/maze_solver.py` & `mazely-0.1.1/src/mazely/algorithms/maze_solver.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely/algorithms/recursive_backtracking.py` & `mazely-0.1.1/src/mazely/algorithms/recursive_backtracking.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely/algorithms/shortest_path.py` & `mazely-0.1.1/src/mazely/algorithms/shortest_path.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely/maze.py` & `mazely-0.1.1/src/mazely/maze.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely/utilities.py` & `mazely-0.1.1/src/mazely/utilities.py`

 * *Files identical despite different names*

### Comparing `mazely-0.1.0/src/mazely.egg-info/PKG-INFO` & `mazely-0.1.1/src/mazely.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazely
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implementation of maze-related algorithms
 Author: Kenneth C.
 License: MIT
 Project-URL: Documentation, https://mazely.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Munckenh/mazely
 Keywords: mazely,maze,algorithms
 Classifier: Development Status :: 1 - Planning
@@ -13,14 +13,15 @@
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
 </p>
 
 # mazely
@@ -41,15 +42,15 @@
 Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
 
 ### Load and display a maze
 
 Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2015apec.maze")
 utils = Utilities()
 utils.show_grid(maze.grid)
 ```
 
 <p align="center">
@@ -57,15 +58,15 @@
 </p>
 
 ### Solve a maze and display its solution
 
 A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(path="resources/2019japan.maze")
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
@@ -73,15 +74,15 @@
 </p>
 
 ### Generate a maze and display its solution
 
 To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
 
 ```py
-from maze import Maze, Utilities
+from mazely import Maze, Utilities
 
 maze = Maze(32, 32)
 utils = Utilities()
 utils.show_solution()
 ```
 
 <p align="center">
```

### Comparing `mazely-0.1.0/src/mazely.egg-info/SOURCES.txt` & `mazely-0.1.1/src/mazely.egg-info/SOURCES.txt`

 * *Files identical despite different names*

