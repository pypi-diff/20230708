# Comparing `tmp/djaodjin-signup-0.8.2.tar.gz` & `tmp/djaodjin-signup-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-signup-0.8.2.tar", last modified: Thu May 18 23:23:16 2023, max compression
+gzip compressed data, was "djaodjin-signup-0.8.3.tar", last modified: Fri Jul  7 23:18:52 2023, max compression
```

## Comparing `djaodjin-signup-0.8.2.tar` & `djaodjin-signup-0.8.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.042556 djaodjin-signup-0.8.2/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-05-18 23:23:16.042625 djaodjin-signup-0.8.2/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2742 2023-04-21 22:41:35.000000 djaodjin-signup-0.8.2/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.023269 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2517 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      300 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     1951 2023-04-18 20:03:09.000000 djaodjin-signup-0.8.2/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-05-18 23:23:16.042836 djaodjin-signup-0.8.2/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 18:47:59.000000 djaodjin-signup-0.8.2/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.028587 djaodjin-signup-0.8.2/signup/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-05-18 23:22:28.000000 djaodjin-signup-0.8.2/signup/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.030221 djaodjin-signup-0.8.2/signup/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4728 2023-03-11 21:02:26.000000 djaodjin-signup-0.8.2/signup/api/activities.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12165 2023-04-18 21:49:58.000000 djaodjin-signup-0.8.2/signup/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.8.2/signup/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6122 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.8.2/signup/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)    33478 2023-05-18 20:21:41.000000 djaodjin-signup-0.8.2/signup/api/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2798 2023-01-21 18:23:23.000000 djaodjin-signup-0.8.2/signup/authentication.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.031460 djaodjin-signup-0.8.2/signup/backends/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/backends/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5598 2023-05-12 18:10:12.000000 djaodjin-signup-0.8.2/signup/backends/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6083 2023-05-12 22:39:02.000000 djaodjin-signup-0.8.2/signup/backends/auth_ldap.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2346 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/backends/mfa.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/backends/sts_credentials.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.8.2/signup/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10560 2023-05-12 20:52:33.000000 djaodjin-signup-0.8.2/signup/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12836 2023-04-08 20:24:46.000000 djaodjin-signup-0.8.2/signup/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17812 2023-05-12 21:32:45.000000 djaodjin-signup-0.8.2/signup/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3762 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.8.2/signup/middleware.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.033371 djaodjin-signup-0.8.2/signup/migrations/
--rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0001_v0_1_9.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0002_0_2_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0003_0_2_1.py
--rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0004_0_2_6.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0005_0_2_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4912 2023-04-14 19:44:41.000000 djaodjin-signup-0.8.2/signup/migrations/0006_v0_4_7.py
--rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.8.2/signup/migrations/0007_v0_4_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0008_v0_6_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1830 2023-04-14 20:13:48.000000 djaodjin-signup-0.8.2/signup/migrations/0009_v0_8_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    25217 2023-05-18 21:06:48.000000 djaodjin-signup-0.8.2/signup/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    36070 2023-05-18 20:39:54.000000 djaodjin-signup-0.8.2/signup/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9177 2023-04-12 16:28:00.000000 djaodjin-signup-0.8.2/signup/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7863 2022-09-12 17:12:06.000000 djaodjin-signup-0.8.2/signup/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6677 2023-05-08 17:19:44.000000 djaodjin-signup-0.8.2/signup/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1887 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.021050 djaodjin-signup-0.8.2/signup/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.034644 djaodjin-signup-0.8.2/signup/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    14494 2023-04-12 16:40:38.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-password-strength.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:46.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-angular.js
--rw-r--r--   0 smirolo    (501) staff       (20)    13054 2023-04-14 19:06:38.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-vue.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.021294 djaodjin-signup-0.8.2/signup/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.036411 djaodjin-signup-0.8.2/signup/templates/accounts/
--rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/disabled.html
--rw-r--r--   0 smirolo    (501) staff       (20)      775 2023-03-16 16:54:13.000000 djaodjin-signup-0.8.2/signup/templates/accounts/login.html
--rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/logout.html
--rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/recover.html
--rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/register.html
--rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/reset.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.037139 djaodjin-signup-0.8.2/signup/templates/notification/
--rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/password_reset.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/user_activated.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/user_registered.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/verification.eml
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.037848 djaodjin-signup-0.8.2/signup/templates/users/
--rw-r--r--   0 smirolo    (501) staff       (20)     1465 2023-03-02 23:05:43.000000 djaodjin-signup-0.8.2/signup/templates/users/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/users/notifications.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2856 2023-04-14 19:13:40.000000 djaodjin-signup-0.8.2/signup/templates/users/password.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1839 2023-02-15 21:47:15.000000 djaodjin-signup-0.8.2/signup/templates/users/pubkey.html
--rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/tests.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.038062 djaodjin-signup-0.8.2/signup/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1551 2023-02-14 15:00:54.000000 djaodjin-signup-0.8.2/signup/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.039838 djaodjin-signup-0.8.2/signup/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.8.2/signup/urls/api/activate.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1926 2023-03-08 02:03:00.000000 djaodjin-signup-0.8.2/signup/urls/api/activities.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1857 2023-03-02 05:24:17.000000 djaodjin-signup-0.8.2/signup/urls/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.8.2/signup/urls/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.8.2/signup/urls/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.8.2/signup/urls/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2165 2023-04-05 22:33:04.000000 djaodjin-signup-0.8.2/signup/urls/api/users.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.040894 djaodjin-signup-0.8.2/signup/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.8.2/signup/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2545 2023-03-02 05:23:57.000000 djaodjin-signup-0.8.2/signup/urls/views/accounts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1649 2023-03-04 00:46:08.000000 djaodjin-signup-0.8.2/signup/urls/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.8.2/signup/urls/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-04-05 22:31:53.000000 djaodjin-signup-0.8.2/signup/urls/views/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8894 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/utils.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4272 2023-02-15 03:45:50.000000 djaodjin-signup-0.8.2/signup/validators.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.042050 djaodjin-signup-0.8.2/signup/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    16462 2023-05-18 22:43:56.000000 djaodjin-signup-0.8.2/signup/views/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2739 2023-02-15 03:48:21.000000 djaodjin-signup-0.8.2/signup/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1903 2023-02-15 03:50:06.000000 djaodjin-signup-0.8.2/signup/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12802 2023-05-18 20:22:34.000000 djaodjin-signup-0.8.2/signup/views/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.380678 djaodjin-signup-0.8.3/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     3514 2023-07-07 23:18:52.380753 djaodjin-signup-0.8.3/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2718 2023-07-07 23:16:25.000000 djaodjin-signup-0.8.3/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.360493 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     3514 2023-07-07 23:18:52.000000 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2517 2023-07-07 23:18:52.000000 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-07-07 23:18:52.000000 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      300 2023-07-07 23:18:52.000000 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-07-07 23:18:52.000000 djaodjin-signup-0.8.3/djaodjin_signup.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1951 2023-04-18 20:03:09.000000 djaodjin-signup-0.8.3/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-07-07 23:18:52.380976 djaodjin-signup-0.8.3/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 18:47:59.000000 djaodjin-signup-0.8.3/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.366321 djaodjin-signup-0.8.3/signup/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-07-07 23:16:43.000000 djaodjin-signup-0.8.3/signup/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.368014 djaodjin-signup-0.8.3/signup/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4728 2023-03-11 21:02:26.000000 djaodjin-signup-0.8.3/signup/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14719 2023-07-07 23:17:45.000000 djaodjin-signup-0.8.3/signup/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.8.3/signup/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6122 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.3/signup/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.8.3/signup/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    33069 2023-06-24 06:47:07.000000 djaodjin-signup-0.8.3/signup/api/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2798 2023-01-21 18:23:23.000000 djaodjin-signup-0.8.3/signup/authentication.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.369538 djaodjin-signup-0.8.3/signup/backends/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/backends/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5598 2023-05-12 18:10:12.000000 djaodjin-signup-0.8.3/signup/backends/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6150 2023-05-19 00:11:20.000000 djaodjin-signup-0.8.3/signup/backends/auth_ldap.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2346 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.3/signup/backends/mfa.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/backends/sts_credentials.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.8.3/signup/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10554 2023-07-07 22:25:46.000000 djaodjin-signup-0.8.3/signup/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12836 2023-04-08 20:24:46.000000 djaodjin-signup-0.8.3/signup/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17732 2023-07-07 20:27:20.000000 djaodjin-signup-0.8.3/signup/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3762 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.3/signup/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.8.3/signup/middleware.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.371703 djaodjin-signup-0.8.3/signup/migrations/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0001_v0_1_9.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0002_0_2_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0003_0_2_1.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0004_0_2_6.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0005_0_2_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4912 2023-04-14 19:44:41.000000 djaodjin-signup-0.8.3/signup/migrations/0006_v0_4_7.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.8.3/signup/migrations/0007_v0_4_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/0008_v0_6_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1830 2023-04-14 20:13:48.000000 djaodjin-signup-0.8.3/signup/migrations/0009_v0_8_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/migrations/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    27368 2023-07-07 22:18:18.000000 djaodjin-signup-0.8.3/signup/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    36659 2023-07-07 21:18:39.000000 djaodjin-signup-0.8.3/signup/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9177 2023-04-12 16:28:00.000000 djaodjin-signup-0.8.3/signup/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8360 2023-06-01 11:49:28.000000 djaodjin-signup-0.8.3/signup/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6677 2023-05-08 17:19:44.000000 djaodjin-signup-0.8.3/signup/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1994 2023-06-01 09:42:06.000000 djaodjin-signup-0.8.3/signup/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.358444 djaodjin-signup-0.8.3/signup/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.373028 djaodjin-signup-0.8.3/signup/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    14494 2023-04-12 16:40:38.000000 djaodjin-signup-0.8.3/signup/static/js/djaodjin-password-strength.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:46.000000 djaodjin-signup-0.8.3/signup/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/static/js/djaodjin-signup-angular.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    13069 2023-07-07 22:23:54.000000 djaodjin-signup-0.8.3/signup/static/js/djaodjin-signup-vue.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.358701 djaodjin-signup-0.8.3/signup/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.374029 djaodjin-signup-0.8.3/signup/templates/accounts/
+-rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/accounts/disabled.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      775 2023-03-16 16:54:13.000000 djaodjin-signup-0.8.3/signup/templates/accounts/login.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/accounts/logout.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/accounts/recover.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/accounts/register.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/accounts/reset.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.374940 djaodjin-signup-0.8.3/signup/templates/notification/
+-rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/notification/password_reset.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/notification/user_activated.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/notification/user_registered.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/notification/verification.eml
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.375640 djaodjin-signup-0.8.3/signup/templates/users/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1465 2023-03-02 23:05:43.000000 djaodjin-signup-0.8.3/signup/templates/users/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/templates/users/notifications.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2856 2023-04-14 19:13:40.000000 djaodjin-signup-0.8.3/signup/templates/users/password.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1839 2023-02-15 21:47:15.000000 djaodjin-signup-0.8.3/signup/templates/users/pubkey.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/tests.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.375876 djaodjin-signup-0.8.3/signup/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1551 2023-02-14 15:00:54.000000 djaodjin-signup-0.8.3/signup/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.377714 djaodjin-signup-0.8.3/signup/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.8.3/signup/urls/api/activate.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1926 2023-03-08 02:03:00.000000 djaodjin-signup-0.8.3/signup/urls/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2041 2023-07-07 19:26:12.000000 djaodjin-signup-0.8.3/signup/urls/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.8.3/signup/urls/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.8.3/signup/urls/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.8.3/signup/urls/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2165 2023-04-05 22:33:04.000000 djaodjin-signup-0.8.3/signup/urls/api/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.378985 djaodjin-signup-0.8.3/signup/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.8.3/signup/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2738 2023-07-07 22:12:15.000000 djaodjin-signup-0.8.3/signup/urls/views/accounts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1649 2023-03-04 00:46:08.000000 djaodjin-signup-0.8.3/signup/urls/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.8.3/signup/urls/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-04-05 22:31:53.000000 djaodjin-signup-0.8.3/signup/urls/views/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8894 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.3/signup/utils.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4272 2023-02-15 03:45:50.000000 djaodjin-signup-0.8.3/signup/validators.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 23:18:52.380191 djaodjin-signup-0.8.3/signup/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.3/signup/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    16385 2023-07-07 22:38:52.000000 djaodjin-signup-0.8.3/signup/views/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2739 2023-02-15 03:48:21.000000 djaodjin-signup-0.8.3/signup/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1903 2023-02-15 03:50:06.000000 djaodjin-signup-0.8.3/signup/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12802 2023-05-18 20:22:34.000000 djaodjin-signup-0.8.3/signup/views/users.py
```

### Comparing `djaodjin-signup-0.8.2/LICENSE.txt` & `djaodjin-signup-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/PKG-INFO` & `djaodjin-signup-0.8.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.8.2
+Version: 0.8.3
 Summary: Django app for user authentication
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
 Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
