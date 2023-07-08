# Comparing `tmp/nescs-0.3.1.tar.gz` & `tmp/nescs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nescs-0.3.1.tar", last modified: Thu Jul  6 17:03:48 2023, max compression
+gzip compressed data, was "nescs-0.3.2.tar", last modified: Sat Jul  8 18:21:05 2023, max compression
```

## Comparing `nescs-0.3.1.tar` & `nescs-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:03:48.527094 nescs-0.3.1/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-06 15:30:37.000000 nescs-0.3.1/MANIFEST.in
--rw-r--r--   0 twoics    (1000) twoics    (1000)      422 2023-07-06 17:03:48.527094 nescs-0.3.1/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      210 2023-07-06 15:48:59.000000 nescs-0.3.1/README.rst
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:03:48.526094 nescs-0.3.1/nesc/
--rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-06 16:08:50.000000 nescs-0.3.1/nesc/__init__.py
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5062 2023-07-06 15:30:37.000000 nescs-0.3.1/nesc/service.py
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:03:48.527094 nescs-0.3.1/nescs.egg-info/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      422 2023-07-06 17:03:48.000000 nescs-0.3.1/nescs.egg-info/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-06 17:03:48.000000 nescs-0.3.1/nescs.egg-info/SOURCES.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-06 17:03:48.000000 nescs-0.3.1/nescs.egg-info/dependency_links.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       27 2023-07-06 17:03:48.000000 nescs-0.3.1/nescs.egg-info/requires.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-06 17:03:48.000000 nescs-0.3.1/nescs.egg-info/top_level.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-06 15:30:37.000000 nescs-0.3.1/pyproject.toml
--rw-r--r--   0 twoics    (1000) twoics    (1000)      340 2023-07-06 17:03:48.527094 nescs-0.3.1/setup.cfg
--rw-r--r--   0 twoics    (1000) twoics    (1000)      116 2023-07-06 17:03:18.000000 nescs-0.3.1/setup.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.614515 nescs-0.3.2/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-08 05:36:40.000000 nescs-0.3.2/MANIFEST.in
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5094 2023-07-08 18:21:05.614515 nescs-0.3.2/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     4882 2023-07-08 18:18:34.000000 nescs-0.3.2/README.rst
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.613515 nescs-0.3.2/nesc/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-08 05:36:40.000000 nescs-0.3.2/nesc/__init__.py
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5189 2023-07-08 18:11:53.000000 nescs-0.3.2/nesc/service.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.614515 nescs-0.3.2/nescs.egg-info/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5094 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/SOURCES.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/dependency_links.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       42 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/requires.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/top_level.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-08 05:36:40.000000 nescs-0.3.2/pyproject.toml
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      408 2023-07-08 18:21:05.614515 nescs-0.3.2/setup.cfg
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      131 2023-07-08 05:36:40.000000 nescs-0.3.2/setup.py
```

### Comparing `nescs-0.3.1/nesc/service.py` & `nescs-0.3.2/nesc/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 class SerializerCreateService:
     def __init__(self, serializer, validated_data, child_fields=None, fk_fields=None, m2m_fields=None):
         self._serializer = serializer
         self._validated_data = validated_data
         self._child_fields = child_fields or []
         self._fk_fields = fk_fields or []
         self._m2m_fields = m2m_fields or []
-        for field in self._child_fields:
+
+        poped_fields = self._m2m_fields + self._child_fields
+        for field in poped_fields:
             self._validated_data.pop(field, None)
 
     @staticmethod
     def get_related_name_from_field_name(serializer_class, field_name):
         model = serializer_class.Meta.model
         for field in model._meta.get_fields():
             if hasattr(field, '_related_name') and field_name == field._related_name:
@@ -61,15 +63,16 @@
             for raw_data in raw_data_list:
                 nested_context = {
                     'request': context.get("request"),
                     'raw_data': raw_data,
                 }
                 nested_serializer = serializer_class(data=raw_data, context=nested_context)
                 nested_serializer.is_valid(raise_exception=True)
-                nested_serializer.save(**{related_name: parent_instance})
+                instance = nested_serializer.save(**{related_name: parent_instance})
+                self._validated_data[field_name] = instance
 
     def create_fk_instances(self):
         context = self._serializer.context
         for field_name, field_type in self._serializer.fields.items():
             if field_name not in self._fk_fields:
                 continue
             serializer_class = self.get_serializer_class(field_type)
```

