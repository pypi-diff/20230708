# Comparing `tmp/AnnoMate-0.0.0.tar.gz` & `tmp/AnnoMate-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnnoMate-0.0.0.tar", last modified: Mon Jun 26 17:45:07 2023, max compression
+gzip compressed data, was "dist/AnnoMate-0.0.1.tar", last modified: Fri Jul  7 22:49:09 2023, max compression
```

## Comparing `AnnoMate-0.0.0.tar` & `AnnoMate-0.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.202668 AnnoMate-0.0.0/
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.191806 AnnoMate-0.0.0/AnnoMate/
--rw-r--r--   0 cchu       (502) staff       (20)     4567 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/AnnotationDisplayComponent.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.192297 AnnoMate-0.0.0/AnnoMate/AnnotationDisplayComponents/
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/AnnotationDisplayComponents/__init__.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.197621 AnnoMate-0.0.0/AnnoMate/AppComponents/
--rw-r--r--   0 cchu       (502) staff       (20)    15160 2023-06-26 17:06:39.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/CNVPlotComponent.py
--rw-r--r--   0 cchu       (502) staff       (20)     2972 2023-06-26 17:06:48.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/DataTableComponents.py
--rw-r--r--   0 cchu       (502) staff       (20)    19646 2023-06-26 17:06:52.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/MutationTableComponent.py
--rw-r--r--   0 cchu       (502) staff       (20)    27892 2023-06-26 17:06:56.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/PhylogicComponents.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)     4963 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/AppComponents/utils.py
--rw-r--r--   0 cchu       (502) staff       (20)     4364 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/Data.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.199684 AnnoMate-0.0.0/AnnoMate/DataTypes/
--rw-r--r--   0 cchu       (502) staff       (20)     1101 2023-06-26 17:06:21.000000 AnnoMate-0.0.0/AnnoMate/DataTypes/GenericData.py
--rw-r--r--   0 cchu       (502) staff       (20)      885 2023-06-26 17:06:24.000000 AnnoMate-0.0.0/AnnoMate/DataTypes/PatientSampleData.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/DataTypes/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)    47314 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/ReviewDataApp.py
--rw-r--r--   0 cchu       (502) staff       (20)     7395 2023-06-26 17:05:52.000000 AnnoMate-0.0.0/AnnoMate/ReviewDataInterface.py
--rw-r--r--   0 cchu       (502) staff       (20)    18501 2023-06-26 17:05:56.000000 AnnoMate-0.0.0/AnnoMate/ReviewerTemplate.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.200671 AnnoMate-0.0.0/AnnoMate/Reviewers/
--rw-r--r--   0 cchu       (502) staff       (20)     5770 2023-06-26 17:06:12.000000 AnnoMate-0.0.0/AnnoMate/Reviewers/ExampleReviewer.py
--rw-r--r--   0 cchu       (502) staff       (20)       43 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/Reviewers/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/AnnoMate/__init__.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-06-26 17:45:07.202395 AnnoMate-0.0.0/AnnoMate.egg-info/
--rw-r--r--   0 cchu       (502) staff       (20)     5783 2023-06-26 17:45:06.000000 AnnoMate-0.0.0/AnnoMate.egg-info/PKG-INFO
--rw-r--r--   0 cchu       (502) staff       (20)      887 2023-06-26 17:45:07.000000 AnnoMate-0.0.0/AnnoMate.egg-info/SOURCES.txt
--rw-r--r--   0 cchu       (502) staff       (20)        1 2023-06-26 17:45:06.000000 AnnoMate-0.0.0/AnnoMate.egg-info/dependency_links.txt
--rw-r--r--   0 cchu       (502) staff       (20)      259 2023-06-26 17:45:07.000000 AnnoMate-0.0.0/AnnoMate.egg-info/requires.txt
--rw-r--r--   0 cchu       (502) staff       (20)        9 2023-06-26 17:45:07.000000 AnnoMate-0.0.0/AnnoMate.egg-info/top_level.txt
--rw-r--r--   0 cchu       (502) staff       (20)     1074 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/LICENSE.txt
--rw-r--r--   0 cchu       (502) staff       (20)     5783 2023-06-26 17:45:07.202811 AnnoMate-0.0.0/PKG-INFO
--rw-r--r--   0 cchu       (502) staff       (20)     5221 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/README.md
--rw-r--r--   0 cchu       (502) staff       (20)       86 2023-06-26 16:14:26.000000 AnnoMate-0.0.0/pyproject.toml
--rw-r--r--   0 cchu       (502) staff       (20)       79 2023-06-26 17:45:07.203267 AnnoMate-0.0.0/setup.cfg
--rw-r--r--   0 cchu       (502) staff       (20)     1983 2023-06-26 17:43:58.000000 AnnoMate-0.0.0/setup.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.791458 AnnoMate-0.0.1/
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.782002 AnnoMate-0.0.1/AnnoMate/
+-rw-r--r--   0 cchu       (502) staff       (20)     4567 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AnnotationDisplayComponent.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.782395 AnnoMate-0.0.1/AnnoMate/AnnotationDisplayComponents/
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AnnotationDisplayComponents/__init__.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.786339 AnnoMate-0.0.1/AnnoMate/AppComponents/
+-rw-r--r--   0 cchu       (502) staff       (20)    15160 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/CNVPlotComponent.py
+-rw-r--r--   0 cchu       (502) staff       (20)     2972 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/DataTableComponents.py
+-rw-r--r--   0 cchu       (502) staff       (20)    19646 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/MutationTableComponent.py
+-rw-r--r--   0 cchu       (502) staff       (20)    27892 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/PhylogicComponents.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)     4963 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/AppComponents/utils.py
+-rw-r--r--   0 cchu       (502) staff       (20)     4364 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/Data.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.788070 AnnoMate-0.0.1/AnnoMate/DataTypes/
+-rw-r--r--   0 cchu       (502) staff       (20)     1101 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/DataTypes/GenericData.py
+-rw-r--r--   0 cchu       (502) staff       (20)      885 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/DataTypes/PatientSampleData.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/DataTypes/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)    48376 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/ReviewDataApp.py
+-rw-r--r--   0 cchu       (502) staff       (20)     7395 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/ReviewDataInterface.py
+-rw-r--r--   0 cchu       (502) staff       (20)    18501 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/ReviewerTemplate.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.788968 AnnoMate-0.0.1/AnnoMate/Reviewers/
+-rw-r--r--   0 cchu       (502) staff       (20)     5770 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/Reviewers/ExampleReviewer.py
+-rw-r--r--   0 cchu       (502) staff       (20)       43 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/Reviewers/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/AnnoMate/__init__.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2023-07-07 22:49:09.791107 AnnoMate-0.0.1/AnnoMate.egg-info/
+-rw-r--r--   0 cchu       (502) staff       (20)     5746 2023-07-07 22:49:09.000000 AnnoMate-0.0.1/AnnoMate.egg-info/PKG-INFO
+-rw-r--r--   0 cchu       (502) staff       (20)      887 2023-07-07 22:49:09.000000 AnnoMate-0.0.1/AnnoMate.egg-info/SOURCES.txt
+-rw-r--r--   0 cchu       (502) staff       (20)        1 2023-07-07 22:49:09.000000 AnnoMate-0.0.1/AnnoMate.egg-info/dependency_links.txt
+-rw-r--r--   0 cchu       (502) staff       (20)      269 2023-07-07 22:49:09.000000 AnnoMate-0.0.1/AnnoMate.egg-info/requires.txt
+-rw-r--r--   0 cchu       (502) staff       (20)        9 2023-07-07 22:49:09.000000 AnnoMate-0.0.1/AnnoMate.egg-info/top_level.txt
+-rw-r--r--   0 cchu       (502) staff       (20)     1074 2023-06-26 16:14:26.000000 AnnoMate-0.0.1/LICENSE.txt
+-rw-r--r--   0 cchu       (502) staff       (20)     5746 2023-07-07 22:49:09.791612 AnnoMate-0.0.1/PKG-INFO
+-rw-r--r--   0 cchu       (502) staff       (20)     5221 2023-06-26 16:14:26.000000 AnnoMate-0.0.1/README.md
+-rw-r--r--   0 cchu       (502) staff       (20)       86 2023-06-26 16:14:26.000000 AnnoMate-0.0.1/pyproject.toml
+-rw-r--r--   0 cchu       (502) staff       (20)       79 2023-07-07 22:49:09.792337 AnnoMate-0.0.1/setup.cfg
+-rw-r--r--   0 cchu       (502) staff       (20)     1966 2023-07-07 22:14:15.000000 AnnoMate-0.0.1/setup.py
```

### Comparing `AnnoMate-0.0.0/AnnoMate/AnnotationDisplayComponent.py` & `AnnoMate-0.0.1/AnnoMate/AnnotationDisplayComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/AppComponents/CNVPlotComponent.py` & `AnnoMate-0.0.1/AnnoMate/AppComponents/CNVPlotComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/AppComponents/DataTableComponents.py` & `AnnoMate-0.0.1/AnnoMate/AppComponents/DataTableComponents.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/AppComponents/MutationTableComponent.py` & `AnnoMate-0.0.1/AnnoMate/AppComponents/MutationTableComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/AppComponents/PhylogicComponents.py` & `AnnoMate-0.0.1/AnnoMate/AppComponents/PhylogicComponents.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/AppComponents/utils.py` & `AnnoMate-0.0.1/AnnoMate/AppComponents/utils.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/Data.py` & `AnnoMate-0.0.1/AnnoMate/Data.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/DataTypes/GenericData.py` & `AnnoMate-0.0.1/AnnoMate/DataTypes/GenericData.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/DataTypes/PatientSampleData.py` & `AnnoMate-0.0.1/AnnoMate/DataTypes/PatientSampleData.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/ReviewDataApp.py` & `AnnoMate-0.0.1/AnnoMate/ReviewDataApp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 import numpy as np
-from jupyter_dash import JupyterDash
+# from jupyter_dash import JupyterDash
+from dash import jupyter_dash
 from dash import dcc
