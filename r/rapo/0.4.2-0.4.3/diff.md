# Comparing `tmp/rapo-0.4.2.tar.gz` & `tmp/rapo-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapo-0.4.2.tar", last modified: Sat Jul  8 18:10:56 2023, max compression
+gzip compressed data, was "rapo-0.4.3.tar", last modified: Sat Jul  8 17:51:31 2023, max compression
```

## Comparing `rapo-0.4.2.tar` & `rapo-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0 timur      (501) staff       (20)     1241 2023-06-08 12:00:13.196041 PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)     1074 2023-04-11 10:47:36.000000 LICENSE
--rw-r--r--   0 timur      (501) staff       (20)      736 2023-05-05 01:01:51.000000 README.md
--rw-r--r--   0 timur      (501) staff       (20)     1363 2023-06-08 11:51:17.000000 setup.py
--rw-r--r--   0 timur      (501) staff       (20)       38 2023-06-08 12:00:13.196228 setup.cfg
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.193024 rapo.egg-info/
--rw-r--r--   0 timur      (501) staff       (20)     1241 2023-06-08 12:00:13.000000 rapo.egg-info/PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)      507 2023-06-08 12:00:13.000000 rapo.egg-info/SOURCES.txt
--rw-r--r--   0 timur      (501) staff       (20)        1 2023-06-08 12:00:13.000000 rapo.egg-info/dependency_links.txt
--rw-r--r--   0 timur      (501) staff       (20)      134 2023-06-08 12:00:13.000000 rapo.egg-info/requires.txt
--rw-r--r--   0 timur      (501) staff       (20)        5 2023-06-08 12:00:13.000000 rapo.egg-info/top_level.txt
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.192238 rapo/
--rw-r--r--   0 timur      (501) staff       (20)      469 2023-06-08 11:57:44.000000 rapo/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)     3028 2023-06-08 11:40:17.000000 rapo/config.py
--rw-r--r--   0 timur      (501) staff       (20)     8367 2023-06-08 11:40:17.000000 rapo/database.py
--rw-r--r--   0 timur      (501) staff       (20)      290 2023-06-08 11:40:17.000000 rapo/logger.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.194155 rapo/main/
--rw-r--r--   0 timur      (501) staff       (20)      155 2023-04-11 10:47:36.000000 rapo/main/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)      166 2023-05-24 22:17:47.000000 rapo/main/case.py
--rw-r--r--   0 timur      (501) staff       (20)    77165 2023-06-08 11:40:17.000000 rapo/main/control.py
--rw-r--r--   0 timur      (501) staff       (20)      799 2023-05-23 18:23:42.000000 rapo/main/fields.py
--rw-r--r--   0 timur      (501) staff       (20)    14082 2023-06-08 11:40:17.000000 rapo/main/scheduler.py
--rw-r--r--   0 timur      (501) staff       (20)     3523 2023-05-05 00:23:30.000000 rapo/reader.py
--rw-r--r--   0 timur      (501) staff       (20)     2848 2023-05-24 22:38:45.000000 rapo/utils.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.194373 rapo/web/
--rw-r--r--   0 timur      (501) staff       (20)     4525 2023-05-05 00:23:06.000000 rapo/web/__init__.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.195359 rapo/web/api/
--rw-r--r--   0 timur      (501) staff       (20)       48 2023-04-11 10:47:36.000000 rapo/web/api/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)     3025 2023-05-24 22:19:27.000000 rapo/web/api/app.py
--rw-r--r--   0 timur      (501) staff       (20)      249 2023-04-11 10:47:36.000000 rapo/web/api/auth.py
--rw-r--r--   0 timur      (501) staff       (20)      170 2023-04-11 10:47:36.000000 rapo/web/api/response.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-06-08 12:00:13.195596 rapo/web/api/templates/
--rw-r--r--   0 timur      (501) staff       (20)      279 2023-04-11 10:47:36.000000 rapo/web/api/templates/help.html
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.145784 rapo-0.4.3/
+-rw-r--r--   0 timur      (501) staff       (20)     1074 2023-04-11 10:47:36.000000 rapo-0.4.3/LICENSE
+-rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-08 17:51:31.145570 rapo-0.4.3/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)     3199 2023-07-08 17:44:30.000000 rapo-0.4.3/README.md
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.142525 rapo-0.4.3/rapo/
+-rw-r--r--   0 timur      (501) staff       (20)      469 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)     3028 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/config.py
+-rw-r--r--   0 timur      (501) staff       (20)     8367 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/database.py
+-rw-r--r--   0 timur      (501) staff       (20)      290 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/logger.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144007 rapo-0.4.3/rapo/main/
+-rw-r--r--   0 timur      (501) staff       (20)      155 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/main/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)      166 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/case.py
+-rw-r--r--   0 timur      (501) staff       (20)    77165 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/control.py
+-rw-r--r--   0 timur      (501) staff       (20)      799 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/fields.py
+-rw-r--r--   0 timur      (501) staff       (20)    14060 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/scheduler.py
+-rw-r--r--   0 timur      (501) staff       (20)     3523 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/reader.py
+-rw-r--r--   0 timur      (501) staff       (20)     2848 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/utils.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144150 rapo-0.4.3/rapo/web/
+-rw-r--r--   0 timur      (501) staff       (20)     4525 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/web/__init__.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144634 rapo-0.4.3/rapo/web/api/
+-rw-r--r--   0 timur      (501) staff       (20)       48 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)     3025 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/web/api/app.py
+-rw-r--r--   0 timur      (501) staff       (20)      249 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/auth.py
+-rw-r--r--   0 timur      (501) staff       (20)      170 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/response.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144773 rapo-0.4.3/rapo/web/api/templates/
+-rw-r--r--   0 timur      (501) staff       (20)      279 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/templates/help.html
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.143241 rapo-0.4.3/rapo.egg-info/
+-rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)      507 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/SOURCES.txt
+-rw-r--r--   0 timur      (501) staff       (20)        1 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/dependency_links.txt
+-rw-r--r--   0 timur      (501) staff       (20)      134 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/requires.txt
+-rw-r--r--   0 timur      (501) staff       (20)        5 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/top_level.txt
+-rw-r--r--   0 timur      (501) staff       (20)       38 2023-07-08 17:51:31.145837 rapo-0.4.3/setup.cfg
+-rw-r--r--   0 timur      (501) staff       (20)     1363 2023-07-08 17:44:30.000000 rapo-0.4.3/setup.py
```

### Comparing `LICENSE` & `rapo-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `setup.py` & `rapo-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `rapo/config.py` & `rapo-0.4.3/rapo/config.py`

 * *Files identical despite different names*

### Comparing `rapo/database.py` & `rapo-0.4.3/rapo/database.py`

 * *Files identical despite different names*

### Comparing `rapo/main/control.py` & `rapo-0.4.3/rapo/main/control.py`

 * *Files identical despite different names*

### Comparing `rapo/main/fields.py` & `rapo-0.4.3/rapo/main/fields.py`

 * *Files identical despite different names*

### Comparing `rapo/main/scheduler.py` & `rapo-0.4.3/rapo/main/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,14 @@
     def _maintain(self):
         while True:
             if self.maintenance.is_set():
                 logger.info('Starting maintenance')
                 self._clean()
                 self.maintenance.clear()
                 logger.info('Maintenance performed')
-                break
             time.sleep(1)
 
     def _clean(self):
         config = db.tables.config
         select = config.select().order_by(config.c.control_id)
         result = db.execute(select)
         for row in result:
```

### Comparing `rapo/reader.py` & `rapo-0.4.3/rapo/reader.py`

 * *Files identical despite different names*

### Comparing `rapo/utils.py` & `rapo-0.4.3/rapo/utils.py`

 * *Files identical despite different names*

### Comparing `rapo/web/__init__.py` & `rapo-0.4.3/rapo/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rapo/web/api/app.py` & `rapo-0.4.3/rapo/web/api/app.py`

 * *Files identical despite different names*

