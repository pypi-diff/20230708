# Comparing `tmp/cla-2.0.2.tar.gz` & `tmp/cla-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cla-2.0.2.tar", last modified: Fri Jul  7 10:38:33 2023, max compression
+gzip compressed data, was "cla-2.0.3.tar", last modified: Sat Jul  8 11:47:08 2023, max compression
```

## Comparing `cla-2.0.2.tar` & `cla-2.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:33.045652 cla-2.0.2/
--rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-2.0.2/LICENCE
--rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4563 2023-07-07 10:38:33.043652 cla-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:32.774719 cla-2.0.2/cla/
--rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-2.0.2/cla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:32.999393 cla-2.0.2/cla/gui/
--rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-2.0.2/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-2.0.2/cla/gui/__init__.py
--rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-2.0.2/cla/gui/run.py
--rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-2.0.2/cla/gui/sample.csv
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:33.016398 cla-2.0.2/cla/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-2.0.2/cla/gui/static/__init__.py
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-2.0.2/cla/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-2.0.2/cla/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-2.0.2/cla/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-2.0.2/cla/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-2.0.2/cla/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-2.0.2/cla/gui/static/sample.csv
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:33.021394 cla-2.0.2/cla/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-2.0.2/cla/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-2.0.2/cla/gui/templates/home.html
--rw-rw-rw-   0        0        0    80747 2023-07-04 09:19:03.000000 cla-2.0.2/cla/metrics.py
--rw-rw-rw-   0        0        0    16031 2023-07-06 10:06:52.000000 cla-2.0.2/cla/unify.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:33.039382 cla-2.0.2/cla/vis/
--rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-2.0.2/cla/vis/__init__.py
--rw-rw-rw-   0        0        0     6471 2023-06-28 15:04:04.000000 cla-2.0.2/cla/vis/confusion_matrix.py
--rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-2.0.2/cla/vis/feature_importance.py
--rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-2.0.2/cla/vis/plotComponents1D.py
--rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-2.0.2/cla/vis/plotComponents2D.py
--rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-2.0.2/cla/vis/plotComponents3D.py
--rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-2.0.2/cla/vis/plt2base64.py
--rw-rw-rw-   0        0        0     4953 2023-06-28 11:18:59.000000 cla-2.0.2/cla/vis/unsupervised_dimension_reductions.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:32.992401 cla-2.0.2/cla.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-07-07 10:38:32.000000 cla-2.0.2/cla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-07 10:38:32.000000 cla-2.0.2/cla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:38:32.000000 cla-2.0.2/cla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-07 10:38:32.000000 cla-2.0.2/cla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-07 10:38:32.000000 cla-2.0.2/cla.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 10:38:33.041397 cla-2.0.2/data/
--rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-2.0.2/data/sample.csv
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 10:38:33.045652 cla-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-07-07 10:38:15.000000 cla-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.814050 cla-2.0.3/
+-rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-2.0.3/LICENCE
+-rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4563 2023-07-08 11:47:08.813054 cla-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.561169 cla-2.0.3/cla/
+-rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-2.0.3/cla/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.778867 cla-2.0.3/cla/gui/
+-rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-2.0.3/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-2.0.3/cla/gui/__init__.py
+-rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-2.0.3/cla/gui/run.py
+-rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-2.0.3/cla/gui/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.791958 cla-2.0.3/cla/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-2.0.3/cla/gui/static/__init__.py
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-2.0.3/cla/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-2.0.3/cla/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-2.0.3/cla/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-2.0.3/cla/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-2.0.3/cla/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-2.0.3/cla/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.795953 cla-2.0.3/cla/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-2.0.3/cla/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-2.0.3/cla/gui/templates/home.html
+-rw-rw-rw-   0        0        0    80640 2023-07-08 11:46:40.000000 cla-2.0.3/cla/metrics.py
+-rw-rw-rw-   0        0        0    16300 2023-07-08 11:22:00.000000 cla-2.0.3/cla/unify.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.810072 cla-2.0.3/cla/vis/
+-rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-2.0.3/cla/vis/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-06-28 15:04:04.000000 cla-2.0.3/cla/vis/confusion_matrix.py
+-rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-2.0.3/cla/vis/feature_importance.py
+-rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-2.0.3/cla/vis/plotComponents1D.py
+-rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-2.0.3/cla/vis/plotComponents2D.py
+-rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-2.0.3/cla/vis/plotComponents3D.py
+-rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-2.0.3/cla/vis/plt2base64.py
+-rw-rw-rw-   0        0        0     4953 2023-06-28 11:18:59.000000 cla-2.0.3/cla/vis/unsupervised_dimension_reductions.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.762087 cla-2.0.3/cla.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-07-08 11:47:08.000000 cla-2.0.3/cla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-08 11:47:08.000000 cla-2.0.3/cla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 11:47:08.000000 cla-2.0.3/cla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-08 11:47:08.000000 cla-2.0.3/cla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 11:47:08.000000 cla-2.0.3/cla.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 11:47:08.812053 cla-2.0.3/data/
+-rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-2.0.3/data/sample.csv
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 11:47:08.815051 cla-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-08 08:29:12.000000 cla-2.0.3/setup.py
```

### Comparing `cla-2.0.2/PKG-INFO` & `cla-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 2.0.2
+Version: 2.0.3
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 2.0.2 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 2.0.3 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-2.0.2/README.md` & `cla-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv` & `cla-2.0.3/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/run.py` & `cla-2.0.3/cla/gui/run.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/sample.csv` & `cla-2.0.3/cla/gui/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/bootstrap.css` & `cla-2.0.3/cla/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/bootstrap.js` & `cla-2.0.3/cla/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/jquery-3.3.1.min.js` & `cla-2.0.3/cla/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/jquery.blockUI.js` & `cla-2.0.3/cla/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/jquery.form.min.js` & `cla-2.0.3/cla/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/static/sample.csv` & `cla-2.0.3/cla/gui/static/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/gui/templates/home.html` & `cla-2.0.3/cla/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/metrics.py` & `cla-2.0.3/cla/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -861,14 +861,15 @@
 
     try:
         mi = mutual_info_classif(X, y, discrete_features=False)
     except Exception as e:
         print('Exception in mutual_info_classif().', e)
         return None, None
 
