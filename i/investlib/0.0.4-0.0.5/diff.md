# Comparing `tmp/investlib-0.0.4.tar.gz` & `tmp/investlib-0.0.5.tar.gz`

## Comparing `investlib-0.0.4.tar` & `investlib-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 investlib-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/__init__.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/data.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/filters.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/rebalance.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/strategy.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 investlib-0.0.4/investlib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_data.py
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_filters.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_rebalance.py
--rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_strategy.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 investlib-0.0.4/tests/test_utils.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.4/LICENSE
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 investlib-0.0.4/README.md
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 investlib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 investlib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 investlib-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/data.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/filters.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/rebalance.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/strategy.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/report/__init__.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/report/draw.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 investlib-0.0.5/investlib/report/templates/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/test_data.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/test_filters.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/test_rebalance.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/test_strategy.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 investlib-0.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 investlib-0.0.5/README.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 investlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 investlib-0.0.5/PKG-INFO
```

### Comparing `investlib-0.0.4/investlib/data.py` & `investlib-0.0.5/investlib/data.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/investlib/filters.py` & `investlib-0.0.5/investlib/filters.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/investlib/rebalance.py` & `investlib-0.0.5/investlib/rebalance.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/investlib/strategy.py` & `investlib-0.0.5/investlib/strategy.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,18 +46,52 @@
     
     def get_assets_to_allocate(self, equities, date):
         assets = equities.columns.tolist() 
         for f in self.filters:
             assets = f.get_filtered(equities[assets], date)
         return assets
 
+    def get_equity(self):
+        eq= self.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + self.cash['post_close']
+        eq = eq.rename('abs',inplace=True).to_frame()
+        eq['pct'] = ((1+eq['abs'].pct_change().fillna(0)).cumprod()-1)*100
+        return eq.round(2)
+
+    def get_drawdown(self):
+        eq= self.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + self.cash['post_close']
+        dd = eq-eq.cummax()
+        dd = dd.rename('abs',inplace=True).to_frame()
+        dd['pct'] = (eq/eq.cummax()-1)*100
+        return dd.round(2)
+
+    def get_loss_period(self):
+        dd = self.get_drawdown()['abs']
+        dd_zero = dd[dd==0].index
+        end_date = dd_zero.to_series().diff().idxmax()
+        start_locix = dd_zero.get_loc(end_date)-1
+        start_date = dd_zero[dd_zero.to_list().index(dd_zero[start_locix])]
+        loss_days = dd_zero.to_series().diff().max().days-1
+        return (start_date, end_date, loss_days)
+
+    def get_duration(self):
+        """
+            Approximate average number of days in a year, taking leap years into account
+        """
+        equity = self.get_equity()['abs']
+        return round((equity.index[-1]-equity.index[0]).days/365.25,1)
+         
+    def get_cagr(self):
+        equity = self.get_equity()['abs']
+        t = self.get_duration()
+        return round((pow(equity.iloc[-1]/equity.iloc[0],1/t)-1)*100,2)
+
     def run(self):
         history = self.load_data()
         self.init_run(history)
-        timer = MonthlyTimer(months=1, day=FirstFriday())
+        #timer = MonthlyTimer(months=1, day=FirstFriday())
         #timer.set_rebalancing_days(pd.to_datetime(self.start), pd.to_datetime(self.end))
         invest_range = history.copy()
         invest_range = invest_range.loc[self.start:self.end]
         self.history=history
         for i, date in invest_range.iterrows():
             self.quantity.loc[i,:] = self.quantity.shift(1).fillna(0).loc[i,:]*history.loc[i].xs('splitFactor',  level=1)
             # CASO DI NON RIBILANCIAMENTO
@@ -95,9 +129,7 @@
                 quantity = (capital_to_use/current_close).fillna(0).round(2).apply(math.floor)
                 self.quantity.loc[i, :] += quantity
                 #self.quantity.loc[i, pos_asset] += (capital_to_use/current_close).apply(math.floor)
                 self.invested.loc[i, (slice(None), 'current')] = history.loc[i].xs('close',  level=1).mul(quantity).tolist()
                 self.invested.loc[i, (slice(None), 'value')] = self.quantity.loc[i,:].mul(history.loc[i].xs('close',  level=1)).tolist()
 
             self.cash.loc[i, 'post_close'] = self.cash.loc[i, 'pre_close']-self.invested.loc[i, (slice(None), 'current')].sum()
