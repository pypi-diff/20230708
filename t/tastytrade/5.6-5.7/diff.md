# Comparing `tmp/tastytrade-5.6.tar.gz` & `tmp/tastytrade-5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.6.tar", last modified: Thu Jun 22 14:59:41 2023, max compression
+gzip compressed data, was "tastytrade-5.7.tar", last modified: Sat Jul  8 03:39:01 2023, max compression
```

## Comparing `tastytrade-5.6.tar` & `tastytrade-5.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.991850 tastytrade-5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 14:59:29.000000 tastytrade-5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-22 14:59:41.991850 tastytrade-5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-06-22 14:59:29.000000 tastytrade-5.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:59:41.991850 tastytrade-5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 14:59:29.000000 tastytrade-5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.987849 tastytrade-5.6/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.991850 tastytrade-5.6/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-22 14:59:29.000000 tastytrade-5.6/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:59:41.987849 tastytrade-5.6/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 14:59:41.000000 tastytrade-5.6/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 03:38:47.000000 tastytrade-5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-08 03:39:01.782328 tastytrade-5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-08 03:38:47.000000 tastytrade-5.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 03:39:01.782328 tastytrade-5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-08 03:38:47.000000 tastytrade-5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.778328 tastytrade-5.7/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.6/LICENSE` & `tastytrade-5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.6/PKG-INFO` & `tastytrade-5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.6
+Version: 5.7
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.6/README.rst` & `tastytrade-5.7/README.rst`

 * *Files identical despite different names*

### Comparing `tastytrade-5.6/setup.py` & `tastytrade-5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,13 @@
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
     install_requires=[
         'requests<3',
-        'dataclasses',
         'websockets>=11.0.3',
-        'pydantic>=1.10.7'
+        'pydantic<2'
     ],
     packages=find_packages(exclude=['ez_setup', 'tests*']),
     include_package_data=True
 )
```

### Comparing `tastytrade-5.6/tastytrade/account.py` & `tastytrade-5.7/tastytrade/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
     bond_margin_requirement: Decimal
     snapshot_date: date
     reg_t_margin_requirement: Decimal
     futures_overnight_margin_requirement: Decimal
     futures_intraday_margin_requirement: Decimal
     maintenance_excess: Decimal
     pending_margin_interest: Decimal
-    apex_starting_day_margin_equity: Decimal
-    buying_power_adjustment: Decimal
-    buying_power_adjustment_effect: PriceEffect
     effective_cryptocurrency_buying_power: Decimal
     updated_at: datetime
+    apex_starting_day_margin_equity: Optional[Decimal] = None
+    buying_power_adjustment: Optional[Decimal] = None
+    buying_power_adjustment_effect: Optional[PriceEffect] = None
     time_of_day: Optional[str] = None
 
 
 class AccountBalanceSnapshot(TastytradeJsonDataclass):
     """
     Dataclass containing account balance for a moment in time (snapshot).
     """
@@ -109,15 +109,16 @@
     equity_offering_margin_requirement: Optional[Decimal] = None
     long_bond_value: Optional[Decimal] = None
     bond_margin_requirement: Optional[Decimal] = None
 
 
 class CurrentPosition(TastytradeJsonDataclass):
     """
-    Dataclass containing imformation about an individual position in a portfolio.
+    Dataclass containing imformation about an individual position in a
+    portfolio.
     """
     account_number: str
     symbol: str
     instrument_type: InstrumentType
     underlying_symbol: str
     quantity: Decimal
     quantity_direction: str
@@ -387,15 +388,19 @@
     investment_time_horizon: Optional[str] = None
     futures_account_purpose: Optional[str] = None
     external_fdid: Optional[str] = None
     suitable_options_level: Optional[str] = None
     submitting_user_id: Optional[str] = None
 
     @classmethod
-    def get_accounts(cls, session: Session, include_closed=False) -> list['Account']:
+    def get_accounts(
+        cls,
+        session: Session,
+        include_closed=False
+    ) -> list['Account']:
         """
         Gets all trading accounts from the Tastyworks platform. By default
         excludes closed accounts from the results.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Account` objects.
@@ -441,15 +446,15 @@
         Get the trading status of the account.
 
         :param session: the session to use for the request.
 
         :return: a Tastytrade 'TradingStatus' object in JSON format.
         """
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/trading-status',
+            f'{session.base_url}/accounts/{self.account_number}/trading-status',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)  # throws exception if not 200
 
         data = response.json()['data']
 
         return TradingStatus(**data)
@@ -473,33 +478,36 @@
     def get_balance_snapshots(
         self,
         session: Session,
         snapshot_date: Optional[date] = None,
         time_of_day: Optional[str] = None
     ) -> list[AccountBalanceSnapshot]:
         """
-        Returns a list of two balance snapshots. The first one is the specified date,
-        or, if not provided, the oldest snapshot available. The second one is the most
-        recent snapshot.
+        Returns a list of two balance snapshots. The first one is the
+        specified date, or, if not provided, the oldest snapshot available.
+        The second one is the most recent snapshot.
 
-        If you provide the snapshot date, you must also provide the time of day.
+        If you provide the snapshot date, you must also provide the time of
+        day.
 
         :param session: the session to use for the request.
         :param snapshot_date: the date of the snapshot to get.
-        :param time_of_day: the time of day of the snapshot to get, either 'EOD' or 'BOD'.
+        :param time_of_day:
+            the time of day of the snapshot to get, either 'EOD' or 'BOD'.
 
-        :return: a list of two Tastytrade 'AccountBalanceSnapshot' objects in JSON format.
+        :return:
+            a list of two Tastytrade 'AccountBalanceSnapshot' in JSON format.
         """
         params: dict[str, Any] = {
             'snapshot-date': snapshot_date,
             'time-of-day': time_of_day
         }
 
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/balance-snapshots',
+            f'{session.base_url}/accounts/{self.account_number}/balance-snapshots',  # noqa: E501
             headers=session.headers,
             params={k: v for k, v in params.items() if v is not None}
         )
         validate_response(response)  # throws exception if not 200
 
         data = response.json()['data']['items']
 
@@ -517,22 +525,26 @@
         net_positions: bool = False,
         include_marks: bool = False
     ) -> list[CurrentPosition]:
         """
         Get the current positions of the account.
 
         :param session: the session to use for the request.
-        :param underlying_symbols: an array of underlying symbols for positions.
+        :param underlying_symbols:
+            an array of underlying symbols for positions.
         :param symbol: a single symbol.
         :param instrument_type: the type of instrument.
-        :param include_closed: if closed positions should be included in the query.
+        :param include_closed:
+            if closed positions should be included in the query.
         :param underlying_product_code: the underlying future's product code.
         :param partition_keys: account partition keys.
-        :param net_positions: returns net positions grouped by instrument type and symbol.
-        :param include_marks: include current quote mark (note: can decrease performance).
+        :param net_positions:
+            returns net positions grouped by instrument type and symbol.
+        :param include_marks:
+            include current quote mark (note: can decrease performance).
 
         :return: a list of Tastytrade 'CurrentPosition' objects in JSON format.
         """
         params: dict[str, Any] = {
             'underlying-symbol[]': underlying_symbols,
             'symbol': symbol,
             'instrument-type': instrument_type,
@@ -574,31 +586,34 @@
         end_at: Optional[datetime] = None
     ) -> list[Transaction]:
         """
         Get transaction history of the account.
 
         :param session: the session to use for the request.
         :param per_page: the number of results to return per page.
-        :param page_offset: provide a specific page to get; if not provided, get all pages
+        :param page_offset:
+            provide a specific page to get; if not provided, get all pages
         :param sort: the order to sort results in, either 'Desc' or 'Asc'.
         :param type: the type of transaction.
         :param types: a list of transaction types to filter by.
         :param sub_types: an array of transaction subtypes to filter by.
         :param start_date: the start date of transactions to query.
         :param end_date: the end date of transactions to query.
         :param instrument_type: the type of instrument.
         :param symbol: a single symbol.
         :param underlying_symbol: the underlying symbol.
         :param action:
-            the action of the transaction: 'Sell to Open', 'Sell to Close', 'Buy to Open',
-            'Buy to Close', 'Sell' or 'Buy'.
+            the action of the transaction: 'Sell to Open', 'Sell to Close',
+            'Buy to Open', 'Buy to Close', 'Sell' or 'Buy'.
         :param partition_key: account partition key.
         :param futures_symbol: the full TW Future Symbol, e.g. /ESZ9, /NGZ19.
-        :param start_at: datetime start range for filtering transactions in full date-time.
-        :param end_at: datetime end range for filtering transactions in full date-time.
+        :param start_at:
+            datetime start range for filtering transactions in full date-time.
+        :param end_at:
+            datetime end range for filtering transactions in full date-time.
 
         :return: a list of Tastytrade 'Transaction' objects in JSON format.
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
@@ -623,15 +638,15 @@
             'end-at': end_at
         }
 
         # loop through pages and get all transactions
         results = []
         while True:
             response = requests.get(
-                f'{session.base_url}/accounts/{self.account_number}/transactions',
+                f'{session.base_url}/accounts/{self.account_number}/transactions',  # noqa: E501
                 headers=session.headers,
                 params={k: v for k, v in params.items() if v is not None}
             )
             validate_response(response)
 
             json = response.json()
             results.extend(json['data']['items'])
@@ -651,73 +666,82 @@
 
         :param session: the session to use for the request.
         :param id: the ID of the transaction to fetch.
 
         :return: a Tastytrade 'Transaction' object in JSON format.
         """
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/transactions/{id}',
+            f'{session.base_url}/accounts/{self.account_number}/transactions/{id}',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return Transaction(**data)
 
