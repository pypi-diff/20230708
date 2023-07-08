# Comparing `tmp/wcc-timetable-generator-0.1.0.tar.gz` & `tmp/wcc-timetable-generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcc-timetable-generator-0.1.0.tar", max compression
+gzip compressed data, was "wcc-timetable-generator-0.2.0.tar", max compression
```

## Comparing `wcc-timetable-generator-0.1.0.tar` & `wcc-timetable-generator-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rwxr-xr-x   0        0        0      669 2023-07-08 12:47:30.471058 wcc-timetable-generator-0.1.0/README.md
--rwxr-xr-x   0        0        0      302 2023-07-08 13:40:59.044638 wcc-timetable-generator-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-0.1.0/wcc_timetable_generator/__init__.py
--rwxr-xr-x   0        0        0     1705 2023-07-08 12:38:40.191165 wcc-timetable-generator-0.1.0/wcc_timetable_generator/algo.py
--rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-0.1.0/wcc_timetable_generator/subject_model.py
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.1.0/setup.py
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      669 2023-07-08 12:47:30.471058 wcc-timetable-generator-0.2.0/README.md
+-rwxr-xr-x   0        0        0      405 2023-07-08 16:56:58.927434 wcc-timetable-generator-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-0.2.0/wcc_timetable_generator/__init__.py
+-rwxr-xr-x   0        0        0       73 2023-07-08 16:55:35.366224 wcc-timetable-generator-0.2.0/wcc_timetable_generator/__main__.py
+-rwxr-xr-x   0        0        0     1705 2023-07-08 12:38:40.191165 wcc-timetable-generator-0.2.0/wcc_timetable_generator/algo.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-0.2.0/wcc_timetable_generator/components/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-0.2.0/wcc_timetable_generator/components/entry.py
+-rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-0.2.0/wcc_timetable_generator/subject_model.py
+-rwxr-xr-x   0        0        0      214 2023-07-08 16:45:51.394562 wcc-timetable-generator-0.2.0/wcc_timetable_generator/timetable.css
+-rwxr-xr-x   0        0        0     1289 2023-07-08 16:45:51.394991 wcc-timetable-generator-0.2.0/wcc_timetable_generator/timetable.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.0/setup.py
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.0/PKG-INFO
```

### Comparing `wcc-timetable-generator-0.1.0/README.md` & `wcc-timetable-generator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-0.1.0/wcc_timetable_generator/algo.py` & `wcc-timetable-generator-0.2.0/wcc_timetable_generator/algo.py`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-0.1.0/setup.py` & `wcc-timetable-generator-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['wcc_timetable_generator']
+['wcc_timetable_generator', 'wcc_timetable_generator.components']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['textual>=0.29.0,<0.30.0']
+
+entry_points = \
+{'console_scripts': ['generate-timetable = '
+                     'wcc_timetable_generator.__main__:main']}
+
 setup_kwargs = {
     'name': 'wcc-timetable-generator',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\n ### 🌐 Installation with PIP\n\n## 🖱 Usage\n\n## Roadmap\n- [x] Add the algorithm \n- [ ] Add GUI\n- [ ] Write tests\n- [ ] Publish to PyPI",
     'author': 'Tsierenana Bôtramanagna Gracy',
     'author_email': 'gtsierenana@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `wcc-timetable-generator-0.1.0/PKG-INFO` & `wcc-timetable-generator-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: wcc-timetable-generator
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Tsierenana Bôtramanagna Gracy
 Author-email: gtsierenana@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: textual (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 # Timetable 📊
 
 ## 📰 Description 
 A CLI tool that allow you to generate a timetable for your school or university such that : 
  - A subject can't be seen on two consecutive days
```

