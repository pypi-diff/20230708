# Comparing `tmp/asserto-0.1.3.tar.gz` & `tmp/asserto-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asserto-0.1.3.tar", max compression
+gzip compressed data, was "asserto-0.1.4.tar", max compression
```

## Comparing `asserto-0.1.3.tar` & `asserto-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1064 2023-07-02 11:38:03.004915 asserto-0.1.3/LICENSE
--rw-r--r--   0        0        0     3841 2023-07-02 11:38:03.004915 asserto-0.1.3/README.md
--rw-r--r--   0        0        0      303 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/__init__.py
--rw-r--r--   0        0        0     2609 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_api.py
--rw-r--r--   0        0        0    19516 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_asserto.py
--rw-r--r--   0        0        0     1369 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_constants.py
--rw-r--r--   0        0        0      562 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_decorators.py
--rw-r--r--   0        0        0     3182 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_error_handling.py
--rw-r--r--   0        0        0     2714 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_exc_handling.py
--rw-r--r--   0        0        0      923 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_protocols.py
--rw-r--r--   0        0        0     1187 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_softly.py
--rw-r--r--   0        0        0     1281 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_templates.py
--rw-r--r--   0        0        0      295 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_types.py
--rw-r--r--   0        0        0      928 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_util.py
--rw-r--r--   0        0        0      130 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_warnings.py
--rw-r--r--   0        0        0      142 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/__init__.py
--rw-r--r--   0        0        0      561 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/_abc.py
--rw-r--r--   0        0        0      704 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/_validators.py
--rw-r--r--   0        0        0      254 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/__init__.py
--rw-r--r--   0        0        0     2520 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_base.py
--rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_date.py
--rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_files.py
--rw-r--r--   0        0        0     1199 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_handler.py
--rw-r--r--   0        0        0     3544 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_numeric.py
--rw-r--r--   0        0        0     1784 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_regex.py
--rw-r--r--   0        0        0     1094 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_strings.py
--rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/py.typed
--rw-r--r--   0        0        0     1709 2023-07-02 11:38:03.008915 asserto-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 asserto-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-08 20:55:52.532178 asserto-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-08 20:55:52.532178 asserto-0.1.4/README.md
+-rw-r--r--   0        0        0      375 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/__init__.py
+-rw-r--r--   0        0        0     2633 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_api.py
+-rw-r--r--   0        0        0    18125 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_asserto.py
+-rw-r--r--   0        0        0     1507 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_constants.py
+-rw-r--r--   0        0        0     1529 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_decorators.py
+-rw-r--r--   0        0        0     3182 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_error_handling.py
+-rw-r--r--   0        0        0     2714 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_exc_handling.py
+-rw-r--r--   0        0        0      923 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_exceptions.py
+-rw-r--r--   0        0        0      564 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_protocols.py
+-rw-r--r--   0        0        0     1187 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_softly.py
+-rw-r--r--   0        0        0     1281 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_templates.py
+-rw-r--r--   0        0        0      295 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_types.py
+-rw-r--r--   0        0        0     1106 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_util.py
+-rw-r--r--   0        0        0      130 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/_warnings.py
+-rw-r--r--   0        0        0      142 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/descriptors/__init__.py
+-rw-r--r--   0        0        0      561 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/descriptors/_abc.py
+-rw-r--r--   0        0        0      704 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/descriptors/_validators.py
+-rw-r--r--   0        0        0      201 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/__init__.py
+-rw-r--r--   0        0        0     2520 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_base.py
+-rw-r--r--   0        0        0        0 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_date.py
+-rw-r--r--   0        0        0        0 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_files.py
+-rw-r--r--   0        0        0     1199 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_handler.py
+-rw-r--r--   0        0        0     3544 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_numeric.py
+-rw-r--r--   0        0        0     1784 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/handlers/_regex.py
+-rw-r--r--   0        0        0       83 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/mixins/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/mixins/_base.py
+-rw-r--r--   0        0        0     4848 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/mixins/_string_mixin.py
+-rw-r--r--   0        0        0      835 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/mixins/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-08 20:55:52.532178 asserto-0.1.4/asserto/py.typed
+-rw-r--r--   0        0        0     1731 2023-07-08 20:55:52.532178 asserto-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 asserto-0.1.4/PKG-INFO
```

### Comparing `asserto-0.1.3/LICENSE` & `asserto-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/README.md` & `asserto-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_api.py` & `asserto-0.1.4/asserto/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     :param actual: The value to compare against later and defer a type specific asserter from.
     :param warn_unused: Emit a warning if not a single assertion was performed to detect user errors.
     :return: An instance of an asserter
     """
     return Asserto(actual, warn_unused)
 
 
+assert_that = asserto
+
+
 def register_assert(func: types.FunctionType) -> typing.Callable[[typing.Any], typing.Any]:
     """
     # Todo: There is a lot of edge cases here that I'm not (yet) aware of.
     Automatically registers a user defined callable (function) to all future instances of Asserto.
     This is done magically using setattr and the functions must be imported before instantiating
     instances of Asserto to benefit from them,  store your custom assertion functions somewhere
     loaded early in your code and bind them before instantiating `Asserto` instances.
