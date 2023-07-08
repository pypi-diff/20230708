# Comparing `tmp/df_websockets-1.0.3.tar.gz` & `tmp/df_websockets-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df_websockets-1.0.3.tar", last modified: Sat Apr 22 16:50:05 2023, max compression
+gzip compressed data, was "dist/df_websockets-1.0.8.tar", last modified: Sat Jul  8 12:19:21 2023, max compression
```

## Comparing `df_websockets-1.0.3.tar` & `df_websockets-1.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.638219 df_websockets-1.0.3/
--rw-r--r--   0 flanker    (501) staff       (20)     3094 2023-04-22 16:43:51.000000 df_websockets-1.0.3/.gitignore
--rw-r--r--   0 flanker    (501) staff       (20)      478 2021-03-25 18:53:48.000000 df_websockets-1.0.3/.travis.yml
--rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.3/LICENSE
--rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.3/MANIFEST.in
--rw-r--r--   0 flanker    (501) staff       (20)    19848 2023-04-22 16:50:05.638555 df_websockets-1.0.3/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)    18598 2023-04-22 16:43:51.000000 df_websockets-1.0.3/README.md
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.577858 df_websockets-1.0.3/demo_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5682 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     5475 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/signals.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.579933 df_websockets-1.0.3/demo_df_websockets/static/
--rw-r--r--   0 flanker    (501) staff       (20)      224 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/static/demo.css
--rw-r--r--   0 flanker    (501) staff       (20)      329 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/static/demo.js
--rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.3/demo_df_websockets/static/image.png
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.580826 df_websockets-1.0.3/demo_df_websockets/templates/
--rw-r--r--   0 flanker    (501) staff       (20)    29153 2023-04-22 16:43:51.000000 df_websockets-1.0.3/demo_df_websockets/templates/index.html
--rw-r--r--   0 flanker    (501) staff       (20)      769 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/urls.py
--rw-r--r--   0 flanker    (501) staff       (20)      215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_df_websockets/views.py
--rwxr-xr-x   0 flanker    (501) staff       (20)      334 2023-01-28 22:42:08.000000 df_websockets-1.0.3/demo_manage.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.610794 df_websockets-1.0.3/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     1237 2023-04-22 16:49:52.000000 df_websockets-1.0.3/df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)      301 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/apps.py
--rw-r--r--   0 flanker    (501) staff       (20)     2900 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     1414 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/checks.py
--rw-r--r--   0 flanker    (501) staff       (20)     1471 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/constants.py
--rw-r--r--   0 flanker    (501) staff       (20)     8285 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)    13765 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/decorators.py
--rw-r--r--   0 flanker    (501) staff       (20)      217 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/load.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.616988 df_websockets-1.0.3/df_websockets/management/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/__init__.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.619643 df_websockets-1.0.3/df_websockets/management/commands/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/commands/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1685 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/management/commands/celery.py
--rw-r--r--   0 flanker    (501) staff       (20)     3489 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/management/commands/worker.py
--rw-r--r--   0 flanker    (501) staff       (20)     3829 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1989 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/routing.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.566543 df_websockets-1.0.3/df_websockets/static/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.621103 df_websockets-1.0.3/df_websockets/static/js/
--rw-r--r--   0 flanker    (501) staff       (20)     7866 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js
--rw-r--r--   0 flanker    (501) staff       (20)    44971 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js.map
--rw-r--r--   0 flanker    (501) staff       (20)    16911 2023-04-22 16:47:25.000000 df_websockets-1.0.3/df_websockets/tasks.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.623127 df_websockets-1.0.3/df_websockets/templatetags/
--rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/templatetags/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     2579 2023-01-28 22:42:08.000000 df_websockets-1.0.3/df_websockets/templatetags/websockets.py
--rw-r--r--   0 flanker    (501) staff       (20)     5424 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/testing.py
--rw-r--r--   0 flanker    (501) staff       (20)     3039 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/topics.py
--rw-r--r--   0 flanker    (501) staff       (20)     6143 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     5736 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/window_info.py
--rw-r--r--   0 flanker    (501) staff       (20)    11796 2023-04-22 16:48:31.000000 df_websockets-1.0.3/df_websockets/ws_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     3547 2023-04-22 16:43:51.000000 df_websockets-1.0.3/df_websockets/ws_settings.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.616209 df_websockets-1.0.3/df_websockets.egg-info/
--rw-r--r--   0 flanker    (501) staff       (20)    19848 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     1828 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.3/df_websockets.egg-info/not-zip-safe
--rw-r--r--   0 flanker    (501) staff       (20)       45 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/requires.txt
--rw-r--r--   0 flanker    (501) staff       (20)       52 2023-04-22 16:50:05.000000 df_websockets-1.0.3/df_websockets.egg-info/top_level.txt
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.628277 df_websockets-1.0.3/npm/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.631419 df_websockets-1.0.3/npm/df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)     5253 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/app.js
--rw-r--r--   0 flanker    (501) staff       (20)    13295 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/base.js
--rw-r--r--   0 flanker    (501) staff       (20)    10672 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/forms.ts
--rw-r--r--   0 flanker    (501) staff       (20)     4494 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/df_websockets/html.js
--rw-r--r--   0 flanker    (501) staff       (20)   112499 2023-04-22 16:45:55.000000 df_websockets-1.0.3/npm/package-lock.json
--rw-r--r--   0 flanker    (501) staff       (20)      475 2021-03-25 21:22:08.000000 df_websockets-1.0.3/npm/package.json
--rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.3/npm/tsconfig.json
--rw-r--r--   0 flanker    (501) staff       (20)     1963 2023-01-28 22:42:08.000000 df_websockets-1.0.3/npm/webpack.config.js
--rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2023-01-28 22:42:08.000000 df_websockets-1.0.3/pre-commit.sh
--rw-r--r--   0 flanker    (501) staff       (20)     2700 2023-04-22 16:50:05.640344 df_websockets-1.0.3/setup.cfg
--rw-r--r--   0 flanker    (501) staff       (20)     1254 2023-01-28 22:42:08.000000 df_websockets-1.0.3/setup.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-04-22 16:50:05.637521 df_websockets-1.0.3/test_df_websockets/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.3/test_df_websockets/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     5824 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_consumers.py
--rw-r--r--   0 flanker    (501) staff       (20)     1339 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_decorators.py
--rw-r--r--   0 flanker    (501) staff       (20)     3350 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     1834 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_testing.py
--rw-r--r--   0 flanker    (501) staff       (20)      414 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_utils.py
--rw-r--r--   0 flanker    (501) staff       (20)      998 2023-04-22 16:43:51.000000 df_websockets-1.0.3/test_df_websockets/test_window_info.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.575796 df_websockets-1.0.8/
+-rw-r--r--   0 flanker    (501) staff       (20)     3094 2023-04-29 20:53:03.000000 df_websockets-1.0.8/.gitignore
+-rw-r--r--   0 flanker    (501) staff       (20)      656 2023-07-07 10:01:48.000000 df_websockets-1.0.8/.travis.yml
+-rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-11-04 09:00:51.000000 df_websockets-1.0.8/LICENSE
+-rw-r--r--   0 flanker    (501) staff       (20)      105 2020-11-04 09:00:51.000000 df_websockets-1.0.8/MANIFEST.in
+-rw-r--r--   0 flanker    (501) staff       (20)    20912 2023-07-08 12:19:21.576209 df_websockets-1.0.8/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)    19623 2023-07-08 11:12:02.000000 df_websockets-1.0.8/README.md
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.497206 df_websockets-1.0.8/demo_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5682 2023-04-22 16:43:51.000000 df_websockets-1.0.8/demo_df_websockets/settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5475 2023-04-22 16:43:51.000000 df_websockets-1.0.8/demo_df_websockets/signals.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.499914 df_websockets-1.0.8/demo_df_websockets/static/
+-rw-r--r--   0 flanker    (501) staff       (20)      224 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_df_websockets/static/demo.css
+-rw-r--r--   0 flanker    (501) staff       (20)      329 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_df_websockets/static/demo.js
+-rw-r--r--   0 flanker    (501) staff       (20)    15390 2021-03-22 07:04:44.000000 df_websockets-1.0.8/demo_df_websockets/static/image.png
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.501376 df_websockets-1.0.8/demo_df_websockets/templates/
+-rw-r--r--   0 flanker    (501) staff       (20)    29153 2023-04-22 16:43:51.000000 df_websockets-1.0.8/demo_df_websockets/templates/index.html
+-rw-r--r--   0 flanker    (501) staff       (20)      769 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_df_websockets/urls.py
+-rw-r--r--   0 flanker    (501) staff       (20)      215 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_df_websockets/views.py
+-rwxr-xr-x   0 flanker    (501) staff       (20)      334 2023-01-28 22:42:08.000000 df_websockets-1.0.8/demo_manage.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.531928 df_websockets-1.0.8/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     1238 2023-07-08 11:16:37.000000 df_websockets-1.0.8/df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)      301 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/apps.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2900 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1414 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/checks.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1471 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/constants.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8382 2023-04-29 13:26:58.000000 df_websockets-1.0.8/df_websockets/consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)    13765 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/decorators.py
+-rw-r--r--   0 flanker    (501) staff       (20)      217 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/load.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.536853 df_websockets-1.0.8/df_websockets/management/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.8/df_websockets/management/__init__.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.539357 df_websockets-1.0.8/df_websockets/management/commands/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.8/df_websockets/management/commands/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1685 2023-01-28 22:42:08.000000 df_websockets-1.0.8/df_websockets/management/commands/celery.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3489 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/management/commands/worker.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3829 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1989 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/routing.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.484254 df_websockets-1.0.8/df_websockets/static/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.541316 df_websockets-1.0.8/df_websockets/static/js/
+-rw-r--r--   0 flanker    (501) staff       (20)     8053 2023-05-01 20:39:22.000000 df_websockets-1.0.8/df_websockets/static/js/df_websockets.min.js
+-rw-r--r--   0 flanker    (501) staff       (20)    46909 2023-05-01 20:39:22.000000 df_websockets-1.0.8/df_websockets/static/js/df_websockets.min.js.map
+-rw-r--r--   0 flanker    (501) staff       (20)    16911 2023-04-22 16:47:25.000000 df_websockets-1.0.8/df_websockets/tasks.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.543444 df_websockets-1.0.8/df_websockets/templatetags/
+-rw-r--r--   0 flanker    (501) staff       (20)     1215 2023-01-28 22:42:08.000000 df_websockets-1.0.8/df_websockets/templatetags/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2579 2023-01-28 22:42:08.000000 df_websockets-1.0.8/df_websockets/templatetags/websockets.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5424 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3039 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/topics.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6143 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5736 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/window_info.py
+-rw-r--r--   0 flanker    (501) staff       (20)    11796 2023-04-22 16:48:31.000000 df_websockets-1.0.8/df_websockets/ws_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3547 2023-04-22 16:43:51.000000 df_websockets-1.0.8/df_websockets/ws_settings.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.536255 df_websockets-1.0.8/df_websockets.egg-info/
+-rw-r--r--   0 flanker    (501) staff       (20)    20912 2023-07-08 12:19:21.000000 df_websockets-1.0.8/df_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     1828 2023-07-08 12:19:21.000000 df_websockets-1.0.8/df_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2023-07-08 12:19:21.000000 df_websockets-1.0.8/df_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-11-21 14:07:31.000000 df_websockets-1.0.8/df_websockets.egg-info/not-zip-safe
+-rw-r--r--   0 flanker    (501) staff       (20)       45 2023-07-08 12:19:21.000000 df_websockets-1.0.8/df_websockets.egg-info/requires.txt
+-rw-r--r--   0 flanker    (501) staff       (20)       52 2023-07-08 12:19:21.000000 df_websockets-1.0.8/df_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.547928 df_websockets-1.0.8/npm/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.552025 df_websockets-1.0.8/npm/df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)     5203 2023-04-29 14:51:26.000000 df_websockets-1.0.8/npm/df_websockets/app.js
+-rw-r--r--   0 flanker    (501) staff       (20)    13773 2023-04-29 21:05:59.000000 df_websockets-1.0.8/npm/df_websockets/base.js
+-rw-r--r--   0 flanker    (501) staff       (20)    11452 2023-05-01 20:35:31.000000 df_websockets-1.0.8/npm/df_websockets/forms.ts
+-rw-r--r--   0 flanker    (501) staff       (20)     4930 2023-05-01 20:35:31.000000 df_websockets-1.0.8/npm/df_websockets/html.js
+-rw-r--r--   0 flanker    (501) staff       (20)   112515 2023-04-29 20:07:19.000000 df_websockets-1.0.8/npm/package-lock.json
+-rw-r--r--   0 flanker    (501) staff       (20)      801 2023-07-08 12:13:43.000000 df_websockets-1.0.8/npm/package.json
+-rw-r--r--   0 flanker    (501) staff       (20)      256 2021-03-23 20:46:59.000000 df_websockets-1.0.8/npm/tsconfig.json
+-rw-r--r--   0 flanker    (501) staff       (20)     3002 2023-04-29 21:04:38.000000 df_websockets-1.0.8/npm/webpack.config.js
+-rwxr-xr-x   0 flanker    (501) staff       (20)     1250 2023-01-28 22:42:08.000000 df_websockets-1.0.8/pre-commit.sh
+-rw-r--r--   0 flanker    (501) staff       (20)     2732 2023-07-08 12:19:21.578108 df_websockets-1.0.8/setup.cfg
+-rw-r--r--   0 flanker    (501) staff       (20)     1254 2023-01-28 22:42:08.000000 df_websockets-1.0.8/setup.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-07-08 12:19:21.575047 df_websockets-1.0.8/test_df_websockets/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-28 22:42:08.000000 df_websockets-1.0.8/test_df_websockets/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5824 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_consumers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1339 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_decorators.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3350 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1834 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_testing.py
+-rw-r--r--   0 flanker    (501) staff       (20)      414 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)      998 2023-04-22 16:43:51.000000 df_websockets-1.0.8/test_df_websockets/test_window_info.py
```

### Comparing `df_websockets-1.0.3/.gitignore` & `df_websockets-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/LICENSE` & `df_websockets-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/PKG-INFO` & `df_websockets-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: df_websockets
-Version: 1.0.3
+Version: 1.0.8
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 df_websockets
 =============
 
 `df_websockets` extends [django-channels](https://channels.readthedocs.io) to simplify communications between 
@@ -99,15 +100,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
-_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
+_`daphne` must be separately installed and added to `INSTALLED_APPS` with `channels>=4.0`_ 
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
@@ -235,14 +236,45 @@
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
 
+Cache backends
+--------------
+
+Task data are passed by the server process to the workers using the Django cache infrastructure. 
+For obvious reasons, you cannot use DummyCache nor LocMemCache with Celery or Channels workers, since these caching methods are not shared accross processes.
+So, you need either to use a shared cache backend as default backend, or dedicate a cache backend to websockets. 
+
+First case needs to update your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    }
+}
+```
+
+Second case, still in your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
+        "LOCATION": "unique-snowflake",
+    },
+    "websockets": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    },
+}
+WEBSOCKET_CACHE_BACKEND = "websockets"
+```
 
 HTML forms
 ----------
 
 `df_websockets` comes with some helper functions when you signals to be trigger on the server when a form is submitted or changed.
 Assuming that you have a `signals.py` file that contains:
 ```python
```

### Comparing `df_websockets-1.0.3/README.md` & `df_websockets-1.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
-_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
+_`daphne` must be separately installed and added to `INSTALLED_APPS` with `channels>=4.0`_ 
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
@@ -204,14 +204,45 @@
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
 
+Cache backends
+--------------
+
+Task data are passed by the server process to the workers using the Django cache infrastructure. 
+For obvious reasons, you cannot use DummyCache nor LocMemCache with Celery or Channels workers, since these caching methods are not shared accross processes.
+So, you need either to use a shared cache backend as default backend, or dedicate a cache backend to websockets. 
+
+First case needs to update your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    }
+}
+```
+
+Second case, still in your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
+        "LOCATION": "unique-snowflake",
+    },
+    "websockets": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    },
+}
+WEBSOCKET_CACHE_BACKEND = "websockets"
+```
 
 HTML forms
 ----------
 
 `df_websockets` comes with some helper functions when you signals to be trigger on the server when a form is submitted or changed.
 Assuming that you have a `signals.py` file that contains:
 ```python
```

### Comparing `df_websockets-1.0.3/demo_df_websockets/settings.py` & `df_websockets-1.0.8/demo_df_websockets/settings.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/demo_df_websockets/signals.py` & `df_websockets-1.0.8/demo_df_websockets/signals.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/demo_df_websockets/static/image.png` & `df_websockets-1.0.8/demo_df_websockets/static/image.png`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/demo_df_websockets/templates/index.html` & `df_websockets-1.0.8/demo_df_websockets/templates/index.html`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/demo_df_websockets/urls.py` & `df_websockets-1.0.8/demo_df_websockets/urls.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/__init__.py` & `df_websockets-1.0.8/df_websockets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 #                                                                              #
 #  You should have received a copy of the CeCILL-B license with                #
 #  this file. If not, please visit:                                            #
 #  https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           #
 #  or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         #
 #                                                                              #
 # ##############################################################################
-__version__ = "1.0.3"
+
+__version__ = "1.0.8"
```

### Comparing `df_websockets-1.0.3/df_websockets/celery.py` & `df_websockets-1.0.8/df_websockets/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/checks.py` & `df_websockets-1.0.8/df_websockets/checks.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/constants.py` & `df_websockets-1.0.8/df_websockets/constants.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/consumers.py` & `df_websockets-1.0.8/df_websockets/consumers.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         if self.scope.get("server", None):
             request.META["SERVER_NAME"] = self.scope["server"][0]
             request.META["SERVER_PORT"] = str(self.scope["server"][1])
         else:
             request.META["SERVER_NAME"] = "unknown"
             request.META["SERVER_PORT"] = "0"
         request.META["HTTP_X_REQUESTED_WITH"] = "XMLHttpRequest"
+        request.META["wsgi.multithread"] = True
+        request.META["wsgi.multiprocess"] = True
         request.COOKIES = self.scope.get("cookies", {})
         return request
 
     def disconnect(self, close_code):
         for topic in self.topics:
             async_to_sync(self.channel_layer.group_discard)(topic, self.channel_name)