+
     mi_sorted = np.sort(mi)[::-1]  # sort in desceding order
     mi_sorted_idx = np.argsort(mi)[::-1]
 
     if (X.shape[1] > 50):
         plt.figure(figsize=(20, 3))
     else:
         plt.figure()  # use default fig size
@@ -897,15 +898,15 @@
         plt.show()
     else:
         plt.close()
 
     return mi, IMG
 
 
-def CHISQ(X, y, show=False, save_fig=''):
+def CHISQ(X, y, show=False, save_fig='', verbose = False):
     """
     Performa feature-wise chi-square test. 
     Returns an array of chi2 statistics and p-values on all the features.
 
     This test can be used to select the n_features features with the highest values
     for the test chi-squared statistic from X, which must contain only non-negative
     features such as booleans or frequencies (e.g., term counts in document 
@@ -1021,15 +1022,14 @@
     if (len(set(y)) != 2):
         if verbose:
             print('The dataset must have two classes for t test.')
         return None, None, None
 
     ps = []
     Ts = []
-    cnt = 0
     IMG = ''
 
     for i in range(X.shape[1]):
         Xi = X[:, i]
         Xcis = []
 
         labels = []
@@ -1048,32 +1048,32 @@
             T, p = scipy.stats.ttest_ind(Xcis[0], Xcis[1])
         else:
             T, p = scipy.stats.ttest_ind(Xcis[0], Xcis[1], equal_var=False)
 
         ps.append(p)
         Ts.append(T)
 
-        if (cnt < max_plot_num):
+        if (i < max_plot_num):
             plt.figure()
             # plot ith feature of different classes
             plt.boxplot(Xcis, notch=False, labels=labels)
             test_result = "independent t test on X{}: T={},p={}".format(
                 i + 1, round(T, 3), round(p, 3))
             # plt.legend(labels)
             plt.title(test_result)
             IMG += plt2html(plt)
 
             if show:
                 plt.show()
             else:
                 plt.close()
-        elif cnt == max_plot_num:
+        elif i == max_plot_num:
             IMG += '<p>Showing the first ' + str(max_plot_num) + ' plots.</p>'
         else:
-            pass  # plot no more to avoid memory cost
+            pass # plot no more to avoid memory cost
 
     if verbose:
         print('The P values of X in dimensions 1 to {}:{}'.format(
             len(X[0]), ps))
         print('The values of T statistics of X in dimensions 1 to {}:{}'.format(
             len(X[0]), Ts))
 
@@ -1196,16 +1196,14 @@
             print('The dataset must have at least two classes for ANOVA test.')
         return None, None, None
 
     ps = []
     IMG = ''
     Fs = []
 
-    cnt = 0
-
     for i in range(X.shape[1]):
         Xi = X[:, i]
         Xcis = []
 
         labels = []
         for c in set(y):
             Xc = Xi[y == c]
@@ -1243,34 +1241,32 @@
         anova_table = sm.stats.anova_lm(model, typ=1)
         anova_table
         """
 
         ps.append(p)
         Fs.append(f)
 
