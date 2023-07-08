# Comparing `tmp/degiroasync-0.17.0.tar.gz` & `tmp/degiroasync-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.17.0.tar", last modified: Sun Jul  2 20:30:08 2023, max compression
+gzip compressed data, was "degiroasync-0.18.0.tar", last modified: Sat Jul  8 08:42:07 2023, max compression
```

## Comparing `degiroasync-0.17.0.tar` & `degiroasync-0.18.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.498612 degiroasync-0.17.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.17.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5242 2023-07-02 20:30:08.498612 degiroasync-0.17.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4550 2022-07-26 12:50:54.000000 degiroasync-0.17.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.17.0/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4268 2022-04-13 18:57:09.000000 degiroasync-0.17.0/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.17.0/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    26358 2023-07-01 19:46:09.000000 degiroasync-0.17.0/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-02 19:55:02.000000 degiroasync-0.17.0/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.17.0/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6509 2023-07-01 20:41:23.000000 degiroasync-0.17.0/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    13962 2023-07-02 17:26:14.000000 degiroasync-0.17.0/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.17.0/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16478 2023-07-02 19:53:38.000000 degiroasync-0.17.0/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1853 2022-04-05 15:36:45.000000 degiroasync-0.17.0/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-02 17:18:01.000000 degiroasync-0.17.0/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.17.0/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    27905 2023-07-02 17:49:05.000000 degiroasync-0.17.0/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5242 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      251 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.17.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-02 20:30:08.498612 degiroasync-0.17.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2098 2022-07-26 12:37:58.000000 degiroasync-0.17.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.498612 degiroasync-0.17.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.17.0/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.17.0/tests/integration_login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4825 2023-07-02 16:47:13.000000 degiroasync-0.17.0/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    29523 2023-07-02 18:01:35.000000 degiroasync-0.17.0/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    18372 2023-07-02 17:46:52.000000 degiroasync-0.17.0/tests/test_degirowebapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.17.0/tests/test_setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.18.0/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-08 08:42:07.048696 degiroasync-0.18.0/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4352 2023-07-08 08:35:06.000000 degiroasync-0.18.0/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.044696 degiroasync-0.18.0/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.18.0/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4266 2023-07-08 08:13:36.000000 degiroasync-0.18.0/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.18.0/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    31824 2023-07-08 08:24:47.000000 degiroasync-0.18.0/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-02 19:55:02.000000 degiroasync-0.18.0/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.18.0/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6556 2023-07-08 08:00:18.000000 degiroasync-0.18.0/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14273 2023-07-05 15:56:57.000000 degiroasync-0.18.0/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.18.0/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16476 2023-07-08 08:24:23.000000 degiroasync-0.18.0/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1857 2023-07-08 08:08:05.000000 degiroasync-0.18.0/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-02 17:18:01.000000 degiroasync-0.18.0/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.18.0/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    28777 2023-07-08 08:17:42.000000 degiroasync-0.18.0/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.044696 degiroasync-0.18.0/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      293 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.18.0/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-08 08:42:07.048696 degiroasync-0.18.0/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2209 2023-07-07 09:15:51.000000 degiroasync-0.18.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.18.0/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.18.0/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.18.0/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    36370 2023-07-08 08:14:24.000000 degiroasync-0.18.0/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    19359 2023-07-08 08:14:36.000000 degiroasync-0.18.0/tests/test_degirowebapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.18.0/tests/test_setup.py
```

### Comparing `degiroasync-0.17.0/LICENSE` & `degiroasync-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/PKG-INFO` & `degiroasync-0.18.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.17.0
+Version: 0.18.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,18 +22,14 @@
 Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
 
-There are currently several Degiro Python Libraries that were
-active in 2021, check the _Other Python Degiro Libraries_ section for a
-non-exhaustive list and assess which one best fits your needs.
-
 
 ## Precautions
 
 This software is *not* an official Degiro product, nor is it backed by a company.
 It is made available to the users community, as a community effort to enable
 automation of Degiro trading platform.
```

### Comparing `degiroasync-0.17.0/README.md` & `degiroasync-0.18.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
 
-There are currently several Degiro Python Libraries that were
-active in 2021, check the _Other Python Degiro Libraries_ section for a
-non-exhaustive list and assess which one best fits your needs.
-
 
 ## Precautions
 
 This software is *not* an official Degiro product, nor is it backed by a company.
 It is made available to the users community, as a community effort to enable
 automation of Degiro trading platform.
```

### Comparing `degiroasync-0.17.0/degiroasync/__init__.py` & `degiroasync-0.18.0/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/api/__init__.py` & `degiroasync-0.18.0/degiroasync/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     - *login*
       Builds a `Session` instance, this supports login with or without 2FA.
     - *get_portfolio* and *get_portfolio_total*
       Provide data on products currently held on the account.
     - *search_product*
       Find and instantiate DEGIRO products from various search options (text,
       ISIN, symbol, exchange ...).
