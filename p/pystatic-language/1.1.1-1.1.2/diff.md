# Comparing `tmp/pystatic-language-1.1.1.tar.gz` & `tmp/pystatic-language-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystatic-language-1.1.1.tar", last modified: Sat Jul  1 08:19:44 2023, max compression
+gzip compressed data, was "pystatic-language-1.1.2.tar", last modified: Sat Jul  8 07:33:27 2023, max compression
```

## Comparing `pystatic-language-1.1.1.tar` & `pystatic-language-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/
--rw-rw-rw-   0        0        0      115 2023-07-01 08:19:43.000000 pystatic-language-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4116 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3028 2023-06-29 08:39:46.000000 pystatic-language-1.1.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.1.1/build.py
--rw-rw-rw-   0        0        0      925 2023-07-01 08:19:43.000000 pystatic-language-1.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.284794 pystatic-language-1.1.1/pystatic/
--rw-rw-rw-   0        0        0     2900 2023-06-29 08:31:21.000000 pystatic-language-1.1.1/pystatic/casting.py
--rw-rw-rw-   0        0        0     1408 2023-06-29 08:31:59.000000 pystatic-language-1.1.1/pystatic/clean.py
--rw-rw-rw-   0        0        0     5536 2023-06-29 08:34:59.000000 pystatic-language-1.1.1/pystatic/overload.py
--rw-rw-rw-   0        0        0     2879 2023-06-29 08:35:26.000000 pystatic-language-1.1.1/pystatic/private.py
--rw-rw-rw-   0        0        0     8106 2023-06-29 07:23:27.000000 pystatic-language-1.1.1/pystatic/types.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.301037 pystatic-language-1.1.1/pystatic_language.egg-info/
--rw-rw-rw-   0        0        0     4116 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-07-01 08:19:22.000000 pystatic-language-1.1.1/setup.py
--rw-rw-rw-   0        0        0     2783 2023-06-29 08:38:30.000000 pystatic-language-1.1.1/test.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:33:27.206944 pystatic-language-1.1.2/
+-rw-rw-rw-   0        0        0      115 2023-07-08 07:33:25.000000 pystatic-language-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4116 2023-07-08 07:33:27.205945 pystatic-language-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3028 2023-06-29 08:39:46.000000 pystatic-language-1.1.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.1.2/build.py
+-rw-rw-rw-   0        0        0      925 2023-07-08 07:33:25.000000 pystatic-language-1.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-08 07:33:27.190437 pystatic-language-1.1.2/pystatic/
+-rw-rw-rw-   0        0        0     2927 2023-07-08 07:27:18.000000 pystatic-language-1.1.2/pystatic/casting.py
+-rw-rw-rw-   0        0        0     1408 2023-06-29 08:31:59.000000 pystatic-language-1.1.2/pystatic/clean.py
+-rw-rw-rw-   0        0        0     5715 2023-07-08 07:30:07.000000 pystatic-language-1.1.2/pystatic/overload.py
+-rw-rw-rw-   0        0        0     2969 2023-07-08 07:31:56.000000 pystatic-language-1.1.2/pystatic/private.py
+-rw-rw-rw-   0        0        0     8106 2023-06-29 07:23:27.000000 pystatic-language-1.1.2/pystatic/types.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:33:27.204975 pystatic-language-1.1.2/pystatic_language.egg-info/
+-rw-rw-rw-   0        0        0     4116 2023-07-08 07:33:27.000000 pystatic-language-1.1.2/pystatic_language.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-07-08 07:33:27.000000 pystatic-language-1.1.2/pystatic_language.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 07:33:27.000000 pystatic-language-1.1.2/pystatic_language.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-08 07:33:27.000000 pystatic-language-1.1.2/pystatic_language.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 07:33:27.000000 pystatic-language-1.1.2/pystatic_language.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.1.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 07:33:27.206944 pystatic-language-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-07-08 07:32:26.000000 pystatic-language-1.1.2/setup.py
+-rw-rw-rw-   0        0        0     2783 2023-06-29 08:38:30.000000 pystatic-language-1.1.2/test.py
```

### Comparing `pystatic-language-1.1.1/PKG-INFO` & `pystatic-language-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.1.1
+Version: 1.1.2
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.1.1/README.md` & `pystatic-language-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.1/build.py` & `pystatic-language-1.1.2/build.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.1/pyproject.toml` & `pystatic-language-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pystatic-language'
-version = '1.1.1'
+version = '1.1.2'
 description = "This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and."
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pystatic-language-1.1.1/pystatic/casting.py` & `pystatic-language-1.1.2/pystatic/casting.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 _T = TypeVar("_T")
 _O = TypeVar("_O")
 
 class CastType:
     """A class to represent a casting type mechanism."""
 
+    __slots__ = "base",
+
     def __init__(self, base: Type[_T]) -> None:
         """
         Defines the class attributes.
 
         :param base: The type to cast the object into.
         """