-        if (cnt < max_plot_num):
+        if (i < max_plot_num):
 
             plt.figure()
             # plot ith feature of different classes
             plt.boxplot(Xcis, notch=False, labels=labels)
             test_result = "ANOVA on X{}: f={},p={}".format(i+1, f, round(p, 3))
             # plt.legend(labels)
             plt.title(test_result)
             IMG += plt2html(plt)
 
             if show:
                 plt.show()
             else:
                 plt.close()
-        elif cnt == max_plot_num:
+        elif i == max_plot_num:
             IMG += '<p>Showing the first ' + str(max_plot_num) + ' plots.</p>'
         else:
-            pass  # plot no more to avoid memory cost
-
-        cnt = cnt+1
+            pass # plot no more to avoid memory cost
 
         if verbose:
             print(test_result)
 
     IMG += '<br/>'
 
     return ps, Fs, IMG
@@ -1336,16 +1332,14 @@
             print('The dataset must have two classes for MWW test.')
         return None, None, None
 
     ps = []
     Us = []
     IMG = ''
 
-    cnt = 0
-
     for i in range(X.shape[1]):
         Xi = X[:, i]
         Xcis = []
 
         for c in set(y):
             Xc = Xi[y == c]
             Xcis.append(Xc)
@@ -1361,15 +1355,15 @@
             p = 1
         else:
             U, p = scipy.stats.mannwhitneyu(Xcis[0], Xcis[1])
 
         ps.append(p)
         Us.append(U)
 
-        if cnt < max_plot_num:
+        if i < max_plot_num:
             plt.figure()
             plt.hist(Xcis, bins=min(12, int(len(y)/3)), alpha=0.4, edgecolor='black', label=["$ X_"+str(
                 i+1)+"^{( y_"+str(0)+")} $", "$ X_"+str(i+1)+"^{( y_"+str(1)+")} $"])  # plot ith feature of different classes
             test_result = "MWW test on X{}: U={},p={}".format(
                 i+1, U, round(p, 3))
             plt.title('Feature X{} histogram on different classes\n'.format(
                 i+1) + test_result)
@@ -1377,22 +1371,19 @@
             IMG += plt2html(plt) + '<br/>'
 
             if show:
                 plt.show()
             else:
                 plt.close()
 
-        elif cnt == max_plot_num:
+        elif i == max_plot_num:
             IMG += '<p>Showing the first ' + str(max_plot_num) + ' plots.</p>'
-
         else:
             pass  # plot no more to avoid memory cost
 
-        cnt = cnt + 1
-
         if verbose:
             print(test_result)
 
     IMG += '<br/>'
 
     return ps, Us, IMG
 
@@ -1559,15 +1550,14 @@
         if verbose:
             print('The dataset must have two classes for KS test.')
         return None, None, None
     
     ps = []
     Ds = []
     IMG = ''
-    cnt = 0
 
     for i in range(X.shape[1]):
         Xi = X[:, i]
         Xcis = []
 
         for c in set(y):
             Xc = Xi[y == c]
@@ -1576,15 +1566,15 @@
         # Xcis = np.array(Xcis)
 
         D, p = scipy.stats.ks_2samp(Xcis[0], Xcis[1])
 
         ps.append(p)
         Ds.append(D)
 
