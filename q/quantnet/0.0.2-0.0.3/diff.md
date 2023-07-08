# Comparing `tmp/quantnet-0.0.2.tar.gz` & `tmp/quantnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnet-0.0.2.tar", last modified: Sat May 15 13:31:25 2021, max compression
+gzip compressed data, was "quantnet-0.0.3.tar", last modified: Sat Jul  8 13:55:24 2023, max compression
```

## Comparing `quantnet-0.0.2.tar` & `quantnet-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 brilhana   (501) staff       (20)        0 2021-05-15 13:31:25.044099 quantnet-0.0.2/
--rw-r--r--   0 brilhana   (501) staff       (20)     1062 2021-05-11 21:12:07.000000 quantnet-0.0.2/LICENSE.md
--rw-r--r--   0 brilhana   (501) staff       (20)     1004 2021-05-15 13:31:25.044250 quantnet-0.0.2/PKG-INFO
--rw-r--r--   0 brilhana   (501) staff       (20)      349 2021-05-15 13:23:13.000000 quantnet-0.0.2/README.md
-drwxr-xr-x   0 brilhana   (501) staff       (20)        0 2021-05-15 13:31:24.965319 quantnet-0.0.2/quantnet/
--rw-r--r--   0 brilhana   (501) staff       (20)        0 2021-05-15 13:20:17.000000 quantnet-0.0.2/quantnet/__init__.py
--rw-r--r--   0 brilhana   (501) staff       (20)     6989 2021-05-15 13:09:20.000000 quantnet-0.0.2/quantnet/baseline.py
-drwxr-xr-x   0 brilhana   (501) staff       (20)        0 2021-05-15 13:31:25.003095 quantnet-0.0.2/quantnet/global/
--rw-r--r--   0 brilhana   (501) staff       (20)        0 2021-05-15 13:20:29.000000 quantnet-0.0.2/quantnet/global/__init__.py
--rwxr--r--   0 brilhana   (501) staff       (20)     7276 2021-05-15 12:58:13.000000 quantnet-0.0.2/quantnet/global/linear_linear.py
--rwxr--r--   0 brilhana   (501) staff       (20)    10107 2021-05-15 12:56:31.000000 quantnet-0.0.2/quantnet/global/linear_lstm.py
--rwxr--r--   0 brilhana   (501) staff       (20)     8108 2021-05-15 12:56:26.000000 quantnet-0.0.2/quantnet/global/lstm_linear.py
--rwxr--r--   0 brilhana   (501) staff       (20)    10844 2021-05-15 12:56:21.000000 quantnet-0.0.2/quantnet/global/lstm_lstm.py
-drwxr-xr-x   0 brilhana   (501) staff       (20)        0 2021-05-15 13:31:25.032654 quantnet-0.0.2/quantnet/no_transfer/
--rw-r--r--   0 brilhana   (501) staff       (20)        0 2021-05-15 13:20:24.000000 quantnet-0.0.2/quantnet/no_transfer/__init__.py
--rwxr--r--   0 brilhana   (501) staff       (20)     5411 2021-05-15 12:56:38.000000 quantnet-0.0.2/quantnet/no_transfer/linear.py
--rwxr--r--   0 brilhana   (501) staff       (20)     6849 2021-05-15 12:58:30.000000 quantnet-0.0.2/quantnet/no_transfer/lstm.py
--rw-r--r--   0 brilhana   (501) staff       (20)      125 2021-05-15 13:17:28.000000 quantnet-0.0.2/quantnet/quantnet.py
--rwxr--r--   0 brilhana   (501) staff       (20)     2946 2021-05-15 13:16:56.000000 quantnet-0.0.2/quantnet/utils.py
-drwxr-xr-x   0 brilhana   (501) staff       (20)        0 2021-05-15 13:31:24.971310 quantnet-0.0.2/quantnet.egg-info/
--rw-r--r--   0 brilhana   (501) staff       (20)     1004 2021-05-15 13:31:24.000000 quantnet-0.0.2/quantnet.egg-info/PKG-INFO
--rw-r--r--   0 brilhana   (501) staff       (20)      493 2021-05-15 13:31:24.000000 quantnet-0.0.2/quantnet.egg-info/SOURCES.txt
--rw-r--r--   0 brilhana   (501) staff       (20)        1 2021-05-15 13:31:24.000000 quantnet-0.0.2/quantnet.egg-info/dependency_links.txt
--rw-r--r--   0 brilhana   (501) staff       (20)        9 2021-05-15 13:31:24.000000 quantnet-0.0.2/quantnet.egg-info/top_level.txt
--rw-r--r--   0 brilhana   (501) staff       (20)       79 2021-05-15 13:31:25.044784 quantnet-0.0.2/setup.cfg
--rw-r--r--   0 brilhana   (501) staff       (20)      839 2021-05-15 13:31:20.000000 quantnet-0.0.2/setup.py
+drwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-08 13:55:24.768916 quantnet-0.0.3/
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)     1037 2023-07-08 13:35:54.000000 quantnet-0.0.3/LICENSE.md
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)      922 2023-07-08 13:55:24.768976 quantnet-0.0.3/PKG-INFO
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)      338 2023-07-08 13:35:42.000000 quantnet-0.0.3/README.md
+drwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-08 13:55:24.767149 quantnet-0.0.3/quantnet/
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-08 13:04:47.000000 quantnet-0.0.3/quantnet/__init__.py
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)     8429 2023-07-08 13:35:17.000000 quantnet-0.0.3/quantnet/app.py
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)     7103 2023-07-08 13:39:26.000000 quantnet-0.0.3/quantnet/baselines.py
+drwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-08 13:55:24.768772 quantnet-0.0.3/quantnet/no_transfer/
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-04 23:48:15.000000 quantnet-0.0.3/quantnet/no_transfer/__init__.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)     5416 2023-07-04 23:56:38.000000 quantnet-0.0.3/quantnet/no_transfer/linear.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)     7279 2023-07-04 23:56:54.000000 quantnet-0.0.3/quantnet/no_transfer/linear_linear.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)    10080 2023-07-04 23:57:00.000000 quantnet-0.0.3/quantnet/no_transfer/linear_lstm.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)     6844 2023-07-08 12:36:54.000000 quantnet-0.0.3/quantnet/no_transfer/lstm.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)     8115 2023-07-05 00:20:32.000000 quantnet-0.0.3/quantnet/no_transfer/lstm_linear.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)    10817 2023-07-05 00:20:18.000000 quantnet-0.0.3/quantnet/no_transfer/lstm_lstm.py
+-rwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)     2948 2023-07-08 13:39:46.000000 quantnet-0.0.3/quantnet/utils.py
+drwxr-xr-x   0 alexandre-brilhante   (501) staff       (20)        0 2023-07-08 13:55:24.767716 quantnet-0.0.3/quantnet.egg-info/
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)      922 2023-07-08 13:55:24.000000 quantnet-0.0.3/quantnet.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)      481 2023-07-08 13:55:24.000000 quantnet-0.0.3/quantnet.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)        1 2023-07-08 13:55:24.000000 quantnet-0.0.3/quantnet.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)        9 2023-07-08 13:55:24.000000 quantnet-0.0.3/quantnet.egg-info/top_level.txt
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)       79 2023-07-08 13:55:24.769238 quantnet-0.0.3/setup.cfg
+-rw-r--r--   0 alexandre-brilhante   (501) staff       (20)      839 2023-07-08 13:37:10.000000 quantnet-0.0.3/setup.py
```

### Comparing `quantnet-0.0.2/LICENSE.md` & `quantnet-0.0.3/LICENSE.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Alexandre Brilhante
+Copyright (c)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `quantnet-0.0.2/quantnet/baseline.py` & `quantnet-0.0.3/quantnet/no_transfer/linear_linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,198 @@
-import pickle
-import random
-from time import time
-
-import numpy as np
-import pandas as pd
-from sklearn.gaussian_process import GaussianProcessRegressor
-from sklearn.gaussian_process.kernels import (
-    RBF,
-    ExpSineSquared,
-    RationalQuadratic,
-    WhiteKernel,
-)
-from sklearn.linear_model import LinearRegression, MultiTaskElasticNetCV
-from sklearn.model_selection import TimeSeriesSplit
-from sktime.pipeline import Pipeline
-from sktime.regressors import TimeSeriesForestRegressor
-from sktime.transformers.compose import ColumnConcatenator
-
-
-class BuyAndHold:
-    def __init__(self, x_tasks, model_config):
-        self.Xtrain_tasks = x_tasks
-        self.export_path = model_config["export_path"]
-        self.export_label = model_config["export_label"]
-        self.mtl_list = self.Xtrain_tasks.keys()
-        self.sub_mtl_list = {}
-        self.signal = {}
-
-        for tk in self.mtl_list:
-            self.signal[tk] = {}
-            self.sub_mtl_list[tk] = self.Xtrain_tasks[tk].keys()
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                self.signal[tk][sub_tk] = LinearRegression()
-
-    def train(self):
-        for tk in self.mtl_list:
-            for sub_tk in self.sub_mtl_list[tk]:
-                X_train = self.Xtrain_tasks[tk][sub_tk][:-1, :]
-                Y_train = self.Xtrain_tasks[tk][sub_tk][1:, :]
-
-                self.signal[tk][sub_tk].fit(X_train, Y_train)
-                self.signal[tk][sub_tk].intercept_ = 1.0
-                self.signal[tk][sub_tk].coef_ = self.signal[tk][sub_tk].coef_ * 0.0
-
-                print(tk, sub_tk)
-
-    def predict(self, x_test):
-        y_pred = {}
-
-        for tk in self.mtl_list:
-            y_pred[tk] = {}
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                y_pred[tk][sub_tk] = self.signal[tk][sub_tk].predict(x_test[tk][sub_tk])
-
-        return y_pred
-
-
-class RiskParity:
-    def __init__(self, x_tasks, model_config):
-        self.Xtrain_tasks = x_tasks
-        self.export_path = model_config["export_path"]
-        self.export_label = model_config["export_label"]
-        self.window = model_config["risk_parity"]["window"]
-
-        self.mtl_list = self.Xtrain_tasks.keys()
-        self.sub_mtl_list = {}
-        self.signal = {}
-
-        for tk in self.mtl_list:
-            self.signal[tk] = {}
-            self.sub_mtl_list[tk] = self.Xtrain_tasks[tk].keys()
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                self.signal[tk][sub_tk] = LinearRegression()
-
-    def train(self):
-        for tk in self.mtl_list:
-            for sub_tk in self.sub_mtl_list[tk]:
-                X_train = self.Xtrain_tasks[tk][sub_tk][self.window : -1, :]
-                Y_train = self.Xtrain_tasks[tk][sub_tk][self.window + 1 :, :]
-
-                print(tk, sub_tk)
-
-    def predict(self, x_test):
-        y_pred = {}
-
-        for tk in self.mtl_list:
-            y_pred[tk] = {}
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                x = pd.DataFrame(
-                    np.concatenate(
-                        [self.Xtrain_tasks[tk][sub_tk], x_test[tk][sub_tk]], axis=0
-                    )
-                )
-                risk = (
-                    x.rolling(window=self.window)
-                    .std()
-                    .values[-x_test[tk][sub_tk].shape[0] :, :]
-                )
-                y_pred[tk][sub_tk] = (1.0 / risk) / np.repeat(
-                    np.sum((1.0 / risk), axis=1).reshape(-1, 1), risk.shape[1], axis=1
-                )
-
-        return y_pred
-
-
-class TimeSeriesMomentum:
-    def __init__(self, x_tasks, model_config):
-        self.Xtrain_tasks = x_tasks
-        self.export_path = model_config["export_path"]
-        self.export_label = model_config["export_label"]
-        self.window = model_config["ts_mom"]["window"]
-
-        self.mtl_list = self.Xtrain_tasks.keys()
-        self.sub_mtl_list = {}
-        self.signal = {}
-
-        for tk in self.mtl_list:
-            self.signal[tk] = {}
-            self.sub_mtl_list[tk] = self.Xtrain_tasks[tk].keys()
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                self.signal[tk][sub_tk] = LinearRegression()
-
-                print(tk, sub_tk)
-
-    def train(self):
-        for tk in self.mtl_list:
-            for sub_tk in self.sub_mtl_list[tk]:
-                X_train = pd.DataFrame(self.Xtrain_tasks[tk][sub_tk][:-1, :])
-                Y_train = pd.DataFrame(self.Xtrain_tasks[tk][sub_tk][1:, :])
-
-                print(tk, sub_tk)
-
-    def predict(self, x_test):
-        y_pred = {}
-
-        for tk in self.mtl_list:
-            y_pred[tk] = {}
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                x = pd.DataFrame(
-                    np.concatenate(
-                        [self.Xtrain_tasks[tk][sub_tk], x_test[tk][sub_tk]], axis=0
-                    )
-                )
-                y_pred[tk][sub_tk] = (
-                    -x.rolling(window=self.window)
-                    .mean()
-                    .values[-x_test[tk][sub_tk].shape[0] :, :]
-                )
-
-        return y_pred
-
-
-class CrossSectionalMomentum:
-    def __init__(self, x_tasks, model_config):
-        self.Xtrain_tasks = x_tasks
-        self.export_path = model_config["export_path"]
-        self.export_label = model_config["export_label"]
-        self.window = model_config["csec_mom"]["window"]
-        self.fraction = model_config["csec_mom"]["fraction"]
-
-        self.mtl_list = self.Xtrain_tasks.keys()
-        self.sub_mtl_list = {}
-        self.signal = {}
-
-        for tk in self.mtl_list:
-            self.signal[tk] = {}
-            self.sub_mtl_list[tk] = self.Xtrain_tasks[tk].keys()
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                self.signal[tk][sub_tk] = LinearRegression()
-
-                print(tk, sub_tk)
-
-    def train(self):
-        for tk in self.mtl_list:
-            for sub_tk in self.sub_mtl_list[tk]:
-                X_train = pd.DataFrame(self.Xtrain_tasks[tk][sub_tk][:-1, :])
-                Y_train = pd.DataFrame(self.Xtrain_tasks[tk][sub_tk][1:, :])
-
-                print(tk, sub_tk)
-
-    def predict(self, x_test):
-        y_pred = {}
-
-        for tk in self.mtl_list:
-            y_pred[tk] = {}
-
-            for sub_tk in self.sub_mtl_list[tk]:
-                x = pd.DataFrame(
-                    np.concatenate(
-                        [self.Xtrain_tasks[tk][sub_tk], x_test[tk][sub_tk]], axis=0
-                    )
-                )
-                signal = (
-                    x.rolling(window=self.window)
-                    .mean()
-                    .values[-x_test[tk][sub_tk].shape[0] :, :]
-                )
-                bottom = (
-                    pd.DataFrame(signal).rank(axis=1) / signal.shape[1]
-                ).values < self.fraction
-                top = (pd.DataFrame(signal).rank(axis=1) / signal.shape[1]).values > (
-                    1 - self.fraction
-                )
-                y_pred[tk][sub_tk] = np.multiply(-signal, (bottom + top))
-
-        return y_pred
+import numpy as np
+import torch
+from torch import nn
+
+
+class GlobalLinearLinear:
+    def __init__(self, x_tasks, model_config):
+        self.criterion = self.avg_sharpe_ratio
+        self.X_train_tasks = x_tasks
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
+        self.batch_size = model_config["batch_size"]
+        self.seq_len = model_config["seq_len"]
+        self.device = model_config["device"]
+        self.export_path = model_config["export_path"]
+        self.export_label = model_config["export_label"]
+        self.opt_lr = model_config["global_linear_linear"]["opt_lr"]
+        self.amsgrad = model_config["global_linear_linear"]["amsgrad"]
+        self.export_weights = model_config["global_linear_linear"]["export_weights"]
+        self.in_transfer_dim = model_config["global_linear_linear"]["in_transfer_dim"]
+        self.out_transfer_dim = model_config["global_linear_linear"]["out_transfer_dim"]
+
+        self.mtl_list = self.X_train_tasks.keys()
+
+        self.sub_mtl_list = {}
+        (
+            self.model_in_dict,
+            self.model_out_dict,
+            self.opt_dict,
+            self.signal_layer,
+            self.losses,
+        ) = ({}, {}, {}, {}, {})
+
+        self.global_transfer_linear = (
+            nn.Linear(self.in_transfer_dim, self.out_transfer_dim)
+            .double()
+            .to(self.device)
+        )
+
+        for tk in self.mtl_list:
+            (
+                self.model_in_dict[tk],
+                self.model_out_dict[tk],
+                self.signal_layer[tk],
+                self.opt_dict[tk],
+                self.losses[tk],
+            ) = ({}, {}, {}, {}, {})
+
+            self.sub_mtl_list[tk] = self.X_train_tasks[tk].keys()
+
+            for sub_tk in self.sub_mtl_list[tk]:
+                self.losses[tk][sub_tk] = []
+                nin = self.X_train_tasks[tk][sub_tk].shape[1]
+                nout = self.X_train_tasks[tk][sub_tk].shape[1]
+
+                self.model_in_dict[tk][sub_tk] = (
+                    nn.Linear(nin, self.in_transfer_dim).double().to(self.device)
+                )
+                self.model_out_dict[tk][sub_tk] = (
+                    nn.Linear(self.out_transfer_dim, nout).double().to(self.device)
+                )
+                self.signal_layer[tk][sub_tk] = nn.Tanh().to(self.device)
+
+                self.opt_dict[tk][sub_tk] = torch.optim.Adam(
+                    list(self.model_in_dict[tk][sub_tk].parameters())
+                    + list(self.model_out_dict[tk][sub_tk].parameters())
+                    + list(self.global_transfer_linear.parameters())
+                    + list(self.signal_layer[tk][sub_tk].parameters()),
+                    lr=self.opt_lr,
+                    amsgrad=self.amsgrad,
+                )
+
+                print(
+                    tk,
+                    sub_tk,
+                    self.model_in_dict[tk][sub_tk],
+                    self.model_out_dict[tk][sub_tk],
+                    self.model_lin_dict[tk][sub_tk],
+                    self.transfer_linear,
+                    self.signal_layer[tk][sub_tk],
+                    self.opt_dict[tk][sub_tk],
+                )
+
+    def train(self):
+        for i in range(self.t_steps):
+            for tk in self.mtl_list:
+                for sub_tk in self.sub_mtl_list[tk]:
+                    start_ids = np.random.permutation(
+                        list(
+                            range(
+                                self.X_train_tasks[tk][sub_tk].size(0)
+                                - self.seq_len
+                                - 1
+                            )
+                        )
+                    )[: self.batch_size]
+
+                    X_Y_batch = torch.stack(
+                        [
+                            self.X_train_tasks[tk][sub_tk][i : i + self.seq_len + 1]
+                            for i in start_ids
+                        ],
+                        dim=0,
+                    )
+
+                    Y_train = X_Y_batch[:, 1:, :]
+                    X_train = X_Y_batch[:, :-1, :]
+
+                    self.opt_dict[tk][sub_tk].zero_grad()
+
+                    in_pred = self.model_in_dict[tk][sub_tk](X_train)
+                    global_pred = self.global_transfer_linear(in_pred)
+
+                    preds = self.signal_layer[tk][sub_tk](
+                        self.model_out_dict[tk][sub_tk](global_pred)
+                    )
+
+                    loss = self.criterion(preds, Y_train)
+                    self.losses[tk][sub_tk].append(loss.item())
+
+                    loss.backward()
+                    self.opt_dict[tk][sub_tk].step()
+
+            if (i % 100) == 1:
+                print(i)
+
+        if self.export_weights:
+            for tk in self.mtl_list:
+                for sub_tk in self.sub_mtl_list[tk]:
+                    torch.save(
+                        self.model_in_dict[tk][sub_tk],
+                        self.export_path
+                        + tk
+                        + "_"
+                        + sub_tk
+                        + "_"
+                        + self.export_label
+                        + "_intransferlinear.pt",
+                    )
+
+                    torch.save(
+                        self.model_out_dict[tk][sub_tk],
+                        self.export_path
+                        + tk
+                        + "_"
+                        + sub_tk
+                        + "_"
+                        + self.export_label
+                        + "_outtransferlinear.pt",
+                    )
+
+                torch.save(
+                    self.global_transfer_linear,
+                    self.export_path
+                    + tk
+                    + "_"
+                    + self.export_label
+                    + "_globaltransferlinear.pt",
+                )
+
+    def predict(self, x_test):
+        y_pred = {}
+
+        for tk in self.mtl_list:
+            y_pred[tk] = {}
+
+            for sub_tk in self.sub_mtl_list[tk]:
+                x_flat = x_test[tk][sub_tk].view(1, -1, x_test[tk][sub_tk].size(1))
+
+                with torch.autograd.no_grad():
+                    in_pred = self.model_in_dict[tk][sub_tk](x_flat[:, :-1])
+                    global_pred = self.global_transfer_linear(in_pred)
+                    y_pred[tk][sub_tk] = self.signal_layer[tk][sub_tk](
+                        self.model_out_dict[tk][sub_tk](global_pred)
+                    )
+
+        return y_pred
+
+    def avg_sharpe_ratio(self, output, target):
+        slip = 0.0005 * 0.00
+        bp = 0.0020 * 0.00
+        rets = torch.mul(output, target)
+
+        tc = torch.abs(output[:, 1:, :] - output[:, :-1, :]) * (bp + slip)
+        tc = torch.cat(
+            [
+                torch.zeros(output.size(0), 1, output.size(2)).double().to(self.device),
+                tc,
+            ],
+            dim=1,
+        )
+
+        rets = rets - tc
+        avg_rets = torch.mean(rets)
+        vol_rets = torch.std(rets)
+        loss = torch.neg(torch.div(avg_rets, vol_rets))
+
+        return loss.mean()
```

