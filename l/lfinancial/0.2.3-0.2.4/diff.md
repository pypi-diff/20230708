# Comparing `tmp/lfinancial-0.2.3.tar.gz` & `tmp/lfinancial-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.3.tar", last modified: Sat Jul  8 10:35:59 2023, max compression
+gzip compressed data, was "lfinancial-0.2.4.tar", last modified: Sat Jul  8 13:26:23 2023, max compression
```

## Comparing `lfinancial-0.2.3.tar` & `lfinancial-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:59.424192 lfinancial-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-08 10:35:37.000000 lfinancial-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 10:35:59.424192 lfinancial-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-08 10:35:37.000000 lfinancial-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:59.424192 lfinancial-0.2.3/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:59.424192 lfinancial-0.2.3/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-08 10:35:37.000000 lfinancial-0.2.3/lfinancial/generators/swift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:59.424192 lfinancial-0.2.3/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 10:35:59.000000 lfinancial-0.2.3/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 10:35:59.000000 lfinancial-0.2.3/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:35:59.000000 lfinancial-0.2.3/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 10:35:59.000000 lfinancial-0.2.3/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:35:59.424192 lfinancial-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 10:35:37.000000 lfinancial-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:35:59.424192 lfinancial-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-08 10:35:37.000000 lfinancial-0.2.3/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:23.048183 lfinancial-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-08 13:26:04.000000 lfinancial-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-08 13:26:23.048183 lfinancial-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-08 13:26:04.000000 lfinancial-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:23.044183 lfinancial-0.2.4/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:23.048183 lfinancial-0.2.4/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-08 13:26:04.000000 lfinancial-0.2.4/lfinancial/generators/swift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:23.044183 lfinancial-0.2.4/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-08 13:26:23.000000 lfinancial-0.2.4/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 13:26:23.000000 lfinancial-0.2.4/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:26:23.000000 lfinancial-0.2.4/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 13:26:23.000000 lfinancial-0.2.4/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:26:23.048183 lfinancial-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 13:26:04.000000 lfinancial-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:26:23.048183 lfinancial-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-08 13:26:04.000000 lfinancial-0.2.4/tests/test_document.py
```

### Comparing `lfinancial-0.2.3/LICENSE.txt` & `lfinancial-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/PKG-INFO` & `lfinancial-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -81,8 +81,14 @@
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
 
 f.swift_code()
 # ABOCCNBJ040
+
+f.stock_exchange()
+# Hong Kong Stock Exchange
+
+f.ticker_symbol()
+# AAPL
 ```
```

### Comparing `lfinancial-0.2.3/README.md` & `lfinancial-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -69,8 +69,14 @@
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
 
 f.swift_code()
 # ABOCCNBJ040
+
+f.stock_exchange()
+# Hong Kong Stock Exchange
+
+f.ticker_symbol()
+# AAPL
 ```
```

### Comparing `lfinancial-0.2.3/lfinancial/factory.py` & `lfinancial-0.2.4/lfinancial/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             "area_code": PhoneGenerator(),
             "high_risk": CountryGenerator(),
             "email": EmailGenerator(),
             "bank": BankGenerator(),
             "currency": CurrencyGenerator(),
             "swift_code": SwiftGenerator(),
             "stock_exchange": StockGenerator(),
+            "ticker_symbol": StockGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.2.3/lfinancial/financial.py` & `lfinancial-0.2.4/lfinancial/financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
     def swift_code(self, country=None):
         return self.__generate("swift_code", country)
 
     def stock_exchange(self, country=None):
         return self.__generate("stock_exchange", country)
 
+    def ticker_symbol(self, country=None):
+        return self.__generate("ticker_symbol", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -80,7 +83,8 @@
     print(f.area_code())
     print(f.high_risk_country())
     print(f.email())
     print(f.bank())
     print(f.currency())
     print(f.swift_code())
     print(f.stock_exchange())
+    print(f.ticker_symbol())
```

### Comparing `lfinancial-0.2.3/lfinancial/generators/bank.py` & `lfinancial-0.2.4/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/const.py` & `lfinancial-0.2.4/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/contry.py` & `lfinancial-0.2.4/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/currency.py` & `lfinancial-0.2.4/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/document.py` & `lfinancial-0.2.4/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/mail.py` & `lfinancial-0.2.4/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/name.py` & `lfinancial-0.2.4/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/phone.py` & `lfinancial-0.2.4/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial/generators/swift.py` & `lfinancial-0.2.4/lfinancial/generators/swift.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.4/lfinancial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -81,8 +81,14 @@
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
 
 f.swift_code()
 # ABOCCNBJ040
+
+f.stock_exchange()
+# Hong Kong Stock Exchange
+
+f.ticker_symbol()
+# AAPL
 ```
```

### Comparing `lfinancial-0.2.3/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.2.4/lfinancial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.3/setup.py` & `lfinancial-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.3',
+    version='0.2.4',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