-from dash import html
+from dash import html, Dash
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash
 import dash_bootstrap_components as dbc
 import inspect
 from collections import OrderedDict
 from typing import Dict
@@ -104,17 +105,37 @@
 
         use_name_as_title: bool
             use the `name` parameter as a title for the component.
         """
         
         all_ids = np.array(get_component_ids(layout))
         check_duplicates(all_ids, 'component')
-        
-        check_duplicate_objects(callback_output, 'callback_output_objects')
-        callback_output_ids = get_callback_io_ids(callback_output, expected_io_type=Output)
+
+        # preprocess callback_output to include allow_duplicate=True
+        if isinstance(callback_output, list):
+            new_callback_output = [
+                Output(**{
+                    'component_id': output.component_id, 
+                    'component_property': output.component_property, 
+                    'allow_duplicate': True
+                }) for output in callback_output
+            ]  
+        elif isinstance(callback_output, dict):
+            new_callback_output = {
+                k: Output(**{
+                    'component_id': output.component_id, 
+                    'component_property': output.component_property, 
+                    'allow_duplicate': True
+                }) for k, output in callback_output.items()
+            }
+        else:
+            raise ValueError(f'callback output {callback_output} is neither a list or a dictionary.')
+
+        check_duplicate_objects(new_callback_output, 'callback_output_objects')
+        callback_output_ids = get_callback_io_ids(new_callback_output, expected_io_type=Output)
         check_callback_io_id_in_list(callback_output_ids, all_ids, ids_type='output_ids', all_ids_type='component_ids')
         
         check_duplicate_objects(callback_input, 'callback_input_objects')
         callback_input_ids = get_callback_io_ids(callback_input, expected_io_type=Input)
         check_callback_io_id_in_list(callback_input_ids, all_ids, ids_type='input_ids', all_ids_type='component_ids')
         
         check_duplicate_objects(callback_state, 'callback_state_objects')
@@ -130,15 +151,15 @@
         self.name = name
         if use_name_as_title:
             self.layout = html.Div([html.H1(name), html.Div(layout)])
         else:
             self.layout = html.Div(layout)
             
         self.all_component_ids = all_ids
-        self.callback_output = callback_output
+        self.callback_output = new_callback_output
         self.callback_input = callback_input
         self.callback_state = callback_state
         self.callback_state_external = callback_state_external
         
         self.new_data_callback = new_data_callback
         self.internal_callback = internal_callback
 
@@ -155,38 +176,39 @@
     def columns_to_string(self, df, columns):
         new_df = df.copy()
         for c in columns:
             new_df[c] = new_df[c].astype(str)
 
         return new_df
         
-    def run(self,
-            review_data: ReviewDataInterface,
-            annot_app_display_types_dict: Dict = None,
-            autofill_dict: Dict = None,
-            review_data_table_df: pd.DataFrame = None,
-            review_data_table_page_size: int = 10,
-            collapsable=True,
-            auto_export: bool = True,
-            auto_export_path: Union[Path, str] = None, 
-            attributes_to_export: List = ['annot_df', 'history_df'],
-            mode='external',
-            host='0.0.0.0',
-            port=8050,
-           ):
+    def run(
+        self,
+        review_data: ReviewDataInterface,
+        annot_app_display_types_dict: Dict = None,
+        autofill_dict: Dict = None,
+        review_data_table_df: pd.DataFrame = None,
+        review_data_table_page_size: int = 10,
+        collapsable=True,
+        auto_export: bool = True,
+        auto_export_path: Union[Path, str] = None, 
+        attributes_to_export: List = ['annot_df', 'history_df'],
+        mode='external',
+        host='0.0.0.0',
+        port=8050,
+    ):
 
         """
         Run the app
 
         Parameters
         ----------
         review_data: ReviewDataInterface
             ReviewData object to review with the app
 