-    - *get_price_data*
+    - *get_price_series*
       Get price data on a Product.
     - *get_orders* and *check_order*
       Get orders on the account, start placing an order. Note: `webapi` module
       must currently be used to confirm an order.
 
 """
 from .orders import check_order
@@ -65,22 +65,22 @@
 from .session import Session
 from .session import login
 from .session import get_exchange_dictionary
 from .session import ExchangeDictionary
 from .session import Exchange, Region, Country
 from .product import get_portfolio
 from .product import get_portfolio_total
-from .product import get_price_data
+from .product import get_price_series
 from .product import search_product
 from .product import Stock
 from .product import Currency
 from .product import ProductBase
 from .product import ProductFactory  # Don't expose in __all__
 from .product import ProductGeneric
-from .product import PriceSeriesTime
+from .product import PriceSeries
 from .product import TotalPortfolio
 from ..core import Credentials
 from ..core.constants import PRODUCT
 from ..core.constants import PRICE
 from ..core.constants import ORDER
 from ..core.constants import POSITION
 
@@ -98,18 +98,18 @@
             get_exchange_dictionary,
             ExchangeDictionary,
             Exchange, Region, Country,
 
             # Product
             search_product,
             get_portfolio,
-            get_price_data,
+            get_price_series,
 
             # PriceData,
-            PriceSeriesTime,
+            PriceSeries,
             Stock,
             Currency,
             ProductBase,
             ProductGeneric,
 
             get_portfolio,
             get_portfolio_total,
```

### Comparing `degiroasync-0.17.0/degiroasync/api/orders.py` & `degiroasync-0.18.0/degiroasync/api/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/api/product.py` & `degiroasync-0.18.0/degiroasync/api/product.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import Iterable, Any, List, Dict, Union, AnyStr
+from typing import Iterable, Any, List, Dict, Union
 from typing import Optional, AsyncGenerator, Sequence
+from typing import Tuple
+import re
 import logging
 import pprint
 import itertools
 import asyncio
 import datetime
 try:
     from enum import StrEnum
@@ -83,15 +85,15 @@
             what you're doing.
         """
         if not force_init:
             raise NotImplementedError("Please use ProductFactory.init_batch.")
 
     def __repr__(self):
         return (f'<degiroasync.api.product.{self.__class__.__name__} '
-                f'[self.info.name | self.info.symbol]>')
+                f'[{self.info.name} | {self.info.symbol}]>')
 
 
 class ProductFactory:
     @classmethod
     async def init_batch(
             cls,
             session: SessionCore,
@@ -419,209 +421,341 @@
     total_args = dict_from_attr_list(resp_json['totalPortfolio']['value'],
                                      ignore_error=True)
     total_portfolio = TotalPortfolio(camelcase_dict_to_snake(total_args))
 
     return total_portfolio
 
 
-@JSONclass(annotations=True, annotations_type=True)
-class PriceSeries:
-    type: str
-    expires: str
-
-
-@JSONclass(annotations=True, annotations_type=True)
 class PriceSeriesTime:
     """
-    Converted Wrapper for PriceSeriestime for get_price_data.
+    Deprecated: please use PriceSeries class. This will be removed in a future
+    version.
+    """
 
-    times
-        Starting time of the series.
 
-    price
-        Price floats of the series
+class PriceSeries(PriceSeriesTime):
+    type: PRICE.TYPE
+    start: datetime.datetime
+    end: datetime.datetime
+    expires: datetime.datetime
+    resolution: PRICE.RESOLUTION
+    __data: List[List[Union[int, float]]]
+
+    def __init__(
+            self,
+            *,
+            start: datetime.datetime,
+            end: datetime.datetime,
+            currency: str,
+            resolution: PRICE.RESOLUTION,
+            series: Dict[str, List[List[Union[int, float]]]]
+            ):
+        """
+        Base class for price data.
 
-    date
-        Dates in ISO 8601 format. A data point (`date`, `price`) shares the
-        same index in the `price` and `date` list attributes.
+        Attributes
+        ----------
 
-    resolution
-        `PRICE.RESOLUTION` of the data, if known. It may differ from requested
-        resolution.
+        start
+            Start time of the price data series returned by remote API.
+
+        end
+            End time of the price data series returned by remote API.
+
+        currency
+            Currency for the prices data.
+
+        resolution
+            Resolution of the price series.
+            See :class:`~degiroasync.core.PRICE.RESOLUTION`.
+
+        series
+            Price Data Series returned by remote API. For example:
+
+            .. code-block:: python
+                {
+                    'times': '2023-06-29/P1D',
+                    'expires': '2023-07-05T17:54:21.7030064+02:00',
+                    'data': [
+                        [0, 130.54, 131.64, 129.93, 130.46],
+                        [1, 131.16, 132.68, 130.42, 132.36],
+                        [4, 132.8, 133.7, 131.62, 132.61],
+                        [5, 132.6, 132.98, 130.96, 131.32],
+                        [6, 131.2, 133.5, 130.88, 132.82]],
+                    'id': 'ohlc:issueid:350118230',
+                    'type': 'ohlc'
+                }
+        """
+        # Example data containing series:
+        # {
+        #        'requestid': '1',
+        #        'start': '2023-06-29T00:00:00',
+        #        'end': '2023-07-05T00:00:00',
+        #        'resolution': 'P1D',
+        #        'series': [
+        #            {
+        #                'times': '2023-06-29/P1D',
+        #                'expires': '2023-07-05T17:54:21.7030064+02:00',
+        #                'data': [
+        #                    [0, 130.54, 131.64, 129.93, 130.46],
+        #                    [1, 131.16, 132.68, 130.42, 132.36],
+        #                    [4, 132.8, 133.7, 131.62, 132.61],
+        #                    [5, 132.6, 132.98, 130.96, 131.32],
+        #                    [6, 131.2, 133.5, 130.88, 132.82]],
+        #                'id': 'ohlc:issueid:350118230',
+        #                'type': 'ohlc'
+        #                }
+        #            ]
+        #        }
+        self.start = start
+        self.end = end
+
+        expires_str = series['expires']
+        # Example expire_str: '2023-07-05T17:54:21.7030064+02:00'
+        # microseconds will be more then enough, remove extra digit
+        expires_str = re.sub(r'\.(\d{6})\d\+', r'.\1+', expires_str)
+        expires_str = re.sub(r'\+(\d{2}):(\d{2})$', r'+\1\2', expires_str)
+        self.expires = datetime.datetime.strptime(
+                expires_str,
+                '%Y-%m-%dT%H:%M:%S.%f%z'
+                )
+
+        self.resolution = resolution
+        self.currency = currency
+        self.__series = series
+        if series['type'] == 'time':
+            self.type = PRICE.TYPE.PRICE
+        elif series['type'] == 'ohlc':
+            self.type = PRICE.TYPE.OHLC
+        else:
+            raise NotImplementedError(
+                    f"Series type {series['type']} not supported.")
 
-    expires
-        As returned per end point. Can be used as indication when to query
-        for new data.
-    """
-    times: str
-    price: List[float]
-    date: List[str]
-    resolution: Union[PRICE.RESOLUTION, str]
-    expires: str
+    def _get_delta(self):
+        if self.resolution == PRICE.RESOLUTION.PT1D:
+            delta = datetime.timedelta(days=1)
+        elif self.resolution == PRICE.RESOLUTION.PT1M:
+            delta = datetime.timedelta(minutes=1)
+        else:
+            raise NotImplementedError(
+                    f"Resolution {self.resolution} not supported.")
+        return delta
+
+    def _get_dates_it(self) -> Iterable[datetime.datetime]:
+        times_split = self.__series['times'].split('/')
+        start = datetime.datetime.fromisoformat(times_split[0])
+        if len(times_split) > 1:
+            assert PRICE.RESOLUTION(times_split[1]) == self.resolution
+        delta = self._get_delta()
+        data = self.__series['data']
+        delta = self._get_delta()
+        return [start + d[0] * delta for d in data]
+
+    def items(self) -> Iterable[
+            Tuple[str, List[Union[float, datetime.datetime]]]
+                ]:
+        """
+
+        """
+        data = self.__series['data']
+        yield ('date', self._get_dates_it())
+        if self.type == PRICE.TYPE.OHLC:
+            yield ('open', [x[1] for x in data])
+            yield ('high', [x[2] for x in data])
+            yield ('low', [x[3] for x in data])
+            yield ('close', [x[4] for x in data])
+        elif self.type == PRICE.TYPE.PRICE:
+            yield ('close', [x[1] for x in data])
+        else:
+            raise NotImplementedError(f"Price type {self.type} not supported.")
+
+    def iterrows(self) -> Iterable[Dict[str, Union[datetime.datetime, float]]]:
+        """
+        Provide data by columns, can be fed directly to instantiate a
+        `pandas.DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`
+
+        With `pandas.DataFrame`:
+
+            >>> pricedata = PriceData(
+                    start=datetime.datetime(2023, 6, 29),
+                    end=datetime.datetime(2023, 7, 5),
+                    resolution=PRICE.RESOLUTION.OHLC
+                    currency='EUR',
+                    data={
+                        'data': [
+                            [0, 1., 4., 0., 2.],
+                            [1, 2., 4., 0., 2.]
+                            ],
+                        'type': 'ohlc',
+                        'times': '2023-06-29/P1D',
+                        'expires': '2023-07-05T17:54:21.7030064+02:00',
+                        }
+                    )
+            >>> import pandas as pd
+            >>> df = pd.DataFrame(pricedata.iterrows())
+            >>> df.columns
+            Index(['date', 'open', 'high', 'low', 'close'], dtype='object')
+            >>> df.iloc[0]['date']
+            Timestamp('2023-06-29 00:00:00')
+            >>> df['open']
+            0    1.
+            1    2.
+            Name: open, dtype: float64
+        """
+
+        data = self.__series['data']
+        if self.type == PRICE.TYPE.PRICE:
+            for date, row in zip(self._get_dates_it(), data):
+                yield {'date': date, 'close': row[1]}
+        elif self.type == PRICE.TYPE.OHLC:
+            for date, row in zip(self._get_dates_it(), data):
+                yield {
+                        'date': date,
+                        'open': row[1],
+                        'high': row[2],
+                        'low': row[3],
+                        'close': row[4],
+                        }
+        else:
+            raise NotImplementedError(f"Price type {self.type} not supported.")
+
+    @property
+    def date(self):
+        #print(
+        #        "degiroasync.PriceSeries.date is deprecated and will be "
+        #        "removed in a future version. "
+        #        "Please use PriceSeries.items() or PriceSeries.iterrows().",
+        #        file=sys.stderr
+        #        )
+        return [d.isoformat() for d in self._get_dates_it()]
+
+    @property
+    def price(self) -> Sequence[Union[float, Sequence[float]]]:
+        #print(
+        #        "degiroasync.PriceSeries.price is deprecated and will be "
+        #        "removed in a future version. "
+        #        "Please use PriceSeries.items() or PriceSeries.iterrows()",
+        #        file=sys.stderr
+        #        )
+        if self.type == PRICE.TYPE.OHLC:
+            return [row[1:] for row in self.__series['data']]
+        if self.type == PRICE.TYPE.PRICE:
+            return [row[1] for row in self.__series['data']]
+        raise NotImplementedError(
+                f"price is supported only for PRICE.TYPE.PRICE, "
+                f"not {self.type}")
+
+
+class PriceSeriesTime(PriceSeries):
+    """
+    DEPRECATED: This will be removed in a future verison, please use
+    PriceSeries.
+    """
+
+
+async def get_price_data(*args, **kwargs):
+    "DEPRECATED: Please use get_price_series instead."
+    LOGGER.warn(
+            "get_price_data is deprecated, please use get_price_series instead"
+            )
+    return await get_price_series(*args, **kwargs)
 
 
 # 2022.04: mypy limited support for StrEnum, ignore until proper support.
-async def get_price_data(
+async def get_price_series(
         session: SessionCore,
         product: Stock,
-        resolution: PRICE.RESOLUTION = PRICE.RESOLUTION.PT1M,  # type: ignore
-        period: PRICE.PERIOD = PRICE.PERIOD.P1DAY,  # type: ignore
+        resolution: PRICE.RESOLUTION = PRICE.RESOLUTION.PT1D,  # type: ignore
+        period: PRICE.PERIOD = PRICE.PERIOD.P1MONTH,  # type: ignore
         timezone: str = 'Europe/Paris',
         culture: str = 'fr-FR',
         data_type: PRICE.TYPE = PRICE.TYPE.PRICE  # type: ignore
-        ) -> PriceSeriesTime:
+        ) -> PriceSeries:
     """
     Get price data for `product`.
 
+    Parameters
+    ----------
     product
         Product to look for the data.
 
     resolution
-        How close do we request data points to be.
+        How often do we want data points.
+
+        See :class:`~degiroasync.core.constants.PRICE.RESOLUTION` for available
+        values.
 
     period
-        How long of data do we want
+        Period between now and data starting point.
+
+        See :class:`~degiroasync.core.constants.PRICE.PERIOD` for available
+        values.
 
     data_type
         Specify if we want raw price, or 'ohlc' (open, high, low, close)
         information. The latter might be useful for long periods where high
         resolution is not available.
 
+        See :class:`~degiroasync.core.constants.PRICE.TYPE` for available
+        values.
+
     Returns
     -------
         PriceSeriesTime
             Contains price data and time information.
 
     """
     # Ensure product got results of product_info
     if product.info.product_type_id != PRODUCT.TYPEID.STOCK:
         raise NotImplementedError(
             "Only productTypeId == PRODUCT.TYPEID.STOCK is currently "
-            "supported by get_price_data")
-    resp_json = await webapi.get_price_data(
+            "supported by get_price_series")
+    resp_json = await webapi.get_price_series(
         session,
         vwdId=product.info.vwd_id,
         vwdIdentifierType=product.info.vwd_identifier_type,
         resolution=resolution,
         period=period,
         timezone=timezone,
         culture=culture,
-        data_type=data_type)
-    LOGGER.debug("api.get_price_data resp_json| %s", resp_json)
-    timeseries_ind = -1
+        data_type=data_type,
+        )
+    LOGGER.debug("api.get_price_series resp_json| %s", resp_json)
+
+    # Look for price series
+    series_ind = -1
     objectseries_ind = -1
-    # Look for time series
     for ind, series in enumerate(resp_json['series']):
         if series['type'] == 'time':
-            timeseries_ind = ind
+            assert series_ind < 0, "Unexpected more than 1 series."
+            series_ind = ind
         if series['type'] == 'object':
-            objectseries_ind = ind  # Might be used in later revisions.
-    if timeseries_ind < 0:
-        raise ResponseError("No 'time' series found in answer.")
-    converted_time_series = convert_time_series(resp_json['series'][ind])
-    converted_time_series['date'] = converted_time_series['data']['date']
-    converted_time_series['price'] = converted_time_series['data']['price']
-    try:
-        resolution_out = PRICE.RESOLUTION(converted_time_series['resolution'])
-        converted_time_series['resolution'] = resolution_out
-    except ValueError:
-        LOGGER.debug(
-                "converted_time_series['resolution'] is unknown: %s. "
-                "Leave as str",
-                converted_time_series['resolution']
-                )
-    del converted_time_series['data']
-    return PriceSeriesTime(converted_time_series)
-
-
-def convert_time_series(
-        data_series: Dict[str, Union[str, List[Union[float, int]]]]
-    ) -> Dict[str,
-              Union[str, Dict[str, Union[float, str]]]
-              ]:
-    """
-    Helper to convert data series.
-
-    Aims to make it easier to feed inin a pandas friendly format.
-
-    >>> data = {
-    ...     "times": "2022-01-20T00:00:00/PT1M",
-    ...     "expires": "2022-01-20T10:12:56+01:00",
-    ...     "data": [
-    ...         [
-    ...             540,
-    ...             114.0
-    ...         ],
-    ...         [
-    ...             541,
-    ...             114.08
-    ...         ],
-    ...         [
-    ...             542,
-    ...             114.12
-    ...         ]
-    ...     ]
-    ... }
-    >>> data_out = convert_time_series(data)
-    {
-
-        "type": "time",
-        "times": "2022-01-20T00:00:00",
-        "resolution": "PT1M",
-        "expires": "2022-01-20T10:11:53+01:00",
-        "data": {
-            'price': [114.0, 114.08, 114.12],
-            'date': [
-                '2022-01-20T09:00:00',
-                '2022-01-20T09:01:00',
-                '2022-01-20T09:02:00']
-        }
-    }
-
-    """
-    time_t, resolution_t = data_series['times'].split('/')
-    data_out: Dict[str, Any] = data_series.copy()
-
-    for key in ('times', 'expires', 'data'):
-        if key not in data_series:
-            raise KeyError(f'{key} not found in data_series {data_series}')
-
-    resolution_whitelist = (PRICE.RESOLUTION.PT1M, PRICE.RESOLUTION.PT1D)
-    if resolution_t not in resolution_whitelist:
-        raise NotImplementedError("convert_time_series has not been tested "
-                                  "with resolutions other than {}. "
-                                  "Received resolution: {}".format(
-                                        resolution_whitelist,
-                                        resolution_t
-                                        )
-                                  )
-
-    data_new: Dict[str, Union[Sequence[str], Sequence[float]]] = {
-        'price': [],
-        'date': [],
-        }
-    data_out['data'] = data_new
-    data_out['type'] = 'time'
-    data_out['resolution'] = resolution_t
-    data_out['times'] = time_t
-    # Multiplier to get time delta (in minutes) from time index
-    # returned by API.
-    time_multiplier: int = {
-        PRICE.RESOLUTION.PT1M: 1,
-        PRICE.RESOLUTION.PT1D: 60*24
-        }[resolution_t]
-
-    start_date = datetime.datetime.fromisoformat(time_t)
-    for kv in data_series['data']:
-        data_new['price'].append(float(kv[1]))
-        time_ind = kv[0]
-        time_delta = float(time_ind) * time_multiplier
-        measure_date = start_date + datetime.timedelta(minutes=time_delta)
-        data_new['date'].append(measure_date.isoformat())
-    return data_out
+            # This is not always returned by API, don't rely on it
+            objectseries_ind = ind
+        if series['type'] == 'ohlc':
+            assert series_ind < 0, "Unexpected more than 1 series"
+            series_ind = ind
+
+    if series_ind < 0:
+        raise ResponseError("No 'time' or 'ohlc' series found in answer.")
+    if objectseries_ind < 0:
+        # Check currency if we have info
+        object_series = resp_json['series'][objectseries_ind]
+        if 'currency' in object_series.get('data', {}):
+            assert object_series['data']['currency'] == product.info.currency
+
+    series_d = resp_json['series'][series_ind]
+    prices_series = PriceSeries(
+            start=datetime.datetime.fromisoformat(resp_json['start']),
+            end=datetime.datetime.fromisoformat(resp_json['end']),
+            resolution=PRICE.RESOLUTION(resp_json['resolution']),
+            currency=product.info.currency,
+            series=series_d,
+            )
+    return prices_series
 
 
 async def search_product(
         session: Session,
         *,
         by_text: Optional[str] = None,
         by_isin: Optional[str] = None,
@@ -664,15 +798,15 @@
             by_text = by_symbol
         elif by_isin is not None:
             by_text = by_isin
         else:
             raise AssertionError(
                     "by_text is None and no search parameters was set or "
                     "found. Have you set a search parameters to "
-                    "get_price_data?"
+                    "get_price_series?"
                     "\n If yes, this shouldn't be happening, please open a bug"
                     " report."
                     )
 
     exchange_id = None
     if by_exchange is not None:
         if isinstance(by_exchange, Exchange):
@@ -746,18 +880,19 @@
 __all__ = [
     obj.__name__ for obj in (  # type: ignore
         # Login & setup
         Credentials,
         Session,
         SessionCore,
         Config,
+        PriceSeries,
 
         # Product data structures
         # PriceData,
         Stock,
         Currency,
         ProductBase,
         get_portfolio,
-        get_price_data,
+        get_price_series,
         search_product
     )
 ]
```

### Comparing `degiroasync-0.17.0/degiroasync/api/session.py` & `degiroasync-0.18.0/degiroasync/api/session.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/core/__init__.py` & `degiroasync-0.18.0/degiroasync/core/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/core/constants.py` & `degiroasync-0.18.0/degiroasync/core/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,21 +267,23 @@
     class RESOLUTION(StrEnum):
         # Resolution
         PT1M = 'PT1M'  # Higher resolution, 1 minute
         PT1D = 'P1D'   # 1 tic per day
 
     class PERIOD(StrEnum):
         # Periods
-        # P stands for Prior
+        # P stands for Prior?
         P1DAY = 'P1D'
         P1WEEK = 'P1W'
         P1MONTH = 'P1M'
         P3MONTH = 'P3M'
         P6MONTH = 'P6M'
         P1YEAR = 'P1Y'
+        P3YEAR = 'P3Y'
+        P5YEAR = 'P5Y'
         P50YEAR = 'P50Y'
 
     class TYPE(StrEnum):
         PRICE = 'price'
         OHLC = 'ohlc'
```

### Comparing `degiroasync-0.17.0/degiroasync/core/core.py` & `degiroasync-0.18.0/degiroasync/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,32 +158,45 @@
 @dataclasses.dataclass
 class SessionCore:
     JSESSIONID = 'JSESSIONID'
 
     config: Optional[Config] = None
     client: Optional[PAClient] = None
 
-    _max_requests_default: int = 30
+    _max_requests_default: int = 40
     _period_seconds_default: int = 1
 
     # Cookies
-    # Wrap to not leak httpx
     _cookies: Optional[httpx.Cookies] = None
     _http_client: Optional[ThrottlingClient] = None
 
     @property
     def cookies(self):
         return dict(self._cookies)
 
     def update_throttling(
             self,
             max_requests: int = 20,
             period_seconds: float = 1
             ):
-        "Update throttling parameters. No limit if max_requests <= 0."
+        """
+        Update throttling parameters. No limit if max_requests <= 0.
+
+        Note: going over 40 requests per second seems to trigger API bans.
+
+        Parameters
+        ----------
+
+        max_requests
+            Maximum number of requests per `period_seconds` before throttling.
+            If <= 0, no limit.
+
+        period_seconds
+            Period on which to count requests.
+        """
         if self._http_client is None:
             self._max_requests_default = max_requests
             self._period_seconds_default = period_seconds
         else:
             self._http_client._max_requests = max_requests
             self._http_client._period_s = period_seconds
```

### Comparing `degiroasync-0.17.0/degiroasync/core/exceptions.py` & `degiroasync-0.18.0/degiroasync/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/core/helpers.py` & `degiroasync-0.18.0/degiroasync/core/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from .constants import LOGGER_NAME
 from .constants import LOGIN
 from .exceptions import ResponseError
 from .exceptions import BadCredentialsError
 
 
 LOGGER = logging.getLogger(LOGGER_NAME)
+# Logs helpers
+FORMAT_DEFAULT = '%(asctime)s-%(name)s-%(levelname)s- %(message)s'
+STREAMHANDLER_DEFAULT = logging.StreamHandler(stream=sys.stdout)
 
 
 class CoroCache:
     def __init__(self, coro: Coroutine):
         """
         Cache to allow awaiting coroutines several times.
 
@@ -509,12 +512,7 @@
     async def options(self, *args, **kwargs):
         return await self._client_open.options(*args, **kwargs)
 
     @_throttle
     @functools.wraps(httpx.AsyncClient.delete)
     async def delete(self, *args, **kwargs):
         return await self._client_open.delete(*args, **kwargs)
-
-
-# Logs helpers
-FORMAT_DEFAULT = '%(asctime)s-%(name)s-%(levelname)s- %(message)s'
-STREAMHANDLER_DEFAULT = logging.StreamHandler(stream=sys.stdout)
```

### Comparing `degiroasync-0.17.0/degiroasync/webapi/__init__.py` & `degiroasync-0.18.0/degiroasync/webapi/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .login import get_account_info
 from .product import get_products_info
 from .product import search_product
 from .product import get_portfolio
 from .product import get_portfolio_total
 from .product import get_company_profile
 from .product import get_news_by_company
-from .product import get_price_data
+from .product import get_price_series
 from .orders import get_orders
 from .orders import get_orders_history
 from .orders import get_transactions
 from .orders import confirm_order
 from .orders import check_order
 from .orders import ORDER_DATE_FORMAT
 
@@ -46,15 +46,15 @@
                 # product
                 get_portfolio,
                 get_portfolio_total,
                 get_products_info,
                 search_product,
                 get_company_profile,
                 get_news_by_company,
-                get_price_data,
+                get_price_series,
                 # orders
                 get_orders,
                 get_orders_history,
                 get_transactions,
                 confirm_order,
                 check_order,
         )