### Comparing `quantnet-0.0.2/quantnet/global/linear_linear.py` & `quantnet-0.0.3/quantnet/no_transfer/lstm_linear.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 import numpy as np
 import torch
 from torch import nn
 
 
-class GlobalLinearLinear:
+class GlobalLstmLinear:
     def __init__(
         self, x_tasks, model_config):
         self.criterion = self.avg_sharpe_ratio
         self.X_train_tasks = x_tasks
-        self.tsteps = model_config["tsteps"]
-        self.tasks_tsteps = model_config["tasks_tsteps"]
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
         self.batch_size = model_config["batch_size"]
         self.seq_len = model_config["seq_len"]
         self.device = model_config["device"]
         self.export_path = model_config["export_path"]
         self.export_label = model_config["export_label"]
-        self.opt_lr = model_config["global_linear_linear"]["opt_lr"]
-        self.amsgrad = model_config["global_linear_linear"]["amsgrad"]
-        self.export_weights = model_config["global_linear_linear"]["export_weights"]
-        self.in_transfer_dim = model_config["global_linear_linear"]["in_transfer_dim"]
-        self.out_transfer_dim = model_config["global_linear_linear"]["out_transfer_dim"]
+        self.opt_lr = model_config["global_lstm_linear"]["opt_lr"]
+        self.amsgrad = model_config["global_lstm_linear"]["amsgrad"]
+        self.export_weights = model_config["global_lstm_linear"]["export_model"]
+        self.in_transfer_dim = model_config["global_lstm_linear"]["in_transfer_dim"]
+        self.out_transfer_dim = model_config["global_lstm_linear"]["out_transfer_dim"]
+        self.transfer_layers = model_config["global_lstm_linear"]["n_layers"]
+        self.dropout = model_config["global_lstm_linear"]["drop_rate"]
 
         self.mtl_list = self.X_train_tasks.keys()
 
         self.sub_mtl_list = {}
         (
             self.model_in_dict,
             self.model_out_dict,
             self.opt_dict,
             self.signal_layer,
             self.losses,
         ) = ({}, {}, {}, {}, {})
 
