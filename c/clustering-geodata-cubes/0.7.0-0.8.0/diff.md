# Comparing `tmp/clustering-geodata-cubes-0.7.0.tar.gz` & `tmp/clustering-geodata-cubes-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustering-geodata-cubes-0.7.0.tar", last modified: Fri May  5 16:01:35 2023, max compression
+gzip compressed data, was "clustering-geodata-cubes-0.8.0.tar", last modified: Sat Jul  8 21:05:22 2023, max compression
```

## Comparing `clustering-geodata-cubes-0.7.0.tar` & `clustering-geodata-cubes-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:01:35.929626 clustering-geodata-cubes-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-05-05 16:01:35.929626 clustering-geodata-cubes-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:01:35.925626 clustering-geodata-cubes-0.7.0/cgc/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/cgc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/coclustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/coclustering_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/coclustering_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/triclustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/triclustering_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/triclustering_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/cgc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:01:35.925626 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-05-05 16:01:35.000000 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 16:01:35.000000 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:01:35.000000 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 16:01:35.000000 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 16:01:35.000000 clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:01:35.929626 clustering-geodata-cubes-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:01:35.929626 clustering-geodata-cubes-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_coclustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_coclustering_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_coclustering_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_triclustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_triclustering_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_triclustering_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_triclustering_numpy_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-05 16:01:12.000000 clustering-geodata-cubes-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/cgc/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/cgc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/coclustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/coclustering_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/coclustering_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/triclustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/triclustering_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/triclustering_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/cgc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-08 21:05:22.000000 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-08 21:05:22.000000 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:05:22.000000 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 21:05:22.000000 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-08 21:05:22.000000 clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:05:22.143987 clustering-geodata-cubes-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_coclustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_coclustering_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_coclustering_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_triclustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_triclustering_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_triclustering_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_triclustering_numpy_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-08 21:05:02.000000 clustering-geodata-cubes-0.8.0/tests/test_utils.py
```

### Comparing `clustering-geodata-cubes-0.7.0/LICENSE` & `clustering-geodata-cubes-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/PKG-INFO` & `clustering-geodata-cubes-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustering-geodata-cubes
-Version: 0.7.0
+Version: 0.8.0
 Summary: CGC: a Scalable Python Package for Co- and Tri-Clustering of Geodata Cubes
 Author: Ou Ku, Meiert W. Grootes, Emma Izquierdo-Verdiguier, Serkan Girgin, Raul Zurita-Milla
 Author-email: Francesco Nattino <f.nattino@esciencecenter.nl>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `clustering-geodata-cubes-0.7.0/README.rst` & `clustering-geodata-cubes-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/coclustering.py` & `clustering-geodata-cubes-0.8.0/cgc/coclustering.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/coclustering_dask.py` & `clustering-geodata-cubes-0.8.0/cgc/coclustering_dask.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/coclustering_numpy.py` & `clustering-geodata-cubes-0.8.0/cgc/coclustering_numpy.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/kmeans.py` & `clustering-geodata-cubes-0.8.0/cgc/kmeans.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,43 +20,46 @@
 ]
 
 
 class KMeansResults(Results):
     """
     Contains results and metadata of a k-means refinement calculation.
 
-    :var k_value: Optimal K value (value with maximum Silhouette score).
+    :var k_value: Optimal K value (value with maximum silhouette score).
     :type k_value: int
     :var labels: Refined clusters labels. It is a 2D- (for coclustering)
                  or 3D- (for triclustering) array, with the shape of
                  `nclusters`. The value at location (band, row, column)
                  represents the refined cluster label of the corresponding
                  band/row/column cluster combination.
     :type labels: np.ndarray
-    :var measure_list: List of Silhouette coefficients for all tested k values.
-    :type measure_list: np.ndarray
+    :var inertia: List of inertia values for all tested k values.
+    :type inertia: list
+    :var measure_list: List of silhouette coefficients for all tested k values.
+    :type measure_list: list
     :var cluster_averages: Refined cluster averages. They are computed as means
         over all elements of the co-/tri-clusters assigned to the refined
         clusters. Initially empty clusters are assigned NaN values.
     :type cluster_averages: np.ndarray
     """
     k_value = None
     labels = None
+    inertia = None
     measure_list = None
     cluster_averages = None
 
 
 class KMeans(object):
     """
     Perform a clustering refinement using k-means.
 
     A set of statistics is computed for all co- or tri-clusters, then these
     clusters are in turned grouped using k-means. K-means clustering is
     performed for multiple k values, then the optimal value is selected on the
-    basis of the Silhouette coefficient.
+    basis of the silhouette coefficient.
 
     :param Z: Data array (N dimensions).
     :type Z: numpy.ndarray or dask.array.Array
     :param clusters: Iterable with length N. It should contain the cluster
         labels for each dimension, following the same ordering as for Z.
     :type clusters: tuple, list, or numpy.ndarray
     :param nclusters: Iterable with length N. It should contains the number of
@@ -65,16 +68,17 @@
     :param k_range: Range of k values to test. Default from 2 to
         a fraction of the number of non-empty clusters (see max_k_ratio).
     :type k_range: tuple, list, or numpy.ndarray, optional
     :param max_k_ratio: If k_range is not provided, test all k values from 2
         to `max_k_ratio*max_k`, where `max_k` is the number of non-empty co- or
         tri-clusters. It will be ignored if `k_range` is given. Default to 0.8.
     :type max_k_ratio: float, optional
-    :param kmeans_max_iter: Maximum number of iterations of k-means.
-    :type kmeans_max_iter: int, optional
+    :param kmeans_kwargs: Arguments passed on when initializing the
+        scikit-learn's KMeans object.
+    :type kmeans_kwargs: dict, optional
     :param statistics: Statistics to be computed over the clusters, which are
         then used to refine these. These are provided as an iterable of
         callable functions, with optional keyword arguments. For example:
         [(func1, {'kwarg1': val1, ...}), (func2, {'kwarg2': val2, ...}, ...] .
         See cgc.kmeans.DEFAULT_STATISTICS for the default statistics, and
         cgc.utils.calculate_cluster_feature for input function requirements.
     :type statistics: tuple or list, optional
@@ -87,29 +91,29 @@
     >>> Z = np.array([[4, 4, 1, 1], [4, 4, 1, 1], [2, 2, 3, 3], [2, 2, 3, 3],
                    [2, 2, 3, 3]])
     >>> clusters = [np.array([0, 0, 1, 1, 1]), np.array([0, 0, 1, 1])]
     >>> km = KMeans(Z=Z,
                 clusters=clusters,
                 nclusters=[2, 2],
                 k_range= range(2, 4),
-                kmeans_max_iter=2)
+                kmeans_kwargs={"max_iter": 100})
     """
     def __init__(self,
                  Z,
                  clusters,
                  nclusters,
                  k_range=None,
                  max_k_ratio=0.8,
-                 kmeans_max_iter=100,
+                 kmeans_kwargs=None,
                  statistics=None,
                  output_filename=''):
         # Input parameters -----------------
         self.clusters = clusters
         self.nclusters = nclusters
-        self.kmeans_max_iter = kmeans_max_iter
+        self.kmeans_kwargs = {} if kmeans_kwargs is None else kmeans_kwargs
         self.output_filename = output_filename
 
         max_k = np.prod(self.nclusters)
         if k_range is None:
             self.k_range = list(range(2, int(max_k * max_k_ratio)))
         else:
             self.k_range = list(k_range)
@@ -126,15 +130,15 @@
             self.statistics.append((func, kwargs))
         # Input parameters end -------------
 
         # Store input parameters in results object
         self.results = KMeansResults(
             clusters=self.clusters,
             nclusters=self.nclusters,
-            kmean_max_iter=self.kmeans_max_iter,
+            kmeans_kwargs=self.kmeans_kwargs,
             output_filename=self.output_filename,
             k_range=self.k_range,
             statistics=[(func.__name__, kw) for func, kw in self.statistics],
         )
 
         self.Z = Z
 
@@ -171,53 +175,57 @@
                            "of the number of clusters or more)")
 
         self.stat_measures_norm = None
 
     def compute(self, recalc_statistics=False):
         """
         Compute statistics for each clustering group. Then loop through the
-        range of k values, and compute the averaged Silhouette measure of each
-        k value. Finally select the k with the maximum Silhouette measure.
+        range of k values, and compute the averaged silhouette measure of each
+        k value. Finally select the k with the maximum silhouette measure.
 
         :param recalc_statistics: If True, always recompute statistics.
         :type recalc_statistics: bool, optional
         :return: K-means results.
         :type: cgc.kmeans.KMeansResults
         """
         # Compute statistics
         if self.stat_measures_norm is None or recalc_statistics:
             self._compute_statistic_measures()
 
         # Search for value k
-        silhouette_avg_list = np.array([])  # average silhouette measure vs k
+        inertia_list = []
+        silhouette_list = []  # average silhouette score vs k
         kmeans_label_list = []
         for k in self.k_range:
-            # Compute Kmean
+            # Compute k-means
             km = sklearn.cluster.KMeans(
-                n_clusters=k, max_iter=self.kmeans_max_iter
+                n_clusters=k, **self.kmeans_kwargs
             )
             kmeans_cluster = km.fit(self.stat_measures_norm)
-            silhouette_avg = silhouette_score(self.stat_measures_norm,
-                                              kmeans_cluster.labels_)
-            silhouette_avg_list = np.append(silhouette_avg_list,
-                                            silhouette_avg)
+            silhouette = silhouette_score(
+                self.stat_measures_norm, kmeans_cluster.labels_
+            )
+            silhouette_list.append(silhouette)
             kmeans_label_list.append(kmeans_cluster.labels_)
-        idx_k = np.argmax(silhouette_avg_list)
-        if np.sum(silhouette_avg_list == silhouette_avg_list[idx_k]) > 1:
-            idx_k_list = np.argwhere(
-                silhouette_avg_list == silhouette_avg_list[idx_k]).reshape(
-                    -1).tolist()
+            inertia_list.append(kmeans_cluster.inertia_)
+        idx = np.argmax(silhouette_list)
+        max_silhouette_mask = np.array(silhouette_list) == silhouette_list[idx]
+        if np.sum(max_silhouette_mask) > 1:
+            idxs = np.argwhere(max_silhouette_mask)
             logger.warning(
                 "Multiple k values with the same silhouette score: {},"
                 "picking the smallest one: {}".format(
-                    [self.k_range[i] for i in idx_k_list],
-                    self.k_range[idx_k]))
-        self.results.measure_list = silhouette_avg_list
-        self.results.k_value = self.k_range[idx_k]
-        labels = kmeans_label_list[idx_k]
+                    [self.k_range[i] for i in idxs.flatten()],
+                    self.k_range[idx]
+                )
+            )
+        self.results.measure_list = silhouette_list
+        self.results.k_value = self.k_range[idx]
+        self.results.inertia = inertia_list
+        labels = kmeans_label_list[idx]
 
         indices = np.meshgrid(*[np.unique(cl) for cl in self.clusters],
                               indexing='ij')
         mask = np.zeros(self.nclusters, dtype=bool)
         mask[tuple(indices)] = True
 
         # Make a lookup matrix from un-refined clusters to Kmean clusters
```

