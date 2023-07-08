# Comparing `tmp/transaction-accounts-0.2.0.tar.gz` & `tmp/transaction-accounts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.2.0.tar", last modified: Sat May 20 14:32:40 2023, max compression
+gzip compressed data, was "transaction-accounts-0.2.1.tar", last modified: Sat Jul  8 14:46:59 2023, max compression
```

## Comparing `transaction-accounts-0.2.0.tar` & `transaction-accounts-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.340746 transaction-accounts-0.2.0/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.2.0/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-20 14:32:40.340894 transaction-accounts-0.2.0/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.331696 transaction-accounts-0.2.0/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.2.0/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.2.0/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    21392 2023-05-20 14:27:48.000000 transaction-accounts-0.2.0/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.2.0/accounts/utility.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-20 14:32:40.341443 transaction-accounts-0.2.0/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7631 2023-05-20 14:32:39.000000 transaction-accounts-0.2.0/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.337038 transaction-accounts-0.2.0/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.2.0/tests/test_calendar.py
--rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.2.0/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.2.0/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     4673 2023-05-20 14:28:42.000000 transaction-accounts-0.2.0/tests/test_loanGiven.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.2.0/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     6240 2023-05-20 14:31:40.000000 transaction-accounts-0.2.0/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.2.0/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.340371 transaction-accounts-0.2.0/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       31 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 ivamusic   (502) staff       (20)        0 2023-07-08 14:46:59.984864 transaction-accounts-0.2.1/
+-rw-r--r--   0 ivamusic   (502) staff       (20)     1066 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/LICENSE.txt
+-rw-r--r--   0 ivamusic   (502) staff       (20)     7342 2023-07-08 14:46:59.985119 transaction-accounts-0.2.1/PKG-INFO
+drwxr-xr-x   0 ivamusic   (502) staff       (20)        0 2023-07-08 14:46:59.971417 transaction-accounts-0.2.1/accounts/
+-rw-r--r--   0 ivamusic   (502) staff       (20)        0 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/accounts/__init__.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)    10332 2023-07-08 14:21:38.000000 transaction-accounts-0.2.1/accounts/metadata.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)    21392 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/accounts/runtime.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)      201 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/accounts/utility.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)       79 2023-07-08 14:46:59.985960 transaction-accounts-0.2.1/setup.cfg
+-rw-r--r--   0 ivamusic   (502) staff       (20)     7631 2023-07-08 14:24:03.000000 transaction-accounts-0.2.1/setup.py
+drwxr-xr-x   0 ivamusic   (502) staff       (20)        0 2023-07-08 14:46:59.977695 transaction-accounts-0.2.1/tests/
+-rw-r--r--   0 ivamusic   (502) staff       (20)     2834 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_calendar.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)    18462 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_config.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)     1054 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_configuration.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)     4673 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_loanGiven.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)     2197 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_rate_type.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)     6240 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_runtime.py
+-rw-r--r--   0 ivamusic   (502) staff       (20)     3942 2023-07-08 14:17:43.000000 transaction-accounts-0.2.1/tests/test_schedule.py
+drwxr-xr-x   0 ivamusic   (502) staff       (20)        0 2023-07-08 14:46:59.982967 transaction-accounts-0.2.1/transaction_accounts.egg-info/
+-rw-r--r--   0 ivamusic   (502) staff       (20)     7342 2023-07-08 14:46:59.000000 transaction-accounts-0.2.1/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 ivamusic   (502) staff       (20)      496 2023-07-08 14:46:59.000000 transaction-accounts-0.2.1/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 ivamusic   (502) staff       (20)        1 2023-07-08 14:46:59.000000 transaction-accounts-0.2.1/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 ivamusic   (502) staff       (20)       31 2023-07-08 14:46:59.000000 transaction-accounts-0.2.1/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 ivamusic   (502) staff       (20)        9 2023-07-08 14:46:59.000000 transaction-accounts-0.2.1/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.2.0/LICENSE.txt` & `transaction-accounts-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/PKG-INFO` & `transaction-accounts-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

### Comparing `transaction-accounts-0.2.0/accounts/metadata.py` & `transaction-accounts-0.2.1/accounts/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,18 +164,18 @@
     name: str
     label: str
     frequency: ScheduleFrequency
     end_type: ScheduleEndType
     business_day_adjustment: BusinessDayAdjustment
     interval_expression: str
     start_date_expression: str
-    end_date_expression: str = None
-    number_of_repeats_expression: str = None
-    include_dates_expression: str = None
-    exclude_dates_expression: str = None
+    end_date_expression: Optional[str] = None
+    number_of_repeats_expression: Optional[str] = None
+    include_dates_expression: Optional[str] = None
+    exclude_dates_expression: Optional[str] = None
     editable: bool = True
 
 
 class ScheduledTransaction(BaseModel):
     schedule_name: str
     timing: ScheduledTransactionTiming
     generated_transaction_type: str
```

### Comparing `transaction-accounts-0.2.0/accounts/runtime.py` & `transaction-accounts-0.2.1/accounts/runtime.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/setup.py` & `transaction-accounts-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.2.0',
+    version='0.2.1',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction accounts.
```

### Comparing `transaction-accounts-0.2.0/tests/test_calendar.py` & `transaction-accounts-0.2.1/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_config.py` & `transaction-accounts-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_configuration.py` & `transaction-accounts-0.2.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_loanGiven.py` & `transaction-accounts-0.2.1/tests/test_loanGiven.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_rate_type.py` & `transaction-accounts-0.2.1/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_runtime.py` & `transaction-accounts-0.2.1/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/tests/test_schedule.py` & `transaction-accounts-0.2.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.2.0/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.2.1/transaction_accounts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