-        self.global_transfer_linear = (
-            nn.Linear(self.in_transfer_dim, self.out_transfer_dim)
+        self.global_transfer_lstm = (
+            nn.LSTM(
+                self.in_transfer_dim,
+                self.out_transfer_dim,
+                self.transfer_layers,
+                batch_first=True,
+                dropout=self.dropout,
+            )
             .double()
             .to(self.device)
         )
 
         for tk in self.mtl_list:
             (
                 self.model_in_dict[tk],
                 self.model_out_dict[tk],
                 self.signal_layer[tk],
                 self.opt_dict[tk],
                 self.losses[tk],
             ) = ({}, {}, {}, {}, {})
+
             self.sub_mtl_list[tk] = self.X_train_tasks[tk].keys()
 
             for sub_tk in self.sub_mtl_list[tk]:
                 self.losses[tk][sub_tk] = []
                 nin = self.X_train_tasks[tk][sub_tk].shape[1]
                 nout = self.X_train_tasks[tk][sub_tk].shape[1]
 
@@ -60,60 +69,62 @@
                     nn.Linear(self.out_transfer_dim, nout).double().to(self.device)
                 )
                 self.signal_layer[tk][sub_tk] = nn.Tanh().to(self.device)
 
                 self.opt_dict[tk][sub_tk] = torch.optim.Adam(
                     list(self.model_in_dict[tk][sub_tk].parameters())
                     + list(self.model_out_dict[tk][sub_tk].parameters())
-                    + list(self.global_transfer_linear.parameters())
+                    + list(self.global_transfer_lstm.parameters())
                     + list(self.signal_layer[tk][sub_tk].parameters()),
                     lr=self.opt_lr,
                     amsgrad=self.amsgrad,
                 )
 
                 print(
                     tk,
                     sub_tk,
                     self.model_in_dict[tk][sub_tk],
                     self.model_out_dict[tk][sub_tk],
-                    self.model_lin_dict[tk][sub_tk],
-                    self.transfer_linear,
+                    self.global_transfer_lstm,
                     self.signal_layer[tk][sub_tk],
                     self.opt_dict[tk][sub_tk],
                 )
 
     def train(self):
