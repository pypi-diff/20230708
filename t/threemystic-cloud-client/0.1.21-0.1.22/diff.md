# Comparing `tmp/threemystic_cloud_client-0.1.21.tar.gz` & `tmp/threemystic_cloud_client-0.1.22.tar.gz`

## Comparing `threemystic_cloud_client-0.1.21.tar` & `threemystic_cloud_client-0.1.22.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12319 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    22417 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/hatch.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.22/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,21 +240,20 @@
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
       region = self.get_default_region()
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
       account = self.get_default_account()
 
     if not refresh and self._get_assumed_role_credentials().get(self._get_assumed_role_credentials_key(account= account, role= role)) is not None:
-      experation = self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["roleCredentials"]["expiration"]
-      print(f'expiration: {experation}')
-      if self.get_common().helper_type().general().is_type(obj= experation, type_check= str):
-        experation = self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=experation)
+      expiration = self._auto_parse_aws_expiration(
+        expiration= self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["roleCredentials"]["expiration"]
+      )
 
-        if not self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= experation):
-          return self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["roleCredentials"]
+      if not self.get_common().helper_type().datetime().is_token_expired_now(compare_datetime= expiration):
+        return self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)]["roleCredentials"]
     
     self._get_assumed_role_credentials()[self._get_assumed_role_credentials_key(account= account, role= role)] = self.__get_sso_boto_session().client('sso').get_role_credentials(
       roleName=role,
       accountId=self.get_account_id(account= account),
       accessToken=self._get_session_accesstoken()
     )
```

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
       return config
     
     config.region_name = region
     return config
 
-  def get_boto_client(self, client, account=None, role = None, region = None, *argv, **kwargs):    
+  def get_boto_client(self, client, account=None, role = None, region = None, *argv, **kwargs):
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
       region = self.get_default_region()
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= role):
       region = self.get_default_rolename()
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
@@ -375,24 +375,35 @@
     if hasattr(session, "create_client"):
        self._get_created_boto_clients()[cache_key] = session.create_client(client, config= self.get_boto_config(region= region, *argv, **kwargs))
        return self._get_created_boto_clients()[cache_key]
        
     self._get_created_boto_clients()[cache_key] = session.client(client, config= self.get_boto_config(region= region, *argv, **kwargs))
     return self._get_created_boto_clients()[cache_key]
 
+  def _auto_parse_aws_expiration(self, expiration, *argv, **kwargs):
+    if self.get_common().helper_type().general().is_type(obj= expiration, type_check= int):
+      return self.get_common().helper_type().datetime().get_from_timestamp(time_delta=expiration)
+    
+    if self.get_common().helper_type().general().is_type(obj= expiration, type_check= str):
+      return self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=expiration)
+    
+        
   def _convert_assume_role_credentials_boto_session(self, credentials):
-    experation = credentials["expiration"]
-    if self.get_common().helper_type().general().is_type(obj= experation, type_check= str):
-      experation = self.get_common().helper_type().datetime().parse_iso(iso_datetime_str=experation)
+    expiration = self._auto_parse_aws_expiration(
+      expiration= credentials["expiration"]
+    )
     
+
     return {
         "access_key": credentials["accessKeyId"],
         "secret_key": credentials["secretAccessKey"],
         "token": credentials["sessionToken"],
-        "expiry_time": f"{experation}+00:00" 
+        "expiry_time": self.get_common().helper_type().datetime().get_iso_datetime(
+          dt= expiration
+        )
       }
 
 
   def __get_boto_session(self, role = None, region = None, profile = None, **kwargs):
     if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile):
       return boto_session(profile_name= profile) if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region) else boto_session(profile_name= profile, region_name= region)
```

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.22/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/.gitignore` & `threemystic_cloud_client-0.1.22/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/LICENSE` & `threemystic_cloud_client-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/README.md` & `threemystic_cloud_client-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/hatch.toml` & `threemystic_cloud_client-0.1.22/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.21/pyproject.toml` & `threemystic_cloud_client-0.1.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.7",
+  "threemystic-common >= 0.1.8",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
```

### Comparing `threemystic_cloud_client-0.1.21/PKG-INFO` & `threemystic_cloud_client-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.21
+Version: 0.1.22
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
-Requires-Dist: threemystic-common>=0.1.7
+Requires-Dist: threemystic-common>=0.1.8
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

