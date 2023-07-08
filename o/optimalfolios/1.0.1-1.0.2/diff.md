# Comparing `tmp/optimalfolios-1.0.1.tar.gz` & `tmp/optimalfolios-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimalfolios-1.0.1.tar", max compression
+gzip compressed data, was "optimalfolios-1.0.2.tar", max compression
```

## Comparing `optimalfolios-1.0.1.tar` & `optimalfolios-1.0.2.tar`

### file list

```diff
@@ -1,79 +1,35 @@
--rw-r--r--   0        0        0       15 2023-07-08 17:40:30.503064 optimalfolios-1.0.1/optimalfolios/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0      313 2023-07-08 17:40:32.516044 optimalfolios-1.0.1/optimalfolios/.git/config
--rw-r--r--   0        0        0       73 2023-07-08 17:31:05.728124 optimalfolios-1.0.1/optimalfolios/.git/description
--rw-r--r--   0        0        0       23 2023-07-08 17:31:05.742087 optimalfolios-1.0.1/optimalfolios/.git/HEAD
--rw-r--r--   0        0        0      478 2023-07-08 17:31:05.729122 optimalfolios-1.0.1/optimalfolios/.git/hooks/applypatch-msg.sample
--rw-r--r--   0        0        0      896 2023-07-08 17:31:05.730119 optimalfolios-1.0.1/optimalfolios/.git/hooks/commit-msg.sample
--rw-r--r--   0        0        0     4655 2023-07-08 17:31:05.731117 optimalfolios-1.0.1/optimalfolios/.git/hooks/fsmonitor-watchman.sample
--rw-r--r--   0        0        0      189 2023-07-08 17:31:05.732114 optimalfolios-1.0.1/optimalfolios/.git/hooks/post-update.sample
--rw-r--r--   0        0        0      424 2023-07-08 17:31:05.733111 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-applypatch.sample
--rw-r--r--   0        0        0     1643 2023-07-08 17:31:05.734108 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-commit.sample
--rw-r--r--   0        0        0      416 2023-07-08 17:31:05.734108 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-merge-commit.sample
--rw-r--r--   0        0        0     1374 2023-07-08 17:31:05.735106 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-push.sample
--rw-r--r--   0        0        0     4898 2023-07-08 17:31:05.736104 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-rebase.sample
--rw-r--r--   0        0        0      544 2023-07-08 17:31:05.737101 optimalfolios-1.0.1/optimalfolios/.git/hooks/pre-receive.sample
--rw-r--r--   0        0        0     1492 2023-07-08 17:31:05.738098 optimalfolios-1.0.1/optimalfolios/.git/hooks/prepare-commit-msg.sample
--rw-r--r--   0        0        0     2783 2023-07-08 17:31:05.739096 optimalfolios-1.0.1/optimalfolios/.git/hooks/push-to-checkout.sample
--rw-r--r--   0        0        0     3650 2023-07-08 17:31:05.739096 optimalfolios-1.0.1/optimalfolios/.git/hooks/update.sample
--rw-r--r--   0        0        0     2038 2023-07-08 20:44:11.649996 optimalfolios-1.0.1/optimalfolios/.git/index
--rw-r--r--   0        0        0      240 2023-07-08 17:31:05.740093 optimalfolios-1.0.1/optimalfolios/.git/info/exclude
--rw-r--r--   0        0        0      188 2023-07-08 17:40:30.511042 optimalfolios-1.0.1/optimalfolios/.git/logs/HEAD
--rw-r--r--   0        0        0      188 2023-07-08 17:40:30.511042 optimalfolios-1.0.1/optimalfolios/.git/logs/refs/heads/master
--rw-r--r--   0        0        0      170 2023-07-08 17:40:32.520035 optimalfolios-1.0.1/optimalfolios/.git/logs/refs/remotes/origin/master
--rw-r--r--   0        0        0       97 2023-07-08 17:40:30.495086 optimalfolios-1.0.1/optimalfolios/.git/objects/05/afbfa9490f57dd4f1fafbcfc77d9d15a36ac21
--rw-r--r--   0        0        0     4098 2023-07-08 17:40:30.383619 optimalfolios-1.0.1/optimalfolios/.git/objects/0e/bf82a62ab97c22f8da769a39add40bc14ed564
--rw-r--r--   0        0        0     4434 2023-07-08 17:40:30.402568 optimalfolios-1.0.1/optimalfolios/.git/objects/10/1f9173206d7a9725fb73e37c605702056b6676
--rw-r--r--   0        0        0      131 2023-07-08 17:40:30.491097 optimalfolios-1.0.1/optimalfolios/.git/objects/37/d53fe7c2b1e9e1988633b321e6be610455cf00
--rw-r--r--   0        0        0     2231 2023-07-08 17:40:30.389602 optimalfolios-1.0.1/optimalfolios/.git/objects/3b/5782205ea2986619502999d943b8818f4b42db
--rw-r--r--   0        0        0     9971 2023-07-08 17:40:30.386611 optimalfolios-1.0.1/optimalfolios/.git/objects/50/be8932b1a633a1a3077ee752ec03ea0a8bedba
--rw-r--r--   0        0        0      162 2023-07-08 17:40:30.488104 optimalfolios-1.0.1/optimalfolios/.git/objects/57/4801560c5067309f2456c8048078e48a0fc943
--rw-r--r--   0        0        0      182 2023-07-08 17:40:30.482120 optimalfolios-1.0.1/optimalfolios/.git/objects/5c/84bdea7aa66f2581e5259656bd8966a148d3af
--rw-r--r--   0        0        0     2786 2023-07-08 17:40:30.415533 optimalfolios-1.0.1/optimalfolios/.git/objects/64/5f0c2209d5ca34e1a2c3d01d2b2cff32936c13
--rw-r--r--   0        0        0      146 2023-07-08 17:40:30.504062 optimalfolios-1.0.1/optimalfolios/.git/objects/69/50e6d9310f70280891ddc4094be78c6f178e24
--rw-r--r--   0        0        0   350942 2023-07-08 20:24:28.321692 optimalfolios-1.0.1/optimalfolios/.git/objects/7a/dcaebad12ecfcff60a4604aa039b5f4bff92f8
--rw-r--r--   0        0        0       27 2023-07-08 17:40:30.368659 optimalfolios-1.0.1/optimalfolios/.git/objects/80/045cd3cfef43b2c2808eb3b838ce5aefb1a4db
--rw-r--r--   0        0        0     2417 2023-07-08 17:40:30.399577 optimalfolios-1.0.1/optimalfolios/.git/objects/8c/255a0913586bbde2646272ffa76ce233b605a2
--rw-r--r--   0        0        0      195 2023-07-08 17:40:30.485112 optimalfolios-1.0.1/optimalfolios/.git/objects/90/f35e7cb267571b66665c20509480629d6c532b
--rw-r--r--   0        0        0     4765 2023-07-08 17:40:30.406556 optimalfolios-1.0.1/optimalfolios/.git/objects/b0/55594e3786fd7bb741732cc66f2749f441e05e
--rw-r--r--   0        0        0     1150 2023-07-08 17:40:30.409549 optimalfolios-1.0.1/optimalfolios/.git/objects/c3/f23ecf221a4815c1b1b733deb7b97697c63535
--rw-r--r--   0        0        0      221 2023-07-08 17:40:30.499074 optimalfolios-1.0.1/optimalfolios/.git/objects/d5/41a3d24c65822ba5320903e5a2512cccbb7b05
--rw-r--r--   0        0        0       15 2023-07-08 20:22:39.020866 optimalfolios-1.0.1/optimalfolios/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0      949 2023-07-08 17:40:30.392594 optimalfolios-1.0.1/optimalfolios/.git/objects/ed/731046c58b46d4c36fc65413e1b1ac6f1bdc2d
--rw-r--r--   0        0        0     2327 2023-07-08 17:40:30.412542 optimalfolios-1.0.1/optimalfolios/.git/objects/ef/0238664f1840f9a947ff530bdc8c1fb6c401c3
--rw-r--r--   0        0        0      827 2023-07-08 17:40:30.395586 optimalfolios-1.0.1/optimalfolios/.git/objects/ef/9b889ec782e6d45d306812b9727fff54873509
--rw-r--r--   0        0        0       41 2023-07-08 17:40:30.510045 optimalfolios-1.0.1/optimalfolios/.git/refs/heads/master
--rw-r--r--   0        0        0       41 2023-07-08 17:40:32.518040 optimalfolios-1.0.1/optimalfolios/.git/refs/remotes/origin/master
--rw-r--r--   0        0        0        0 2023-04-10 12:39:00.221075 optimalfolios-1.0.1/optimalfolios/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 12:39:15.297526 optimalfolios-1.0.1/optimalfolios/examples/__init__.py
--rw-r--r--   0        0        0      154 2023-04-10 15:10:01.448884 optimalfolios-1.0.1/optimalfolios/examples/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-04-10 13:22:32.718157 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/__init__.py
--rw-r--r--   0        0        0      172 2023-04-10 15:10:01.450879 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5554 2023-07-08 20:25:20.737092 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/__pycache__/load_prices.cpython-310.pyc
--rw-r--r--   0        0        0    17681 2023-07-08 17:13:49.880137 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/article_figures.py
--rw-r--r--   0        0        0    49694 2023-07-08 20:35:30.949471 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/backtest_crypto_portfolios.py
--rw-r--r--   0        0        0   844149 2023-06-08 15:07:44.076495 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/crypto_allocation_prices.csv
--rw-r--r--   0        0        0     7022 2023-07-08 20:25:17.589786 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/load_prices.py
--rw-r--r--   0        0        0        0 2023-07-08 20:22:36.696312 optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/README.md
--rw-r--r--   0        0        0     2137 2023-07-08 20:27:18.304815 optimalfolios-1.0.1/optimalfolios/examples/gaussian_mixure_scatter.py
--rw-r--r--   0        0        0     2263 2023-07-08 17:13:49.905071 optimalfolios-1.0.1/optimalfolios/examples/portfolio_opt_backtest.py
--rw-r--r--   0        0        0        0 2021-10-10 14:27:53.224013 optimalfolios-1.0.1/optimalfolios/optimization/__init__.py
--rw-r--r--   0        0        0      158 2023-04-10 12:53:58.012971 optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10012 2023-06-07 10:04:35.000000 optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/opt_solvers.cpython-310.pyc
--rw-r--r--   0        0        0     9550 2023-05-11 14:59:01.000000 optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/qp_solvers.cpython-310.pyc
--rw-r--r--   0        0        0    11370 2023-07-08 20:27:21.666935 optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/rolling_portfolios.cpython-310.pyc
--rw-r--r--   0        0        0    12191 2023-06-07 10:04:33.000000 optimalfolios-1.0.1/optimalfolios/optimization/opt_solvers.py
--rw-r--r--   0        0        0    20063 2023-05-11 14:57:46.000000 optimalfolios-1.0.1/optimalfolios/optimization/qp_solvers.py
--rw-r--r--   0        0        0    22575 2023-07-08 17:13:49.929517 optimalfolios-1.0.1/optimalfolios/optimization/rolling_portfolios.py
--rw-r--r--   0        0        0        0 2023-05-04 17:56:18.312760 optimalfolios-1.0.1/optimalfolios/reports/__init__.py
--rw-r--r--   0        0        0      153 2023-05-04 18:57:12.945211 optimalfolios-1.0.1/optimalfolios/reports/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2197 2023-05-30 13:33:48.000000 optimalfolios-1.0.1/optimalfolios/reports/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     4843 2023-07-08 20:30:19.441174 optimalfolios-1.0.1/optimalfolios/reports/__pycache__/marginal_backtest.cpython-310.pyc
--rw-r--r--   0        0        0     3878 2023-05-30 12:41:29.000000 optimalfolios-1.0.1/optimalfolios/reports/config.py
--rw-r--r--   0        0        0    13316 2023-07-08 17:13:49.810794 optimalfolios-1.0.1/optimalfolios/reports/marginal_backtest.py
--rw-r--r--   0        0        0        0 2023-04-10 12:46:24.405225 optimalfolios-1.0.1/optimalfolios/utils/__init__.py
--rw-r--r--   0        0        0      151 2023-04-10 12:53:58.204484 optimalfolios-1.0.1/optimalfolios/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8076 2023-06-19 14:18:39.000000 optimalfolios-1.0.1/optimalfolios/utils/__pycache__/gaussian_mixture.cpython-310.pyc
--rw-r--r--   0        0        0     8575 2023-06-19 14:18:38.000000 optimalfolios-1.0.1/optimalfolios/utils/gaussian_mixture.py
--rw-r--r--   0        0        0     1740 2023-07-08 20:53:14.891131 optimalfolios-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       15 2023-07-08 20:43:29.444730 optimalfolios-1.0.1/README.md
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 optimalfolios-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35802 2023-07-08 20:58:25.467501 optimalfolios-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-10 12:39:00.221075 optimalfolios-1.0.2/optimalfolios/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:39:15.297526 optimalfolios-1.0.2/optimalfolios/examples/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-10 15:10:01.448884 optimalfolios-1.0.2/optimalfolios/examples/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-10 13:22:32.718157 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-10 15:10:01.450879 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5554 2023-07-08 20:25:20.737092 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/__pycache__/load_prices.cpython-310.pyc
+-rw-r--r--   0        0        0    17681 2023-07-08 17:13:49.880137 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/article_figures.py
+-rw-r--r--   0        0        0    49694 2023-07-08 20:35:30.949471 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/backtest_crypto_portfolios.py
+-rw-r--r--   0        0        0   844149 2023-06-08 15:07:44.076495 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/crypto_allocation_prices.csv
+-rw-r--r--   0        0        0     7022 2023-07-08 20:25:17.589786 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/load_prices.py
+-rw-r--r--   0        0        0        0 2023-07-08 20:22:36.696312 optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/README.md
+-rw-r--r--   0        0        0     2137 2023-07-08 20:27:18.304815 optimalfolios-1.0.2/optimalfolios/examples/gaussian_mixure_scatter.py
+-rw-r--r--   0        0        0     2263 2023-07-08 17:13:49.905071 optimalfolios-1.0.2/optimalfolios/examples/portfolio_opt_backtest.py
+-rw-r--r--   0        0        0        0 2021-10-10 14:27:53.224013 optimalfolios-1.0.2/optimalfolios/optimization/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-10 12:53:58.012971 optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10012 2023-06-07 10:04:35.000000 optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/opt_solvers.cpython-310.pyc
+-rw-r--r--   0        0        0     9550 2023-05-11 14:59:01.000000 optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/qp_solvers.cpython-310.pyc
+-rw-r--r--   0        0        0    11370 2023-07-08 20:27:21.666935 optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/rolling_portfolios.cpython-310.pyc
+-rw-r--r--   0        0        0    12191 2023-06-07 10:04:33.000000 optimalfolios-1.0.2/optimalfolios/optimization/opt_solvers.py
+-rw-r--r--   0        0        0    20063 2023-05-11 14:57:46.000000 optimalfolios-1.0.2/optimalfolios/optimization/qp_solvers.py
+-rw-r--r--   0        0        0    22575 2023-07-08 17:13:49.929517 optimalfolios-1.0.2/optimalfolios/optimization/rolling_portfolios.py
+-rw-r--r--   0        0        0        0 2023-05-04 17:56:18.312760 optimalfolios-1.0.2/optimalfolios/reports/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-04 18:57:12.945211 optimalfolios-1.0.2/optimalfolios/reports/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2197 2023-05-30 13:33:48.000000 optimalfolios-1.0.2/optimalfolios/reports/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     4843 2023-07-08 20:30:19.441174 optimalfolios-1.0.2/optimalfolios/reports/__pycache__/marginal_backtest.cpython-310.pyc
+-rw-r--r--   0        0        0     3878 2023-05-30 12:41:29.000000 optimalfolios-1.0.2/optimalfolios/reports/config.py
+-rw-r--r--   0        0        0    13316 2023-07-08 17:13:49.810794 optimalfolios-1.0.2/optimalfolios/reports/marginal_backtest.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:46:24.405225 optimalfolios-1.0.2/optimalfolios/utils/__init__.py
+-rw-r--r--   0        0        0      151 2023-04-10 12:53:58.204484 optimalfolios-1.0.2/optimalfolios/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8076 2023-06-19 14:18:39.000000 optimalfolios-1.0.2/optimalfolios/utils/__pycache__/gaussian_mixture.cpython-310.pyc
+-rw-r--r--   0        0        0     8575 2023-06-19 14:18:38.000000 optimalfolios-1.0.2/optimalfolios/utils/gaussian_mixture.py
+-rw-r--r--   0        0        0     1740 2023-07-08 21:02:10.557129 optimalfolios-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-07-08 20:43:29.444730 optimalfolios-1.0.2/README.md
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 optimalfolios-1.0.2/PKG-INFO
```

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/__pycache__/load_prices.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/__pycache__/load_prices.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/article_figures.py` & `optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/article_figures.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/backtest_crypto_portfolios.py` & `optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/backtest_crypto_portfolios.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/crypto_allocation_prices.csv` & `optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/crypto_allocation_prices.csv`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/crypto_allocation/load_prices.py` & `optimalfolios-1.0.2/optimalfolios/examples/crypto_allocation/load_prices.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/gaussian_mixure_scatter.py` & `optimalfolios-1.0.2/optimalfolios/examples/gaussian_mixure_scatter.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/examples/portfolio_opt_backtest.py` & `optimalfolios-1.0.2/optimalfolios/examples/portfolio_opt_backtest.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/opt_solvers.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/opt_solvers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/qp_solvers.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/qp_solvers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/__pycache__/rolling_portfolios.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/optimization/__pycache__/rolling_portfolios.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/opt_solvers.py` & `optimalfolios-1.0.2/optimalfolios/optimization/opt_solvers.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/qp_solvers.py` & `optimalfolios-1.0.2/optimalfolios/optimization/qp_solvers.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/optimization/rolling_portfolios.py` & `optimalfolios-1.0.2/optimalfolios/optimization/rolling_portfolios.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/reports/__pycache__/config.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/reports/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/reports/__pycache__/marginal_backtest.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/reports/__pycache__/marginal_backtest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/reports/config.py` & `optimalfolios-1.0.2/optimalfolios/reports/config.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/reports/marginal_backtest.py` & `optimalfolios-1.0.2/optimalfolios/reports/marginal_backtest.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/utils/__pycache__/gaussian_mixture.cpython-310.pyc` & `optimalfolios-1.0.2/optimalfolios/utils/__pycache__/gaussian_mixture.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/optimalfolios/utils/gaussian_mixture.py` & `optimalfolios-1.0.2/optimalfolios/utils/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `optimalfolios-1.0.1/pyproject.toml` & `optimalfolios-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 226f 7074 696d 616c 666f  ame = "optimalfo
 00000020: 6c69 6f73 220d 0a76 6572 7369 6f6e 203d  lios"..version =
-00000030: 2022 312e 302e 3122 0d0a 6465 7363 7269   "1.0.1"..descri
+00000030: 2022 312e 302e 3222 0d0a 6465 7363 7269   "1.0.2"..descri
 00000040: 7074 696f 6e20 3d20 2253 696d 756c 6174  ption = "Simulat
 00000050: 696f 6e20 616e 6420 6261 636b 7465 7374  ion and backtest
 00000060: 696e 6720 6f66 206f 7074 696d 616c 2070  ing of optimal p
 00000070: 6f72 7466 6f6c 696f 7322 0d0a 6c69 6365  ortfolios"..lice
 00000080: 6e73 6520 3d20 224c 4943 454e 5345 2e74  nse = "LICENSE.t
 00000090: 7874 220d 0a61 7574 686f 7273 203d 205b  xt"..authors = [
 000000a0: 2241 7274 7572 2053 6570 7020 3c61 7274  "Artur Sepp <art
```

### Comparing `optimalfolios-1.0.1/PKG-INFO` & `optimalfolios-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimalfolios
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simulation and backtesting of optimal portfolios
 Home-page: https://github.com/ArturSepp/OptimalPortfolios
 License: LICENSE.txt
 Keywords: quantitative,investing,portfolio optimization,systematic strategies,volatility
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