-        mode: {'inline', 'external'}
+        mode: {'inline', 'external', 'tab'}
             How to display the dashboard
 
         host: str
             Host address
 
         port: int
             Port access number
@@ -229,15 +251,16 @@
             filtered_history_df = review_data.data.history_df.loc[
                 review_data.data.history_df['index'] == subject_index_value
             ].loc[::-1]
             
             return self.columns_to_string(filtered_history_df, multi_type_columns)
         
         
-        app = JupyterDash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
+        # app = JupyterDash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
+        app = Dash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
         
         reviewed_data_df = pd.DataFrame(index=review_data.data.index, columns=['label'])
         reviewed_data_df['label'] = reviewed_data_df.apply(lambda r: self.gen_dropdown_labels(review_data, r), 
                                                            axis=1)
         reviewed_data_df.index.name = 'value'
         
         app.layout, annotation_panel_component, autofill_buttons, gen_autofill_states, autofill_literals = \
@@ -260,221 +283,383 @@
                 print(f'Setting auto_export_path to {auto_export_path}')
             if not os.path.exists(auto_export_path):
                 print(f'Making directory {auto_export_path} for auto exporting.')
                 os.mkdir(auto_export_path)
             
             print(f'Using {auto_export_path} for auto exporting.')
         
-        def validate_callback_outputs(component_output, 
-                                      component, 
-                                      which_callback='callback function(s)'):
+        def validate_callback_outputs(
+            component_output, 
+            component, 
+            which_callback='callback function(s)'
+        ):
             if not isinstance(component_output, list) or (len(component.callback_output) != len(component_output)):
-                raise ValueError(f'Component ({component.name}) {which_callback} does not return '
-                                 'the same length output as component\'s callback_output.\n'
-                                 'Make sure your output from the callback function is a list, '
-                                 'and the values correspond to your defined callback_outputs list\n'
-                                 f'Expected output: {component.callback_output}\n'
-                                 f'Runtime callback output: {component_output}\n')
+                raise ValueError(
+                    f'Component ({component.name}) {which_callback} does not return '
+                     'the same length output as component\'s callback_output.\n'
+                     'Make sure your output from the callback function is a list, '
+                     'and the values correspond to your defined callback_outputs list\n'
+                     f'Expected output: {component.callback_output}\n'
+                     f'Runtime callback output: {component_output}\n'
+                )
             return
-        
-        @app.callback(output=dict(history_table=Output(f'APP-history-table', 'data'),
-                                  annot_panel=annotation_panel_component.callback_output,
-                                  dropdown_list_options=Output(f'APP-dropdown-data-state', 'options'),
-                                  dropdown_value=Output('APP-dropdown-data-state', 'value'),
-                                  review_data_selected_value=Output('APP-review-data-table', 'selected_rows'),
-                                  review_data_page_current=Output('APP-review-data-table', 'page_current'),
-                                  review_data_table_data=Output('APP-review-data-table', 'data'),
-                                  history_table_selected_row_state=Output('APP-history-table', 'selected_rows'),
-                                  more_component_outputs={c.name: c.callback_output for c_name, c in
-                                                          self.more_components.items()}),
-                      inputs=dict(dropdown_value=Input('APP-dropdown-data-state', 'value'),
-                                  review_data_selected_value=Input('APP-review-data-table', 'selected_rows'),
-                                  review_data_table_state=State('APP-review-data-table', 'data'),
-                                  review_data_table_derived_virtual_data_state=State('APP-review-data-table', 'derived_virtual_data'),
-                                  autofill_buttons=[Input(b.id, 'n_clicks') for b in autofill_buttons],
-                                  autofill_states=gen_autofill_states,
-                                  submit_annot_button=Input('APP-submit-button-state', 'n_clicks'),
-                                  annot_input_state=annotation_panel_component.callback_state,
-                                  revert_annot_button=Input('APP-revert-annot-button', 'n_clicks'),
-                                  history_table_selected_row_state=State('APP-history-table', 'selected_rows'),
-                                  clear_annot_button=Input('APP-clear-annot-button', 'n_clicks'),
-                                  more_component_inputs={
-                                      c.name: c.callback_input + c.callback_state + c.callback_state_external for
-                                      c_name, c in
-                                      self.more_components.items()}))
-        def component_callback(dropdown_value,
-                               review_data_selected_value,
-                               review_data_table_state, # full data table
-                               review_data_table_derived_virtual_data_state,  # what is currently displayed
-                               autofill_buttons,
-                               autofill_states,
-                               submit_annot_button, 
-                               annot_input_state, 
-                               revert_annot_button,
-                               history_table_selected_row_state,
-                               clear_annot_button,
-                               more_component_inputs):
-            
-            ctx = dash.callback_context
-            if not ctx.triggered:
-                raise PreventUpdate
+
+        more_component_inputs = {
+            c.name: c.callback_input + c.callback_state + c.callback_state_external for c_name, c in self.more_components.items()
+        }
+
+        more_component_inputs_as_states = {
+            c_name: [
+                State(**{'component_id': c.component_id, 'component_property': c.component_property}) for c in c_list
+            ] for c_name, c_list in more_component_inputs.items()
+        }
+
+        more_component_outputs = {c.name: c.callback_output for c_name, c in self.more_components.items()}
+               
+        def update_components(output_dict, subject_index_value, more_component_inputs_as_states):
+            output_dict['more_component_outputs'] = {
+                c.name: list(np.full(len(c.callback_output), dash.no_update)) for c_name, c in self.more_components.items()
+            }
+            
+            for c_name, component in self.more_components.items():
+                if component.new_data_callback is not None:
+                    component_output = component.new_data_callback(
+                        review_data.data,
+                        subject_index_value,
+                        *more_component_inputs_as_states[component.name]
+                    )
+                    validate_callback_outputs(component_output, component, which_callback='new_data_callback')
+                    output_dict['more_component_outputs'][component.name] = component_output
+            
+            history_df = get_history_display_table(subject_index_value)
+            output_dict['history_table'] = history_df.to_dict('records')
+            output_dict['history_table_selected_row_state'] = []
+            
+            if history_df.empty:
+                output_dict['annot_panel'] = {
+                    annot_name: annot_display_component.default_display_value if \
+                    annot_display_component.default_display_value is not None else '' \
+                    for annot_name, annot_display_component in annot_app_display_types_dict.items() 
+                }
             else:
-                prop_id = ctx.triggered[0]['prop_id'].split('.')[0]
+                current_annotations = review_data.data.annot_df.loc[subject_index_value, list(annot_app_display_types_dict.keys())].to_dict()
+                for annot_name, v in current_annotations.items():
+                    if isinstance(v, list):
+                        continue
+                    
+                    if (
+                        (pd.isna(v) or (v == '') or (v is None)) and 
+                        (annot_app_display_types_dict[annot_name].default_display_value is not None)
+                    ):
+                        current_annotations[annot_name] = annot_app_display_types_dict[annot_name].default_display_value
+                    
+                output_dict['annot_panel'] = current_annotations
+            return output_dict
+
+        ####### Callbacks
+
+        @app.callback(
+            output=dict(
+                more_component_outputs=more_component_outputs,
+                history_table=Output('APP-history-table', 'data', allow_duplicate=True),
+                history_table_selected_row_state=Output('APP-history-table', 'selected_rows', allow_duplicate=True),
+                annot_panel=annotation_panel_component.callback_output,
+                review_data_selected_value=Output('APP-review-data-table', 'selected_rows', allow_duplicate=True),
+                review_data_page_current=Output('APP-review-data-table', 'page_current', allow_duplicate=True)
+            ),
+            inputs=dict(
+                dropdown_value=Input('APP-dropdown-data-state', 'value'),
+                review_data_table_state=State('APP-review-data-table', 'data'),
+                more_component_inputs_as_states=more_component_inputs_as_states,
+                review_data_table_derived_virtual_data_state=State('APP-review-data-table', 'derived_virtual_data')
+            ),
+            prevent_initial_call=True,
+        )
+        def update_sample_via_dropdown(
+            dropdown_value,
+            review_data_table_state,
+            more_component_inputs_as_states,
+            review_data_table_derived_virtual_data_state
+        ):
+            """
+            Update the whole dashboard with the corresponding data of 
+            the selected subject in the dropdown menu
+            """
+            output_dict = {
+                'review_data_page_current': dash.no_update,
+                'review_data_selected_value': dash.no_update,
+            }
+            
+            tmp_review_data_table_df = pd.DataFrame.from_records(review_data_table_state)
+            subject_index_value = dropdown_value
+
+            if review_data_table_df is not None: # if the table is being used
+                index_tmp_review_data_table_df = tmp_review_data_table_df.loc[
+                    tmp_review_data_table_df['index'] == subject_index_value
+                ]
+                output_dict['review_data_selected_value'] = index_tmp_review_data_table_df.index
+
+                review_data_table_derived_virtual_df = pd.DataFrame.from_records(
+                    review_data_table_derived_virtual_data_state)
+                index_relative_review_data_table_df = review_data_table_derived_virtual_df.loc[
+                    review_data_table_derived_virtual_df['index'] == subject_index_value,
+                ]
+                if not index_relative_review_data_table_df.empty:
+                    output_dict['review_data_page_current'] = floor(index_relative_review_data_table_df.index[0] / review_data_table_page_size)
+
+
+            output_dict = update_components(output_dict, subject_index_value, more_component_inputs_as_states)
+            return output_dict
             
-            output_dict = {'history_table': dash.no_update,
-                           'annot_panel': {annot_col: dash.no_update for annot_col in
-                                           annot_app_display_types_dict.keys()},
-                           'dropdown_list_options': dash.no_update,
-                           'dropdown_value': dash.no_update,
-                           'review_data_selected_value': dash.no_update,
-                           'review_data_page_current': dash.no_update,
-                           'review_data_table_data': dash.no_update,
-                           'history_table_selected_row_state': dash.no_update,
-                           'more_component_outputs': {c.name: list(np.full(len(c.callback_output), dash.no_update)) for
-                                                      c_name, c in self.more_components.items()},
-                           }
+
+        @app.callback(
+            output=dict(
+                dropdown_value=Output('APP-dropdown-data-state', 'value', allow_duplicate=True),
+                more_component_outputs=more_component_outputs,
+                history_table=Output('APP-history-table', 'data', allow_duplicate=True),
+                history_table_selected_row_state=Output('APP-history-table', 'selected_rows', allow_duplicate=True),
+                annot_panel=annotation_panel_component.callback_output,
+            ),
+            inputs=dict(
+                review_data_selected_value=Input('APP-review-data-table', 'selected_rows'),
+                review_data_table_state=State('APP-review-data-table', 'data'),
+                more_component_inputs_as_states=more_component_inputs_as_states,
+            ),
+            prevent_initial_call=True,
+        )
+        def update_sample_via_review_table(
+            review_data_selected_value,
+            review_data_table_state,
+            more_component_inputs_as_states
+        ):
+            """
+            Update the whole dashboard with the corresponding data of the selected subject in the dash table
+            """
+            output_dict = {}
+            
+            tmp_review_data_table_df = pd.DataFrame.from_records(review_data_table_state)
+            subject_index_value = tmp_review_data_table_df.loc[review_data_selected_value[0], 'index'] 
+            output_dict['dropdown_value'] = subject_index_value
+
+            output_dict = update_components(output_dict, subject_index_value, more_component_inputs_as_states)
+            return output_dict
             