-        for i in range(self.tsteps):
+        for i in range(self.t_steps):
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     start_ids = np.random.permutation(
                         list(
                             range(
                                 self.X_train_tasks[tk][sub_tk].size(0)
                                 - self.seq_len
                                 - 1
                             )
                         )
                     )[: self.batch_size]
-
                     X_Y_batch = torch.stack(
                         [
                             self.X_train_tasks[tk][sub_tk][i : i + self.seq_len + 1]
                             for i in start_ids
                         ],
                         dim=0,
                     )
-
                     Y_train = X_Y_batch[:, 1:, :]
                     X_train = X_Y_batch[:, :-1, :]
 
                     self.opt_dict[tk][sub_tk].zero_grad()
 
                     in_pred = self.model_in_dict[tk][sub_tk](X_train)
-                    global_pred = self.global_transfer_linear(in_pred)
+
+                    (hidden, cell) = self.get_hidden(
+                        self.batch_size, self.transfer_layers, self.in_transfer_dim
+                    )
+                    global_pred, _ = self.global_transfer_lstm(in_pred, (hidden, cell))
+
                     preds = self.signal_layer[tk][sub_tk](
                         self.model_out_dict[tk][sub_tk](global_pred)
                     )
 
                     loss = self.criterion(preds, Y_train)
                     self.losses[tk][sub_tk].append(loss.item())
 