```

### Comparing `df_websockets-1.0.3/df_websockets/decorators.py` & `df_websockets-1.0.8/df_websockets/decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/management/__init__.py` & `df_websockets-1.0.8/df_websockets/management/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/management/commands/__init__.py` & `df_websockets-1.0.8/df_websockets/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/management/commands/celery.py` & `df_websockets-1.0.8/df_websockets/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/management/commands/worker.py` & `df_websockets-1.0.8/df_websockets/management/commands/worker.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/middleware.py` & `df_websockets-1.0.8/df_websockets/middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/routing.py` & `df_websockets-1.0.8/df_websockets/routing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js` & `df_websockets-1.0.8/df_websockets/static/js/df_websockets.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,41 +3,42 @@
             821: () => {
                 window.DFSignals = {
                     connection: null,
                     buffer: [],
                     registry: {},
                     wsurl: null
                 }, document.addEventListener("DOMContentLoaded", (function e() {
+                    const n = "dfwsurl";
                     if (null === window.DFSignals.wsurl) {
                         const e = function(e) {
-                            const n = "dfwsurl=",
+                            const n = e + "=",
                                 t = decodeURIComponent(document.cookie).split(";");
                             for (let e = 0; e < t.length; e++) {
                                 let o = t[e];
                                 for (;
                                     " " === o.charAt(0);) o = o.substring(1);
-                                if (0 === o.indexOf(n)) return o.substring(n.length, o.length)
+                                if (0 === o.indexOf(n)) return o.substring(8, o.length)
                             }
                             return ""
-                        }();
+                        }(n);
                         window.DFSignals.wsurl = decodeURIComponent(e)
                     }
-                    if (!window.DFSignals.wsurl) return void console.info("Unable to get the websocket URL in the 'dfwsurl' cookie.");
-                    const n = new WebSocket(window.DFSignals.wsurl);
-                    n.onopen = () => {
-                        window.DFSignals.connection = n;
-                        for (let e = 0; e < window.DFSignals.buffer.length; e++) n.send(window.DFSignals.buffer[e]);
+                    if (!window.DFSignals.wsurl) return void console.info("Unable to get the websocket URL in the '" + n + "' cookie.");
+                    const t = new WebSocket(window.DFSignals.wsurl);
+                    t.onopen = () => {
+                        window.DFSignals.connection = t;
+                        for (let e = 0; e < window.DFSignals.buffer.length; e++) t.send(window.DFSignals.buffer[e]);
                         window.DFSignals.buffer = []
-                    }, n.onmessage = e => {
+                    }, t.onmessage = e => {
                         console.debug("received call " + e.data + " from server.");
                         const n = JSON.parse(e.data);
                         n.signal && n.signal_id && window.DFSignals.call(n.signal, n.opts, n.signal_id)
-                    }, n.onerror = e => {
+                    }, t.onerror = e => {
                         console.error("WS error: " + e)
-                    }, n.onclose = () => {
+                    }, t.onclose = () => {
                         window.DFSignals.connection = null, setTimeout(e, 3e3)
                     }
                 })), window.DFSignals.call = function(e, n, t) {
                     if (void 0 !== t && void 0 !== window.DFSignals.registry[t]) return !1;
                     if (void 0 !== t && (window.DFSignals.registry[t] = !0), void 0 !== window.DFSignals.registry[e]) {
                         console.debug('call "' + e + '"', n);
                         for (let o = 0; o < window.DFSignals.registry[e].length; o += 1) window.DFSignals.registry[e][o](n, t)
@@ -59,66 +60,66 @@
                 "use strict";
                 var o = t(125);
                 const l = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             const t = n.nextSibling;
                             n.insertAdjacentHTML("afterend", e.content);
                             let o = n.nextSibling;
-                            for (; o && o !== t;) o.dispatchEvent(new Event("DOMContentAdded", {
+                            for (; o && o !== t;) o.querySelectorAll && o.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), o = o.nextSibling
                         }))
                     },
                     i = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             const t = n.lastChild;
                             n.insertAdjacentHTML("beforeend", e.content);
                             let o = n.lastChild;
-                            for (; o && o !== t;) o.dispatchEvent(new Event("DOMContentAdded", {
+                            for (; o && o !== t;) o.querySelectorAll && o.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), o = o.previousSibling
                         }))
                     },
                     r = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             const t = n.firstChild;
                             n.insertAdjacentHTML("afterbegin", e.content);
                             let o = n.firstChild;
-                            for (; o && o !== t;) o.dispatchEvent(new Event("DOMContentAdded", {
+                            for (; o && o !== t;) o.querySelectorAll && o.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), o = o.nextSibling
                         }))
                     },
                     c = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             const t = n.previousSibling;
                             n.insertAdjacentHTML("beforebegin", e.content);
                             let o = n.previousSibling;
-                            for (; o && o !== t;) o.dispatchEvent(new Event("DOMContentAdded", {
+                            for (; o && o !== t;) o.querySelectorAll && o.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), o = o.previousSibling
                         }))
                     },
                     s = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             n.innerHTML = e.content;
                             let t = n.firstChild;
-                            for (; t;) t.dispatchEvent(new Event("DOMContentAdded", {
+                            for (; t;) t.querySelectorAll && t.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), t = t.nextSibling
                         }))
                     },
                     a = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             const t = n.previousSibling,
                                 o = n.nextSibling,
                                 l = n.parentNode;
                             n.outerHTML = e.content;
                             let i = l.firstChild;
-                            for (t && (i = t.nextSibling); i && i !== o;) i.dispatchEvent(new Event("DOMContentAdded", {
+                            for (t && (i = t.nextSibling); i && i !== o;) i.querySelectorAll && i.dispatchEvent(new Event("DOMContentAdded", {
                                 bubbles: !0
                             })), i = i.nextSibling
                         }))
                     },
                     d = e => {
                         document.querySelectorAll(e.selector).forEach((e => {
                             for (; e.firstChild;) e.removeChild(e.firstChild)
@@ -129,59 +130,61 @@
                             e.parentNode.removeChild(e)
                         }))
                     },
                     f = e => {
                         document.querySelectorAll(e.selector).forEach((n => {
                             n.textContent = e.content
                         }))
-                    },
-                    w = e => {
-                        document.querySelectorAll(e.selector).forEach((n => {
-                            n.classList.add(e.class_name)
-                        }))
-                    },
-                    g = e => {
-                        document.querySelectorAll(e.selector).forEach((n => {
-                            n.classList.remove(e.class_name)
-                        }))
-                    },
-                    m = e => {
-                        document.querySelectorAll(e.selector).forEach((n => {
-                            n.removeAttribute(e.attr_name)
-                        }))
-                    },
-                    h = e => {
-                        document.querySelectorAll(e.selector).forEach((n => {
-                            n.setAttribute(e.attr_name, e.attr_value)
-                        }))
-                    },
-                    v = e => {
-                        document.querySelectorAll(e.selector).forEach((n => {
-                            e.value ? n.setAttribute(e.name, e.name) : n.removeAttribute(e.name)
-                        }))
-                    },
-                    S = e => {
-                        const n = document.createElement("a");
-                        n.href = e.url, n.target = "_blank", n.download = e.filename || "unknown";
-                        const t = new MouseEvent("click", {
-                            view: window,
-                            bubbles: !0,
-                            cancelable: !1
-                        });
-                        n.dispatchEvent(t), (window.URL || window.webkitURL).revokeObjectURL(n.href)
-                    },
-                    b = e => {
-                        const n = document.querySelector(e.selector);
-                        n && n.focus({
-                            preventScroll: !1
-                        })
                     };
-                document.addEventListener("DOMContentLoaded", (function() {
-                    window.DFSignals.connect("html.after", l), window.DFSignals.connect("html.append", i), window.DFSignals.connect("html.prepend", r), window.DFSignals.connect("html.before", c), window.DFSignals.connect("html.content", s), window.DFSignals.connect("html.replace_with", a), window.DFSignals.connect("html.empty", d), window.DFSignals.connect("html.remove", u), window.DFSignals.connect("html.add_class", w), window.DFSignals.connect("html.remove_class", g), window.DFSignals.connect("html.remove_attr", m), window.DFSignals.connect("html.add_attribute", h), window.DFSignals.connect("html.boolean_attribute", v), window.DFSignals.connect("html.text", f), window.DFSignals.connect("html.download_file", S), window.DFSignals.connect("html.focus", b), window.DFSignals.connect("html.forms.set", o._)
-                }))
+                (() => {
+                    const e = e => {
+                            document.querySelectorAll(e.selector).forEach((n => {
+                                n.classList.add(e.class_name)
+                            }))
+                        },
+                        n = e => {
+                            document.querySelectorAll(e.selector).forEach((n => {
+                                n.classList.remove(e.class_name)
+                            }))
+                        },
+                        t = e => {
+                            document.querySelectorAll(e.selector).forEach((n => {
+                                n.removeAttribute(e.attr_name)
+                            }))
+                        },
+                        w = e => {
+                            document.querySelectorAll(e.selector).forEach((n => {
+                                n.setAttribute(e.attr_name, e.attr_value)
+                            }))
+                        },
+                        g = e => {
+                            document.querySelectorAll(e.selector).forEach((n => {
+                                e.value ? n.setAttribute(e.name, e.name) : n.removeAttribute(e.name)
+                            }))
+                        },
+                        m = e => {
+                            const n = document.createElement("a");
+                            n.href = e.url, n.target = "_blank", n.download = e.filename || "unknown";
+                            const t = new MouseEvent("click", {
+                                view: window,
+                                bubbles: !0,
+                                cancelable: !1
+                            });
+                            n.dispatchEvent(t), (window.URL || window.webkitURL).revokeObjectURL(n.href)
+                        },
+                        h = e => {
+                            const n = document.querySelector(e.selector);
+                            n && n.focus({
+                                preventScroll: !1
+                            })
+                        };
+                    document.addEventListener("DOMContentLoaded", (function() {
+                        window.DFSignals.connect("html.after", l), window.DFSignals.connect("html.append", i), window.DFSignals.connect("html.prepend", r), window.DFSignals.connect("html.before", c), window.DFSignals.connect("html.content", s), window.DFSignals.connect("html.replace_with", a), window.DFSignals.connect("html.empty", d), window.DFSignals.connect("html.remove", u), window.DFSignals.connect("html.add_class", e), window.DFSignals.connect("html.remove_class", n), window.DFSignals.connect("html.remove_attr", t), window.DFSignals.connect("html.add_attribute", w), window.DFSignals.connect("html.boolean_attribute", g), window.DFSignals.connect("html.text", f), window.DFSignals.connect("html.download_file", m), window.DFSignals.connect("html.focus", h), window.DFSignals.connect("html.forms.set", o._)
+                    }))
+                })()
             },
             125: (e, n, t) => {
                 "use strict";
 
                 function o(e) {
                     document.querySelectorAll(e.selector).forEach((function(n) {
                         e.values.forEach((function(e) {
@@ -209,65 +212,67 @@
                                     else
                                         for (c = 0; c < i.length; c++) i[c].selected = i[c].value === t
                                 } else o instanceof HTMLInputElement && (o.value = t)
                             }(n, e.name, e.value)
                         }))
                     }))
                 }