@@ -82,22 +82,19 @@
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
 Tested with
 
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.8.1
+0.8.3
 
-  * fixes regression handling auth URLs with extra characters
-
-0.8.0
-
-  * publishes distribution using pyproject.toml
-  * enables/disables OTP 2FA through user profile
-  * moves API keys to their own page
+  * removes connection btw user and contact on delete
+  * fixes activation with e-mail that looks like a bot
+  * verifies and activates contact with no user
+  * restores workflow to recover password from an e-mail
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.8.2/README.md` & `djaodjin-signup-0.8.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -62,22 +62,19 @@
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
 Tested with
 
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.8.1
+0.8.3
 
-  * fixes regression handling auth URLs with extra characters
-
-0.8.0
-
-  * publishes distribution using pyproject.toml
-  * enables/disables OTP 2FA through user profile
-  * moves API keys to their own page
+  * removes connection btw user and contact on delete
+  * fixes activation with e-mail that looks like a bot
+  * verifies and activates contact with no user
+  * restores workflow to recover password from an e-mail
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.8.2/djaodjin_signup.egg-info/PKG-INFO` & `djaodjin-signup-0.8.3/djaodjin_signup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.8.2
+Version: 0.8.3
 Summary: Django app for user authentication
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
 Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
@@ -82,22 +82,19 @@
     # Browse http://localhost:8000/
 
 Release Notes
 =============
 
 Tested with
 
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest) - see [#55](https://github.com/djaodjin/djaodjin-signup/issues/55)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.8.1
+0.8.3
 
-  * fixes regression handling auth URLs with extra characters
-
-0.8.0
-
-  * publishes distribution using pyproject.toml
-  * enables/disables OTP 2FA through user profile
-  * moves API keys to their own page
+  * removes connection btw user and contact on delete
+  * fixes activation with e-mail that looks like a bot
+  * verifies and activates contact with no user
+  * restores workflow to recover password from an e-mail
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-signup-0.8.2/djaodjin_signup.egg-info/SOURCES.txt` & `djaodjin-signup-0.8.3/djaodjin_signup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/pyproject.toml` & `djaodjin-signup-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/setup.py` & `djaodjin-signup-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/__init__.py` & `djaodjin-signup-0.8.3/signup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the signup django app.
 """
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
```

### Comparing `djaodjin-signup-0.8.2/signup/api/activities.py` & `djaodjin-signup-0.8.3/signup/api/activities.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/api/auth.py` & `djaodjin-signup-0.8.3/signup/api/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 from rest_framework.response import Response
 
 
 from .. import settings
 from ..compat import gettext_lazy as _
 from ..docs import OpenAPIResponse, no_body, swagger_auto_schema
 from ..helpers import as_timestamp, datetime_or_now
-from ..mixins import (LoginMixin, RegisterMixin, VerifyMixin,
-    VerifyCompleteMixin, SSORequired)
+from ..mixins import (LoginMixin, PasswordResetConfirmMixin, RegisterMixin,
+    VerifyMixin, VerifyCompleteMixin, SSORequired)
 from ..models import Contact
 from ..serializers_overrides import UserDetailSerializer
 from ..serializers import (CredentialsSerializer,
     RecoverSerializer, TokenSerializer, UserActivateSerializer,
     UserCreateSerializer, ValidationErrorSerializer)
 from ..utils import get_disabled_registration
 
@@ -200,15 +200,15 @@
                     'provider': err.printable_name},
                     'provider': err.delegate_auth.provider,
                     'url': self.request.build_absolute_uri(err.url)})
 
         raise serializers.ValidationError({'detail': "invalid request"})
 
 
-class JWTActivate(VerifyCompleteMixin, JWTRegister):
+class JWTActivate(VerifyCompleteMixin, JWTBase):
     """
     Retrieves an activation key
 
     This API is typically used to pre-populate a registration form
     when a user was invited to the site by another user.
 
     The response is usually presented in an HTML
@@ -233,14 +233,15 @@
           "username": "joe1",
           "email": "joe1@localhost.localdomain",
           "full_name": "Joe Act",
           "printable_name": "Joe Act",
           "created_at": "2020-05-30T00:00:00Z"
         }
     """
+    model = get_user_model()
     serializer_class = UserActivateSerializer
 
     def get_serializer_class(self):
         if self.request.method.lower() == 'get':
             return  UserDetailSerializer
         return super(JWTActivate, self).get_serializer_class()
 
@@ -287,16 +288,101 @@
             {
                 "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
     ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
     SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
     JwcBUUMECj8AKxsHtRHUSypco"
             }
         """