@@ -132,45 +143,51 @@
                         + tk
                         + "_"
                         + sub_tk
                         + "_"
                         + self.export_label
                         + "_intransferlinear.pt",
                     )
+
                     torch.save(
                         self.model_out_dict[tk][sub_tk],
                         self.export_path
                         + tk
                         + "_"
                         + sub_tk
                         + "_"
                         + self.export_label
                         + "_outtransferlinear.pt",
                     )
+
                 torch.save(
-                    self.global_transfer_linear,
+                    self.global_transfer_lstm,
                     self.export_path
                     + tk
                     + "_"
                     + self.export_label
-                    + "_globaltransferlinear.pt",
+                    + "_globaltransferlstm.pt",
                 )
 
     def predict(self, x_test):
         y_pred = {}
 
         for tk in self.mtl_list:
             y_pred[tk] = {}
 
             for sub_tk in self.sub_mtl_list[tk]:
-                x_flat = x_test[tk][sub_tk].view(1, -1, x_test[tk][sub_tk].size(1))
+                xflat = x_test[tk][sub_tk].view(1, -1, x_test[tk][sub_tk].size(1))
 
                 with torch.autograd.no_grad():
-                    in_pred = self.model_in_dict[tk][sub_tk](x_flat[:, :-1])
-                    global_pred = self.global_transfer_linear(in_pred)
+                    in_pred = self.model_in_dict[tk][sub_tk](xflat[:, :-1])
+                    (hidden, cell) = self.get_hidden(
+                        1, self.transfer_layers, self.in_transfer_dim
+                    )
+
+                    global_pred, _ = self.global_transfer_lstm(in_pred, (hidden, cell))
                     y_pred[tk][sub_tk] = self.signal_layer[tk][sub_tk](
                         self.model_out_dict[tk][sub_tk](global_pred)
                     )
 
         return y_pred
 
     def avg_sharpe_ratio(self, output, target):
@@ -189,7 +206,13 @@
 
         rets = rets - tc
         avg_rets = torch.mean(rets)
         vol_rets = torch.std(rets)
         loss = torch.neg(torch.div(avg_rets, vol_rets))
 
         return loss.mean()
+
+    def get_hidden(self, batch_size, n_layers, nhi):
+        return (
+            torch.zeros(n_layers, batch_size, nhi).double().to(self.device),
+            torch.zeros(n_layers, batch_size, nhi).double().to(self.device),
+        )
```

### Comparing `quantnet-0.0.2/quantnet/global/linear_lstm.py` & `quantnet-0.0.3/quantnet/no_transfer/linear_lstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Dict, Union
-
 import numpy as np
 import torch
 from torch import nn
 
 
 class GlobalLinearLstm:
     def __init__(
         self, x_tasks, model_config):
         self.criterion = self.avg_sharpe_ratio
         self.X_train_tasks = x_tasks