-        
-        self.equity = self.invested.loc[:, (slice(None), 'value')].droplevel(1, axis=1).sum(axis=1) + self.cash['post_close']
```

### Comparing `investlib-0.0.4/tests/test_data.py` & `investlib-0.0.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/tests/test_filters.py` & `investlib-0.0.5/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/tests/test_rebalance.py` & `investlib-0.0.5/tests/test_rebalance.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/tests/test_strategy.py` & `investlib-0.0.5/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/tests/test_utils.py` & `investlib-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/.gitignore` & `investlib-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/LICENSE` & `investlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `investlib-0.0.4/README.md` & `investlib-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,33 @@
 
 ## Data
 The current unique data source is Tiingo. InvestLib automatically manages cash to avoid making repeated data calls. To use this feature, you need to create a free account on Tiingo and set the following environment variables:
 
 - **tiingo_api_key**: the API token provided by Tiingo upon subscription
 - **tiingo_backup_path**: the folder where you want to save the end-of-day CSV data for all the ETFs you need (default '/tmp/Tiingo'). 
 
-## Examples
+# Installation 
+
+I raccomand to use virtualenv:
+    
+    pip install investlib
+
+## Example
 
 Here's some code to test out some famous **portfolios**:
 
 ### 60/40 (60 stocks/40 bond)
 
     import os
-    import pandas as pd
-    import plotly.graph_objects as go
     
     from investlib.strategy import Strategy
     from investlib.rebalance import FixedAllocation
     from investlib.rebalance import MonthlyTimer
     from investlib.rebalance import FirstFriday
+    from investlib.report.draw import generate_report
     
     os.environ['tiingo_api_key'] = '<tiingo_api_key>'
     
     start = '2007-01-01'
     end = '2021-06-04'
     tickers = ['VTI', 'IEF']
     
@@ -56,21 +61,16 @@
         start=start, 
         end=end, 
         timer=MonthlyTimer(months=1, day=FirstFriday()),
         allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4})
     )
     s.run()
    
-    # Plot the results
-    fig = go.Figure()
-    fig.add_trace(go.Scatter(x=s.invested.index, y=s.equity, name='6040'))
-    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI'))
-
-    fig.show()
-
+    generate_report(s, path='/tmp/6040.pdf', name='60/40')
     
 ### Futures 
     - Add more stats
+    - Add more source of data
     - Currency
     - Tax
     - Portfolio over Strategy
```

### Comparing `investlib-0.0.4/pyproject.toml` & `investlib-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "investlib"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Cellarosi Marco", email="cellarosi@gmail.com" },
 ]
 description = "InvestLib is a Python package for backtesting ETF investments"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `investlib-0.0.4/PKG-INFO` & `investlib-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investlib
-Version: 0.0.4
+Version: 0.0.5
 Summary: InvestLib is a Python package for backtesting ETF investments
 Project-URL: Homepage, https://github.com/cellarosi/investlib
 Project-URL: Bug Tracker, https://github.com/cellarosi/investlib/issues
 Author-email: Cellarosi Marco <cellarosi@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,28 +51,33 @@
 
 ## Data
 The current unique data source is Tiingo. InvestLib automatically manages cash to avoid making repeated data calls. To use this feature, you need to create a free account on Tiingo and set the following environment variables:
 
 - **tiingo_api_key**: the API token provided by Tiingo upon subscription
 - **tiingo_backup_path**: the folder where you want to save the end-of-day CSV data for all the ETFs you need (default '/tmp/Tiingo'). 
 
-## Examples
+# Installation 
+
+I raccomand to use virtualenv:
+    
+    pip install investlib
+
+## Example
 
 Here's some code to test out some famous **portfolios**:
 
 ### 60/40 (60 stocks/40 bond)
 
     import os
-    import pandas as pd
-    import plotly.graph_objects as go
     
     from investlib.strategy import Strategy
     from investlib.rebalance import FixedAllocation
     from investlib.rebalance import MonthlyTimer
     from investlib.rebalance import FirstFriday
+    from investlib.report.draw import generate_report
     
     os.environ['tiingo_api_key'] = '<tiingo_api_key>'
     
     start = '2007-01-01'
     end = '2021-06-04'
     tickers = ['VTI', 'IEF']
     
@@ -83,21 +88,16 @@
         start=start, 
         end=end, 
         timer=MonthlyTimer(months=1, day=FirstFriday()),
         allocation_class=FixedAllocation({'VTI':0.6,'IEF':0.4})
     )
     s.run()
    
-    # Plot the results
-    fig = go.Figure()
-    fig.add_trace(go.Scatter(x=s.invested.index, y=s.equity, name='6040'))
-    fig.add_trace(go.Scatter(x=bench.invested.index, y=bench_eq, name='VTI'))
-
-    fig.show()
-
+    generate_report(s, path='/tmp/6040.pdf', name='60/40')
     
 ### Futures 
     - Add more stats
+    - Add more source of data
     - Currency
     - Tax
     - Portfolio over Strategy
```

