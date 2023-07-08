# Comparing `tmp/scrape_schema-0.3.0.tar.gz` & `tmp/scrape_schema-0.3.2.tar.gz`

## Comparing `scrape_schema-0.3.0.tar` & `scrape_schema-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/_logger.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/_typing.py
--rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/base.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/field.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/nested.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/type_caster.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/LICENSE
--rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/README.md
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/_logger.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    16576 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/base.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/field.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/field_protocols.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/LICENSE
+-rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/README.md
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/PKG-INFO
```

### Comparing `scrape_schema-0.3.0/scrape_schema/_typing.py` & `scrape_schema-0.3.2/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/scrape_schema/base.py` & `scrape_schema-0.3.2/scrape_schema/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,40 @@
     Optional,
     Pattern,
     Tuple,
     Type,
     Union,
 )
 
+import chompjs
 from parsel import Selector
+
 from scrape_schema._logger import _logger
 from scrape_schema._typing import (
     Annotated,
     NoneType,
     Self,
     get_args,
     get_origin,
     get_type_hints,
 )
+from scrape_schema.field_protocols import SpecialMethodsProtocol
 from scrape_schema.type_caster import TypeCaster
 
 
 class SpecialMethods(Enum):
     # special methods for another methods
     FN = 0
     CONCAT_L = 1
     CONCAT_R = 2
     REPLACE = 3
     REGEX_SEARCH = 4
     REGEX_FINDALL = 5
+    CHOMP_JS_PARSE = 6
+    CHOMP_JS_PARSE_ALL = 7
 
 
 class MarkupMethod(NamedTuple):
     METHOD_NAME: Union[str, SpecialMethods]
     args: Tuple[Any, ...] = ()
     kwargs: Dict[str, Any] = {}
 
@@ -126,14 +131,20 @@
                 if not pattern.groupindex:
                     raise TypeError(
                         f"Pattern `{pattern.pattern}` is not contains groups"
                     )
                 return [match.groupdict() for match in pattern.finditer(markup)]
             return pattern.findall(markup)
 
+        elif method.METHOD_NAME == SpecialMethods.CHOMP_JS_PARSE:
+            return chompjs.parse_js_object(markup, *method.args)
+
+        elif method.METHOD_NAME == SpecialMethods.CHOMP_JS_PARSE_ALL:
+            return chompjs.parse_js_objects(markup, *method.args)
+
         raise TypeError("Unknown special method")
 
     @staticmethod
     def _accept_method(markup: Any, method: MarkupMethod) -> Any:
         if isinstance(method.METHOD_NAME, str):
             class_method = getattr(markup, method.METHOD_NAME)
             if isinstance(class_method, (property, dict)):  # attrib check
@@ -170,63 +181,101 @@
 
     def sc_parse(self, markup: Any) -> Any:
         markup = self._prepare_markup(markup)
         return self._call_stack_methods(markup)
 
     # build in methods
 
-    def fn(self, function: Callable[..., Any]) -> Self:
+    def fn(self, function: Callable[..., Any]) -> SpecialMethodsProtocol:
         """call another function and return result"""
-        return self.add_method(SpecialMethods.FN, function=function)
+        return self.add_method(SpecialMethods.FN, function=function)  # type: ignore
 
-    def concat_l(self, left_string: str) -> Self:
+    def concat_l(self, left_string: str) -> SpecialMethodsProtocol:
         """add string to left. Last argument should be string"""
-        return self.add_method(SpecialMethods.CONCAT_L, left_string)
+        return self.add_method(SpecialMethods.CONCAT_L, left_string)  # type: ignore
 
-    def concat_r(self, right_string: str) -> Self:
+    def concat_r(self, right_string: str) -> SpecialMethodsProtocol:
         """add string to right. Last argument should be string"""
-        return self.add_method(SpecialMethods.CONCAT_R, right_string)
+        return self.add_method(SpecialMethods.CONCAT_R, right_string)  # type: ignore
 
-    def sc_replace(self, old: str, new: str, count: int = -1) -> Self:
+    def sc_replace(self, old: str, new: str, count: int = -1) -> SpecialMethodsProtocol:
         """replace string method. Last argument should be string"""
-        return self.add_method(SpecialMethods.REPLACE, old, new, count)
+        return self.add_method(SpecialMethods.REPLACE, old, new, count)  # type: ignore
 
     def re_search(
         self,
         pattern: Union[str, Pattern[str]],
         flags: Union[int, RegexFlag] = 0,
         groupdict: bool = False,
-    ) -> Self:
+    ) -> SpecialMethodsProtocol:
         """re.search method for text result.
 
         Last chain should be return string.
 
         :param pattern: regex pattern
         :param flags: compilation flags
         :param groupdict: accept groupdict method. patter required named groups. default False
         """
         pattern = re.compile(pattern, flags=flags)
