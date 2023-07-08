# Comparing `tmp/lfinancial-0.2.1.tar.gz` & `tmp/lfinancial-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.1.tar", last modified: Fri Jul  7 15:08:03 2023, max compression
+gzip compressed data, was "lfinancial-0.2.2.tar", last modified: Sat Jul  8 03:37:33 2023, max compression
```

## Comparing `lfinancial-0.2.1.tar` & `lfinancial-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-07 15:07:42.000000 lfinancial-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 15:08:03.055751 lfinancial-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 15:07:42.000000 lfinancial-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/phone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:08:03.059751 lfinancial-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 15:07:42.000000 lfinancial-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 15:07:42.000000 lfinancial-0.2.1/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:33.392707 lfinancial-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-08 03:37:16.000000 lfinancial-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 03:37:33.392707 lfinancial-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-08 03:37:16.000000 lfinancial-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:33.388707 lfinancial-0.2.2/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:33.392707 lfinancial-0.2.2/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-08 03:37:16.000000 lfinancial-0.2.2/lfinancial/generators/swift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:33.388707 lfinancial-0.2.2/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-08 03:37:33.000000 lfinancial-0.2.2/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-08 03:37:33.000000 lfinancial-0.2.2/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 03:37:33.000000 lfinancial-0.2.2/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 03:37:33.000000 lfinancial-0.2.2/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 03:37:33.392707 lfinancial-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 03:37:16.000000 lfinancial-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:37:33.392707 lfinancial-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-08 03:37:16.000000 lfinancial-0.2.2/tests/test_document.py
```

### Comparing `lfinancial-0.2.1/LICENSE.txt` & `lfinancial-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/PKG-INFO` & `lfinancial-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -78,8 +78,11 @@
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
+
+f.swift_code()
+# ABOCCNBJ040
 ```
```

### Comparing `lfinancial-0.2.1/README.md` & `lfinancial-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -66,8 +66,11 @@
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
+
+f.swift_code()
+# ABOCCNBJ040
 ```
```

### Comparing `lfinancial-0.2.1/lfinancial/factory.py` & `lfinancial-0.2.2/lfinancial/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from lfinancial.generators.bank import BankGenerator
 from lfinancial.generators.contry import CountryGenerator
 from lfinancial.generators.currency import CurrencyGenerator
 from lfinancial.generators.document import IDCodeGenerator
 from lfinancial.generators.mail import EmailGenerator
 from lfinancial.generators.name import NameGenerator
 from lfinancial.generators.phone import PhoneGenerator
+from lfinancial.generators.swift import SwiftGenerator
 
 
 class GeneratorFactory:
     def __init__(self):
         self.generators = {
             "SSN": IDCodeGenerator(),
             "IDCard": IDCodeGenerator(),
@@ -22,14 +23,15 @@
             "kana_name": NameGenerator(),
             "cellphone": PhoneGenerator(),
             "area_code": PhoneGenerator(),
             "high_risk": CountryGenerator(),
             "email": EmailGenerator(),
             "bank": BankGenerator(),
             "currency": CurrencyGenerator(),
+            "swift_code": SwiftGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.2.1/lfinancial/financial.py` & `lfinancial-0.2.2/lfinancial/financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
     def bank(self, country=None):
         return self.__generate("bank", country)
 
     def currency(self, country=None):
         return self.__generate("currency", country)
 
+    def swift_code(self, country=None):
+        return self.__generate("swift_code", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -71,8 +74,9 @@
     print(f.kana_name())
     print(f.cn_name())
     print(f.cellphone())
     print(f.area_code())
     print(f.high_risk_country())
     print(f.email())
     print(f.bank())
-    print(f.currency())
+    print(f.currency())
+    print(f.swift_code())
```

### Comparing `lfinancial-0.2.1/lfinancial/generators/bank.py` & `lfinancial-0.2.2/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/const.py` & `lfinancial-0.2.2/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/contry.py` & `lfinancial-0.2.2/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/currency.py` & `lfinancial-0.2.2/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/document.py` & `lfinancial-0.2.2/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/mail.py` & `lfinancial-0.2.2/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/name.py` & `lfinancial-0.2.2/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial/generators/phone.py` & `lfinancial-0.2.2/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.1/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.2/lfinancial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -78,8 +78,11 @@
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
 
 f.currency()
 # CNY
+
+f.swift_code()
+# ABOCCNBJ040
 ```
```

### Comparing `lfinancial-0.2.1/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.2.2/lfinancial.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 lfinancial/generators/const.py
 lfinancial/generators/contry.py
 lfinancial/generators/currency.py
 lfinancial/generators/document.py
 lfinancial/generators/mail.py
 lfinancial/generators/name.py
 lfinancial/generators/phone.py
+lfinancial/generators/swift.py
 tests/test_document.py
```

### Comparing `lfinancial-0.2.1/setup.py` & `lfinancial-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.1',
+    version='0.2.2',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

