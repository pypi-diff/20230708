# Comparing `tmp/django_hmac_authentication-1.3.2.tar.gz` & `tmp/django_hmac_authentication-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.3.2.tar", last modified: Mon Jun 26 08:56:03 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.4.0.tar", last modified: Sat Jul  8 02:31:08 2023, max compression
```

## Comparing `django_hmac_authentication-1.3.2.tar` & `django_hmac_authentication-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-26 08:49:07.000000 django_hmac_authentication-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.982444 django_hmac_authentication-1.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.986444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-26 08:49:07.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/aes.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-26 08:22:01.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2023-06-26 08:43:45.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/client_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1312 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6871 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6333 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-08 02:25:39.000000 django_hmac_authentication-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.616911 django_hmac_authentication-1.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.620911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-08 02:25:39.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-26 08:22:01.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4447 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6871 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/top_level.txt
```

### Comparing `django_hmac_authentication-1.3.2/LICENSE` & `django_hmac_authentication-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/PKG-INFO` & `django_hmac_authentication-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-Metadata-Version: 2.1
-Name: django_hmac_authentication
-Version: 1.3.2
-Summary: Django HMAC authentication using shared secret
-Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
-Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # django_hmac_authentication
 Django hmac authentication with shared secret
 
 * Django model with HMAC shared secret 
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
-
-New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
+New features
+* Option to speedup using cache in Django's `CACHES` settings.
+* A lru_cache is enabled locally to save compute time to decode hmac keys
+
+> :rocket: :rocket: Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -44,14 +33,17 @@
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
 * `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
 
+* `HMAC_CACHE_ALIAS` Alias of a cache backend in Django's `CACHES` settings. When set, the cache specified by the alias 
+   is used to cache hmac keys. Example: `hmac_cache`. Default: None (i.e caching disabled)
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -70,14 +62,17 @@
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
 HMAC_EXPIRES_IN = '5m'
+# This cache alias must be defined in Django's CACHES. 
+# See https://docs.djangoproject.com/en/4.2/ref/settings/#caches
+HMAC_CACHE_ALIAS = 'hmac_cache'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.3.2/README.md` & `django_hmac_authentication-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,38 @@
+Metadata-Version: 2.1
+Name: django_hmac_authentication
+Version: 1.4.0
+Summary: Django HMAC authentication using shared secret
+Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
+Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # django_hmac_authentication
 Django hmac authentication with shared secret
 
 * Django model with HMAC shared secret 
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
-
-New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
+New features
+* Option to speedup using cache in Django's `CACHES` settings.
+* A lru_cache is enabled locally to save compute time to decode hmac keys
+
+> :rocket: :rocket: Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -31,14 +46,17 @@
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
 * `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
 
+* `HMAC_CACHE_ALIAS` Alias of a cache backend in Django's `CACHES` settings. When set, the cache specified by the alias 
+   is used to cache hmac keys. Example: `hmac_cache`. Default: None (i.e caching disabled)
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -57,14 +75,17 @@
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
 HMAC_EXPIRES_IN = '5m'
+# This cache alias must be defined in Django's CACHES. 
+# See https://docs.djangoproject.com/en/4.2/ref/settings/#caches
+HMAC_CACHE_ALIAS = 'hmac_cache'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.3.2/pyproject.toml` & `django_hmac_authentication-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["django_hmac_authentication*"]
 namespaces = false
 
 [project]
 name = "django_hmac_authentication"
-version = "1.3.2"
+version = "1.4.0"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,18 @@
     ExpiredRequestException,
     FutureRequestException,
     KeyDoesNotExistException,
     RevokedKeyException,
     SignatureVerificationException,
     UnsupportedHMACMethodException,
 )
-from django_hmac_authentication.models import ApiHMACKey
-from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
+from django_hmac_authentication.server_utils import (
+    aes_decrypt_hmac_secret,
+    get_api_hmac_key,
+)
 
 auth_req_timeout = getattr(settings, 'HMAC_AUTH_REQUEST_TIMEOUT', 5)
 failed_attempts_threshold = getattr(settings, 'HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD', -1)
 hmac_expires_in = getattr(settings, 'HMAC_EXPIRES_IN', None)
 
 
 class HMACAuthentication(authentication.BaseAuthentication):
@@ -80,15 +82,16 @@
         if req_utc >= utcnow:
             raise FutureRequestException()
 
         delta = utcnow - req_utc
         if delta.total_seconds() > auth_req_timeout:
             raise ExpiredRequestException()
 
