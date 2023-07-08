# Comparing `tmp/q2report-0.1.28.tar.gz` & `tmp/q2report-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.28.tar", max compression
+gzip compressed data, was "q2report-0.1.29.tar", max compression
```

## Comparing `q2report-0.1.28.tar` & `q2report-0.1.29.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.28/LICENSE
--rw-r--r--   0        0        0      536 2023-06-28 16:26:52.084404 q2report-0.1.28/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.28/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.28/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.28/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.28/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.28/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8678 2023-06-21 10:36:17.872724 q2report-0.1.28/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.28/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18820 2023-06-28 08:23:20.140407 q2report-0.1.28/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.28/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20678 2023-06-21 17:49:55.953006 q2report-0.1.28/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.28/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    30045 2023-06-28 16:03:56.151488 q2report-0.1.28/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.28/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-06-28 16:26:54.663552 q2report-0.1.28/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.28/README.md
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.29/LICENSE
+-rw-r--r--   0        0        0      536 2023-07-08 21:36:37.928411 q2report-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.29/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.29/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8678 2023-06-21 10:36:17.872724 q2report-0.1.29/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.29/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18820 2023-06-28 08:23:20.140407 q2report-0.1.29/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.29/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20678 2023-06-21 17:49:55.953006 q2report-0.1.29/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.29/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    30080 2023-07-08 20:20:24.915617 q2report-0.1.29/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.29/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-07-08 21:36:40.175773 q2report-0.1.29/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.29/README.md
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.29/PKG-INFO
```

### Comparing `q2report-0.1.28/LICENSE` & `q2report-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/pyproject.toml` & `q2report-0.1.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.28"
+version = "0.1.29"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pillow = "^9.4.0"
```

### Comparing `q2report-0.1.28/q2report/q2printer/docx_parts.py` & `q2report-0.1.29/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2printer/q2printer.py` & `q2report-0.1.29/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.29/q2report/q2printer/q2printer_docx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2printer/q2printer_html.py` & `q2report-0.1.29/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.29/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.29/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/q2report/q2report.py` & `q2report-0.1.29/q2report/q2report.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,16 @@
         rows.set_cell(row, col, data, style, rowspan, colspan, format, name)
         return rows
 
     def load(self, content):
         if os.path.isfile(content):
             self.report_content = json.load(open(content))
         else:
-            self.report_content = json.loads(content)
+            if content != "":
+                self.report_content = json.loads(content)
         self.params = self.report_content.get("params", {})
 
     def data_start(self):
         self.current_data_set_row_number = 0
 
     def data_step(self):
         self.current_data_set_row_number += 1
```

### Comparing `q2report-0.1.28/q2report/q2utils.py` & `q2report-0.1.29/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/README.md` & `q2report-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.28/PKG-INFO` & `q2report-0.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.28
+Version: 0.1.29
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

