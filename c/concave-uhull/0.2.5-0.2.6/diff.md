# Comparing `tmp/concave_uhull-0.2.5.tar.gz` & `tmp/concave_uhull-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concave_uhull-0.2.5.tar", max compression
+gzip compressed data, was "concave_uhull-0.2.6.tar", max compression
```

## Comparing `concave_uhull-0.2.5.tar` & `concave_uhull-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      321 2023-02-13 23:11:05.234480 concave_uhull-0.2.5/README_pypi.rst
--rw-r--r--   0        0        0        0 2023-02-08 19:07:35.341531 concave_uhull-0.2.5/concave_uhull/__init__.py
--rw-r--r--   0        0        0    12270 2023-02-14 14:11:00.923949 concave_uhull-0.2.5/concave_uhull/alpha_shape.py
--rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341531 concave_uhull-0.2.5/concave_uhull/geometry.py
--rw-r--r--   0        0        0     7621 2023-04-24 15:42:23.043369 concave_uhull-0.2.5/concave_uhull/graph.py
--rw-r--r--   0        0        0      835 2023-04-24 17:56:42.423275 concave_uhull-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 concave_uhull-0.2.5/setup.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 concave_uhull-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-02-13 23:11:05.234480 concave_uhull-0.2.6/README_pypi.rst
+-rw-r--r--   0        0        0        0 2023-02-08 19:07:35.341531 concave_uhull-0.2.6/concave_uhull/__init__.py
+-rw-r--r--   0        0        0    12313 2023-07-08 14:53:02.390568 concave_uhull-0.2.6/concave_uhull/alpha_shape.py
+-rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341531 concave_uhull-0.2.6/concave_uhull/geometry.py
+-rw-r--r--   0        0        0     7660 2023-06-17 20:10:07.464809 concave_uhull-0.2.6/concave_uhull/graph.py
+-rw-r--r--   0        0        0      834 2023-07-08 15:09:57.743993 concave_uhull-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 concave_uhull-0.2.6/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 concave_uhull-0.2.6/PKG-INFO
```

### Comparing `concave_uhull-0.2.5/concave_uhull/alpha_shape.py` & `concave_uhull-0.2.6/concave_uhull/alpha_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,34 +272,33 @@
     alpha_shape_polygons_list: List = []
     while nodes_to_explore:
 
         # Step 3.1: A random edge is selected, its extreme points memorized and
         # the edge removed from the graph.
         edge_source = nodes_to_explore.pop()
         edge_target = next(iter(graph[edge_source]), None)
-        if edge_target is None:
-            continue
-        graph.remove_edge(
-            edge_source=edge_source,
-            edge_target=edge_target,
-        )
+        if edge_target:
+            graph.remove_edge(
+                edge_source=edge_source,
+                edge_target=edge_target,
+            )
 
-        # Step 3.2: The shortest path from one memorized extreme point to the
-        # other is obtained. With this path, we form a polygon of the alpha shape
-        # by adding the first point to the end of the path.
-        polygon_vertices = shortest_path_algorithm(
-            graph=graph, edge_source=edge_source, edge_target=edge_target
-        )
-        polygon_vertices.append(edge_source)
+            # Step 3.2: The shortest path from one memorized extreme point to the
+            # other is obtained. With this path, we form a polygon of the alpha shape
+            # by adding the first point to the end of the path.
+            polygon_vertices = shortest_path_algorithm(
+                graph=graph, edge_source=edge_source, edge_target=edge_target
+            )
+            polygon_vertices.append(edge_source)
 
-        # Step 3.3:  After that all waypoints are removed from the set of points
-        # to be explored. And then add the obtained polygon to the polygon list of
-        # the alpha shape.
-        for vertice in polygon_vertices:
-            if vertice in nodes_to_explore:
-                nodes_to_explore.remove(vertice)
-        alpha_shape_polygons_list.append(polygon_vertices)
+            # Step 3.3:  After that all waypoints are removed from the set of points
+            # to be explored. And then add the obtained polygon to the polygon list of
+            # the alpha shape.
+            for vertice in polygon_vertices:
+                if vertice in nodes_to_explore:
+                    nodes_to_explore.remove(vertice)
+            alpha_shape_polygons_list.append(polygon_vertices)
 
     # Step 4: Returns list of alpha shape polygons in descending order by
     # polygon area.
     alpha_shape_polygons_list.sort(key=area_of_polygon, reverse=True)
     return alpha_shape_polygons_list
```

### Comparing `concave_uhull-0.2.5/concave_uhull/geometry.py` & `concave_uhull-0.2.6/concave_uhull/geometry.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.5/concave_uhull/graph.py` & `concave_uhull-0.2.6/concave_uhull/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,20 +154,21 @@
     }
     heap: List = [(distance[edge_source], edge_source)]
     predecessors: Dict = dict()
     while heap:
         distance_node, node = heappop(heap)
         if node == edge_target:
             break
-        if node in explored:
-            continue
-        explored.add(node)
         for neighbor in graph[node]:
             distance_neighbor = distance_node + graph.weight[node][neighbor]
-            if distance_neighbor < distance[neighbor]:
+            if (
+                neighbor not in explored
+                and distance_neighbor < distance[neighbor]
+            ):
+                explored.add(neighbor)
                 distance[neighbor] = distance_neighbor
                 heappush(heap, (distance[neighbor], neighbor))
                 predecessors[neighbor] = node
     return distance, predecessors
 
 
 def shortest_path_algorithm(
```

### Comparing `concave_uhull-0.2.5/pyproject.toml` & `concave_uhull-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "concave_uhull"
-version = "0.2.5"
+version = "0.2.6"
 description = "A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm."
 readme = "README_pypi.rst"
 authors = ["Luan <llvdmoraes@gmail.com>"]
 repository = "https://github.com/luanleonardo/concave_uhull"
 homepage = "https://luanleonardo.github.io/concave_uhull/"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-numpy = "^1.24.1"
+numpy = "1.22.4"
 scipy = "^1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^22.12.0"}
 isort = "^5.11.4"
 ipython = "^8.8.0"
 pytest-cov = "^4.0.0"
```

### Comparing `concave_uhull-0.2.5/setup.py` & `concave_uhull-0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['concave_uhull']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.1,<2.0.0', 'scipy>=1.10.0,<2.0.0']
+['numpy==1.22.4', 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'concave-uhull',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.',
     'long_description': '==============\nConcave uhull*\n==============\n\nA simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.\n\nNotes\n-----\n  * uhull! (Brazil) yeah! (expresses joy or celebration)\n\nHomepage\n========\n* `Project Homepage <https://luanleonardo.github.io/concave_uhull/>`_\n',
     'author': 'Luan',
     'author_email': 'llvdmoraes@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://luanleonardo.github.io/concave_uhull/',
```

### Comparing `concave_uhull-0.2.5/PKG-INFO` & `concave_uhull-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: concave-uhull
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.
 Home-page: https://luanleonardo.github.io/concave_uhull/
 Author: Luan
 Author-email: llvdmoraes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: numpy (==1.22.4)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/luanleonardo/concave_uhull
 Description-Content-Type: text/x-rst
 
 ==============
 Concave uhull*
 ==============
```

