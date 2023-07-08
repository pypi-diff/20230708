# Comparing `tmp/fscraper-1.0.0.tar.gz` & `tmp/fscraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fscraper-1.0.0.tar", last modified: Fri May 26 02:18:07 2023, max compression
+gzip compressed data, was "fscraper-1.0.1.tar", last modified: Sat Jul  8 02:51:39 2023, max compression
```

## Comparing `fscraper-1.0.0.tar` & `fscraper-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 02:18:07.751357 fscraper-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-04-22 01:43:56.000000 fscraper-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      337 2023-05-26 02:18:07.751357 fscraper-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2023-05-26 01:50:11.000000 fscraper-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 02:18:07.719802 fscraper-1.0.0/fscraper/
--rw-rw-rw-   0        0        0      426 2023-05-15 02:47:44.000000 fscraper-1.0.0/fscraper/__init__.py
--rw-rw-rw-   0        0        0      206 2023-04-22 01:43:56.000000 fscraper-1.0.0/fscraper/kabutanscraper.py
--rw-rw-rw-   0        0        0     9918 2023-05-15 05:27:51.000000 fscraper-1.0.0/fscraper/kabuyohoscraper.py
--rw-rw-rw-   0        0        0     3211 2023-05-16 13:37:49.000000 fscraper-1.0.0/fscraper/reuterscraper.py
--rw-rw-rw-   0        0        0     5313 2023-05-16 13:27:14.000000 fscraper-1.0.0/fscraper/utils.py
--rw-rw-rw-   0        0        0     4363 2023-05-15 02:57:15.000000 fscraper-1.0.0/fscraper/xpath_table.py
--rw-rw-rw-   0        0        0     4976 2023-05-26 01:28:15.000000 fscraper-1.0.0/fscraper/yfscraper.py
-drwxrwxrwx   0        0        0        0 2023-05-26 02:18:07.736866 fscraper-1.0.0/fscraper.egg-info/
--rw-rw-rw-   0        0        0      337 2023-05-26 02:18:07.000000 fscraper-1.0.0/fscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-26 02:18:07.000000 fscraper-1.0.0/fscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 02:18:07.000000 fscraper-1.0.0/fscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-26 02:18:07.000000 fscraper-1.0.0/fscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 02:18:07.000000 fscraper-1.0.0/fscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 02:18:07.751357 fscraper-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      560 2023-05-16 13:30:05.000000 fscraper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.183396 fscraper-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-04-22 01:43:56.000000 fscraper-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2968 2023-07-08 02:51:39.178472 fscraper-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2586 2023-05-29 13:08:02.000000 fscraper-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.053405 fscraper-1.0.1/fscraper/
+-rw-rw-rw-   0        0        0      426 2023-05-15 02:47:44.000000 fscraper-1.0.1/fscraper/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-06-25 10:08:25.000000 fscraper-1.0.1/fscraper/kabutanscraper.py
+-rw-rw-rw-   0        0        0     9918 2023-05-15 05:27:51.000000 fscraper-1.0.1/fscraper/kabuyohoscraper.py
+-rw-rw-rw-   0        0        0     3211 2023-05-16 13:37:49.000000 fscraper-1.0.1/fscraper/reuterscraper.py
+-rw-rw-rw-   0        0        0     5585 2023-07-01 14:35:21.000000 fscraper-1.0.1/fscraper/utils.py
+-rw-rw-rw-   0        0        0     4363 2023-05-15 02:57:15.000000 fscraper-1.0.1/fscraper/xpath_table.py
+-rw-rw-rw-   0        0        0     4976 2023-05-26 01:28:15.000000 fscraper-1.0.1/fscraper/yfscraper.py
+drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.163890 fscraper-1.0.1/fscraper.egg-info/
+-rw-rw-rw-   0        0        0     2968 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 02:51:39.184440 fscraper-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-07-02 01:55:58.000000 fscraper-1.0.1/setup.py
```

### Comparing `fscraper-1.0.0/LICENSE` & `fscraper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.0/README.md` & `fscraper-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # fscraper
-Financial Data Web Scraper
+Financial Data Scraper
 
 ## Introduction
 The project contains a collection of functions used to scrape financial data from the internet, mainly in Japan, and to calculate financial indicators such as *RSI*, *beta*, *MACD*, etc. Web scraping is implemented using `BeautifulSoup` and `requests` for the site that provides a RESTful API endpoint.
 
 ## Getting Started 
+### Installation
+    pip install fscraper
+
 ### Financial Data
 ```python
 import fscraper as fs
 
 # Yahoo Finance
 yfs = fs.YahooFinanceScraper('7203.T')
 df = yfs.get_stock_price(peroid='10y', interval='1d')
@@ -57,11 +60,11 @@
 beta = fs.calculate_beta(code='6753.T', market='^N225', period='1y')
 
 # 100 days min&max price
 df['100-high'], df['100-low'] = fs.set_x_days_high_low(df['high'], df['low'], window=100)
 ```
 
 ## Contribution
-Any suggestions for improvement or contribution to this project are appreciated! 
+Any suggestions for improvement or contribution to this project are appreciated.
 
 ## Disclaimer
-The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project. 
+The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project.
```

### Comparing `fscraper-1.0.0/fscraper/kabuyohoscraper.py` & `fscraper-1.0.1/fscraper/kabuyohoscraper.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.0/fscraper/reuterscraper.py` & `fscraper-1.0.1/fscraper/reuterscraper.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.0/fscraper/utils.py` & `fscraper-1.0.1/fscraper/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,8 +141,17 @@
 def set_x_days_high_low(high: pd.Series, low: pd.Series, window: int):
     r"""
     Description:
         Set x days high/low price.
     Usage:
         `df['3-day-high'], df['3-day-low'] = set_x_days_high_low(df['high'], df['low'], window=3)`
     """
-    return high.rolling(window=window).max(), low.rolling(window=window).min()
+    return high.rolling(window=window).max(), low.rolling(window=window).min()
+
+def calculate_obv(close: pd.Series, volume: pd.Series):
+    r"""
+    Description:
+        On Balance Volume (OBV)
+    Usage:
+        `df['OBV'] = fs.calculate_obv(df['close'], df['volume'])`
+    """
+    return (np.sign(close.diff()) * volume).fillna(0).cumsum()
```

### Comparing `fscraper-1.0.0/fscraper/xpath_table.py` & `fscraper-1.0.1/fscraper/xpath_table.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.0/fscraper/yfscraper.py` & `fscraper-1.0.1/fscraper/yfscraper.py`

 * *Files identical despite different names*