-        self.tsteps = model_config["tsteps"]
-        self.tasks_tsteps = model_config["tasks_tsteps"]
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
         self.batch_size = model_config["batch_size"]
         self.seq_len = model_config["seq_len"]
         self.device = model_config["device"]
         self.export_path = model_config["export_path"]
         self.export_label = model_config["export_label"]
         self.opt_lr = model_config["global_linear_lstm"]["opt_lr"]
         self.amsgrad = model_config["global_linear_lstm"]["amsgrad"]
@@ -50,14 +48,15 @@
                 self.model_in_dict[tk],
                 self.model_out_dict[tk],
                 self.model_lin_dict[tk],
                 self.signal_layer[tk],
                 self.opt_dict[tk],
                 self.losses[tk],
             ) = ({}, {}, {}, {}, {}, {})
+
             self.sub_mtl_list[tk] = self.X_train_tasks[tk].keys()
 
             for sub_tk in self.sub_mtl_list[tk]:
                 self.losses[tk][sub_tk] = []
                 nin = self.X_train_tasks[tk][sub_tk].shape[1]
                 nout = self.X_train_tasks[tk][sub_tk].shape[1]
 
@@ -115,15 +114,15 @@
                     self.model_lin_dict[tk][sub_tk],
                     self.transfer_linear,
                     self.signal_layer[tk][sub_tk],
                     self.opt_dict[tk][sub_tk],
                 )
 
     def train(self):