-
-                function l(e) {
-                    e.target.querySelectorAll("[data-df-signal]").forEach((function(e) {
-                        JSON.parse(e.getAttribute("data-df-signal")).forEach((function(n) {
-                            var t = n.on;
-                            t || (t = "FORM" === e.tagName ? "submit" : "INPUT" === e.tagName && "reset" !== e.type && "submit" !== e.type && "button" !== e.type || "TEXTAREA" === e.tagName ? "change" : "click"), e.addEventListener(t, (function(o) {
-                                var l = n.prevent,
-                                    i = n.opts || {};
-                                if (n.form && (i[n.form] = function(e) {
-                                        for (var n = [], t = 0; t < e.elements.length; t++) {
-                                            var o = e.elements[t];
-                                            if (o.name && !o.disabled && "reset" !== o.type && "submit" !== o.type && "button" !== o.type)
-                                                if ("file" === o.type)
-                                                    for (var l = 0; l < o.files.length; l++) n.push({
+                t.d(n, {
+                        _: () => o
+                    }),
+                    function() {
+                        function e(e) {
+                            e.target.querySelectorAll && e.target.querySelectorAll("[data-df-signal]").forEach((function(e) {
+                                JSON.parse(e.getAttribute("data-df-signal")).forEach((function(n) {
+                                    var t = n.on;
+                                    t || (t = "FORM" === e.tagName ? "submit" : "INPUT" === e.tagName && "reset" !== e.type && "submit" !== e.type && "button" !== e.type || "TEXTAREA" === e.tagName ? "change" : "click"), e.addEventListener(t, (function(o) {
+                                        var l = n.prevent,
+                                            i = n.opts || {};
+                                        if (n.form && (i[n.form] = function(e) {
+                                                for (var n = [], t = 0; t < e.elements.length; t++) {
+                                                    var o = e.elements[t];
+                                                    if (o.name && !o.disabled && "reset" !== o.type && "submit" !== o.type && "button" !== o.type)
+                                                        if ("file" === o.type)
+                                                            for (var l = 0; l < o.files.length; l++) n.push({
+                                                                name: o.name,
+                                                                value: o.files[l].name
+                                                            });
+                                                        else if ("select-multiple" === o.type)
+                                                        for (l = 0; l < o.selectedOptions.length; l++) n.push({
+                                                            name: o.name,
+                                                            value: o.selectedOptions[l].value
+                                                        });
+                                                    else("checkbox" !== o.type && "radio" !== o.type || o.checked) && n.push({
                                                         name: o.name,
-                                                        value: o.files[l].name
-                                                    });
-                                                else if ("select-multiple" === o.type)
-                                                for (l = 0; l < o.selectedOptions.length; l++) n.push({
-                                                    name: o.name,
-                                                    value: o.selectedOptions[l].value
-                                                });
-                                            else("checkbox" !== o.type && "radio" !== o.type || o.checked) && n.push({
-                                                name: o.name,
-                                                value: o.value
-                                            })
-                                        }
-                                        return n
-                                    }(e)), n.value)
-                                    if ("file" === e.type) {
-                                        i[n.value] = [];
-                                        for (var r = 0; r < e.files.length; r++) i[n.value].push(e.files[r].name)
-                                    } else if ("select-multiple" === e.type)
-                                    for (i[n.value] = [], r = 0; r < e.selectedOptions.length; r++) i[n.value].push(e.selectedOptions[r].value);
-                                else "checkbox" === e.type || "radio" === e.type ? i[n.value] = e.checked : i[n.value] = e.value;
-                                window.DFSignals.call(n.name, i), (!0 === l || null === l && "change" !== t) && o.preventDefault()
+                                                        value: o.value
+                                                    })
+                                                }
+                                                return n
+                                            }(e)), n.value)
+                                            if ("file" === e.type) {
+                                                i[n.value] = [];
+                                                for (var r = 0; r < e.files.length; r++) i[n.value].push(e.files[r].name)
+                                            } else if ("select-multiple" === e.type)
+                                            for (i[n.value] = [], r = 0; r < e.selectedOptions.length; r++) i[n.value].push(e.selectedOptions[r].value);
+                                        else "checkbox" === e.type || "radio" === e.type ? i[n.value] = e.checked : i[n.value] = e.value;
+                                        window.DFSignals.call(n.name, i, void 0), (!0 === l || null === l && "change" !== t) && o.preventDefault()
+                                    }))
+                                }))
                             }))
+                        }
+                        document.addEventListener("DOMContentAdded", (function(n) {
+                            window.setTimeout((function() {
+                                e(n)
+                            }), 50)
+                        })), document.addEventListener("DOMContentLoaded", (function(n) {
+                            window.setTimeout((function() {
+                                e(n)
+                            }), 50)
                         }))
-                    }))
-                }
-                t.d(n, {
-                    _: () => o
-                }), document.addEventListener("DOMContentAdded", (function(e) {
-                    window.setTimeout((function() {
-                        l(e)
-                    }), 200)
-                })), document.addEventListener("DOMContentLoaded", (function(e) {
-                    window.setTimeout((function() {
-                        l(e)
-                    }), 200)
-                }))
+                    }()
             }
         },
         n = {};
 
     function t(o) {
         var l = n[o];
         if (void 0 !== l) return l.exports;
```

### Comparing `df_websockets-1.0.3/df_websockets/static/js/df_websockets.min.js.map` & `df_websockets-1.0.8/df_websockets/static/js/df_websockets.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8082779623477298%*

 * *Differences: {"'mappings'": "'sBAiBEA,OAAOC,UAAY,CACjBC,WAAY,KACZC,OAAQ,GACRC,SAAU,CAAC,EACXC,MAAO,MAiHTC,SAASC,iBAAiB,oBA9F1B,SAASC,IACP,MAAMC,EAAa,UACnB,GAA+B,OAA3BT,OAAOC,UAAUI,MAAgB,CACnC,MAAMK,EAnBV,SAAmBC,GACjB,MAAMC,EAAOD,EAAQ,IAEfE,EADgBC,mBAAmBR,SAASS,QACzBC,MAAM,KAC/B,IAAK,IAAIC,EAAI,EAAGA,EAAIJ,EAAGK,OAAQD,IAAK,CAClC,IAAIE,EAAIN,EAAGI,GACX,KAAuB,MAAhBE,EAAEC,OAAO,IACdD,EAAIA,EAAEE,UAAU,GAElB,GAAwB,IAApBF,EAAEG,QAAQV,GACZ,OAAOO,EAAEE,UAAUT,EAAaO,EAAED,OAEtC,CACA,MAAO,EACT,CAKoBK,CAAUd,GAC1BT,OAAOC,UAAUI,MAAQS, […]*

```diff
@@ -1,20 +1,21 @@
 {
     "file": "df_websockets/static/js/df_websockets.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "window",
         "DFSignals",
         "connection",
         "buffer",
         "registry",
         "wsurl",
         "document",
         "addEventListener",
         "websocketConnect",
+        "cookieName",
         "dfWsURL",
         "cname",
         "name",
         "ca",
         "decodeURIComponent",
         "cookie",
         "split",
@@ -135,15 +136,15 @@
         "HTMLInputElement",
         "type",
         "HTMLSelectElement",
         "options",
         "valuesSet",
         "selected",
         "setFormFieldValue",
-        "DOMContentAdded",
+        "websocketForms",
         "getAttribute",
         "eventName",
         "on",
         "tagName",
         "prevent",
         "serialized",
         "field",
@@ -171,28 +172,28 @@
         "obj",
         "prop",
         "prototype",
         "hasOwnProperty"
     ],
     "sourceRoot": "",
     "sources": [
-        "webpack://df_websockets/./df_websockets/app.js",
-        "webpack://df_websockets/./df_websockets/html.js",
-        "webpack://df_websockets/./df_websockets/base.js",
-        "webpack://df_websockets/./df_websockets/forms.ts",
-        "webpack://df_websockets/webpack/bootstrap",
-        "webpack://df_websockets/webpack/runtime/define property getters",
-        "webpack://df_websockets/webpack/runtime/hasOwnProperty shorthand",
-        "webpack://df_websockets/webpack/startup"
+        "webpack://@d9pouces/df_websockets/./df_websockets/app.js",
+        "webpack://@d9pouces/df_websockets/./df_websockets/html.js",
+        "webpack://@d9pouces/df_websockets/./df_websockets/base.js",
+        "webpack://@d9pouces/df_websockets/./df_websockets/forms.ts",
+        "webpack://@d9pouces/df_websockets/webpack/bootstrap",
+        "webpack://@d9pouces/df_websockets/webpack/runtime/define property getters",
+        "webpack://@d9pouces/df_websockets/webpack/runtime/hasOwnProperty shorthand",
+        "webpack://@d9pouces/df_websockets/webpack/startup"
     ],
     "sourcesContent": [
-        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n\nwindow.DFSignals = {\n    connection: null,\n    buffer: [],\n    registry: {},\n    wsurl: null\n};\n\nfunction getCookie(cname) {\n    const name = cname + \"=\";\n    const decodedCookie = decodeURIComponent(document.cookie);\n    const ca = decodedCookie.split(';');\n    for (let i = 0; i < ca.length; i++) {\n        let c = ca[i];\n        while (c.charAt(0) === ' ') {\n            c = c.substring(1);\n        }\n        if (c.indexOf(name) === 0) {\n            return c.substring(name.length, c.length);\n        }\n    }\n    return \"\";\n}\n\nfunction websocketConnect() {\n    const cookieName = \"dfwsurl\";\n    if (window.DFSignals.wsurl === null) {\n        const dfWsURL = getCookie(cookieName);\n        window.DFSignals.wsurl = decodeURIComponent(dfWsURL);\n    }\n    if (!window.DFSignals.wsurl) {\n        console.info(\"Unable to get the websocket URL in the '\" + cookieName + \"' cookie.\");\n        return;\n    }\n    const connection = new WebSocket(window.DFSignals.wsurl);\n    /* cannot use header or cookies (cookies may change after the initial connection)\n    *  so we use GET parameter\n    *  */\n    connection.onopen = () => {\n        window.DFSignals.connection = connection;\n        for (let i = 0; i < window.DFSignals.buffer.length; i++) {\n            connection.send(window.DFSignals.buffer[i]);\n        }\n        window.DFSignals.buffer = [];\n    };\n    connection.onmessage = (e) => {\n        console.debug('received call ' + e.data + ' from server.')\n        const msg = JSON.parse(e.data);\n        // noinspection JSUnresolvedVariable\n        if (msg.signal && msg.signal_id) {\n            window.DFSignals.call(msg.signal, msg.opts, msg.signal_id);\n        }\n    };\n    connection.onerror = (e) => {\n        console.error(\"WS error: \" + e);\n    };\n    connection.onclose = () => {\n        window.DFSignals.connection = null;\n        setTimeout(websocketConnect, 3000);\n    }\n}\n\nfunction call(signal, opts, id) {\n    /*\"\"\"\n    .. function:: call(signal, opts, id)\n\n        Call a signal.\n        If the signal is also defined in the Python server and available to the user, then the Python signal is also triggered.\n\n        :param string signal: Name of the called signal.\n        :param object opts: Object with signal arguments.\n        :param string id: Unique id of each signal triggered by the server. Do not use it yourself.\n        :returns: always `false`.\n    */\n    // if (window.DFSignals.registry[signal] === undefined) {\n    //     console.debug('unknown call \"' + signal + '\" (from both client and server).');\n    //     return false;\n    // } else\n    if ((id !== undefined) && (window.DFSignals.registry[id] !== undefined)) {\n        return false;\n    } else if (id !== undefined) {\n        window.DFSignals.registry[id] = true;\n    }\n    if (window.DFSignals.registry[signal] !== undefined) {\n        console.debug('call \"' + signal + '\"', opts);\n        for (let i = 0; i < window.DFSignals.registry[signal].length; i += 1) {\n            window.DFSignals.registry[signal][i](opts, id);\n        }\n    }\n    if (id === undefined) {\n        console.debug('call from client: \"' + signal + '\"', opts);\n        const msg = JSON.stringify({signal: signal, opts: opts});\n        if (window.DFSignals.connection) {\n            window.DFSignals.connection.send(msg);\n        } else {\n            window.DFSignals.buffer.push(msg);\n        }\n    }\n\n    return false;\n}\n\nfunction connect(signal, fn) {\n    /*\"\"\"\n    .. function:: connect(signal, fn)\n\n        Connect a javascript code to the given signal name.\n\n        :param string signal: Name of the signal.\n        :param function fn: Function that takes a single object as argument. The properties of this object are the signal arguments.\n        :returns: nothing.\n    */\n    if (window.DFSignals.registry[signal] === undefined) {\n        window.DFSignals.registry[signal] = [];\n    }\n    window.DFSignals.registry[signal].push(fn);\n}\n\ndocument.addEventListener(\"DOMContentLoaded\", websocketConnect);\n\nwindow.DFSignals.call = call;\nwindow.DFSignals.connect = connect;\n",
-        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n\nexport const htmlAfter = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalNextSibling = elt.nextSibling;\n        elt.insertAdjacentHTML('afterend', opts.content);\n        let sibling = elt.nextSibling;\n        while (sibling && (sibling !== originalNextSibling)) {\n            sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            sibling = sibling.nextSibling;\n        }\n    });\n};\nexport const htmlAppend = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalLastChild = elt.lastChild;\n        elt.insertAdjacentHTML('beforeend', opts.content);\n        let child = elt.lastChild;\n        while (child && (child !== originalLastChild)) {\n            child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            child = child.previousSibling;\n        }\n    });\n};\nexport const htmlPrepend = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalFirstChild = elt.firstChild;\n        elt.insertAdjacentHTML('afterbegin', opts.content);\n        let child = elt.firstChild;\n        while (child && (child !== originalFirstChild)) {\n            child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            child = child.nextSibling;\n        }\n    });\n};\nexport const htmlBefore = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalPreviousSibling = elt.previousSibling;\n        elt.insertAdjacentHTML('beforebegin', opts.content);\n        let sibling = elt.previousSibling;\n        while (sibling && (sibling !== originalPreviousSibling)) {\n            sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            sibling = sibling.previousSibling;\n        }\n    });\n};\nexport const htmlContent = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.innerHTML = opts.content;\n        let child = elt.firstChild;\n        while (child) {\n            child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            child = child.nextSibling;\n        }\n    });\n};\nexport const htmlReplaceWith = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const previousSibling = elt.previousSibling;\n        const nextSibling = elt.nextSibling;\n        const parentNode = elt.parentNode;\n        elt.outerHTML = opts.content;\n        let sibling = parentNode.firstChild;\n        if (previousSibling) {\n            sibling = previousSibling.nextSibling;\n        }\n        while (sibling && (sibling !== nextSibling)) {\n            sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            sibling = sibling.nextSibling;\n        }\n    });\n};\nexport const htmlEmpty = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        while (elt.firstChild) {\n            elt.removeChild(elt.firstChild);\n        }\n    });\n};\nexport const htmlRemove = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.parentNode.removeChild(elt);\n    });\n};\nexport const htmlText = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.textContent = opts.content;\n    });\n};\n",
-        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n\nimport {htmlFormsSet, htmlFormsSetAll} from \"./forms\";\nimport {\n    htmlAfter,\n    htmlAppend,\n    htmlBefore,\n    htmlContent,\n    htmlEmpty,\n    htmlPrepend,\n    htmlRemove,\n    htmlReplaceWith, htmlText\n} from \"./html\";\n\nconst htmlAddClass = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.classList.add(opts.class_name)\n    });\n};\nconst htmlRemoveClass = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.classList.remove(opts.class_name);\n    });\n};\nconst htmlRemoveAttr = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.removeAttribute(opts.attr_name);\n    });\n};\nconst htmlAddAttribute = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.setAttribute(opts.attr_name, opts.attr_value);\n    });\n};\nconst htmlBooleanAttribute = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        if (opts.value) {\n            elt.setAttribute(opts.name, opts.name);\n        } else {\n            elt.removeAttribute(opts.name)\n        }\n    });\n};\nconst htmlDownloadFile = (opts) => {\n    const save = document.createElement('a');\n    save.href = opts.url;\n    save.target = '_blank';\n    save.download = opts.filename || 'unknown';\n    const evt = new MouseEvent('click', {view: window, bubbles: true, cancelable: false});\n    save.dispatchEvent(evt);\n    (window.URL || window.webkitURL).revokeObjectURL(save.href);\n};\nconst htmlFocus = (opts) => {\n    const elt = document.querySelector(opts.selector);\n    if (elt) {\n        elt.focus({preventScroll: false});\n    }\n};\n\nfunction connectSignals() {\n\n    window.DFSignals.connect('html.after', htmlAfter);\n    /*\"\"\"\n    .. function:: html.after(opts)\n\n        Insert content, specified by the parameter, after each element in the set of matched elements.\n        Equivalent to `$().after()` or `.insertAdjacentHTML('afterend', ...)`.\n        Trigger a `DOMContentAdded` event on the added content.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.after', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.after', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n\n    window.DFSignals.connect('html.append', htmlAppend);\n    /*\"\"\"\n    .. function:: html.append(opts)\n\n        Insert content, specified by the parameter, to the end of each element in the set of matched elements.\n        Equivalent to `$().append()` or `.insertAdjacentHTML('beforeend', ...)`.\n        Trigger a `DOMContentAdded` event on the added content.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.append', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.append', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n\n    window.DFSignals.connect('html.prepend', htmlPrepend);\n\n    /*\"\"\"\n    .. function:: html.prepend(opts)\n\n        Insert content, specified by the parameter, to the beginning of each element in the set of matched elements.\n        Equivalent to `$().prepend()` or `.insertAdjacentHTML('afterbegin', ...)`.\n        Trigger a `DOMContentAdded` event on the added content.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.prepend', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.prepend', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n\n    window.DFSignals.connect('html.before', htmlBefore);\n    /*\"\"\"\n    .. function:: html.before(opts)\n\n        Insert content, specified by the parameter, before each element in the set of matched elements..\n        Equivalent to `$().before()` or `.insertAdjacentHTML('beforebegin', ...)`.\n        Trigger a `DOMContentAdded` event on the added content.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.before', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.before', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n    window.DFSignals.connect('html.content', htmlContent);\n    /*\"\"\"\n    .. function:: html.content(opts)\n\n        set the HTML contents of every matched element.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.content', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.content', to=WINDOW, selector=\"#obj\", content= \"<span>hello</span>\")\n\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n    */\n\n    window.DFSignals.connect('html.replace_with', htmlReplaceWith);\n    /*\"\"\"\n    .. function:: html.replace_with(opts)\n\n        Replace each element in the set of matched elements with the provided new content.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.replace_with', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.replace_with', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n\n    window.DFSignals.connect('html.empty', htmlEmpty);\n    /*\"\"\"\n    .. function:: html.empty(opts)\n\n        Remove all child nodes of the set of matched elements from the DOM.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.empty', {selector: \"#obj\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.empty', to=WINDOW, selector=\"#obj\")\n\n        :param string selector: HTML selector\n\n    */\n\n    window.DFSignals.connect('html.remove', htmlRemove);\n    /*\"\"\"\n    .. function:: html.remove(opts)\n\n        Remove the set of matched elements from the DOM.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.remove', {selector: \"#obj\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.remove', to=WINDOW, selector=\"#obj\")\n\n        :param string selector: HTML selector\n\n    */\n\n    window.DFSignals.connect('html.add_class', htmlAddClass);\n    /*\"\"\"\n    .. function:: html.add_class(opts)\n\n        Adds the specified class(es) to each of the set of matched elements.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.add_class', {selector: \"#obj\", class_name: \"myclass\"});\n\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.add_class', to=WINDOW, selector=\"#obj\", class_name=\"myclass\")\n\n\n        :param string selector: HTML selector\n        :param string class_name: new class\n\n    */\n    window.DFSignals.connect('html.remove_class', htmlRemoveClass);\n    /*\"\"\"\n    .. function:: html.remove_class(opts)\n\n        Remove a single class, multiple classes, or all classes from each element in the set of matched elements.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.remove_class', {selector: \"#obj\", class_name: \"class\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.remove_class', to=WINDOW, selector=\"#obj\", class_name=\"attr\")\n\n        :param string selector: HTML selector\n        :param string class_name: class to remove\n\n    */\n    window.DFSignals.connect('html.remove_attr', htmlRemoveAttr);\n    /*\"\"\"\n    .. function:: html.remove_attr(opts)\n\n        Remove an attribute from each element in the set of matched elements.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.remove_attr', {selector: \"#obj\", attr_name: \"attr\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.remove_attr', to=WINDOW, selector=\"#obj\", attr_name=\"attr\")\n\n        :param string selector: HTML selector\n        :param string attr_name: attribute to remove\n\n    */\n\n    window.DFSignals.connect('html.add_attribute', htmlAddAttribute);\n    /*\"\"\"\n    .. function:: html.add_attribute(opts)\n\n        Add an attribute to each element matched by the given selector.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.add_attribute', {selector: \"#obj\", attr_name: \"data-df\", attr_value: \"value\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.add_attribute', to=WINDOW, selector=\"#obj\", attr_name=\"data-df\", attr_value= \"value\")\n\n\n        :param string selector: HTML selector\n        :param string attr_name: name of the attribute to add\n        :param string attr_value: value of the attribute to add\n\n    */\n    window.DFSignals.connect('html.boolean_attribute', htmlBooleanAttribute);\n    /*\"\"\"\n    .. function:: html.boolean_attribute(opts)\n\n        Set or remove a boolean attribute. Always set the value of the added attribute to its name.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.boolean_attribute', {selector: \"#input\", name: \"checked\", value: true});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.boolean_attribute', to=WINDOW, selector=\"#input\", name=\"checked\", value=True)\n\n\n        :param string selector: HTML selector\n        :param string name: name of the attribute to add\n        :param string value: if True, add the attribute, if False, remove the attribute\n\n    */\n\n\n    window.DFSignals.connect('html.text', htmlText);\n    /*\"\"\"\n    .. function:: html.text(opts)\n\n        Set the text contents of the matched elements.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.text', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.text', to=WINDOW, selector=\"#obj\", content= \"<span>hello</span>\")\n\n\n        :param string selector: HTML selector\n        :param string content: new HTML content\n\n    */\n\n    window.DFSignals.connect('html.download_file', htmlDownloadFile);\n    /*\"\"\"\n    .. function:: html.download_file(opts)\n\n        Force the client to download the given file.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.download_file', {url: \"http://example.org/test.zip\", filename: \"test.zip\"});\n\n    .. code-block:: python\n\n        trigger(window_info, 'html.download_file', to=WINDOW, url=\"http://example.org/test.zip\", filename=\"test.zip\")\n\n        :param string url: URL of the file\n        :param string filename: name of the file\n\n    */\n\n\n    window.DFSignals.connect('html.focus', htmlFocus);\n    /*\"\"\"\n    .. function:: html.focus(opts)\n\n        Set the focus to the matched element.\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.focus', {selector: \"#obj\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.focus', to=WINDOW, selector=\"#obj\")\n\n        :param string selector: HTML selector\n\n    */\n\n    window.DFSignals.connect('html.forms.set', htmlFormsSet);\n    /*\"\"\"\n    .. function:: html.forms.set(opts)\n\n        Set the value of a form input\n\n        .. code-block:: javascript\n\n            window.DFSignals.call('html.forms.set', {selector: \"[name=title]\", value: \"new title\"});\n\n        .. code-block:: python\n\n            trigger(window_info, 'html.forms.set', to=WINDOW, selector=\"[name=title]\", value=\"new_title\")\n\n        :param string selector: HTML selector\n\n    */\n}\n\ndocument.addEventListener(\"DOMContentLoaded\", connectSignals);\n",
-        "export function serializeForm(form) {\n    /*\n    Serialize a HTMLFormElement as a list of {name: <field name>, value: <field value>}\n    disabled/reset/submit/buttonf fields are ignored\n     */\n    var serialized = [];\n    // Loop through each field in the form\n    for (var i = 0; i < form.elements.length; i++) {\n        var field = form.elements[i];\n        // Respect the same rules as jQuery's serializeArray\n        if (!field.name || field.disabled || field.type === 'reset' || field.type === 'submit' || field.type === 'button') {\n            continue;\n        }\n        if (field.type === \"file\") { // just returns the name of selected files\n            for (var n = 0; n < field.files.length; n++) {\n                serialized.push({ name: field.name, value: field.files[n].name });\n            }\n        }\n        else if (field.type === 'select-multiple') { // get all selected options\n            for (var n = 0; n < field.selectedOptions.length; n++) {\n                serialized.push({ name: field.name, value: field.selectedOptions[n].value });\n            }\n        }\n        else if ((field.type !== 'checkbox' && field.type !== 'radio') || field.checked) {\n            serialized.push({ name: field.name, value: field.value });\n        }\n    }\n    return serialized;\n}\nfunction setFormFieldValue(form, name, value) {\n    var item = form.elements.namedItem(name);\n    if (item === null) {\n        return;\n    }\n    else if (item instanceof RadioNodeList) {\n        if ((value === true) || (value === false)) {\n            item.forEach(function (input) {\n                input.checked = value;\n            });\n        }\n        else if (Array.isArray(value)) {\n            var valuesSet_1 = new Set(value);\n            item.forEach(function (input) {\n                input.checked = valuesSet_1.has(input.value);\n            });\n        }\n        else {\n            item.forEach(function (input) {\n                input.checked = input.value === value;\n            });\n        }\n    }\n    else if (item instanceof HTMLTextAreaElement) {\n        item.value = value;\n    }\n    else if ((item instanceof HTMLInputElement) && (item.type === \"checkbox\")) {\n        if (value === true) {\n            item.checked = true;\n        }\n        else if (value === false) {\n            item.checked = false;\n        }\n        else {\n            item.value = value;\n        }\n    }\n    else if (item instanceof HTMLSelectElement) {\n        var options = item.options;\n        if (Array.isArray(value)) {\n            var valuesSet = new Set(value);\n            for (var i = 0; i < options.length; i++) {\n                options[i].selected = valuesSet.has(options[i].value);\n            }\n        }\n        else {\n            for (var i = 0; i < options.length; i++) {\n                options[i].selected = options[i].value === value;\n            }\n        }\n    }\n    else if (item instanceof HTMLInputElement) {\n        item.value = value;\n    }\n}\nexport function htmlFormsSet(opts) {\n    document.querySelectorAll(opts.selector).forEach(function (form) {\n        opts.values.forEach(function (values) {\n            setFormFieldValue(form, values.name, values.value);\n        });\n    });\n}\nfunction DOMContentAdded(evt) {\n    /*\n    search all HTML elements with an attribute \"data-df-signal\" that contains a JSON list of Signal objects:\n    {\n        name: \"name of the signal to call\",  (required)\n        on: \"name of the listened event\",\n        opts: \"extra options\",               (optional)\n        form: \"name of option to add to opts that contains the serialized form\",  (optional)\n        value: \"name of option to add to opts that contains the value\",  (optional)\n        prevent: preventDefault               (optional, defaults to true for on==\"submit\" or \"click\" else false )\n    }\n\n    When the listened event is not given, the listened event is\n        * \"submit\" for forms,\n        * \"click\" for \"reset\"/\"submit\"/\"button\" input fields,\n        * \"change\" for other fields.\n\n    Using on a HTML form:\n    ```html\n    <form data-df-signal='[{\"name\": \"signal.name\", \"on\": \"change\", \"form\": \"form_data\", \"opts\": {\"id\": 42} }]'>\n        <input type=\"text\" name=\"title\" value=\"df_websockets\">\n    </form>```\n    or, using the Django templating system:\n    ```html\n    {% load df_websockets %}\n    <form {% js_call \"signal.name\" on=\"change\" form=\"form_data\" id=42 %}>\n        <input type=\"text\" name=\"title\" value=\"df_websockets\">\n    </form>```\n\n    When the field \"title\" is modified, a signal \"signal.name\" is triggered on the server (via the websocket) with\n    the following arguments:\n    ```python\n    form_data = [{\"name\": \"title\", \"value\": \"df_websockets\"}]\n    id = 42\n    ```\n\n    Using on a HTML form input field:\n    ```html\n    <form>\n        <input type=\"text\" name=\"title\" data-df-signal='[{\"name\": \"signal.name\", \"on\": \"change\", \"value\": \"title\", \"opts\": {\"id\": 42} }]'>\n    </form>```\n    or, using the Django templating system:\n    ```html\n    {% load df_websockets %}\n    <form>\n        <input type=\"text\" name=\"title\" {% js_call \"signal.name\" on=\"change\" value=\"title\" id=42 %}>\n    </form>```\n\n    When the field \"title\" is modified, a signal \"signal.name\" is triggered on the server (via the websocket) with\n    the following arguments:\n    ```python\n    title = \"new title value\"\n    id = 42\n    ```\n     */\n    evt.target.querySelectorAll(\"[data-df-signal]\").forEach(function (target) {\n        var signals = JSON.parse(target.getAttribute(\"data-df-signal\"));\n        signals.forEach(function (signal) {\n            var eventName = signal.on;\n            if (!eventName) {\n                if (target.tagName === \"FORM\") {\n                    eventName = \"submit\";\n                }\n                else if ((target.tagName === \"INPUT\" && !(target.type === 'reset' || target.type === 'submit' || target.type === 'button')) || (target.tagName === \"TEXTAREA\")) {\n                    eventName = \"change\";\n                }\n                else {\n                    eventName = \"click\";\n                }\n            }\n            var callback = function (evt) {\n                // noinspection JSUnresolvedVariable\n                var prevent = signal.prevent;\n                var opts = signal.opts || {};\n                if (signal.form) {\n                    opts[signal.form] = serializeForm(target);\n                }\n                if (signal.value) {\n                    if (target.type === \"file\") { // just returns the name of selected files\n                        opts[signal.value] = [];\n                        for (var n = 0; n < target.files.length; n++) {\n                            opts[signal.value].push(target.files[n].name);\n                        }\n                    }\n                    else if (target.type === 'select-multiple') { // get all selected options\n                        opts[signal.value] = [];\n                        for (var n = 0; n < target.selectedOptions.length; n++) {\n                            opts[signal.value].push(target.selectedOptions[n].value);\n                        }\n                    }\n                    else if (target.type === 'checkbox' || target.type === 'radio') {\n                        opts[signal.value] = target.checked;\n                    }\n                    else {\n                        opts[signal.value] = target.value;\n                    }\n                }\n                window.DFSignals.call(signal.name, opts);\n                if (prevent === true || (prevent === null && eventName !== \"change\")) {\n                    evt.preventDefault();\n                }\n            };\n            target.addEventListener(eventName, callback);\n        });\n    });\n}\ndocument.addEventListener(\"DOMContentAdded\", function (evt) {\n    window.setTimeout(function () {\n        DOMContentAdded(evt);\n    }, 200);\n    // awful trick for being sure that our addEventListener is the last.\n    // allows things like CKEditor to push its content to the textarea before sending the content of the form.\n});\ndocument.addEventListener(\"DOMContentLoaded\", function (evt) {\n    window.setTimeout(function () {\n        DOMContentAdded(evt);\n    }, 200);\n    // awful trick for being sure that our addEventListener is the last.\n    // allows things like CKEditor to push its content to the textarea before sending the content of the form.\n});\n",
+        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n(() => {\n\n  window.DFSignals = {\n    connection: null,\n    buffer: [],\n    registry: {},\n    wsurl: null\n  };\n\n  function getCookie(cname) {\n    const name = cname + \"=\";\n    const decodedCookie = decodeURIComponent(document.cookie);\n    const ca = decodedCookie.split(';');\n    for (let i = 0; i < ca.length; i++) {\n      let c = ca[i];\n      while (c.charAt(0) === ' ') {\n        c = c.substring(1);\n      }\n      if (c.indexOf(name) === 0) {\n        return c.substring(name.length, c.length);\n      }\n    }\n    return \"\";\n  }\n\n  function websocketConnect() {\n    const cookieName = \"dfwsurl\";\n    if (window.DFSignals.wsurl === null) {\n      const dfWsURL = getCookie(cookieName);\n      window.DFSignals.wsurl = decodeURIComponent(dfWsURL);\n    }\n    if (!window.DFSignals.wsurl) {\n      console.info(\"Unable to get the websocket URL in the '\" + cookieName + \"' cookie.\");\n      return;\n    }\n    const connection = new WebSocket(window.DFSignals.wsurl);\n    /* cannot use header or cookies (cookies may change after the initial connection)\n    *  so we use GET parameter\n    *  */\n    connection.onopen = () => {\n      window.DFSignals.connection = connection;\n      for (let i = 0; i < window.DFSignals.buffer.length; i++) {\n        connection.send(window.DFSignals.buffer[i]);\n      }\n      window.DFSignals.buffer = [];\n    };\n    connection.onmessage = (e) => {\n      console.debug('received call ' + e.data + ' from server.')\n      const msg = JSON.parse(e.data);\n      // noinspection JSUnresolvedVariable\n      if (msg.signal && msg.signal_id) {\n        window.DFSignals.call(msg.signal, msg.opts, msg.signal_id);\n      }\n    };\n    connection.onerror = (e) => {\n      console.error(\"WS error: \" + e);\n    };\n    connection.onclose = () => {\n      window.DFSignals.connection = null;\n      setTimeout(websocketConnect, 3000);\n    }\n  }\n\n  function call(signal, opts, id) {\n    /*\"\"\"\n    .. function:: call(signal, opts, id)\n\n        Call a signal.\n        If the signal is also defined in the Python server and available to the user, then the Python signal is also triggered.\n\n        :param string signal: Name of the called signal.\n        :param object opts: Object with signal arguments.\n        :param string id: Unique id of each signal triggered by the server. Do not use it yourself.\n        :returns: always `false`.\n    */\n    // if (window.DFSignals.registry[signal] === undefined) {\n    //     console.debug('unknown call \"' + signal + '\" (from both client and server).');\n    //     return false;\n    // } else\n    if ((id !== undefined) && (window.DFSignals.registry[id] !== undefined)) {\n      return false;\n    } else if (id !== undefined) {\n      window.DFSignals.registry[id] = true;\n    }\n    if (window.DFSignals.registry[signal] !== undefined) {\n      console.debug('call \"' + signal + '\"', opts);\n      for (let i = 0; i < window.DFSignals.registry[signal].length; i += 1) {\n        window.DFSignals.registry[signal][i](opts, id);\n      }\n    }\n    if (id === undefined) {\n      console.debug('call from client: \"' + signal + '\"', opts);\n      const msg = JSON.stringify({signal: signal, opts: opts});\n      if (window.DFSignals.connection) {\n        window.DFSignals.connection.send(msg);\n      } else {\n        window.DFSignals.buffer.push(msg);\n      }\n    }\n\n    return false;\n  }\n\n  function connect(signal, fn) {\n    /*\"\"\"\n    .. function:: connect(signal, fn)\n\n        Connect a javascript code to the given signal name.\n\n        :param string signal: Name of the signal.\n        :param function fn: Function that takes a single object as argument. The properties of this object are the signal arguments.\n        :returns: nothing.\n    */\n    if (window.DFSignals.registry[signal] === undefined) {\n      window.DFSignals.registry[signal] = [];\n    }\n    window.DFSignals.registry[signal].push(fn);\n  }\n\n  document.addEventListener(\"DOMContentLoaded\", websocketConnect);\n\n  window.DFSignals.call = call;\n  window.DFSignals.connect = connect;\n\n})();\n",
+        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n\nexport const htmlAfter = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalNextSibling = elt.nextSibling;\n        elt.insertAdjacentHTML('afterend', opts.content);\n        let sibling = elt.nextSibling;\n        while (sibling && (sibling !== originalNextSibling)) {\n            if (sibling.querySelectorAll) {\n                sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            }\n            sibling = sibling.nextSibling;\n        }\n    });\n};\nexport const htmlAppend = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalLastChild = elt.lastChild;\n        elt.insertAdjacentHTML('beforeend', opts.content);\n        let child = elt.lastChild;\n        while (child && (child !== originalLastChild)) {\n            if (child.querySelectorAll) {\n                child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            }\n            child = child.previousSibling;\n        }\n    });\n};\nexport const htmlPrepend = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalFirstChild = elt.firstChild;\n        elt.insertAdjacentHTML('afterbegin', opts.content);\n        let child = elt.firstChild;\n        while (child && (child !== originalFirstChild)) {\n            if (child.querySelectorAll) {\n                child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            }\n            child = child.nextSibling;\n        }\n    });\n};\nexport const htmlBefore = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        const originalPreviousSibling = elt.previousSibling;\n        elt.insertAdjacentHTML('beforebegin', opts.content);\n        let sibling = elt.previousSibling;\n        while (sibling && (sibling !== originalPreviousSibling)) {\n            if (sibling.querySelectorAll) {\n                sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            }\n            sibling = sibling.previousSibling;\n        }\n    });\n};\nexport const htmlContent = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.innerHTML = opts.content;\n        let child = elt.firstChild;\n        while (child) {\n            if (child.querySelectorAll) {\n                child.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n            }\n            child = child.nextSibling;\n        }\n    });\n};\nexport const htmlReplaceWith = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n            const previousSibling = elt.previousSibling;\n            const nextSibling = elt.nextSibling;\n            const parentNode = elt.parentNode;\n            elt.outerHTML = opts.content;\n            let sibling = parentNode.firstChild;\n            if (previousSibling) {\n                sibling = previousSibling.nextSibling;\n            }\n            while (sibling && (sibling !== nextSibling)) {\n                if (sibling.querySelectorAll) {\n                    sibling.dispatchEvent(new Event('DOMContentAdded', {bubbles: true}));\n                }\n                sibling = sibling.nextSibling;\n            }\n        }\n    )\n    ;\n};\nexport const htmlEmpty = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        while (elt.firstChild) {\n            elt.removeChild(elt.firstChild);\n        }\n    });\n};\nexport const htmlRemove = opts => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.parentNode.removeChild(elt);\n    });\n};\nexport const htmlText = (opts) => {\n    document.querySelectorAll(opts.selector).forEach(elt => {\n        elt.textContent = opts.content;\n    });\n};\n",
+        "////////////////////////////////////////////////////////////////////////////////\n// This file is part of df_websockets                                          /\n//                                                                             /\n// Copyright (C) 2020 Matthieu Gallet <github@19pouces.net>                    /\n// All Rights Reserved                                                         /\n//                                                                             /\n// You may use, distribute and modify this code under the                      /\n// terms of the (BSD-like) CeCILL-B license.                                   /\n//                                                                             /\n// You should have received a copy of the CeCILL-B license with                /\n// this file. If not, please visit:                                            /\n// https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /\n// or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /\n//                                                                             /\n////////////////////////////////////////////////////////////////////////////////\n\nimport {htmlFormsSet} from \"./forms\";\nimport {\n  htmlAfter,\n  htmlAppend,\n  htmlBefore,\n  htmlContent,\n  htmlEmpty,\n  htmlPrepend,\n  htmlRemove,\n  htmlReplaceWith, htmlText\n} from \"./html\";\n\n(\n  () => {\n    const htmlAddClass = opts => {\n      document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.classList.add(opts.class_name)\n      });\n    };\n    const htmlRemoveClass = (opts) => {\n      document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.classList.remove(opts.class_name);\n      });\n    };\n    const htmlRemoveAttr = (opts) => {\n      document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.removeAttribute(opts.attr_name);\n      });\n    };\n    const htmlAddAttribute = (opts) => {\n      document.querySelectorAll(opts.selector).forEach(elt => {\n        // noinspection JSUnresolvedVariable\n        elt.setAttribute(opts.attr_name, opts.attr_value);\n      });\n    };\n    const htmlBooleanAttribute = (opts) => {\n      document.querySelectorAll(opts.selector).forEach(elt => {\n        if (opts.value) {\n          elt.setAttribute(opts.name, opts.name);\n        } else {\n          elt.removeAttribute(opts.name)\n        }\n      });\n    };\n    const htmlDownloadFile = (opts) => {\n      const save = document.createElement('a');\n      save.href = opts.url;\n      save.target = '_blank';\n      save.download = opts.filename || 'unknown';\n      const evt = new MouseEvent('click', {view: window, bubbles: true, cancelable: false});\n      save.dispatchEvent(evt);\n      (window.URL || window.webkitURL).revokeObjectURL(save.href);\n    };\n    const htmlFocus = (opts) => {\n      const elt = document.querySelector(opts.selector);\n      if (elt) {\n        elt.focus({preventScroll: false});\n      }\n    };\n\n    function connectSignals() {\n\n      window.DFSignals.connect('html.after', htmlAfter);\n      /*\"\"\"\n      .. function:: html.after(opts)\n\n          Insert content, specified by the parameter, after each element in the set of matched elements.\n          Equivalent to `$().after()` or `.insertAdjacentHTML('afterend', ...)`.\n          Trigger a `DOMContentAdded` event on the added content.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.after', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.after', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n\n      window.DFSignals.connect('html.append', htmlAppend);\n      /*\"\"\"\n      .. function:: html.append(opts)\n\n          Insert content, specified by the parameter, to the end of each element in the set of matched elements.\n          Equivalent to `$().append()` or `.insertAdjacentHTML('beforeend', ...)`.\n          Trigger a `DOMContentAdded` event on the added content.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.append', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.append', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n\n      window.DFSignals.connect('html.prepend', htmlPrepend);\n\n      /*\"\"\"\n      .. function:: html.prepend(opts)\n\n          Insert content, specified by the parameter, to the beginning of each element in the set of matched elements.\n          Equivalent to `$().prepend()` or `.insertAdjacentHTML('afterbegin', ...)`.\n          Trigger a `DOMContentAdded` event on the added content.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.prepend', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.prepend', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n\n      window.DFSignals.connect('html.before', htmlBefore);\n      /*\"\"\"\n      .. function:: html.before(opts)\n\n          Insert content, specified by the parameter, before each element in the set of matched elements..\n          Equivalent to `$().before()` or `.insertAdjacentHTML('beforebegin', ...)`.\n          Trigger a `DOMContentAdded` event on the added content.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.before', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.before', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n      window.DFSignals.connect('html.content', htmlContent);\n      /*\"\"\"\n      .. function:: html.content(opts)\n\n          set the HTML contents of every matched element.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.content', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.content', to=WINDOW, selector=\"#obj\", content= \"<span>hello</span>\")\n\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n      */\n\n      window.DFSignals.connect('html.replace_with', htmlReplaceWith);\n      /*\"\"\"\n      .. function:: html.replace_with(opts)\n\n          Replace each element in the set of matched elements with the provided new content.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.replace_with', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.replace_with', to=WINDOW, selector=\"#obj\", content=\"<span>hello</span>\")\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n\n      window.DFSignals.connect('html.empty', htmlEmpty);\n      /*\"\"\"\n      .. function:: html.empty(opts)\n\n          Remove all child nodes of the set of matched elements from the DOM.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.empty', {selector: \"#obj\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.empty', to=WINDOW, selector=\"#obj\")\n\n          :param string selector: HTML selector\n\n      */\n\n      window.DFSignals.connect('html.remove', htmlRemove);\n      /*\"\"\"\n      .. function:: html.remove(opts)\n\n          Remove the set of matched elements from the DOM.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.remove', {selector: \"#obj\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.remove', to=WINDOW, selector=\"#obj\")\n\n          :param string selector: HTML selector\n\n      */\n\n      window.DFSignals.connect('html.add_class', htmlAddClass);\n      /*\"\"\"\n      .. function:: html.add_class(opts)\n\n          Adds the specified class(es) to each of the set of matched elements.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.add_class', {selector: \"#obj\", class_name: \"myclass\"});\n\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.add_class', to=WINDOW, selector=\"#obj\", class_name=\"myclass\")\n\n\n          :param string selector: HTML selector\n          :param string class_name: new class\n\n      */\n      window.DFSignals.connect('html.remove_class', htmlRemoveClass);\n      /*\"\"\"\n      .. function:: html.remove_class(opts)\n\n          Remove a single class, multiple classes, or all classes from each element in the set of matched elements.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.remove_class', {selector: \"#obj\", class_name: \"class\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.remove_class', to=WINDOW, selector=\"#obj\", class_name=\"attr\")\n\n          :param string selector: HTML selector\n          :param string class_name: class to remove\n\n      */\n      window.DFSignals.connect('html.remove_attr', htmlRemoveAttr);\n      /*\"\"\"\n      .. function:: html.remove_attr(opts)\n\n          Remove an attribute from each element in the set of matched elements.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.remove_attr', {selector: \"#obj\", attr_name: \"attr\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.remove_attr', to=WINDOW, selector=\"#obj\", attr_name=\"attr\")\n\n          :param string selector: HTML selector\n          :param string attr_name: attribute to remove\n\n      */\n\n      window.DFSignals.connect('html.add_attribute', htmlAddAttribute);\n      /*\"\"\"\n      .. function:: html.add_attribute(opts)\n\n          Add an attribute to each element matched by the given selector.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.add_attribute', {selector: \"#obj\", attr_name: \"data-df\", attr_value: \"value\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.add_attribute', to=WINDOW, selector=\"#obj\", attr_name=\"data-df\", attr_value= \"value\")\n\n\n          :param string selector: HTML selector\n          :param string attr_name: name of the attribute to add\n          :param string attr_value: value of the attribute to add\n\n      */\n      window.DFSignals.connect('html.boolean_attribute', htmlBooleanAttribute);\n      /*\"\"\"\n      .. function:: html.boolean_attribute(opts)\n\n          Set or remove a boolean attribute. Always set the value of the added attribute to its name.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.boolean_attribute', {selector: \"#input\", name: \"checked\", value: true});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.boolean_attribute', to=WINDOW, selector=\"#input\", name=\"checked\", value=True)\n\n\n          :param string selector: HTML selector\n          :param string name: name of the attribute to add\n          :param string value: if True, add the attribute, if False, remove the attribute\n\n      */\n\n\n      window.DFSignals.connect('html.text', htmlText);\n      /*\"\"\"\n      .. function:: html.text(opts)\n\n          Set the text contents of the matched elements.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.text', {selector: \"#obj\", content: \"<span>hello</span>\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.text', to=WINDOW, selector=\"#obj\", content= \"<span>hello</span>\")\n\n\n          :param string selector: HTML selector\n          :param string content: new HTML content\n\n      */\n\n      window.DFSignals.connect('html.download_file', htmlDownloadFile);\n      /*\"\"\"\n      .. function:: html.download_file(opts)\n\n          Force the client to download the given file.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.download_file', {url: \"http://example.org/test.zip\", filename: \"test.zip\"});\n\n      .. code-block:: python\n\n          trigger(window_info, 'html.download_file', to=WINDOW, url=\"http://example.org/test.zip\", filename=\"test.zip\")\n\n          :param string url: URL of the file\n          :param string filename: name of the file\n\n      */\n\n\n      window.DFSignals.connect('html.focus', htmlFocus);\n      /*\"\"\"\n      .. function:: html.focus(opts)\n\n          Set the focus to the matched element.\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.focus', {selector: \"#obj\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.focus', to=WINDOW, selector=\"#obj\")\n\n          :param string selector: HTML selector\n\n      */\n\n      window.DFSignals.connect('html.forms.set', htmlFormsSet);\n      /*\"\"\"\n      .. function:: html.forms.set(opts)\n\n          Set the value of a form input\n\n          .. code-block:: javascript\n\n              window.DFSignals.call('html.forms.set', {selector: \"[name=title]\", value: \"new title\"});\n\n          .. code-block:: python\n\n              trigger(window_info, 'html.forms.set', to=WINDOW, selector=\"[name=title]\", value=\"new_title\")\n\n          :param string selector: HTML selector\n\n      */\n    }\n\n    document.addEventListener(\"DOMContentLoaded\", connectSignals);\n  }\n)();\n",
+        "export function serializeForm(form) {\n    /*\n    Serialize a HTMLFormElement as a list of {name: <field name>, value: <field value>}\n    disabled/reset/submit/buttonf fields are ignored\n     */\n    var serialized = [];\n    // Loop through each field in the form\n    for (var i = 0; i < form.elements.length; i++) {\n        var field = form.elements[i];\n        // Respect the same rules as jQuery's serializeArray\n        if (!field.name || field.disabled || field.type === 'reset' || field.type === 'submit' || field.type === 'button') {\n            continue;\n        }\n        if (field.type === \"file\") { // just returns the name of selected files\n            for (var n = 0; n < field.files.length; n++) {\n                serialized.push({ name: field.name, value: field.files[n].name });\n            }\n        }\n        else if (field.type === 'select-multiple') { // get all selected options\n            for (var n = 0; n < field.selectedOptions.length; n++) {\n                serialized.push({ name: field.name, value: field.selectedOptions[n].value });\n            }\n        }\n        else if ((field.type !== 'checkbox' && field.type !== 'radio') || field.checked) {\n            serialized.push({ name: field.name, value: field.value });\n        }\n    }\n    return serialized;\n}\nexport function htmlFormsSet(opts) {\n    function setFormFieldValue(form, name, value) {\n        var item = form.elements.namedItem(name);\n        if (item === null) {\n            return;\n        }\n        else if (item instanceof RadioNodeList) {\n            if ((value === true) || (value === false)) {\n                item.forEach(function (input) {\n                    input.checked = value;\n                });\n            }\n            else if (Array.isArray(value)) {\n                var valuesSet_1 = new Set(value);\n                item.forEach(function (input) {\n                    input.checked = valuesSet_1.has(input.value);\n                });\n            }\n            else {\n                item.forEach(function (input) {\n                    input.checked = input.value === value;\n                });\n            }\n        }\n        else if (item instanceof HTMLTextAreaElement) {\n            item.value = value;\n        }\n        else if ((item instanceof HTMLInputElement) && (item.type === \"checkbox\")) {\n            if (value === true) {\n                item.checked = true;\n            }\n            else if (value === false) {\n                item.checked = false;\n            }\n            else {\n                item.value = value;\n            }\n        }\n        else if (item instanceof HTMLSelectElement) {\n            var options = item.options;\n            if (Array.isArray(value)) {\n                var valuesSet = new Set(value);\n                for (var i = 0; i < options.length; i++) {\n                    options[i].selected = valuesSet.has(options[i].value);\n                }\n            }\n            else {\n                for (var i = 0; i < options.length; i++) {\n                    options[i].selected = options[i].value === value;\n                }\n            }\n        }\n        else if (item instanceof HTMLInputElement) {\n            item.value = value;\n        }\n    }\n    document.querySelectorAll(opts.selector).forEach(function (form) {\n        opts.values.forEach(function (values) {\n            setFormFieldValue(form, values.name, values.value);\n        });\n    });\n}\n(function () {\n    function websocketForms(evt) {\n        /*\n        search all HTML elements with an attribute \"data-df-signal\" that contains a JSON list of Signal objects:\n        {\n            name: \"name of the signal to call\",  (required)\n            on: \"name of the listened event\",\n            opts: \"extra options\",               (optional)\n            form: \"name of option to add to opts that contains the serialized form\",  (optional)\n            value: \"name of option to add to opts that contains the value\",  (optional)\n            prevent: preventDefault               (optional, defaults to true for on==\"submit\" or \"click\" else false )\n        }\n\n        When the listened event is not given, the listened event is\n            * \"submit\" for forms,\n            * \"click\" for \"reset\"/\"submit\"/\"button\" input fields,\n            * \"change\" for other fields.\n\n        Using on a HTML form:\n        ```html\n        <form data-df-signal='[{\"name\": \"signal.name\", \"on\": \"change\", \"form\": \"form_data\", \"opts\": {\"id\": 42} }]'>\n            <input type=\"text\" name=\"title\" value=\"df_websockets\">\n        </form>```\n        or, using the Django templating system:\n        ```html\n        {% load df_websockets %}\n        <form {% js_call \"signal.name\" on=\"change\" form=\"form_data\" id=42 %}>\n            <input type=\"text\" name=\"title\" value=\"df_websockets\">\n        </form>```\n\n        When the field \"title\" is modified, a signal \"signal.name\" is triggered on the server (via the websocket) with\n        the following arguments:\n        ```python\n        form_data = [{\"name\": \"title\", \"value\": \"df_websockets\"}]\n        id = 42\n        ```\n\n        Using on a HTML form input field:\n        ```html\n        <form>\n            <input type=\"text\" name=\"title\" data-df-signal='[{\"name\": \"signal.name\", \"on\": \"change\", \"value\": \"title\", \"opts\": {\"id\": 42} }]'>\n        </form>```\n        or, using the Django templating system:\n        ```html\n        {% load df_websockets %}\n        <form>\n            <input type=\"text\" name=\"title\" {% js_call \"signal.name\" on=\"change\" value=\"title\" id=42 %}>\n        </form>```\n\n        When the field \"title\" is modified, a signal \"signal.name\" is triggered on the server (via the websocket) with\n        the following arguments:\n        ```python\n        title = \"new title value\"\n        id = 42\n        ```\n         */\n        if (!evt.target.querySelectorAll) {\n            return;\n        }\n        evt.target.querySelectorAll(\"[data-df-signal]\").forEach(function (target) {\n            var signals = JSON.parse(target.getAttribute(\"data-df-signal\"));\n            signals.forEach(function (signal) {\n                var eventName = signal.on;\n                if (!eventName) {\n                    if (target.tagName === \"FORM\") {\n                        eventName = \"submit\";\n                    }\n                    else if ((target.tagName === \"INPUT\" && !(target.type === 'reset' || target.type === 'submit' || target.type === 'button')) || (target.tagName === \"TEXTAREA\")) {\n                        eventName = \"change\";\n                    }\n                    else {\n                        eventName = \"click\";\n                    }\n                }\n                var callback = function (evt) {\n                    // noinspection JSUnresolvedVariable\n                    var prevent = signal.prevent;\n                    var opts = signal.opts || {};\n                    if (signal.form) {\n                        opts[signal.form] = serializeForm(target);\n                    }\n                    if (signal.value) {\n                        if (target.type === \"file\") { // just returns the name of selected files\n                            opts[signal.value] = [];\n                            for (var n = 0; n < target.files.length; n++) {\n                                opts[signal.value].push(target.files[n].name);\n                            }\n                        }\n                        else if (target.type === 'select-multiple') { // get all selected options\n                            opts[signal.value] = [];\n                            for (var n = 0; n < target.selectedOptions.length; n++) {\n                                opts[signal.value].push(target.selectedOptions[n].value);\n                            }\n                        }\n                        else if (target.type === 'checkbox' || target.type === 'radio') {\n                            opts[signal.value] = target.checked;\n                        }\n                        else {\n                            opts[signal.value] = target.value;\n                        }\n                    }\n                    window.DFSignals.call(signal.name, opts, undefined);\n                    if (prevent === true || (prevent === null && eventName !== \"change\")) {\n                        evt.preventDefault();\n                    }\n                };\n                target.addEventListener(eventName, callback);\n            });\n        });\n    }\n    document.addEventListener(\"DOMContentAdded\", function (evt) {\n        window.setTimeout(function () {\n            websocketForms(evt);\n        }, 50);\n        // awful trick for being sure that our addEventListener is the last.\n        // allows things like CKEditor to push its content to the textarea before sending the content of the form.\n    });\n    document.addEventListener(\"DOMContentLoaded\", function (evt) {\n        window.setTimeout(function () {\n            websocketForms(evt);\n        }, 50);\n        // awful trick for being sure that our addEventListener is the last.\n        // allows things like CKEditor to push its content to the textarea before sending the content of the form.\n    });\n})();\n",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// startup\n// Load entry module and return exports\n__webpack_require__(821);\n__webpack_require__(947);\n// This entry module is referenced by other modules so it can't be inlined\nvar __webpack_exports__ = __webpack_require__(125);\n"
     ],
     "version": 3
 }
