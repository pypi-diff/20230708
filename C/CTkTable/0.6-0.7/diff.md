# Comparing `tmp/CTkTable-0.6.tar.gz` & `tmp/CTkTable-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkTable-0.6.tar", last modified: Tue Jun 27 06:10:13 2023, max compression
+gzip compressed data, was "CTkTable-0.7.tar", last modified: Sat Jul  8 13:20:53 2023, max compression
```

## Comparing `CTkTable-0.6.tar` & `CTkTable-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.703554 CTkTable-0.6/
-drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.687886 CTkTable-0.6/CTkTable/
--rw-rw-rw-   0        0        0      227 2023-06-27 06:09:31.000000 CTkTable-0.6/CTkTable/__init__.py
--rw-rw-rw-   0        0        0    13103 2023-06-27 06:06:40.000000 CTkTable-0.6/CTkTable/ctktable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.703554 CTkTable-0.6/CTkTable.egg-info/
--rw-rw-rw-   0        0        0     3348 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.6/LICENSE
--rw-rw-rw-   0        0        0     3348 2023-06-27 06:10:13.703554 CTkTable-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2762 2023-06-22 11:03:43.000000 CTkTable-0.6/README.md
--rw-rw-rw-   0        0        0      519 2023-06-27 06:10:13.719180 CTkTable-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-06-27 06:09:44.000000 CTkTable-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.187162 CTkTable-0.7/
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.161012 CTkTable-0.7/CTkTable/
+-rw-rw-rw-   0        0        0      227 2023-07-08 13:07:10.000000 CTkTable-0.7/CTkTable/__init__.py
+-rw-rw-rw-   0        0        0    16386 2023-07-08 13:06:29.000000 CTkTable-0.7/CTkTable/ctktable.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:53.187162 CTkTable-0.7/CTkTable.egg-info/
+-rw-rw-rw-   0        0        0     3960 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:20:53.000000 CTkTable-0.7/CTkTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.7/LICENSE
+-rw-rw-rw-   0        0        0     3960 2023-07-08 13:20:53.187162 CTkTable-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3363 2023-07-08 13:20:33.000000 CTkTable-0.7/README.md
+-rw-rw-rw-   0        0        0      519 2023-07-08 13:20:53.187162 CTkTable-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-07-08 13:07:27.000000 CTkTable-0.7/setup.py
```

### Comparing `CTkTable-0.6/CTkTable.egg-info/PKG-INFO` & `CTkTable-0.7/CTkTable.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.6
+Version: 0.7
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -57,20 +57,30 @@
 ```
 
 ## Methods
 - **.add_row(index, values)**
 - **.add_column(index, values)**
 - **.edit_row(row_num, *args)**: edit one full row at once
 - **.edit_column(column_num, *args)**: edit one full column at once
-- **.delete_row(index)**
-- **.delete_column(index)**
+- **.delete_row(index)**: remove one row
+- **.delete_column(index)**: remove one column
+- **.delete_rows(indices)**: remove mutliple rows
+- **.delete_columns(indices)**: remove multiple columns
+- **.select(row, column)**: select one cell
+- **.select_row(row)**: select a row
+- **.deselect_row(row)**: deselect a row
+- **.select_column(column)**: select a column
+- **.deselect_column(column)**: deselect a column
 - **.update_values(values)**: update all values at once
 - **.insert(row, column, value, *args)**: change specific index data
 - **.delete(row, column, *args)**: delete the data from specific index
 - **.get()**: get all values
+- **.get(row, column)**: get specific cell value
+- **.get_row(row)**: get all values of a specific row
+- **.get_column(column)**: get all values of a specific column
 - **.configure(arguments)**: change other table attributes
 
 _here, **args** means ctkbutton parameters which can also be passed_
 
 **Note: treat all the table cells as a ctkbutton class**
 
 ## Arguments
@@ -80,14 +90,15 @@
 | **values** | the default values for table |
 | row | **optional**, set number of default rows |
 | column | **optional**, set number of default columns |
 | padx | add internal padding in x |
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
+| orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues.
```

