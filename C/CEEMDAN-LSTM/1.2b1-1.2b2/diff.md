# Comparing `tmp/CEEMDAN_LSTM-1.2b1.tar.gz` & `tmp/CEEMDAN_LSTM-1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CEEMDAN_LSTM-1.2b1.tar", last modified: Wed Jun 14 11:00:12 2023, max compression
+gzip compressed data, was "CEEMDAN_LSTM-1.2b2.tar", last modified: Sat Jul  8 13:25:37 2023, max compression
```

## Comparing `CEEMDAN_LSTM-1.2b1.tar` & `CEEMDAN_LSTM-1.2b2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.070623 CEEMDAN_LSTM-1.2b1/
-drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.037078 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/
--rw-rw-rw-   0        0        0      916 2022-11-18 01:34:52.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/__init__.py
--rw-rw-rw-   0        0        0    25551 2023-06-14 08:47:20.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/core.py
--rw-rw-rw-   0        0        0    41297 2023-06-11 07:33:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/data_preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.067625 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/
--rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/beijing_ets.csv
--rw-rw-rw-   0        0        0    56764 2023-03-15 06:59:29.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ftse.csv
--rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
--rw-rw-rw-   0        0        0    59837 2023-03-15 06:59:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hsi.csv
--rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hubei_ets.csv
--rw-rw-rw-   0        0        0    57605 2023-06-08 11:49:39.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/n225.csv
--rw-rw-rw-   0        0        0    61006 2023-06-08 11:48:36.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/nasdaq.csv
--rw-rw-rw-   0        0        0    60683 2023-03-15 06:59:00.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sp500.csv
--rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sse_index.csv
--rw-rw-rw-   0        0        0    55845 2023-03-15 06:57:54.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ssec.csv
--rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/tianjin_ets.csv
--rw-rw-rw-   0        0        0    56152 2023-06-14 07:23:48.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/keras_predictor.py
--rw-rw-rw-   0        0        0    16724 2023-04-19 06:45:48.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/sklearn_predictor.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:00:12.041596 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/
--rw-rw-rw-   0        0        0     9923 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-06-14 11:00:12.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-14 11:00:11.000000 CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b1/LICENSE
--rw-rw-rw-   0        0        0     9923 2023-06-14 11:00:12.069627 CEEMDAN_LSTM-1.2b1/PKG-INFO
--rw-rw-rw-   0        0        0     9088 2022-11-18 01:55:56.000000 CEEMDAN_LSTM-1.2b1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 11:00:12.070623 CEEMDAN_LSTM-1.2b1/setup.cfg
--rw-rw-rw-   0        0        0     1374 2023-06-14 05:52:12.000000 CEEMDAN_LSTM-1.2b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.215470 CEEMDAN_LSTM-1.2b2/
+drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.203455 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/
+-rw-rw-rw-   0        0        0      916 2022-11-18 01:34:52.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/__init__.py
+-rw-rw-rw-   0        0        0    27877 2023-06-28 09:46:22.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/core.py
+-rw-rw-rw-   0        0        0    41842 2023-06-28 02:14:57.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/data_preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.213968 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/
+-rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/beijing_ets.csv
+-rw-rw-rw-   0        0        0    56764 2023-03-15 06:59:29.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ftse.csv
+-rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
+-rw-rw-rw-   0        0        0    59837 2023-03-15 06:59:12.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hsi.csv
+-rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hubei_ets.csv
+-rw-rw-rw-   0        0        0    57605 2023-06-08 11:49:39.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/n225.csv
+-rw-rw-rw-   0        0        0    61006 2023-06-08 11:48:36.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/nasdaq.csv
+-rw-rw-rw-   0        0        0    60683 2023-03-15 06:59:00.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sp500.csv
+-rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sse_index.csv
+-rw-rw-rw-   0        0        0    55845 2023-03-15 06:57:54.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ssec.csv
+-rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/tianjin_ets.csv
+-rw-rw-rw-   0        0        0    52234 2023-06-28 10:01:40.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/keras_predictor.py
+-rw-rw-rw-   0        0        0    32567 2023-06-28 05:07:59.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/sklearn_predictor.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.206966 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/
+-rw-rw-rw-   0        0        0     9996 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/LICENSE
+-rw-rw-rw-   0        0        0     9996 2023-07-08 13:25:37.214966 CEEMDAN_LSTM-1.2b2/PKG-INFO
+-rw-rw-rw-   0        0        0     9161 2023-06-14 11:10:49.000000 CEEMDAN_LSTM-1.2b2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:25:37.216475 CEEMDAN_LSTM-1.2b2/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2023-07-08 13:25:18.000000 CEEMDAN_LSTM-1.2b2/setup.py
```

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/__init__.py` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/__init__.py`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/core.py` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,20 +225,21 @@
     for x in redecom_list.values(): 
         if 'vmd' in x.lower() and len(check_data)%2: check_data = check_data.sort_index()[1:] 
     if 'vmd' in decom_mode.lower() and len(check_data)%2: check_data = check_data.sort_index()[1:] 
 
     # Set target
     if 'target' not in check_data.columns:
         if len(check_data.columns) == 1: check_data.columns=['target']
-        elif decom_mode.lower() in ['emd', 'eemd', 'ceemdan']: 
+        elif decom_mode.lower() in ['emd', 'eemd', 'ceemdan', 'vmd', 'ovmd', 'svmd']: 
             check_data['target'] = check_data.sum(axis=1).values
             print('Warning! The sum of all column has been set as the target column.') 
         else:
             check_data.columns = check_data.columns[1:].insert(0, 'target') # set first columns as target 
             print('Warning! The first column has been set as the target column.')  
+            print('Or, you can set DECOM_MODE as "emd" to let the sum of all column be the target column.')  
 
     # Show the inputting data
     if show_data:
         print('Data type is %s.'%type(check_data))
         print('Part of inputting dataset:')
         print(check_data)
         # print('\nData description:')
@@ -275,22 +276,20 @@
     return PATH, FIG_PATH, LOG_PATH
 
 # Name the predictor
 def name_predictor(now, name, module, model, decom_mode=None, redecom_list=None, next_pred=False):
     """
     Name the predictor for convenient saving.
     """
