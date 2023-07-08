# Comparing `tmp/edp_redy_py-0.1.tar.gz` & `tmp/edp_redy_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.tar", last modified: Sat Jul  8 17:21:32 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.1.tar", last modified: Sat Jul  8 17:34:54 2023, max compression
```

## Comparing `edp_redy_py-0.1.tar` & `edp_redy_py-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.846316 edp_redy_py-0.1/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1/LICENSE
--rw-rw-rw-   0        0        0      281 2023-07-08 17:21:32.846822 edp_redy_py-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 17:21:32.848627 edp_redy_py-0.1/setup.cfg
--rw-rw-rw-   0        0        0      373 2023-07-08 17:21:28.000000 edp_redy_py-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.817211 edp_redy_py-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.826747 edp_redy_py-0.1/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1940 2023-07-08 17:15:29.000000 edp_redy_py-0.1/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2570 2023-07-08 17:15:29.000000 edp_redy_py-0.1/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.828321 edp_redy_py-0.1/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7612 2023-07-08 17:15:29.000000 edp_redy_py-0.1/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      591 2023-07-08 16:51:43.000000 edp_redy_py-0.1/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.830436 edp_redy_py-0.1/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2290 2023-07-08 17:15:29.000000 edp_redy_py-0.1/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:21:32.845105 edp_redy_py-0.1/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      281 2023-07-08 17:21:32.000000 edp_redy_py-0.1/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-08 17:21:32.000000 edp_redy_py-0.1/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:21:32.000000 edp_redy_py-0.1/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:21:32.000000 edp_redy_py-0.1/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.654149 edp_redy_py-0.1.1/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:34:54.654149 edp_redy_py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.1/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 17:34:54.655611 edp_redy_py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-07-08 17:34:51.000000 edp_redy_py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.615697 edp_redy_py-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.640292 edp_redy_py-0.1.1/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.1/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-07-08 17:33:35.000000 edp_redy_py-0.1.1/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.1/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2570 2023-07-08 17:15:29.000000 edp_redy_py-0.1.1/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.641339 edp_redy_py-0.1.1/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.1/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.1/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.1/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      594 2023-07-08 17:33:28.000000 edp_redy_py-0.1.1/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.642922 edp_redy_py-0.1.1/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.1/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.1/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:34:54.653101 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 17:34:54.000000 edp_redy_py-0.1.1/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1/LICENSE` & `edp_redy_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.1/src/edp_redy/authenticate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timedelta
 from typing import Any
 
 import requests
 from awscrt import io
 from warrant.aws_srp import AWSSRP
 
-from consts import POOL_ID, CLIENT_ID, POOL_REGION
+from .consts import POOL_ID, CLIENT_ID, POOL_REGION
 
 io.init_logging(io.LogLevel.Error, 'stderr')
 
 
 def authenticate(USERNAME, PASSWORD):
     aws = AWSSRP(username=USERNAME, password=PASSWORD, pool_id=POOL_ID, client_id=CLIENT_ID, pool_region=POOL_REGION)
     authentication = AuthenticationResult.from_dict(json.loads(aws.authenticate_user()))
```

### Comparing `edp_redy_py-0.1/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.1/src/edp_redy/edp_mqtt.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.1/src/edp_redy/equipment/equipment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from datetime import datetime
 from typing import Any
 from typing import List
 from uuid import UUID
 
-from authenticate import AuthenticationResult
-from consts import ENDPOINT
-from helpers import from_str, from_datetime, from_none, from_int, from_list, from_float, from_bool
+from ..authenticate import AuthenticationResult
+from ..consts import ENDPOINT
+from ..helpers import from_str, from_datetime, from_none, from_int, from_list, from_float, from_bool
 
 
 # This code parses date/times, so please
 #
 #     pip install python-dateutil
 #
 # To use this code, make sure you
```

### Comparing `edp_redy_py-0.1/src/edp_redy/helpers.py` & `edp_redy_py-0.1.1/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1/src/edp_redy/redy.py` & `edp_redy_py-0.1.1/src/edp_redy/redy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from authenticate import authenticate, AuthenticationResult
-from edp_mqtt import EDPMQTT
-from usermanagement.usermanagement import UserManagement
+from .authenticate import authenticate, AuthenticationResult
+from .edp_mqtt import EDPMQTT
+from .usermanagement.usermanagement import UserManagement
 
 
 class Redy:
     authentication: AuthenticationResult = None
     user_management: UserManagement
     mqtt: EDPMQTT
```

### Comparing `edp_redy_py-0.1/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.1/src/edp_redy/usermanagement/usermanagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Any
 from uuid import UUID
 
-from authenticate import AuthenticationResult
-from consts import ENDPOINT
-from helpers import from_str, from_datetime, from_none
+from ..authenticate import AuthenticationResult
+from ..consts import ENDPOINT
+from ..helpers import from_str, from_datetime, from_none
 
 
 class User:
     user_id: UUID
     first_name: str
     last_name: str
     email: str
```

