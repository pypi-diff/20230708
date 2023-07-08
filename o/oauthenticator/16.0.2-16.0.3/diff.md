# Comparing `tmp/oauthenticator-16.0.2.tar.gz` & `tmp/oauthenticator-16.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthenticator-16.0.2.tar", last modified: Thu Jul  6 19:19:46 2023, max compression
+gzip compressed data, was "oauthenticator-16.0.3.tar", last modified: Sat Jul  8 12:47:16 2023, max compression
```

## Comparing `oauthenticator-16.0.2.tar` & `oauthenticator-16.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:46.950603 oauthenticator-16.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 19:19:46.950603 oauthenticator-16.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:46.946603 oauthenticator-16.0.2/oauthenticator/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    38268 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/okpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/openshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:46.946603 oauthenticator-16.0.2/oauthenticator/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/schemas/cilogon-schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:46.950603 oauthenticator-16.0.2/oauthenticator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_okpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/oauthenticator/tests/test_openshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:19:46.946603 oauthenticator-16.0.2/oauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 19:19:46.000000 oauthenticator-16.0.2/oauthenticator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:19:46.950603 oauthenticator-16.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-06 19:19:36.000000 oauthenticator-16.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:16.103799 oauthenticator-16.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-08 12:47:16.099799 oauthenticator-16.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:16.099799 oauthenticator-16.0.3/oauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38268 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:16.099799 oauthenticator-16.0.3/oauthenticator/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/schemas/cilogon-schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:16.099799 oauthenticator-16.0.3/oauthenticator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/oauthenticator/tests/test_openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:47:16.099799 oauthenticator-16.0.3/oauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 12:47:16.000000 oauthenticator-16.0.3/oauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:47:16.103799 oauthenticator-16.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-08 12:47:01.000000 oauthenticator-16.0.3/setup.py
```

### Comparing `oauthenticator-16.0.2/CONTRIBUTING.md` & `oauthenticator-16.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/LICENSE` & `oauthenticator-16.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/PKG-INFO` & `oauthenticator-16.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 16.0.2
+Version: 16.0.3
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `oauthenticator-16.0.2/README.md` & `oauthenticator-16.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/auth0.py` & `oauthenticator-16.0.3/oauthenticator/auth0.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/azuread.py` & `oauthenticator-16.0.3/oauthenticator/azuread.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/bitbucket.py` & `oauthenticator-16.0.3/oauthenticator/bitbucket.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/cilogon.py` & `oauthenticator-16.0.3/oauthenticator/cilogon.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/generic.py` & `oauthenticator-16.0.3/oauthenticator/generic.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/github.py` & `oauthenticator-16.0.3/oauthenticator/github.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/gitlab.py` & `oauthenticator-16.0.3/oauthenticator/gitlab.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/globus.py` & `oauthenticator-16.0.3/oauthenticator/globus.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/google.py` & `oauthenticator-16.0.3/oauthenticator/google.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/mediawiki.py` & `oauthenticator-16.0.3/oauthenticator/mediawiki.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/oauth2.py` & `oauthenticator-16.0.3/oauthenticator/oauth2.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/okpy.py` & `oauthenticator-16.0.3/oauthenticator/okpy.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/openshift.py` & `oauthenticator-16.0.3/oauthenticator/openshift.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/schemas/cilogon-schema.yaml` & `oauthenticator-16.0.3/oauthenticator/schemas/cilogon-schema.yaml`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/mocks.py` & `oauthenticator-16.0.3/oauthenticator/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_auth0.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_auth0.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_azuread.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_azuread.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_bitbucket.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_cilogon.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_cilogon.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_generic.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_github.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_gitlab.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_globus.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_globus.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_google.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_google.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_mediawiki.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_oauth2.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_okpy.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_okpy.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator/tests/test_openshift.py` & `oauthenticator-16.0.3/oauthenticator/tests/test_openshift.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator.egg-info/PKG-INFO` & `oauthenticator-16.0.3/oauthenticator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 16.0.2
+Version: 16.0.3
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `oauthenticator-16.0.2/oauthenticator.egg-info/SOURCES.txt` & `oauthenticator-16.0.3/oauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/oauthenticator.egg-info/entry_points.txt` & `oauthenticator-16.0.3/oauthenticator.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.2/pyproject.toml` & `oauthenticator-16.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/oauthenticator"
 
 [tool.tbump.version]
-current = "16.0.2"
+current = "16.0.3"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `oauthenticator-16.0.2/setup.py` & `oauthenticator-16.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "Aborting implicit building of eggs. Use `pip install .` to install from source."
         )
 
 
 setup_args = dict(
     name='oauthenticator',
     packages=find_packages(),
-    version="16.0.2",
+    version="16.0.3",
     description="OAuthenticator: Authenticate JupyterHub users with common OAuth providers",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jupyter Development Team",
     author_email="jupyter@googlegroups.com",
     url="https://jupyter.org",
     license="BSD",
```