-
     redecom_mode = ''
     if redecom_list is not None: # Check redecom_list and get redecom_mode
         try: redecom_list = pd.DataFrame(redecom_list, index=[0]) 
         except: raise ValueError("Invalid input for redecom_list! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
         for i in range(redecom_list.size): redecom_mode = redecom_mode+redecom_list.values.ravel()[i]+'-'
 
-    from tensorflow.python.keras.models import Sequential
     if type(model) == str and '.h5' not in str(model):
         if 'Single' not in name:
             if decom_mode is not None: 
                 name = name + ' ' + decom_mode.upper() + '-' 
                 name = name + redecom_mode.upper()
         else: name = name + ' '
         name = name + model.upper()  # forecasting model
@@ -298,19 +297,63 @@
     if next_pred: name = name+' Next-day' # Next-day forecasting or not
     name = name + ' ' + module+' Forecasting'
     print('==============================================================================')
     print(str(now.strftime('%Y-%m-%d %H:%M:%S'))+' '+ name +' is running...')
     print('==============================================================================')
     return name
 
-# Change name
-def change_name(s): 
-    s = s.replace('-','_')
-    s = s.replace(' ','_')
-    return s
+# Output Result
+def output_result(df_result, name, time, imf='', type='Result'):
+    # Output Result and add Runtime
+    """
+    Input and Parameters:
+    ---------------------
+    name            - predictor_name
+    time            - end-start
+
+    Output
+    ---------------------
+    df_result 
+    """
+    imf_name = ''
+    if imf != '' and imf != 'Final': 
+        imf_name = ' of '+imf
+        print('\n----------'+name+imf_name+' Finished----------')
+    else: print('\n================'+name+' Finished================')
+    if isinstance(df_result, tuple) and len(df_result)==3: # (df_result, df_eval, df_loss)
+        df_result[1]['Runtime'] = time # Output Runtime
+        df_result[1]['IMF'] = imf
+        df_result[0].name, df_result[1].name, df_result[2].name = name+' Result'+imf_name, name+' Evaluation'+imf_name, name+' Loss'+imf_name
+        print(df_result[1]) # print df_eval
+    elif isinstance(df_result, tuple) and len(df_result)==2 and type=='Evaluation': # (df_pred_result, df_eval_result)
+        from CEEMDAN_LSTM.data_preprocessor import eval_result
+        df_pred_result = df_result[0]
+        final_eval = eval_result(df_pred_result['predict'], df_pred_result['real'])
+        final_eval['Runtime'] = time # Output Runtime
+        final_eval['IMF'] = imf
+        print(final_eval)
+        df_plot = df_pred_result[['real', 'predict']]
+        final_eval = pd.concat((final_eval, df_result[1]))
+        df_pred_result.name, final_eval.name, df_plot.name = name+' Result', name+' Evaluation', name+' Result'
+        df_result = [df_pred_result, final_eval, df_plot]
+    elif isinstance(df_result, tuple) and len(df_result)==2 and type=='Result': # (df_result, df_next_result)
+        df_result[0]['Runtime'] = time # Output Runtime
+        df_result[0]['IMF'] = imf
+        df_result = pd.concat((df_result[0], df_result[1]))
+        df_result.name = name+' Result'
+        print(df_result)
+    elif isinstance(df_result, pd.DataFrame) and type=='Result': # (df_result)
+        df_result['Runtime'] = time # Output Runtime
+        df_result['IMF'] = imf
+        df_result.name = name+' Result'+imf_name
+        print(df_result)
+    else: raise ValueError('Unknown Error.')
+    return df_result
+    
+
 
 # Plot and save data
 def plot_save_result(data, name=None, plot=True, save=True, path=None, type=None): 
     """
     Plot and save data.
     Example: cl.plot_save_result(df)
 
@@ -328,42 +371,40 @@
     if name is None: 
         name = datetime.now().strftime('%Y%m%d_%H%M%S_')
     elif isinstance(name, datetime):
         name = name.strftime('%Y%m%d_%H%M%S_')
     else: name = ''
     if PATH is None: save = False
 
-    # Default output function
-    def default_output(df): 
-        if 'Evaluation' not in df.name:
-            if plot:
-                df.plot(figsize=(8,4))
-                plt.title(df.name, fontsize=16, y=1)
-                if save: plt.savefig(FIG_PATH + name + change_name(df.name)+'.jpg', dpi=300, bbox_inches='tight') # Save figure
-                plt.show()
-        if save: pd.DataFrame.to_csv(df, LOG_PATH + name + change_name(df.name)+'.csv', encoding='utf-8') # Save log
+    def default_output(df, file_name): 
+        if 'Evaluation' not in df.name and 'Next' not in df.name and plot:
+            df.plot(figsize=(6,3))
+            plt.title(df.name, fontsize=12, y=1)
+            if save: plt.savefig(FIG_PATH + file_name +'.jpg', dpi=300, bbox_inches='tight') # Save figure
+            plt.show()
+        if save: pd.DataFrame.to_csv(df, LOG_PATH + file_name +'.csv', encoding='utf-8') # Save log
 
     # Ouput
     if isinstance(data, tuple):
         for df in data: # plot and save forecasting result
-            try: df.name # Check df Name
-            except: df.name = 'output'
-            default_output(df)
+            try: file_name = name + df.name.replace('-','_').replace(' ','_') # Check df Name
+            except: df.name, file_name = 'output', name+'output'
+            default_output(df, file_name)
     elif isinstance(data, pd.DataFrame):
-        try: data.name # Check data Name
-        except: data.name = 'output'
+        try: file_name = name + data.name.replace('-','_').replace(' ','_') # Check data Name
+        except: data.name, file_name = 'output', name+'output'
         if 'decom' in data.name: # plot and save plot EMD result
             if plot:
-                data.plot(figsize=(8,2*data.columns.size), subplots=True)
-                plt.gcf().suptitle(data.name, fontsize=16, y=0.9) # Enlarge and Move the title     
-                if save: plt.savefig(FIG_PATH + name + change_name(data.name)+'.jpg', dpi=300, bbox_inches='tight') # Save figure
+                data.plot(figsize=(6,1*data.columns.size), subplots=True)
+                plt.gcf().suptitle(data.name, fontsize=12, y=0.9) # Enlarge and Move the title     
+                if save: plt.savefig(FIG_PATH + file_name +'.jpg', dpi=300, bbox_inches='tight') # Save figure
                 plt.show()
-            if save: pd.DataFrame.to_csv(data, LOG_PATH + name + change_name(data.name)+'.csv', encoding='utf-8') # Save log
+            if save: pd.DataFrame.to_csv(data, LOG_PATH + file_name +'.csv', encoding='utf-8') # Save log
         else:
-            try: default_output(data)
+            try: default_output(data, file_name)
             except: print('Data is:\n', data)
     else:
         try: series = pd.Series(data)
         except: raise ValueError('Sorry! %s is not supported to plot and save, please input pd.DataFrame, pd.Series, nd.array(<=2D)'%type(data))
         default_output(series)
     if PATH is not None and save: print('The figures and logs of forecasting results have been saved into', PATH)
 
@@ -380,18 +421,18 @@
         dataset = load_dataset()
         data = pd.Series(dataset['close'].values, index=dataset.index)
     try: data = pd.Series(data) # 1.Load raw data
     except: raise ValueError('Sorry! %s is not supported, please input pd.DataFrame, pd.Series, nd.array(<=2D)'%type(data))
 
     kr = keras_predictor(**kwargs)
     df_result = kr.hybrid_keras_predict(data=data, show=True, plot=True, save=True)
-    
     return df_result
 
 
+
 # Run the details forecasting
 def details_keras_predict(data=None, fitting=False, **kwargs):
     """
     This function aims to help users know the forecasting framework more clearly, running the forecasting step by step.
     You can also refer the CEEMDAN-VMD-GRU repository: https://github.com/FateMurphy/CEEMDAN-VMD-GRU
     """
     # Decompose, integrate
```

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/data_preprocessor.py` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/data_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     if series is None: raise ValueError('Please input pd.Series, or pd.DataFrame(1D), nd.array(1D).')
     try: series = pd.Series(series)
     except: raise ValueError('Sorry! %s is not supported to decompose, please input pd.Series, or pd.DataFrame(1D), nd.array(1D)'%type(series))
     if len(series)%2: 
         print('Warning! The vmdpy module will delete the last one data point of series before decomposition')
         series = series[1:]
     if FORECAST_LENGTH is None: raise ValueError('Please input FORECAST_LENGTH.')
-    if vmd_params is None and optimize == False: vmd_params = {'K':10, 'tau':0}
+    if vmd_params is None and optimize == False: vmd_params = {'K':10, 'tau':0, 'alpha':2000}
 
     series_train = series[:-FORECAST_LENGTH]
     series_test = series[-FORECAST_LENGTH:]
     if vmd_params is None and optimize:
         try: import optuna
         except: raise ImportError('Cannot import optuna, run: pip install optuna!')
         def objective(trial):
@@ -231,74 +231,79 @@
     Output:
     ---------------------
     df_inte        - the integrating form of each time series
     df_inte_list   - the integrating set of each co-imf
     """
     
     # Check input
+    df_inte_list = []
     try: df_decom = pd.DataFrame(df_decom)
     except: raise ValueError('Invalid input of df_decom!')
     if 'target' in df_decom.columns: 
         tmp_target = df_decom['target']
         df_decom = df_decom.drop('target', axis=1, inplace=False)
     else: tmp_target = None
-    df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
 
-    # Check inte_list
-    df_inte_list = []
-    if inte_list is not None:
-        if str(inte_list).lower() == 'auto': # Without 
-            df_sampen = inte_sampen(df_decom)
-            inte_list = inte_kmeans(df_sampen, num_clusters)
-        elif isinstance(inte_list, pd.DataFrame):
-            if len(inte_list) == 1: inte_list = inte_list.T
-        elif type(inte_list) == str and len(inte_list) < df_decom.columns.size:
-            df_list, n, c, s = {}, 0, 0, 0
-            for i in inte_list: s = s + int(i) 
-            if s != df_decom.columns.size: raise ValueError('Invalid inte_list! %s (%s columns) does not match the number of dataset columns=%s.'%(inte_list, s, df_decom.columns.size)) 
-            for i in inte_list:
-                for j in ['imf'+str(x) for x in range(n, n+int(i))]: 
-                    df_list[j], n = c, n + 1
-                c += 1
-            inte_list = pd.DataFrame(df_list, index=['Cluster']).T
-        elif type(inte_list) == str and len(inte_list) == df_decom.columns.size:
-            inte_list = pd.DataFrame([int(x) for x in inte_list], columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
-        elif type(inte_list) == int and inte_list < df_decom.columns.size:
-            print('Integrate %d columns to be %d columns by K-means.'%(df_decom.columns.size, inte_list))
-            df_sampen = inte_sampen(df_decom)
-            inte_list = inte_kmeans(df_sampen, inte_list)
-        else:
-            try: inte_list = pd.DataFrame(inte_list, columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
-            except: raise ValueError('Invalid inte_list of %s with type %s. Check your input or length.'%(inte_list, type(inte_list)))
-
-        # Integrate, name, and resort
-        df_tmp = pd.DataFrame()
-        for i in range(inte_list.values.max()+1):
-            df_tmp['imf'+str(i)] = df_decom[inte_list[(inte_list['Cluster']==i)].index].sum(axis=1)
-            df_tmp_list = pd.DataFrame(df_tmp['imf'+str(i)])
-            df_tmp_list.columns = ['target']
-            df_inte_list.append(pd.concat((df_tmp_list, df_decom[inte_list[(inte_list['Cluster']==i)].index]), axis=1))
-        df_inte = df_tmp.T # Use Sample Entropy sorting the Co-IMFs
-        df_inte['sampen'] = inte_sampen(df_tmp).values
-        df_inte.sort_values(by=['sampen'], ascending=False, inplace=True)
-        df_inte.index = ['co-imf'+str(i) for i in range(inte_list.values.max()+1)]
-        df_inte = df_inte.drop('sampen', axis=1, inplace=False).T
-
-        # Rename df_inte_list
-        for i in range(len(df_inte.columns)):
-            for j in range(len(df_inte.columns)):
-                try:
-                    if df_inte_list[i]['target'].sum() == df_inte['co-imf'+str(j)].sum():
-                        df_inte_list[i].columns = ['co-imf'+str(j)] + list(df_inte_list[i].columns)[1:]
-                except: break
-
-        # Output
-        df_inte.name = 'df_inte_list_is_'+''.join(str(x) for x in inte_list.values.ravel()) # record integrate list
-        df_inte.index = df_decom.index
-    else: df_inte = df_decom
+    if df_decom.columns.size > num_clusters:
+        df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
+
+        # Check inte_list
+        if inte_list is not None:
+            if str(inte_list).lower() == 'auto': # Without 
+                df_sampen = inte_sampen(df_decom)
+                inte_list = inte_kmeans(df_sampen, num_clusters)
+            elif isinstance(inte_list, pd.DataFrame):
+                if len(inte_list) == 1: inte_list = inte_list.T
+            elif type(inte_list) == str and len(inte_list) < df_decom.columns.size:
+                df_list, n, c, s = {}, 0, 0, 0
+                for i in inte_list: s = s + int(i) 
+                if s != df_decom.columns.size: raise ValueError('Invalid inte_list! %s (%s columns) does not match the number of dataset columns=%s.'%(inte_list, s, df_decom.columns.size)) 
+                for i in inte_list:
+                    for j in ['imf'+str(x) for x in range(n, n+int(i))]: 
+                        df_list[j], n = c, n + 1
+                    c += 1
+                inte_list = pd.DataFrame(df_list, index=['Cluster']).T
+            elif type(inte_list) == str and len(inte_list) == df_decom.columns.size:
+                inte_list = pd.DataFrame([int(x) for x in inte_list], columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
+            elif type(inte_list) == int and inte_list < df_decom.columns.size:
+                print('Integrate %d columns to be %d columns by K-means.'%(df_decom.columns.size, inte_list))
+                df_sampen = inte_sampen(df_decom)
+                inte_list = inte_kmeans(df_sampen, inte_list)
+            else:
+                try: inte_list = pd.DataFrame(inte_list, columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
+                except: raise ValueError('Invalid inte_list of %s with type %s. Check your input or length.'%(inte_list, type(inte_list)))
+
+            # Integrate, name, and resort
+            df_tmp = pd.DataFrame()
+            for i in range(inte_list.values.max()+1):
+                df_tmp['imf'+str(i)] = df_decom[inte_list[(inte_list['Cluster']==i)].index].sum(axis=1)
+                df_tmp_list = pd.DataFrame(df_tmp['imf'+str(i)])
+                df_tmp_list.columns = ['target']
+                df_inte_list.append(pd.concat((df_tmp_list, df_decom[inte_list[(inte_list['Cluster']==i)].index]), axis=1))
+            df_inte = df_tmp.T # Use Sample Entropy sorting the Co-IMFs
+            df_inte['sampen'] = inte_sampen(df_tmp).values
+            df_inte.sort_values(by=['sampen'], ascending=False, inplace=True)
+            df_inte.index = ['co-imf'+str(i) for i in range(inte_list.values.max()+1)]
+            df_inte = df_inte.drop('sampen', axis=1, inplace=False).T
+
+            # Rename df_inte_list
+            for i in range(len(df_inte.columns)):
+                for j in range(len(df_inte.columns)):
+                    try:
+                        if df_inte_list[i]['target'].sum() == df_inte['co-imf'+str(j)].sum():
+                            df_inte_list[i].columns = ['co-imf'+str(j)] + list(df_inte_list[i].columns)[1:]
+                    except: break
+
+            # Output
+            df_inte.name = 'df_inte_list_is_'+''.join(str(x) for x in inte_list.values.ravel()) # record integrate list
+            df_inte.index = df_decom.index
+        else: df_inte = df_decom
+    else: 
+        df_decom.columns = ['co-imf'+str(i) for i in range(df_decom.columns.size)] # less than num_clusters, stop inte and output
+        df_inte = df_decom
     if tmp_target is not None: df_inte['target'] = tmp_target # add tmp target column
     return df_inte, df_inte_list
     
 
 # 2.1 Sample Entropy
 def inte_sampen(df_decom=None, max_len=1, tol=0.1, nor=True, **kwargs):
     """
@@ -314,17 +319,19 @@
     nor        - normalize or not 
     **kwargs   - any parameters of sampen.sampen2()
 
     Output:
     ---------------------
     df_sampen  - the Sample Entropy of each time series in pd.Dataframe
     """
-    try: df_decom = pd.DataFrame(df_decom)
-    except: raise ValueError('Invalid input of df_decom!')
-    if 'target' in df_decom.columns: df_decom = df_decom.drop('target', axis=1, inplace=False)
+    try: 
+        df_decom = pd.DataFrame(df_decom)
+        if 'target' in df_decom.columns: df_decom = df_decom.drop('target', axis=1, inplace=False)
+        if 'imf0' not in df_decom.columns: df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
+    except: raise ValueError('Invalid input of df_decom!') 
     try: import sampen
     except ImportError: raise ImportError('Cannot import sampen, run: pip install sampen!')
     np_sampen = []
     for i in range(df_decom.columns.size):
         sample_entropy = sampen.sampen2(list(df_decom['imf'+str(i)].values), mm=max_len, r=tol, normalize=nor, **kwargs)
         np_sampen.append(sample_entropy[1][1])
     df_sampen = pd.DataFrame(np_sampen, index=['imf'+str(i) for i in range(df_decom.columns.size)])
@@ -359,38 +366,38 @@
     return inte_list
 
 
 
 # 3.Other Mains
 # ------------------------------------------------------
 # 3.Main. Redecompose (inculd decom() and inte())
-def redecom(data=None, show_data=False, decom_mode='ceemdan', inte_list='auto', redecom_list={'co-imf0':'ovmd'}, vmd_params=None, FORECAST_LENGTH=None, **kwargs):
+def redecom(data=None, show=False, decom_mode='ceemdan', inte_list='auto', redecom_list={'co-imf0':'ovmd'}, vmd_params=None, FORECAST_LENGTH=None, **kwargs):
     """
     redecompose data adaptively and return results in pd.Dataframe.
     Example: df_decom = cl.redecom(series, decom_mode='ceemdan', redecom_list={'co-imf0':'vmd'})
     Plot by pandas: df_decom.plot(title='Decomposition Results', subplots=True)
 
     Input and Parameters:
     ---------------------
     series          - the time series (1D) to be decomposed
-    show_data       - show the inputting data set
+    show            - show the inputting data set
     decom_mode      - the decomposing methods eg. 'emd', 'eemd', 'ceemdan', 'vmd'
     inte_list       - the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...
     redecom_list    - the re-decomposition list eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame
     vmd_params      - the best parameters K and tau of OVMD to jump the optimization
     **kwargs        - any parameters of PyEMD.EMD(), PyEMD.EEMD(), PyEMD.CEEMDAN(), vmdpy.VMD()
                     - eg. trials for PyEMD.CEEMDAN(), change the number of inputting white noise 
     Output:
     ---------------------
     df_redecom      - the redecomposing results in pd.Dataframe
     df_redecom_list - each IMF's redecomposing results and itself as target
     """
 
     from CEEMDAN_LSTM.core import check_dataset
-    data = check_dataset(data, show_data, decom_mode, redecom_list)
+    data = check_dataset(data, show, decom_mode, redecom_list)
     if vmd_params is not None and type(vmd_params) != dict: raise ValueError('Invalid input of vmd_params!') 
     if len(data.columns) == 1: 
         df_decom = decom(data[data.columns[0]], decom_mode=decom_mode, FORECAST_LENGTH=FORECAST_LENGTH)
     else: df_decom = data # pd.DataFrame
     df_inte, df_inte_list = inte(df_decom, inte_list=inte_list)
 
     # Re-decompose 
@@ -411,15 +418,15 @@
             for x in df_redecom.columns[::-1]: df_inte.insert(int(i[-1]), x, df_redecom[x].values)
             df_redecom['target'] = df_inte[i] # record each imf redecompose result and itself as target
             df_redecom.name = i
             df_redecom_list.append(df_redecom) 
             df_inte = df_inte.drop(i, axis=1, inplace=False)
         df_inte.name = inte_columns+'_'+str(best_params_dict) # record redecomposition parameters
     else: df_inte.name = 'None'
-    if show_data:
+    if show:
         print('\nPart of preprocessing dataset (inculde training and test set):')
         print(df_inte)
     return df_inte, df_redecom_list
 
 # 3.Main. Evaluate
 def eval_result(y_real, y_pred): 
     """
```

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/beijing_ets.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/beijing_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ftse.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ftse.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/guangzhou_ets.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/guangzhou_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hsi.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hsi.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/hubei_ets.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hubei_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/n225.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/n225.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/nasdaq.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/nasdaq.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sp500.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sp500.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/sse_index.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sse_index.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/ssec.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ssec.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/datasets/tianjin_ets.csv` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/tianjin_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM/keras_predictor.py` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/keras_predictor.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,24 +26,22 @@
 import time
 import pandas as pd
 import numpy as np
 import warnings
 from datetime import datetime
 warnings.filterwarnings("ignore") # Ignore some annoying warnings
 # CEEMDAN_LSTM
-from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor, change_name
+from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor, output_result
 # Keras
-try: from tensorflow.python.keras.models import Sequential, load_model
+try: from tensorflow import constant 
 except: raise ImportError('Cannot import tensorflow, install or check your tensorflow verison!')
-from tensorflow import constant
-# from tcn import TCN # pip install keras-tcn
-from tensorflow.python.keras.layers import Dense, Activation, Dropout, LSTM, GRU, Flatten
-from tensorflow.python.keras.optimizer_v2.adam import Adam
-from tensorflow.python.keras.callbacks import ReduceLROnPlateau, EarlyStopping, ModelCheckpoint
-
+from tensorflow.keras.models import Sequential, load_model
+from tensorflow.keras.layers import Dense, Activation, Dropout, LSTM, GRU, Flatten, BatchNormalization
+from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.callbacks import ReduceLROnPlateau, EarlyStopping, ModelCheckpoint
 
 
 class keras_predictor:
     # 0.Initialize
     # ------------------------------------------------------
     def __init__(self, PATH=None, FORECAST_HORIZONS=30, FORECAST_LENGTH=30, KERAS_MODEL='GRU', DECOM_MODE='CEEMDAN', INTE_LIST='auto', 
                  REDECOM_LIST={'co-imf0':'ovmd'}, NEXT_DAY=False, DAY_AHEAD=1, NOR_METHOD='minmax', FIT_METHOD='add', USE_TPU=False , **kwargs):
@@ -160,19 +158,17 @@
                 try: KERAS_MODEL = pd.DataFrame(KERAS_MODEL, index=[0])
                 except: raise ValueError("Invalid input for KERAS_MODEL! Please input eg. 'GRU', 'LSTM', or model = Sequential(), h5 file, dict, pd.DataFrame.")
                 for file_name in KERAS_MODEL.values.ravel():
                     if '.h5' not in str(file_name): raise ValueError("Invalid input for KERAS_MODEL values! Please input eg. 'GRU', 'LSTM', or model = Sequential(), h5 file, dict, pd.DataFrame.")
                     if not os.path.exists(self.PATH+file_name): raise ValueError("File does not exist:", self.PATH+file_name)
 
         if type(DECOM_MODE) == str: self.DECOM_MODE = str(DECOM_MODE).upper() # Check DECOM_MODE
-
         if REDECOM_LIST is not None:# Check REDECOM_LIST
             try: REDECOM_LIST = pd.DataFrame(REDECOM_LIST, index=[0]) 
             except: raise ValueError("Invalid input for REDECOM_LIST! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
-
         if DAY_AHEAD == 0 and FIT_METHOD == 'ensemble': # Check DAY_AHEAD
                 raise ValueError('Warning! When DAY_AHEAD = 0, it is not support the fitting method, already fit today.')
 
         if self.opt_lr != 0.001 and self.opt == 'adam': self.opt = Adam(learning_rate=self.opt_lr) # Check optimizer
         if self.opt_patience > self.epochs: self.opt_patience = self.epochs // 10 # adjust opt_patience
         if self.stop_patience > self.epochs and self.stop_patience > 10: self.stop_patience = self.epochs // 2 # adjust stop_patience
         
@@ -188,45 +184,46 @@
         if model_file is not None and os.path.exists(str(model_file)):
             print('Load Keras model:', model_file)
             return load_model(model_file) # load user's saving custom model
         elif isinstance(self.KERAS_MODEL, Sequential): # if not load a model
             return self.KERAS_MODEL  
         elif self.KERAS_MODEL == 'LSTM':
             model = Sequential(name=model_name)
-            model.add(LSTM(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation, return_sequences=True))
+            model.add(LSTM(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), recurrent_activation='sigmoid', 
+                           activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(LSTM(self.units*2, activation=self.activation, return_sequences=True))
+            model.add(LSTM(self.units*2, recurrent_activation='sigmoid', activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(LSTM(self.units, activation=self.activation, return_sequences=False))
+            model.add(LSTM(self.units, recurrent_activation='sigmoid', activation=self.activation, return_sequences=False))
             model.add(Dropout(self.dropout))
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
         elif self.KERAS_MODEL == 'GRU':
             model = Sequential(name=model_name)
-            model.add(GRU(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), recurrent_activation = 'sigmoid', reset_after = True,
-                          activation=self.activation, return_sequences=True))
+            model.add(GRU(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), recurrent_activation='sigmoid', 
+                          reset_after=True, activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(GRU(self.units*2, recurrent_activation = 'sigmoid', reset_after = True,
-                          activation=self.activation, return_sequences=True))
+            model.add(GRU(self.units*2, recurrent_activation='sigmoid', reset_after=True, activation=self.activation, return_sequences=True))
             model.add(Dropout(self.dropout))
-            model.add(GRU(self.units, recurrent_activation = 'sigmoid', reset_after = True,
-                          activation=self.activation, return_sequences=False))
+            model.add(GRU(self.units, recurrent_activation='sigmoid', reset_after=True, activation=self.activation, return_sequences=False))
             model.add(Dropout(self.dropout))
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
         elif self.KERAS_MODEL == 'DNN':
             model = Sequential(name=model_name)
-            model.add(Dense(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation))
-            model.add(Dropout(self.dropout))
-            model.add(Dense(self.units*2, activation=self.activation))
+            model.add(Flatten(input_shape=(trainset_shape[1], trainset_shape[2])))
+            for _ in range(8):
+                model.add(Dense(self.units*4, activation=self.activation)) 
+                # model.add(BatchNormalization())
+                model.add(Dropout(self.dropout))
+            model.add(Dense(self.units*2, activation=self.activation)) 
             model.add(Dropout(self.dropout))
-            model.add(Flatten())
-            model.add(Dense(self.units, activation=self.activation))
+            model.add(Dense(self.units, activation=self.activation)) 
             model.add(Dropout(self.dropout))
             model.add(Dense(1, activation=self.activation))
             model.compile(loss=self.opt_loss, optimizer=self.opt)
             return model
         elif self.KERAS_MODEL == 'BPNN':
             model = Sequential(name=model_name)
             model.add(Dense(self.units*4, input_shape=(trainset_shape[1], trainset_shape[2]), activation=self.activation))
@@ -279,37 +276,41 @@
         """
 
         # Initialize
         from CEEMDAN_LSTM.data_preprocessor import create_train_test_set
         x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD, fitting_set) 
 
         # Convert to tensor = tf.constant()
-        today_x = x_train[-1].reshape(1, x_train.shape[1], x_train.shape[2])
+        today_x = x_train[-1].reshape(1, x_train.shape[1], x_train.shape[2]) # aviod resahpe tf.constant - tensor
         x_train = constant(x_train) # x_train = x_train.reshape((x_train.shape[0], x_train.shape[1], x_train.shape[2])) 
         if not self.NEXT_DAY: x_test = constant(x_test) # x_test = x_test.reshape((x_test.shape[0], x_test.shape[1], x_test.shape[2])) 
         
         # Set callbacks
         Reduce = ReduceLROnPlateau(monitor=self.callbacks_monitor, patience=self.opt_patience, verbose=self.verbose, mode='auto') # Adaptive learning rate
         EarlyStop = EarlyStopping(monitor=self.callbacks_monitor, patience=self.stop_patience, verbose=self.verbose, mode='auto') # Early stop at small learning rate 
         callbacks_list = [Reduce, EarlyStop]
 
-        # Load and save model
+        # Name model
         try: 
-            if '.h5' and '\'' and ':' not in str(data.name): data.name = data.name + '.h5'
-            else: data.name = 'Keras_model.h5'
+            data.name = data.name.replace('-','_').replace(' ','_')
+            if '.h5' not in str(data.name): data.name = data.name + '.h5'
         except: data.name = 'Keras_model.h5'
+        
+        # Load and save model
         model_file = None
         if self.PATH is not None:
-            if not isinstance(self.KERAS_MODEL, Sequential): # set model_file to load model
-                if isinstance(self.KERAS_MODEL, pd.DataFrame):
-                    for x in self.KERAS_MODEL.columns:
-                        if change_name(x) in data.name: model_file = x # change to be key value
-                    if model_file is not None: model_file = self.PATH + self.KERAS_MODEL[model_file][0]
-                    else: raise KeyError("Cannot match an appropriate model file by the column name of pd.DataFrame. Please check KERAS_MODEL.")
-                elif '.h5' in str(self.KERAS_MODEL): model_file = self.PATH + self.KERAS_MODEL
+            # Load model if get input of self.KERAS_MODEL
+            if isinstance(self.KERAS_MODEL, dict): self.KERAS_MODEL = pd.DataFrame(self.KERAS_MODEL, index=[0])
+            if isinstance(self.KERAS_MODEL, pd.DataFrame): # KERAS_MODEL eg. {'co-imf0':'co_imf0_model.h5', 'co-imf1':'co_imf1_model.h5'}
+                for x in self.KERAS_MODEL.columns:
+                    if (x).replace('-','_').replace(' ','_') in data.name: model_file = x # change to be key value
+                if model_file is not None: model_file = self.PATH + self.KERAS_MODEL[model_file][0]
+                else: raise KeyError("Cannot match an appropriate model file by the column name of pd.DataFrame. Please check KERAS_MODEL.")
+            if isinstance(self.KERAS_MODEL, str) and '.h5' in str(self.KERAS_MODEL): model_file = self.PATH + self.KERAS_MODEL
+            # Save model by CheckPoint with model name = data.name = df_redecom.name
             CheckPoint = ModelCheckpoint(self.PATH+data.name, monitor=self.callbacks_monitor, save_best_only=True, verbose=self.verbose, mode='auto') # Save the model to self.PATH after each epoch
             callbacks_list.append(CheckPoint) # save Keras model in .h5 file eg. predictor_name+'_of_'+imf+'_model.h5'
 
         # Build or load the model
         if self.USE_TPU: model = self.tpu_model(x_train.shape, data.name, model_file)
         else: model = self.build_model(x_train.shape, data.name, model_file)
         if show_model: 
@@ -329,30 +330,31 @@
                                 shuffle=self.shuffle, 
                                 callbacks=callbacks_list,
                                 **kwargs)
 
         # load the best one to predict when set PATH
         if self.PATH is not None: model = load_model(self.PATH+data.name) 
 
+        # Get results and evaluate
+        from CEEMDAN_LSTM.data_preprocessor import eval_result
+        df_loss = pd.DataFrame({'loss': history.history['loss'], 'val_loss': history.history['val_loss']}, index=range(len(history.history['val_loss'])))
         if not self.NEXT_DAY:
-            # Get results and evaluate
-            from CEEMDAN_LSTM.data_preprocessor import eval_result
+            # Get general results and evaluate
             y_predict = model(x_test) # Predict # replace y_predict = model.predict(x_test) to aviod warning
             df_eval = eval_result(y_test, y_predict) # Evaluate model
             y_predict = np.array(y_predict).ravel().reshape(-1,1) 
             if scalarY is not None: 
                 y_test = scalarY.inverse_transform(y_test)
                 y_predict = scalarY.inverse_transform(y_predict) # De-normalize 
             if self.TARGET is not None: result_index = self.TARGET.index[-self.FORECAST_LENGTH:] # Forecasting result idnex
             else: result_index = range(len(y_test.ravel()))
             df_result = pd.DataFrame({'real': y_test.ravel(), 'predict': y_predict.ravel()}, index=result_index) # Output
-            df_loss = pd.DataFrame({'loss': history.history['loss'], 'val_loss': history.history['val_loss']}, index=range(len(history.history['val_loss'])))
             return df_result, df_eval, df_loss
         else:
-            # Get next day's results and evaluate
+            # Get next day's results
             today_y = np.array(model(today_x))
             next_y = np.array(model(next_x.reshape(1, today_x.shape[1], today_x.shape[2])))
             if scalarY is not None: # De-normalize 
                 today_real = scalarY.inverse_transform([y_train[-1]])
                 today_y = scalarY.inverse_transform(today_y)
                 next_y = scalarY.inverse_transform(next_y)
             else: today_real = self.TARGET.values[-1]
@@ -372,15 +374,15 @@
         Use Keras model to directly forecast with vector input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.single_keras_predict(data, show=True, plot=True, save=True)
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data            - data set (include training set and test set)
         show            - show the inputting data set and Keras model structure
         plot            - show figure result or not
         save            - save forecasting result when set PATH
         **kwargs        - any parameters of self.keras_predict()
 
         Output
@@ -391,42 +393,25 @@
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name and set 
         now = datetime.now()
         predictor_name = name_predictor(now, 'Single', 'Keras', self.KERAS_MODEL, None, None, self.NEXT_DAY)
-        data = check_dataset(data, show, self.DECOM_MODE, self.REDECOM_LIST)
-        data.name = change_name(predictor_name+'_model.h5')
-        
-        # set target and model
-        try: 
-            if 'Keras_Forecasting' in data.name: predictor_name = data.name
-            else:
-                data.name = ''
-                self.TARGET = data['target']
-        except: 
-            data.name = ''
-            self.TARGET = data['target']
+        data = check_dataset(data, show, self.DECOM_MODE, None)
+        data.name = (predictor_name+'_model.h5').replace('-','_').replace(' ','_')
+        self.TARGET = data['target']
 
         # Forecast
         start = time.time()
         df_result = self.keras_predict(data=data, show_model=show, **kwargs)
         end = time.time()
 
         # Output
-        print('\n=========='+predictor_name+' Finished==========')
-        if not self.NEXT_DAY: 
-            df_result[1]['Runtime'] = end-start # Output Runtime
-            df_result[0].name, df_result[1].name, df_result[2].name = predictor_name+' Result', predictor_name+' Evaluation', predictor_name+' Loss'
-            print(df_result[1]) # print df_eval
-        else: 
-            df_result['Runtime'] = end-start # Output Runtime
-            df_result.name = predictor_name+' Result'
-            print(df_result)
+        df_result = output_result(df_result, predictor_name, end-start)
         plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
         return df_result
 
 
 
     # 2.2. Ensemble Method (decompose then directly forecast)
     def ensemble_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
@@ -435,15 +420,15 @@
         Use decomposition-integration Keras model to directly forecast with matrix input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.ensemble_keras_predict(data, show=True, plot=True, save=True)
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data            - data set (include training set and test set)  
         show            - show the inputting data set and Keras model structure
         plot            - show figure result or not
         save            - save forecasting result when set PATH
         **kwargs        - any parameters of self.keras_predict()       
 
         Output
@@ -459,40 +444,23 @@
         now = datetime.now()
         predictor_name = name_predictor(now, 'Ensemble', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        df_redecom.name = change_name(predictor_name+'_model.h5')
-
-        # set target and model
-        try: 
-            if 'Keras_Forecasting' in data.name: predictor_name = data.name
-            else:
-                data.name = ''
-                self.TARGET = df_redecom['target']
-        except: 
-            data.name = ''
-            self.TARGET = df_redecom['target']
+        df_redecom.name = (predictor_name+'_model.h5').replace('-','_').replace(' ','_') # model name input to self.keras_predict
+        self.TARGET = df_redecom['target']
 
         # Forecast
         df_result = self.keras_predict(data=df_redecom, show_model=show, **kwargs)
         end = time.time()
 
         # Output
-        print('\n=========='+predictor_name+' Finished==========')
-        if not self.NEXT_DAY: 
-            df_result[1]['Runtime'] = end-start # Output Runtime
-            df_result[0].name, df_result[1].name, df_result[2].name = predictor_name+' Result', predictor_name+' Evaluation', predictor_name+' Loss'
-            print(df_result[1]) # print df_eval
-        else: 
-            df_result['Runtime'] = end-start # Output Runtime
-            df_result.name = predictor_name+' Result'
-            print(df_result)
+        df_result = output_result(df_result, predictor_name, end-start)
         plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
         return df_result
 
 
     
     # 2.3. Respective Method (decompose then respectively forecast each IMFs)
     def respective_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
@@ -501,15 +469,15 @@
         Use decomposition-integration Keras model to respectively forecast each IMFs with vector input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.respective_keras_predict(data, show=True, plot=True, save=True)
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data            - data set (include training set and test set)
         show            - show the inputting data set and Keras model structure
         plot            - show figure result or not
         save            - save forecasting result when set PATH
         **kwargs        - any parameters of self.keras_predict()
 
         Output
@@ -525,77 +493,53 @@
         now = datetime.now()
         predictor_name = name_predictor(now, 'Respective', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        
+        self.TARGET = df_redecom['target']
         # set target and model
         try: 
             if 'Keras_Forecasting' in data.name: predictor_name = data.name
-            else:
-                data.name = ''
-                self.TARGET = df_redecom['target']
-        except: 
-            data.name = ''
-            self.TARGET = df_redecom['target']
+            else: data.name, self.TARGET = '', df_redecom['target']
+        except: data.name, self.TARGET = '', df_redecom['target']
 
         # Forecast and ouput each Co-IMF
         df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
         for imf in df_redecom.columns.difference(['target']):
-            df_redecom[imf].name = change_name(predictor_name+'_of_'+imf+'_model.h5')
+            df_redecom[imf].name = (predictor_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_')
             time1 = time.time()
             df_result = self.keras_predict(data=df_redecom[imf], show_model=show, **kwargs)
             time2 = time.time()
-            print('----'+predictor_name+' of '+imf+' Finished----')
-            if not self.NEXT_DAY: 
-                df_result[1]['Runtime'] = time2-time1 # Output Runtime
-                df_result[1]['IMF'] = imf
-                df_result[0].name, df_result[1].name, df_result[2].name = predictor_name+' Result of '+imf, predictor_name+' Evaluation of '+imf, predictor_name+' Loss of '+imf
-                print(df_result[1]) # print df_eval
+            df_result = output_result(df_result, predictor_name, time2-time1, imf)
+            if not self.NEXT_DAY:
                 df_pred_result[imf+'-real'] = df_result[0]['real'] # add real values
                 df_pred_result[imf+'-predict'] = df_result[0]['predict'] # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
-            else: 
-                df_result['Runtime'] = time2-time1 # Output Runtime
-                df_result['IMF'] = imf
-                df_result.name = predictor_name+' Result of '+imf
-                print(df_result)
-                df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
-            plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
+                plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
+            else: df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
             print('')
         end = time.time()
 
         # Final Output
-        print('=========='+predictor_name+' Finished==========')
-        from CEEMDAN_LSTM.data_preprocessor import eval_result
+        # Final Output
         if not self.NEXT_DAY: 
             df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
             df_pred_result['predict'] = df_pred_result[[x for x in df_pred_result.columns if 'predict' in x]].sum(axis=1)
-            final_eval = eval_result(df_pred_result['predict'], df_pred_result['real'])
-            final_eval['Runtime'] = end-start # Output Runtime
-            final_eval['IMF'] = 'Final'
-            print(final_eval) # print df_eval
-            final_eval = pd.concat((final_eval, df_eval_result))
-            df_plot = df_pred_result[['real', 'predict']]
-            df_pred_result.name, final_eval.name, df_plot.name = predictor_name+' Result', predictor_name+' Evaluation', predictor_name+' Result'
-            plot_save_result(df_plot, name=now, plot=plot, save=False, path=self.PATH)
-            df_result = (df_pred_result, final_eval)
+            df_result = output_result((df_pred_result,df_eval_result), predictor_name, end-start, imf='Final', type='Evaluation')
+            plot_save_result(df_result[2], name=now, plot=plot, save=save, path=self.PATH) # only plot result
+            df_result = (df_result[0], df_result[1])
         else:
             df_result = pd.DataFrame({'today_real': self.TARGET.values[-1], 'today_pred': df_next_result['today_pred'].sum(), 
                                       'next_pred': df_next_result['next_pred'].sum()}, index=[df_next_result.index[0]]) # Output
-            df_result['Runtime'] = end-start # Output Runtime
-            df_result['IMF'] = 'Final'
-            df_result = pd.concat((df_result, df_next_result))
-            df_result.name = predictor_name+' Result'
-            print(df_result)
-        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH)
+            df_result = output_result((df_result, df_next_result), predictor_name, end-start, imf='Final', type='Result')
+        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH) # save result 
         return df_result
 
 
 
     # 2.4. Hybrid Method (decompose then forecast high-frequency IMF by ensemble method and forecast other by respective method)
     def hybrid_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
         """
@@ -603,15 +547,15 @@
         Use the ensemble method to forecast high-frequency IMF and the respective method for other IMFs.
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.hybrid_keras_predict(data, show=True, plot=True, save=True)
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data            - data set (include training set and test set)
         show            - show the inputting data set and Keras model structure
         plot            - show figure result or not
         save            - save forecasting result when set PATH
         **kwargs        - any parameters of self.keras_predict()
 
         Output
@@ -634,67 +578,45 @@
         df_rest_columns, df_rest_list = [], []
         for x in df_redecom_list: # create df_rest_list
             df_redecom[x.name] = x['target']
             df_rest_columns.append(x.name)
             df_redecom = df_redecom[df_redecom.columns.difference(x.columns.difference(['target']))]
         for x in df_redecom.columns.difference(df_rest_columns): 
             if x != 'target': df_rest_list.append(df_redecom[x])
-
-        # set target and model
-        try: 
-            if 'Keras_Forecasting' in data.name: predictor_name = data.name
-            else:
-                data.name = ''
-                self.TARGET = df_redecom['target']
-        except: 
-            data.name = ''
-            self.TARGET = df_redecom['target']
+        self.TARGET = df_redecom['target']
 
         # Forecast
         df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
         for df in df_redecom_list+df_rest_list: # both ensemble (matrix-input) and respective (vector-input) method 
             imf = df.name
-            df.name = change_name(predictor_name+'_of_'+imf+'_model.h5') # Save model
+            df.name = (predictor_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_') # Save model
             time1 = time.time()
             df_result = self.keras_predict(data=df, show_model=show, **kwargs) # the ensemble method with matrix input 
             time2 = time.time()
-            print('\n----------'+predictor_name+' of '+imf+' Finished----------')
+            df_result = output_result(df_result, predictor_name, time2-time1, imf)
             if not self.NEXT_DAY: 
-                df_result[1]['Runtime'] = time2-time1 # Output Runtime
-                df_result[1]['IMF'] = imf
-                df_result[0].name, df_result[1].name, df_result[2].name = predictor_name+' Result of '+imf, predictor_name+' Evaluation of '+imf, predictor_name+' Loss of '+imf
-                print(df_result[1]) # print df_eval
                 df_pred_result[imf+'-real'] = df_result[0]['real'] # add real values
                 df_pred_result[imf+'-predict'] = df_result[0]['predict'] # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
                 plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
-            else: 
-                df_result['Runtime'] = time2-time1 # Output Runtime
-                df_result['IMF'] = imf
-                df_result.name = predictor_name+' Result of '+imf
-                print(df_result)
-                df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
+            else: df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
             print('')
 
         # Fitting 
         if not self.NEXT_DAY: 
             if self.FIT_METHOD == 'ensemble': # fitting method
                 print('Fitting of the ensemble method is running...')        
                 fitting_set = df_pred_result[[x for x in df_pred_result.columns if '-predict' in x]]
-                df_redecom.name = change_name(predictor_name+'_of_Fitting_model.h5') # Save model
+                df_redecom.name = (predictor_name+'_of_Fitting_model.h5').replace('-','_').replace(' ','_') # Save model
                 time1 = time.time()
                 df_result = self.keras_predict(data=df_redecom, show_model=show, fitting_set=fitting_set, **kwargs) # the ensemble method with matrix input 
                 time2 = time.time()
-                print('-------------'+predictor_name+' of Fitting Finished-------------')
-                df_result[1]['Runtime'] = time2-time1 # Output Runtime
-                df_result[1]['IMF'] = 'fitting'
-                df_result[0].name, df_result[1].name, df_result[2].name = predictor_name+' Result of Fitting', predictor_name+' Evaluation of Fitting', predictor_name+' Loss of Fitting'
-                print(df_result[1]) # print df_eval
+                df_result = output_result(df_result, predictor_name, time2-time1, 'fitting')
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
                 df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
                 df_pred_result['add-predict'] = df_pred_result[[x for x in df_pred_result.columns if '-predict' in x]].sum(axis=1) # add all imf predict result
                 df_pred_result['predict'] = df_result[0]['predict']
                 plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
             else: # adding method
                 df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
@@ -704,77 +626,61 @@
                 print('Fitting of the ensemble method is running...')        
                 fitting_set = df_redecom[df_redecom.columns.difference(['target'])][-self.FORECAST_LENGTH+1:]
                 fitting_set_next_index = fitting_set.index[-1]+(fitting_set.index[-1]-fitting_set.index[-2])
                 fitting_set.loc[fitting_set_next_index] = [x for x in range(fitting_set.columns.size)] # create blank row
                 for i in range(df_next_result.index.size): # add next_pred of each imf to fitting_set
                     point_row = df_next_result[i:i+1]
                     fitting_set[point_row['IMF'][0]][fitting_set_next_index] = point_row['next_pred'][0]
-                df_redecom.name = change_name(predictor_name+'_of_Fitting_model.h5') # Save model
+                df_redecom.name = (predictor_name+'_of_Fitting_model.h5').replace('-','_').replace(' ','_') # Save model
                 time1 = time.time()
                 df_result = self.keras_predict(data=df_redecom, show_model=show, fitting_set=fitting_set, **kwargs) # the ensemble method with matrix input 
                 time2 = time.time()
-                print('---------'+predictor_name+' of Fitting Finished---------')
-                df_result['Runtime'] = time2-time1 # Output Runtime
-                df_result['IMF'] = 'fitting'
-                df_result.name = predictor_name+' Result of Fitting'
-                print(df_result)
+                df_result = output_result(df_result, predictor_name, time2-time1, imf='fitting')
                 df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
                 today_result = df_result['today_pred']
                 next_reuslt = df_result['next_pred']
             else: # adding method
                 today_result = df_next_result['today_pred'].sum()
                 next_reuslt = df_next_result['next_pred'].sum() # adding method
         end = time.time()
 
         # Final Output
-        print('\n================'+predictor_name+' Finished================')
-        from CEEMDAN_LSTM.data_preprocessor import eval_result
         if not self.NEXT_DAY: 
-            final_eval = eval_result(df_pred_result['predict'], df_pred_result['real'])
-            final_eval['Runtime'] = end-start # Output Runtime
-            final_eval['IMF'] = 'Final'
-            print(final_eval) # print df_eval
-            final_eval = pd.concat((final_eval, df_eval_result))
-            df_plot = df_pred_result[['real', 'predict']]
-            df_pred_result.name, final_eval.name, df_plot.name = predictor_name+' Result', predictor_name+' Evaluation', predictor_name+' Result'
-            plot_save_result(df_plot, name=now, plot=plot, save=save, path=self.PATH)
-            df_result = (df_pred_result, final_eval)
+            df_result = output_result((df_pred_result,df_eval_result), predictor_name, end-start, imf='Final', type='Evaluation')
+            plot_save_result(df_result[2], name=now, plot=plot, save=save, path=self.PATH) # only plot result 
+            df_result = (df_result[0], df_result[1])
         else:
             df_result = pd.DataFrame({'today_real': self.TARGET.values[-1], 'today_pred': today_result, 'next_pred': next_reuslt}, index=[df_next_result.index[0]]) # Output
-            df_result['Runtime'] = end-start # Output Runtime
-            df_result['IMF'] = 'Final'
-            df_result = pd.concat((df_result, df_next_result))
-            df_result.name = predictor_name+' Result'
-            print(df_result)
-        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH)
+            df_result = output_result((df_result, df_next_result), predictor_name, end-start, imf='Final', type='Result')
+        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH) # save result 
         return df_result
 
     # A class used to hide the print
     class HiddenPrints: 
         """
         A class used to hide the print
         """
         def __enter__(self):
             self._original_stdout = sys.stdout
             sys.stdout = open(os.devnull, 'w')
         def __exit__(self, exc_type, exc_val, exc_tb):
             sys.stdout.close()
             sys.stdout = self._original_stdout
 
-     # 2.5. Multiple Run Predictor
+    # 2.5. Multiple Run Predictor
     def multiple_keras_predict(self, data=None, run_times=10, predict_method=None, **kwargs):
         """
         Multiple Run Predictor, multiple run of above method
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
-        df_result = kr.multiple_predict(data, run_times=10, predict_method='single')
+        df_result = kr.multiple_keras_predict(data, run_times=10, predict_method='single')
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data               - data set (include training set and test set)
         run_times          - running times
         predict_method     - run different method eg. 'single', 'ensemble', 'respective', 'hybrid'
                            - single: self.single_keras_predict()
                            - ensemble: self.ensemble_keras_predict()
                            - respective: self.respective_keras_predict()
                            - hybrid: self.hybrid_keras_predict()
@@ -832,15 +738,15 @@
         Rolling run of above method to avoid the look-ahead bias, but take a long long time
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.rolling_keras_predict(data, predict_method='single', transfer_learning=True)
 
         Input and Parameters:
         ---------------------
-        Note important hyperarameters of class cl.keras_predict()
+        Note important hyperarameters of class cl.keras_predictor()
         data               - data set (include training set and test set)
         predict_method     - run different method eg. 'single', 'ensemble', 'respective', 'hybrid'
                            - single: self.single_keras_predict()
                            - ensemble: self.ensemble_keras_predict()
                            - respective: self.respective_keras_predict()
                            - hybrid: self.hybrid_keras_predict()
         transfer_learning  - use transfer learning method, load previous model and continue training; save Keras model in .h5 file
@@ -853,16 +759,16 @@
 
         # Initialize 
         self.NEXT_DAY = True
         now = datetime.now()
         start = time.time()
         data = check_dataset(data, False, self.DECOM_MODE, self.REDECOM_LIST)
         if self.PATH is None: 
-            if transfer_learning: raise ValueError('Do not set a PATH! Please set a PATH to start transfer Learning.')
-            print('Do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
+            if transfer_learning: raise ValueError('Please set a PATH to start transfer Learning!')
+            print('You do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
         if predict_method is None: raise ValueError("Please input a predict method! eg. 'single', 'ensemble', 'respective', 'hybrid'.")
         else: predict_method = predict_method.capitalize()
         if predict_method == 'Single': predictor_name = name_predictor(now, 'Rolling Single', 'Keras', self.KERAS_MODEL, None, None, False)
         else: predictor_name = name_predictor(now, 'Rolling '+predict_method, 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, False)
         
         # Transfer Learning (save and load h5 model file)
         model, model_name = None, ''
@@ -881,30 +787,30 @@
             time2 = time.time()
             print('taking time: %.3fs'%(time2-time1))
 
             # get model name and VMD_PARAMS 
             with self.HiddenPrints():
                 model_name = name_predictor(now, predict_method, 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
             from CEEMDAN_LSTM.data_preprocessor import redecom
-            if predict_method == 'Single': model = change_name(model_name)+'_model.h5'
+            if predict_method == 'Single': model = (model_name).replace('-','_').replace(' ','_')+'_model.h5'
             else:
                 df_redecom = None
                 if self.INTE_LIST is None: print('Warning! It is recommended to set INTE_LIST. Otherwise, a different number of decomposed IMFs per run may lead to errors.')
                 if self.REDECOM_LIST is not None:
                     if 'vmd' not in str(self.REDECOM_LIST).lower(): print('Warning! It is recommended to use VMD or OVMD in REDECOM_LIST. Otherwise, a different number of decomposed IMFs per run may lead to errors.')
                     model = pd.DataFrame(index=[0])
                     if predict_method == 'Ensemble': 
-                        model = change_name(model_name)+'_model.h5'
+                        model = (model_name).replace('-','_').replace(' ','_')+'_model.h5'
                         if self.REDECOM_LIST is not None: df_redecom, df_redecom_list = redecom(data, False, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.FORECAST_LENGTH)
                     elif predict_method == 'Respective': 
                         df_redecom, df_redecom_list = redecom(data, False, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.FORECAST_LENGTH)
-                        for imf in df_redecom.columns.difference(['target']): model[imf] = change_name(model_name+'_of_'+imf+'_model.h5')
+                        for imf in df_redecom.columns.difference(['target']): model[imf] = (model_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_')
                     elif predict_method == 'Hybrid': 
                         df_redecom, df_redecom_list = redecom(data, False, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.FORECAST_LENGTH)
-                        for imf in eval(df_redecom.name.split('_')[0]): model[imf] = change_name(model_name+'_of_'+imf+'_model.h5')
+                        for imf in eval(df_redecom.name.split('_')[0]): model[imf] = (model_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_')
                     self.VMD_PARAMS = eval(df_redecom.name.split('_')[1])
                     if self.VMD_PARAMS is not None: print('Get vmd_params:', self.VMD_PARAMS)
 
         # Forecast
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'Run']) # df for storing Next-day forecasting result
         series_next_forecast = [] # record the Next-day forecasting series
         for i in range(self.FORECAST_LENGTH):
@@ -912,15 +818,15 @@
             time1 = time.time()
             with self.HiddenPrints():
                 if i == 0:
                     if model is not None: self.KERAS_MODEL = model
                 transfer_data = data[:-self.FORECAST_LENGTH+i]
                 self.TARGET = transfer_data.copy(deep=True)
                 if out_of_sample and i != 0: transfer_data['target'][-i:] = series_next_forecast
-                transfer_data.name = change_name(model_name)
+                transfer_data.name = (model_name).replace('-','_').replace(' ','_')
                 if predict_method == 'Single': df_result = self.single_keras_predict(data=transfer_data, **kwargs)
                 if predict_method == 'Ensemble': df_result = self.ensemble_keras_predict(data=transfer_data, **kwargs) 
                 if predict_method == 'Respective': df_result = self.respective_keras_predict(data=transfer_data, **kwargs)
                 if predict_method == 'Hybrid': df_result = self.hybrid_keras_predict(data=transfer_data, **kwargs)
             time2 = time.time()
             print('taking time: %.3fs'%(time2-time1))
             df_result['Run'] = i
```

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/PKG-INFO` & `CEEMDAN_LSTM-1.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: CEEMDAN-LSTM
-Version: 1.2b1
+Name: CEEMDAN_LSTM
+Version: 1.2b2
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -48,15 +48,15 @@
 ## Import and quickly predict
 ```python
 import CEEMDAN_LSTM as cl
 cl.quick_keras_predict(data=None) # default dataset: sse_index.csv
 ```
 #### Load dataset
 ```python
-data = cl.load_dataset()
+data = cl.load_dataset() # some built-in dataset eg. sp500.csv hsi.csv ftse.csv nsdaq.csv n225.csv
 # data = pd.read_csv(your_file_path + its_name + '.csv', header=0, index_col=['date'], parse_dates=['date'])
 ```
 
 ## Help and example
 You can use the code to call for a help. You can copy the code from the output of `cl.show_keras_example()` to run forecasting and help you learn more about the code.
 ```python
 cl.help()
@@ -92,16 +92,16 @@
 ```
 
 | HyperParameters | Description | 
 | :-----| :----- | 
 |PATH               |the saving path of figures and logs, eg. 'D:/CEEMDAN_LSTM/'|
 |FORECAST_HORIZONS  |the length of each input row(x_train.shape), which means the number of previous days related to today, also called Timestep, Forecast_horizons, or Sliding_windows_length in some papers|
 |FORECAST_LENGTH    |the length of the days to forecast (test set)|
-|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', 'CUDNNLSTM', 'CUDNNGRU', model = Sequential(), or load_model.|
-|DECOM_MODE         |the decomposition method, eg.'EMD', 'VMD', 'CEEMDAN'|
+|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', model = Sequential(), or load_model.|
+|DECOM_MODE         |the decomposition method, eg.'EMD', 'EEMD', 'CEEMDAN', 'VMD', 'OVMD', 'SVMD'|
 |INTE_LIST          |the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...|
 |REDECOM_LIST       |the re-decomposition list, eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame|
 |NEXT_DAY           |set True to only predict next out-of-sample value|
 |DAY_AHEAD          |define to forecast n days' ahead, eg. 0, 1, 2 (default int 1)|
 |NOR_METHOD         |the normalizing method, eg. 'minmax'-MinMaxScaler, 'std'-StandardScaler, otherwise without normalization|
 |FIT_METHOD         |the fitting method to stablize the forecasting result (not necessarily useful), eg. 'add', 'ensemble' (there some error for ensembleFIT_METHOD, please use add method as default.)|
 |USE_TPU            |change Keras model to TPU model (for google Colab)|
```

### Comparing `CEEMDAN_LSTM-1.2b1/CEEMDAN_LSTM.egg-info/SOURCES.txt` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/LICENSE` & `CEEMDAN_LSTM-1.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b1/PKG-INFO` & `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: CEEMDAN_LSTM
-Version: 1.2b1
+Name: CEEMDAN-LSTM
+Version: 1.2b2
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -48,15 +48,15 @@
 ## Import and quickly predict
 ```python
 import CEEMDAN_LSTM as cl
 cl.quick_keras_predict(data=None) # default dataset: sse_index.csv
 ```
 #### Load dataset
 ```python
-data = cl.load_dataset()
+data = cl.load_dataset() # some built-in dataset eg. sp500.csv hsi.csv ftse.csv nsdaq.csv n225.csv
 # data = pd.read_csv(your_file_path + its_name + '.csv', header=0, index_col=['date'], parse_dates=['date'])
 ```
 
 ## Help and example
 You can use the code to call for a help. You can copy the code from the output of `cl.show_keras_example()` to run forecasting and help you learn more about the code.
 ```python
 cl.help()
@@ -92,16 +92,16 @@
 ```
 
 | HyperParameters | Description | 
 | :-----| :----- | 
 |PATH               |the saving path of figures and logs, eg. 'D:/CEEMDAN_LSTM/'|
 |FORECAST_HORIZONS  |the length of each input row(x_train.shape), which means the number of previous days related to today, also called Timestep, Forecast_horizons, or Sliding_windows_length in some papers|
 |FORECAST_LENGTH    |the length of the days to forecast (test set)|
-|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', 'CUDNNLSTM', 'CUDNNGRU', model = Sequential(), or load_model.|
-|DECOM_MODE         |the decomposition method, eg.'EMD', 'VMD', 'CEEMDAN'|
+|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', model = Sequential(), or load_model.|
+|DECOM_MODE         |the decomposition method, eg.'EMD', 'EEMD', 'CEEMDAN', 'VMD', 'OVMD', 'SVMD'|
 |INTE_LIST          |the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...|
 |REDECOM_LIST       |the re-decomposition list, eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame|
 |NEXT_DAY           |set True to only predict next out-of-sample value|
 |DAY_AHEAD          |define to forecast n days' ahead, eg. 0, 1, 2 (default int 1)|
 |NOR_METHOD         |the normalizing method, eg. 'minmax'-MinMaxScaler, 'std'-StandardScaler, otherwise without normalization|
 |FIT_METHOD         |the fitting method to stablize the forecasting result (not necessarily useful), eg. 'add', 'ensemble' (there some error for ensembleFIT_METHOD, please use add method as default.)|
 |USE_TPU            |change Keras model to TPU model (for google Colab)|
```

### Comparing `CEEMDAN_LSTM-1.2b1/README.md` & `CEEMDAN_LSTM-1.2b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## Import and quickly predict
 ```python
 import CEEMDAN_LSTM as cl
 cl.quick_keras_predict(data=None) # default dataset: sse_index.csv
 ```
 #### Load dataset
 ```python
-data = cl.load_dataset()
+data = cl.load_dataset() # some built-in dataset eg. sp500.csv hsi.csv ftse.csv nsdaq.csv n225.csv
 # data = pd.read_csv(your_file_path + its_name + '.csv', header=0, index_col=['date'], parse_dates=['date'])
 ```
 
 ## Help and example
 You can use the code to call for a help. You can copy the code from the output of `cl.show_keras_example()` to run forecasting and help you learn more about the code.
 ```python
 cl.help()
@@ -76,16 +76,16 @@
 ```
 
 | HyperParameters | Description | 
 | :-----| :----- | 
 |PATH               |the saving path of figures and logs, eg. 'D:/CEEMDAN_LSTM/'|
 |FORECAST_HORIZONS  |the length of each input row(x_train.shape), which means the number of previous days related to today, also called Timestep, Forecast_horizons, or Sliding_windows_length in some papers|
 |FORECAST_LENGTH    |the length of the days to forecast (test set)|
-|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', 'CUDNNLSTM', 'CUDNNGRU', model = Sequential(), or load_model.|
-|DECOM_MODE         |the decomposition method, eg.'EMD', 'VMD', 'CEEMDAN'|
+|KERAS_MODEL        |the Keras model, eg. 'GRU', 'LSTM', 'DNN', 'BPNN', model = Sequential(), or load_model.|
+|DECOM_MODE         |the decomposition method, eg.'EMD', 'EEMD', 'CEEMDAN', 'VMD', 'OVMD', 'SVMD'|
 |INTE_LIST          |the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...|
 |REDECOM_LIST       |the re-decomposition list, eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame|
 |NEXT_DAY           |set True to only predict next out-of-sample value|
 |DAY_AHEAD          |define to forecast n days' ahead, eg. 0, 1, 2 (default int 1)|
 |NOR_METHOD         |the normalizing method, eg. 'minmax'-MinMaxScaler, 'std'-StandardScaler, otherwise without normalization|
 |FIT_METHOD         |the fitting method to stablize the forecasting result (not necessarily useful), eg. 'add', 'ensemble' (there some error for ensembleFIT_METHOD, please use add method as default.)|
 |USE_TPU            |change Keras model to TPU model (for google Colab)|
```

### Comparing `CEEMDAN_LSTM-1.2b1/setup.py` & `CEEMDAN_LSTM-1.2b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='CEEMDAN_LSTM',
-    version='1.2b1',
+    version='1.2b2',
     packages=setuptools.find_packages(),
     install_requires=['numpy >= 1.17.3',
                       'pandas >= 1.2.0',
                       'EMD-signal >= 1.2.3',
                       'optuna >= 3.0.0',
                       'vmdpy',
                       'sampen',
```