-    def get_total_fees(self, session: Session, date: date = date.today()) -> dict[str, Any]:
+    def get_total_fees(
+        self,
+        session: Session,
+        date: date = date.today()
+    ) -> dict[str, Any]:
         """
         Get the total fees for a given date.
 
         :param session: the session to use for the request.
         :param date: the date to get fees for.
 
         :return: a dict containing the total fees and the price effect.
         """
         params: dict[str, Any] = {'date': date}
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/transactions/total-fees',
+            f'{session.base_url}/accounts/{self.account_number}/transactions/total-fees',  # noqa: E501
             headers=session.headers,
             params=params
         )
         validate_response(response)
 
         return response.json()['data']
 
     def get_net_liquidating_value_history(
         self,
         session: Session,
         time_back: Optional[str] = None,
         start_time: Optional[datetime] = None
     ) -> list[NetLiqOhlc]:
         """
-        Returns a list of account net liquidating value snapshots over the specified time period.
+        Returns a list of account net liquidating value snapshots over the
+        specified time period.
 
         :param session: the session to use for the request.
         :param time_back:
-            the time period to get net liquidating value snapshots for. This param is required
-            if start_time is not given. Possible values are: '1d', '1m', '3m', '6m', '1y', 'all'.
+            the time period to get net liquidating value snapshots for. This
+            param is required if start_time is not given. Possible values are:
+            '1d', '1m', '3m', '6m', '1y', 'all'.
         :param start_time:
-            the start point for the query. This param is required is time-back is not given.
-            If given, will take precedence over time-back.
+            the start point for the query. This param is required is time-back
+            is not given. If given, will take precedence over time-back.
 
         :return: a list of Tastytrade 'NetLiqOhlc' objects in JSON format.
         """
         params: dict[str, Any] = {}
         if start_time:
             # format to Tastytrade DateTime format
-            start_time = str(start_time).replace(' ', 'T').split('.')[0] + 'Z'  # type: ignore
+            start_time = str(start_time) \
+                .replace(' ', 'T') \
+                .split('.')[0] + 'Z'  # type: ignore
             params = {'start-time': start_time}
         elif not time_back:
-            raise TastytradeError('Either time_back or start_time must be specified.')
+            msg = 'Either time_back or start_time must be specified.'
+            raise TastytradeError(msg)
         else:
             params = {'time-back': time_back}
 
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/net-liq/history',
+            f'{session.base_url}/accounts/{self.account_number}/net-liq/history',  # noqa: E501
             headers=session.headers,
             params=params
         )
         validate_response(response)
 
         data = response.json()['data']['items']
 
@@ -728,55 +752,59 @@
         Get the maximum order size information for the account.
 
         :param session: the session to use for the request.
 
         :return: a Tastytrade 'PositionLimit' object in JSON format.
         """
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/position-limit',
+            f'{session.base_url}/accounts/{self.account_number}/position-limit',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return PositionLimit(**data)
 
-    def get_effective_margin_requirements(self, session: Session, symbol: str) -> MarginRequirement:
+    def get_effective_margin_requirements(
+        self,
+        session: Session,
+        symbol: str
+    ) -> MarginRequirement:
         """
         Get the effective margin requirements for a given symbol.
 
         :param session: the session to use for the request.
         :param symbol: the symbol to get margin requirements for.
 
         :return: a :class:`MarginRequirement` object.
         """
         if symbol:
             symbol = symbol.replace('/', '%2F')
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/margin-requirements/{symbol}/effective',
+            f'{session.base_url}/accounts/{self.account_number}/margin-requirements/{symbol}/effective',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return MarginRequirement(**data)
 
     def get_margin_requirements(self, session: Session) -> MarginReport:
         """