-        return self.add_method(SpecialMethods.REGEX_SEARCH, pattern, groupdict)
+        return self.add_method(SpecialMethods.REGEX_SEARCH, pattern, groupdict)  # type: ignore
 
     def re_findall(
         self,
         pattern: Union[str, Pattern[str]],
         flags: Union[int, RegexFlag] = 0,
         groupdict: bool = False,
-    ):
+    ) -> SpecialMethodsProtocol:
         """[match for match in re.finditer(...)] method for text result.
 
         Last chain should be return string.
 
         :param pattern: regex pattern
         :param flags: compilation flags
         :param groupdict: accept groupdict method. patter required named groups. default False
         """
         pattern = re.compile(pattern, flags=flags)
-        return self.add_method(SpecialMethods.REGEX_FINDALL, pattern, groupdict)
+        return self.add_method(SpecialMethods.REGEX_FINDALL, pattern, groupdict)  # type: ignore
+
+    def chomp_js_parse(
+        self, unicode_escape: Any = False, json_params: Any = None
+    ) -> SpecialMethodsProtocol:
+        """Extracts first JSON object encountered in the input string
+
+        Params:
+            string – Input string
+            unicode_escape – Attempt to fix input string if it contains escaped special characters
+            json_params – Allow passing down standard json.loads options
+
+        Returns:
+            Extracted JSON object
+        """
+        return self.add_method(
+            SpecialMethods.CHOMP_JS_PARSE, unicode_escape, json_params
+        )
+
+    def chomp_js_parse_all(
+        self,
+        unicode_escape: Any = False,
+        omitempty: Any = False,
+        json_params: Any = None,
+    ) -> SpecialMethodsProtocol:
+        """Returns a list extracting all JSON objects encountered in the input string. Can be used to read JSON Lines
+
+        Params:
+            string – Input string
+            unicode_escape – Attempt to fix input string if it contains escaped special characters
+            omitempty – Skip empty dictionaries and lists
+            json_params – Allow passing down standard json.loads flags
+
+        Returns:
+            Iterating over it yields all encountered JSON objects
+        """
+        return self.add_method(
+            SpecialMethods.CHOMP_JS_PARSE_ALL, unicode_escape, omitempty, json_params
+        )
 
     def add_method(
         self, method_name: Union[str, SpecialMethods], *args, **kwargs
     ) -> Self:
         """low-level interface adding methods to call stack"""
         self._stack_methods.append(MarkupMethod(method_name, args=args, kwargs=kwargs))
         return self
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrape_schema-0.3.0/scrape_schema/field.py` & `scrape_schema-0.3.2/scrape_schema/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-from typing import Any, Hashable, Mapping, Optional, Pattern, Union, overload
+from typing import Any, Hashable, Mapping, Optional, Pattern, Union
 
 from parsel import Selector
+
 from scrape_schema._logger import _logger
 from scrape_schema._typing import Self
 from scrape_schema.base import Field, FieldConfig
+from scrape_schema.field_protocols import AttribProtocol, SpecialMethodsProtocol
 
 
 class Parsel(Field):
     class Config(FieldConfig):
         instance = Selector
 
     def __init__(
         self, auto_type: bool = True, default: Any = ..., *, raw: bool = False
     ):
         super().__init__(auto_type=auto_type, default=default)
         if raw:
             self.xpath("//p/text()").get()
 
-    def css(self, query: str):
+    def css(self, query: str) -> Self:
         """Apply the given CSS selector and return a SelectorList instance.
 
         query is a string containing the CSS selector to apply.
 
         In the background, CSS queries are translated into XPath queries using cssselect  library and run .xpath() method.
         """
         return self.add_method("css", query)
 
     @property
-    def raw_text(self):
+    def raw_text(self) -> SpecialMethodsProtocol:
         """Shortcut `Parsel().xpath('//p/text()')` call.
 
         This method for getting raw text (not html), when calling `parsel.Selector` methods will raise an error
         """
         # Parsel is not meant for raw text: it will try to "fix" html and parse as html usage `raw_text` property
         # or `xpath(//p/text()).get()` or raw=True in init constructor
         return self.xpath("//p/text()").get()
 
     def xpath(
         self, query: str, namespaces: Optional[Mapping[str, str]] = None, **kwargs: Any
-    ):
+    ) -> Self:
         """
         Find nodes matching the xpath ``query`` and return the result as a
         :class:`SelectorList` instance with all elements flattened. List
         elements implement :class:`Selector` interface too.
 
         ``query`` is a string containing the XPATH query to apply.
 
@@ -55,54 +57,58 @@
         variables in the XPath expression, e.g.::
 
             selector.xpath('//a[href=$url]', url="http://www.example.com")
         """
 
         return self.add_method("xpath", query, namespaces, **kwargs)
 