-        hmac_key = ApiHMACKey.objects.filter(id=key).first()
+        hmac_key = get_api_hmac_key(key_id=key)
+
         if not hmac_key:
             raise KeyDoesNotExistException()
 
         if hmac_key.revoked:
             raise RevokedKeyException()
 
         if hmac_expires_in and (
```

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/checks.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,8 +66,20 @@
                 f'If set, HMAC_EXPIRES_IN expire keys after interval in hours, minutes or seconds.  Found {repr(hmac_expires_in)}',
                 hint="Example '1h', '5m', '3600s'",
                 obj=repr(hmac_expires_in),
                 id='django_hmac_authentication.E004',
             )
         )
 
+    # HMAC_CACHE_ALIAS
+    hmac_cache_alias = getattr(settings, 'HMAC_CACHE_ALIAS', None)
+    if hmac_cache_alias and hmac_cache_alias not in settings.CACHES:
+        errors.append(
+            Error(
+                f'Missing entry in settings.py CACHES for HMAC_CACHE_ALIAS "{hmac_cache_alias}"',
+                hint="See https://docs.djangoproject.com/en/4.2/ref/settings/#caches",
+                obj=repr(hmac_expires_in),
+                id='django_hmac_authentication.E005',
+            )
+        )
+
     return errors
```

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/server_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import base64
 import os
 import secrets
 from datetime import datetime, timedelta, timezone
+from functools import lru_cache
 from hashlib import pbkdf2_hmac
 
 from django.conf import settings
+from django.core.cache import caches
 from rest_framework.exceptions import ValidationError
 
 from django_hmac_authentication.aes import aes_crypt
 from django_hmac_authentication.models import ApiHMACKey
 
 encoding = 'utf-8'
 hash_func = 'sha256'
@@ -16,25 +18,28 @@
 user_model = settings.AUTH_USER_MODEL
 max_hmacs_per_user = getattr(settings, 'MAX_HMACS_PER_USER', 10)
 
 hmac_expires_in = getattr(settings, 'HMAC_EXPIRES_IN', None)
 expires_in_units = ('h', 'm', 's')
 expires_in_config_err = 'expires_in config must be string. Example: 4h, 5m, 3600s etc'
 
+hmac_cache_alias = getattr(settings, 'HMAC_CACHE_ALIAS', None)
+
 
 def aes_encrypted_hmac_secret() -> tuple:
     salt = os.urandom(24)
     iv = salt[-16:]
     enc_key = pbkdf2_hmac(hash_func, settings.SECRET_KEY.encode(encoding), salt, 1000)
 
     hmac_secret = secrets.token_bytes(32)
     encrypted = aes_crypt(hmac_secret, enc_key, iv)
     return hmac_secret, encrypted, enc_key, salt
 
 
+@lru_cache(maxsize=100)
 def aes_decrypt_hmac_secret(encrypted: bytes, salt: bytes) -> bytes:
     enc_key = pbkdf2_hmac(hash_func, settings.SECRET_KEY.encode(encoding), salt, 1000)
     return aes_crypt(encrypted, enc_key, salt[-16:], False)
 
 
 def create_shared_secret_for_user(user: user_model):
     expires_at = None
@@ -70,7 +75,20 @@
 
     if unit == 'h':
         return timedelta(hours=value)
     elif unit == 'm':
         return timedelta(minutes=value)
     else:
         return timedelta(seconds=value)
+
+
+def get_api_hmac_key(key_id):
+    cache_key = f'ApiHMACKey.id.{key_id}'
+    if hmac_cache_alias:
+        hmac_key = caches[hmac_cache_alias].get(cache_key)
+        if not hmac_key:
+            hmac_key = ApiHMACKey.objects.filter(id=key_id).first()
+            caches[hmac_cache_alias].set(cache_key, hmac_key)
+
+        return hmac_key
+    else:
+        return ApiHMACKey.objects.filter(id=key_id).first()
```

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.3.2
+Version: 1.4.0
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -18,19 +18,21 @@
 * Each user's shared secret is protected with separate key
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
-
-New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
+New features
+* Option to speedup using cache in Django's `CACHES` settings.
+* A lru_cache is enabled locally to save compute time to decode hmac keys
+
+> :rocket: :rocket: Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -44,14 +46,17 @@
 Optional configurations:
 
 * `HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD` for maximum tolerated failed attempts.
   Setting this value will enable revoking keys that exceed max failed attempts.
 
 * `HMAC_EXPIRES_IN` to expire keys after interval in hours, minutes or seconds.  Example`'1h'`, `'5m'`, `'3600s'` 
 
+* `HMAC_CACHE_ALIAS` Alias of a cache backend in Django's `CACHES` settings. When set, the cache specified by the alias 
+   is used to cache hmac keys. Example: `hmac_cache`. Default: None (i.e caching disabled)
+
 Example
 ```python
 MAX_HMACS_PER_USER = 10
 HMAC_AUTH_REQUEST_TIMEOUT = 4
 
 INSTALLED_APPS = [
     ...,
@@ -70,14 +75,17 @@
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
 HMAC_EXPIRES_IN = '5m'
+# This cache alias must be defined in Django's CACHES. 
+# See https://docs.djangoproject.com/en/4.2/ref/settings/#caches
+HMAC_CACHE_ALIAS = 'hmac_cache'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