```

### Comparing `df_websockets-1.0.3/df_websockets/tasks.py` & `df_websockets-1.0.8/df_websockets/tasks.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/templatetags/__init__.py` & `df_websockets-1.0.8/df_websockets/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/templatetags/websockets.py` & `df_websockets-1.0.8/df_websockets/templatetags/websockets.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/testing.py` & `df_websockets-1.0.8/df_websockets/testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/topics.py` & `df_websockets-1.0.8/df_websockets/topics.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/utils.py` & `df_websockets-1.0.8/df_websockets/utils.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/window_info.py` & `df_websockets-1.0.8/df_websockets/window_info.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/ws_middleware.py` & `df_websockets-1.0.8/df_websockets/ws_middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets/ws_settings.py` & `df_websockets-1.0.8/df_websockets/ws_settings.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/df_websockets.egg-info/PKG-INFO` & `df_websockets-1.0.8/df_websockets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: df-websockets
-Version: 1.0.3
+Version: 1.0.8
 Summary: Websocket integration for Django
 Home-page: https://github.com/d9pouces/df_websockets
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: github@19pouces.net
 License: CeCILL-B
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 df_websockets
 =============
 
 `df_websockets` extends [django-channels](https://channels.readthedocs.io) to simplify communications between 
@@ -99,15 +100,15 @@
 A bidirectionnal websocket connection will be established in your page.
 
 You can start the development server:
 ```bash
 python manage.py runserver
 ```
 
-_`daphne` must be present in `INSTALLED_APPS` with `channels>=4.0`_
+_`daphne` must be separately installed and added to `INSTALLED_APPS` with `channels>=4.0`_ 
 
 If you use Channels workers (WEBSOCKET_WORKERS = "channels"), you also need to start a Channel worker:
 ```bash
 python manage.py run_worker celery
 ```
 If you use Celery (WEBSOCKET_WORKERS = "celery"), you also need to start a Celery worker:
 ```bash
@@ -235,14 +236,45 @@
 - `WEBSOCKET_SIGNAL_DECODER`: the JSON decoder to decode signal arguments
 - `WEBSOCKET_TOPIC_SERIALIZER`: the function used to transform Python topics into valid topic names  
 - `WEBSOCKET_POOL_SIZES`: a dict associating a queue name to a number of threads (or processes)
 - `WINDOW_INFO_MIDDLEWARES`: a list of middlewares for transforming a HttpRequest to a WindowInfo 
 - `WEBSOCKET_URL`: URL prefix (`/ws/` by default)
 - `ASGI_APPLICATION`: the ASGI application 
 
+Cache backends
+--------------
+
+Task data are passed by the server process to the workers using the Django cache infrastructure. 
+For obvious reasons, you cannot use DummyCache nor LocMemCache with Celery or Channels workers, since these caching methods are not shared accross processes.
+So, you need either to use a shared cache backend as default backend, or dedicate a cache backend to websockets. 
+
+First case needs to update your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    }
+}
+```
+
+Second case, still in your `settings.py` file:
+```python
+CACHES = {
+    "default": {
+        "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
+        "LOCATION": "unique-snowflake",
+    },
+    "websockets": {
+        "BACKEND": "django.core.cache.backends.redis.RedisCache",
+        "LOCATION": "redis://127.0.0.1:6379",
+    },
+}
+WEBSOCKET_CACHE_BACKEND = "websockets"
+```
 
 HTML forms
 ----------
 
 `df_websockets` comes with some helper functions when you signals to be trigger on the server when a form is submitted or changed.
 Assuming that you have a `signals.py` file that contains:
 ```python
```

### Comparing `df_websockets-1.0.3/df_websockets.egg-info/SOURCES.txt` & `df_websockets-1.0.8/df_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/npm/df_websockets/app.js` & `df_websockets-1.0.8/npm/df_websockets/app.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -9,132 +9,135 @@
 //                                                                             /
 // You should have received a copy of the CeCILL-B license with                /
 // this file. If not, please visit:                                            /
 // https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /
 // or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /
 //                                                                             /
 ////////////////////////////////////////////////////////////////////////////////
+(() => {
 
-window.DFSignals = {
-    connection: null,
-    buffer: [],
-    registry: {},
-    wsurl: null
-};
-
-function getCookie(cname) {
-    const name = cname + "=";
-    const decodedCookie = decodeURIComponent(document.cookie);
-    const ca = decodedCookie.split(';');
-    for (let i = 0; i < ca.length; i++) {
-        let c = ca[i];
-        while (c.charAt(0) === ' ') {
-            c = c.substring(1);
-        }
-        if (c.indexOf(name) === 0) {
-            return c.substring(name.length, c.length);
-        }
-    }
-    return "";
-}
-
-function websocketConnect() {
-    const cookieName = "dfwsurl";
-    if (window.DFSignals.wsurl === null) {
-        const dfWsURL = getCookie(cookieName);
-        window.DFSignals.wsurl = decodeURIComponent(dfWsURL);
-    }
-    if (!window.DFSignals.wsurl) {
-        console.info("Unable to get the websocket URL in the '" + cookieName + "' cookie.");
-        return;
-    }
-    const connection = new WebSocket(window.DFSignals.wsurl);
-    /* cannot use header or cookies (cookies may change after the initial connection)
-     *  so we use GET parameter
-     *  */
-    connection.onopen = () => {
-        window.DFSignals.connection = connection;
-        for (let i = 0; i < window.DFSignals.buffer.length; i++) {
-            connection.send(window.DFSignals.buffer[i]);
-        }
-        window.DFSignals.buffer = [];
+    window.DFSignals = {
+        connection: null,
+        buffer: [],
+        registry: {},
+        wsurl: null
     };
-    connection.onmessage = (e) => {
-        console.debug('received call ' + e.data + ' from server.')
-        const msg = JSON.parse(e.data);
-        // noinspection JSUnresolvedVariable
-        if (msg.signal && msg.signal_id) {
-            window.DFSignals.call(msg.signal, msg.opts, msg.signal_id);
+
+    function getCookie(cname) {
+        const name = cname + "=";
+        const decodedCookie = decodeURIComponent(document.cookie);
+        const ca = decodedCookie.split(';');
+        for (let i = 0; i < ca.length; i++) {
+            let c = ca[i];
+            while (c.charAt(0) === ' ') {
+                c = c.substring(1);
+            }
+            if (c.indexOf(name) === 0) {
+                return c.substring(name.length, c.length);
+            }
+        }
+        return "";
+    }
+
+    function websocketConnect() {
+        const cookieName = "dfwsurl";
+        if (window.DFSignals.wsurl === null) {
+            const dfWsURL = getCookie(cookieName);
+            window.DFSignals.wsurl = decodeURIComponent(dfWsURL);
+        }
+        if (!window.DFSignals.wsurl) {
+            console.info("Unable to get the websocket URL in the '" + cookieName + "' cookie.");
+            return;
+        }
+        const connection = new WebSocket(window.DFSignals.wsurl);
+        /* cannot use header or cookies (cookies may change after the initial connection)
+         *  so we use GET parameter
+         *  */
+        connection.onopen = () => {
+            window.DFSignals.connection = connection;
+            for (let i = 0; i < window.DFSignals.buffer.length; i++) {
+                connection.send(window.DFSignals.buffer[i]);
+            }
+            window.DFSignals.buffer = [];
+        };
+        connection.onmessage = (e) => {
+            console.debug('received call ' + e.data + ' from server.')
+            const msg = JSON.parse(e.data);
+            // noinspection JSUnresolvedVariable
+            if (msg.signal && msg.signal_id) {
+                window.DFSignals.call(msg.signal, msg.opts, msg.signal_id);
+            }
+        };
+        connection.onerror = (e) => {
+            console.error("WS error: " + e);
+        };
+        connection.onclose = () => {
+            window.DFSignals.connection = null;
+            setTimeout(websocketConnect, 3000);
+        }
+    }
+
+    function call(signal, opts, id) {
+        /*"""
+        .. function:: call(signal, opts, id)
+
+            Call a signal.
+            If the signal is also defined in the Python server and available to the user, then the Python signal is also triggered.
+
+            :param string signal: Name of the called signal.
+            :param object opts: Object with signal arguments.
+            :param string id: Unique id of each signal triggered by the server. Do not use it yourself.
+            :returns: always `false`.
+        */
+        // if (window.DFSignals.registry[signal] === undefined) {
+        //     console.debug('unknown call "' + signal + '" (from both client and server).');
+        //     return false;
+        // } else
+        if ((id !== undefined) && (window.DFSignals.registry[id] !== undefined)) {
+            return false;
+        } else if (id !== undefined) {
+            window.DFSignals.registry[id] = true;
+        }
+        if (window.DFSignals.registry[signal] !== undefined) {
+            console.debug('call "' + signal + '"', opts);
+            for (let i = 0; i < window.DFSignals.registry[signal].length; i += 1) {
+                window.DFSignals.registry[signal][i](opts, id);
+            }
+        }
+        if (id === undefined) {
+            console.debug('call from client: "' + signal + '"', opts);
+            const msg = JSON.stringify({
+                signal: signal,
+                opts: opts
+            });
+            if (window.DFSignals.connection) {
+                window.DFSignals.connection.send(msg);
+            } else {
+                window.DFSignals.buffer.push(msg);
+            }
         }
-    };
-    connection.onerror = (e) => {
-        console.error("WS error: " + e);
-    };
-    connection.onclose = () => {
-        window.DFSignals.connection = null;
-        setTimeout(websocketConnect, 3000);
-    }
-}
 
-function call(signal, opts, id) {
-    /*"""
-    .. function:: call(signal, opts, id)
-
-        Call a signal.
-        If the signal is also defined in the Python server and available to the user, then the Python signal is also triggered.
-
-        :param string signal: Name of the called signal.
-        :param object opts: Object with signal arguments.
-        :param string id: Unique id of each signal triggered by the server. Do not use it yourself.
-        :returns: always `false`.
-    */
-    // if (window.DFSignals.registry[signal] === undefined) {
-    //     console.debug('unknown call "' + signal + '" (from both client and server).');
-    //     return false;
-    // } else
-    if ((id !== undefined) && (window.DFSignals.registry[id] !== undefined)) {
         return false;
-    } else if (id !== undefined) {
-        window.DFSignals.registry[id] = true;
-    }
-    if (window.DFSignals.registry[signal] !== undefined) {
-        console.debug('call "' + signal + '"', opts);
-        for (let i = 0; i < window.DFSignals.registry[signal].length; i += 1) {
-            window.DFSignals.registry[signal][i](opts, id);
-        }
-    }
-    if (id === undefined) {
-        console.debug('call from client: "' + signal + '"', opts);
-        const msg = JSON.stringify({
-            signal: signal,
-            opts: opts
-        });
-        if (window.DFSignals.connection) {
-            window.DFSignals.connection.send(msg);
-        } else {
-            window.DFSignals.buffer.push(msg);
-        }
     }
 
-    return false;
-}
+    function connect(signal, fn) {
+        /*"""
+        .. function:: connect(signal, fn)
+
+            Connect a javascript code to the given signal name.
 
-function connect(signal, fn) {
-    /*"""
-    .. function:: connect(signal, fn)
-
-        Connect a javascript code to the given signal name.
-
-        :param string signal: Name of the signal.
-        :param function fn: Function that takes a single object as argument. The properties of this object are the signal arguments.
-        :returns: nothing.
-    */
-    if (window.DFSignals.registry[signal] === undefined) {
-        window.DFSignals.registry[signal] = [];
+            :param string signal: Name of the signal.
+            :param function fn: Function that takes a single object as argument. The properties of this object are the signal arguments.
+            :returns: nothing.
+        */
+        if (window.DFSignals.registry[signal] === undefined) {
+            window.DFSignals.registry[signal] = [];
+        }
+        window.DFSignals.registry[signal].push(fn);
     }
-    window.DFSignals.registry[signal].push(fn);
-}
 
-document.addEventListener("DOMContentLoaded", websocketConnect);
+    document.addEventListener("DOMContentLoaded", websocketConnect);
+
+    window.DFSignals.call = call;
+    window.DFSignals.connect = connect;
 
-window.DFSignals.call = call;
-window.DFSignals.connect = connect;
+})();
```

### Comparing `df_websockets-1.0.3/npm/df_websockets/base.js` & `df_websockets-1.0.8/npm/df_websockets/base.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -11,414 +11,417 @@
 // this file. If not, please visit:                                            /
 // https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           /
 // or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         /
 //                                                                             /
 ////////////////////////////////////////////////////////////////////////////////
 
 import {
-    htmlFormsSet,
-    htmlFormsSetAll
+    htmlFormsSet
 } from "./forms";
 import {
     htmlAfter,
     htmlAppend,
     htmlBefore,
     htmlContent,
     htmlEmpty,
     htmlPrepend,
     htmlRemove,
     htmlReplaceWith,
     htmlText
 } from "./html";
 
-const htmlAddClass = opts => {
-    document.querySelectorAll(opts.selector).forEach(elt => {
-        // noinspection JSUnresolvedVariable
-        elt.classList.add(opts.class_name)
-    });
-};
-const htmlRemoveClass = (opts) => {
-    document.querySelectorAll(opts.selector).forEach(elt => {
-        // noinspection JSUnresolvedVariable
-        elt.classList.remove(opts.class_name);
-    });
-};
-const htmlRemoveAttr = (opts) => {
-    document.querySelectorAll(opts.selector).forEach(elt => {
-        // noinspection JSUnresolvedVariable
-        elt.removeAttribute(opts.attr_name);
-    });
-};
-const htmlAddAttribute = (opts) => {
-    document.querySelectorAll(opts.selector).forEach(elt => {
-        // noinspection JSUnresolvedVariable
-        elt.setAttribute(opts.attr_name, opts.attr_value);
-    });
-};
-const htmlBooleanAttribute = (opts) => {
-    document.querySelectorAll(opts.selector).forEach(elt => {
-        if (opts.value) {
-            elt.setAttribute(opts.name, opts.name);
-        } else {
-            elt.removeAttribute(opts.name)
-        }
-    });
-};
-const htmlDownloadFile = (opts) => {
-    const save = document.createElement('a');
-    save.href = opts.url;
-    save.target = '_blank';
-    save.download = opts.filename || 'unknown';
-    const evt = new MouseEvent('click', {
-        view: window,
-        bubbles: true,
-        cancelable: false
-    });
-    save.dispatchEvent(evt);
-    (window.URL || window.webkitURL).revokeObjectURL(save.href);
-};
-const htmlFocus = (opts) => {
-    const elt = document.querySelector(opts.selector);
-    if (elt) {
-        elt.focus({
-            preventScroll: false
-        });
-    }
-};
+(
+    () => {
+        const htmlAddClass = opts => {
+            document.querySelectorAll(opts.selector).forEach(elt => {
+                // noinspection JSUnresolvedVariable
+                elt.classList.add(opts.class_name)
+            });
+        };
+        const htmlRemoveClass = (opts) => {
+            document.querySelectorAll(opts.selector).forEach(elt => {
+                // noinspection JSUnresolvedVariable
+                elt.classList.remove(opts.class_name);
+            });
+        };
+        const htmlRemoveAttr = (opts) => {
+            document.querySelectorAll(opts.selector).forEach(elt => {
+                // noinspection JSUnresolvedVariable
+                elt.removeAttribute(opts.attr_name);
+            });
+        };
+        const htmlAddAttribute = (opts) => {
+            document.querySelectorAll(opts.selector).forEach(elt => {
+                // noinspection JSUnresolvedVariable
+                elt.setAttribute(opts.attr_name, opts.attr_value);
+            });
+        };
+        const htmlBooleanAttribute = (opts) => {
+            document.querySelectorAll(opts.selector).forEach(elt => {
+                if (opts.value) {
+                    elt.setAttribute(opts.name, opts.name);
+                } else {
+                    elt.removeAttribute(opts.name)
+                }
+            });
+        };
+        const htmlDownloadFile = (opts) => {
+            const save = document.createElement('a');
+            save.href = opts.url;
+            save.target = '_blank';
+            save.download = opts.filename || 'unknown';
+            const evt = new MouseEvent('click', {
+                view: window,
+                bubbles: true,
+                cancelable: false
+            });
+            save.dispatchEvent(evt);
+            (window.URL || window.webkitURL).revokeObjectURL(save.href);
+        };
+        const htmlFocus = (opts) => {
+            const elt = document.querySelector(opts.selector);
+            if (elt) {
+                elt.focus({
+                    preventScroll: false
+                });
+            }
+        };
 
-function connectSignals() {
+        function connectSignals() {
 
-    window.DFSignals.connect('html.after', htmlAfter);
-    /*"""
-    .. function:: html.after(opts)
+            window.DFSignals.connect('html.after', htmlAfter);
+            /*"""
+            .. function:: html.after(opts)
 
-        Insert content, specified by the parameter, after each element in the set of matched elements.
-        Equivalent to `$().after()` or `.insertAdjacentHTML('afterend', ...)`.
-        Trigger a `DOMContentAdded` event on the added content.
+                Insert content, specified by the parameter, after each element in the set of matched elements.
+                Equivalent to `$().after()` or `.insertAdjacentHTML('afterend', ...)`.
+                Trigger a `DOMContentAdded` event on the added content.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.after', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.after', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.after', to=WINDOW, selector="#obj", content="<span>hello</span>")
+                    trigger(window_info, 'html.after', to=WINDOW, selector="#obj", content="<span>hello</span>")
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
+            */
 
-    window.DFSignals.connect('html.append', htmlAppend);
-    /*"""
-    .. function:: html.append(opts)
+            window.DFSignals.connect('html.append', htmlAppend);
+            /*"""
+            .. function:: html.append(opts)
 
-        Insert content, specified by the parameter, to the end of each element in the set of matched elements.
-        Equivalent to `$().append()` or `.insertAdjacentHTML('beforeend', ...)`.
-        Trigger a `DOMContentAdded` event on the added content.
+                Insert content, specified by the parameter, to the end of each element in the set of matched elements.
+                Equivalent to `$().append()` or `.insertAdjacentHTML('beforeend', ...)`.
+                Trigger a `DOMContentAdded` event on the added content.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.append', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.append', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.append', to=WINDOW, selector="#obj", content="<span>hello</span>")
+                    trigger(window_info, 'html.append', to=WINDOW, selector="#obj", content="<span>hello</span>")
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
+            */
 
-    window.DFSignals.connect('html.prepend', htmlPrepend);
+            window.DFSignals.connect('html.prepend', htmlPrepend);
 
-    /*"""
-    .. function:: html.prepend(opts)
+            /*"""
+            .. function:: html.prepend(opts)
 
-        Insert content, specified by the parameter, to the beginning of each element in the set of matched elements.
-        Equivalent to `$().prepend()` or `.insertAdjacentHTML('afterbegin', ...)`.
-        Trigger a `DOMContentAdded` event on the added content.
+                Insert content, specified by the parameter, to the beginning of each element in the set of matched elements.
+                Equivalent to `$().prepend()` or `.insertAdjacentHTML('afterbegin', ...)`.
+                Trigger a `DOMContentAdded` event on the added content.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.prepend', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.prepend', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.prepend', to=WINDOW, selector="#obj", content="<span>hello</span>")
+                    trigger(window_info, 'html.prepend', to=WINDOW, selector="#obj", content="<span>hello</span>")
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
+            */
 
-    window.DFSignals.connect('html.before', htmlBefore);
-    /*"""
-    .. function:: html.before(opts)
+            window.DFSignals.connect('html.before', htmlBefore);
+            /*"""
+            .. function:: html.before(opts)
 
-        Insert content, specified by the parameter, before each element in the set of matched elements..
-        Equivalent to `$().before()` or `.insertAdjacentHTML('beforebegin', ...)`.
-        Trigger a `DOMContentAdded` event on the added content.
+                Insert content, specified by the parameter, before each element in the set of matched elements..
+                Equivalent to `$().before()` or `.insertAdjacentHTML('beforebegin', ...)`.
+                Trigger a `DOMContentAdded` event on the added content.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.before', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.before', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.before', to=WINDOW, selector="#obj", content="<span>hello</span>")
+                    trigger(window_info, 'html.before', to=WINDOW, selector="#obj", content="<span>hello</span>")
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
-    window.DFSignals.connect('html.content', htmlContent);
-    /*"""
-    .. function:: html.content(opts)
+            */
+            window.DFSignals.connect('html.content', htmlContent);
+            /*"""
+            .. function:: html.content(opts)
 
-        set the HTML contents of every matched element.
+                set the HTML contents of every matched element.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.content', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.content', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.content', to=WINDOW, selector="#obj", content= "<span>hello</span>")
+                    trigger(window_info, 'html.content', to=WINDOW, selector="#obj", content= "<span>hello</span>")
 
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
-    */
+                :param string selector: HTML selector
+                :param string content: new HTML content
+            */
 
-    window.DFSignals.connect('html.replace_with', htmlReplaceWith);
-    /*"""
-    .. function:: html.replace_with(opts)
+            window.DFSignals.connect('html.replace_with', htmlReplaceWith);
+            /*"""
+            .. function:: html.replace_with(opts)
 
-        Replace each element in the set of matched elements with the provided new content.
+                Replace each element in the set of matched elements with the provided new content.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.replace_with', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.replace_with', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.replace_with', to=WINDOW, selector="#obj", content="<span>hello</span>")
+                    trigger(window_info, 'html.replace_with', to=WINDOW, selector="#obj", content="<span>hello</span>")
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
+            */
 
-    window.DFSignals.connect('html.empty', htmlEmpty);
-    /*"""
-    .. function:: html.empty(opts)
+            window.DFSignals.connect('html.empty', htmlEmpty);
+            /*"""
+            .. function:: html.empty(opts)
 
-        Remove all child nodes of the set of matched elements from the DOM.
+                Remove all child nodes of the set of matched elements from the DOM.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.empty', {selector: "#obj"});
+                    window.DFSignals.call('html.empty', {selector: "#obj"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.empty', to=WINDOW, selector="#obj")
+                    trigger(window_info, 'html.empty', to=WINDOW, selector="#obj")
 
-        :param string selector: HTML selector
+                :param string selector: HTML selector
 
-    */
+            */
 
-    window.DFSignals.connect('html.remove', htmlRemove);
-    /*"""
-    .. function:: html.remove(opts)
+            window.DFSignals.connect('html.remove', htmlRemove);
+            /*"""
+            .. function:: html.remove(opts)
 
-        Remove the set of matched elements from the DOM.
+                Remove the set of matched elements from the DOM.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.remove', {selector: "#obj"});
+                    window.DFSignals.call('html.remove', {selector: "#obj"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.remove', to=WINDOW, selector="#obj")
+                    trigger(window_info, 'html.remove', to=WINDOW, selector="#obj")
 
-        :param string selector: HTML selector
+                :param string selector: HTML selector
 
-    */
+            */
 
-    window.DFSignals.connect('html.add_class', htmlAddClass);
-    /*"""
-    .. function:: html.add_class(opts)
+            window.DFSignals.connect('html.add_class', htmlAddClass);
+            /*"""
+            .. function:: html.add_class(opts)
 
-        Adds the specified class(es) to each of the set of matched elements.
+                Adds the specified class(es) to each of the set of matched elements.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.add_class', {selector: "#obj", class_name: "myclass"});
+                    window.DFSignals.call('html.add_class', {selector: "#obj", class_name: "myclass"});
 
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.add_class', to=WINDOW, selector="#obj", class_name="myclass")
+                    trigger(window_info, 'html.add_class', to=WINDOW, selector="#obj", class_name="myclass")
 
 
-        :param string selector: HTML selector
-        :param string class_name: new class
+                :param string selector: HTML selector
+                :param string class_name: new class
 
-    */
-    window.DFSignals.connect('html.remove_class', htmlRemoveClass);
-    /*"""
-    .. function:: html.remove_class(opts)
+            */
+            window.DFSignals.connect('html.remove_class', htmlRemoveClass);
+            /*"""
+            .. function:: html.remove_class(opts)
 
-        Remove a single class, multiple classes, or all classes from each element in the set of matched elements.
+                Remove a single class, multiple classes, or all classes from each element in the set of matched elements.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.remove_class', {selector: "#obj", class_name: "class"});
+                    window.DFSignals.call('html.remove_class', {selector: "#obj", class_name: "class"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.remove_class', to=WINDOW, selector="#obj", class_name="attr")
+                    trigger(window_info, 'html.remove_class', to=WINDOW, selector="#obj", class_name="attr")
 
-        :param string selector: HTML selector
-        :param string class_name: class to remove
+                :param string selector: HTML selector
+                :param string class_name: class to remove
 
-    */
-    window.DFSignals.connect('html.remove_attr', htmlRemoveAttr);
-    /*"""
-    .. function:: html.remove_attr(opts)
+            */
+            window.DFSignals.connect('html.remove_attr', htmlRemoveAttr);
+            /*"""
+            .. function:: html.remove_attr(opts)
 
-        Remove an attribute from each element in the set of matched elements.
+                Remove an attribute from each element in the set of matched elements.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.remove_attr', {selector: "#obj", attr_name: "attr"});
+                    window.DFSignals.call('html.remove_attr', {selector: "#obj", attr_name: "attr"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.remove_attr', to=WINDOW, selector="#obj", attr_name="attr")
+                    trigger(window_info, 'html.remove_attr', to=WINDOW, selector="#obj", attr_name="attr")
 
-        :param string selector: HTML selector
-        :param string attr_name: attribute to remove
+                :param string selector: HTML selector
+                :param string attr_name: attribute to remove
 
-    */
+            */
 
-    window.DFSignals.connect('html.add_attribute', htmlAddAttribute);
-    /*"""
-    .. function:: html.add_attribute(opts)
+            window.DFSignals.connect('html.add_attribute', htmlAddAttribute);
+            /*"""
+            .. function:: html.add_attribute(opts)
 
-        Add an attribute to each element matched by the given selector.
+                Add an attribute to each element matched by the given selector.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.add_attribute', {selector: "#obj", attr_name: "data-df", attr_value: "value"});
+                    window.DFSignals.call('html.add_attribute', {selector: "#obj", attr_name: "data-df", attr_value: "value"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.add_attribute', to=WINDOW, selector="#obj", attr_name="data-df", attr_value= "value")
+                    trigger(window_info, 'html.add_attribute', to=WINDOW, selector="#obj", attr_name="data-df", attr_value= "value")
 
 
-        :param string selector: HTML selector
-        :param string attr_name: name of the attribute to add
-        :param string attr_value: value of the attribute to add
+                :param string selector: HTML selector
+                :param string attr_name: name of the attribute to add
+                :param string attr_value: value of the attribute to add
 
-    */
-    window.DFSignals.connect('html.boolean_attribute', htmlBooleanAttribute);
-    /*"""
-    .. function:: html.boolean_attribute(opts)
+            */
+            window.DFSignals.connect('html.boolean_attribute', htmlBooleanAttribute);
+            /*"""
+            .. function:: html.boolean_attribute(opts)
 
-        Set or remove a boolean attribute. Always set the value of the added attribute to its name.
+                Set or remove a boolean attribute. Always set the value of the added attribute to its name.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.boolean_attribute', {selector: "#input", name: "checked", value: true});
+                    window.DFSignals.call('html.boolean_attribute', {selector: "#input", name: "checked", value: true});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.boolean_attribute', to=WINDOW, selector="#input", name="checked", value=True)
+                    trigger(window_info, 'html.boolean_attribute', to=WINDOW, selector="#input", name="checked", value=True)
 
 
-        :param string selector: HTML selector
-        :param string name: name of the attribute to add
-        :param string value: if True, add the attribute, if False, remove the attribute
+                :param string selector: HTML selector
+                :param string name: name of the attribute to add
+                :param string value: if True, add the attribute, if False, remove the attribute
 
-    */
+            */
 
 
-    window.DFSignals.connect('html.text', htmlText);
-    /*"""
-    .. function:: html.text(opts)
+            window.DFSignals.connect('html.text', htmlText);
+            /*"""
+            .. function:: html.text(opts)
 
-        Set the text contents of the matched elements.
+                Set the text contents of the matched elements.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.text', {selector: "#obj", content: "<span>hello</span>"});
+                    window.DFSignals.call('html.text', {selector: "#obj", content: "<span>hello</span>"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.text', to=WINDOW, selector="#obj", content= "<span>hello</span>")
+                    trigger(window_info, 'html.text', to=WINDOW, selector="#obj", content= "<span>hello</span>")
 
 
-        :param string selector: HTML selector
-        :param string content: new HTML content
+                :param string selector: HTML selector
+                :param string content: new HTML content
 
-    */
+            */
 
-    window.DFSignals.connect('html.download_file', htmlDownloadFile);
-    /*"""
-    .. function:: html.download_file(opts)
+            window.DFSignals.connect('html.download_file', htmlDownloadFile);
+            /*"""
+            .. function:: html.download_file(opts)
 
-        Force the client to download the given file.
+                Force the client to download the given file.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.download_file', {url: "http://example.org/test.zip", filename: "test.zip"});
+                    window.DFSignals.call('html.download_file', {url: "http://example.org/test.zip", filename: "test.zip"});
 
-    .. code-block:: python
+            .. code-block:: python
 
-        trigger(window_info, 'html.download_file', to=WINDOW, url="http://example.org/test.zip", filename="test.zip")
+                trigger(window_info, 'html.download_file', to=WINDOW, url="http://example.org/test.zip", filename="test.zip")
 
-        :param string url: URL of the file
-        :param string filename: name of the file
+                :param string url: URL of the file
+                :param string filename: name of the file
 
-    */
+            */
 
 
-    window.DFSignals.connect('html.focus', htmlFocus);
-    /*"""
-    .. function:: html.focus(opts)
+            window.DFSignals.connect('html.focus', htmlFocus);
+            /*"""
+            .. function:: html.focus(opts)
 
-        Set the focus to the matched element.
+                Set the focus to the matched element.
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.focus', {selector: "#obj"});
+                    window.DFSignals.call('html.focus', {selector: "#obj"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.focus', to=WINDOW, selector="#obj")
+                    trigger(window_info, 'html.focus', to=WINDOW, selector="#obj")
 
-        :param string selector: HTML selector
+                :param string selector: HTML selector
 
-    */
+            */
 
-    window.DFSignals.connect('html.forms.set', htmlFormsSet);
-    /*"""
-    .. function:: html.forms.set(opts)
+            window.DFSignals.connect('html.forms.set', htmlFormsSet);
+            /*"""
+            .. function:: html.forms.set(opts)
 
-        Set the value of a form input
+                Set the value of a form input
 
-        .. code-block:: javascript
+                .. code-block:: javascript
 
-            window.DFSignals.call('html.forms.set', {selector: "[name=title]", value: "new title"});
+                    window.DFSignals.call('html.forms.set', {selector: "[name=title]", value: "new title"});
 
-        .. code-block:: python
+                .. code-block:: python
 
-            trigger(window_info, 'html.forms.set', to=WINDOW, selector="[name=title]", value="new_title")
+                    trigger(window_info, 'html.forms.set', to=WINDOW, selector="[name=title]", value="new_title")
 
-        :param string selector: HTML selector
+                :param string selector: HTML selector
 
-    */
-}
+            */
+        }
 
-document.addEventListener("DOMContentLoaded", connectSignals);
+        document.addEventListener("DOMContentLoaded", connectSignals);
+    }
+)();
```

### Comparing `df_websockets-1.0.3/npm/df_websockets/forms.ts` & `df_websockets-1.0.8/npm/df_websockets/forms.ts`

 * *Files 5% similar despite different names*

```diff
@@ -43,73 +43,74 @@
         } else if ((field.type !== 'checkbox' && field.type !== 'radio') || (<HTMLInputElement>field).checked) {
             serialized.push({name: field.name, value: field.value});
         }
     }
     return serialized;
 }
 
-function setFormFieldValue(form: HTMLFormElement, name: string, value: string | boolean | Array<string>) {
-    const item = form.elements.namedItem(name);
-    if (item === null) {
-        return;
-    } else if (item instanceof RadioNodeList) {
-        if ((value === true) || (value === false)) {
-            item.forEach((input: HTMLInputElement) => {
-                input.checked = value
-            });
-        } else if (Array.isArray(value)) {
-            const valuesSet = new Set(value);
-            item.forEach((input: HTMLInputElement) => {
-                input.checked = valuesSet.has(input.value);
-            });
-        } else {
-            item.forEach((input: HTMLInputElement) => {
-                input.checked = input.value === value;
-            });
-        }
-    } else if (item instanceof HTMLTextAreaElement) {
-        item.value = <string>value;
-    } else if ((item instanceof HTMLInputElement) && (item.type === "checkbox")) {
-        if (value === true) {
-            item.checked = true;
-        } else if (value === false) {
-            item.checked = false;
-        } else {
-            item.value = <string>value;
-        }
-    } else if (item instanceof HTMLSelectElement) {
-        const options = item.options;
-        if (Array.isArray(value)) {
-            const valuesSet = new Set(value);
-            for (let i = 0; i < options.length; i++) {
-                options[i].selected = valuesSet.has(options[i].value);
-            }
-        } else {
-            for (let i = 0; i < options.length; i++) {
-                options[i].selected = options[i].value === value;
-            }
-        }
-    } else if (item instanceof HTMLInputElement) {
-        item.value = <string>value;
-    }
-
-}
-
 
 interface formSingleValue {
     name: string;
     value: string | Array<string> | boolean;
 }
 
 interface formValueList {
     selector: string;
     values: Array<formSingleValue>;
 }
 
 export function htmlFormsSet(opts: formValueList) {
+    function setFormFieldValue(form: HTMLFormElement, name: string, value: string | boolean | Array<string>) {
+        const item = form.elements.namedItem(name);
+        if (item === null) {
+            return;
+        } else if (item instanceof RadioNodeList) {
+            if ((value === true) || (value === false)) {
+                item.forEach((input: HTMLInputElement) => {
+                    input.checked = value
+                });
+            } else if (Array.isArray(value)) {
+                const valuesSet = new Set(value);
+                item.forEach((input: HTMLInputElement) => {
+                    input.checked = valuesSet.has(input.value);
+                });
+            } else {
+                item.forEach((input: HTMLInputElement) => {
+                    input.checked = input.value === value;
+                });
+            }
+        } else if (item instanceof HTMLTextAreaElement) {
+            item.value = <string>value;
+        } else if ((item instanceof HTMLInputElement) && (item.type === "checkbox")) {
+            if (value === true) {
+                item.checked = true;
+            } else if (value === false) {
+                item.checked = false;
+            } else {
+                item.value = <string>value;
+            }
+        } else if (item instanceof HTMLSelectElement) {
+            const options = item.options;
+            if (Array.isArray(value)) {
+                const valuesSet = new Set(value);
+                for (let i = 0; i < options.length; i++) {
+                    options[i].selected = valuesSet.has(options[i].value);
+                }
+            } else {
+                for (let i = 0; i < options.length; i++) {
+                    options[i].selected = options[i].value === value;
+                }
+            }
+        } else if (item instanceof HTMLInputElement) {
+            item.value = <string>value;
+        }
+
+    }
+
+
     document.querySelectorAll(opts.selector).forEach(
         (form: HTMLFormElement) => {
             opts.values.forEach(
                 (values) => {
                     setFormFieldValue(form, values.name, values.value);
                 }
             )
@@ -124,132 +125,138 @@
     on: string,
     form: string,
     opts: Record<string, any>,
     value: string,
     prevent: boolean
 }
 
-function DOMContentAdded(evt: Event) {
-    /*
-    search all HTML elements with an attribute "data-df-signal" that contains a JSON list of Signal objects:
-    {
-        name: "name of the signal to call",  (required)
-        on: "name of the listened event",
-        opts: "extra options",               (optional)
-        form: "name of option to add to opts that contains the serialized form",  (optional)
-        value: "name of option to add to opts that contains the value",  (optional)
-        prevent: preventDefault               (optional, defaults to true for on=="submit" or "click" else false )
-    }
-
-    When the listened event is not given, the listened event is
-        * "submit" for forms,
-        * "click" for "reset"/"submit"/"button" input fields,
-        * "change" for other fields.
-
-    Using on a HTML form:
-    ```html
-    <form data-df-signal='[{"name": "signal.name", "on": "change", "form": "form_data", "opts": {"id": 42} }]'>
-        <input type="text" name="title" value="df_websockets">
-    </form>```
-    or, using the Django templating system:
-    ```html
-    {% load df_websockets %}
-    <form {% js_call "signal.name" on="change" form="form_data" id=42 %}>
-        <input type="text" name="title" value="df_websockets">
-    </form>```
-
-    When the field "title" is modified, a signal "signal.name" is triggered on the server (via the websocket) with
-    the following arguments:
-    ```python
-    form_data = [{"name": "title", "value": "df_websockets"}]
-    id = 42
-    ```
-
-    Using on a HTML form input field:
-    ```html
-    <form>
-        <input type="text" name="title" data-df-signal='[{"name": "signal.name", "on": "change", "value": "title", "opts": {"id": 42} }]'>
-    </form>```
-    or, using the Django templating system:
-    ```html
-    {% load df_websockets %}
-    <form>
-        <input type="text" name="title" {% js_call "signal.name" on="change" value="title" id=42 %}>
-    </form>```
-
-    When the field "title" is modified, a signal "signal.name" is triggered on the server (via the websocket) with
-    the following arguments:
-    ```python
-    title = "new title value"
-    id = 42
-    ```
-     */
-    (<HTMLElement>evt.target).querySelectorAll("[data-df-signal]").forEach(
-        (target: HTMLInputElement | HTMLSelectElement | HTMLFormElement) => {
-            const signals = <Array<Signal>>JSON.parse(target.getAttribute("data-df-signal"));
-            signals.forEach((signal: Signal) => {
-                let eventName = signal.on;
-                if (!eventName) {
-                    if (target.tagName === "FORM") {
-                        eventName = "submit";
-                    } else if ((target.tagName === "INPUT" && !(target.type === 'reset' || target.type === 'submit' || target.type === 'button')) || (target.tagName === "TEXTAREA")) {
-                        eventName = "change";
-                    } else {
-                        eventName = "click";
-                    }
-                }
-                const callback = (evt: Event) => {
-                    // noinspection JSUnresolvedVariable
-                    const prevent = signal.prevent;
-                    const opts = signal.opts || {};
-                    if (signal.form) {
-                        opts[signal.form] = serializeForm(<HTMLFormElement>target);
+(() => {
+    function websocketForms(evt: Event) {
+        /*
+        search all HTML elements with an attribute "data-df-signal" that contains a JSON list of Signal objects:
+        {
+            name: "name of the signal to call",  (required)
+            on: "name of the listened event",
+            opts: "extra options",               (optional)
+            form: "name of option to add to opts that contains the serialized form",  (optional)
+            value: "name of option to add to opts that contains the value",  (optional)
+            prevent: preventDefault               (optional, defaults to true for on=="submit" or "click" else false )
+        }
+
+        When the listened event is not given, the listened event is
+            * "submit" for forms,
+            * "click" for "reset"/"submit"/"button" input fields,
+            * "change" for other fields.
+
+        Using on a HTML form:
+        ```html
+        <form data-df-signal='[{"name": "signal.name", "on": "change", "form": "form_data", "opts": {"id": 42} }]'>
+            <input type="text" name="title" value="df_websockets">
+        </form>```
+        or, using the Django templating system:
+        ```html
+        {% load df_websockets %}
+        <form {% js_call "signal.name" on="change" form="form_data" id=42 %}>
+            <input type="text" name="title" value="df_websockets">
+        </form>```
+
+        When the field "title" is modified, a signal "signal.name" is triggered on the server (via the websocket) with
+        the following arguments:
+        ```python
+        form_data = [{"name": "title", "value": "df_websockets"}]
+        id = 42
+        ```
+
+        Using on a HTML form input field:
+        ```html
+        <form>
+            <input type="text" name="title" data-df-signal='[{"name": "signal.name", "on": "change", "value": "title", "opts": {"id": 42} }]'>
+        </form>```
+        or, using the Django templating system:
+        ```html
+        {% load df_websockets %}
+        <form>
+            <input type="text" name="title" {% js_call "signal.name" on="change" value="title" id=42 %}>
+        </form>```
+
+        When the field "title" is modified, a signal "signal.name" is triggered on the server (via the websocket) with
+        the following arguments:
+        ```python
+        title = "new title value"
+        id = 42
+        ```
+         */
+        if (!(<HTMLElement>evt.target).querySelectorAll) {
+            return;
+        }
+        (<HTMLElement>evt.target).querySelectorAll("[data-df-signal]").forEach(
+            (target: HTMLInputElement | HTMLSelectElement | HTMLFormElement) => {
+                const signals = <Array<Signal>>JSON.parse(target.getAttribute("data-df-signal"));
+                signals.forEach((signal: Signal) => {
+                    let eventName = signal.on;
+                    if (!eventName) {
+                        if (target.tagName === "FORM") {
+                            eventName = "submit";
+                        } else if ((target.tagName === "INPUT" && !(target.type === 'reset' || target.type === 'submit' || target.type === 'button')) || (target.tagName === "TEXTAREA")) {
+                            eventName = "change";
+                        } else {
+                            eventName = "click";
+                        }
                     }
-                    if (signal.value) {
+                    const callback = (evt: Event) => {
+                        // noinspection JSUnresolvedVariable
+                        const prevent = signal.prevent;
+                        const opts = signal.opts || {};
+                        if (signal.form) {
+                            opts[signal.form] = serializeForm(<HTMLFormElement>target);
+                        }
+                        if (signal.value) {
 
-                        if (target.type === "file") {  // just returns the name of selected files
-                            opts[signal.value] = [];
-                            for (let n = 0; n < (<HTMLInputElement>target).files.length; n++) {
-                                opts[signal.value].push((<HTMLInputElement>target).files[n].name);
-                            }
-                        } else if (target.type === 'select-multiple') { // get all selected options
-                            opts[signal.value] = [];
-                            for (let n = 0; n < (<HTMLSelectElement>target).selectedOptions.length; n++) {
-                                opts[signal.value].push((<HTMLSelectElement>target).selectedOptions[n].value);
-                            }
-                        } else if (target.type === 'checkbox' || target.type === 'radio') {
-                            opts[signal.value] = (<HTMLInputElement>target).checked;
+                            if (target.type === "file") {  // just returns the name of selected files
+                                opts[signal.value] = [];
+                                for (let n = 0; n < (<HTMLInputElement>target).files.length; n++) {
+                                    opts[signal.value].push((<HTMLInputElement>target).files[n].name);
+                                }
+                            } else if (target.type === 'select-multiple') { // get all selected options
+                                opts[signal.value] = [];
+                                for (let n = 0; n < (<HTMLSelectElement>target).selectedOptions.length; n++) {
+                                    opts[signal.value].push((<HTMLSelectElement>target).selectedOptions[n].value);
+                                }
+                            } else if (target.type === 'checkbox' || target.type === 'radio') {
+                                opts[signal.value] = (<HTMLInputElement>target).checked;
 
-                        } else {
-                            opts[signal.value] = target.value;
+                            } else {
+                                opts[signal.value] = target.value;
+                            }
                         }
-                    }
-                    (<Window>window).DFSignals.call(
-                        signal.name,
-                        opts
-                    );
+                        (<Window>window).DFSignals.call(
+                            signal.name,
+                            opts,
+                            undefined
+                        );
 
-                    if (prevent === true || (prevent === null && eventName !== "change")) {
-                        evt.preventDefault();
+                        if (prevent === true || (prevent === null && eventName !== "change")) {
+                            evt.preventDefault();
+                        }
                     }
-                }
-                target.addEventListener(eventName, callback);
-            });
-        }
-    );
-}
+                    target.addEventListener(eventName, callback);
+                });
+            }
+        );
+    }
 
 
-document.addEventListener("DOMContentAdded", (evt) => {
-    window.setTimeout(() => {
-        DOMContentAdded(evt);
-    }, 200);
-    // awful trick for being sure that our addEventListener is the last.
-    // allows things like CKEditor to push its content to the textarea before sending the content of the form.
-});
-document.addEventListener("DOMContentLoaded", (evt) => {
-    window.setTimeout(() => {
-        DOMContentAdded(evt);
-    }, 200);
-    // awful trick for being sure that our addEventListener is the last.
-    // allows things like CKEditor to push its content to the textarea before sending the content of the form.
-});
+    document.addEventListener("DOMContentAdded", (evt) => {
+        window.setTimeout(() => {
+            websocketForms(evt);
+        }, 50);
+        // awful trick for being sure that our addEventListener is the last.
+        // allows things like CKEditor to push its content to the textarea before sending the content of the form.
+    });
+    document.addEventListener("DOMContentLoaded", (evt) => {
+        window.setTimeout(() => {
+            websocketForms(evt);
+        }, 50);
+        // awful trick for being sure that our addEventListener is the last.
+        // allows things like CKEditor to push its content to the textarea before sending the content of the form.
+    });
+})();
```

### Comparing `df_websockets-1.0.3/npm/df_websockets/html.js` & `df_websockets-1.0.8/npm/df_websockets/html.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -16,68 +16,78 @@
 
 export const htmlAfter = opts => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         const originalNextSibling = elt.nextSibling;
         elt.insertAdjacentHTML('afterend', opts.content);
         let sibling = elt.nextSibling;
         while (sibling && (sibling !== originalNextSibling)) {
-            sibling.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (sibling.querySelectorAll) {
+                sibling.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             sibling = sibling.nextSibling;
         }
     });
 };
 export const htmlAppend = opts => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         const originalLastChild = elt.lastChild;
         elt.insertAdjacentHTML('beforeend', opts.content);
         let child = elt.lastChild;
         while (child && (child !== originalLastChild)) {
-            child.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (child.querySelectorAll) {
+                child.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             child = child.previousSibling;
         }
     });
 };
 export const htmlPrepend = opts => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         const originalFirstChild = elt.firstChild;
         elt.insertAdjacentHTML('afterbegin', opts.content);
         let child = elt.firstChild;
         while (child && (child !== originalFirstChild)) {
-            child.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (child.querySelectorAll) {
+                child.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             child = child.nextSibling;
         }
     });
 };
 export const htmlBefore = opts => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         const originalPreviousSibling = elt.previousSibling;
         elt.insertAdjacentHTML('beforebegin', opts.content);
         let sibling = elt.previousSibling;
         while (sibling && (sibling !== originalPreviousSibling)) {
-            sibling.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (sibling.querySelectorAll) {
+                sibling.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             sibling = sibling.previousSibling;
         }
     });
 };
 export const htmlContent = (opts) => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         elt.innerHTML = opts.content;
         let child = elt.firstChild;
         while (child) {
-            child.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (child.querySelectorAll) {
+                child.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             child = child.nextSibling;
         }
     });
 };
 export const htmlReplaceWith = (opts) => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         const previousSibling = elt.previousSibling;