-        for i in range(self.tsteps):
+        for i in range(self.t_steps):
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     start_ids = np.random.permutation(
                         list(
                             range(
                                 self.X_train_tasks[tk][sub_tk].size(0)
                                 - self.seq_len
```

### Comparing `quantnet-0.0.2/quantnet/global/lstm_linear.py` & `quantnet-0.0.3/quantnet/no_transfer/lstm_lstm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,194 +1,264 @@
 import numpy as np
 import torch
 from torch import nn
 
 
-class GlobalLstmLinear:
+class GlobalLstmLstm:
     def __init__(
         self, x_tasks, model_config):
         self.criterion = self.avg_sharpe_ratio
         self.X_train_tasks = x_tasks
-        self.tsteps = model_config["tsteps"]
-        self.tasks_tsteps = model_config["tasks_tsteps"]
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
         self.batch_size = model_config["batch_size"]
         self.seq_len = model_config["seq_len"]
         self.device = model_config["device"]
         self.export_path = model_config["export_path"]
         self.export_label = model_config["export_label"]
-        self.opt_lr = model_config["global_lstm_linear"]["opt_lr"]
-        self.amsgrad = model_config["global_lstm_linear"]["amsgrad"]
-        self.export_weights = model_config["global_lstm_linear"]["export_model"]
-        self.in_transfer_dim = model_config["global_lstm_linear"]["in_transfer_dim"]
-        self.out_transfer_dim = model_config["global_lstm_linear"]["out_transfer_dim"]
-        self.transfer_layers = model_config["global_lstm_linear"]["n_layers"]
-        self.dropout = model_config["global_lstm_linear"]["drop_rate"]
+        self.opt_lr = model_config["global_lstm_lstm"]["opt_lr"]
+        self.amsgrad = model_config["global_lstm_lstm"]["amsgrad"]
+        self.export_model = model_config["global_lstm_lstm"]["export_model"]
+        self.in_n_layers = model_config["global_lstm_lstm"]["in_n_layers"]
+        self.out_n_layers = model_config["global_lstm_lstm"]["out_n_layers"]
+        self.out_nhi = model_config["global_lstm_lstm"]["out_nhi"]
+        self.dropout = model_config["global_lstm_lstm"]["drop_rate"]
+        self.in_transfer_dim = model_config["global_lstm_lstm"]["in_transfer_dim"]
+        self.out_transfer_dim = model_config["global_lstm_lstm"]["out_transfer_dim"]
+        self.transfer_layers = model_config["global_lstm_lstm"]["n_layers"]
+        self.dropout_transfer = model_config["global_lstm_lstm"]["drop_rate_transfer"]
 
         self.mtl_list = self.X_train_tasks.keys()
 
-        self.sub_mtl_list = {}
         (
+            self.sub_mtl_list,
+            self.transfer_lstm_dict,
             self.model_in_dict,
             self.model_out_dict,
+            self.model_lin_dict,
             self.opt_dict,
             self.signal_layer,
             self.losses,
-        ) = ({}, {}, {}, {}, {})
+        ) = ({}, {}, {}, {}, {}, {}, {}, {})
 
         self.global_transfer_lstm = (
             nn.LSTM(
                 self.in_transfer_dim,
                 self.out_transfer_dim,
                 self.transfer_layers,
                 batch_first=True,
-                dropout=self.dropout,
+                dropout=self.dropout_transfer,
             )
             .double()
             .to(self.device)
         )
 
         for tk in self.mtl_list:
             (
                 self.model_in_dict[tk],
                 self.model_out_dict[tk],
+                self.model_lin_dict[tk],
                 self.signal_layer[tk],
                 self.opt_dict[tk],
                 self.losses[tk],
-            ) = ({}, {}, {}, {}, {})
+            ) = ({}, {}, {}, {}, {}, {})
+
             self.sub_mtl_list[tk] = self.X_train_tasks[tk].keys()
 
             for sub_tk in self.sub_mtl_list[tk]:
                 self.losses[tk][sub_tk] = []
                 nin = self.X_train_tasks[tk][sub_tk].shape[1]
                 nout = self.X_train_tasks[tk][sub_tk].shape[1]
 
+                in_n_layers, out_n_layers, out_nhi = (
+                    self.in_n_layers,
+                    self.out_n_layers,
+                    self.out_nhi,
+                )
+
                 self.model_in_dict[tk][sub_tk] = (
-                    nn.Linear(nin, self.in_transfer_dim).double().to(self.device)
+                    nn.LSTM(
+                        nin,
+                        self.in_transfer_dim,
+                        in_n_layers,
+                        batch_first=True,
+                        dropout=self.dropout,
+                    )
+                    .double()
+                    .to(self.device)
                 )
+
                 self.model_out_dict[tk][sub_tk] = (
-                    nn.Linear(self.out_transfer_dim, nout).double().to(self.device)
+                    nn.LSTM(
+                        self.out_transfer_dim,
+                        out_nhi,
+                        out_n_layers,
+                        batch_first=True,
+                        dropout=self.dropout,
+                    )
+                    .double()
+                    .to(self.device)
+                )
+                self.model_lin_dict[tk][sub_tk] = (
+                    nn.Linear(out_nhi, nout).double().to(self.device)
                 )
                 self.signal_layer[tk][sub_tk] = nn.Tanh().to(self.device)
 
                 self.opt_dict[tk][sub_tk] = torch.optim.Adam(
                     list(self.model_in_dict[tk][sub_tk].parameters())
                     + list(self.model_out_dict[tk][sub_tk].parameters())
+                    + list(self.model_lin_dict[tk][sub_tk].parameters())
                     + list(self.global_transfer_lstm.parameters())
                     + list(self.signal_layer[tk][sub_tk].parameters()),
                     lr=self.opt_lr,
                     amsgrad=self.amsgrad,
                 )
 
                 print(
                     tk,
                     sub_tk,
                     self.model_in_dict[tk][sub_tk],
                     self.model_out_dict[tk][sub_tk],
+                    self.model_lin_dict[tk][sub_tk],
                     self.global_transfer_lstm,
                     self.signal_layer[tk][sub_tk],
                     self.opt_dict[tk][sub_tk],
                 )
 
-    def train(self):
-        for i in range(self.tsteps):
+    def train(self) -> None:
+        for i in range(self.t_steps):
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     start_ids = np.random.permutation(
                         list(
                             range(
                                 self.X_train_tasks[tk][sub_tk].size(0)
                                 - self.seq_len
                                 - 1
                             )
                         )
                     )[: self.batch_size]
+
                     X_Y_batch = torch.stack(
                         [
                             self.X_train_tasks[tk][sub_tk][i : i + self.seq_len + 1]
                             for i in start_ids
                         ],
                         dim=0,
                     )
                     Y_train = X_Y_batch[:, 1:, :]
                     X_train = X_Y_batch[:, :-1, :]
 
                     self.opt_dict[tk][sub_tk].zero_grad()
 
-                    in_pred = self.model_in_dict[tk][sub_tk](X_train)
+                    (hidden, cell) = self.get_hidden(
+                        self.batch_size, self.in_n_layers, self.in_transfer_dim
+                    )
+                    in_pred, _ = self.model_in_dict[tk][sub_tk](X_train, (hidden, cell))
 
                     (hidden, cell) = self.get_hidden(
-                        self.batch_size, self.transfer_layers, self.in_transfer_dim
+                        self.batch_size, self.transfer_layers, self.out_transfer_dim
                     )
                     global_pred, _ = self.global_transfer_lstm(in_pred, (hidden, cell))
 
+                    (hidden, cell) = self.get_hidden(
+                        self.batch_size, self.out_n_layers, self.out_nhi
+                    )
+                    hidden_pred, _ = self.model_out_dict[tk][sub_tk](
+                        global_pred, (hidden, cell)
+                    )
+
                     preds = self.signal_layer[tk][sub_tk](
-                        self.model_out_dict[tk][sub_tk](global_pred)
+                        self.model_lin_dict[tk][sub_tk](hidden_pred)
                     )
 
                     loss = self.criterion(preds, Y_train)
                     self.losses[tk][sub_tk].append(loss.item())
 
                     loss.backward()
                     self.opt_dict[tk][sub_tk].step()
 
             if (i % 100) == 1:
                 print(i)
 
-        if self.export_weights:
+        if self.export_model:
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     torch.save(
                         self.model_in_dict[tk][sub_tk],
                         self.export_path
                         + tk
                         + "_"
                         + sub_tk
                         + "_"
                         + self.export_label
-                        + "_intransferlinear.pt",
+                        + "_intransferlstm.pt",
                     )
 
                     torch.save(
                         self.model_out_dict[tk][sub_tk],
                         self.export_path
                         + tk
                         + "_"
                         + sub_tk
                         + "_"
                         + self.export_label
-                        + "_outtransferlinear.pt",
+                        + "_outtransferlstm.pt",
+                    )
+
+                    torch.save(
+                        self.model_lin_dict[tk][sub_tk],
+                        self.export_path
+                        + tk
+                        + "_"
+                        + sub_tk
+                        + "_"
+                        + self.export_label
+                        + "_outtransferlstm.pt",
                     )
 
                 torch.save(
                     self.global_transfer_lstm,
                     self.export_path
                     + tk
                     + "_"
                     + self.export_label
-                    + "_globaltransferlstm.pt",
+                    + "_transferlstm.pt",
                 )
 
     def predict(self, x_test):
         y_pred = {}
 
         for tk in self.mtl_list:
             y_pred[tk] = {}
 
             for sub_tk in self.sub_mtl_list[tk]:
-                xflat = x_test[tk][sub_tk].view(1, -1, x_test[tk][sub_tk].size(1))
+                x_flat = x_test[tk][sub_tk].view(1, -1, x_test[tk][sub_tk].size(1))
 
                 with torch.autograd.no_grad():
-                    in_pred = self.model_in_dict[tk][sub_tk](xflat[:, :-1])
                     (hidden, cell) = self.get_hidden(
-                        1, self.transfer_layers, self.in_transfer_dim
+                        1, self.in_n_layers, self.in_transfer_dim
                     )
 
+                    in_pred, _ = self.model_in_dict[tk][sub_tk](
+                        x_flat[:, :-1], (hidden, cell)
+                    )
+
+                    (hidden, cell) = self.get_hidden(
+                        1, self.transfer_layers, self.out_transfer_dim
+                    )
                     global_pred, _ = self.global_transfer_lstm(in_pred, (hidden, cell))
+
+                    (hidden, cell) = self.get_hidden(1, self.out_n_layers, self.out_nhi)
+                    hidden_pred, _ = self.model_out_dict[tk][sub_tk](
+                        global_pred, (hidden, cell)
+                    )
+
                     y_pred[tk][sub_tk] = self.signal_layer[tk][sub_tk](
-                        self.model_out_dict[tk][sub_tk](global_pred)
+                        self.model_lin_dict[tk][sub_tk](hidden_pred)
                     )
 
         return y_pred
 
     def avg_sharpe_ratio(self, output, target):
         slip = 0.0005 * 0.00
         bp = 0.0020 * 0.00
```

### Comparing `quantnet-0.0.2/quantnet/no_transfer/linear.py` & `quantnet-0.0.3/quantnet/no_transfer/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from torch import nn
 
 
 class NoTransferLinear:
     def __init__(self, x_tasks, model_config):
         self.criterion = self.avg_sharpe_ratio
         self.X_train_tasks = x_tasks
-        self.tsteps = model_config["tsteps"]
-        self.tasks_tsteps = model_config["tasks_tsteps"]
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
         self.batch_size = model_config["batch_size"]
         self.seq_len = model_config["seq_len"]
         self.device = model_config["device"]
         self.export_path = model_config["export_path"]
         self.export_label = model_config["export_label"]
         self.opt_lr = model_config["no_transfer_linear"]["opt_lr"]
         self.amsgrad = model_config["no_transfer_linear"]["amsgrad"]
@@ -60,15 +60,15 @@
                     sub_tk,
                     self.model_lin_dict[tk][sub_tk],
                     self.signal_layer[tk][sub_tk],
                     self.opt_dict[tk][sub_tk],
                 )
 
     def train(self):