-        if cnt < max_plot_num:
+        if i < max_plot_num:
 
             plt.figure()
             plt.hist(Xcis, cumulative=True, histtype=u'step', bins=min(12, int(len(y)/3)), label=["$ CDF( X_"+str(
                 i+1)+"^{(y_"+str(0)+")} ) $", "$ CDF( X_"+str(i+1)+"^{(y_"+str(1)+")} ) $"])  # plot ith feature of different classes
             test_result = "KS test on X{}: D={},p={}".format(
                 i+1, D, round(p, 3))
             plt.title('Feature X{} CDF on the two classes\n'.format(
@@ -1598,16 +1588,14 @@
                 plt.close()
 
         elif cnt == max_plot_num:
             IMG += '<p>Showing the first ' + str(max_plot_num) + ' plots.</p>'
         else:
             pass  # plot no more to avoid memory cost
 
-        cnt = cnt+1
-
     IMG += "<br/>"
     return ps, Ds, IMG
 
 
 ECoL_METRICS = ['overlapping.F1.mean',
                 'overlapping.F1.sd',
                 'overlapping.F1v.mean',
@@ -1812,15 +1800,15 @@
             dic['test.KS'] = p
             dic['test.KS.min'] = np.min(p)
             dic['test.KS.min.log10'] = np.log10(np.min(p))
         if D is not None:
             dic['test.KS.D'] = D
             dic['test.KS.D.max'] = np.max(D)
 
-    p, C, _ = CHISQ(X, y)
+    p, C, _ = CHISQ(X, y, verbose = verbose)
     dic['test.CHISQ'] = p
     dic['test.CHISQ.min'] = np.min(p)
     dic['test.CHISQ.min.log10'] = np.log10(np.min(p))
     dic['test.CHISQ.CHI2'] = C
     dic['test.CHISQ.CHI2.max'] = np.max(C)
 
     # H follows chi2, its critical value of chi2(k-1) at 0.5
```

### Comparing `cla-2.0.2/cla/unify.py` & `cla-2.0.3/cla/unify.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,23 +45,24 @@
         dic = joblib.load(pkl) # load an existing pkl file
         pkl_file = pkl
         print('Load atom metrics from', pkl_file)
     else:
         dic = calculate_atom_metrics(mu = X.mean(axis = 0), s = X.std(axis = 0),
                             mds = np.linspace(0, 6, 7+6*2),
                             repeat = 5, nobs = 100,
-                            show_curve = True, show_html = True, verbose = verbose)
+                            show_curve = True, show_html = True, 
+                            verbose = verbose)
         pkl_file = str(datetime.now()).replace(':','').replace('-','').replace(' ','') + '.pkl'
         joblib.dump(dic, pkl_file) # later we can reload with: dic = joblib.load('x.pkl')
         print('Save atom metrics to', pkl_file)
 
     _, keys, _, M = filter_metrics(dic, threshold = (0.5 if use_filter else None))
     if method == 'decompose.pca':
         model, x_min, x_max, slope = train_decomposer_pca(M, dic['d'])
-        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method)
+        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method, verbose=verbose)
 
         # maps to the [0,1] range
         print('before scaling: ', umetric_bw, umetric_in)
         print('PC1 range: ', x_min, x_max)
 
         '''
         np.interp(x, xp, fp, left=None, right=None)
@@ -76,31 +77,31 @@
         '''
         umetric_bw = np.interp(umetric_bw,[x_min,x_max],[0,1] if slope else [1,0])
         umetric_in = np.interp(umetric_in,[x_min,x_max],[0,1] if slope else [1,0])
         print('after scaling: ', umetric_bw, umetric_in)
 
     elif method == 'meta.logistic':
         model = train_metalearner_logistic(M, dic['d'])
-        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method)
+        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method, verbose=verbose)
     
     elif method == 'decompose.lda':
         model, x_min, x_max, slope = train_decomposer_lda(M, dic['d'])
-        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method)
+        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method, verbose=verbose)
 
         # maps to the [0,1] range
         print('before scaling: ', umetric_bw, umetric_in)
         print('C1 range: ', x_min, x_max)
 
         umetric_bw = np.interp(umetric_bw, [x_min, x_max], [0, 1] if slope else [1,0])
         umetric_in = np.interp(umetric_in, [x_min, x_max], [0, 1] if slope else [1,0])
         print('after scaling: ', umetric_bw, umetric_in)
 
     elif method == 'meta.linear':
         model = train_metalearner_linear(M, dic['d'])