```

### Comparing `asserto-0.1.3/asserto/_asserto.py` & `asserto-0.1.4/asserto/_asserto.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,55 +15,51 @@
 from ._types import RE_PATTERN_ALIAS
 from ._util import is_namedtuple_like
 from ._warnings import NoAssertAttemptedWarning
 from .handlers import BaseHandler
 from .handlers import Handler
 from .handlers import NumberHandler
 from .handlers import RegexHandler
-from .handlers import StringHandler
+from .mixins import AssertsStringsMixin
 
 # Todo: base: `tidy up docstrings`
 # Todo: base `remove duplication here`
 # Todo: Api feels cumbersome with decorators; can we improve DRY-ness?
 # Todo: Consider short hand methods; are they worth it vs a single API?
 
 
-class Asserto:
+class Asserto(AssertsStringsMixin):
     """
     The entrypoint into asserting objects.
 
     :param actual: ...
     :param warn_unused: ...
     """
 
     def __init__(
         self,
         actual: typing.Any,
         warn_unused: bool = False,
         error_handler: typing.Type[RaisesErrors] = ErrorHandler,
     ):
-        self.actual = actual
+        self._actual = actual
         self._triggered = False
         self.warn_unused = warn_unused
         self._in_context = False
         self._error_handler = error_handler()
         self.category: typing.Optional[str] = None
         self.description: typing.Optional[str] = None
 
-    def reassign(self, actual: typing.Any) -> Asserto:
-        """Binds the actual value to the given asserto instances actual value.  This is purposefully not
-        added as a property or promoted via simply attr assignment as it should be seldom used as is an
-        experimental API for now.
-
-        :param actual: The new actual value for underlying assertions.
-
-        ** EXPERIMENTAL: Subject to change **
-        """
-        self.actual = actual
-        return self
+    @property
+    def actual(self) -> typing.Any:
+        return self._actual
+
+    @actual.setter
+    def actual(self, value: typing.Any) -> None:
+        self._actual = value
 
     def error(self, cause: typing.Union[AssertionError, str]) -> Asserto:
         """
         The single point of assertion failing.  All functions delegate here to raise the underlying
         assertion errors.
         :param cause: A reason for the failure. if description was set; it takes precedence.
         :return: The `Asserto` instance for fluency
@@ -103,41 +99,14 @@
         :param match: An optional message to enforce against when the function is called later.
         :return: The `Asserto` instance for fluency
         """
         return ExceptionChecker(exc_types=exceptions, value=self.actual, _referent=self, match=match)
 
     # Todo: should_not_raise
 
-    def ends_with(self, suffix: str) -> Asserto:
-        """
-        Asserts that the actual value ends with suffix.
-
-        :param suffix: The suffix to compare the tail of the string against.
-        """
-        return self._dispatch(
-            StringHandler,
-            Methods.ENDS_WITH,
-            suffix,
-        )
-
-    def starts_with(self, prefix: str) -> Asserto:
-        """
-        Asserts that the actual value ends with prefix.
-
-        :param prefix: The prefix to compare the head of the string against.
-        """
-        return self._dispatch(StringHandler, Methods.STARTS_WITH, prefix)
-
-    def is_digit(self) -> Asserto:
-        """
-        Asserts that the actual value contains only unicode letters and that the string has
-        at least a single character.
-        """
-        return self._dispatch(StringHandler, Methods.IS_DIGIT)
-
     def is_between(self, low: float, high: float, inclusive: bool = False):
         """
         Asserts that the actual value is between a low and high bounds.  If inclusive is true
         the actual value is considered between if it is equal to either of those bounds.
         """
         return self._dispatch(NumberHandler, Methods.IS_BETWEEN, low, high, inclusive)
 
@@ -162,21 +131,14 @@
         Asserts that the actual value is not between the low and high bounds.  if the actual value
         is equal to the low or high bounds it is considered to be between them
         """
         return self.is_not_between(low, high, inclusive=True)
 
     is_not_between_incl = is_not_between_inclusive
 
-    def is_alpha(self) -> Asserto:
-        """
-        Asserts that the actual value contains only unicode letters and that the string has
-        at least a single character.
-        """
-        return self._dispatch(StringHandler, Methods.IS_ALPHA)
-
     def match(self, pattern: RE_PATTERN_ALIAS, flags: RE_FLAGS_ALIAS = 0) -> Asserto:
         """
         Asserts that the actual value provided matches (at least in part) from the beginning of it
         the pattern provided.  This is only a 'begins with' partial match.  Opt for `fullmatch` to
         perform a pattern match on the entirety of the actual value.
 
         :param pattern: The regular expression pattern to use; r"" is encouraged.