-        Get the margin report for the account, with total margin requirements as well
-        as a breakdown per symbol/instrument.
+        Get the margin report for the account, with total margin requirements
+        as well as a breakdown per symbol/instrument.
 
         :param session: the session to use for the request.
 
         :return: a :class:`MarginReport` object.
         """
         response = requests.get(
-            f'{session.base_url}/margin/accounts/{self.account_number}/requirements',
+            f'{session.base_url}/margin/accounts/{self.account_number}/requirements',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return MarginReport(**data)
@@ -804,15 +832,15 @@
         Gets an order with the given ID.
 
         :param session: the session to use for the request.
 
         :return: an :class:`Order` object corresponding to the given ID.
         """
         response = requests.get(
-            f'{session.base_url}/accounts/{self.account_number}/orders/{order_id}',
+            f'{session.base_url}/accounts/{self.account_number}/orders/{order_id}',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return PlacedOrder(**data)
@@ -821,15 +849,15 @@
         """
         Delete an order by ID.
 
         :param session: the session to use for the request.
         :param order_id: the ID of the order to delete.
         """
         response = requests.delete(
-            f'{session.base_url}/accounts/{self.account_number}/orders/{order_id}',
+            f'{session.base_url}/accounts/{self.account_number}/orders/{order_id}',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
     def get_order_history(
         self,
         session: Session,
@@ -846,24 +874,28 @@
         end_at: Optional[datetime] = None
     ) -> list[PlacedOrder]:
         """
         Get order history of the account.
 
         :param session: the session to use for the request.
         :param per_page: the number of results to return per page.
-        :param page_offset: provide a specific page to get; if not provided, get all pages
+        :param page_offset:
+            provide a specific page to get; if not provided, get all pages
         :param start_date: the start date of orders to query.
         :param end_date: the end date of orders to query.
         :param underlying_symbol: underlying symbol to filter by.
         :param statuses: a list of statuses to filter by.
-        :param futures_symbol: Tastytrade future symbol for futures and future options.
-        :param underlying_instrument_type: the type of instrument to filter by.
+        :param futures_symbol:
+            Tastytrade future symbol for futures and future options.
+        :param underlying_instrument_type: the type of instrument to filter by
         :param sort: the order to sort results in, either 'Desc' or 'Asc'.
-        :param start_at: datetime start range for filtering transactions in full date-time.
-        :param end_at: datetime end range for filtering transactions in full date-time.
+        :param start_at:
+            datetime start range for filtering transactions in full date-time.
+        :param end_at:
+            datetime end range for filtering transactions in full date-time.
 
         :return: a list of Tastytrade 'Transaction' objects in JSON format.
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
@@ -901,15 +933,20 @@
                 break
             if not paginate:
                 break
             params['page-offset'] += 1  # type: ignore
 
         return [PlacedOrder(**entry) for entry in results]
 
-    def place_order(self, session: Session, order: NewOrder, dry_run=True) -> PlacedOrderResponse:
+    def place_order(
+        self,
+        session: Session,
+        order: NewOrder,
+        dry_run=True
+    ) -> PlacedOrderResponse:
         """
         Place the given order.
 
         :param session: the session to use for the request.
         :param order: the order to place.
         :param dry_run: whether this is a test order or not.
 
@@ -926,30 +963,40 @@
         response = requests.post(url, headers=session.headers, data=json)
         validate_response(response)
 
         data = response.json()['data']
 
         return PlacedOrderResponse(**data)
 
-    def replace_order(self, session: Session, old_order_id: str, new_order: NewOrder) -> PlacedOrder:
+    def replace_order(
+        self,
+        session: Session,
+        old_order_id: str,
+        new_order: NewOrder
+    ) -> PlacedOrder:
         """
-        Replace an order with a new order with different characteristics (but same legs).
+        Replace an order with a new order with different characteristics (but
+        same legs).
 
         :param session: the session to use for the request.
         :param old_order_id: the ID of the order to replace.
         :param new_order: the new order to replace the old order with.
 
         :return: a :class:`PlacedOrder` object for the modified order.
         """
         headers = session.headers
         # required because we're passing the JSON as a string
         headers['Content-Type'] = 'application/json'
         response = requests.put(
-            f'{session.base_url}/accounts/{self.account_number}/orders/{old_order_id}',
+            f'{session.base_url}/accounts/{self.account_number}/orders/{old_order_id}',  # noqa: E501
             headers=headers,
-            data=new_order.json(exclude={'legs'}, exclude_none=True, by_alias=True)
+            data=new_order.json(
+                exclude={'legs'},
+                exclude_none=True,
+                by_alias=True
+            )
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return PlacedOrder(**data)
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/candle.py` & `tastytrade-5.7/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.6/tastytrade/dxfeed/greeks.py` & `tastytrade-5.7/tastytrade/dxfeed/greeks.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
 from .event import Event
 
 
 @dataclass
 class Greeks(Event):
     """
-    Greek ratios, or simply Greeks, are differential values that show how the price of an option depends on other market parameters: on the price of the underlying asset, its volatility, etc. Greeks are used to assess the risks of customer portfolios. Greeks are derivatives of the value of securities in different axes. If a derivative is very far from zero, then the portfolio has a risky sensitivity in this parameter.
+    Greek ratios, or simply Greeks, are differential values that show how the
+    price of an option depends on other market parameters: on the price of the
+    underlying asset, its volatility, etc. Greeks are used to assess the risks
+    of customer portfolios. Greeks are derivatives of the value of securities
+    in different axes. If a derivative is very far from zero, then the
+    portfolio has a risky sensitivity in this parameter.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: transactional event flags
     eventFlags: int
     #: unique per-symbol index of this event
     index: int
     #: timestamp of this event in milliseconds
     time: int
-    #: sequence number of thie event to distinguish events that have the same time
+    #: sequence number to distinguish events that have the same time
     sequence: int
     #: option market price
     price: float
     #: Black-Scholes implied volatility of the option
     volatility: float
     #: option delta
     delta: float
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/profile.py` & `tastytrade-5.7/tastytrade/dxfeed/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from .event import Event
 
 
 @dataclass
 class Profile(Event):
     """
-    A Profile event provides the security instrument description. It represents the most recent information that is available about the traded security on the market at any given moment of time.
+    A Profile event provides the security instrument description. It
+    represents the most recent information that is available about the
+    traded security on the market at any given moment of time.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: description of the security instrument
     description: str
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/quote.py` & `tastytrade-5.7/tastytrade/dxfeed/quote.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from .event import Event
 
 
 @dataclass
 class Quote(Event):
     """
-    A Quote event is a snapshot of the best bid and ask prices, and other fields that change with each quote.
+    A Quote event is a snapshot of the best bid and ask prices, and other
+    fields that change with each quote.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: sequence of this quote
     sequence: int
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/summary.py` & `tastytrade-5.7/tastytrade/dxfeed/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from .event import Event
 
 
 @dataclass
 class Summary(Event):
     """
-    Summary is an information snapshot about the trading session including session highs, lows, etc. This record has two goals:
+    Summary is an information snapshot about the trading session including
+    session highs, lows, etc. This record has two goals:
 
     1. Transmit OHLC values.
-
-    2. Provide data for charting. OHLC is required for a daily chart, and if an exchange does not provide it, the charting services refer to the Summary event.
+    2. Provide data for charting. OHLC is required for a daily chart, and
+    if an exchange does not provide it, the charting services refer to the
+    Summary event.
 
     Before opening the bidding, the values are reset to N/A or NaN.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.7/tastytrade/dxfeed/theoprice.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 from .event import Event
 
 
 @dataclass
 class TheoPrice(Event):
     """
-    Theo price is a snapshot of the theoretical option price computation that is periodically performed by dxPrice model-free computation. dxFeed does not send recalculations for all options at the same time, so we provide you with a formula so you can perform calculations based on values from this event.
+    Theo price is a snapshot of the theoretical option price computation that
+    is periodically performed by dxPrice model-free computation. dxFeed does
+    not send recalculations for all options at the same time, so we provide
+    you with a formula so you can perform calculations based on values from
+    this event.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: transactional event flags
     eventFlags: int
     #: unique per-symbol index of this event
     index: int
     #: timestamp of this event in milliseconds
     time: int
-    #: sequence number of this event to distinguish events that have the same time
+    #: sequence number to distinguish events that have the same time
     sequence: int
     #: theoretical price
     price: float
     #: underlying price at the time of theo price computation
     underlyingPrice: float
     #: delta of the theoretical price
     delta: float
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/timeandsale.py` & `tastytrade-5.7/tastytrade/dxfeed/timeandsale.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from .event import Event
 
 
 @dataclass
 class TimeAndSale(Event):
     """
-    TimeAndSale event represents a trade or other market event with a price, like
-    market open/close price. TimeAndSale events are intended to provide information
-    about trades in a continuous-time slice (unlike Trade events which are supposed
-    to provide snapshots about the most recent trade). TimeAndSale events have a
-    unique index that can be used for later correction/cancellation processing.
+    TimeAndSale event represents a trade or other market event with a price,
+    like market open/close price. TimeAndSale events are intended to provide
+    information about trades in a continuous-time slice (unlike Trade events
+    which are supposed to provide snapshots about the most recent trade).
+    TimeAndSale events have a unique index that can be used for later
+    correction/cancellation processing.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: transactional event flags
     eventFlags: int
@@ -28,17 +29,17 @@
     sequence: int
     #: exchange code of this time and sale event
     exchangeCode: str
     #: price of this time and sale event
     price: float
     #: size of this time and sale event as integer number (rounded toward zero)
     size: int
-    #: the current bid price on the market when this time and sale event had occured
+    #: the bid price on the market when this time and sale event occured
     bidPrice: float
-    #: the current ask price on the market when this time and sale event had occured
+    #: the ask price on the market when this time and sale event occured
     askPrice: float
     #: sale conditions provided for this event by data feed
     exchangeSaleConditions: str
     #: transaction is concluded by exempting from compliance with some rule
     tradeThroughExempt: str
     #: initiator of the trade
     aggressorSide: str
```

### Comparing `tastytrade-5.6/tastytrade/dxfeed/trade.py` & `tastytrade-5.7/tastytrade/dxfeed/trade.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 from .event import Event
 
 
 @dataclass
 class Trade(Event):
     """
-    A Trade event provides prices and the volume of the last transaction in regular trading hours, as well as the total amount per day in the number of securities and in their value. This event does not contain information about all transactions, but only about the last transaction for a single instrument.
+    A Trade event provides prices and the volume of the last transaction in
+    regular trading hours, as well as the total amount per day in the number
+    of securities and in their value. This event does not contain information
+    about all transactions, but only about the last transaction for a single
+    instrument.
     """
     #: symbol of this event
     eventSymbol: str
     #: time of this event
     eventTime: int
     #: time of the last trade
     time: int
```

### Comparing `tastytrade-5.6/tastytrade/instruments.py` & `tastytrade-5.7/tastytrade/instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from tastytrade.order import InstrumentType, TradeableTastytradeJsonDataclass
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
 
 class OptionType(str, Enum):
     """
-    This is an :class:`~enum.Enum` that contains the valid types of options and
-    their abbreviations in the API.
+    This is an :class:`~enum.Enum` that contains the valid types of options
+    and their abbreviations in the API.
     """
     CALL = 'C'
     PUT = 'P'
 
 
 class FutureMonthCode(str, Enum):
     """
-    This is an :class:`~enum.Enum` that contains the valid month codes for futures.
+    This is an :class:`~enum.Enum` that contains the valid month codes for
+    futures.
 
-    This is really just here for reference, as the API barely uses these codes.
+    This is really here for reference, as the API barely uses these codes.
     """
     JAN = 'F'
     FEB = 'G'
     MAR = 'H'
     APR = 'J'
     MAY = 'K'
     JUN = 'M'
@@ -51,38 +52,40 @@
     symbol: str
     instrument_type: InstrumentType
     percent: str
 
 
 class DestinationVenueSymbol(TastytradeJsonDataclass):
     """
-    Dataclass representing a specific destination venue symbol for a cryptocurrency.
+    Dataclass representing a specific destination venue symbol for a
+    cryptocurrency.
     """
     id: int
     symbol: str
     destination_venue: str
     routable: bool
     max_quantity_precision: Optional[int] = None
     max_price_precision: Optional[int] = None
 
 
 class QuantityDecimalPrecision(TastytradeJsonDataclass):
     """
-    Dataclass representing the decimal precision (number of places) for an instrument.
+    Dataclass representing the decimal precision (number of places) for an
+    instrument.
     """
     instrument_type: InstrumentType
     value: int
     minimum_increment_precision: int
     symbol: Optional[str] = None
 
 
 class Strike(TastytradeJsonDataclass):
     """
-    Dataclass representing a specific strike in an options chain, containing the
-    symbols for the call and put options.
+    Dataclass representing a specific strike in an options chain, containing
+    the symbols for the call and put options.
     """
     strike_price: Decimal
     call: str
     put: str
 
 
 class TickSize(TastytradeJsonDataclass):
@@ -125,15 +128,16 @@
     settlement_type: str
     strikes: list[Strike]
     tick_sizes: list[TickSize]
 
 
 class NestedFutureOptionFuture(TastytradeJsonDataclass):
     """
-    Dataclass representing an underlying future in a nested future options chain.
+    Dataclass representing an underlying future in a nested future options
+    chain.
     """
     root_symbol: str
     days_to_expiration: int
     expiration_date: date
     expires_at: datetime
     next_active_month: bool
     symbol: str
@@ -178,35 +182,39 @@
     streamer_symbol: Optional[str] = None
 
     @classmethod
     def get_cryptocurrencies(
         cls, session: Session, symbols: list[str] = []
     ) -> list['Cryptocurrency']:
         """
-        Returns a list of :class:`Cryptocurrency` objects from the given symbols.
+        Returns a list of cryptocurrency objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: the symbols to get the cryptocurrencies for.
 
-        :return: a list of :class:`Cryptocurrency` objects.
+        :return: a list of cryptocurrency objects.
         """
         params = {'symbol[]': symbols} if symbols else None
         response = requests.get(
             f'{session.base_url}/instruments/cryptocurrencies',
             headers=session.headers,
             params=params
         )
         validate_response(response)
 
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
-    def get_cryptocurrency(cls, session: Session, symbol: str) -> 'Cryptocurrency':
+    def get_cryptocurrency(
+        cls,
+        session: Session,
+        symbol: str
+    ) -> 'Cryptocurrency':
         """
         Returns a :class:`Cryptocurrency` object from the given symbol.
 
         :param session: the session to use for the request.
         :param symbol: the symbol to get the cryptocurrency for.
 
         :return: a :class:`Cryptocurrency` object.
@@ -258,16 +266,19 @@
         lendability: Optional[str] = None
     ) -> list['Equity']:
         """
         Returns a list of actively traded :class:`Equity` objects.
 
         :param session: the session to use for the request.
         :param per_page: the number of equities to get per page.
-        :param page_offset: provide a specific page to get; if not provided, get all pages
-        :param lendability: the lendability of the equities; 'Easy To Borrow', 'Locate Required', 'Preborrow'
+        :param page_offset:
+            provide a specific page to get; if not provided, get all pages
+        :param lendability:
+            the lendability of the equities; e.g. 'Easy To Borrow',
+            'Locate Required', 'Preborrow'
 
         :return: a list of :class:`Equity` objects.
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
@@ -313,15 +324,16 @@
     ) -> list['Equity']:
         """
         Returns a list of :class:`Equity` objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: the symbols to get the equities for.
         :param lendability:
-            the lendability of the equities; 'Easy To Borrow', 'Locate Required', 'Preborrow'
+            the lendability of the equities; e.g. 'Easy To Borrow',
+            'Locate Required', 'Preborrow'
         :param is_index: whether the equities are indexes.
         :param is_etf: whether the equities are ETFs.
 
         :return: a list of :class:`Equity` objects.
         """
         params: dict[str, Any] = {
             'symbol[]': symbols,
@@ -466,20 +478,21 @@
         exp = self.expiration_date.strftime('%y%m%d')
         self.streamer_symbol = \
             f".{self.underlying_symbol}{exp}{self.option_type.value}{strike}"
 
 
 class NestedOptionChain(TastytradeJsonDataclass):
     """
-    Dataclass that represents a Tastytrade nested option chain object. Contains
-    information about the option chain and a method to fetch one for a symbol.
-
-    The nested option chain is a bit neater than calling :meth:`get_option_chain` but
-    if you want to create actual :class:`Option` objects you'll need to make an extra
-    API request or two.
+    Dataclass that represents a Tastytrade nested option chain object.
+    Contains information about the option chain and a method to fetch one for
+    a symbol.
+
+    This is cleaner than calling :meth:`get_option_chain` but if you want to
+    create actual :class:`Option` objects you'll need to make an extra API
+    request or two.
     """
     underlying_symbol: str
     root_symbol: str
     option_chain_type: str
     shares_per_contract: int
     tick_sizes: list[TickSize]
     deliverables: list[Deliverable]
@@ -506,15 +519,16 @@
 
         return cls(**data)
 
 
 class FutureProduct(TastytradeJsonDataclass):
     """
     Dataclass that represents a Tastytrade future product object. Contains
-    information about the future product and a method to fetch one for a symbol.
+    information about the future product and a method to fetch one for a
+    symbol.
 
     Useful for fetching general information about a family of futures, without
     knowing the specific expirations or symbols.
     """
     root_symbol: str
     code: str
     description: str
@@ -575,34 +589,35 @@
         exchange: str = 'CME'
     ) -> 'FutureProduct':
         """
         Returns a :class:`FutureProduct` object from the given symbol.
 
         :param session: the session to use for the request.
         :param code: the product code, e.g. 'ES'
-        :param exchange: the exchange to get the product from: 'CME', 'SMALLS', 'CFE', 'CBOED'
+        :param exchange:
+            the exchange to fetch from: 'CME', 'SMALLS', 'CFE', 'CBOED'
 
         :return: a :class:`FutureProduct` object.
         """
         code = code.replace('/', '')
         response = requests.get(
-            f'{session.base_url}/instruments/future-products/{exchange}/{code}',
+            f'{session.base_url}/instruments/future-products/{exchange}/{code}',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
 
 class Future(TradeableTastytradeJsonDataclass):
     """
-    Dataclass that represents a Tastytrade future object. Contains information about
-    the future and methods to fetch futures for symbol(s).
+    Dataclass that represents a Tastytrade future object. Contains information
+    about the future and methods to fetch futures for symbol(s).
     """
     product_code: str
     tick_size: Decimal
     notional_multiplier: Decimal
     display_factor: Decimal
     last_trade_date: date
     expiration_date: date
@@ -612,19 +627,19 @@
     next_active_month: bool
     is_closing_only: bool
     stops_trading_at: datetime
     expires_at: datetime
     product_group: str
     exchange: str
     streamer_exchange_code: str
-    streamer_symbol: str
     back_month_first_calendar_symbol: bool
-    is_tradeable: bool
-    future_product: 'FutureProduct'
     instrument_type: InstrumentType = InstrumentType.FUTURE
+    streamer_symbol: Optional[str] = None
+    is_tradeable: Optional[bool] = None
+    future_product: Optional['FutureProduct'] = None
     contract_size: Optional[Decimal] = None
     main_fraction: Optional[Decimal] = None
     sub_fraction: Optional[Decimal] = None
     first_notice_date: Optional[date] = None
     roll_target_symbol: Optional[str] = None
     true_underlying_symbol: Optional[str] = None
     future_etf_equivalent: Optional[FutureEtfEquivalent] = None
@@ -636,21 +651,23 @@
     def get_futures(
         cls,
         session: Session,
         symbols: Optional[list[str]] = None,
         product_codes: Optional[list[str]] = None
     ) -> list['Future']:
         """
-        Returns a list of :class:`Future` objects from the given symbols or product codes.
+        Returns a list of :class:`Future` objects from the given symbols
+        or product codes.
 
         :param session: the session to use for the request.
         :param symbols:
-            symbols of the futures, e.g. 'ESZ9'. Leading forward slash is not required.
+            symbols of the futures, e.g. 'ESZ9', '/ESZ9'.
         :param product_codes:
-            the product codes of the futures, e.g. 'ES', '6A'. Ignored if symbols are provided.
+            the product codes of the futures, e.g. 'ES', '6A'. Ignored if
+            symbols are provided.
 
         :return: a list of :class:`Future` objects.
         """
         params: dict[str, Any] = {
             'symbol[]': symbols,
             'product-code[]': product_codes
         }
@@ -685,16 +702,17 @@
         data = response.json()['data']
 
         return cls(**data)
 
 
 class FutureOptionProduct(TastytradeJsonDataclass):
     """
-    Dataclass that represents a Tastytrade future option product object. Contains
-    information about the future option product (deliverable for the future option).
+    Dataclass that represents a Tastytrade future option product object.
+    Contains information about the future option product (deliverable for
+    the future option).
     """
     root_symbol: str
     cash_settled: bool
     code: str
     display_factor: Decimal
     exchange: str
     product_type: str
@@ -746,15 +764,15 @@
         :param code: the root symbol of the future option
         :param exchange: the exchange to get the product from
 
         :return: a :class:`FutureOptionProduct` object.
         """
         root_symbol = root_symbol.replace('/', '')
         response = requests.get(
-            f'{session.base_url}/instruments/future-option-products/{exchange}/{root_symbol}',
+            f'{session.base_url}/instruments/future-option-products/{exchange}/{root_symbol}',  # noqa: E501
             headers=session.headers
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
@@ -808,19 +826,21 @@
         expiration_date: Optional[date] = None,
         option_type: Optional[OptionType] = None,
         strike_price: Optional[Decimal] = None
     ) -> list['FutureOption']:
         """
         Returns a list of :class:`FutureOption` objects from the given symbols.
 
-        NOTE: As far as I can tell, all of the parameters are bugged except for `symbols`.
+        NOTE: As far as I can tell, all of the parameters are bugged except
+        for `symbols`.
 
         :param session: the session to use for the request.
         :param symbols: the Tastytrade symbols to filter by.
-        :param root_symbol: the root symbol to get the future options for, e.g. 'EW3', 'SO'
+        :param root_symbol:
+            the root symbol to get the future options for, e.g. 'EW3', 'SO'
         :param expiration_date: the expiration date for the future options.
         :param option_type: the option type to filter by.
         :param strike_price: the strike price to filter by.
 
         :return: a list of :class:`FutureOption` objects.
         """
         params: dict[str, Any] = {
@@ -879,23 +899,27 @@
 
 
 class NestedFutureOptionChain(TastytradeJsonDataclass):
     """
     Dataclass that represents a Tastytrade nested option chain object. Contains
     information about the option chain and a method to fetch one for a symbol.
 
-    The nested option chain is a bit neater than calling :meth:`get_future_option_chain`
-    but if you want to create actual :class:`FutureOption` objects you'll need to make an
+    This is cleaner than calling :meth:`get_future_option_chain` but if you
+    want to create actual :class:`FutureOption` objects you'll need to make an
     extra API request or two.
     """
     futures: list[NestedFutureOptionFuture]
     option_chains: list[NestedFutureOptionSubchain]
 
     @classmethod
-    def get_chain(cls, session: Session, symbol: str) -> 'NestedFutureOptionChain':
+    def get_chain(
+        cls,
+        session: Session,
+        symbol: str
+    ) -> 'NestedFutureOptionChain':
         """
         Gets the futures option chain for the given symbol in nested format.
 
         :param session: the session to use for the request.
         :param symbol: the symbol to get the option chain for.
 
         :return: a :class:`NestedFutureOptionChain` object.
@@ -972,15 +996,17 @@
         return cls(**data)
 
 
 # fix pydantic forward references
 FutureProduct.update_forward_refs()
 
 
-def get_quantity_decimal_precisions(session: Session) -> list[QuantityDecimalPrecision]:
+def get_quantity_decimal_precisions(
+    session: Session
+) -> list[QuantityDecimalPrecision]:
     """
     Returns a list of :class:`QuantityDecimalPrecision` objects for different
     types of instruments.
 
     :param session: the session to use for the request.
 
     :return: a list of :class:`QuantityDecimalPrecision` objects.
@@ -992,27 +1018,31 @@
     validate_response(response)
 
     data = response.json()['data']['items']
 
     return [QuantityDecimalPrecision(**entry) for entry in data]
 
 
-def get_option_chain(session: Session, symbol: str) -> dict[date, list[Option]]:
+def get_option_chain(
+    session: Session,
+    symbol: str
+) -> dict[date, list[Option]]:
     """
-    Returns a mapping of expiration date to a list of :class:`Option` objects
+    Returns a mapping of expiration date to a list of option objects
     representing the options chain for the given symbol.
 
-    In the case that there are two expiries on the same day (e.g. SPXW and SPX AM
-    options), both will be returned in the same list. If you just want one expiry,
-    you'll need to filter the list yourself, or use ~:class:`NestedOptionChain` instead.
+    In the case that there are two expiries on the same day (e.g. SPXW
+    and SPX AM options), both will be returned in the same list. If you
+    just want one expiry, you'll need to filter the list yourself, or use
+    ~:class:`NestedOptionChain` instead.
 
     :param session: the session to use for the request.
     :param symbol: the symbol to get the option chain for.
 
-    :return: a dict mapping expiration date to a list of :class:`Option` objects.
+    :return: a dict mapping expiration date to a list of options
     """
     symbol = symbol.replace('/', '%2F')
     response = requests.get(
         f'{session.base_url}/option-chains/{symbol}',
         headers=session.headers
     )
     validate_response(response)
@@ -1025,27 +1055,31 @@
             chain[option.expiration_date] = [option]
         else:
             chain[option.expiration_date].append(option)
 
     return chain
 
 
-def get_future_option_chain(session: Session, symbol: str) -> dict[date, list[FutureOption]]:
+def get_future_option_chain(
+    session: Session,
+    symbol: str
+) -> dict[date, list[FutureOption]]:
     """
-    Returns a mapping of expiration date to a list of :class:`FutureOption` objects
-    representing the options chain for the given symbol.
+    Returns a mapping of expiration date to a list of futures options
+    objects representing the options chain for the given symbol.
 
-    In the case that there are two expiries on the same day (e.g. EW and ES options),
-    both will be returned in the same list. If you just want one expiry, you'll need
-    to filter the list yourself, or use ~:class:`NestedFutureOptionChain` instead.
+    In the case that there are two expiries on the same day (e.g. EW
+    and ES options), both will be returned in the same list. If you
+    just want one expiry, you'll need to filter the list yourself, or
+    use ~:class:`NestedFutureOptionChain` instead.
 
     :param session: the session to use for the request.
     :param symbol: the symbol to get the option chain for.
 
-    :return: a dict mapping expiration date to a list of :class:`FutureOption` objects.
+    :return: a dict mapping expiration date to a list of futures options.
     """
     symbol = symbol.replace('/', '')
     response = requests.get(
         f'{session.base_url}/futures-option-chains/{symbol}',
         headers=session.headers
     )
     validate_response(response)
```

### Comparing `tastytrade-5.6/tastytrade/metrics.py` & `tastytrade-5.7/tastytrade/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,17 +60,16 @@
     tos_implied_volatility_index_rank_updated_at: datetime
     implied_volatility_index_rank_source: str
     implied_volatility_percentile: Decimal
     implied_volatility_updated_at: datetime
     liquidity_value: Decimal
     liquidity_rank: Decimal
     liquidity_rating: int
-    created_at: datetime
     updated_at: datetime
-    option_expiration_implied_volatilities: list[OptionExpirationImpliedVolatility]
+    option_expiration_implied_volatilities: list[OptionExpirationImpliedVolatility]  # noqa: E501
     liquidity_running_state: Liquidity
     beta: Decimal
     beta_updated_at: datetime
     corr_spy_3month: Decimal
     dividend_rate_per_share: Decimal
     dividend_yield: Decimal
     listed_market: str
@@ -80,21 +79,25 @@
     implied_volatility_30_day: Decimal
     historical_volatility_30_day: Decimal
     historical_volatility_60_day: Decimal
     historical_volatility_90_day: Decimal
     iv_hv_30_day_difference: Decimal
     price_earnings_ratio: Decimal
     earnings_per_share: Decimal
+    created_at: Optional[datetime] = None
     dividend_ex_date: Optional[date] = None
     dividend_next_date: Optional[date] = None
     dividend_pay_date: Optional[date] = None
     dividend_updated_at: Optional[datetime] = None
 
 
-def get_market_metrics(session: Session, symbols: list[str]) -> list[MarketMetricInfo]:
+def get_market_metrics(
+    session: Session,
+    symbols: list[str]
+) -> list[MarketMetricInfo]:
     """
     Retrieves market metrics for the given symbols.
 
     :param session: active user session to use
     :param symbols: list of symbols to retrieve metrics for
 
     :return: a list of Tastytrade 'MarketMetricInfo' objects in JSON format.
@@ -118,39 +121,61 @@
     :param session: active user session to use
     :param symbol: symbol to retrieve dividend information for
 
     :return: a list of Tastytrade 'DividendInfo' objects in JSON format.
     """
     symbol = symbol.replace('/', '%2F')
     response = requests.get(
-        f'{session.base_url}/market-metrics/historic-corporate-events/dividends/{symbol}',
+        f'{session.base_url}/market-metrics/historic-corporate-events/dividends/{symbol}',  # noqa: E501
         headers=session.headers
     )
     validate_response(response)
 
     data = response.json()['data']['items']
 
     return [DividendInfo(**entry) for entry in data]
 
 
-def get_earnings(session: Session, symbol: str, start_date: date) -> list[EarningsInfo]:
+def get_earnings(
+    session: Session,
+    symbol: str,
+    start_date: date
+) -> list[EarningsInfo]:
     """
     Retrieves earnings information for the given symbol.
 
     :param session: active user session to use
     :param symbol: symbol to retrieve earnings information for
     :param start_date: limits earnings to those on or after the given date
 
     :return: a list of Tastytrade 'EarningsInfo' objects in JSON format.
     """
     symbol = symbol.replace('/', '%2F')
     params: dict[str, Any] = {'start-date': start_date}
     response = requests.get(
-        f'{session.base_url}/market-metrics/historic-corporate-events/earnings-reports/{symbol}',
+        f'{session.base_url}/market-metrics/historic-corporate-events/earnings-reports/{symbol}',  # noqa: E501
         headers=session.headers,
         params=params
     )
     validate_response(response)
 
     data = response.json()['data']['items']
 
     return [EarningsInfo(**entry) for entry in data]
+
+
+def get_risk_free_rate(session: Session) -> Decimal:
+    """
+    Retrieves the current risk-free rate.
+
+    :param session: active user session to use
+
+    :return: the current risk-free rate
+    """
+    response = requests.get(
+        f'{session.base_url}/margin-requirements-public-configuration',
+        headers=session.headers
+    )
+    validate_response(response)
+
+    data = response.json()['data']['risk-free-rate']
+    return Decimal(data)
```

### Comparing `tastytrade-5.6/tastytrade/order.py` & `tastytrade-5.7/tastytrade/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,16 @@
     quantity: str
     quantity_type: str
     quantity_numeric: Decimal
 
 
 class OrderChainLeg(TastytradeJsonDataclass):
     """
-    Dataclass containing information about a single leg in an order from an order chain.
+    Dataclass containing information about a single leg in an order
+    from an order chain.
     """
     symbol: str
     instrument_type: InstrumentType
     action: OrderAction
     fill_quantity: Decimal
     order_quantity: Decimal
 
@@ -405,16 +406,17 @@
     open_entries: list[OrderChainEntry]
     total_cost_per_unit: Optional[Decimal] = None
     total_cost_per_unit_effect: Optional[PriceEffect] = None
 
 
 class OrderChain(TastytradeJsonDataclass):
     """
-    Dataclass containing information about an order chain: a group of orders for a
-    specific underlying, such as total P/L, rolls, current P/L in a symbol, etc.
+    Dataclass containing information about an order chain: a group of orders
+    for a specific underlying, such as total P/L, rolls, current P/L in a
+    symbol, etc.
     """
     id: int
     updated_at: datetime
     created_at: datetime
     account_number: str
     description: str
     underlying_symbol: str
```

### Comparing `tastytrade-5.6/tastytrade/search.py` & `tastytrade-5.7/tastytrade/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     """
     symbol: str
     description: str
 
 
 def symbol_search(session: Session, symbol: str) -> list[SymbolData]:
     """
-    Performs a symbol search using the Tastytrade API and returns a list of symbols that
-    are similar to the given search phrase.
+    Performs a symbol search using the Tastytrade API and returns a
+    list of symbols that are similar to the given search phrase.
 
     :param session: active user session to use
     :param symbol: search phrase
 
     :return: a list of symbols and descriptions that match the search phrase
     """
     symbol = symbol.replace('/', '%2F')
     response = requests.get(
         f'{session.base_url}/symbols/search/{symbol}',
         headers=session.headers
     )
     if response.status_code // 100 != 2:
-        # here it doesn't really make sense to throw an exception; we'll just return nothing
+        # here it doesn't really make sense to throw an exception
         return []
     else:
         data = response.json()['data']['items']
         return [SymbolData(**entry) for entry in data]
```

### Comparing `tastytrade-5.6/tastytrade/session.py` & `tastytrade-5.7/tastytrade/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,77 +4,101 @@
 
 from tastytrade import API_URL, CERT_URL
 from tastytrade.utils import validate_response
 
 
 class Session:
     """
-    Contains a local user login which can then be used to interact with the remote API.
+    Contains a local user login which can then be used to interact with the
+    remote API.
 
     :param login: tastytrade username or email
-    :param password: tastytrade password or a remember token obtained previously
+    :param password:
+        tastytrade password or a remember token obtained previously
     :param remember_me:
-        whether or not to generate a token which can be used to login without a password;
-        appears to be bugged currently.
+        whether or not to create a single-use remember token to use in place
+        of a password; currently appears to be bugged.
     :param two_factor_authentication:
-        if two factor authentication is enabled, this is the code sent to the user's device
+        if two factor authentication is enabled, this is the code sent to the
+        user's device
     :param is_certification: whether or not to use the certification API
     """
-    def __init__(self, login: str, password: str, remember_me: bool = False,
-                 two_factor_authentication: str = '', is_certification: bool = False):
+    def __init__(
+        self,
+        login: str,
+        password: str,
+        remember_me: bool = False,
+        two_factor_authentication: str = '',
+        is_certification: bool = False
+    ):
         body = {
             'login': login,
             'password': password,
             'remember-me': remember_me
         }
         #: The base url to use for API requests
         self.base_url: str = CERT_URL if is_certification else API_URL
         #: Whether or not this session is using the certification API
         self.is_certification: bool = is_certification
 
         if two_factor_authentication:
             headers = {'X-Tastyworks-OTP': two_factor_authentication}
-            response = requests.post(f'{self.base_url}/sessions', json=body, headers=headers)
+            response = requests.post(
+                f'{self.base_url}/sessions',
+                json=body,
+                headers=headers
+            )
         else:
             response = requests.post(f'{self.base_url}/sessions', json=body)
         validate_response(response)  # throws exception if not 200
 
         json = response.json()
         #: The user dict returned by the API; contains basic user information
         self.user: dict[str, str] = json['data']['user']
         #: The session token used to authenticate requests
         self.session_token: str = json['data']['session-token']
-        #: An alternate token which can be used to login without a password
-        self.remember_token: Optional[str] = json['data']['remember-token'] if remember_me else None
+        #: A single-use token which can be used to login without a password
+        self.remember_token: Optional[str] = \
+            json['data']['remember-token'] if remember_me else None
         #: The headers to use for API requests
         self.headers: dict[str, str] = {'Authorization': self.session_token}
         self.validate()
 
     def validate(self) -> bool:
         """
         Validates the current session by sending a request to the API.
 
         :return: True if the session is valid and False otherwise.
         """
-        response = requests.post(f'{self.base_url}/sessions/validate', headers=self.headers)
+        response = requests.post(
+            f'{self.base_url}/sessions/validate',
+            headers=self.headers
+        )
         return (response.status_code // 100 == 2)
 
     def destroy(self) -> bool:
         """
-        Sends a API request to log out of the existing session. This will invalidate the
-        current session token and login.
+        Sends a API request to log out of the existing session. This will
+        invalidate the current session token and login.
 
-        :return: True if the session was terminated successfully and False otherwise.
+        :return: True if the session was terminated successfully and
+        False otherwise.
         """
-        response = requests.delete(f'{self.base_url}/sessions', headers=self.headers)
+        response = requests.delete(
+            f'{self.base_url}/sessions',
+            headers=self.headers
+        )
         return (response.status_code // 100 == 2)
 
     def get_customer(self) -> dict[str, Any]:
         """
         Gets the customer dict from the API.
 
         :return: a Tastytrade 'Customer' object in JSON format.
         """
-        response = requests.get(f'{self.base_url}/customers/me', headers=self.headers)
+        response = requests.get(
+            f'{self.base_url}/customers/me',
+            headers=self.headers
+        )
         validate_response(response)  # throws exception if not 200
 
         return response.json()['data']
```

### Comparing `tastytrade-5.6/tastytrade/streamer.py` & `tastytrade-5.7/tastytrade/streamer.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     threshold: str
     threshold_numeric: Decimal
     dx_symbol: str
 
 
 class UnderlyingYearGainSummary(TastytradeJsonDataclass):
     """
-    Dataclass that contains information about the yearly gainYloss for an underlying
+    Dataclass that contains information about the yearly gain
+    or loss for an underlying
     """
     year: int
     account_number: str
     symbol: str
     instrument_type: InstrumentType
     fees: Decimal
     fees_effect: PriceEffect
@@ -67,29 +68,30 @@
     yearly_realized_gain_effect: PriceEffect
     realized_lot_gain: Decimal
     realized_lot_gain_effect: PriceEffect
 
 
 class SubscriptionType(str, Enum):
     """
-    This is an :class:`~enum.Enum` that contains the subscription types for the alert streamer.
+    This is an :class:`~enum.Enum` that contains the subscription types
+    for the alert streamer.
     """
-    ACCOUNT = 'account-subscribe'  # 'account-subscribe' may be deprecated in the future
+    ACCOUNT = 'account-subscribe'  # may be 'connect' in the future
     HEARTBEAT = 'heartbeat'
     PUBLIC_WATCHLISTS = 'public-watchlists-subscribe'
     QUOTE_ALERTS = 'quote-alerts-subscribe'
     USER_MESSAGE = 'user-message-subscribe'
 
 
 class AlertStreamer:
     """
-    Used to subscribe to account-level updates (balances, orders, positions), public
-    watchlist updates, quote alerts, and user-level messages. It should always be
-    initialized using the :meth:`create` function, since the object cannot be fully
-    instantiated without using async.
+    Used to subscribe to account-level updates (balances, orders, positions),
+    public watchlist updates, quote alerts, and user-level messages. It should
+    always be initialized using the :meth:`create` function, since the object
+    cannot be fully instantiated without using async.
 
     Example usage::
 
         session = Session('user', 'pass')
         streamer = await AlertStreamer.create(session)
         accounts = Account.get_accounts(session)
 
@@ -101,43 +103,47 @@
             print(data)
 
     """
     def __init__(self, session: Session):
         #: The active session used to initiate the streamer or make requests
         self.token: str = session.session_token
         #: The base url for the streamer websocket
-        self.base_url: str = CERT_STREAMER_URL if session.is_certification else STREAMER_URL
+        self.base_url: str = \
+            CERT_STREAMER_URL if session.is_certification else STREAMER_URL
 
         self._queue: Queue = Queue()
         self._websocket = None
 
         self._connect_task = asyncio.create_task(self._connect())
 
     @classmethod
     async def create(cls, session: Session) -> 'AlertStreamer':
         """
         Factory method for the :class:`DataStreamer` object. Simply calls the
-        constructor and performs the asynchronous setup tasks. This should be used
-        instead of the constructor.
+        constructor and performs the asynchronous setup tasks. This should be
+        used instead of the constructor.
 
         :param session: active user session to use
         """
         self = cls(session)
         while not self._websocket:
             await asyncio.sleep(0.1)
 
         return self
 
     async def _connect(self) -> None:
         """
-        Connect to the websocket server using the URL and authorization token provided
-        during initialization.
+        Connect to the websocket server using the URL and authorization
+        token provided during initialization.
         """
         headers = {'Authorization': f'Bearer {self.token}'}
-        async with websockets.connect(self.base_url, extra_headers=headers) as websocket:  # type: ignore
+        async with websockets.connect(  # type: ignore
+            self.base_url,
+            extra_headers=headers
+        ) as websocket:
             self._websocket = websocket
             self._heartbeat_task = asyncio.create_task(self._heartbeat())
 
             while True:
                 raw_message = await self._websocket.recv()  # type: ignore
                 logger.debug('raw message: %s', raw_message)
                 await self._queue.put(json.loads(raw_message))
@@ -151,17 +157,22 @@
             data = await self._queue.get()
             type_str = data.get('type')
             if type_str is not None:
                 yield self._map_message(type_str, data['data'])
             elif data.get('action') != 'heartbeat':
                 logger.debug('subscription message: %s', data)
 
-    def _map_message(self, type_str: str, data: dict) -> TastytradeJsonDataclass:
+    def _map_message(
+        self,
+        type_str: str,
+        data: dict
+    ) -> TastytradeJsonDataclass:
         """
-        I'm not sure what the user-status messages look like, so they're absent.
+        I'm not sure what the user-status messages look like,
+        so they're absent.
         """
         if type_str == 'AccountBalance':
             return AccountBalance(**data)
         elif type_str == 'CurrentPosition':
             return CurrentPosition(**data)
         elif type_str == 'Order':
             return PlacedOrder(**data)
@@ -178,17 +189,20 @@
         else:
             raise TastytradeError(f'Unknown message type: {type_str}\n{data}')
 
     async def account_subscribe(self, accounts: list[Account]) -> None:
         """
         Subscribes to account-level updates (balances, orders, positions).
 
-        :param accounts: list of :class:`tastytrade.account.Account`s to subscribe to updates for
+        :param accounts: list of :class:`Account` to subscribe to updates for
         """
-        await self._subscribe(SubscriptionType.ACCOUNT, [acc.account_number for acc in accounts])
+        await self._subscribe(
+            SubscriptionType.ACCOUNT,
+            [acc.account_number for acc in accounts]
+        )
 
     async def public_watchlists_subscribe(self) -> None:
         """
         Subscribes to public watchlist updates.
         """
         await self._subscribe(SubscriptionType.PUBLIC_WATCHLISTS)
 
@@ -210,41 +224,47 @@
         Closes the websocket connection and cancels the heartbeat task.
         """
         self._connect_task.cancel()
         self._heartbeat_task.cancel()
 
     async def _heartbeat(self) -> None:
         """
-        Sends a heartbeat message every 10 seconds to keep the connection alive.
+        Sends a heartbeat message every 10 seconds to keep the connection
+        alive.
         """
         while True:
             await self._subscribe(SubscriptionType.HEARTBEAT, '')
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
-    async def _subscribe(self, subscription: SubscriptionType, value: Union[Optional[str], list[str]] = '') -> None:
+    async def _subscribe(
+        self,
+        subscription: SubscriptionType,
+        value: Union[Optional[str], list[str]] = ''
+    ) -> None:
         """
-        Subscribes to one of the :class:`SubscriptionType`s. Depending on the kind of
+        Subscribes to a :class:`SubscriptionType`. Depending on the kind of
         subscription, the value parameter may be required.
         """
         message: dict[str, Any] = {
             'auth-token': self.token,
             'action': subscription
         }
         if value:
             message['value'] = value
         logger.debug('sending alert subscription: %s', message)
         await self._websocket.send(json.dumps(message))  # type: ignore
 
 
 class DataStreamer:
     """
-    A :class:`DataStreamer` object is used to fetch quotes or greeks for a given symbol
-    or list of symbols. It should always be initialized using the :meth:`create` function,
-    since the object cannot be fully instantiated without using async.
+    A :class:`DataStreamer` object is used to fetch quotes or greeks
+    for a given symbol or list of symbols. It should always be
+    initialized using the :meth:`create` function, since the object
+    cannot be fully instantiated without using async.
 
     Example usage::
 
         session = Session('user', 'pass')
         streamer = await DataStreamer.create(session)
 
         subs = ['SPY', 'GLD']  # list of quotes to fetch
@@ -263,29 +283,32 @@
         self._counter = 0
         self._lock: Lock = Lock()
         self._queue: Queue = Queue()
         self._queue_candle: Queue = Queue()
         #: The unique client identifier received from the server
         self.client_id: Optional[str] = None
 
-        response = requests.get(f'{session.base_url}/quote-streamer-tokens', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/quote-streamer-tokens',
+            headers=session.headers
+        )
         validate_response(response)
         logger.debug('response %s', json.dumps(response.json()))
         self._auth_token = response.json()['data']['token']
         url = response.json()['data']['websocket-url'] + '/cometd'
         self._wss_url = url.replace('https', 'wss')
 
         self._connect_task = asyncio.create_task(self._connect())
 
     @classmethod
     async def create(cls, session: Session) -> 'DataStreamer':
         """
-        Factory method for the :class:`DataStreamer` object. Simply calls the
-        constructor and performs the asynchronous setup tasks. This should be used
-        instead of the constructor.
+        Factory method for the :class:`DataStreamer` object.
+        Simply calls the constructor and performs the asynchronous
+        setup tasks. This should be used instead of the constructor.
 
         Setup time is around 10-15 seconds.
 
         :param session: active user session to use
         """
         self = cls(session)
         while not self.client_id:
@@ -296,32 +319,36 @@
     async def _next_id(self):
         async with self._lock:
             self._counter += 1
         return self._counter
 
     async def _connect(self) -> None:
         """
-        Connect to the websocket server using the URL and authorization token provided
-        during initialization.
+        Connect to the websocket server using the URL and
+        authorization token provided during initialization.
         """
         headers = {'Authorization': f'Bearer {self._auth_token}'}
 
-        async with websockets.connect(self._wss_url, extra_headers=headers) as websocket:  # type: ignore
+        async with websockets.connect(  # type: ignore
+            self._wss_url,
+            extra_headers=headers
+        ) as websocket:
             self._websocket = websocket
             await self._handshake()
 
             while not self.client_id:
                 raw_message = await self._websocket.recv()
                 message = json.loads(raw_message)[0]
 
                 logger.debug('received: %s', message)
                 if message['channel'] == Channel.HANDSHAKE:
                     if message['successful']:
                         self.client_id = message['clientId']
-                        self._heartbeat_task = asyncio.create_task(self._heartbeat())
+                        self._heartbeat_task = \
+                            asyncio.create_task(self._heartbeat())
                     else:
                         raise TastytradeError('Handshake failed')
 
             # main loop
             while True:
                 raw_message = await self._websocket.recv()
                 message = json.loads(raw_message)[0]
@@ -333,47 +360,53 @@
                     logger.debug('candle received: %s', message)
                     await self._queue_candle.put(message['data'])
                 elif message['channel'] == Channel.SUBSCRIPTION:
                     logger.debug('sub received: %s', message)
 
     async def _handshake(self) -> None:
         """
-        Sends a handshake message to the specified WebSocket connection. The handshake
-        message is sent as a JSON-encoded array with a single element, containing the
+        Sends a handshake message to the specified WebSocket
+        connection. The handshake message is sent as a JSON
+        encoded array with a single element, containing the
         handshake message as its only element.
         """
         id = await self._next_id()
         message = {
             'id': id,
             'version': '1.0',
             'minimumVersion': '1.0',
             'channel': Channel.HANDSHAKE,
-            'supportedConnectionTypes': ['websocket', 'long-polling', 'callback-polling'],
+            'supportedConnectionTypes': [
+                'websocket',
+                'long-polling',
+                'callback-polling'
+            ],
             'ext': {'com.devexperts.auth.AuthToken': self._auth_token},
             'advice': {
                 'timeout': 60000,
                 'interval': 0
             }
         }
         await self._websocket.send(json.dumps([message]))
 
     async def listen(self) -> AsyncIterator[Event]:
         """
-        Using the existing subscriptions, pulls :class:`~tastytrade.dxfeed.event.Event`s and yield returns
+        Using the existing subscriptions, pulls events and yield returns
         them. Never exits unless there's an error or the channel is closed.
         """
         while True:
             raw_data = await self._queue.get()
             messages = self._map_message(raw_data)
             for message in messages:
                 yield message
 
     async def listen_candle(self) -> AsyncIterator[Candle]:
         """
-        Using the existing subscriptions, pulls candles and yield returns them.
+        Using the existing subscriptions, pulls candles and yield
+        returns them.
         Never exits unless there's an error or the channel is closed.
         """
         while True:
             raw_data = await self._queue_candle.get()
             messages = self._map_message(raw_data)
             for message in messages:
                 yield message  # type: ignore
@@ -383,52 +416,64 @@
         Closes the websocket connection and cancels the heartbeat task.
         """
         self._connect_task.cancel()
         self._heartbeat_task.cancel()
 
     async def _heartbeat(self) -> None:
         """
-        Sends a heartbeat message every 10 seconds to keep the connection alive.
+        Sends a heartbeat message every 10 seconds to keep the connection
+        alive.
         """
         while True:
             id = await self._next_id()
             message = {
                 'id': id,
                 'channel': Channel.HEARTBEAT,
                 'clientId': self.client_id,
                 'connectionType': 'websocket'
             }
             logger.debug('sending heartbeat: %s', message)
             await self._websocket.send(json.dumps([message]))
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
-    async def subscribe(self, event_type: EventType, symbols: list[str], reset: bool = False) -> None:
+    async def subscribe(
+        self,
+        event_type: EventType,
+        symbols: list[str],
+        reset: bool = False
+    ) -> None:
         """
-        Subscribes to quotes for given list of symbols. Used for recurring data feeds.
+        Subscribes to quotes for given list of symbols. Used for recurring data
+        feeds.
 
         :param event_type: type of subscription to add
         :param symbols: list of symbols to subscribe for
         :param reset:
-            whether to reset the subscription list (remove all other subscriptions of all types)
+            whether to reset the subscription list (remove all other
+            subscriptions of all types)
         """
         id = await self._next_id()
         message = {
             'id': id,
             'channel': Channel.SUBSCRIPTION,
             'data': {
                 'reset': reset,
                 'add': {event_type: symbols}
             },
             'clientId': self.client_id
         }
         logger.debug('sending subscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
-    async def unsubscribe(self, event_type: EventType, symbols: list[str]) -> None:
+    async def unsubscribe(
+        self,
+        event_type: EventType,
+        symbols: list[str]
+    ) -> None:
         """
         Removes existing subscription for given list of symbols.
 
         :param event_type: type of subscription to remove
         :param symbols: list of symbols to unsubscribe from
         """
         id = await self._next_id()
@@ -440,21 +485,28 @@
                 'remove': {event_type: symbols}
             },
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
-    async def subscribe_candle(self, ticker: str, start_time: datetime, interval: str) -> None:
+    async def subscribe_candle(
+        self,
+        ticker: str,
+        start_time: datetime,
+        interval: str
+    ) -> None:
         """
         Subscribes to candle-style 'OHLC' data for the given symbol.
 
         :param ticker: symbol to get date for
         :param start_time: starting time for the data range
-        :param interval: the width of each candle in time, e.g. '5m', '1h', '3d', '1w', '1mo'
+        :param interval:
+            the width of each candle in time, e.g. '5m', '1h', '3d',
+            '1w', '1mo'
         """
         id = await self._next_id()
         message = {
             'id': id,
             'channel': Channel.SUBSCRIPTION,
             'data': {
                 'addTimeSeries': {
@@ -467,15 +519,15 @@
             'clientId': self.client_id
         }
         logger.debug('sending subscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
     async def unsubscribe_candle(self, ticker: str, interval: str) -> None:
         """
-        Removes existing :class:`~tastytrade.dxfeed.event.Candle` subscription for given list of symbols.
+        Removes existing candle subscription for given list of symbols.
 
         :param ticker: symbol to unsubscribe from
         :param interval: candle width to unsubscribe from
         """
         id = await self._next_id()
         message = {
             'id': id,
@@ -486,15 +538,15 @@
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
     def _map_message(self, message) -> list[Event]:
         """
-        Takes the raw JSON data and returns a list of parsed :class:`~tastytrade.dxfeed.event.Event` objects.
+        Takes the raw JSON data and returns a list of parsed event objects.
         """
         # the first time around, types are shown
         if isinstance(message[0], str):
             msg_type = message[0]
         else:
             msg_type = message[0][0]
         # regardless, the second element will be the raw data
@@ -514,8 +566,9 @@
         elif msg_type == EventType.THEO_PRICE:
             return TheoPrice.from_stream(data)
         elif msg_type == EventType.TIME_AND_SALE:
             return TimeAndSale.from_stream(data)
         elif msg_type == EventType.TRADE:
             return Trade.from_stream(data)
         else:
-            raise TastytradeError(f'Unknown message type received from streamer: {message}')
+            msg = f'Unknown message type received from streamer: {message}'
+            raise TastytradeError(msg)
```

### Comparing `tastytrade-5.6/tastytrade/utils.py` & `tastytrade-5.7/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.6/tastytrade/watchlists.py` & `tastytrade-5.7/tastytrade/watchlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,31 +32,41 @@
         """
         Fetches a list of all Tastytrade public pairs watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`PairsWatchlist` objects.
         """
-        response = requests.get(f'{session.base_url}/pairs-watchlists', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/pairs-watchlists',
+            headers=session.headers
+        )
         validate_response(response)
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
-    def get_pairs_watchlist(cls, session: Session, name: str) -> 'PairsWatchlist':
+    def get_pairs_watchlist(
+        cls,
+        session: Session,
+        name: str
+    ) -> 'PairsWatchlist':
         """
         Fetches a Tastytrade public pairs watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the pairs watchlist to fetch.
 
         :return: a :class:`PairsWatchlist` object.
         """
-        response = requests.get(f'{session.base_url}/pairs-watchlists/{name}', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/pairs-watchlists/{name}',
+            headers=session.headers
+        )
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
 
@@ -67,15 +77,19 @@
     """
     name: str
     watchlist_entries: Optional[list[dict[str, str]]] = None
     group_name: str = 'default'
     order_index: int = 9999
 
     @classmethod
-    def get_public_watchlists(cls, session: Session, counts_only: bool = False) -> list['Watchlist']:
+    def get_public_watchlists(
+        cls,
+        session: Session,
+        counts_only: bool = False
+    ) -> list['Watchlist']:
         """
         Fetches a list of all Tastytrade public watchlists.
 
         :param session: the session to use for the request.
         :param counts_only: whether to only fetch the counts of the watchlists.
 
         :return: a list of :class:`Watchlist` objects.
@@ -97,15 +111,18 @@
         Fetches a Tastytrade public watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to fetch.
 
         :return: a :class:`Watchlist` object.
         """
-        response = requests.get(f'{session.base_url}/public-watchlists/{name}', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/public-watchlists/{name}',
+            headers=session.headers
+        )
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
     @classmethod
@@ -113,15 +130,18 @@
         """
         Fetches a the user's private watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Watchlist` objects.
         """
-        response = requests.get(f'{session.base_url}/watchlists', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/watchlists',
+            headers=session.headers
+        )
         validate_response(response)
 
         data = response.json()['data']['items']
 
         return [cls(**entry) for entry in data]
 
     @classmethod
@@ -130,30 +150,36 @@
         Fetches a user's watchlist by name.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to fetch.
 
         :return: a :class:`Watchlist` object.
         """
-        response = requests.get(f'{session.base_url}/watchlists/{name}', headers=session.headers)
+        response = requests.get(
+            f'{session.base_url}/watchlists/{name}',
+            headers=session.headers
+        )
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
     @classmethod
     def remove_private_watchlist(cls, session: Session, name: str) -> None:
         """
         Deletes the named private watchlist.
 
         :param session: the session to use for the request.
         :param name: the name of the watchlist to delete.
         """
-        response = requests.delete(f'{session.base_url}/watchlists/{name}', headers=session.headers)
+        response = requests.delete(
+            f'{session.base_url}/watchlists/{name}',
+            headers=session.headers
+        )
         validate_response(response)
 
     def upload_private_watchlist(self, session: Session) -> None:
         """
         Creates a private remote watchlist identical to this local one.
 
         :param session: the session to use for the request.
@@ -180,15 +206,25 @@
 
     def add_symbol(self, symbol: str, instrument_type: InstrumentType) -> None:
         """
         Adds a symbol to the watchlist.
         """
         if self.watchlist_entries is None:
             self.watchlist_entries = []
-        self.watchlist_entries.append({'symbol': symbol, 'instrument-type': instrument_type})
-
-    def remove_symbol(self, symbol: str, instrument_type: InstrumentType) -> None:
+        self.watchlist_entries.append({
+            'symbol': symbol,
+            'instrument-type': instrument_type
+        })
+
+    def remove_symbol(
+        self,
+        symbol: str,
+        instrument_type: InstrumentType
+    ) -> None:
         """
         Removes a symbol from the watchlist.
         """
         if self.watchlist_entries is not None:
-            self.watchlist_entries.remove({'symbol': symbol, 'instrument-type': instrument_type})
+            self.watchlist_entries.remove({
+                'symbol': symbol,
+                'instrument-type': instrument_type
+            })
```

### Comparing `tastytrade-5.6/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.7/tastytrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.6
+Version: 5.7
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-5.6/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.7/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