### Comparing `clustering-geodata-cubes-0.7.0/cgc/results.py` & `clustering-geodata-cubes-0.8.0/cgc/results.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/triclustering.py` & `clustering-geodata-cubes-0.8.0/cgc/triclustering.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/triclustering_dask.py` & `clustering-geodata-cubes-0.8.0/cgc/triclustering_dask.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/triclustering_numpy.py` & `clustering-geodata-cubes-0.8.0/cgc/triclustering_numpy.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/cgc/utils.py` & `clustering-geodata-cubes-0.8.0/cgc/utils.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/PKG-INFO` & `clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustering-geodata-cubes
-Version: 0.7.0
+Version: 0.8.0
 Summary: CGC: a Scalable Python Package for Co- and Tri-Clustering of Geodata Cubes
 Author: Ou Ku, Meiert W. Grootes, Emma Izquierdo-Verdiguier, Serkan Girgin, Raul Zurita-Milla
 Author-email: Francesco Nattino <f.nattino@esciencecenter.nl>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `clustering-geodata-cubes-0.7.0/clustering_geodata_cubes.egg-info/SOURCES.txt` & `clustering-geodata-cubes-0.8.0/clustering_geodata_cubes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/pyproject.toml` & `clustering-geodata-cubes-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustering-geodata-cubes"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
     "dask[complete]",
     "matplotlib",
     "numba",
     "numpy",
     "scikit-learn",
 ]
```

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_coclustering.py` & `clustering-geodata-cubes-0.8.0/tests/test_coclustering.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_coclustering_dask.py` & `clustering-geodata-cubes-0.8.0/tests/test_coclustering_dask.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_coclustering_numpy.py` & `clustering-geodata-cubes-0.8.0/tests/test_coclustering_numpy.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_kmeans.py` & `clustering-geodata-cubes-0.8.0/tests/test_kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,20 @@
                   [1, 1, 0, 0]])
     row_clusters = np.array([0, 0, 1, 1, 1])
     col_clusters = np.array([0, 0, 1, 1])
     nrow_clusters, ncol_clusters = 3, 2  # 1 non populated row/col cluster
     clusters = [row_clusters, col_clusters]
     nclusters = [nrow_clusters, ncol_clusters]
     k_range = range(2, 4)
