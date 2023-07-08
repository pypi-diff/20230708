# Comparing `tmp/task2a-1.0.3.tar.gz` & `tmp/task2a-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.3.tar", max compression
+gzip compressed data, was "task2a-1.0.4.tar", max compression
```

## Comparing `task2a-1.0.3.tar` & `task2a-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:00:47.124418 task2a-1.0.3/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.3/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.3/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-08 14:16:02.463794 task2a-1.0.3/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.3/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.3/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.3/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8361 2023-07-07 02:48:43.373616 task2a-1.0.3/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    19900 2023-07-07 02:48:43.375617 task2a-1.0.3/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      464 2023-07-08 14:16:02.458793 task2a-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    36970 2023-07-08 14:11:17.636090 task2a-1.0.3/README.md
--rw-r--r--   0        0        0    36772 1970-01-01 00:00:00.000000 task2a-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.4/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.4/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.4/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-08 14:32:13.099683 task2a-1.0.4/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.4/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.4/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.4/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8361 2023-07-07 02:48:43.373616 task2a-1.0.4/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.4/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.4/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.4/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.4/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    19900 2023-07-07 02:48:43.375617 task2a-1.0.4/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      464 2023-07-08 14:32:08.013686 task2a-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    37394 2023-07-08 14:45:47.894091 task2a-1.0.4/README.md
+-rw-r--r--   0        0        0    37191 1970-01-01 00:00:00.000000 task2a-1.0.4/PKG-INFO
```

### Comparing `task2a-1.0.3/pwgen/cli/cli.py` & `task2a-1.0.4/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.3/pwgen/pwgen.py` & `task2a-1.0.4/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.3/pwgen/showcase/showcase.py` & `task2a-1.0.4/pwgen/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.3/README.md` & `task2a-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 
 <h1 align="center">
   <div align="center" aria-colspan="0">Password generator.</div>
   <div align="center" aria-colspan="0">Module 2: Python. Task 2A.</div>
 </h1>
 
 <p align="center">
-  <a href="https://pypi.org/project/task2a/">
-    <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge" alt="PYPI v." />
-  </a>&nbsp;
-  <a href="https://www.python.org/downloads/">
-    <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
-  </a>&nbsp;
-  <a href="https://discord.gg/angular">
-    <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
-  </a>
+  <div align="center">
+    <a href="https://pypi.org/project/task2a/">
+      <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge&label=task 2a" alt="PYPI v." />
+    </a>&nbsp;
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
+      <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
+    </a>&nbsp;
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
+      <img src="https://img.shields.io/pypi/v/poetry.svg?style=for-the-badge&label=poetry&color=green" alt="License" />
+    </a>&nbsp;
+    <a href="https://www.python.org/downloads/">
+      <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
+    </a>&nbsp;
+  </div>
 </p>
 
 
 ## Preface
 
 This project contains a solution to one of the tasks of the EPAM DevOps Initial Internal Training Course #7 in 2023.
 Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
-                       [PYPI_v.]  [Python_v.]  [License]
+                 [PYPI_v.]  [License]  [License]  [Python_v.] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
 one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-
 avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
 raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
 12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
```

### Comparing `task2a-1.0.3/PKG-INFO` & `task2a-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,23 +21,28 @@
 
 <h1 align="center">
   <div align="center" aria-colspan="0">Password generator.</div>
   <div align="center" aria-colspan="0">Module 2: Python. Task 2A.</div>
 </h1>
 
 <p align="center">
-  <a href="https://pypi.org/project/task2a/">
-    <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge" alt="PYPI v." />
-  </a>&nbsp;
-  <a href="https://www.python.org/downloads/">
-    <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
-  </a>&nbsp;
-  <a href="https://discord.gg/angular">
-    <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
-  </a>
+  <div align="center">
+    <a href="https://pypi.org/project/task2a/">
+      <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge&label=task 2a" alt="PYPI v." />
+    </a>&nbsp;
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
+      <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
+    </a>&nbsp;
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
+      <img src="https://img.shields.io/pypi/v/poetry.svg?style=for-the-badge&label=poetry&color=green" alt="License" />
+    </a>&nbsp;
+    <a href="https://www.python.org/downloads/">
+      <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
+    </a>&nbsp;
+  </div>
 </p>
 
 
 ## Preface
 
 This project contains a solution to one of the tasks of the EPAM DevOps Initial Internal Training Course #7 in 2023.
 Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.3 Summary: License: MIT Author:
+Metadata-Version: 2.1 Name: task2a Version: 1.0.4 Summary: License: MIT Author:
 Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
-                       [PYPI_v.]  [Python_v.]  [License]
+                 [PYPI_v.]  [License]  [License]  [Python_v.] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
 one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-
 avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
 raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
 12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
```

