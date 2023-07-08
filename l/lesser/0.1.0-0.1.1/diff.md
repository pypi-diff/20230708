# Comparing `tmp/lesser-0.1.0.tar.gz` & `tmp/lesser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesser-0.1.0.tar", last modified: Fri Dec  3 23:56:22 2021, max compression
+gzip compressed data, was "lesser-0.1.1.tar", last modified: Sat Jul  8 01:45:41 2023, max compression
```

## Comparing `lesser-0.1.0.tar` & `lesser-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2021-12-03 23:56:22.710211 lesser-0.1.0/
--rw-r--r--   0 jeffwu     (501) staff       (20)       37 2021-03-01 01:12:27.000000 lesser-0.1.0/.gitignore
--rw-r--r--   0 jeffwu     (501) staff       (20)      170 2021-12-03 23:56:22.709897 lesser-0.1.0/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)     1629 2021-12-03 23:31:22.000000 lesser-0.1.0/README.md
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2021-12-03 23:56:22.707926 lesser-0.1.0/lesser.egg-info/
--rw-r--r--   0 jeffwu     (501) staff       (20)      170 2021-12-03 23:56:22.000000 lesser-0.1.0/lesser.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)      233 2021-12-03 23:56:22.000000 lesser-0.1.0/lesser.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)        1 2021-12-03 23:56:22.000000 lesser-0.1.0/lesser.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)        7 2021-12-03 23:56:22.000000 lesser-0.1.0/lesser.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)     4907 2021-12-03 23:55:49.000000 lesser-0.1.0/lesser.py
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2021-12-03 23:56:22.709290 lesser-0.1.0/old_functional/
--rw-r--r--   0 jeffwu     (501) staff       (20)     2719 2021-03-01 01:12:27.000000 lesser-0.1.0/old_functional/lesser.py
--rw-r--r--   0 jeffwu     (501) staff       (20)      722 2021-03-01 01:12:27.000000 lesser-0.1.0/old_functional/old_test_lesser.py
--rw-r--r--   0 jeffwu     (501) staff       (20)       38 2021-12-03 23:56:22.710310 lesser-0.1.0/setup.cfg
--rw-r--r--   0 jeffwu     (501) staff       (20)      203 2021-12-03 23:56:10.000000 lesser-0.1.0/setup.py
--rw-r--r--   0 jeffwu     (501) staff       (20)     1848 2021-03-01 01:12:27.000000 lesser-0.1.0/test_lesser.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-08 01:45:41.515880 lesser-0.1.1/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       37 2021-03-01 01:12:27.000000 lesser-0.1.1/.gitignore
+-rw-r--r--   0 jeffwu     (503) staff       (20)      106 2023-07-08 01:45:41.515393 lesser-0.1.1/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)     1629 2021-12-03 23:31:22.000000 lesser-0.1.1/README.md
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-08 01:45:41.508239 lesser-0.1.1/lesser.egg-info/
+-rw-r--r--   0 jeffwu     (503) staff       (20)      106 2023-07-08 01:45:40.000000 lesser-0.1.1/lesser.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)      233 2023-07-08 01:45:40.000000 lesser-0.1.1/lesser.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-07-08 01:45:40.000000 lesser-0.1.1/lesser.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        7 2023-07-08 01:45:40.000000 lesser-0.1.1/lesser.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)     5151 2023-07-08 01:45:09.000000 lesser-0.1.1/lesser.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-08 01:45:41.514593 lesser-0.1.1/old_functional/
+-rw-r--r--   0 jeffwu     (503) staff       (20)     2719 2021-03-01 01:12:27.000000 lesser-0.1.1/old_functional/lesser.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)      722 2021-03-01 01:12:27.000000 lesser-0.1.1/old_functional/old_test_lesser.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-07-08 01:45:41.515985 lesser-0.1.1/setup.cfg
+-rw-r--r--   0 jeffwu     (503) staff       (20)      203 2023-07-08 01:45:36.000000 lesser-0.1.1/setup.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)     1991 2023-07-08 01:45:05.000000 lesser-0.1.1/test_lesser.py
```

### Comparing `lesser-0.1.0/README.md` & `lesser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lesser-0.1.0/lesser.py` & `lesser-0.1.1/lesser.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,21 @@
 
     def __add__(self, other):
         f = self.clone()
         for d in other.to_dicts():
             f.append(d)
         return f
 
+    def __getitem__(self, key):
+        if isinstance(key, slice):
+            return Frame(**{k: v[key] for k, v in self.items()})
+        if isinstance(key, int):
+            return self.index(key)
+        return dict.__getitem__(self, key)
+
     def at(self, inds):
         """
         Like iloc for a list of integers
         """
         result = Frame()
         for i in inds:
             result.append(self.index(i))
```

### Comparing `lesser-0.1.0/old_functional/lesser.py` & `lesser-0.1.1/old_functional/lesser.py`

 * *Files identical despite different names*

### Comparing `lesser-0.1.0/old_functional/old_test_lesser.py` & `lesser-0.1.1/old_functional/old_test_lesser.py`

 * *Files identical despite different names*

### Comparing `lesser-0.1.0/test_lesser.py` & `lesser-0.1.1/test_lesser.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 def test_simple():
     dicts = [
         dict(x=1, y=2),
         dict(x=2, z=3),
     ]
     f = lpd.from_dicts(dicts)
     assert lpd.to_dicts(f) == dicts
+    assert f[0] == dicts[0]
+    assert f[-1] == dicts[-1]
+    assert f[:].to_dicts() == dicts[:]
 
     new = dict(x=2, y=2)
     assert lpd.size(f) == 2
     f.append(new)
     assert lpd.size(f) == 3
     assert lpd.to_dicts(f) == dicts + [new]
     grouped = lpd.group_by(f, 'x')
@@ -46,7 +49,10 @@
         )
         .sort_by(lambda x: x["sleep_hours"])
     )
 
     assert reactions_by_sleep['sleep_hours'] == [5, 6, 7, 8, 9]
     assert reactions_by_sleep['average_reaction_time'] == [88, 94, 81, (60 + 71) / 2, 62]
 
+
+if __name__ == "__main__":
+    pytest.main()
```

