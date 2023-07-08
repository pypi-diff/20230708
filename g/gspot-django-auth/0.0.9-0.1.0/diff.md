# Comparing `tmp/gspot_django_auth-0.0.9.tar.gz` & `tmp/gspot_django_auth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.9.tar", last modified: Thu Jun 29 18:24:47 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.1.0.tar", last modified: Sat Jul  8 19:52:40 2023, max compression
```

## Comparing `gspot_django_auth-0.0.9.tar` & `gspot_django_auth-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.284955 gspot_django_auth-0.0.9/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.9/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.9/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:24:47.285071 gspot_django_auth-0.0.9/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-29 18:24:44.000000 gspot_django_auth-0.0.9/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.283858 gspot_django_auth-0.0.9/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.9/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-06-29 18:23:56.000000 gspot_django_auth-0.0.9/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      362 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.9/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1204 2023-06-27 17:15:40.000000 gspot_django_auth-0.0.9/gspot_django_auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      557 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.9/gspot_django_auth/permissions.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.9/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.9/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.284790 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      487 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-29 18:24:17.000000 gspot_django_auth-0.0.9/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-29 18:24:47.285433 gspot_django_auth-0.0.9/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      132 2023-06-29 18:20:10.000000 gspot_django_auth-0.0.9/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-08 19:52:40.804633 gspot_django_auth-0.1.0/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.0/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.0/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-07-08 19:52:40.804722 gspot_django_auth-0.1.0/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-29 18:24:44.000000 gspot_django_auth-0.1.0/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-08 19:52:40.803006 gspot_django_auth-0.1.0/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.0/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.0/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.0/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1244 2023-07-08 19:21:47.000000 gspot_django_auth-0.1.0/gspot_django_auth/models.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-08 19:52:40.804489 gspot_django_auth-0.1.0/gspot_django_auth/permissions/
+-rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.0/gspot_django_auth/permissions/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.0/gspot_django_auth/permissions/permissons.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.0/gspot_django_auth/permissions/validators.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.0/gspot_django_auth/permissions/verifiers.py
+-rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.0/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.0/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-08 19:52:40.803857 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-07-08 19:52:40.000000 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      627 2023-07-08 19:52:40.000000 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-08 19:52:40.000000 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-08 19:52:40.000000 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-08 19:52:40.000000 gspot_django_auth-0.1.0/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-08 19:40:14.000000 gspot_django_auth-0.1.0/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-08 19:52:40.805041 gspot_django_auth-0.1.0/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.0/setup.py
```

### Comparing `gspot_django_auth-0.0.9/LICENSE` & `gspot_django_auth-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.9/PKG-INFO` & `gspot_django_auth-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.9/README.md` & `gspot_django_auth-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.9/gspot_django_auth/authentication.py` & `gspot_django_auth-0.1.0/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.9/gspot_django_auth/models.py` & `gspot_django_auth-0.1.0/gspot_django_auth/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 @dataclass(frozen=True)
 class BaseUser:
     user_id: UUID
     email: str
     phone: str
     avatar: str
     country: str
+    is_banned: bool
+    is_active: bool
     created_at: datetime
     updated_at: datetime
 
     to_dict = asdict
 
 
 @dataclass(frozen=True)
```

### Comparing `gspot_django_auth-0.0.9/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.1.0/gspot_django_auth/redis_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,10 @@
         return self.__redis_client
 
     def __get(self, name: str) -> dict | None:
         value = self.conn.get(name)
         if value:
             return json.loads(value)
 
-    def __put(self, name: str, value: dict, ttl: int) -> None:
-        value_data = json.dumps(value)
-        self.conn.set(name=name, value=value_data, ex=ttl)
-
     def is_token_exist(self, token: str, prefix: bool = True) -> dict | None:
         key = f'{self._prefix}:{token}' if prefix else token
         return self.__get(key)
```

### Comparing `gspot_django_auth-0.0.9/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.1.0/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.9/pyproject.toml` & `gspot_django_auth-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.0.9/setup.cfg` & `gspot_django_auth-0.1.0/setup.cfg`

 * *Files identical despite different names*