-    kmeans_max_iter = 100
+    kmeans_kwargs = {"init": "k-means++", "n_init": "auto"}
     km = KMeans(Z=Z,
                 clusters=clusters,
                 nclusters=nclusters,
                 k_range=k_range,
-                kmeans_max_iter=kmeans_max_iter)
+                kmeans_kwargs=kmeans_kwargs)
     return km
 
 
 def init_cocluster_km_with_noise():
     Z = np.array([
         [0.0, 0.2, 1.0, 1.1],
         [0.2, 0.0, 1.1, 1.0],
@@ -47,20 +47,20 @@
     ])
     row_clusters = np.array([0, 0, 1, 1, 1])
     col_clusters = np.array([0, 0, 1, 1])
     nrow_clusters, ncol_clusters = 3, 2  # 1 non populated row/col cluster
     clusters = [row_clusters, col_clusters]
     nclusters = [nrow_clusters, ncol_clusters]
     k_range = range(2, 4)
-    kmeans_max_iter = 2
+    kmeans_kwargs = {"init": "k-means++", "n_init": "auto"}
     km = KMeans(Z=Z,
                 clusters=clusters,
                 nclusters=nclusters,
                 k_range=k_range,
-                kmeans_max_iter=kmeans_max_iter)
+                kmeans_kwargs=kmeans_kwargs)
     return km
 
 
 def init_tricluster_km():
     Z1 = np.array([[0, 0, 1, 1], [0, 0, 1, 1], [1, 1, 0, 0]])
     Z = np.full((4, 3, 4), 0)
     Z[:2] = Z1
