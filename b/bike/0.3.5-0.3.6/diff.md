# Comparing `tmp/bike-0.3.5.tar.gz` & `tmp/bike-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.3.5.tar", max compression
+gzip compressed data, was "bike-0.3.6.tar", max compression
```

## Comparing `bike-0.3.5.tar` & `bike-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.5/LICENSE
--rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.5/README.md
--rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.5/bike/__init__.py
--rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.5/bike/controllers.py
--rw-r--r--   0        0        0     3086 2023-07-06 18:04:51.285877 bike-0.3.5/bike/fields.py
--rw-r--r--   0        0        0     8609 2023-07-07 09:34:46.693316 bike-0.3.5/bike/models.py
--rw-r--r--   0        0        0      495 2023-07-07 09:34:46.681316 bike-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.6/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.6/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.6/bike/controllers.py
+-rw-r--r--   0        0        0     3064 2023-07-08 11:11:57.800247 bike-0.3.6/bike/fields.py
+-rw-r--r--   0        0        0     8743 2023-07-07 10:13:56.882414 bike-0.3.6/bike/models.py
+-rw-r--r--   0        0        0      495 2023-07-08 11:08:57.388699 bike-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.6/PKG-INFO
```

### Comparing `bike-0.3.5/LICENSE` & `bike-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.3.5/README.md` & `bike-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bike-0.3.5/bike/controllers.py` & `bike-0.3.6/bike/controllers.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.5/bike/fields.py` & `bike-0.3.6/bike/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return value
 
     def __set__(self, obj, value):
         value = self.__prepare_value(value, self)
         setattr(obj, f'_{self.name}', value)
 
     def __prepare_value(self, value, instance):
-        if (value is None or str(value) == '') and self.required:
+        if value is None and self.required:
             if self.default is not None:
                 return self.default
             else:
                 raise Exception(f'Field {self.name} required.')
         for validator in self.validators_pre:
             value = validator(self.model, value)
         if value is None:
```

### Comparing `bike-0.3.5/bike/models.py` & `bike-0.3.6/bike/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,24 +166,26 @@
             field_name = getattr(member, '__validator_field__')
             field = fields.get(field_name, None)
             pre = getattr(member, '__validator_pre__')
             field.set_validators(member, pre=pre)
             remove_members.append(name)
         elif inspect.isfunction(member) and not name.startswith('__') and not name.endswith('__'):
             methods[name] = member
+    module_name = cls.__module__
     class_name = cls.__name__
     if issubclass(cls, Model):
         for name, field in fields.items():
             setattr(cls, name, field)
     elif not hasattr(cls, '__ready__') and not issubclass(cls, Model):
         cls = type(class_name, (Model,), {**fields, **methods})
     cls.__fields__ = fields
     cls.__fields_type_list__ = fields_list
     cls.__fields_type_object__ = fields_object
     cls.__name__ = class_name
+    cls.__module__ = module_name
     cls.__ready__ = True
     init_fn = create_init_function(fields)
     setattr(cls, '__init__', init_fn)
     return cls
 
 
 def get_fields_from_annotations(
@@ -252,12 +254,18 @@
         func.__validator_field__ = field
         func.__validator_pre__ = pre
         return func
     return wrapper
 
 
 def model(
+        cls=None,
+        /,
+        *,
         alias_load: bool = True
-) -> callable:
-    def wrapper(cls) -> Model:
+):
+    def wrapper(cls):
         return prepare_fields(cls, alias_load=alias_load)
-    return wrapper
+
+    if cls is None:
+        return wrapper
+    return wrapper(cls)
```

### Comparing `bike-0.3.5/PKG-INFO` & `bike-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bike
-Version: 0.3.5
+Version: 0.3.6
 Summary: A lightweight model validator for modern projects.
 Home-page: https://github.com/manasseslima/bike
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