-            # don't load components if no index is selected from table/dropdown
-            if (dropdown_value is None) and (len(review_data_selected_value) == 0):
-                return output_dict
 
-            if (prop_id == 'APP-dropdown-data-state') or (prop_id == 'APP-review-data-table'):
-                tmp_review_data_table_df = pd.DataFrame.from_records(review_data_table_state)
-                if prop_id == 'APP-dropdown-data-state':
-                    subject_index_value = dropdown_value
-
-                    if review_data_table_df is not None: # if the table is being used
-                        index_tmp_review_data_table_df = tmp_review_data_table_df.loc[
-                            tmp_review_data_table_df['index'] == subject_index_value
-                        ]
-                        output_dict['review_data_selected_value'] = index_tmp_review_data_table_df.index
-
-                        review_data_table_derived_virtual_df = pd.DataFrame.from_records(
-                            review_data_table_derived_virtual_data_state)
-                        index_relative_review_data_table_df = review_data_table_derived_virtual_df.loc[
-                            review_data_table_derived_virtual_df['index'] == subject_index_value,
-                        ]
-                        if not index_relative_review_data_table_df.empty:
-                            output_dict['review_data_page_current'] = floor(index_relative_review_data_table_df.index[0] / review_data_table_page_size)
-                else:
-                    subject_index_value = tmp_review_data_table_df.loc[review_data_selected_value[0], 'index'] 
-                    output_dict['dropdown_value'] = subject_index_value
-
-
-                for c_name, component in self.more_components.items():
-                    if component.new_data_callback is not None:
-                        component_output = component.new_data_callback(review_data.data,
-                                                                       subject_index_value,
-                                                                       *more_component_inputs[component.name])
-                        validate_callback_outputs(component_output, component, which_callback='new_data_callback')
-                        output_dict['more_component_outputs'][component.name] = component_output
-                
-                history_df = get_history_display_table(subject_index_value)
-                output_dict['history_table'] = history_df.to_dict('records')
-                output_dict['history_table_selected_row_state'] = []
+        @app.callback(
+            output=dict(
+                history_table=Output('APP-history-table', 'data', allow_duplicate=True),
+                dropdown_list_options=Output('APP-dropdown-data-state', 'options', allow_duplicate=True),
+                review_data_table_data=Output('APP-review-data-table', 'data', allow_duplicate=True)
+            ),
+            inputs=dict(
+                submit_annot_button=Input('APP-submit-button-state', 'n_clicks'),
+                annot_input_state=annotation_panel_component.callback_state,
+                dropdown_value=State('APP-dropdown-data-state', 'value'),
+                review_data_table_state=State('APP-review-data-table', 'data'),
+            ),
+            prevent_initial_call=True,
+        )
+        def submit_button_annotation(
+            submit_annot_button,
+            annot_input_state,
+            dropdown_value,
+            review_data_table_state
+        ):
+            """
+            Save current annotations to the annot_df field, and update the dropdown menu timestamp and history table
+            """
+            output_dict = {'review_data_table_data': dash.no_update}
+            for annot_name in annot_app_display_types_dict.keys():
+                annot_type = review_data.data.annot_col_config_dict[annot_name]
+                # Convert type
+                if annot_app_display_types_dict[annot_name].display_output_format is not None:
+                    annot_input_state[annot_name] = annot_app_display_types_dict[annot_name].display_output_format(
+                        annot_input_state[annot_name]
+                    )
                 
-                if history_df.empty:
-                    output_dict['annot_panel'] = {
-                        annot_name: annot_display_component.default_display_value if \
-                        annot_display_component.default_display_value is not None else '' \
-                        for annot_name, annot_display_component in annot_app_display_types_dict.items() 
-                    }
-                else:
-                    current_annotations = review_data.data.annot_df.loc[subject_index_value, list(annot_app_display_types_dict.keys())].to_dict()
-                    for annot_name, v in current_annotations.items():
-                        if isinstance(v, list):
-                            continue
-                        
-                        if (
-                            (pd.isna(v) or (v == '') or (v is None)) and 
-                            (annot_app_display_types_dict[annot_name].default_display_value is not None)
-                        ):
-                            current_annotations[annot_name] = annot_app_display_types_dict[annot_name].default_display_value
-                        
-                    output_dict['annot_panel'] = current_annotations
-                            
-            elif (prop_id == 'APP-submit-button-state') & (submit_annot_button > 0):
-                for annot_name in annot_app_display_types_dict.keys():
-                    annot_type = review_data.data.annot_col_config_dict[annot_name]
-                    # Convert type
-                    if annot_app_display_types_dict[annot_name].display_output_format is not None:
-                        annot_input_state[annot_name] = annot_app_display_types_dict[annot_name].display_output_format(
-                            annot_input_state[annot_name]
-                        )
-                    
-                    validate_annot_data(annot_type, annot_input_state[annot_name])
+                validate_annot_data(annot_type, annot_input_state[annot_name])
                     
                 new_annot_input_state = dict(annot_input_state)
                 review_data._update(dropdown_value, new_annot_input_state)
                 
                 if auto_export:
                     review_data.export_data(auto_export_path, attributes_to_export=attributes_to_export, verbose=False)
 
                 output_dict['history_table'] = get_history_display_table(dropdown_value).to_dict('records')
                 
-                reviewed_data_df.loc[dropdown_value, 'label'] = self.gen_dropdown_labels(review_data,
-                                                                                         reviewed_data_df.loc[
-                                                                                             dropdown_value])
+                reviewed_data_df.loc[dropdown_value, 'label'] = self.gen_dropdown_labels(
+                    review_data,
+                    reviewed_data_df.loc[dropdown_value]
+                )
                 output_dict['dropdown_list_options'] = reviewed_data_df.reset_index().to_dict('records')
 
                 if review_data_table_df is not None:
                     tmp_review_data_table_df = pd.DataFrame.from_records(review_data_table_state).set_index('index')
                     tmp_review_data_table_df.loc[
                         dropdown_value,
                         review_data.data.annot_df.columns
                     ] = review_data.data.annot_df.loc[dropdown_value].values