@@ -85,17 +95,19 @@
         const parentNode = elt.parentNode;
         elt.outerHTML = opts.content;
         let sibling = parentNode.firstChild;
         if (previousSibling) {
             sibling = previousSibling.nextSibling;
         }
         while (sibling && (sibling !== nextSibling)) {
-            sibling.dispatchEvent(new Event('DOMContentAdded', {
-                bubbles: true
-            }));
+            if (sibling.querySelectorAll) {
+                sibling.dispatchEvent(new Event('DOMContentAdded', {
+                    bubbles: true
+                }));
+            }
             sibling = sibling.nextSibling;
         }
     });
 };
 export const htmlEmpty = opts => {
     document.querySelectorAll(opts.selector).forEach(elt => {
         while (elt.firstChild) {
```

### Comparing `df_websockets-1.0.3/npm/package-lock.json` & `df_websockets-1.0.8/npm/package-lock.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9111649914113021%*

 * *Differences: {"'dependencies'": "{'@jridgewell/gen-mapping': {'version': '0.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ=='}, "*

 * *                   "'@jridgewell/source-map': {'version': '0.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.t […]*

```diff
@@ -4,22 +4,22 @@
             "dev": true,
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
             "resolved": "https://registry.npmjs.org/@discoveryjs/json-ext/-/json-ext-0.5.7.tgz",
             "version": "0.5.7"
         },
         "@jridgewell/gen-mapping": {
             "dev": true,
-            "integrity": "sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==",
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
             "requires": {
                 "@jridgewell/set-array": "^1.0.1",
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz",
-            "version": "0.3.2"
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "@jridgewell/resolve-uri": {
             "dev": true,
             "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
             "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz",
             "version": "3.1.0"
         },
@@ -27,37 +27,37 @@
             "dev": true,
             "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
             "version": "1.1.2"
         },
         "@jridgewell/source-map": {
             "dev": true,
-            "integrity": "sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==",
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
             "requires": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.2.tgz",
-            "version": "0.3.2"
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
             "version": "1.4.14"
         },
         "@jridgewell/trace-mapping": {
             "dev": true,
-            "integrity": "sha512-oWZNOULl+UbhsgB51uuZzglikfIKSUBO/M9W2OfEjn7cmqoAiCgmv9lyACTUacZwBz0ITnJ2NqjU8Tx0DHL88g==",
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
             "requires": {
-                "@jridgewell/resolve-uri": "^3.0.3",
-                "@jridgewell/sourcemap-codec": "^1.4.10"
+                "@jridgewell/resolve-uri": "3.1.0",
+                "@jridgewell/sourcemap-codec": "1.4.14"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.15.tgz",
-            "version": "0.3.15"
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
         },
         "@types/eslint": {
             "dev": true,
             "integrity": "sha512-/fqTbjxyFUaYNO7VcW5g+4npmqVACz1bB7RTHYuLj+PRjw9hrCwrUXVQFpChUS0JsyEFvMZ7U/PfmvWgxJhI9g==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
@@ -73,175 +73,175 @@
                 "@types/estree": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "@types/estree": {
             "dev": true,
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "@types/json-schema": {
             "dev": true,
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
         "@types/node": {
             "dev": true,
-            "integrity": "sha512-46yIhxSe5xEaJZXWdIBP7GU4HDTG8/eo0qd9atdiL+lFpA03y8KS+lkTN834TWJj5767GbWv4n/P6efyTFt1Dw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.7.13.tgz",
-            "version": "18.7.13"
+            "integrity": "sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.16.3.tgz",
+            "version": "18.16.3"
         },
         "@webassemblyjs/ast": {
             "dev": true,
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-numbers": {
             "dev": true,
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-section": {
             "dev": true,
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/ieee754": {
             "dev": true,
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/leb128": {
             "dev": true,
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-edit": {
             "dev": true,
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-gen": {
             "dev": true,
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-opt": {
             "dev": true,
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-parser": {
             "dev": true,
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wast-printer": {
             "dev": true,
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webpack-cli/configtest": {
             "dev": true,
             "integrity": "sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-1.2.0.tgz",
             "version": "1.2.0"
@@ -461,17 +461,17 @@
                 "prr": "~1.0.1"
             },
             "resolved": "https://registry.npmjs.org/errno/-/errno-0.1.8.tgz",
             "version": "0.1.8"
         },
         "es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "escalade": {
             "dev": true,
             "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
             "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz",
             "version": "3.1.1"
         },
@@ -680,17 +680,17 @@
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
         "json5": {
             "dev": true,
-            "integrity": "sha512-1hqLFMSrGHRHxav9q9gNjJ5EXznIxGVO09xQRrwplcS8qs28pZ8s8hupZAmqDwZUmVZ2Qb2jnyPOWcDH8m8dlA==",
-            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.1.tgz",
-            "version": "2.2.1"
+            "integrity": "sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==",
+            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.3.tgz",
+            "version": "2.2.3"
         },
         "kind-of": {
             "dev": true,
             "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
             "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz",
             "version": "6.0.3"
         },
@@ -698,22 +698,22 @@
             "dev": true,
             "integrity": "sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==",
             "resolved": "https://registry.npmjs.org/loader-runner/-/loader-runner-4.3.0.tgz",
             "version": "4.3.0"
         },
         "loader-utils": {
             "dev": true,
-            "integrity": "sha512-TM57VeHptv569d/GKh6TAYdzKblwDNiumOdkFnejjD0XwTH87K90w3O7AiJRqdQoXygvi1VQTJTLGhJl7WqA7A==",
+            "integrity": "sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==",
             "requires": {
                 "big.js": "^5.2.2",
                 "emojis-list": "^3.0.0",
                 "json5": "^2.1.2"
             },
-            "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.2.tgz",
-            "version": "2.0.2"
+            "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.4.tgz",
+            "version": "2.0.4"
         },
         "locate-path": {
             "dev": true,
             "integrity": "sha512-t7hw9pI+WvuwNJXwk5zVHpyhIqzg2qTlklJOf0mVxGSbe3Fp2VieZcduNYjaLDoy6p9uGpQEGWG87WpMKlNq8g==",
             "requires": {
                 "p-locate": "^4.1.0"
             },
@@ -855,17 +855,17 @@
             "dev": true,
             "integrity": "sha512-yPw4Sng1gWghHQWj0B3ZggWUm4qVbPwPFcRG8KyxiU7J2OHFSoEHKS+EZ3fv5l1t9CyCiop6l/ZYeWbrgoQejw==",
             "resolved": "https://registry.npmjs.org/prr/-/prr-1.0.1.tgz",
             "version": "1.0.1"
         },
         "punycode": {
             "dev": true,
-            "integrity": "sha512-XRsRjdf+j5ml+y/6GKHPZbrF/8p2Yga0JPtdqTIY2Xe5ohJPD9saDJJLPvp9+NSBprVvevdXZybnj2cv8OEd0A==",
-            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.1.1.tgz",
-            "version": "2.1.1"
+            "integrity": "sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==",
+            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz",
+            "version": "2.3.0"
         },
         "randombytes": {
             "dev": true,
             "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
             "requires": {
                 "safe-buffer": "^5.1.0"
             },
@@ -926,40 +926,40 @@
             "dev": true,
             "integrity": "sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==",
             "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz",
             "version": "5.1.2"
         },
         "schema-utils": {
             "dev": true,
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
             "requires": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "semver": {
             "dev": true,
             "integrity": "sha512-QlYTucUYOews+WeEujDoEGziz4K6c47V/Bd+LjSSYcA94p+DmINdf7ncaUinThfvZyu13lN9OY1XDxt8C0Tw0g==",
             "requires": {
                 "lru-cache": "^6.0.0"
             },
             "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.7.tgz",
             "version": "7.3.7"
         },
         "serialize-javascript": {
             "dev": true,
-            "integrity": "sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==",
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
             "requires": {
                 "randombytes": "^2.1.0"
             },
-            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.0.tgz",
-            "version": "6.0.0"
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "shallow-clone": {
             "dev": true,
             "integrity": "sha512-/6KqX+GVUdqPuPPd2LxDDxzX6CAbjJehAAOKlNpqqUpAqPM6HeL8f+o3a+JsyGjn2lv0WY8UsTgUJjU9Ok55NA==",
             "requires": {
                 "kind-of": "^6.0.2"
             },
@@ -1025,36 +1025,36 @@
             "dev": true,
             "integrity": "sha512-4WK/bYZmj8xLr+HUCODHGF1ZFzsYffasLUgEiMBY4fgtltdO6B4WJtlSbPaDTLpYTcGVwM2qLnFTICEcNxs3kA==",
             "resolved": "https://registry.npmjs.org/tapable/-/tapable-1.1.3.tgz",
             "version": "1.1.3"
         },
         "terser": {
             "dev": true,
-            "integrity": "sha512-L1BJiXVmheAQQy+as0oF3Pwtlo4s3Wi1X2zNZ2NxOB4wx9bdS9Vk67XQENLFdLYGCK/Z2di53mTj/hBafR+dTA==",
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
             "requires": {
                 "@jridgewell/source-map": "^0.3.2",
                 "acorn": "^8.5.0",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.15.0.tgz",
-            "version": "5.15.0"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "terser-webpack-plugin": {
             "dev": true,
-            "integrity": "sha512-kfLFk+PoLUQIbLmB1+PZDMRSZS99Mp+/MHqDNmMA6tOItzRt+Npe3E+fsMs5mfcM0wCtrrdU387UnV+vnSffXQ==",
+            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
             "requires": {
-                "@jridgewell/trace-mapping": "^0.3.14",
+                "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
-                "serialize-javascript": "^6.0.0",
-                "terser": "^5.14.1"
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.5"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.6.tgz",
-            "version": "5.3.6"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
+            "version": "5.3.7"
         },
         "to-regex-range": {
             "dev": true,
             "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
             "requires": {
                 "is-number": "^7.0.0"
             },
@@ -1115,59 +1115,59 @@
             "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
             "version": "2.4.0"
         },
         "webpack": {
             "dependencies": {
                 "enhanced-resolve": {
                     "dev": true,
-                    "integrity": "sha512-T0yTFjdpldGY8PmuXXR0PyQ1ufZpEGiHVrp7zHKB7jdR4qlmZHhONVM5AQOAWXuF/w3dnHbEQVrNptJgt7F+cQ==",
+                    "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
                     "requires": {
                         "graceful-fs": "^4.2.4",
                         "tapable": "^2.2.0"
                     },
-                    "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.10.0.tgz",
-                    "version": "5.10.0"
+                    "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+                    "version": "5.13.0"
                 },
                 "tapable": {
                     "dev": true,
                     "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
                     "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz",
                     "version": "2.2.1"
                 }
             },
             "dev": true,
-            "integrity": "sha512-A2InDwnhhGN4LYctJj6M1JEaGL7Luj6LOmyBHjcI8529cm5p6VXiTIW2sn6ffvEAKmveLzvu4jrihwXtPojlAA==",
+            "integrity": "sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==",
             "requires": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.74.0.tgz",
-            "version": "5.74.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.81.0.tgz",
+            "version": "5.81.0"
         },
         "webpack-cli": {
             "dependencies": {
                 "commander": {
                     "dev": true,
                     "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
@@ -1228,25 +1228,25 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "lockfileVersion": 2,
-    "name": "df_websockets",
+    "name": "@d9pouces/df_websockets",
     "packages": {
         "": {
             "devDependencies": {
                 "ts-loader": "^8.0.18",
                 "typescript": "^4.2.3",
-                "webpack": "^5.28.0",
+                "webpack": "^5.81.0",
                 "webpack-cli": "^4.5.0"
             },
             "license": "CECILL-B",
-            "name": "df_websockets",
+            "name": "@d9pouces/df_websockets",
             "version": "0.9.0"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
@@ -1260,17 +1260,17 @@
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/resolve-uri": {
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
@@ -1288,33 +1288,33 @@
         },
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
-            "integrity": "sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
             "version": "1.4.14"
         },
         "node_modules/@jridgewell/trace-mapping": {
             "dependencies": {
-                "@jridgewell/resolve-uri": "^3.0.3",
-                "@jridgewell/sourcemap-codec": "^1.4.10"
+                "@jridgewell/resolve-uri": "3.1.0",
+                "@jridgewell/sourcemap-codec": "1.4.14"
             },
             "dev": true,
-            "integrity": "sha512-oWZNOULl+UbhsgB51uuZzglikfIKSUBO/M9W2OfEjn7cmqoAiCgmv9lyACTUacZwBz0ITnJ2NqjU8Tx0DHL88g==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.15.tgz",
-            "version": "0.3.15"
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
             "dev": true,
@@ -1330,175 +1330,175 @@
             "dev": true,
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "node_modules/@types/estree": {
             "dev": true,
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "node_modules/@types/json-schema": {
             "dev": true,
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
         "node_modules/@types/node": {
             "dev": true,
-            "integrity": "sha512-46yIhxSe5xEaJZXWdIBP7GU4HDTG8/eo0qd9atdiL+lFpA03y8KS+lkTN834TWJj5767GbWv4n/P6efyTFt1Dw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.7.13.tgz",
-            "version": "18.7.13"
+            "integrity": "sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.16.3.tgz",
+            "version": "18.16.3"
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
             "dev": true,
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/leb128": {
             "dependencies": {
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
             "integrity": "sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==",
             "peerDependencies": {
                 "webpack": "4.x.x || 5.x.x",
                 "webpack-cli": "4.x.x"
@@ -1816,17 +1816,17 @@
             "dev": true,
             "integrity": "sha512-dJ6oBr5SQ1VSd9qkk7ByRgb/1SH4JZjCHSW/mr63/QcXO9zLVxvJ6Oy13nio03rxpSnVDDjFor75SjVeZWPW/A==",
             "resolved": "https://registry.npmjs.org/errno/-/errno-0.1.8.tgz",
             "version": "0.1.8"
         },
         "node_modules/es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/escalade": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
@@ -2103,17 +2103,17 @@
             "bin": {
                 "json5": "lib/cli.js"
             },
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
-            "integrity": "sha512-1hqLFMSrGHRHxav9q9gNjJ5EXznIxGVO09xQRrwplcS8qs28pZ8s8hupZAmqDwZUmVZ2Qb2jnyPOWcDH8m8dlA==",
-            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.1.tgz",
-            "version": "2.2.1"
+            "integrity": "sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==",
+            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.3.tgz",
+            "version": "2.2.3"
         },
         "node_modules/kind-of": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
@@ -2135,17 +2135,17 @@
                 "emojis-list": "^3.0.0",
                 "json5": "^2.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=8.9.0"
             },
-            "integrity": "sha512-TM57VeHptv569d/GKh6TAYdzKblwDNiumOdkFnejjD0XwTH87K90w3O7AiJRqdQoXygvi1VQTJTLGhJl7WqA7A==",
-            "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.2.tgz",
-            "version": "2.0.2"
+            "integrity": "sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==",
+            "resolved": "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.4.tgz",
+            "version": "2.0.4"
         },
         "node_modules/locate-path": {
             "dependencies": {
                 "p-locate": "^4.1.0"
             },
             "dev": true,
             "engines": {
@@ -2335,17 +2335,17 @@
             "version": "1.0.1"
         },
         "node_modules/punycode": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
-            "integrity": "sha512-XRsRjdf+j5ml+y/6GKHPZbrF/8p2Yga0JPtdqTIY2Xe5ohJPD9saDJJLPvp9+NSBprVvevdXZybnj2cv8OEd0A==",
-            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.1.1.tgz",
-            "version": "2.1.1"
+            "integrity": "sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==",
+            "resolved": "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz",
+            "version": "2.3.0"
         },
         "node_modules/randombytes": {
             "dependencies": {
                 "safe-buffer": "^5.1.0"
             },
             "dev": true,
             "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
@@ -2433,17 +2433,17 @@
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
@@ -2457,17 +2457,17 @@
             "version": "7.3.7"
         },
         "node_modules/serialize-javascript": {
             "dependencies": {
                 "randombytes": "^2.1.0"
             },
             "dev": true,
-            "integrity": "sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==",
-            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.0.tgz",
-            "version": "6.0.0"
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/shallow-clone": {
             "dependencies": {
                 "kind-of": "^6.0.2"
             },
             "dev": true,
             "engines": {
@@ -2569,51 +2569,51 @@
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-L1BJiXVmheAQQy+as0oF3Pwtlo4s3Wi1X2zNZ2NxOB4wx9bdS9Vk67XQENLFdLYGCK/Z2di53mTj/hBafR+dTA==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.15.0.tgz",
-            "version": "5.15.0"
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
-                "@jridgewell/trace-mapping": "^0.3.14",
+                "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
-                "serialize-javascript": "^6.0.0",
-                "terser": "^5.14.1"
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.5"
             },
             "dev": true,
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-kfLFk+PoLUQIbLmB1+PZDMRSZS99Mp+/MHqDNmMA6tOItzRt+Npe3E+fsMs5mfcM0wCtrrdU387UnV+vnSffXQ==",
+            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.6.tgz",
-            "version": "5.3.6"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
+            "version": "5.3.7"
         },
         "node_modules/to-regex-range": {
             "dependencies": {
                 "is-number": "^7.0.0"
             },
             "dev": true,
             "engines": {
@@ -2712,54 +2712,54 @@
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-A2InDwnhhGN4LYctJj6M1JEaGL7Luj6LOmyBHjcI8529cm5p6VXiTIW2sn6ffvEAKmveLzvu4jrihwXtPojlAA==",
+            "integrity": "sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.74.0.tgz",
-            "version": "5.74.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.81.0.tgz",
+            "version": "5.81.0"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
@@ -2840,17 +2840,17 @@
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-T0yTFjdpldGY8PmuXXR0PyQ1ufZpEGiHVrp7zHKB7jdR4qlmZHhONVM5AQOAWXuF/w3dnHbEQVrNptJgt7F+cQ==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.10.0.tgz",
-            "version": "5.10.0"
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "node_modules/webpack/node_modules/tapable": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
```

### Comparing `df_websockets-1.0.3/npm/webpack.config.js` & `df_websockets-1.0.8/npm/webpack.config.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -16,32 +16,82 @@
 
 'use strict';
 
 // noinspection JSUnresolvedFunction
 const path = require('path');
 
 // noinspection JSUnresolvedVariable,JSUnresolvedFunction
-module.exports = {
+module.exports = [{
     entry: {
         "df_websockets": ['./df_websockets/app.js', './df_websockets/base.js', './df_websockets/forms.ts'],
     },
     resolve: {
         extensions: ['.ts', '.js', '.json']
     },
     output: {
         path: path.resolve(__dirname, '../'),
-        filename: '[name]/static/js/[name].min.js'
+        filename: 'df_websockets/static/js/[name].min.js'
     },
 
     module: {
         rules: [{
             test: /\.tsx?$/,
             use: 'ts-loader',
             exclude: /node_modules/,
         }]
     },
     // Useful for debugging.
     devtool: 'source-map',
     performance: {
         hints: false
     }
-};
+}, {
+    entry: {
+        "df_websockets": ['./df_websockets/app.js', './df_websockets/base.js', './df_websockets/forms.ts'],
+    },
+    resolve: {
+        extensions: ['.ts', '.js', '.json']
+    },
+    output: {
+        path: path.resolve(__dirname, './'),
+        filename: 'dist/js/[name].min.js'
+    },
+
+    module: {
+        rules: [{
+            test: /\.tsx?$/,
+            use: 'ts-loader',
+            exclude: /node_modules/,
+        }]
+    },
+    // Useful for debugging.
+    devtool: 'source-map',
+    performance: {
+        hints: false
+    }
+}, {
+    entry: {
+        "df_websockets": ['./df_websockets/app.js', './df_websockets/base.js', './df_websockets/forms.ts'],
+    },
+    resolve: {
+        extensions: ['.ts', '.js', '.json']
+    },
+    output: {
+        path: path.resolve(__dirname, './'),
+        filename: 'dist/js/[name].js'
+    },
+
+    module: {
+        rules: [{
+            test: /\.tsx?$/,
+            use: 'ts-loader',
+            exclude: /node_modules/,
+        }]
+    },
+    devtool: 'source-map',
+    optimization: {
+        minimize: false
+    },
+    performance: {
+        hints: "warning"
+    }
+}];
```

### Comparing `df_websockets-1.0.3/pre-commit.sh` & `df_websockets-1.0.8/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/setup.cfg` & `df_websockets-1.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: BSD
 	Operating System :: POSIX :: Linux
 	Operating System :: Unix
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 description = Websocket integration for Django
 license = CeCILL-B
 long_description = file: README.md
 long_description_content_type = text/markdown
 maintainer = Matthieu Gallet
 maintainer_email = github@19pouces.net
 name = df_websockets
@@ -73,19 +74,20 @@
 	python demo_manage.py makemigrations
 	python demo_manage.py migrate
 	python demo_manage.py test test_df_websockets
 deps = 
 	aiosmtpd
 	hypothesis
 	nose
+	daphne
 	django22: Django>=2.2,<2.3
 	django30: Django>=3.0,<3.1
 	django31: Django>=3.1,<3.2
 	django32: Django>=3.2,<4.0
-	django40: Django==4.0rc1^
+	django40: Django==4.0
 	channels24: channels>=2.4,<3.0
 	channels30: channels>=3.0,<3.1
 setenv = 
 	DF_REDIS_DB=1
 	DF_REDIS_HOST=localhost
 	DF_REDIS_PASSWORD=
 	DF_REDIS_PORT=16379
```

### Comparing `df_websockets-1.0.3/setup.py` & `df_websockets-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/test_df_websockets/test_consumers.py` & `df_websockets-1.0.8/test_df_websockets/test_consumers.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/test_df_websockets/test_decorators.py` & `df_websockets-1.0.8/test_df_websockets/test_decorators.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/test_df_websockets/test_middleware.py` & `df_websockets-1.0.8/test_df_websockets/test_middleware.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/test_df_websockets/test_testing.py` & `df_websockets-1.0.8/test_df_websockets/test_testing.py`

 * *Files identical despite different names*

### Comparing `df_websockets-1.0.3/test_df_websockets/test_window_info.py` & `df_websockets-1.0.8/test_df_websockets/test_window_info.py`

 * *Files identical despite different names*