-        return super(JWTActivate, self).post(request, *args, **kwargs)
+        try:
+            user_with_backend = self.run_pipeline()
+            return self.create_token(user_with_backend)
+        except SSORequired as err:
+            raise serializers.ValidationError({'detail': _(
+                "SSO required through %(provider)s") % {
+                    'provider': err.printable_name},
+                    'provider': err.delegate_auth.provider,
+                    'url': self.request.build_absolute_uri(err.url)})
+
+        raise serializers.ValidationError({'detail': "invalid request"})
+
+
+class JWTPasswordConfirm(PasswordResetConfirmMixin, JWTActivate):
+    """
+    Resets user password
+
+    This API resets a user password, hence triggering an activation
+    workflow.
+
+    The response is usually presented in an HTML
+    `activate page </docs/guides/themes/#workflow_activate>`_
+    as present in the default theme.
 
+    **Tags: auth, visitor, usermodel
+
+    **Example
+
+    .. code-block:: http
+
+        GET /api/auth/reset/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
+ HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+        {
+          "slug": "joe1",
+          "username": "joe1",
+          "email": "joe1@localhost.localdomain",
+          "full_name": "Joe Act",
+          "printable_name": "Joe Act",
+          "created_at": "2020-05-30T00:00:00Z"
+        }
+    """
+
+    @swagger_auto_schema(responses={
+        201: OpenAPIResponse("", TokenSerializer),
+        400: OpenAPIResponse("parameters error", ValidationErrorSerializer)})
+    def post(self, request, *args, **kwargs):#pylint:disable=unused-argument
+        """
+        Enters a new password after a reset
+
+        Activates a new user and returns a JSON Web Token that can subsequently
+        be used to authenticate the new user in HTTP requests.
+
+        **Tags: auth, visitor, usermodel
+
+        **Example
+
+        .. code-block:: http
+
+            POST /api/auth/reset/16793aa72a4c7ae94b50b20c2eca52df5b0fe2c6\
+ HTTP/1.1
+
+        .. code-block:: json
+
+            {
+              "username": "joe1",
+              "email": "joe1@locahost.localdomain",
+              "new_password": "yoyo",
+              "full_name": "Joe Card1"
+            }
+
+        responds
+
+        .. code-block:: json
+
+            {
+                "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VybmFtZSI6\
+    ImpvZTEiLCJlbWFpbCI6ImpvZSsxQGRqYW9kamluLmNvbSIsImZ1bGxfbmFtZ\
+    SI6IkpvZSAgQ2FyZDEiLCJleHAiOjE1Mjk2NTUyMjR9.GFxjU5AvcCQbVylF1P\
+    JwcBUUMECj8AKxsHtRHUSypco"
+            }
+        """
+        return super(JWTPasswordConfirm, self).post(request, *args, **kwargs)
 
 class JWTLogout(JWTBase):
     """
     Logs a user out
 
     Removes all cookies associated with the session.
```

### Comparing `djaodjin-signup-0.8.2/signup/api/contacts.py` & `djaodjin-signup-0.8.3/signup/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/api/keys.py` & `djaodjin-signup-0.8.3/signup/api/keys.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/api/tokens.py` & `djaodjin-signup-0.8.3/signup/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/api/users.py` & `djaodjin-signup-0.8.3/signup/api/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from ..mixins import ContactMixin, UserMixin
 from ..models import (Contact, Credentials, Notification, OTPGenerator,
     get_disabled_email_update)
 from ..serializers_overrides import UserSerializer, UserDetailSerializer
 from ..serializers import (OTPSerializer, OTPUpdateSerializer,
     PasswordChangeSerializer, NotificationsSerializer, UploadBlobSerializer,
     UserCreateSerializer, ValidationErrorSerializer)
-from ..utils import generate_random_code, get_picture_storage, handle_uniq_error
+from ..utils import get_picture_storage, handle_uniq_error
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_order_func(fields):
     """