@@ -68,20 +68,20 @@
     row_clusters = np.array([0, 0, 1])
     col_clusters = np.array([0, 0, 1, 1])
     band_clusters = np.array([0, 0, 1, 1])
     nrow_clusters, ncol_clusters, nband_clusters = 2, 2, 2
     clusters = [band_clusters, row_clusters, col_clusters]
     nclusters = [nband_clusters, nrow_clusters, ncol_clusters]
     k_range = range(2, 4)
-    kmeans_max_iter = 2
+    kmeans_kwargs = {"init": "k-means++", "n_init": "auto"}
     km = KMeans(Z=Z,
                 clusters=clusters,
                 nclusters=nclusters,
                 k_range=k_range,
-                kmeans_max_iter=kmeans_max_iter)
+                kmeans_kwargs=kmeans_kwargs)
     return km
 
 
 class TestKMeans(unittest.TestCase):
     def test_Z_and_cluster_shape_not_match(self):
         with self.assertRaises(ValueError):
             KMeans(Z=np.random.random((5, 5)),
@@ -260,20 +260,18 @@
                       [1, 1, 2, 2]])
         row_clusters = np.array([0, 0, 1, 1, 1])
         col_clusters = np.array([0, 0, 1, 1])
         nrow_clusters, ncol_clusters = 2, 2
         clusters = [row_clusters, col_clusters]
         nclusters = [nrow_clusters, ncol_clusters]
         k_range = [2, 3]
-        kmeans_max_iter = 100
         km = KMeans(Z=Z,
                     clusters=clusters,
                     nclusters=nclusters,
                     k_range=k_range,
-                    kmeans_max_iter=kmeans_max_iter,
                     statistics=(np.mean, (np.std, {'axis': None})))
         res = km.compute()
         assert res.input_parameters["statistics"][0][0] == "mean"
         assert len(res.input_parameters["statistics"][0][1]) == 0
         assert res.input_parameters["statistics"][1][0] == "std"
         assert len(res.input_parameters["statistics"][1][1]) == 1
         assert res.k_value == 3
@@ -287,21 +285,21 @@
                       [1, 0.5, 2, 0.5]])
         row_clusters = np.array([0, 0, 1, 1, 1])
         col_clusters = np.array([0, 0, 1, 1])
         nrow_clusters, ncol_clusters = 2, 2
         clusters = [row_clusters, col_clusters]
         nclusters = [nrow_clusters, ncol_clusters]
         k_range = [2, 3]
-        kmeans_max_iter = 100
+        kmeans_kwargs = {"init": "k-means++", "n_init": "auto"}
 
         def run_kmeans(statistics=None):
             km = KMeans(Z=Z,
                         clusters=clusters,
                         nclusters=nclusters,
                         k_range=k_range,
-                        kmeans_max_iter=kmeans_max_iter,
+                        kmeans_kwargs=kmeans_kwargs,
                         statistics=statistics)
             res = km.compute()
             return res.k_value
 
         assert run_kmeans() == 3
         assert run_kmeans((np.min,)) == 2
```

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_lint.py` & `clustering-geodata-cubes-0.8.0/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_triclustering.py` & `clustering-geodata-cubes-0.8.0/tests/test_triclustering.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_triclustering_dask.py` & `clustering-geodata-cubes-0.8.0/tests/test_triclustering_dask.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_triclustering_numpy.py` & `clustering-geodata-cubes-0.8.0/tests/test_triclustering_numpy.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_triclustering_numpy_legacy.py` & `clustering-geodata-cubes-0.8.0/tests/test_triclustering_numpy_legacy.py`

 * *Files identical despite different names*

### Comparing `clustering-geodata-cubes-0.7.0/tests/test_utils.py` & `clustering-geodata-cubes-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