```

### Comparing `asserto-0.1.3/asserto/_constants.py` & `asserto-0.1.4/asserto/_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,7 +42,11 @@
     # -- Numeric
     IS_ZERO: str = "is_zero"
     IS_NOT_ZERO: str = "is_not_zero"
     IS_GREATER_THAN: str = "is_greater_than"
     IS_LESSER_THAN: str = "is_lesser_than"
     IS_POSITIVE: str = "is_positive"
     IS_NEGATIVE: str = "is_negative"
+
+
+class MixinErrorTemplates:
+    ASSERTO_TYPE_ERROR = "value passed to asserto({0}) must be of type {1} when calling {2} but it was {3}."
```

### Comparing `asserto-0.1.3/asserto/_error_handling.py` & `asserto-0.1.4/asserto/_error_handling.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_exc_handling.py` & `asserto-0.1.4/asserto/_exc_handling.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_exceptions.py` & `asserto-0.1.4/asserto/_exceptions.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_softly.py` & `asserto-0.1.4/asserto/_softly.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_templates.py` & `asserto-0.1.4/asserto/_templates.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/_util.py` & `asserto-0.1.4/asserto/_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import typing
 
 T = typing.TypeVar("T")
 
 
+def is_iterable(item: typing.Any) -> bool:
+    """Checks if an item is an iterable in a python 3 compliant manner.  This encompasses both
+    new iterator protocol aswell as older protocol via __getitem__ etc."""
+    try:
+        iter(item)
+        return True
+    except TypeError:
+        return False
+
+
 def to_iterable(item: typing.Any) -> typing.Tuple[T, ...]:
     """
     Converts a tuple from any items that can be iterated over.
     :param item: Anything, if iterable is concerted to tuple otherwise is a single element tuple of T.
     :return: A tuple of items
     """
     try:
@@ -25,12 +35,7 @@
     bases = t.__bases__
     if len(bases) != 1 and bases[0] != tuple:
         return False
     fields = getattr(obj, "_fields", None)
     if not isinstance(fields, tuple):
         return False
     return all(type(f) == str for f in fields)
-
-
-def object_to_name(obj: typing.Any) -> str:
-    """Returns the class name of any object."""
-    return obj.__class__.__name__
```

### Comparing `asserto-0.1.3/asserto/descriptors/_abc.py` & `asserto-0.1.4/asserto/descriptors/_abc.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/descriptors/_validators.py` & `asserto-0.1.4/asserto/descriptors/_validators.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/handlers/_base.py` & `asserto-0.1.4/asserto/handlers/_base.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/handlers/_handler.py` & `asserto-0.1.4/asserto/handlers/_handler.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/handlers/_numeric.py` & `asserto-0.1.4/asserto/handlers/_numeric.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/asserto/handlers/_regex.py` & `asserto-0.1.4/asserto/handlers/_regex.py`

 * *Files identical despite different names*

### Comparing `asserto-0.1.3/pyproject.toml` & `asserto-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,40 @@
 version = "21.9.0"
 name = "asserto"
 underlines = "=-~"
 all_bullets = true
 
 [tool.poetry]
 name = "asserto"
-version = "0.1.3"
+version = "0.1.4"
 description = "A fluent DSL for python assertions."
 authors = ["symonk <jackofspaces@gmail.com>"]
 readme = "README.md"
 include = ["asserto/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.3.4"
 
 [tool.poetry.dev-dependencies]
-codecov = "^2.1.12"
-pre-commit = "^2.20.0"
-mkdocs = "^1.4.0"
-mkdocs-material = "^9"
-mkdocstrings= {extras = ["python"], version = "^0.19.0"}
+codecov = "^2"
+pre-commit = "^3"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocstrings= "^0.22.0"
+mkdocstrings-python = "^1.1.2"
 pytest = "^7"
 tox = "^4"
 pip = "^22"
 coverage = "^7"
-towncrier = "^22"
+towncrier = "^23"
 
 [tool.poetry.group.dev.dependencies]
 pytest-xdist = "^3.3.1"
+typing-extensions = "^4.7.1"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:RequestsDependencyWarning:"
 ]
 
 [tool.isort]
```

### Comparing `asserto-0.1.3/PKG-INFO` & `asserto-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asserto
-Version: 0.1.3
+Version: 0.1.4
 Summary: A fluent DSL for python assertions.
 Author: symonk
 Author-email: jackofspaces@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