@@ -274,64 +274,53 @@
 
             DELETE /api/users/xia HTTP/1.1
         """
         return self.destroy(request, *args, **kwargs)
 
     def perform_destroy(self, instance):
         user = instance
-        pkid = user.pk if user.pk else generate_random_code()
         email = user.email
         username = user.username
-
-        # We mark the user as inactive and scramble personal information
-        # such that we don't remove audit records (ex: billing transactions)
-        # from the database.
-        slug = '_archive_%d' % pkid
-        LOGGER.info("%s deleted user profile for '%s <%s>' (%s).",
-            self.request.user, username, email, slug, extra={'event': 'delete',
-                'request': self.request, 'username': username, 'email': email,
-                'pk': pkid})
-
-        look = re.match(r'.*(@\S+)', settings.DEFAULT_FROM_EMAIL)
-        if look:
-            email = '%s%s' % (slug, look.group(1))
-
-        with transaction.atomic():
-            contacts = list((user.contacts.all() if user.pk
-                else Contact.objects.filter(
-                        slug=self.kwargs.get(self.lookup_url_kwarg))))
-            if contacts:
-                for contact in contacts:
-                    contact.email = None
-                    contact.phone = None
-                    contact.full_name = ""
-                    contact.nick_name = ""
-                    contact.picture = ""
-                    contact.email_verification_key = None
-                    contact.email_verification_at = None
-                    contact.email_verified_at = None
-                    contact.phone_verification_key = None
-                    contact.phone_verification_at = None
-                    contact.phone_verified_at = None
-                    contact.one_time_code = None
-                Contact.objects.bulk_update(contacts, [
-                    'email', 'phone', 'full_name', 'nick_name', 'picture',
-                    'email_verification_key', 'email_verification_at',
-                    'email_verified_at', 'phone_verification_key',
-                    'phone_verification_at', 'one_time_code'])
-            if user.pk:
+        if user.pk:
+            # We mark the user as inactive and scramble personal information
+            # such that we don't remove audit records (ex: billing transactions)
+            # from the database.
+            pkid = user.pk
+            slug = '_archive_%d' % pkid
+            LOGGER.info("%s deleted user profile for '%s <%s>' (%s).",
+                self.request.user, username, email, slug, extra={
+                    'event': 'delete', 'request': self.request,
+                    'username': username, 'email': email, 'pk': pkid})
+            look = re.match(r'.*(@\S+)', settings.DEFAULT_FROM_EMAIL)
+            if look:
+                email = '%s%s' % (slug, look.group(1))
+            # We are deleting a `User` model. Let's unlink the `Contact`
+            # info but otherwise leave the poor-man's CRM's data intact.
+            with transaction.atomic():
+                user.contacts.all().update(user=None)
                 self.delete_records(user)
                 requires_logout = (self.request.user == user)
                 user.username = slug
                 user.email = email
                 user.password = '!'
                 user.is_active = False
                 user.save()
                 if requires_logout:
                     auth_logout(self.request)
+        else:
+            contacts = Contact.objects.filter(
+                slug=self.kwargs.get(self.lookup_url_kwarg))
+            if contacts:
+                for contact in contacts:
+                    LOGGER.info("%s deleted contact for '%s <%s>'.",
+                        self.request.user, contact.full_name, contact.email,
+                        extra={'event': 'delete', 'request': self.request,
+                            'full_name': contact.full_name,
+                            'email': contact.email, 'pk': contact.pk})
+                contacts.delete()
 
     def delete_records(self, user):
         user.notifications.all().delete()
         if Credentials.objects.filter(user=user).exists():
             user.credentials.delete()
```

### Comparing `djaodjin-signup-0.8.2/signup/auth.py` & `djaodjin-signup-0.8.3/signup/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/authentication.py` & `djaodjin-signup-0.8.3/signup/authentication.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/backends/auth.py` & `djaodjin-signup-0.8.3/signup/backends/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/backends/auth_ldap.py` & `djaodjin-signup-0.8.3/signup/backends/auth_ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     """
     model = get_user_model()
 
     def authenticate(self, request, username=None, password=None, **kwargs):
         #pylint:disable=unused-argument
         user = None
         bind_dn = _get_bind_dn(username)
+        ldap_connection = None
         try:
             ldap_connection = ldap.initialize(
                 settings.LDAP_SERVER_URI, bytes_mode=False)
             ldap_connection.simple_bind_s(
                 force_str(bind_dn), force_str(password))
 
             resp = ldap_connection.search_s(
@@ -149,15 +150,16 @@
             })
             if created:
                 LOGGER.debug("created user '%s' in database.", username)
             user = db_user
         except ldap.LDAPError: #pylint:disable=no-member
             user = None
         finally:
-            ldap_connection.unbind_s()
+            if ldap_connection:
+                ldap_connection.unbind_s()
 
         return user
 
     def get_user(self, user_id):
         try:
             user = self.model.objects.get(pk=user_id)
             return user
```

### Comparing `djaodjin-signup-0.8.2/signup/backends/mfa.py` & `djaodjin-signup-0.8.3/signup/backends/mfa.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/backends/sts_credentials.py` & `djaodjin-signup-0.8.3/signup/backends/sts_credentials.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/compat.py` & `djaodjin-signup-0.8.3/signup/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/decorators.py` & `djaodjin-signup-0.8.3/signup/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -26,15 +26,15 @@
 Decorators that check a User a verified email address.
 """
 from __future__ import unicode_literals
 
 from functools import wraps
 
 from django.contrib import messages
-from django.contrib.auth import (REDIRECT_FIELD_NAME, logout as auth_logout)
+from django.contrib.auth import REDIRECT_FIELD_NAME, logout as auth_logout
 from django.contrib.auth.views import redirect_to_login
 from django.core.exceptions import PermissionDenied
 
 from . import settings, signals
 from .auth import validate_redirect
 from .compat import (available_attrs, gettext_lazy as _, is_authenticated,
     reverse, six)
@@ -83,15 +83,15 @@
     workflow once verification is completed.
     """
     back_url = request.build_absolute_uri(reverse('registration_activate',
         args=(contact.email_verification_key,)))
     if next_url:
         back_url += '?%s=%s' % (redirect_field_name, next_url)
     signals.user_verification.send(
-        sender=__name__, user=contact.user, request=request,
+        sender=__name__, user=contact, request=request,
         back_url=back_url, expiration_days=settings.KEY_EXPIRATION)
 
 
 def send_verification_phone(contact, request,
                            next_url=None,
                            redirect_field_name=REDIRECT_FIELD_NAME):
     """
@@ -102,16 +102,16 @@
     workflow once verification is completed.
     """
     # XXX needs to send phone text message instead of e-mail!!!
     back_url = request.build_absolute_uri(reverse('registration_activate',
         args=(contact.phone_verification_key,)))
     if next_url:
         back_url += '?%s=%s' % (redirect_field_name, next_url)