-    def re(self, regex: Union[str, Pattern[str]], replace_entities: bool = True):
+    def re(
+        self, regex: Union[str, Pattern[str]], replace_entities: bool = True
+    ) -> SpecialMethodsProtocol:
         """
         Apply the given regex and return a list of strings with the
         matches.
 
         ``regex`` can be either a compiled regular expression or a string which
         will be compiled to a regular expression using ``re.compile(regex)``.
 
         By default, character entity references are replaced by their
         corresponding character (except for ``&amp;`` and ``&lt;``).
         Passing ``replace_entities`` as ``False`` switches off these
         replacements.
         """
-        return self.add_method("re", regex=regex, replace_entities=replace_entities)
+        return self.add_method("re", regex=regex, replace_entities=replace_entities)  # type: ignore
 
     def _is_attrib(self):
         if (method := self._stack_methods[-1].METHOD_NAME) != "attrib":
             _logger.error("Last method should be `attrib, not %s", method)
             raise TypeError(f"Last method should be `attrib`, not `{method}`")
         return True
 
-    def get(self, default: Optional[str] = None, key: Optional[Hashable] = None) -> Self:  # type: ignore
+    def get(
+        self, default: Optional[str] = None, key: Optional[Hashable] = None
+    ) -> SpecialMethodsProtocol:  # type: ignore
         """
         Serialize and return the matched nodes in a single string. Percent encoded content is unquoted.
 
         If `key` param passed - get value from attrib property. attrib should be called in chain methods
         """
         if key and default:
             _logger.error(
                 "get should be accept `key` OR `default` param, not `key` AND `default`"
             )
             raise TypeError(
                 "get should be accept `key` OR `default` param, not `key` AND `default`"
             )
         elif key:
             if self._is_attrib():
-                return self.add_method("get", key)
-        return self.add_method("get", default)
+                return self.add_method("get", key)  # type: ignore
+        return self.add_method("get", default)  # type: ignore
 
-    def jmespath(self, query: str, **kwargs: Any):
+    def jmespath(self, query: str, **kwargs: Any) -> Self:
         """
         Find objects matching the JMESPath ``query`` and return the result as a
         :class:`SelectorList` instance with all elements flattened. List
         elements implement :class:`Selector` interface too.
 
         ``query`` is a string containing the `JMESPath
         <https://jmespath.org/>`_ query to apply.
@@ -110,28 +116,28 @@
         Any additional named arguments are passed to the underlying
         ``jmespath.search`` call, e.g.::
 
             selector.jmespath('author.name', options=jmespath.Options(dict_cls=collections.OrderedDict))
         """
         return self.add_method("jmespath", query, **kwargs)
 
-    def getall(self):
+    def getall(self) -> SpecialMethodsProtocol:
         """Call the .get() method for each element is this list
         and return their results flattened, as a list of strings."""
 
-        return self.add_method("getall")
+        return self.add_method("getall")  # type: ignore
 
     @property
-    def attrib(self):
+    def attrib(self) -> AttribProtocol:
         """
         Return the attributes dictionary for the first element.
 
         If the list is empty, return an empty dict.
         """
-        return self.add_method("attrib")
+        return self.add_method("attrib")  # type: ignore
 
     def keys(self):
         if self._is_attrib():
             return self.add_method("keys")
 
     def values(self):
         if self._is_attrib():
```

### Comparing `scrape_schema-0.3.0/scrape_schema/nested.py` & `scrape_schema-0.3.2/scrape_schema/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/scrape_schema/type_caster.py` & `scrape_schema-0.3.2/scrape_schema/type_caster.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/.gitignore` & `scrape_schema-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/LICENSE` & `scrape_schema-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/README.md` & `scrape_schema-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.0/pyproject.toml` & `scrape_schema-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   "Topic :: Internet",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing"
 ]
 dependencies = [
   'colorlog',
   'parsel',
+  'chompjs',
   'typing_extensions; python_version < "3.11"'
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/vypivshiy/scrape-schema#readme"
 Issues = "https://github.com/vypivshiy/scrape-schema/issues"
```

### Comparing `scrape_schema-0.3.0/PKG-INFO` & `scrape_schema-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.0
+Version: 0.3.2
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
+Requires-Dist: chompjs
 Requires-Dist: colorlog
 Requires-Dist: parsel
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: ci
 Requires-Dist: black; extra == 'ci'
 Requires-Dist: bs4; extra == 'ci'
 Requires-Dist: flake8; extra == 'ci'
```