-                    output_dict['review_data_table_data'] = self.columns_to_string(tmp_review_data_table_df, multi_type_columns).reset_index().to_dict('records')
-                    
-            elif 'APP-autofill-' in prop_id:
-                component_name = prop_id.split('APP-autofill-')[-1]
-                for autofill_annot_col, value in autofill_states[prop_id].items():
-                    output_dict['annot_panel'][autofill_annot_col] = value
-                    
-                for autofill_annot_col, value in autofill_literals[prop_id].items():
-                    output_dict['annot_panel'][autofill_annot_col] = value
-                    
-            elif (prop_id == 'APP-revert-annot-button'):
-                if len(history_table_selected_row_state) > 0:
-                    history_df = review_data.data.history_df.loc[review_data.data.history_df['index'] == dropdown_value].loc[::-1].reset_index()
-                    output_dict['annot_panel'] = history_df.iloc[history_table_selected_row_state[0]][review_data.data.annot_df.columns].fillna('').to_dict()
-                    
-            elif prop_id == 'APP-clear-annot-button':
-                output_dict['annot_panel'] = {annot_col: '' for annot_col in review_data.data.annot_df.columns}
+                    output_dict['review_data_table_data'] = self.columns_to_string(
+                        tmp_review_data_table_df, 
+                        multi_type_columns
+                    ).reset_index().to_dict('records')
+
+                return output_dict
+
+               
+        @app.callback(
+            output=dict(
+                annot_panel=annotation_panel_component.callback_output
+            ),
+            inputs=dict(
+                autofill_buttons=[Input(b.id, 'n_clicks') for b in autofill_buttons],
+                autofill_states=gen_autofill_states,
+            ),
+            prevent_initial_call=True,
+        )
+        def autofill_annot(
+            autofill_buttons,
+            autofill_states
+        ):
+            """
+            Detect and fill annotation panel from autofill trigger
+            """
+            ctx = dash.callback_context
+            if not ctx.triggered:
+                raise PreventUpdate
             else:
-                for c_name, component in self.more_components.items():
-                    if sum([ci.component_id == prop_id for ci in component.callback_input]) > 0:
-                        if component.internal_callback is None:
-                            raise ValueError(
-                                f'Component ({component.name}) has Inputs that change ({prop_id}), '
-                                f'but no internal_callback defined to handle it.'
-                                f'Either remove Input "{prop_id}" from "{component.name}.callback_input" attribute, '
-                                f'or define a callback function')
-
-                        component_output = component.internal_callback(review_data.data,
-                                                                       dropdown_value,
-                                                                       *more_component_inputs[component.name])
+                prop_id = ctx.triggered[0]['prop_id'].split('.')[0]
+                
+            output_dict = {
+                'annot_panel': {
+                    annot_col: dash.no_update for annot_col in annot_app_display_types_dict.keys()
+                }
+            }
+            component_name = prop_id.split('APP-autofill-')[-1]
+            for autofill_annot_col, value in autofill_states[prop_id].items():
+                output_dict['annot_panel'][autofill_annot_col] = value
+                
+            for autofill_annot_col, value in autofill_literals[prop_id].items():
+                output_dict['annot_panel'][autofill_annot_col] = value
+            return output_dict
 
-                        validate_callback_outputs(component_output, component, which_callback='internal_callback')
-                        output_dict['more_component_outputs'][component.name] = component_output
 
+        @app.callback(
+            output=dict(
+                annot_panel=annotation_panel_component.callback_output
+            ),
+            inputs=dict(
+                revert_annot_button=Input('APP-revert-annot-button', 'n_clicks'),
+                history_table_selected_row_state=State('APP-history-table', 'selected_rows'),
+                dropdown_value=State('APP-dropdown-data-state', 'value')
+            ),
+            prevent_initial_call=True,
+        )
+        def revert_annot(
+            revert_annot_button,
+            history_table_selected_row_state,
+            dropdown_value
+        ):
+            """
+            Revert the annotation fields to a previous annotation by selecting the row in the history table
+            """
+            output_dict = {
+                'annot_panel': {
+                    annot_col: dash.no_update for annot_col in annot_app_display_types_dict.keys()
+                }
+            }
+            if len(history_table_selected_row_state) > 0:
+                history_df = review_data.data.history_df.loc[review_data.data.history_df['index'] == dropdown_value].loc[::-1].reset_index()
+                output_dict['annot_panel'] = history_df.iloc[
+                    history_table_selected_row_state[0]
+                ][review_data.data.annot_df.columns].fillna('').to_dict()
+                
             return output_dict
+
+
+        @app.callback(
+            output=dict(
+                annot_panel=annotation_panel_component.callback_output
+            ),
+            inputs=dict(
+                clear_annot_button=Input('APP-clear-annot-button', 'n_clicks'),
+            ),
+            prevent_initial_call=True,
+        )
+        def clear_annot(clear_annot_button):
+            """
+            Clear the data currently entered in the annotation panel
+            """
+            output_dict = {}
+            output_dict['annot_panel'] = {annot_col: '' for annot_col in review_data.data.annot_df.columns}
+            return output_dict
+
+               
+        @app.callback(
+            output=dict(
+                more_component_outputs=more_component_outputs
+            ),
+            inputs=dict(
+                more_component_inputs=more_component_inputs,
+                dropdown_value=State('APP-dropdown-data-state', 'value'),
+            ),
+            prevent_initial_call=True,
+        )
+        def internal_update_components(more_component_inputs, dropdown_value):
+            """
+            Update triggered component
+            """
+            ctx = dash.callback_context
+            if not ctx.triggered:
+                raise PreventUpdate
+            else:
+                prop_id = ctx.triggered[0]['prop_id'].split('.')[0]
+
+            output_dict = {
+                'more_component_outputs': {
+                    c.name: list(np.full(len(c.callback_output), dash.no_update)) for c_name, c in self.more_components.items()
+                }
+            }
+            for c_name, component in self.more_components.items():
+                if sum([ci.component_id == prop_id for ci in component.callback_input]) > 0:
+                    if component.internal_callback is None:
+                        raise ValueError(
+                            f'Component ({component.name}) has Inputs that change ({prop_id}), '
+                            f'but no internal_callback defined to handle it.'
+                            f'Either remove Input "{prop_id}" from "{component.name}.callback_input" attribute, '
+                            f'or define a callback function'
+                        )
+
+                    component_output = component.internal_callback(
+                        review_data.data,
+                        dropdown_value,
+                        *more_component_inputs[component.name]
+                    )
+
+                    validate_callback_outputs(component_output, component, which_callback='internal_callback')
+                    output_dict['more_component_outputs'][component.name] = component_output
+            return output_dict
+
+        jupyter_dash.default_mode = mode
+        app.run(host=host, port=port, debug=True)
         