```

### Comparing `degiroasync-0.17.0/degiroasync/webapi/login.py` & `degiroasync-0.18.0/degiroasync/webapi/login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/webapi/orders.py` & `degiroasync-0.18.0/degiroasync/webapi/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/degiroasync/webapi/product.py` & `degiroasync-0.18.0/degiroasync/webapi/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,139 +629,159 @@
             })
     check_response(response)
     resp_json = response.json()
     LOGGER.debug("get_news_by_company| %s", resp_json)
     return resp_json
 
 
-async def get_price_data(
+async def get_price_data(*args, **kwargs):
+    "DEPRECATED: Please use get_price_series instead"
+    LOGGER.warn(
+            "get_price_data is deprecated, please use get_price_series "
+            "instead."
+            )
+    return await get_price_series(*args, **kwargs)
+
+
+async def get_price_series(
         session: SessionCore,
         vwdId: str,
         vwdIdentifierType: str,
-        resolution: PRICE.RESOLUTION = PRICE.RESOLUTION.PT1M,
-        period: PRICE.PERIOD = PRICE.PERIOD.P1DAY,
+        resolution: PRICE.RESOLUTION = PRICE.RESOLUTION.PT1D,
+        period: PRICE.PERIOD = PRICE.PERIOD.P1MONTH,
         timezone: str = 'Europe/Paris',
         culture: str = 'fr-FR',
         data_type: PRICE.TYPE = PRICE.TYPE.PRICE
 ) -> Dict[str, Any]:
     """
     Get price data for a company.
 
+    Parameters
+    ----------
+
     data_type = 'ohlc' provides access to 'Open', 'High', 'Low', 'Close' in
     that order for each period, instead of price data.
 
     vwdIdentifierType can be 'issueid' or 'vwdkey'
 
+    Returns
+    -------
     Example returned JSON:
-    {
-        "requestid": "1",
-        "start": "2022-01-20T00:00:00",
-        "end": "2022-01-20T14:12:24",
-        "resolution": "PT1M",
-        "series": [
-            {
-                "expires": "2022-01-20T10:12:56+01:00",
-                "data": {
-                    "issueId": 360114899,
-                    "companyId": 1001,
-                    "name": "AIRBUS",
-                    "identifier": "issueid:360114899",
-                    "isin": "NL0000235190",
-                    "alfa": "AIR15598",
-                    "market": "XPAR",
-                    "currency": "EUR",
-                    "type": "AAN",
-                    "quality": "REALTIME",
-                    "lastPrice": 113.1,
-                    "lastTime": "2022-01-21T14:12:24",
-                    "absDiff": -2.62,
-                    "relDiff": -0.02264,
-                    "highPrice": 114.46,
-                    "highTime": "2022-01-21T10:31:14",
-                    "lowPrice": 112.78,
-                    "lowTime": "2022-01-21T13:56:36",
-                    "openPrice": 114.0,
-                    "openTime": "2022-01-21T09:00:19",
-                    "closePrice": 114.0,
-                    "closeTime": "2022-01-21T09:00:19",
-                    "cumulativeVolume": 857092.0,
-                    "previousClosePrice": 115.72,
-                    "previousCloseTime": "2022-01-20T17:35:03",
-                    "tradingStartTime": "09:00:00",
-                    "tradingEndTime": "17:40:00",
-                    "tradingAddedTime": "00:10:00",
-                    "lowPriceP1Y": 81.84,
-                    "highPriceP1Y": 121.1,
-                    "windowStart": "2022-01-20T00:00:00",
-                    "windowEnd": "2022-01-20T10:11:22",
-                    "windowFirst": "2022-01-20T09:00:00",
-                    "windowLast": "2022-01-20T10:11:00",
-                    "windowHighTime": "2022-01-20T10:11:00",
-                    "windowHighPrice": 114.46,
-                    "windowLowTime": "2022-01-20T10:16:00",
-                    "windowLowPrice": 112.78,
-                    "windowOpenTime": "2022-01-20T09:00:19",
-                    "windowOpenPrice": 114.0,
-                    "windowPreviousCloseTime": "2022-01-19T17:35:03",
-                    "windowPreviousClosePrice": 115.72,
-                    "windowTrend": -0.02264
-                },
-                "id": "issueid:360114899",
-                "type": "object"
-                "times": "2022-01-20T00:00:00",
-                "expires": "2022-01-20T10:12:56+01:00",
-                "data": [
-                    [
-                    540,
-                    114.0
-                    ],
-                    [
-                    541,
-                    114.08
-                    ],
-                    [
-                    542,
-                    113.62
-                    ],
-                    [
-                    543,
-                    113.8
-                    ],
-                    ...
-                    [
-                    552,
-                    113.7
-                    ]],
-            "id":"price:issueid:360114899",
-            "type":"time"}]
-        }
+
+    .. code-block:: json
+
+        {
+            "requestid": "1",
+            "start": "2022-01-20T00:00:00",
+            "end": "2022-01-20T14:12:24",
+            "resolution": "PT1M",
+            "series": [
+                {
+                    "expires": "2022-01-20T10:12:56+01:00",
+                    "data": {
+                        "issueId": 360114899,
+                        "companyId": 1001,
+                        "name": "AIRBUS",
+                        "identifier": "issueid:360114899",
+                        "isin": "NL0000235190",
+                        "alfa": "AIR15598",
+                        "market": "XPAR",
+                        "currency": "EUR",
+                        "type": "AAN",
+                        "quality": "REALTIME",
+                        "lastPrice": 113.1,
+                        "lastTime": "2022-01-21T14:12:24",
+                        "absDiff": -2.62,
+                        "relDiff": -0.02264,
+                        "highPrice": 114.46,
+                        "highTime": "2022-01-21T10:31:14",
+                        "lowPrice": 112.78,
+                        "lowTime": "2022-01-21T13:56:36",
+                        "openPrice": 114.0,
+                        "openTime": "2022-01-21T09:00:19",
+                        "closePrice": 114.0,
+                        "closeTime": "2022-01-21T09:00:19",
+                        "cumulativeVolume": 857092.0,
+                        "previousClosePrice": 115.72,
+                        "previousCloseTime": "2022-01-20T17:35:03",
+                        "tradingStartTime": "09:00:00",
+                        "tradingEndTime": "17:40:00",
+                        "tradingAddedTime": "00:10:00",
+                        "lowPriceP1Y": 81.84,
+                        "highPriceP1Y": 121.1,
+                        "windowStart": "2022-01-20T00:00:00",
+                        "windowEnd": "2022-01-20T10:11:22",
+                        "windowFirst": "2022-01-20T09:00:00",
+                        "windowLast": "2022-01-20T10:11:00",
+                        "windowHighTime": "2022-01-20T10:11:00",
+                        "windowHighPrice": 114.46,
+                        "windowLowTime": "2022-01-20T10:16:00",
+                        "windowLowPrice": 112.78,
+                        "windowOpenTime": "2022-01-20T09:00:19",
+                        "windowOpenPrice": 114.0,
+                        "windowPreviousCloseTime": "2022-01-19T17:35:03",
+                        "windowPreviousClosePrice": 115.72,
+                        "windowTrend": -0.02264
+                    },
+                    "id": "issueid:360114899",
+                    "type": "object"
+                    "times": "2022-01-20T00:00:00",
+                    "expires": "2022-01-20T10:12:56+01:00",
+                    "data": [
+                        [
+                        540,
+                        114.0
+                        ],
+                        [
+                        541,
+                        114.08
+                        ],
+                        [
+                        542,
+                        113.62
+                        ],
+                        [
+                        543,
+                        113.8
+                        ],
+                        ...
+                        [
+                        552,
+                        113.7
+                        ]],
+                "id":"price:issueid:360114899",
+                "type":"time"}]
+            }
     """
+    # TODO: There may be an issue with the above JSON example, review.
     if vwdIdentifierType not in ('issueid', 'vwdkey'):
         raise ValueError("vwdIdentifierType must be 'issueid' or 'vwdkey'")
 
     check_session_config(session)
     url = URLs.get_price_data_url(session)
-    LOGGER.debug('get_price_data url| %s', url)
+    LOGGER.debug('get_price_series url| %s', url)
     params = {
         'requestid': 1,
-        'resolution': resolution,
+        'resolution': str(resolution),
         'culture': culture,
-        'period': period,
-        'series': f'price:{vwdIdentifierType}:{vwdId}',
+        'period': str(period),
+        'series': f'{data_type}:{vwdIdentifierType}:{vwdId}',
         'format': 'json',
         'userToken': session.config.client_id
     }
-    LOGGER.debug('get_price_data params| %s', params)
+    LOGGER.debug('get_price_series params| %s', params)
     async with session as client:
+        # 2023: Cookies are not needed for that call.
+        # Since it looks like a third party, don't share session id if not
+        # needed.
         response = await client.get(url,
-                                    cookies=session.cookies,
                                     params=params)
     check_response(response)
     resp_json = response.json()
-    LOGGER.debug('get_price_data response| %s', resp_json)
+    LOGGER.debug('get_price_series response| %s', resp_json)
     return resp_json
 
 
 async def get_trading_update(
         session: SessionCore,
         params: Dict[str, int]
 ) -> Dict[str, Any]:
@@ -884,9 +904,9 @@
 
 
 __all__ = [
     get_portfolio.__name__,
     get_portfolio_total.__name__,
     get_news_by_company.__name__,
     get_company_profile.__name__,
-    get_price_data.__name__,
+    get_price_series.__name__,
 ]
```

### Comparing `degiroasync-0.17.0/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.18.0/degiroasync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.17.0
+Version: 0.18.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,18 +22,14 @@
 Check out the online documentation [here](https://ohmajesticlama.github.io/degiroasync/index.html).
 
 ## Introduction
 
 This project aims to provide an *unofficial* API for Degiro platform that works
 asynchronously.
 
-There are currently several Degiro Python Libraries that were
-active in 2021, check the _Other Python Degiro Libraries_ section for a
-non-exhaustive list and assess which one best fits your needs.
-
 
 ## Precautions
 
 This software is *not* an official Degiro product, nor is it backed by a company.
 It is made available to the users community, as a community effort to enable
 automation of Degiro trading platform.
```

### Comparing `degiroasync-0.17.0/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.18.0/degiroasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/setup.py` & `degiroasync-0.18.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,37 +11,38 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.17.0",
+        version="0.18.0",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
                 'https://ohmajesticlama.github.io/degiroasync/index.html'
             },
         packages=setuptools.find_packages(),
         install_requires=[
-            'httpx >= 0.21.3',
-            'jsonloader >= 0.8.1',
-            'typeguard >= 2.13.3',
-            'asyncstdlib >= 3.10.3',
-            'more_itertools >= 8.12.0'
+            'httpx >= 0.21.3, < 1.0',
+            'jsonloader >= 0.8.1, < 1.0',
+            'typeguard >= 2.13.3, < 3.0',
+            'asyncstdlib >= 3.10.3, < 4.0',
+            'more_itertools >= 8.12.0, < 9'
             ],
         extras_require={
             'dev': [
                 # Tests
                 'pytest >= 7.0.1',
                 'coverage >= 6.3',
+                'pandas >= 2.0.3, <3.0',  # For testing integration w/ pandas
                 # Code quality
                 'flake8 >= 4.0.1',
                 'mypy >= 0.931',
                 # For shipping
                 'build >= 0.7.0',
                 'twine >= 3.8.0',
                 # Documentation
```

### Comparing `degiroasync-0.17.0/tests/integration_login.py` & `degiroasync-0.18.0/tests/integration_login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.17.0/tests/test_core.py` & `degiroasync-0.18.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,7 +140,8 @@
             calls.append(client.get())
         for c in calls:
             await c
         del calls
         self.assertGreaterEqual(
                 time.time() - start,
                 (n_calls-max_requests) * period_seconds / max_requests)
+
```

### Comparing `degiroasync-0.17.0/tests/test_degiroapi.py` & `degiroasync-0.18.0/tests/test_degiroapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import degiroasync
 import degiroasync.webapi
 import degiroasync.api
 import degiroasync.webapi
 import degiroasync.core
 import degiroasync.core.helpers
 from degiroasync.core import Credentials
-from degiroasync.api.product import convert_time_series
+#from degiroasync.api.product import convert_time_series
 from degiroasync.api import ProductFactory
 from degiroasync.api import Order
 from degiroasync.api import ORDER
 from degiroasync.api import Exchange
 from degiroasync.core.constants import PRODUCT
 from degiroasync.core.constants import PRICE
 from degiroasync.core import BadCredentialsError
@@ -35,15 +35,15 @@
 
 LOGGER.debug('Python Version: %s', sys.version)
 
 RUN_INTEGRATION_TESTS = 0
 try:
     _env_var = os.environ.get('DEGIROASYNC_INTEGRATION')
     RUN_INTEGRATION_TESTS = int(_env_var)
-except ValueError:
+except (ValueError, TypeError):
     LOGGER.info('degiroasync integration tests will *not* run.')
 del _env_var
 
 
 #############
 # Unittests #
 #############
@@ -149,52 +149,52 @@
 
         for o in (order, orderh):
             self.assertEqual(order.order_id, 'weiurpoiwejaklsj')
             self.assertEqual(order.size, 50)
             self.assertEqual(order.buysell, ORDER.ACTION.BUY)
 
 
-class TestDegiroAsyncAPIHelpers(unittest.TestCase):
-    def test_convert_time_series(self):
-        data = {
-            "times": "2022-01-20T00:00:00/PT1M",
-            "expires": "2022-01-20T10:12:56+01:00",
-            "data": [
-                [
-                    540,
-                    114.0
-                ],
-                [
-                    541,
-                    114.08
-                ],
-                [
-                    542,
-                    114.12
-                ]
-            ]
-        }
-        data_out = convert_time_series(data)
-        self.maxDiff = None
-        self.assertEqual(
-                data_out,
-                {
-
-                    "type": "time",
-                    "times": "2022-01-20T00:00:00",
-                    "resolution": "PT1M",
-                    "expires": "2022-01-20T10:12:56+01:00",
-                    "data": {
-                        'price': [114.0, 114.08, 114.12],
-                        'date': [
-                            '2022-01-20T09:00:00',
-                            '2022-01-20T09:01:00',
-                            '2022-01-20T09:02:00']
-                    }
-                })
+#class TestDegiroAsyncAPIHelpers(unittest.TestCase):
+#    def test_convert_time_series(self):
+#        data = {
+#            "times": "2022-01-20T00:00:00/PT1M",
+#            "expires": "2022-01-20T10:12:56+01:00",
+#            "data": [
+#                [
+#                    540,
+#                    114.0
+#                ],
+#                [
+#                    541,
+#                    114.08
+#                ],
+#                [
+#                    542,
+#                    114.12
+#                ]
+#            ]
+#        }
+#        data_out = convert_time_series(data)
+#        self.maxDiff = None
+#        self.assertEqual(
+#                data_out,
+#                {
+#
+#                    "type": "time",
+#                    "times": "2022-01-20T00:00:00",
+#                    "resolution": "PT1M",
+#                    "expires": "2022-01-20T10:12:56+01:00",
+#                    "data": {
+#                        'price': [114.0, 114.08, 114.12],
+#                        'date': [
+#                            '2022-01-20T09:00:00',
+#                            '2022-01-20T09:01:00',
+#                            '2022-01-20T09:02:00']
+#                    }
+#                })
 
 
 class TestExchangeDictionary(unittest.IsolatedAsyncioTestCase):
     "Unittest for api.ExchangeDictionary"
     def setUp(self):
         resp_mock = unittest.mock.MagicMock()
         self._product_dictionary_dummy = {
@@ -327,28 +327,14 @@
         self.assertEqual(products[0].info.name, 'foo')
         self.assertEqual(products[0].info.symbol, 'FOO')
         self.assertIsInstance(repr(products[0]), str)  # don't raise exception
 
     @unittest.mock.patch('degiroasync.webapi.get_products_info')
     async def test_product_no_batch(self, wapi_prodinfo_m):
         # Same as test_product but with size=1 to test corner case.
-        # Mock get_products_info
-        #resp = MagicMock()
-        #resp.json = MagicMock(return_value={'data': {
-        #    '123': {
-        #        'id': '123',
-        #        'product_type_id': 'UNKNOWNPRODUCTID',
-        #        'name': 'foo',
-        #        'symbol': 'FOO',
-        #        'currency': 'EUR',
-        #        'exchangeId': 'exid',
-        #        'tradable': True,
-        #        'isin': 'isinexample',
-        #    }
-        #    }})
         wapi_prodinfo_m.return_value = {'data': {
                 '123': {
                     'id': '123',
                     'product_type_id': 99,
                     'name': 'foo',
                     'symbol': 'FOO',
                     'currency': 'EUR',
@@ -373,14 +359,183 @@
         self.assertEqual(len(products), 1)
         self.assertEqual(products[0].base.id, '123')
         self.assertEqual(products[0].base.additional, 123)
         self.assertEqual(products[0].info.name, 'foo')
         self.assertEqual(products[0].info.symbol, 'FOO')
 
 
+class TestDegiroasyncPrice(
+        unittest.IsolatedAsyncioTestCase):
+
+    def test_priceseries_items(self):
+        resp_json = {
+                'requestid': '1',
+                'start': '2023-06-29T00:00:00',
+                'end': '2023-07-05T00:00:00',
+                'resolution': 'P1D',
+                'series': [
+                    {
+                        'times': '2023-06-29/P1D',
+                        'expires': '2023-07-05T17:54:21.7030064+02:00',
+                        'data': [
+                            [0, 130.54, 131.64, 129.93, 130.46],
+                            [1, 131.16, 132.68, 130.42, 132.36],
+                            [4, 132.8, 133.7, 131.62, 132.61],
+                            [5, 132.6, 132.98, 130.96, 131.32],
+                            [6, 131.2, 133.5, 130.88, 132.82]],
+                        'id': 'ohlc:issueid:350118230',
+                        'type': 'ohlc'
+                        }
+                    ]
+                }
+        series = resp_json['series'][0]
+        price_data = degiroasync.api.product.PriceSeries(
+                start=datetime.datetime.fromisoformat(resp_json['start']),
+                end=datetime.datetime.fromisoformat(resp_json['end']),
+                resolution=PRICE.RESOLUTION(resp_json['resolution']),
+                currency='EUR',
+                series=series,
+                )
+        price_dict = dict(price_data.items())
+        self.assertEqual(
+                price_dict['open'],
+                [130.54, 131.16, 132.8, 132.6, 131.2])
+        self.assertEqual(
+                price_dict['date'],
+                [
+                    datetime.datetime(2023, 6, 29),
+                    datetime.datetime(2023, 6, 30),
+                    datetime.datetime(2023, 7, 3),
+                    datetime.datetime(2023, 7, 4),
+                    datetime.datetime(2023, 7, 5),
+                ])
+
+    def test_priceseries_iterrows(self):
+        resp_json = {
+                'requestid': '1',
+                'start': '2023-06-29T00:00:00',
+                'end': '2023-07-05T00:00:00',
+                'resolution': 'P1D',
+                'series': [
+                    {
+                        'times': '2023-06-29/P1D',
+                        'expires': '2023-07-05T17:54:21.7030064+02:00',
+                        'data': [
+                            [0, 130.54, 131.64, 129.93, 130.46],
+                            [1, 131.16, 132.68, 130.42, 132.36],
+                            [4, 132.8, 133.7, 131.62, 132.61],
+                            [5, 132.6, 132.98, 130.96, 131.32],
+                            [6, 131.2, 133.5, 130.88, 132.82]],
+                        'id': 'ohlc:issueid:350118230',
+                        'type': 'ohlc'
+                        }
+                    ]
+                }
+        series = resp_json['series'][0]
+        price_data = degiroasync.api.product.PriceSeries(
+                start=datetime.datetime.fromisoformat(resp_json['start']),
+                end=datetime.datetime.fromisoformat(resp_json['end']),
+                resolution=PRICE.RESOLUTION(resp_json['resolution']),
+                currency='EUR',
+                series=series,
+                )
+
+        data = series['data']
+        for ind, row in enumerate(price_data.iterrows()):
+            self.assertEqual(row['open'], data[ind][1])
+            self.assertEqual(row['high'], data[ind][2])
+            self.assertEqual(row['low'], data[ind][3])
+            self.assertEqual(row['close'], data[ind][4])
+
+        self.assertEqual(ind, 4)
+
+    def test_priceseries_pandas(self):
+        resp_json = {
+                'requestid': '1',
+                'start': '2023-06-29T00:00:00',
+                'end': '2023-07-05T00:00:00',
+                'resolution': 'P1D',
+                'series': [
+                    {
+                        'times': '2023-06-29/P1D',
+                        'expires': '2023-07-05T17:54:21.7030064+02:00',
+                        'data': [
+                            [0, 130.54, 131.64, 129.93, 130.46],
+                            [1, 131.16, 132.68, 130.42, 132.36],
+                            [4, 132.8, 133.7, 131.62, 132.61],
+                            [5, 132.6, 132.98, 130.96, 131.32],
+                            [6, 131.2, 133.5, 130.88, 132.82]],
+                        'id': 'ohlc:issueid:350118230',
+                        'type': 'ohlc'
+                        }
+                    ]
+                }
+        series = resp_json['series'][0]
+        price_data = degiroasync.api.product.PriceSeries(
+                start=datetime.datetime.fromisoformat(resp_json['start']),
+                end=datetime.datetime.fromisoformat(resp_json['end']),
+                resolution=PRICE.RESOLUTION(resp_json['resolution']),
+                currency='EUR',
+                series=series,
+                )
+
+        import pandas as pd
+        df = pd.DataFrame(price_data.iterrows())
+        self.assertEqual(df['open'][0], 130.54)
+        self.assertEqual(df['open'][2], 132.8)
+        self.assertEqual(df['close'][4], 132.82)
+
+    @unittest.mock.patch('degiroasync.webapi.get_price_series')
+    async def test_get_price_series_ohlc(self, price_m):
+        resp_json = {
+                'requestid': '1',
+                'start': '2023-06-29T00:00:00',
+                'end': '2023-07-05T00:00:00',
+                'resolution': 'P1D',
+                'series': [
+                    {
+                        'times': '2023-06-29/P1D',
+                        'expires': '2023-07-05T17:54:21.7030064+02:00',
+                        'data': [
+                            [0, 130.54, 131.64, 129.93, 130.46],
+                            [1, 131.16, 132.68, 130.42, 132.36],
+                            [4, 132.8, 133.7, 131.62, 132.61],
+                            [5, 132.6, 132.98, 130.96, 131.32],
+                            [6, 131.2, 133.5, 130.88, 132.82]],
+                        'id': 'ohlc:issueid:350118230',
+                        'type': 'ohlc'
+                        },
+                    {
+                        'type': 'object',
+                        'data': {'currency': 'EUR'}
+                    }
+                    ]
+                }
+        price_m.return_value = resp_json
+        product = MagicMock()
+        product.info = MagicMock()
+        product.info.product_type_id = PRODUCT.TYPEID.STOCK
+
+        ohlc_series = await degiroasync.api.get_price_series(
+                None,
+                product,
+                None,
+                None,
+                None,
+                None,
+                None
+                )
+        data = resp_json['series'][0]['data']
+        for ind, row in enumerate(ohlc_series.iterrows()):
+            self.assertEqual(row['open'], data[ind][1])
+            self.assertEqual(row['high'], data[ind][2])
+            self.assertEqual(row['low'], data[ind][3])
+            self.assertEqual(row['close'], data[ind][4])
+
+
 #####################
 # Integration tests #
 #####################
 if RUN_INTEGRATION_TESTS:
     LOGGER.info('degiroasync.api integration tests will run.')
 
     class TestDegiroasyncIntegrationLogin(
@@ -426,126 +581,135 @@
                 self.assertIsInstance(product.info.isin, str,
                                       f"{product.base.id}:{product.info.name}")
 
     class TestDegiroasyncIntegrationPrice(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
 
-        async def test_get_price_data(self):
+        async def test_get_price_series(self):
             session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_isin='NL0000235190',
                     product_type_id=PRODUCT.TYPEID.STOCK
                     )
-            #products_awaitable = [p.await_product_info() for p in products]
-            #LOGGER.debug('test_get_price_data products_awaitable| %s', products_awaitable)
 
             # In a context where we'd want to optimize, we want to
             # build the pipeline by awaiting on each product instead of a bulk
             # gather to not block execution while we wait for data on some
             # of the products.
-            #await asyncio.gather(*[p.await_product_info() for p in products])
-            #products = [p async for p in products_gen]
             self.assertGreaterEqual(len(products), 1, products)
 
-            LOGGER.debug('test_get_price_data products| %s',
+            LOGGER.debug('test_get_price_series products| %s',
                          tuple(p.__dict__ for p in products))
 
             products = filter(
                     lambda p: (
                         p.info.product_type == PRODUCT.TYPE.STOCK
                         and p.info.tradable is True
                         and p.info.symbol == 'AIR'
                         ),
                     products)
             products = list(products)
-            LOGGER.debug('test_get_price_data products filtered| %s',
+            LOGGER.debug('test_get_price_series products filtered| %s',
                          pprint.pformat(tuple(p.__dict__ for p in products)))
 
             self.assertGreaterEqual(len(products), 1)
             # Select product
             for product in products:
                 if product.base.product_type_id == PRODUCT.TYPEID.STOCK:
                     # Let's take the first stock as example
                     break
 
-            LOGGER.debug('test_get_price_data price_data 1| %s',
+            LOGGER.debug('test_get_price_series price_data 1| %s',
                          product.__dict__)
-            price_data = await degiroasync.api.get_price_data(session, product)
-            LOGGER.debug('test_get_price_data price_data 2| %s',
+            price_data = await degiroasync.api.get_price_series(session, product)
+            LOGGER.debug('test_get_price_series price_data 2| %s',
                          price_data)
             self.assertGreaterEqual(len(price_data.price), 1)
             self.assertGreaterEqual(len(price_data.date), 1)
 
-        async def test_get_price_data_symbol_exchange(self):
+            price_data = await degiroasync.api.get_price_series(
+                    session,
+                    product,
+                    period=PRICE.PERIOD.P1WEEK,
+                    resolution=PRICE.RESOLUTION.PT1D,
+                    data_type=PRICE.TYPE.OHLC)
+            LOGGER.debug('test_get_price_series price_data ohlc 3| %s',
+                         price_data)
+            self.assertGreaterEqual(len(price_data.price), 1)
+            self.assertEqual(len(price_data.price[0]), 4)
+            self.assertGreaterEqual(
+                    len(price_data.date),
+                    len(price_data.price))
+
+        async def test_get_price_series_symbol_exchange(self):
             # First get product
             session = await _IntegrationLogin._login()
             symbol = 'FGR'
             exchange = 'EPA'
             products = await degiroasync.api.search_product(
                     session,
                     by_symbol=symbol,
                     by_exchange=exchange,
                     product_type_id=PRODUCT.TYPEID.STOCK)
             self.assertEqual(len(products), 1)
             product = products[0]
             self.assertEqual(symbol, product.info.symbol, product.info)
 
-            price_data = await degiroasync.api.get_price_data(session, product)
-            LOGGER.debug("test_get_price_data| %s", price_data.price)
-            LOGGER.debug("test_get_price_data| %s", price_data.date)
+            price_data = await degiroasync.api.get_price_series(session, product)
+            LOGGER.debug("test_get_price_series| %s", price_data.price)
+            LOGGER.debug("test_get_price_series| %s", price_data.date)
             self.assertGreaterEqual(len(price_data.price), 1)
             self.assertGreaterEqual(len(price_data.date), 1)
 
             date = price_data.date
             price = price_data.price
             self.assertEqual(len(date), len(price))
 
-        async def test_get_price_data_day_resolution(self):
+        async def test_get_price_series_day_resolution(self):
             session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_isin='NL0000235190',
                     by_exchange='EPA',
                     product_type_id=PRODUCT.TYPEID.STOCK
                     )
-            LOGGER.debug('test_get_price_data_day_resolution| products %s',
+            LOGGER.debug('test_get_price_series_day_resolution| products %s',
                          pprint.pformat([p.__dict__ for p in products]))
-            #LOGGER.debug('test_get_price_data products_awaitable| %s', products_awaitable)
 
             # In a context where we'd want to optimize, we want to
             # build the pipeline by awaiting on each product instead of a bulk
             # gather to not block execution while we wait for data on some
             # of the products.
             #await asyncio.gather(*[p.await_product_info() for p in products])
             #products = [p async for p in products_gen]
             self.assertEqual(len(products), 1)
             product = products[0]
 
-            LOGGER.debug('test_get_price_data_day_resolution| product %s',
+            LOGGER.debug('test_get_price_series_day_resolution| product %s',
                          pprint.pformat(product.__dict__))
 
             self.assertEqual(product.info.product_type_id,
                              PRODUCT.TYPEID.STOCK)
 
-            price_data = await degiroasync.api.get_price_data(
+            price_data = await degiroasync.api.get_price_series(
                     session,
                     product,
                     resolution=PRICE.RESOLUTION.PT1D,
                     period=PRICE.PERIOD.P1MONTH,
                     )
-            LOGGER.debug('test_get_price_data_day_resolution| price_data %s',
+            LOGGER.debug('test_get_price_series_day_resolution| price_data %s',
                          price_data)
             self.assertGreaterEqual(len(price_data.price), 1)
             self.assertGreaterEqual(len(price_data.date), 1)
             date_series = price_data.date
             price_series = price_data.price
             self.assertEqual(len(date_series), len(price_series))
-            LOGGER.debug("test_get_price_data_day_resolution| "
+            LOGGER.debug("test_get_price_series_day_resolution| "
                          "date_series len %s", len(date_series))
             self.assertGreaterEqual(
                     len(date_series), 15,
                     "We should have daily data for a month with one sample "
                     "per day.")
 
             # We entered PT1D resolution, check that we have one data point
@@ -712,10 +876,11 @@
 if __name__ == '__main__':
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     formatter = logging.Formatter(
             "%(asctime)s-%(name)s-%(levelname)s-%(message)",
             "%Y%m%d"
             )
-    LOGGER.addHandler(handler)
+    if handler not in LOGGER.handlers:
+        LOGGER.addHandler(handler)
     LOGGER.setLevel(logging.DEBUG)
     unittest.main()
```

### Comparing `degiroasync-0.17.0/tests/test_degirowebapi.py` & `degiroasync-0.18.0/tests/test_degirowebapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,60 +177,82 @@
             session = await _IntegrationLogin._login()
 
             isin = "NL0000235190"
             resp_json = await get_news_by_company(session, isin)
             self.assertTrue('data' in resp_json, resp_json)
             self.assertTrue('items' in resp_json['data'], resp_json)
 
-        async def test_get_price_data(self):
+        async def test_get_price_series(self):
             """
             Simply check that we don't have an error and data is not empty.
             """
             session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
-            resp_json = await degiroasync.webapi.get_price_data(
+            resp_json = await degiroasync.webapi.get_price_series(
                     session,
                     vwdId=vwdId,
                     vwdIdentifierType='issueid')
-            LOGGER.debug('get_price_data response: %s', resp_json)
+            LOGGER.debug('get_price_series response: %s', resp_json)
             LOGGER.debug(resp_json)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
-        async def test_get_price_data_month(self):
+        async def test_get_price_series_month(self):
             session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
-            resp_json = await degiroasync.webapi.get_price_data(
+            resp_json = await degiroasync.webapi.get_price_series(
                     session,
                     vwdId=vwdId,
                     period=PRICE.PERIOD.P1MONTH,
                     resolution=PRICE.RESOLUTION.PT1M,
                     vwdIdentifierType='issueid')
             LOGGER.debug(resp_json)
             self.assertIn('resolution', resp_json)
             self.assertEqual(resp_json['resolution'], PRICE.RESOLUTION.PT1M)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
-        async def test_get_price_data_month_pt1d(self):
+        async def test_get_price_series_ohlc(self):
             session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
-            resp_json = await degiroasync.webapi.get_price_data(
+            resp_json = await degiroasync.webapi.get_price_series(
+                    session,
+                    vwdId=vwdId,
+                    period=PRICE.PERIOD.P1MONTH,
+                    resolution=PRICE.RESOLUTION.PT1M,
+                    vwdIdentifierType='issueid',
+                    data_type=PRICE.TYPE.OHLC,
+                    )
+            LOGGER.debug(resp_json)
+            self.assertIn('resolution', resp_json)
+            self.assertEqual(resp_json['resolution'], PRICE.RESOLUTION.PT1M)
+            self.assertIn('series', resp_json)
+            self.assertIn('data', resp_json['series'][0])
+            self.assertEqual(
+                    len(resp_json['series'][0]['data'][0]), 5,
+                    "We should have 5 entries per row (index + O H L C)")
+
+        async def test_get_price_series_month_pt1d(self):
+            session = await _IntegrationLogin._login()
+
+            vwdId = '360114899'
+
+            resp_json = await degiroasync.webapi.get_price_series(
                     session,
                     vwdId=vwdId,
                     period=PRICE.PERIOD.P1MONTH,
                     resolution=PRICE.RESOLUTION.PT1D,
                     vwdIdentifierType='issueid')
-            LOGGER.debug('get_price_data_month_pt1d| response: %s',
+            LOGGER.debug('get_price_series_month_pt1d| response: %s',
                          resp_json)
             LOGGER.debug(resp_json)
             self.assertIn('resolution', resp_json)
             self.assertEqual(resp_json['resolution'], PRICE.RESOLUTION.PT1D)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
@@ -431,10 +453,11 @@
 if __name__ == '__main__':
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     formatter = logging.Formatter(
             "%(asctime)s-%(name)s-%(levelname)s-%(message)",
             "%Y%m%d"
             )
-    LOGGER.addHandler(handler)
+    if handler not in LOGGER.handlers:
+        LOGGER.addHandler(handler)
     LOGGER.setLevel(logging.DEBUG)
     unittest.main()
```

