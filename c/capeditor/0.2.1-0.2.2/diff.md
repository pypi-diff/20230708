# Comparing `tmp/capeditor-0.2.1.tar.gz` & `tmp/capeditor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.1.tar", last modified: Fri Jul  7 22:51:20 2023, max compression
+gzip compressed data, was "capeditor-0.2.2.tar", last modified: Fri Jul  7 23:30:25 2023, max compression
```

## Comparing `capeditor-0.2.1.tar` & `capeditor-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 22:51:11.000000 capeditor-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 22:51:20.467099 capeditor-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-07 22:51:11.000000 capeditor-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/migrations/0002_alter_alertinfo_language.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/migrations/0003_alter_alert_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.463099 capeditor-0.2.1/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/static/capeditor/css/cap_style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/static/capeditor/js/hide_attributes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/alert_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/alert_filter_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/alert_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/alert_item_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/alert_list_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/latest_alert_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/pagination_include.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/widgets/basemap_polygon.html
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templates/capeditor/widgets/polygon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/templatetags/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 22:51:11.000000 capeditor-0.2.1/capeditor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:51:20.467099 capeditor-0.2.1/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 22:51:20.000000 capeditor-0.2.1/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-07 22:51:20.000000 capeditor-0.2.1/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:51:20.000000 capeditor-0.2.1/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 22:51:20.000000 capeditor-0.2.1/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 22:51:20.000000 capeditor-0.2.1/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:51:20.467099 capeditor-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-07 22:51:11.000000 capeditor-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.128951 capeditor-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 23:30:14.000000 capeditor-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 23:30:25.128951 capeditor-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-07 23:30:14.000000 capeditor-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.120951 capeditor-0.2.2/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0002_alter_alertinfo_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/0003_alter_alert_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/css/cap_style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/static/capeditor/js/hide_attributes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.112951 capeditor-0.2.2/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_filter_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_item_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/alert_list_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/latest_alert_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/pagination_include.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.124951 capeditor-0.2.2/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/widgets/basemap_polygon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templates/capeditor/widgets/polygon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.128951 capeditor-0.2.2/capeditor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/templatetags/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 23:30:14.000000 capeditor-0.2.2/capeditor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:30:25.120951 capeditor-0.2.2/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 23:30:25.000000 capeditor-0.2.2/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:30:25.128951 capeditor-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-07 23:30:14.000000 capeditor-0.2.2/setup.py
```

### Comparing `capeditor-0.2.1/PKG-INFO` & `capeditor-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.2.1/README.md` & `capeditor-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/migrations/0001_initial.py` & `capeditor-0.2.2/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/migrations/0002_alter_alertinfo_language.py` & `capeditor-0.2.2/capeditor/migrations/0002_alter_alertinfo_language.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/migrations/0003_alter_alert_sender.py` & `capeditor-0.2.2/capeditor/migrations/0003_alter_alert_sender.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/models.py` & `capeditor-0.2.2/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/renderers.py` & `capeditor-0.2.2/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/serializers.py` & `capeditor-0.2.2/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/static/capeditor/css/cap_style.css` & `capeditor-0.2.2/capeditor/static/capeditor/css/cap_style.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.2.2/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/static/capeditor/js/hide_attributes.js` & `capeditor-0.2.2/capeditor/static/capeditor/js/hide_attributes.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/alert_detail.html` & `capeditor-0.2.2/capeditor/templates/capeditor/alert_detail.html`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load wagtailcore_tags static %}
 
 {% block extra_css %}
 {{ block.super }}
 
 <link href='https://unpkg.com/maplibre-gl@2.4.0/dist/maplibre-gl.css' rel='stylesheet' />
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
-<link rel="stylesheet" type="text/css" href="{% static 'css/capeditor/cap_style.css' %}">
+<link rel="stylesheet" type="text/css" href="{% static 'capeditor/css/cap_style.css' %}">
 
 <style>
   .tabs li a {
     color: rgb(239, 239, 239);
   }
   .tabs.is-active {
     color: #333;
```

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/alert_filter_include.html` & `capeditor-0.2.2/capeditor/templates/capeditor/alert_filter_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/alert_index.html` & `capeditor-0.2.2/capeditor/templates/capeditor/alert_index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load wagtailcore_tags static %}
 
 {% block extra_css %}
 {{ block.super }}
 
 <link href='https://unpkg.com/maplibre-gl@2.4.0/dist/maplibre-gl.css' rel='stylesheet' />
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
-<link rel="stylesheet" type="text/css" href="{% static 'css/capeditor/cap_style.css' %}">
+<link rel="stylesheet" type="text/css" href="{% static 'capeditor/css/cap_style.css' %}">
 
 {% endblock %} 
 
 {% block extra_js %} 
 
 {{ block.super }}
 <script src="https://kit.fontawesome.com/db8ac3c257.js" crossorigin="anonymous"></script>
```

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/alert_item_include.html` & `capeditor-0.2.2/capeditor/templates/capeditor/alert_item_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/alert_list_include.html` & `capeditor-0.2.2/capeditor/templates/capeditor/alert_list_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/latest_alert_include.html` & `capeditor-0.2.2/capeditor/templates/capeditor/latest_alert_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/pagination_include.html` & `capeditor-0.2.2/capeditor/templates/capeditor/pagination_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templates/capeditor/widgets/polygon.html` & `capeditor-0.2.2/capeditor/templates/capeditor/widgets/polygon.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/templatetags/pagination.py` & `capeditor-0.2.2/capeditor/templatetags/pagination.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/utils.py` & `capeditor-0.2.2/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/views.py` & `capeditor-0.2.2/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/wagtail_hooks.py` & `capeditor-0.2.2/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor/widgets.py` & `capeditor-0.2.2/capeditor/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/capeditor.egg-info/PKG-INFO` & `capeditor-0.2.2/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.2.1/capeditor.egg-info/SOURCES.txt` & `capeditor-0.2.2/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.1/setup.py` & `capeditor-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requirements = parse_requirements(os.path.join(PROJECT_ROOT, 'requirements.txt'), session=uuid.uuid1())
 
 # e.g. ['django', 'google-api-python-client']
 requirements = [getattr(ir, 'requirement', str(getattr(ir, 'req', None))) for ir in install_requirements]
 
 setup(
     name='capeditor',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     install_requires=requirements,
     include_package_data=True,
     license='MIT License',
     description='Wagtail CAP Editor can be run as standalone or integrated into website',
     long_description=README,
     long_description_content_type='text/markdown',
```