-        app.run_server(mode=mode, host=host, port=port, debug=True) 
-        
-    def gen_layout(self,
-                   review_data: ReviewDataInterface,
-                   reviewed_data_df: pd.DataFrame,
-                   annot_app_display_types_dict: Dict,
-                   autofill_dict: Dict,
-                   review_data_table_df: pd.DataFrame=None,
-                   review_data_table_page_size: int = 10,
-                   collapsable=True,
-                   multi_type_columns=[]
-                   ):
-        
+    def gen_layout(
+        self,
+        review_data: ReviewDataInterface,
+        reviewed_data_df: pd.DataFrame,
+        annot_app_display_types_dict: Dict,
+        autofill_dict: Dict,
+        review_data_table_df: pd.DataFrame=None,
+        review_data_table_page_size: int = 10,
+        collapsable=True,
+        multi_type_columns=[]
+    ):
+        """
+        Generate layout of the dashboard
+        """
         review_data_title = html.Div([html.H1(review_data.data_pkl_fn.split('/')[-1].split('.')[0])])
         review_data_path = html.Div([html.P(f'Path: {review_data.data_pkl_fn}')])
         review_data_description = html.Div([html.P(f'Description: {review_data.data.description}')])
         dropdown = html.Div(dcc.Dropdown(options=reviewed_data_df.reset_index().to_dict('records'),
                                          value=None, 
                                          id='APP-dropdown-data-state'))
         
@@ -685,24 +870,27 @@
             autofill_buttons += [autofill_button_component]
             autofill_states[autofill_button_component.id] = button_autofill_states_dict
             autofill_literals[autofill_button_component.id] = button_autofill_non_states_dict
             
         return autofill_buttons, autofill_states, autofill_literals
 
 
-    def gen_annotation_panel_component(self,
-                                       review_data: ReviewDataInterface,
-                                       autofill_buttons: [html.Button],
-                                       annot_app_display_types_dict: Dict
-                                       ):
+    def gen_annotation_panel_component(
+        self,
+        review_data: ReviewDataInterface,
+        autofill_buttons: [html.Button],
+        annot_app_display_types_dict: Dict
+    ):
 
         if len(annot_app_display_types_dict) == 0:
-            raise ValueError(f'annot_app_display_types_dict is empty. '
-                             f'Make sure to run reviewer.set_default_review_data_annotations_configuration(), '
-                             f'or manually set up your annotations')
+            raise ValueError(
+                f'annot_app_display_types_dict is empty. '
+                f'Make sure to run reviewer.set_default_review_data_annotations_configuration(), '
+                f'or manually set up your annotations'
+            )
         submit_annot_button = html.Button(id='APP-submit-button-state', 
                                           n_clicks=0, 
                                           children='Submit', 
                                           style={"marginBottom": "15px"})
         
         def annotation_display_component_input(annot_name, annot, annot_app_display_type):
             input_component_id = f"APP-{annot_name}-{annot_app_display_type}-input-state"
@@ -723,75 +911,29 @@
         ] + [submit_annot_button]
         
         panel_inputs = [Input('APP-submit-button-state', 'nclicks')]
         return AppComponent(
             name='APP-Panel',
             layout=panel_components,
             callback_output={
-                annot_name: Output(f"APP-{annot_name}-{display_type}-input-state", "value")
+                annot_name: Output(f"APP-{annot_name}-{display_type}-input-state", "value", allow_duplicate=True)
                 for annot_name, display_type in annot_app_display_types_dict.items()},
             callback_input=panel_inputs,
             callback_state={
                 annot_name: State(f"APP-{annot_name}-{display_type}-input-state", "value") for
                     annot_name, display_type in annot_app_display_types_dict.items()},
             use_name_as_title=False
         )
     
-#     def _gen_annotation_input_DEPRECATED(self, annot_name, annot, annot_app_display_type: str, input_component_id):
-        
-#         warnings.warn(f'DEPRECATION WARNING: Annot app display type is string.')
-#         if annot_app_display_type == 'textarea':
-#             input_component = dbc.Textarea(size="lg", 
-#                                            id=input_component_id,
-#                                            value=annot.default),
-#         elif annot_app_display_type == 'text':
-#             input_component = dbc.Input(type="text",
-#                                         id=input_component_id,
-#                                         placeholder=f"Enter {annot_name}",
-#                                         value=annot.default,
-#                                         )
-#         elif annot_app_display_type == 'number':
-#             input_component = dbc.Input(type="number", 
-#                                         id=input_component_id, 
-#                                         placeholder=f"Enter {annot_name}",
-#                                         value=annot.default)
-#         elif annot_app_display_type == 'checklist':
-#             default = [] if annot.default is None else annot.default
-#             if type(default) != list:
-#                 raise ValueError(f'Default for {input_component_id} must be given as a list for checklist annotations, not as a {type(default)}. Perhaps change default to [{default}]?')
-#             input_component = dbc.Checklist(options=[{"label": f, "value": f} for f in annot.options],
-#                                             id=input_component_id, 
-#                                             value=default),
-#         elif annot_app_display_type == 'radioitem':
-#             input_component = dbc.RadioItems(
-#                                             options=[{"label": f, "value": f} for f in annot.options],
-#                                             value=annot.default,
-#                                             id=input_component_id,
-#                                         )
-#         elif annot_app_display_type == 'select':
-#             if annot.default is not None:
-#                 input_component = dbc.Select(
-#                                             options=[{"label": f, "value": f} for f in annot.options],
-#                                             id=input_component_id,
-#                                             ),
-#             else:
-#                 input_component = dbc.Select(
-#                                             options=[{"label": f, "value": f} for f in annot.options],
-#                                             value=annot.default,
-#                                             id=input_component_id,
-#                                             ),
-#         else:
-#             raise ValueError(f'Invalid annotation display type "{annot_app_display_type}"')
-            
-#         return input_component
-    
     
