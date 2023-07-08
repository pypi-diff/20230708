# Comparing `tmp/edp_redy_py-0.1.5.tar.gz` & `tmp/edp_redy_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.5.tar", last modified: Sat Jul  8 17:55:23 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.6.tar", last modified: Sat Jul  8 18:06:04 2023, max compression
```

## Comparing `edp_redy_py-0.1.5.tar` & `edp_redy_py-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.132063 edp_redy_py-0.1.5/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      283 2023-07-08 17:55:23.132603 edp_redy_py-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.5/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 17:55:23.134177 edp_redy_py-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-07-08 17:54:21.000000 edp_redy_py-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.109630 edp_redy_py-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.118243 edp_redy_py-0.1.5/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.5/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.5/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.5/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2573 2023-07-08 17:49:03.000000 edp_redy_py-0.1.5/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.119826 edp_redy_py-0.1.5/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.5/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.5/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.5/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.5/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.121411 edp_redy_py-0.1.5/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.5/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.5/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:55:23.130896 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 17:55:23.000000 edp_redy_py-0.1.5/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.285747 edp_redy_py-0.1.6/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-08 18:06:04.286253 edp_redy_py-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.6/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 18:06:04.287315 edp_redy_py-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-07-08 18:05:16.000000 edp_redy_py-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.259000 edp_redy_py-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.269145 edp_redy_py-0.1.6/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.6/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.6/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.6/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2549 2023-07-08 18:05:54.000000 edp_redy_py-0.1.6/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.271450 edp_redy_py-0.1.6/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.6/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.6/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.6/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.6/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.273568 edp_redy_py-0.1.6/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.6/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.6/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.284479 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1.5/LICENSE` & `edp_redy_py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.5/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.6/src/edp_redy/authenticate.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.5/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.6/src/edp_redy/edp_mqtt.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,19 @@
     authentication: AuthenticationResult = None
     connection: Connection
 
     def __init__(self, authentication: AuthenticationResult):
         self.authentication = authentication
 
     def get_cognito_provider(self, user: User) -> auth.AwsCredentialsProvider:
-        cognito_endpoint = f"cognito-identity.{POOL_REGION}.amazonaws.com"
         credentials_provider = auth.AwsCredentialsProvider.new_cognito(
-            endpoint=cognito_endpoint,
+            endpoint=f"cognito-identity.{POOL_REGION}.amazonaws.com",
             identity=user.identity_id,
             tls_ctx=io.ClientTlsContext(io.TlsContextOptions()),
-            logins=[(f"{cognito_endpoint}/{POOL_ID}", self.authentication.IdToken)]
+            logins=[(f"cognito-idp.{POOL_REGION}.amazonaws.com/{POOL_ID}", self.authentication.IdToken)]
         )
         return credentials_provider
 
     def connect(self, user: User):
         self.connection = mqtt_connection_builder.websockets_with_default_aws_signing(
             endpoint=HOST,
             region=POOL_REGION,
```

### Comparing `edp_redy_py-0.1.5/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.6/src/edp_redy/equipment/equipment.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.5/src/edp_redy/helpers.py` & `edp_redy_py-0.1.6/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.5/src/edp_redy/redy.py` & `edp_redy_py-0.1.6/src/edp_redy/redy.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.5/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.6/src/edp_redy/usermanagement/usermanagement.py`

 * *Files identical despite different names*