```

### Comparing `pystatic-language-1.1.1/pystatic/clean.py` & `pystatic-language-1.1.2/pystatic/clean.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.1/pystatic/overload.py` & `pystatic-language-1.1.2/pystatic/overload.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 __all__ = [
     "Overload",
     "overload"
 ]
 
 def overload_signature_error_message(
-        c: Callable, args: Tuple, kwargs: Dict[str, Any]
+        c: Callable, /, *, args: Tuple, kwargs: Dict[str, Any]
 ) -> str:
     """
     Returns the error message.
 
     :param c: The callable object.
     :param args: The arguments fof the call.
     :param kwargs: The keyword arguments for the call.
@@ -45,15 +45,15 @@
         :param c: The callable object.
     :param args: The arguments fof the call.
     :param kwargs: The keyword arguments for the call.
         """
 
         super().__init__(
             overload_signature_error_message(
-                c=c, args=args, kwargs=kwargs
+                c, args=args, kwargs=kwargs
             )
         )
     # end __init__
 # end OverloadSignatureTypeError
 
 class OverloadSignatureTypeWarning(Warning):
     """A class to represent a runtime type warning."""
@@ -78,15 +78,15 @@
     :returns: The callable method.
     """
 
     return method if is_regular_method(method) else method.__func__
 # end get_callable_method
 
 def call(
-        c: Method,
+        c: Method, /, *,
         instance: Any,
         args: Tuple,
         kwargs: Dict[str, Any]
 ) -> Any:
     """
     Calls the decorated callable with the overloading match.
 
@@ -98,48 +98,56 @@
     :return: The returned value from the callable call.
     """
 
     if isinstance(c, staticmethod):
         c = c.__func__
 
     elif instance is not None:
+        annotations = None
+
         if isinstance(c, classmethod):
-            # noinspection PyUnresolvedReferences
-            annotations = c.__func__.__annotations__
+            if hasattr(c.__func__, '__annotations__'):
+                annotations = c.__func__.__annotations__
+            # end if
+
             c = partial(c, type(instance))
 
         else:
             annotations = c.__annotations__
             c = partial(c, instance)
         # end if
 
-        c.__annotations__ = annotations
+        if annotations is not None:
+            c.__annotations__ = annotations
+        # end if
     # end if
 
     return statictypes(c)(*args, **kwargs)
 # end call
 
 class Overload:
     """A class to create an overload functionality."""
 
-    def __init__(self, c: Callable) -> None:
+    __slots__ = "instance", "c", "signatures"
+
+    def __init__(self, c: Callable, /) -> None:
         """
         Defines the class attributes.
 
         :param c: The decorated callable object.
         """
 
         self.instance: Optional[Any] = None
 
         self.c = c
 
         self.signatures: Dict[inspect.Signature, Method] = {}
     # end __init__
 
-    def overload(self, c: Callable) -> object:
+    def overload(self, c: Callable, /) -> object:
         """
         sets the signature of the decorated overloading callable object in the class.
 
         :param c: The decorated callable object.
 
         :return: The current class object.
         """
@@ -173,38 +181,38 @@
 
         :return: The returned value from the callable call.
         """
 
         for signature, c in self.signatures.items():
             try:
                 return call(
-                    c=c, instance=self.instance,
+                    c, instance=self.instance,
                     args=args, kwargs=kwargs
                 )
 
             except (RuntimeTypeError, RuntimeTypeWarning, TypeError):
                 pass
             # end try
         # end for
 
         try:
             return call(
-                c=self.c, instance=self.instance,
+                self.c, instance=self.instance,
                 args=args, kwargs=kwargs
             )
 
         except (RuntimeTypeError, TypeError):
             raise OverloadSignatureTypeError(
-                c=self.c, args=args, kwargs=kwargs
+                self.c, args=args, kwargs=kwargs
             )
 
         except RuntimeTypeWarning:
             warnings.warn(
                 overload_signature_error_message(
-                    c=self.c, args=args, kwargs=kwargs
+                    self.c, args=args, kwargs=kwargs
                 ), OverloadSignatureTypeWarning
             )
         # end try
     # end __call__
 # end Overload
 
 overload = Overload
```

### Comparing `pystatic-language-1.1.1/pystatic/private.py` & `pystatic-language-1.1.2/pystatic/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,28 @@
 
     return list(frame.f_locals.values())[0] is obj
 # end in_scope
 
 class PrivateProperty:
     """A descriptor for private attributes."""
 
+    __slots__ = "instance", "value", "name"
+
     def __init__(self, value: Optional[Any] = None) -> None:
         """
         Sets the private value.
 
         :param value: The value to store.
         """
 
         self.instance: Optional[Any] = None
 
         self.value = value
+
+        self.name: Optional[str] = None
     # end __init__
 
     def __set_name__(self, instance: Any, name: str) -> None:
         """
         Sets the name of the attribute in the class.
 
         :param instance: The attribute owner as the class.
```

### Comparing `pystatic-language-1.1.1/pystatic/types.py` & `pystatic-language-1.1.2/pystatic/types.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.1/pystatic_language.egg-info/PKG-INFO` & `pystatic-language-1.1.2/pystatic_language.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.1.1
+Version: 1.1.2
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.1.1/setup.py` & `pystatic-language-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pystatic-language',
-        version='1.1.1',
+        version='1.1.2',
         description=(
             "This package is a collection of methods and classes for "
             "making python more secure, robust, and reliable. "
             "This could be achieved through the simple usage of decorators, "
             "function calls and inheritance of base classes. "
             "Generally, this package can make python a programming language, "
             "closer to other static-typed languages, "
```

### Comparing `pystatic-language-1.1.1/test.py` & `pystatic-language-1.1.2/test.py`

 * *Files identical despite different names*