-    def add_component(self, 
-                      component: AppComponent, 
-                      **kwargs):
+    def add_component(
+        self, 
+        component: AppComponent, 
+        **kwargs
+    ):
         """
         component: An AppComponent object to include in the app
         **kwargs: include more arguments for the component's callback functions 
         """
         
         all_component_names = [c_name for c_name, c in self.more_components.items()]
         
@@ -829,22 +971,25 @@
         table_title:     Title of the table
         component_id: component name for the table
         table_fn_col:   column in review_data data dataframe with file path with table to display
         table_cols:     columns to display in table from table_fn_col
         """
         table = html.Div(dbc.Table.from_dataframe(pd.DataFrame()),
                          id=component_id)
-        self.add_component(AppComponent(table_title,
-                                        table,
-                                        new_data_callback=lambda data, idx: [dbc.Table.from_dataframe(
-                                            pd.read_csv(getattr(data, data_table_source).loc[idx, table_fn_col],
-                                                        sep='\t',
-                                                        encoding='iso-8859-1')[table_cols])],
-                                        callback_output=[Output(component_id, 'children')]
-                                        ))
+        self.add_component(
+            AppComponent(
+                table_title,
+                table,
+                new_data_callback=lambda data, idx: [dbc.Table.from_dataframe(
+                    pd.read_csv(getattr(data, data_table_source).loc[idx, table_fn_col],
+                                sep='\t',
+                                encoding='iso-8859-1')[table_cols])],
+                callback_output=[Output(component_id, 'children')]
+            )
+        )
 
 
 def get_component_ids(component: Union[List, Tuple]):
     if isinstance(component, list) or isinstance(component, tuple):
         id_list = []
         for comp in component:
             id_list += get_component_ids(comp)
```

### Comparing `AnnoMate-0.0.0/AnnoMate/ReviewDataInterface.py` & `AnnoMate-0.0.1/AnnoMate/ReviewDataInterface.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/ReviewerTemplate.py` & `AnnoMate-0.0.1/AnnoMate/ReviewerTemplate.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate/Reviewers/ExampleReviewer.py` & `AnnoMate-0.0.1/AnnoMate/Reviewers/ExampleReviewer.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/AnnoMate.egg-info/PKG-INFO` & `AnnoMate-0.0.1/AnnoMate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: AnnoMate
-Version: 0.0.0
+Version: 0.0.1
 Summary: A general tool to create dashboards for manual review
 Home-page: https://github.com/getzlab/AnnoMate
 Author: Claudia Chu
 Author-email: cchu@broadinstitute.org
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/getzlab/AnnoMate/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -118,9 +116,7 @@
 Most ACBs use jupyter notebooks for their analysis. So why not keep the review process in jupyter notebooks too? Additionally, there already exist great tools for making interactive figures and dashboards. We can use these packages to help automatically consildate information and create figures that will make it easier to review, enforce annotation standards, and track changes over time.
 
 The `JupyterReviewer` package makes it simple to create dashboards for reviewing data. Developers and users can easily customize their dashboards to incorpate any data they like, and automatically provides a reviewer an easy way to annotate their data, track changes, and share their annotations with others.
 
 ### Get Started
 
 See `example_notebooks/` for documentation and tutorials.
-
-
```

### Comparing `AnnoMate-0.0.0/AnnoMate.egg-info/SOURCES.txt` & `AnnoMate-0.0.1/AnnoMate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/LICENSE.txt` & `AnnoMate-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/PKG-INFO` & `AnnoMate-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: AnnoMate
-Version: 0.0.0
+Version: 0.0.1
 Summary: A general tool to create dashboards for manual review
 Home-page: https://github.com/getzlab/AnnoMate
 Author: Claudia Chu
 Author-email: cchu@broadinstitute.org
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/getzlab/AnnoMate/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -118,9 +116,7 @@
 Most ACBs use jupyter notebooks for their analysis. So why not keep the review process in jupyter notebooks too? Additionally, there already exist great tools for making interactive figures and dashboards. We can use these packages to help automatically consildate information and create figures that will make it easier to review, enforce annotation standards, and track changes over time.
 
 The `JupyterReviewer` package makes it simple to create dashboards for reviewing data. Developers and users can easily customize their dashboards to incorpate any data they like, and automatically provides a reviewer an easy way to annotate their data, track changes, and share their annotations with others.
 
 ### Get Started
 
 See `example_notebooks/` for documentation and tutorials.
-
-
```

### Comparing `AnnoMate-0.0.0/README.md` & `AnnoMate-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.0/setup.py` & `AnnoMate-0.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnnoMate",
-    version="0.0.0",
+    version="0.0.1",
     author="Claudia Chu",
     author_email="cchu@broadinstitute.org",
     description="A general tool to create dashboards for manual review",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/getzlab/AnnoMate",
     project_urls={
@@ -20,33 +20,32 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "."},
     packages=setuptools.find_packages(where=".", exclude=['zeption.examples', '']),
     python_requires=">=3.6",
     install_requires = ['cnv-suite',
-                        'dash',
+                        'dash>=2.11.0',
                         'dash-bootstrap-components',
                         'dash-cytoscape',
                         'dash-daq',
                         'fsspec',
                         'gcsfs',
                         'google-auth',
                         'google-api-core',
                         'hound',
                         'ipykernel',
                         'ipython',
-                        'jupyter-dash',
-                        'jupyterlab',
+                        'jupyterlab>=4.0.2',
                         'matplotlib',
                         'pandas',
                         'pickleshare',
                         'pillow',
                         'pip',
-                        'plotly',
+                        'plotly>=5.15.0',
                         'scipy',
                         'setuptools',
                         'frozendict',
                         # fixes jupyter-dash bug when repeat calls to run_server hangs
                         # see: https://github.com/plotly/jupyter-dash/issues/103
                         'flask<=2.2.1',
                         'werkzeug<=2.2.1']
```

