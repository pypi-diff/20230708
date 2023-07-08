# Comparing `tmp/KapoorLabs-Lightning-5.2.8.tar.gz` & `tmp/KapoorLabs-Lightning-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-_2ewdrnv/KapoorLabs-Lightning-5.2.8.tar", last modified: Mon Jun 12 13:18:56 2023, max compression
+gzip compressed data, was "KapoorLabs-Lightning-5.3.0.tar", last modified: Sat Jul  8 08:59:02 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.2.8.tar` & `KapoorLabs-Lightning-5.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:56.355449 KapoorLabs-Lightning-5.2.8/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:55.237306 KapoorLabs-Lightning-5.2.8/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:55.493219 KapoorLabs-Lightning-5.2.8/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.8/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.8/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-12 13:18:56.356450 KapoorLabs-Lightning-5.2.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:55.705497 KapoorLabs-Lightning-5.2.8/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-12 13:18:56.362448 KapoorLabs-Lightning-5.2.8/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:55.260166 KapoorLabs-Lightning-5.2.8/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:55.912143 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-12 13:18:54.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-12 13:18:55.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 13:18:54.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-12 13:18:54.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-12 13:18:54.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-12 13:18:54.000000 KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:56.267405 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 13:18:56.325143 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-12 13:18:53.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35200 2023-06-12 13:18:17.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.8/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:02.016022 KapoorLabs-Lightning-5.3.0/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:00.567348 KapoorLabs-Lightning-5.3.0/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:00.812243 KapoorLabs-Lightning-5.3.0/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.3.0/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.3.0/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-07-08 08:59:02.017030 KapoorLabs-Lightning-5.3.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:01.044033 KapoorLabs-Lightning-5.3.0/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1745 2023-07-08 08:59:02.025567 KapoorLabs-Lightning-5.3.0/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:00.589684 KapoorLabs-Lightning-5.3.0/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:01.283722 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-07-08 08:59:00.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       97 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:01.859662 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 08:59:01.963995 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-07-08 08:58:58.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35120 2023-07-03 19:36:03.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.3.0/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.2.8/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.3.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/.gitignore` & `KapoorLabs-Lightning-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/LICENSE` & `KapoorLabs-Lightning-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/PKG-INFO` & `KapoorLabs-Lightning-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.8
+Version: 5.3.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.8/README.md` & `KapoorLabs-Lightning-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/Apache-2` & `KapoorLabs-Lightning-5.3.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/BSD-3` & `KapoorLabs-Lightning-5.3.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/GPL-3` & `KapoorLabs-Lightning-5.3.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/LGPL-3` & `KapoorLabs-Lightning-5.3.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/MIT` & `KapoorLabs-Lightning-5.3.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/licenses/MPL-2` & `KapoorLabs-Lightning-5.3.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/setup.cfg` & `KapoorLabs-Lightning-5.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 	numpy
 	torch
 	torchvision
 	lightning
 	h5py
 	tox
 	pytest-cov
+	pyntcloud
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
```

### Comparing `KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.8
+Version: 5.3.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.3.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from typing import Any, List
 
 import torch
 import torch.nn.functional as F
 from lightning import Callback, LightningDataModule, LightningModule, Trainer
 from lightning.pytorch.loggers.logger import Logger
-from lightning.pytorch.utilities.types import STEP_OUTPUT
 from sklearn.cluster import KMeans
 from torch import optim
 from torch.utils.data import DataLoader, Dataset, random_split
 
 from . import optimizers, schedulers
 from .pytorch_models import CloudAutoEncoder, DeepEmbeddedClustering
 
@@ -619,15 +618,15 @@
         self.predictions = self.predictions.to(self.compute_device)
 
         return self.cluster_distribution
 
     def forward(self, z):
         return self.network(z)
 
-    def predict_step(self, batch, batch_idx) -> STEP_OUTPUT | None:
+    def predict_step(self, batch, batch_idx):
         return self(batch)
 
     def configure_optimizers(self):
         optimizer = self.optim_func(self.parameters())
 
         return {"optimizer": optimizer}
```

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.3.0/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.8/tox.ini` & `KapoorLabs-Lightning-5.3.0/tox.ini`

 * *Files identical despite different names*

