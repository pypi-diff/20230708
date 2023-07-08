# Comparing `tmp/skinny_orm-0.1.0.tar.gz` & `tmp/skinny_orm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skinny_orm-0.1.0.tar", max compression
+gzip compressed data, was "skinny_orm-0.1.1.tar", max compression
```

## Comparing `skinny_orm-0.1.0.tar` & `skinny_orm-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      348 2023-07-04 19:49:28.385172 skinny_orm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 21:26:32.596656 skinny_orm-0.1.0/readme.MD
--rw-r--r--   0        0        0        0 2023-07-03 21:21:19.280907 skinny_orm-0.1.0/skinny_orm/__init__.py
--rw-r--r--   0        0        0     1436 2023-07-05 14:24:09.961093 skinny_orm-0.1.0/skinny_orm/base_field.py
--rw-r--r--   0        0        0     1302 2023-07-05 16:10:11.171173 skinny_orm-0.1.0/skinny_orm/base_orm.py
--rw-r--r--   0        0        0      594 2023-07-06 21:42:12.038160 skinny_orm-0.1.0/skinny_orm/exceptions.py
--rw-r--r--   0        0        0      342 2023-07-05 14:31:57.492154 skinny_orm-0.1.0/skinny_orm/orm.py
--rw-r--r--   0        0        0    11555 2023-07-07 17:49:08.818179 skinny_orm-0.1.0/skinny_orm/sqlite_orm.py
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 skinny_orm-0.1.0/setup.py
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 skinny_orm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-07-08 10:57:57.936905 skinny_orm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2055 2023-07-08 09:38:23.409960 skinny_orm-0.1.1/readme.MD
+-rw-r--r--   0        0        0        0 2023-07-03 21:21:19.280907 skinny_orm-0.1.1/skinny_orm/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-07 18:16:44.910472 skinny_orm-0.1.1/skinny_orm/base_field.py
+-rw-r--r--   0        0        0     1302 2023-07-05 16:10:11.171173 skinny_orm-0.1.1/skinny_orm/base_orm.py
+-rw-r--r--   0        0        0      594 2023-07-06 21:42:12.038160 skinny_orm-0.1.1/skinny_orm/exceptions.py
+-rw-r--r--   0        0        0      342 2023-07-05 14:31:57.492154 skinny_orm-0.1.1/skinny_orm/orm.py
+-rw-r--r--   0        0        0    11562 2023-07-08 10:52:38.220885 skinny_orm-0.1.1/skinny_orm/sqlite_orm.py
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 skinny_orm-0.1.1/setup.py
+-rw-r--r--   0        0        0     2317 1970-01-01 00:00:00.000000 skinny_orm-0.1.1/PKG-INFO
```

### Comparing `skinny_orm-0.1.0/skinny_orm/base_field.py` & `skinny_orm-0.1.1/skinny_orm/base_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,9 @@
 
     def __and__(self, other):
         self.comparators.extend(other.comparators)
         self.and_or_s.append('and')
         return self
 
     def __or__(self, other):
-        self.comparators.extend(other.comparators)
         self.and_or_s.append('or')
         return self
```

### Comparing `skinny_orm-0.1.0/skinny_orm/base_orm.py` & `skinny_orm-0.1.1/skinny_orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `skinny_orm-0.1.0/skinny_orm/exceptions.py` & `skinny_orm-0.1.1/skinny_orm/exceptions.py`

 * *Files identical despite different names*

### Comparing `skinny_orm-0.1.0/skinny_orm/sqlite_orm.py` & `skinny_orm-0.1.1/skinny_orm/sqlite_orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             cursor.close()
             if commit:
                 self.connection.commit()
             return [self.current_entity(*self._parse_and_get_new_tuple(r)) for r in res]
         except sqlite3.OperationalError as e:
             if self.create_tables_if_not_exists and 'no such table' in str(e):
                 self._create_table(self.current_entity, cursor)
-                self.all(commit)
+                return self.all(commit)
             else:
                 raise e
         except Exception as e:
             cursor.close()
             raise e
 
     def first(self):
```