-        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method)
+        umetric_bw, umetric_in = calculate_unified_metric(X, y, model, keys, method, verbose=verbose)
 
     else:
         raise Exception('Unsupported method ' + method )
 
     return umetric_bw, umetric_in, pkl_file
 
 def mvgx(
@@ -367,36 +368,36 @@
     d = np.array(d) >= cutoff # np.median(d)
 
     clf = LogisticRegression(max_iter=1000, solver='liblinear').fit(M, d)
     print('Score: ', clf.score(M, d))
     print('Coef and Intercept: ', clf.coef_, clf.intercept_)
     return clf
 
-def calculate_unified_metric(X, y, model, keys,method):
+def calculate_unified_metric(X, y, model, keys, method, verbose = False):
     '''
     First, fit a linear regression (meta-learner) model for M on d.
     Then, calcualte the between-class and in-class unified metric on real dataset X and y.
 
     Parameters
     ----------
     model : meta-learner model, returned by train_metalearner()
     keys : selected metric names, returned by filter_metrics()
     '''
-    return AnalyzeBetweenClass(X ,y, model, keys,method), AnalyzeInClass(X, y, model, keys,method)
+    return AnalyzeBetweenClass(X ,y, model, keys, method, verbose=verbose), AnalyzeInClass(X, y, model, keys,method, verbose=verbose)
 
-def AnalyzeBetweenClass(X, y, model, keys, method):
+def AnalyzeBetweenClass(X, y, model, keys, method, verbose = False):
 
     X_pca = PCA(n_components = 2).fit_transform(X)
     plotComponents2D(X_pca, y)
 
-    _, new_dic = get_metrics(X, y)
+    _, new_dic = get_metrics(X, y, verbose=verbose)
     vec_metrics = []
 
     for key in keys:
-        vec_metrics.append(new_dic[key])
+        vec_metrics.append(new_dic[key] if key in new_dic else 0)
 
     vec_metrics = np.nan_to_num(vec_metrics,nan=0,posinf=1000,neginf=-1000)
     if method == 'meta.logistic' and isinstance(model, LogisticRegression):
         umetric = model.predict_proba([vec_metrics.T])[0][1]
     elif method == 'decompose.pca' and isinstance(model, PCA):
         M = vec_metrics.reshape(1,-1)
         umetric = model.transform(M)[0][0]
@@ -408,33 +409,33 @@
         # M=(M-mean)/std
         umetric = model.predict(M)
     else:
         raise Exception('Unsupported method ' + method )
     # print("between-class unified metric = ", umetric[1])
     return umetric
 
-def AnalyzeInClass(X, y, model, keys, method, repeat = 3):
+def AnalyzeInClass(X, y, model, keys, method, repeat = 3, verbose = False):
     '''
     Parameters
     ----------
     repeat : to get in-class metrics, samples of each class are randomly assigned different labels.
         This controls how many times to run to get the averaged result.
     '''
 
     umetrics = []
     for c in set(y):
         Xc = X[y == c]
         d = 0
 
         for i in range(repeat):
             yc = (np.random.rand(len(Xc)) > 0.5).astype(int) # random assign y labels
-            _, new_dic = get_metrics(Xc, yc)
+            _, new_dic = get_metrics(Xc, yc, verbose=verbose)
             vec_metrics = []
             for key in keys:
-                vec_metrics.append(new_dic[key])
+                vec_metrics.append(new_dic[key] if key in new_dic else 0)
 
             vec_metrics = np.nan_to_num(vec_metrics,nan=0,posinf=1000,neginf=-1000)
 
             if method == 'meta.logistic' and isinstance(model, LogisticRegression):
                 d += model.predict_proba([vec_metrics.T])[0][1]
             elif method == 'decompose.pca' and isinstance(model, PCA):
                 M = vec_metrics.reshape(1,-1)
```

### Comparing `cla-2.0.2/cla/vis/confusion_matrix.py` & `cla-2.0.3/cla/vis/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/vis/feature_importance.py` & `cla-2.0.3/cla/vis/feature_importance.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/vis/plotComponents1D.py` & `cla-2.0.3/cla/vis/plotComponents1D.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/vis/plotComponents2D.py` & `cla-2.0.3/cla/vis/plotComponents2D.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/vis/plotComponents3D.py` & `cla-2.0.3/cla/vis/plotComponents3D.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla/vis/unsupervised_dimension_reductions.py` & `cla-2.0.3/cla/vis/unsupervised_dimension_reductions.py`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/cla.egg-info/PKG-INFO` & `cla-2.0.3/cla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 2.0.2
+Version: 2.0.3
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 2.0.2 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 2.0.3 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-2.0.2/cla.egg-info/SOURCES.txt` & `cla-2.0.3/cla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/data/sample.csv` & `cla-2.0.3/data/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-2.0.2/setup.py` & `cla-2.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 setup(
     # Application name:
     name="cla",
     
     # Version number (initial):
-    version="2.0.2",
+    version="2.0.3",
     
     # Application author details:
     author="Zhang",
     author_email="oo@zju.edu.cn",
     
     # Packages
     packages=["cla", "cla.vis", "cla.gui", "cla.gui.templates", "cla.gui.static"],
```