-        for i in range(self.tsteps):
+        for i in range(self.t_steps):
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     start_ids = np.random.permutation(
                         list(
                             range(
                                 self.X_train_tasks[tk][sub_tk].size(0)
                                 - self.seq_len
```

### Comparing `quantnet-0.0.2/quantnet/no_transfer/lstm.py` & `quantnet-0.0.3/quantnet/no_transfer/lstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 import torch
 from torch import nn
 
 
 class NoTransferLstm:
-    def __init__(
-        self, x_tasks, model_config):
+    def __init__(self, x_tasks, model_config):
         self.criterion = self.avg_sharpe_ratio
         self.X_train_tasks = x_tasks
-        self.tsteps = model_config["tsteps"]
-        self.tasks_tsteps = model_config["tasks_tsteps"]
+        self.t_steps = model_config["t_steps"]
+        self.tasks_t_steps = model_config["tasks_t_steps"]
         self.batch_size = model_config["batch_size"]
         self.seq_len = model_config["seq_len"]
         self.device = model_config["device"]
         self.export_path = model_config["export_path"]
         self.export_label = model_config["export_label"]
         self.opt_lr = model_config["no_transfer_lstm"]["opt_lr"]
         self.amsgrad = model_config["no_transfer_lstm"]["amsgrad"]
@@ -66,15 +65,15 @@
                     + list(self.model_lin_dict[tk][sub_tk].parameters())
                     + list(self.signal_layer[tk][sub_tk].parameters()),
                     lr=self.opt_lr,
                     amsgrad=self.amsgrad,
                 )
 
     def train(self):
-        for i in range(self.tsteps):
+        for i in range(self.t_steps):
             for tk in self.mtl_list:
                 for sub_tk in self.sub_mtl_list[tk]:
                     start_ids = np.random.permutation(
                         list(
                             range(
                                 self.X_train_tasks[tk][sub_tk].size(0)
                                 - self.seq_len
```

### Comparing `quantnet-0.0.2/quantnet/utils.py` & `quantnet-0.0.3/quantnet/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,34 +42,35 @@
         "TailR",
         "Skew",
         "Kurt",
     ]
 
     df_metrics = pd.DataFrame(index=range(df.shape[1]), columns=pf_metrics_labels)
 
-    for (pf, pf_label) in zip(pf_metrics, pf_metrics_labels):
+    for pf, pf_label in zip(pf_metrics, pf_metrics_labels):
         df_metrics[pf_label] = np.array(pf(df))
 
     df_metrics.index = df.columns
 
     return df_metrics
 
 
 def get_data(data_config, problem_config, model_config):
     X_train_tasks, X_val_tasks, X_test_tasks = {}, {}, {}
 
     for region in data_config["region"]:
         region_task_paths = [t + "_all_assets_data.pkl.gz" for t in data_config[region]]
         X_train_tasks[region], X_val_tasks[region], X_test_tasks[region] = {}, {}, {}
 
-        for (tk_path, tk) in zip(region_task_paths, data_config[region]):
+        for tk_path, tk in zip(region_task_paths, data_config[region]):
             df = pd.read_pickle(data_config["data_path"] + tk_path)
             df_train = df.iloc[
                 : -(problem_config["val_period"] + problem_config["holdout_period"])
             ]
+
             if problem_config["val_period"] != 0:
                 df_val = df.iloc[
                     -(
                         problem_config["val_period"] + problem_config["holdout_period"]
                     ) : -problem_config["holdout_period"]
                 ]
             else:
@@ -78,17 +79,19 @@
                 ]
 
             df_test = df.iloc[-problem_config["holdout_period"] :]
 
             X_train_tasks[region][tk] = torch.from_numpy(df_train.values).to(
                 model_config["device"]
             )
+
             X_val_tasks[region][tk] = torch.from_numpy(df_val.values).to(
                 model_config["device"]
             )
+
             X_test_tasks[region][tk] = torch.from_numpy(df_test.values).to(
                 model_config["device"]
             )
 
     return X_train_tasks, X_val_tasks, X_test_tasks
```

### Comparing `quantnet-0.0.2/setup.py` & `quantnet-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="quantnet",
-    version="0.0.2",
+    version="0.0.3",
     author="Alexandre Brilhante",
     author_email="alexandre.brilhante@gmail.com",
     description="A PyTorch implementation of QuantNet: Transferring Learning Across Systematic Trading Strategies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/brilhana/quantnet",
     project_urls={
```