-    signals.user_verification.send(
-        sender=__name__, user=contact.user, request=request,
+    signals.user_phone_verification.send(
+        sender=__name__, user=contact, request=request,
         back_url=back_url, expiration_days=settings.KEY_EXPIRATION)
 
 
 # The user we are looking to activate might be different from
 # the request.user (which can be Anonymous)
 def check_has_credentials(request, user,
                           redirect_field_name=REDIRECT_FIELD_NAME,
```

### Comparing `djaodjin-signup-0.8.2/signup/docs.py` & `djaodjin-signup-0.8.3/signup/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/filters.py` & `djaodjin-signup-0.8.3/signup/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/forms.py` & `djaodjin-signup-0.8.3/signup/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,14 @@
 from . import settings, validators
 from .compat import gettext_lazy as _, six
 from .helpers import full_name_natural_split
 from .models import get_disabled_email_update
 from .utils import get_recaptcha_form_field
 
 
-class EmailField(forms.EmailField):
-
-    default_validators = [validators.validate_email]
-
-
 class PhoneField(PhoneNumberField):
 
     def __init__(self, *args, **kwargs):
         region = kwargs.get('region')
         if not region:
             params = {'region': 'US'}
             params.update(kwargs)
@@ -88,15 +83,15 @@
 
 class FrictionlessSignupForm(forms.Form):
     """
     Form for frictionless registration of a new user. Just supply
     a full name and a way to notify user (email or phone) and you are in.
     We will ask for username and password later.
     """
-    email = EmailField(label=_("E-mail address"), required=False,
+    email = forms.EmailField(label=_("E-mail address"), required=False,
         widget=forms.TextInput(attrs={'placeholder': _("E-mail")}))
     phone = PhoneField(required=False)
     full_name = forms.RegexField(
         regex=settings.FULL_NAME_PAT, max_length=60,
         widget=forms.TextInput(attrs={
             'placeholder': 'Ex: first name and last name'}),
         label=_("Full name"),
@@ -216,25 +211,14 @@
         widget=forms.PasswordInput(
             attrs={'placeholder': _("Type password again")}))
 
     class Meta:
         model = get_user_model()
         fields = ['new_password', 'new_password2']
 
-    def __init__(self, *args, **kwargs):
-        self.user = kwargs.pop('instance')
-        super(PasswordUpdateForm, self).__init__(*args, **kwargs)
-
-    def save(self, commit=True):
-        new_password = self.cleaned_data['new_password']
-        self.user.set_password(new_password)
-        if commit:
-            self.user.save()
-        return self.user
-
 
 class PasswordResetConfirmForm(PasswordUpdateForm):
     """
     Form displayed when a user clicked on the link sent in the reset e-mail.
     """
 
 
@@ -245,14 +229,25 @@
         widget=forms.PasswordInput(
             attrs={'placeholder': _("Your password")}))
 
     class Meta:
         model = get_user_model()
         fields = ['password', 'new_password', 'new_password2']
 
+    def __init__(self, *args, **kwargs):
+        self.user = kwargs.pop('instance')
+        super(PasswordUpdateForm, self).__init__(*args, **kwargs)
+
+    def save(self, commit=True):
+        new_password = self.cleaned_data['new_password']
+        self.user.set_password(new_password)
+        if commit:
+            self.user.save()
+        return self.user
+
 
 class RecoverForm(forms.Form):
     """
     Form displayed to authenticate through a verification link.
     """
     username = UsernameOrCommField()
 
@@ -265,15 +260,15 @@
     submit_title = _("Activate")
 
     error_messages = {
         'password_mismatch': _("Password and password confirmation"\
         " do not match."),
     }
 
-    email = EmailField(label=_("E-mail address"), required=False)
+    email = forms.EmailField(label=_("E-mail address"), required=False)
     phone = PhoneField(label=_("Phone number"), required=False)
     full_name = forms.RegexField(
         regex=r'^[\w\s]+$', max_length=60,
         widget=forms.TextInput(attrs={'placeholder':'Full name'}),
         label=_("Full name"),
         error_messages={'invalid':
             _("Sorry we do not recognize some characters in your full name.")})
```

### Comparing `djaodjin-signup-0.8.2/signup/helpers.py` & `djaodjin-signup-0.8.3/signup/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/middleware.py` & `djaodjin-signup-0.8.3/signup/middleware.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0001_v0_1_9.py` & `djaodjin-signup-0.8.3/signup/migrations/0001_v0_1_9.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0002_0_2_0.py` & `djaodjin-signup-0.8.3/signup/migrations/0002_0_2_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0003_0_2_1.py` & `djaodjin-signup-0.8.3/signup/migrations/0003_0_2_1.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0004_0_2_6.py` & `djaodjin-signup-0.8.3/signup/migrations/0004_0_2_6.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0005_0_2_8.py` & `djaodjin-signup-0.8.3/signup/migrations/0005_0_2_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0006_v0_4_7.py` & `djaodjin-signup-0.8.3/signup/migrations/0006_v0_4_7.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0007_v0_4_8.py` & `djaodjin-signup-0.8.3/signup/migrations/0007_v0_4_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0008_v0_6_0.py` & `djaodjin-signup-0.8.3/signup/migrations/0008_v0_6_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/migrations/0009_v0_8_0.py` & `djaodjin-signup-0.8.3/signup/migrations/0009_v0_8_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/mixins.py` & `djaodjin-signup-0.8.3/signup/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging, re
 
 from django.http import Http404
-from django.contrib.auth import (authenticate,
+from django.contrib.auth import (REDIRECT_FIELD_NAME, authenticate,
     get_user_model, login as auth_login)
 from django.db import IntegrityError
 from django.utils import translation
 from django.utils.http import urlencode
 from rest_framework import exceptions, serializers
 from rest_framework.generics import get_object_or_404
 
 from . import signals, settings
+from .auth import validate_redirect
 from .compat import gettext_lazy as _, is_authenticated, reverse, six
 from .decorators import send_verification_email, send_verification_phone
 from .helpers import (full_name_natural_split, has_invalid_password,
     update_context_urls)
 from .models import Contact, DelegateAuth, OTPGenerator
 from .utils import (get_disabled_authentication, get_disabled_registration,
     get_email_dynamic_validator, get_login_throttle, handle_uniq_error)
@@ -131,14 +132,15 @@
         # example because there is a `action="."` in the <form> tag
         # in login.html.
         # We cannot catch these by restricting the match pattern.
         # 1. '^login/$' will not match 'login/.' hence trigger the catch
         #    all pattern that might forward the HTTP request.
         # 2. 'login/(?P<extra>.*)' will through a missing argument
         #    exception in `reverse` calls.
+        #pylint:disable=too-many-locals
         try:
             pat = (r'(?P<expected_path>%s)(?P<extra>.*)' %
                 self.request.resolver_match.route)
             look = re.match(pat, self.request.path.lstrip('/'))
             if look:
                 expected_path = '/' + look.group('expected_path')
                 extra =  look.group('extra')
@@ -160,15 +162,17 @@
             if self.request.method.lower() in ('post',):
                 if not form.is_valid():
                     raise serializers.ValidationError()
                 for field_name in six.iterkeys(form.data):
                     cleaned_data.update({
                         field_name: form.cleaned_data.get(
                             field_name, form.data[field_name])})
-            cleaned_data.update({'next_url': self.get_success_url()})
+            next_url = validate_redirect(self.request)
+            if next_url:
+                cleaned_data.update({'next_url': next_url})
         elif self.serializer_class is not None:
             data = initial_data.copy()
             data.update(self.request.data)
             serializer = self.get_serializer(data=data)
             serializer.is_valid(raise_exception=True)
             for field_name in six.iterkeys(data):
                 if field_name == 'phone':
@@ -358,27 +362,51 @@
 
         raise serializers.ValidationError({
             'detail': _("Credentials do not match.")})
 
 
 class VerifyMixin(AuthMixin):
     """
-    Authenticate by verifying e-mail or phone
+    Authenticate by verifying e-mail address
     """
+    pattern_name = 'registration_activate'
+
+    def get_query_param(self, request, key, default_value=None):
+        try:
+            return request.query_params.get(key, default_value)
+        except AttributeError:
+            pass
+        return request.GET.get(key, default_value)
+
+    def send_notification_email(self, contact, next_url=None):
+        request = self.request
+        if self.get_query_param(request, 'noreset'):
+            send_verification_email(contact, request, next_url=next_url)
+        else:
+            back_url = request.build_absolute_uri(
+                reverse('password_reset_confirm', args=(
+                    contact.email_verification_key,)))
+            if next_url:
+                back_url += '?%s=%s' % (REDIRECT_FIELD_NAME, next_url)
+            signals.user_reset_password.send(
+                sender=__name__, user=contact, request=request,
+                back_url=back_url, expiration_days=settings.KEY_EXPIRATION)
+
+
     def check_password(self, user, **cleaned_data):
         next_url = cleaned_data.get('next_url')
         email = cleaned_data.get('email')
         if not email:
             email = user.email
         # send link through e-mail
         if email:
             #pylint:disable=unused-variable
             contact, unused = Contact.objects.prepare_email_verification(
                 email, user=user)
-            send_verification_email(contact, self.request, next_url=next_url)
+            self.send_notification_email(contact, next_url=next_url)
             raise VerifyRequired({'detail': _(
                     "We sent a one-time link to your e-mail address.")})
 
         raise serializers.ValidationError({
             'detail': _("Credentials do not match.")})
 
 
@@ -468,14 +496,22 @@
                     user_extra.update({field_name[5:]: field_value})
         if not user_extra:
             user_extra = None
         user = self.model.objects.create_user(username,
             email=email, password=password, phone=phone,
             first_name=first_name, last_name=last_name,
             lang=lang, extra=user_extra)
+
+        LOGGER.info("'%s <%s>' registered with username '%s'%s%s",
+            user.get_full_name(), user.email, user,
+            (" and phone %s" % str(phone)) if phone else "",
+            (" and preferred language %s" % str(lang)) if lang else "",
+            extra={'event': 'register', 'user': user})
+        signals.user_registered.send(sender=__name__, user=user)
+
         # Bypassing authentication here, we are doing frictionless registration
         # the first time around.
         user.backend = self.backend_path
         return user
 
 
 class VerifyCompleteMixin(AuthMixin):
@@ -489,17 +525,18 @@
         if contact:
             fields = []
             if self.form_class is not None:
                 fields = six.iterkeys(self.get_initial())
             elif self.serializer_class is not None:
                 fields = self.serializer_class.Meta.fields
             for field_name in fields:
-                field_value = getattr(contact, field_name, None)
-                if not field_value and contact.user:
+                if contact.user:
                     field_value = getattr(contact.user, field_name, None)
+                if not field_value:
+                    field_value = getattr(contact, field_name, None)
                 if field_value:
                     data.update({field_name: field_value})
         return data
 
     def find_candidate(self, **cleaned_data):
         verification_key = self.kwargs.get(self.key_url_kwarg)
         contact = Contact.objects.get_token(verification_key)
@@ -539,33 +576,50 @@
                 password=cleaned_data.get('new_password'),
                 full_name=full_name)
         except IntegrityError as err:
             handle_uniq_error(err)
 
         if user:
             if not user.last_login:
-                # XXX copy/paste from models.ActivatedUserManager.create_user
-                LOGGER.info("'%s %s <%s>' registered with username '%s'",
-                    user.first_name, user.last_name, user.email, user,
+                phone = user.get_phone()
+                lang = user.get_lang()
+                LOGGER.info("'%s <%s>' registered with username '%s'%s%s",
+                    user.get_full_name(), user.email, user,
+                    (" and phone %s" % str(phone)) if phone else "",
+                    (" and preferred language %s" % str(lang)) if lang else "",
                     extra={'event': 'register', 'user': user})
                 signals.user_registered.send(sender=__name__, user=user)
             elif previously_inactive:
-                LOGGER.info("'%s %s <%s>' activated with username '%s'",
-                    user.first_name, user.last_name, user.email, user,
+                LOGGER.info("'%s <%s>' activated with username '%s'",
+                    user.get_full_name(), user.email, user,
                     extra={'event': 'activate', 'user': user})
                 signals.user_activated.send(sender=__name__, user=user,
                     verification_key=self.kwargs.get(self.key_url_kwarg),
                     request=self.request)
 
         # Bypassing authentication here, we are doing frictionless registration
         # the first time around.
         user.backend = self.backend_path
         return user
 
 
+class PasswordResetConfirmMixin(VerifyCompleteMixin):
+
+    def check_password(self, user, **cleaned_data):
+        #pylint:disable=unused-argument
+        if self.request.method.lower() == 'get':
+            if user:
+                user.password = '!'
+                user.save()
+            if not user or has_invalid_password(user):
+                raise IncorrectUser({'email': _("Not found.")})
+        return super(PasswordResetConfirmMixin, self).check_password(
+            user, **cleaned_data)
+
+
 class ContactMixin(settings.EXTRA_MIXIN):
 
     lookup_field = 'slug'
     lookup_url_kwarg = 'user'
     user_queryset = get_user_model().objects.filter(is_active=True)
 
     @property
```

### Comparing `djaodjin-signup-0.8.2/signup/models.py` & `djaodjin-signup-0.8.3/signup/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from django.contrib.auth.models import UserManager
 from django.db import models, transaction, IntegrityError
 from django.template.defaultfilters import slugify
 from django.contrib.auth.hashers import check_password, make_password
 from phonenumber_field.modelfields import PhoneNumberField
 from rest_framework.exceptions import ValidationError as DRFValidationError
 
-from . import settings, signals
+from . import settings
 from .backends.auth_ldap import is_ldap_user
 from .backends.mfa import EmailOTCBackend, PhoneOTCBackend
 from .compat import (gettext_lazy as _, import_string,
     python_2_unicode_compatible, six)
 from .helpers import (datetime_or_now, full_name_natural_split,
     has_invalid_password)
 from .utils import generate_random_slug, handle_uniq_error
@@ -223,20 +223,14 @@
             elif phone:
                 # Force is_active to True and create an email verification key
                 # (see above definition of active user).
                 Contact.objects.prepare_phone_verification(phone,
                     user=user, email=email, lang=lang, extra=extra)
             user.is_active = True
             user.save()
-            LOGGER.info("'%s <%s>' registered with username '%s'%s%s",
-                user.get_full_name(), user.email, user,
-                (" and phone %s" % str(phone)) if phone else "",
-                (" and preferred language %s" % str(lang)) if lang else "",
-                extra={'event': 'register', 'user': user})
-            signals.user_registered.send(sender=__name__, user=user)
         return user
 
     def find_user(self, username):
         user_kwargs = {}
         contact_kwargs = {}
         username = str(username) # We could have a ``PhoneNumber`` here.
         try:
@@ -440,29 +434,40 @@
         Activate a user whose email address has been verified.
         """
         #pylint:disable=too-many-arguments
         at_time = datetime_or_now()
         try:
             token = self.get_token(verification_key=verification_key)
             if token:
+                token_username = (
+                    token.user.username if token.user else token.slug)
                 LOGGER.info('active user %s through code: %s ...',
-                    token.user, verification_key,
-                    extra={'event': 'activate', 'username': token.user.username,
+                    token_username, verification_key,
+                    extra={'event': 'activate', 'username': token_username,
                         'verification_key': verification_key,
                         'email_verification_key': token.email_verification_key,
                         'phone_verification_key': token.phone_verification_key})
-                previously_inactive = has_invalid_password(token.user)
+                user_model = get_user_model()
                 with transaction.atomic():
                     if token.email_verification_key == verification_key:
                         token.email_verification_key = None
                         token.email_verified_at = at_time
                     elif token.phone_verification_key == verification_key:
                         token.phone_verification_key = None
                         token.phone_verified_at = at_time
+                    if not token.user:
+                        try:
+                            token.user = user_model.objects.get(
+                                email__iexact=token.email)
+                        except user_model.DoesNotExist:
+                            token.user = user_model.objects.create_user(
+                                username, email=token.email,
+                                password=password)
                     token.save()
+                    previously_inactive = has_invalid_password(token.user)
                     needs_save = False
                     if full_name:
                         token.full_name = full_name
                         #pylint:disable=unused-variable
                         first_name, mid_name, last_name = \
                             full_name_natural_split(full_name)
                         token.user.first_name = first_name
@@ -580,21 +585,41 @@
         return str(self.slug)
 
     @property
     def username(self):
         return self.slug
 
     @property
+    def date_joined(self):
+        return self.created_at
+
+    @property
     def printable_name(self):
         if self.nick_name:
             return self.nick_name
         if self.full_name:
             return self.full_name
         return self.username
 
+    def get_full_name(self):
+        return self.full_name
+
+    def get_nick_name(self):
+        if self.nick_name:
+            return self.nick_name
+        if self.user:
+            return self.user.first_name
+        return ""
+
+    def get_phone(self):
+        return self.phone
+
+    def get_lang(self):
+        return self.lang
+
     def get_otc_backend(self):
         if self.otc_backend == self.EMAIL_BACKEND:
             return EmailOTCBackend()
         if self.otc_backend == self.PHONE_BACKEND:
             return PhoneOTCBackend()
         return None
```

### Comparing `djaodjin-signup-0.8.2/signup/serializers.py` & `djaodjin-signup-0.8.3/signup/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/serializers_overrides.py` & `djaodjin-signup-0.8.3/signup/serializers_overrides.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,26 +118,34 @@
     @staticmethod
     def get_printable_name(obj):
         printable_name = None
         if hasattr(obj, 'nick_name'):
             printable_name = obj.nick_name
         if printable_name:
             return printable_name
-        opk = obj.pk if hasattr(obj, 'pk') else None
-        if opk:
-            contact = obj.contacts.filter(nick_name__isnull=False).order_by(
-                'created_at').first()
-            if contact:
-                printable_name = contact.nick_name
+        if hasattr(obj, 'full_name'):
+            printable_name = obj.full_name
         if printable_name:
             return printable_name
-        printable_name = obj.get_full_name()
-        if printable_name:
-            return printable_name
-        return obj.username
+        if isinstance(obj, get_user_model()):
+            opk = obj.pk if hasattr(obj, 'pk') else None
+            if opk:
+                contact = obj.contacts.filter(nick_name__isnull=False).order_by(
+                    'created_at').first()
+                if contact:
+                    printable_name = contact.nick_name
+            if printable_name:
+                return printable_name
+            printable_name = obj.get_full_name()
+            if printable_name:
+                return printable_name
+            return obj.username
+        if hasattr(obj, 'slug'):
+            printable_name = obj.slug
+        return printable_name
 
 
 class UserDetailSerializer(UserSerializer):
     """
     This serializer is used in APIs where a single Contact/User
     profile is returned.
 
@@ -182,8 +190,11 @@
         fields = UserSerializer.Meta.fields + ('email', 'phone',
             'full_name', 'nick_name', 'lang',
             'credentials', 'created_at', 'last_login')
         read_only_fields = ('credentials', 'created_at', 'last_login')
 
     @staticmethod
     def get_credentials(obj):
-        return hasattr(obj, 'pk') and (not has_invalid_password(obj))
+        return ((isinstance(obj, get_user_model()) and
+            hasattr(obj, 'pk') and (not has_invalid_password(obj))) or
+            hasattr(obj, 'user') and obj.user and
+                (not has_invalid_password(obj.user)))
```

### Comparing `djaodjin-signup-0.8.2/signup/settings.py` & `djaodjin-signup-0.8.3/signup/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/signals.py` & `djaodjin-signup-0.8.3/signup/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,13 +34,16 @@
 )
 user_activated = Signal(
 #    providing_args=['user', 'verification_key', 'request']
 )
 user_verification = Signal(
 #    providing_args=['user', 'request', 'back_url', 'expiration_days']
 )
+user_phone_verification = Signal(
+#    providing_args=['user', 'request', 'back_url', 'expiration_days']
+)
 user_reset_password = Signal(
 #    providing_args=['user', 'request', 'back_url', 'expiration_days']
 )
 user_mfa_code = Signal(
 #    providing_args=['user', 'code', 'request']
 )
```

### Comparing `djaodjin-signup-0.8.2/signup/static/js/djaodjin-password-strength.js` & `djaodjin-signup-0.8.3/signup/static/js/djaodjin-password-strength.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources-vue.js` & `djaodjin-signup-0.8.3/signup/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources.js` & `djaodjin-signup-0.8.3/signup/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-angular.js` & `djaodjin-signup-0.8.3/signup/static/js/djaodjin-signup-angular.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-vue.js` & `djaodjin-signup-0.8.3/signup/static/js/djaodjin-signup-vue.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -130,15 +130,15 @@
 
 Vue.component('user-update', {
     mixins: [httpRequestMixin],
     data: function() {
         return {
             url: this.$urls.user.api_profile,
             picture_url: this.$urls.user.api_user_picture,
-            verify_url: this.$urls.user.api_recover,
+            verify_url: this.$urls.user.api_recover + '?noreset=1',
             redirect_url: this.$urls.profile_redirect,
             api_activate_url: this.$urls.user.api_activate,
             formFields: {},
             userModalOpen: false,
             picture: null,
             codeSent: false
         };
```

### Comparing `djaodjin-signup-0.8.2/signup/templates/accounts/login.html` & `djaodjin-signup-0.8.3/signup/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/templates/accounts/recover.html` & `djaodjin-signup-0.8.3/signup/templates/accounts/recover.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/templates/accounts/register.html` & `djaodjin-signup-0.8.3/signup/templates/accounts/register.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/templates/users/index.html` & `djaodjin-signup-0.8.3/signup/templates/users/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/templates/users/password.html` & `djaodjin-signup-0.8.3/signup/templates/users/password.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/templates/users/pubkey.html` & `djaodjin-signup-0.8.3/signup/templates/users/pubkey.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/tests.py` & `djaodjin-signup-0.8.3/signup/tests.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/__init__.py` & `djaodjin-signup-0.8.3/signup/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/__init__.py` & `djaodjin-signup-0.8.3/signup/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/activate.py` & `djaodjin-signup-0.8.3/signup/urls/api/activate.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/activities.py` & `djaodjin-signup-0.8.3/signup/urls/api/activities.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/auth.py` & `djaodjin-signup-0.8.3/signup/urls/api/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,22 @@
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ... import settings
 from ...compat import path, re_path
-from ...api.auth import (JWTActivate, JWTLogin, JWTRegister,
+from ...api.auth import (JWTActivate, JWTLogin, JWTPasswordConfirm, JWTRegister,
     RecoverAPIView)
 
 
 urlpatterns = [
+    re_path(r'^auth/reset/(?P<verification_key>%s)$'
+        % settings.EMAIL_VERIFICATION_PAT,
+        JWTPasswordConfirm.as_view(), name='api_password_confirm'),
     re_path(r'^auth/activate/(?P<verification_key>%s)$'
         % settings.EMAIL_VERIFICATION_PAT,
         JWTActivate.as_view(), name='api_activate'),
     path('auth/register', JWTRegister.as_view(), name='api_register'),
     path('auth/recover', RecoverAPIView.as_view(), name='api_recover'),
     path('auth', JWTLogin.as_view(), name='api_login'),
 ]
```

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/contacts.py` & `djaodjin-signup-0.8.3/signup/urls/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/keys.py` & `djaodjin-signup-0.8.3/signup/urls/api/keys.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/tokens.py` & `djaodjin-signup-0.8.3/signup/urls/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/api/users.py` & `djaodjin-signup-0.8.3/signup/urls/api/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/views/__init__.py` & `djaodjin-signup-0.8.3/signup/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/views/accounts.py` & `djaodjin-signup-0.8.3/signup/urls/views/accounts.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,22 +21,25 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ... import settings
 from ...compat import include, path, re_path
 from ...forms import StartAuthenticationForm
-from ...views.auth import (ActivationView, RecoverView, SigninView,
-    SignoutView, SignupView)
+from ...views.auth import (ActivationView, PasswordResetConfirmView,
+    RecoverView, SigninView, SignoutView, SignupView)
 from ...views.saml import saml_metadata_view
 
 urlpatterns = [
     # When the key and/or token are wrong we don't want to give any clue
     # as to why that is so. Less information communicated to an attacker,
     # the better.
+    re_path(r'^reset/(?P<verification_key>%s)/'
+        % settings.EMAIL_VERIFICATION_PAT,
+        PasswordResetConfirmView.as_view(), name='password_reset_confirm'),
     re_path(r'^activate/(?P<verification_key>%s)/'
         % settings.EMAIL_VERIFICATION_PAT,
         ActivationView.as_view(), name='registration_activate'),
     path(r'activate/',
         SigninView.as_view(
             form_class=StartAuthenticationForm,
             template_name='accounts/activate/index.html'),
```

### Comparing `djaodjin-signup-0.8.2/signup/urls/views/contacts.py` & `djaodjin-signup-0.8.3/signup/urls/views/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/views/saml.py` & `djaodjin-signup-0.8.3/signup/urls/views/saml.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/urls/views/users.py` & `djaodjin-signup-0.8.3/signup/urls/views/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/utils.py` & `djaodjin-signup-0.8.3/signup/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/validators.py` & `djaodjin-signup-0.8.3/signup/validators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/views/auth.py` & `djaodjin-signup-0.8.3/signup/views/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 from django.views.generic.edit import FormMixin, ProcessFormView
 from rest_framework import exceptions, serializers
 
 from .. import settings
 from ..auth import validate_redirect
 from ..compat import gettext_lazy as _, reverse
 from ..forms import (ActivationForm, AuthenticationForm, FrictionlessSignupForm,
-    MFACodeForm, PasswordAuthForm, RecoverForm)
-from ..helpers import has_invalid_password, update_context_urls
-from ..mixins import (LoginMixin, RegisterMixin,  VerifyMixin,
-    VerifyCompleteMixin, AuthDisabled, OTPRequired, PasswordRequired,
-    VerifyRequired, SSORequired, RegistrationDisabled)
+    MFACodeForm, PasswordAuthForm, PasswordResetConfirmForm, RecoverForm)
+from ..helpers import update_context_urls
+from ..mixins import (LoginMixin, PasswordResetConfirmMixin,
+    RegisterMixin, VerifyMixin, VerifyCompleteMixin, AuthDisabled, OTPRequired,
+    PasswordRequired, VerifyRequired, SSORequired, RegistrationDisabled)
 from ..models import Contact
 from ..utils import fill_form_errors, get_disabled_registration
 
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -186,19 +186,14 @@
     def contact(self):
         if not hasattr(self, '_contact'):
             #pylint:disable=attribute-defined-outside-init
             self._contact = Contact.objects.get_token(
                 self.kwargs.get(self.key_url_kwarg))
         return self._contact
 
-    @property
-    def is_user_active(self):
-        return (self.contact and self.contact.user and
-            not has_invalid_password(self.contact.user))
-
     def get_context_data(self, **kwargs):
         context = super(ActivationView, self).get_context_data(**kwargs)
         context.update({'object': self.contact})
         if self.contact and self.contact.extra:
             # XXX 'reason' might be best as a separate field.
             context.update({'reason': self.contact.extra})
         return context
@@ -225,19 +220,14 @@
             verification_key = self.kwargs.get(self.key_url_kwarg)
             if self.contact.email_verification_key == verification_key:
                 initial.update({'email_verification': True})
             if self.contact.phone_verification_key == verification_key:
                 initial.update({'phone_verification': True})
         return initial
 
-    def get_form_class(self):
-        if self.is_user_active:
-            return FrictionlessSignupForm
-        return super(ActivationView, self).get_form_class()
-
     def dispatch(self, request, *args, **kwargs):
         # We put the code inline instead of using method_decorator() otherwise
         # kwargs is interpreted as parameters in sensitive_post_parameters.
         request.sensitive_post_parameters = '__ALL__'
         response = super(ActivationView, self).dispatch(
             request, *args, **kwargs)
         add_never_cache_headers(response)
@@ -304,14 +294,21 @@
             context = {'disabled_registration': True}
 
         if context is None:
             context = self.get_context_data(form=self.get_form())
         return self.render_to_response(context)
 
 
+class PasswordResetConfirmView(PasswordResetConfirmMixin, ActivationView):
+    """
+    Specific view that will first reset a user's password so the form displays.
+    """
+    form_class = PasswordResetConfirmForm
+
+
 class SigninView(LoginMixin, AuthResponseMixin, ProcessFormView):
     """
     Check credentials and sign in the authenticated user.
     """
     form_class = AuthenticationForm
     password_form_class = PasswordAuthForm
     template_name = 'accounts/login.html'
```

### Comparing `djaodjin-signup-0.8.2/signup/views/contacts.py` & `djaodjin-signup-0.8.3/signup/views/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/views/saml.py` & `djaodjin-signup-0.8.3/signup/views/saml.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.2/signup/views/users.py` & `djaodjin-signup-0.8.3/signup/views/users.py`

 * *Files identical despite different names*