### Comparing `CTkTable-0.6/LICENSE` & `CTkTable-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkTable-0.6/PKG-INFO` & `CTkTable-0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.6
+Version: 0.7
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -57,20 +57,30 @@
 ```
 
 ## Methods
 - **.add_row(index, values)**
 - **.add_column(index, values)**
 - **.edit_row(row_num, *args)**: edit one full row at once
 - **.edit_column(column_num, *args)**: edit one full column at once
-- **.delete_row(index)**
-- **.delete_column(index)**
+- **.delete_row(index)**: remove one row
+- **.delete_column(index)**: remove one column
+- **.delete_rows(indices)**: remove mutliple rows
+- **.delete_columns(indices)**: remove multiple columns
+- **.select(row, column)**: select one cell
+- **.select_row(row)**: select a row
+- **.deselect_row(row)**: deselect a row
+- **.select_column(column)**: select a column
+- **.deselect_column(column)**: deselect a column
 - **.update_values(values)**: update all values at once
 - **.insert(row, column, value, *args)**: change specific index data
 - **.delete(row, column, *args)**: delete the data from specific index
 - **.get()**: get all values
+- **.get(row, column)**: get specific cell value
+- **.get_row(row)**: get all values of a specific row
+- **.get_column(column)**: get all values of a specific column
 - **.configure(arguments)**: change other table attributes
 
 _here, **args** means ctkbutton parameters which can also be passed_
 
 **Note: treat all the table cells as a ctkbutton class**
 
 ## Arguments
@@ -80,14 +90,15 @@
 | **values** | the default values for table |
 | row | **optional**, set number of default rows |
 | column | **optional**, set number of default columns |
 | padx | add internal padding in x |
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
+| orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues.
```

### Comparing `CTkTable-0.6/README.md` & `CTkTable-0.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -42,20 +42,30 @@
 ```
 
 ## Methods
 - **.add_row(index, values)**
 - **.add_column(index, values)**
 - **.edit_row(row_num, *args)**: edit one full row at once
 - **.edit_column(column_num, *args)**: edit one full column at once
-- **.delete_row(index)**
-- **.delete_column(index)**
+- **.delete_row(index)**: remove one row
+- **.delete_column(index)**: remove one column
+- **.delete_rows(indices)**: remove mutliple rows
+- **.delete_columns(indices)**: remove multiple columns
+- **.select(row, column)**: select one cell
+- **.select_row(row)**: select a row
+- **.deselect_row(row)**: deselect a row
+- **.select_column(column)**: select a column
+- **.deselect_column(column)**: deselect a column
 - **.update_values(values)**: update all values at once
 - **.insert(row, column, value, *args)**: change specific index data
 - **.delete(row, column, *args)**: delete the data from specific index
 - **.get()**: get all values
+- **.get(row, column)**: get specific cell value
+- **.get_row(row)**: get all values of a specific row
+- **.get_column(column)**: get all values of a specific column
 - **.configure(arguments)**: change other table attributes
 
 _here, **args** means ctkbutton parameters which can also be passed_
 
 **Note: treat all the table cells as a ctkbutton class**
 
 ## Arguments
@@ -65,14 +75,15 @@
 | **values** | the default values for table |
 | row | **optional**, set number of default rows |
 | column | **optional**, set number of default columns |
 | padx | add internal padding in x |
 | pady | add internal padding in y |
 | colors | set two fg_colors for the table (list), eg: `colors=["yellow", "green"]` |
 | color_phase | set color phase based on rows or columns, eg: `color_phase="vertical"` |
+| orientation | change the orientation of table, `vertical or horizontal` |
 | header_color | define the topmost row color |
 | corner_radius | define the corner roundness of the table |
 | hover_color | enable hover effect on the cells |
 | **command** | specify a command when a table cell is pressed, [returns row, column, value] |
 | **other button parameters* | all other ctk button parameters can be passed |
 
 Note: This library is at early stage so there can be some performance issues.
```

### Comparing `CTkTable-0.6/setup.cfg` & `CTkTable-0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 5461 626c 650d 0a76 6572   = CTkTable..ver
-00000020: 7369 6f6e 203d 2030 2e36 0d0a 6465 7363  sion = 0.6..desc
+00000020: 7369 6f6e 203d 2030 2e37 0d0a 6465 7363  sion = 0.7..desc
 00000030: 7269 7074 696f 6e20 3d20 4375 7374 6f6d  ription = Custom
 00000040: 746b 696e 7465 7220 5461 626c 6520 7769  tkinter Table wi
 00000050: 6467 6574 0d0a 6c6f 6e67 5f64 6573 6372  dget..long_descr
 00000060: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000070: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000080: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 00000090: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
```

### Comparing `CTkTable-0.6/setup.py` & `CTkTable-0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkTable',
-    version = '0.6',
+    version = '0.7',
     description = "Customtkinter Table widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkTable",
```

