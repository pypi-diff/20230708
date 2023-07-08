# Comparing `tmp/typefit-0.4.2.tar.gz` & `tmp/typefit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typefit-0.4.2.tar", max compression
+gzip compressed data, was "typefit-0.5.1.tar", max compression
```

## Comparing `typefit-0.4.2.tar` & `typefit-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      484 2019-10-21 12:47:40.000000 typefit-0.4.2/LICENSE
--rw-r--r--   0        0        0     1539 2019-10-28 09:37:07.000000 typefit-0.4.2/README.md
--rw-r--r--   0        0        0      744 2022-06-21 10:16:46.665943 typefit-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      198 2020-04-30 13:15:54.000000 typefit-0.4.2/src/typefit/__init__.py
--rw-r--r--   0        0        0    15459 2022-06-21 10:14:12.963411 typefit-0.4.2/src/typefit/api.py
--rw-r--r--   0        0        0     1966 2021-06-06 10:38:07.721692 typefit-0.4.2/src/typefit/compat.py
--rw-r--r--   0        0        0     7084 2020-04-30 13:15:54.000000 typefit-0.4.2/src/typefit/fitting.py
--rw-r--r--   0        0        0      453 2021-06-06 10:52:32.707988 typefit-0.4.2/src/typefit/httpx_models.py
--rw-r--r--   0        0        0     1644 2020-04-08 20:09:52.000000 typefit-0.4.2/src/typefit/meta.py
--rw-r--r--   0        0        0     1204 2020-04-08 14:07:42.000000 typefit-0.4.2/src/typefit/narrows.py
--rw-r--r--   0        0        0    14855 2021-06-06 10:52:32.707988 typefit-0.4.2/src/typefit/nodes.py
--rw-r--r--   0        0        0     9722 2021-06-06 10:52:32.707988 typefit-0.4.2/src/typefit/reporting.py
--rw-r--r--   0        0        0     7517 2020-04-30 13:15:54.000000 typefit-0.4.2/src/typefit/serialize.py
--rw-r--r--   0        0        0     2895 2020-04-30 13:15:54.000000 typefit-0.4.2/src/typefit/utils.py
--rw-r--r--   0        0        0     2358 2022-06-21 10:17:08.512731 typefit-0.4.2/setup.py
--rw-r--r--   0        0        0     2330 2022-06-21 10:17:08.513149 typefit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-08 16:45:32.055478 typefit-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1477 2023-07-08 16:45:32.055478 typefit-0.5.1/README.md
+-rw-r--r--   0        0        0     1351 2023-07-08 16:45:32.059479 typefit-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/__init__.py
+-rw-r--r--   0        0        0    15459 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/api.py
+-rw-r--r--   0        0        0     2008 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/compat.py
+-rw-r--r--   0        0        0     8895 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/fitting.py
+-rw-r--r--   0        0        0      453 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/httpx_models.py
+-rw-r--r--   0        0        0     2428 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/meta.py
+-rw-r--r--   0        0        0     1204 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/narrows.py
+-rw-r--r--   0        0        0    23219 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/nodes.py
+-rw-r--r--   0        0        0     9722 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/reporting.py
+-rw-r--r--   0        0        0     7517 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/serialize.py
+-rw-r--r--   0        0        0     2895 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/utils.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.1/PKG-INFO
```

### Comparing `typefit-0.4.2/README.md` & `typefit-0.5.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # TypeFit
 
 [![Read the Docs](https://img.shields.io/readthedocs/typefit)](http://typefit.rtfd.io/)
-[![Build Status](https://img.shields.io/travis/Xowap/typefit)](https://travis-ci.org/Xowap/typefit)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/Xowap/typefit)](https://lgtm.com/projects/g/Xowap/typefit/)
+[![Build Status](https://github.com/Xowap/typefit/actions/workflows/run-tests.yaml/badge.svg)](https://github.com/Xowap/typefit/actions/workflows/run-tests.yaml)
 
 Typing annotations make Python awesome, however it's complicated to keep your
 data annotated when it comes from external sources like APIs. The goal of
 Typefit is to help you map that external data into type-annotated native Python
 objects.
 
 ```python
@@ -32,15 +31,14 @@
 ```
 
 This is the full example of a Hacker News API client. Its functionality is
 limited but in 14 lines counting white space you can build a type-safe client
 for Hacker News. You'll find a [full example](example/typefit_hn) attached if
 you're interested.
 
-
 ## Documentation
 
 [✨ **Documentation is there** ✨](http://typefit.rtfd.io/)
 
 ## Licence
 
 This library is provided under the terms of the [WTFPL](./LICENSE).
```

### Comparing `typefit-0.4.2/src/typefit/api.py` & `typefit-0.5.1/src/typefit/api.py`

 * *Files identical despite different names*

### Comparing `typefit-0.4.2/src/typefit/compat.py` & `typefit-0.5.1/src/typefit/compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,24 @@
 from typing import Any, Generic, Tuple, _GenericAlias
 
 try:
     from typing import get_origin
 except ImportError:
 
     def get_origin(tp) -> Any:
-        """Get the unsubscripted version of a type.
+        """
+        Get the unsubscripted version of a type.
 
-        This supports generic types, Callable, Tuple, Union, Literal, Final and ClassVar.
-        Return None for unsupported types. Examples::
+        This supports generic types, Callable, Tuple, Union, Literal, Final and
+        ClassVar.
+
+        Return None for unsupported types.
+
+        Examples
+        --------
 
             get_origin(Literal[42]) is Literal
             get_origin(int) is None
             get_origin(ClassVar[int]) is ClassVar
             get_origin(Generic) is Generic
             get_origin(Generic[T]) is Generic
             get_origin(Union[T, int]) is Union
```

### Comparing `typefit-0.4.2/src/typefit/fitting.py` & `typefit-0.5.1/src/typefit/fitting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import abc
 from enum import Enum
 from inspect import isclass
-from typing import Any, Optional, Type, Union
+from typing import Any, Callable, Mapping, MutableSequence, Optional, Type, Union
 
 from .compat import get_args, get_origin
 from .nodes import *
 from .reporting import ErrorReporter, LogErrorReporter, PrettyJson5Formatter
 
 
 class Fitter:
@@ -22,31 +22,38 @@
     order and also holds configuration.
     """
 
     def __init__(
         self,
         no_unwanted_keys: bool = False,
         error_reporter: Optional[ErrorReporter] = None,
+        context: Optional[Mapping[str, Any]] = None,
     ):
         """
         Constructs the instance.
 
         Parameters
         ----------
         no_unwanted_keys
             If set to ``True``, it will not be allowed to have unwanted keys
             when fitting mappings into dataclasses/named tuples.
         error_reporter
             Error reporting for when a validation fails. By default no report
             is made but you might want to arrange reporting for your needs,
             otherwise you're going to be debugging in the blind.
+        context
+            Custom context whose values can be injected into fitted object
+            through the use if :py:func:`typefit.meta.meta`'s `context`
+            argument.
         """
 
         self.no_unwanted_keys = no_unwanted_keys
         self.error_reporter = error_reporter
+        self.context = context or {}
+        self.root_injectors: MutableSequence[Callable[[Any], None]] = []
 
     def _as_node(self, value: Any):
         """
         Recursively transforms a value into a node.
 
         Parameters
         ----------
@@ -56,15 +63,18 @@
 
         if isinstance(value, (int, float, str, bool)) or value is None:
             return FlatNode(self, value)
         elif isinstance(value, abc.Sequence):
             return ListNode(self, value, [self._as_node(x) for x in value])
         elif isinstance(value, abc.Mapping):
             return MappingNode(
-                self, value, {k: self._as_node(v) for k, v in value.items()}
+                self,
+                value,
+                {k: self._as_node(v) for k, v in value.items()},
+                context=self.context,
             )
         else:
             raise ValueError
 
     def _fit_union(self, t: Type[T], value: Node) -> T:
         """
         In case of a union, walk through all possible types and try them on
@@ -80,15 +90,15 @@
         value.fail("No matching type in Union")
 
     def _fit_class(self, t: Type[T], value: Node) -> T:
         """
         Wrapper around the ``FlatNode``'s fit method.
         """
 
-        if isinstance(value, FlatNode):
+        if isinstance(value, (FlatNode, LiteralNode)):
             return value.fit(t)
 
         value.fail(f"Node is not {t}")
 
     def _fit_any(self, _: Type[T], value: Node) -> T:
         """
         That's here for consistency but let's be honest, this function is not
@@ -102,15 +112,15 @@
         Does basic checks before returning None or raising an error
         """
 
         if value.value is None:
             value.fit_success = True
             return None
 
-        value.fail(f"Value is not None")
+        value.fail("Value is not None")
 
     def _fit_enum(self, t: Type[T], value: Node) -> T:
         """
         Tries to find back the right enum value
         """
 
         try:
@@ -164,14 +174,32 @@
         """
         Fits data into a type. The data is expected to be JSON-decoded values
         (strings, ints, bools, etc).
 
         On failure a ValueError will arise and if an error reporter is set it
         will be sent the node to generate the error report.
 
+        Notes
+        -----
+        You'll notice down there some "root_injector" business and might wonder
+        what the fuck is this. We have a feature that allows to inject the
+        "root" object (aka the one that we're about to return) into marked
+        fields down the line. However all the child objects are built before
+        the root is built itself. As a result, all those fields are initially
+        filled up by "None" and then when we finally have our root object
+        constructed we go back into each of those objects to set correct
+        values.
+
+        In order to do this in an orthogonal way, each node has the possibility
+        every time they encounter a place to inject a root field to add a
+        callable (which is obviously gonna be a 2nd-order function) into the
+        `root_injectors` attribute of this class. Meaning that at this point
+        all we got to do is to call all the root injectors (no need to recurse
+        into anything, yay).
+
         Parameters
         ----------
         t
             Type you want to fit the value into
         value
             Value you want to fit into a type
 
@@ -179,22 +207,27 @@
         -------
         ValueError
         """
 
         node = self._as_node(value)
 
         try:
-            return self.fit_node(t, node)
+            out = self.fit_node(t, node)
         except ValueError:
             if self.error_reporter:
                 self.error_reporter.report(node)
             raise
+        else:
+            for injector in self.root_injectors:
+                injector(out)
+
+            return out
 
 
-def typefit(t: Type[T], value: Any) -> T:
+def typefit(t: Type[T], value: Any, context: Optional[Mapping[str, Any]] = None) -> T:
     """
     Fits a JSON-decoded value into native Python type-annotated objects.
 
     This uses the default sane settings but it might not be up to your taste.
     By example, errors will be reported in the logging module using ANSI escape
     codes for syntactical coloration, however depending on the situation you
     might not want that.
@@ -212,14 +245,17 @@
           - Enumerations which are subclass of :class:`enum.Enum`.
           - Custom types. The constructor needs to accept exactly one parameter
             and that parameter should have a typing annotation.
           - :class:`typing.Union` to define several possible types
           - :class:`typing.List` to declare a list and the type of list values
     value
         Value to be fit into the type
+    context
+        Custom context whose values can be injected into fitted object through
+        the use if :py:func:`typefit.meta.meta`'s `context` argument.
 
     Returns
     -------
     T
         If the value fits, a value of the right type is returned.
 
     Raises
@@ -231,9 +267,10 @@
     --------
     Fitter.fit
     """
 
     return Fitter(
         error_reporter=LogErrorReporter(
             formatter=PrettyJson5Formatter(colors="terminal16m")
-        )
+        ),
+        context=context,
     ).fit(t, value)
```

### Comparing `typefit-0.4.2/src/typefit/narrows.py` & `typefit-0.5.1/src/typefit/narrows.py`

 * *Files identical despite different names*

### Comparing `typefit-0.4.2/src/typefit/nodes.py` & `typefit-0.5.1/src/typefit/nodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 from dataclasses import dataclass, field, fields, is_dataclass
-from inspect import Parameter, isclass, signature
+from inspect import Parameter, Signature, isclass, signature
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Dict,
+    Iterable,
     List,
+    Mapping,
+    MutableSequence,
     Optional,
+    Sequence,
     Set,
     Text,
+    Tuple,
     Type,
     TypeVar,
     get_type_hints,
 )
 
 from .compat import get_args, get_origin
-from .meta import Source
 from .utils import OrderedSet, format_type_name, is_named_tuple
 
 if TYPE_CHECKING:
     from .fitting import Fitter
 
 
-__all__ = ["T", "Node", "MappingNode", "ListNode", "FlatNode"]
+__all__ = ["T", "Node", "MappingNode", "ListNode", "FlatNode", "LiteralNode"]
 
 
 T = TypeVar("T")
 
 
+def set_root_attr(obj: Any, attr: str):
+    """
+    2nd-order function to set the root object into `obj`'s attribute `attr`.
+    See :py:meth:`typefit.fitting.Fitter.fit` for more information.
+
+    See Also
+    --------
+    typefit.fitting.Fitter.fit
+    """
+
+    def do_it(value: Any):
+        object.__setattr__(obj, attr, value)
+
+    return do_it
+
+
 @dataclass
 class Node:
     """
     Typefit is made to convert JSON structure into Python dataclasses and
     objects. In order to make analyzing a fitting possible after it failed,
     data structures will be converted into a tree of Nodes. This is the base
     class, but there is 3 kinds of nodes:
@@ -121,14 +142,15 @@
         Does the rejection come from the kids? Or is it due to this node only?
     """
 
     children: Dict[Text, Node] = field(repr=False)
     missing_keys: List[Text] = field(default_factory=list, repr=False)
     unwanted_keys: List[Text] = field(default_factory=list, repr=False)
     problem_is_kids: bool = field(default=False, repr=False)
+    context: Mapping[str, Any] = field(default_factory=dict, repr=False)
 
     def fit_dict(self, t: Type[T]) -> T:
         """
         Fitting a JSON object into a Python dictionary. That's basically just
         a copy with a few sanity checks (and typefitting on the values).
 
         Notes
@@ -183,14 +205,28 @@
         if failed[0]:
             self.problem_is_kids = True
             self.fail("Not all items are fit")
 
         self.fit_success = True
         return out
 
+    def value_from_context(self, key: str) -> Callable[[], Any]:
+        """
+        Encapsulates the logic that we're gonna give to the LiteralNode
+        when doing context injection
+        """
+
+        def get_value() -> Any:
+            try:
+                return self.context[key]
+            except KeyError as e:
+                raise ValueError(f"Key {key!r} is missing from the context") from e
+
+        return get_value
+
     def fit_object(self, t: Type[T]) -> T:
         """
         Fitting into dataclasses and named tuples. On paper that's fairly
         simple, but if you want something safe with good error reporting it's
         a little bit more complicated.
 
         Notes
@@ -223,27 +259,123 @@
         t
             Type-annotated named tuple class or dataclass
         """
 
         sig = signature(t)
         hints = get_type_hints(t)
 
-        kwargs = {}
+        fields_injections, fields_sources, root_fields = self.parse_dataclass(t)
+
+        (
+            expected,
+            failed_keys,
+            kwargs,
+            literal_nodes,
+            required,
+        ) = self.make_constructor_kwargs(fields_injections, fields_sources, hints, sig)
+
+        missing = required - set(kwargs) - set(failed_keys)
+        unwanted = set(self.children) - expected
+        errors = []
+
+        self.report_missing(errors, missing)
+        self.report_unwanted(errors, t, unwanted)
+        self.report_failed(errors, failed_keys, fields_injections, literal_nodes)
+
+        if errors:
+            self.problem_is_kids = True
+            self.fail(". ".join([f"Wrong keys set for {format_type_name(t)}", *errors]))
+
+        return self.make_out_instance(kwargs, root_fields, t)
+
+    def parse_dataclass(
+        self, t: Type[T]
+    ) -> Tuple[
+        Mapping[str, Any],
+        Mapping[str, Callable[[Mapping[str, Any]], Any]],
+        Sequence[str],
+    ]:
+        """
+        If the expected type is a dataclass, there might be some metadata on
+        the fields. Which helps for example to source a field from a different
+        field name or to inject context into given fields. We're extracting
+        all this metadata from here (if relevant).
+
+        Parameters
+        ----------
+        t
+            The type of the object that we're instantiating
+        """
+
+        root_fields = []
         fields_sources = {}
+        fields_injections = {}
+
+        if not is_dataclass(t):
+            return fields_injections, fields_sources, root_fields
+
+        for t_field in fields(t):
+            match (t_field.metadata):
+                case {"typefit_source": source}:
+                    fields_sources[t_field.name] = source.value_from_json
+                case {"typefit_from_context": key}:
+                    fields_injections[t_field.name] = self.value_from_context(key)
+                case {"typefit_inject_root": True}:
+                    fields_injections[t_field.name] = None
+                    root_fields.append(t_field.name)
+
+        return fields_injections, fields_sources, root_fields
+
+    def make_constructor_kwargs(
+        self,
+        fields_injections: Mapping[str, Any],
+        fields_sources: Mapping[str, Callable[[Mapping[str, Any]], Any]],
+        hints: Any,
+        sig: Signature,
+    ) -> Tuple[
+        Set[str],
+        Sequence[str],
+        Mapping[str, Any],
+        Mapping[str, "LiteralNode"],
+        Set[str],
+    ]:
+        """
+        We're going through every field of the constructor's signature and we
+        try to fit the corresponding value from the input JSON.
+
+        We only support parameters that can be called by keyword, as this is
+        what we're getting from a mapping type.
+
+        For each field we got three possibilities:
+
+        - The field has some meta mapping (most likely to get its value from
+          another field) in which case we call the mapping function
+        - Or it is subject to some kind of injection (either root or context),
+          which requires to wrap the mapped value into a LiteralNode and to
+          continue the resolution like that
+        - Or finally it's a normal node and we just get its value
+
+        Parameters
+        ----------
+        fields_injections
+            The mapping of keys to the injection functions
+        fields_sources
+            The mapping of keys to the mapping functions
+        hints
+            The type hints of the constructor
+        sig
+            The signature of the constructor
+        """
+
+        literal_nodes: Dict[str, LiteralNode] = {}
+        kwargs = {}
         required = set()
         expected = set()
         failed_keys = []
 
-        if is_dataclass(t):
-            # noinspection PyDataclass
-            for t_field in fields(t):
-                if t_field.metadata and "typefit_source" in t_field.metadata:
-                    source: Source = t_field.metadata["typefit_source"]
-                    fields_sources[t_field.name] = source.value_from_json
-
         param: Parameter
         for param in sig.parameters.values():
             if param.kind not in {
                 Parameter.KEYWORD_ONLY,
                 Parameter.POSITIONAL_OR_KEYWORD,
             }:
                 continue
@@ -252,66 +384,162 @@
 
             if param.default is param.empty:
                 required.add(param.name)
 
             try:
                 if param.name in fields_sources:
                     sub_v = fields_sources[param.name](self.children)
+                elif param.name in fields_injections:
+                    sub_v = LiteralNode(self.fitter, fields_injections[param.name])
+                    literal_nodes[param.name] = sub_v
                 else:
                     sub_v = self.children[param.name]
 
                 if param.name not in hints:
                     sub_v.fail("Missing typing annotations")
             except KeyError:
                 pass
             else:
                 try:
                     kwargs[param.name] = self.fitter.fit_node(hints[param.name], sub_v)
                 except ValueError:
                     failed_keys.append(param.name)
 
-        missing = required - set(kwargs) - set(failed_keys)
-        unwanted = set(self.children) - expected
-        errors = []
+        return expected, failed_keys, kwargs, literal_nodes, required
+
+    def report_missing(
+        self, errors: MutableSequence[str], missing: Iterable[str]
+    ) -> None:
+        """
+        Some keys might be missing from the input JSON. This is where we do
+        the check and report them.
+
+        Parameters
+        ----------
+        errors
+            Output errors list
+        missing
+            The list of missing keys
+        """
 
         if missing:
             self.missing_keys = [*missing]
             errors.append(f'Missing keys: {", ".join(repr(x) for x in missing)}')
 
+    def report_unwanted(
+        self, errors: MutableSequence[str], t: Type[T], unwanted: Iterable[str]
+    ) -> None:
+        """
+        There is an option to report unwanted keys as errors. This is where
+        we do the check.
+
+        Parameters
+        ----------
+        errors
+            Output errors list
+        t
+            The type of the object that we're instantiating
+        unwanted
+            The list of unwanted keys
+        """
+
         if self.fitter.no_unwanted_keys and unwanted:
             self.unwanted_keys = [*unwanted]
             errors.append(f'Unwanted keys: {", ".join(repr(x) for x in unwanted)}')
 
             for k in unwanted:
                 self.children[k].errors.add(f"Unwanted by {format_type_name(t)}")
 
+    def report_failed(
+        self,
+        errors: MutableSequence[str],
+        failed_keys: Sequence[str],
+        fields_injections: Mapping[str, Any],
+        literal_nodes: Mapping[str, "LiteralNode"],
+    ) -> None:
+        """
+        If any sub-key failed to fit, we're going to report the error. One
+        of two thing might have happened:
+
+        - A "normal" key failed, aka it was impossible to fit the JSON value
+          into the expected type.
+        - An injection failed (in theory either root or context injection but
+          in practice it's only context injection that can fail). In that case
+          we'll report the error at this level as the goal is to be able to
+          display the error on the input JSON and since it's an injection the
+          value is not in the input JSON. Thus, the error will have to be
+          displayed at the level of the parent node (aka this node).
+
+        Parameters
+        ----------
+        errors
+            Some output list which will contain errors
+        failed_keys
+            The list of keys that failed to fit
+        fields_injections
+            The mapping of keys to the injection functions
+        literal_nodes
+            The mapping of keys to the literal nodes
+        """
+
         if failed_keys:
-            errors.append(f'No fit for keys: {", ".join(repr(x) for x in failed_keys)}')
+            if normal_failed_keys := set(failed_keys) - fields_injections.keys():
+                errors.append(
+                    f'No fit for keys: {", ".join(repr(x) for x in normal_failed_keys)}'
+                )
+
+            for key in failed_keys:
+                if key in literal_nodes:
+                    for error in literal_nodes[key].errors:
+                        errors.append(error)
+
+    def make_out_instance(
+        self, kwargs: Mapping[str, Any], root_fields: Sequence[str], t: Type[T]
+    ) -> T:
+        """
+        Generates the output instance from the kwargs.
+
+        Additionally this function has the mission to report into which fields
+        the root should be injected (if any). We know this from the root_fields
+        parameter which comes from the dataclass parsing logic in
+        :py:meth:`~.parse_dataclass`.
 
-        if errors:
-            self.problem_is_kids = True
-            self.fail(". ".join([f"Wrong keys set for {format_type_name(t)}", *errors]))
+        Parameters
+        ----------
+        kwargs
+            The kwargs that are going to be passed to the constructor
+        root_fields
+            The fields into which the root should be injected
+        t
+            The type of the object that we're instantiating
+        """
 
         out = t(**kwargs)
         self.fit_success = True
+
+        for field_name in root_fields:
+            self.fitter.root_injectors.append(set_root_attr(out, field_name))
+
         return out
 
     def fit(self, t: Type[T]) -> T:
         """
         This detects if we're dealing with a fit into a dictionary or a fit
         into a named tuple/dataclass.
 
         Parameters
         ----------
         t
             Type to fit into, either a Dict either NamedTuple either a
             @dataclass
         """
 
-        if get_origin(t) is dict:
+        origin = get_origin(t)
+
+        if origin is dict or (isclass(origin) and issubclass(origin, Mapping)):
             return self.fit_dict(t)
         elif is_named_tuple(t) or is_dataclass(t):
             return self.fit_object(t)
         else:
             self.fail(f"{format_type_name(t)} is not a mapping type")
 
 
@@ -335,15 +563,19 @@
     def fit(self, t: Type[T]) -> T:
         """
         After some sanity checks, goes through the whole list to make sure
         that all the content fits. If some of them don't fit, still continue
         to try fitting the rest, for error reporting purposes.
         """
 
-        if not get_origin(t) is list:
+        origin = get_origin(t)
+        is_list = origin is list
+        is_seq = isclass(origin) and issubclass(origin, Sequence)
+
+        if not (is_list or is_seq):
             self.fail(f"{format_type_name(t)} is not a list")
 
         args = get_args(t)
 
         if not args:
             self.fail("Could not determine list item type")
 
@@ -385,27 +617,27 @@
         ----------
         t
             Type to convert into, if not a builtin the None will be returned
         """
 
         if t is int:
             if not isinstance(self.value, int):
-                self.fail(f"Not an int")
+                self.fail("Not an int")
             return self.value
         elif t is float:
             if not isinstance(self.value, (int, float)):
-                self.fail(f"Neither a float nor an int")
+                self.fail("Neither a float nor an int")
             return float(self.value)
         elif t is str:
             if not isinstance(self.value, str):
-                self.fail(f"Not a string")
+                self.fail("Not a string")
             return self.value
         elif t is bool:
             if not isinstance(self.value, bool):
-                self.fail(f"Not a bool")
+                self.fail("Not a bool")
             return self.value
 
     def fit_class(self, t: Type[T]) -> T:
         """
         Fitting the content into a class. That one is a bit tricky but
         basically if the constructor can accept one argument and that this
         argument is properly annotated and that the value can fit into that
@@ -436,15 +668,16 @@
         if param.annotation is param.empty:
             self.fail("Constructor does not specify argument type")
 
         try:
             arg = self.fitter.fit(param.annotation, self.value)
         except ValueError:
             self.fail(
-                f"Constructor {format_type_name(t)} expects {param.annotation} but value does not fit"
+                f"Constructor {format_type_name(t)} expects "
+                f"{param.annotation} but value does not fit"
             )
 
         return t(arg)
 
     def fit(self, t: Type[T]) -> T:
         """
         Tries to use the builtins to fit and if not tries to see if there is
@@ -462,7 +695,28 @@
         out = self.fit_builtin(t)
 
         if out is None:
             out = self.fit_class(t)
 
         self.fit_success = True
         return out
+
+
+@dataclass
+class LiteralNode(Node):
+    """
+    This kind of node is used to inject a literal value that we don't want to
+    fit into anything. That's not really used on things coming from JSON, but
+    rather wraps stuff like context injections.
+
+    If the value is callable, it will be called without arguments. The callable
+    is expected to raise ValueError if its internal validation fails.
+    """
+
+    def fit(self, t: Type[T]) -> T:
+        if callable(self.value):
+            try:
+                return self.value()
+            except ValueError as e:
+                self.fail(e.args[0])
+        else:
+            return self.value
```

### Comparing `typefit-0.4.2/src/typefit/reporting.py` & `typefit-0.5.1/src/typefit/reporting.py`

 * *Files identical despite different names*

### Comparing `typefit-0.4.2/src/typefit/serialize.py` & `typefit-0.5.1/src/typefit/serialize.py`

 * *Files identical despite different names*

### Comparing `typefit-0.4.2/src/typefit/utils.py` & `typefit-0.5.1/src/typefit/utils.py`

 * *Files identical despite different names*

### Comparing `typefit-0.4.2/setup.py` & `typefit-0.5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: typefit
+Version: 0.5.1
+Summary: Fits JSON values into Python type-anotated objects
+Home-page: https://github.com/Xowap/typefit/
+License: WTFPL
+Keywords: typing,json,api
+Author: Rémy Sanchez
+Author-email: remy.sanchez@hyperthese.net
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.22,<2.0.0)
+Requires-Dist: pendulum (<3.0.0)
+Requires-Dist: pygments (<3.0.0)
+Project-URL: Repository, https://github.com/Xowap/typefit/
+Description-Content-Type: text/markdown
+
+# TypeFit
+
+[![Read the Docs](https://img.shields.io/readthedocs/typefit)](http://typefit.rtfd.io/)
+[![Build Status](https://github.com/Xowap/typefit/actions/workflows/run-tests.yaml/badge.svg)](https://github.com/Xowap/typefit/actions/workflows/run-tests.yaml)
+
+Typing annotations make Python awesome, however it's complicated to keep your
+data annotated when it comes from external sources like APIs. The goal of
+Typefit is to help you map that external data into type-annotated native Python
+objects.
+
+```python
+from typefit import api
+from typing import NamedTuple, Text
+
+
+class Item(NamedTuple):
+    id: int
+    title: Text
+
+
+class HackerNews(api.SyncClient):
+    BASE_URL = "https://hacker-news.firebaseio.com/v0/"
+
+    @api.get("item/{item_id}.json")
+    def get_item(self, item_id: int) -> Item:
+        pass
+
+story = HackerNews().get_item(42)
+print(story.title)
+# An alternative to VC: &#34;Selling In&#34;
+```
+
+This is the full example of a Hacker News API client. Its functionality is
+limited but in 14 lines counting white space you can build a type-safe client
+for Hacker News. You'll find a [full example](example/typefit_hn) attached if
+you're interested.
+
+## Documentation
+
+[✨ **Documentation is there** ✨](http://typefit.rtfd.io/)
+
+## Licence
+
+This library is provided under the terms of the [WTFPL](./LICENSE).
+
+If you find it useful, you can have a look at the
+[contributors](https://github.com/Xowap/typefit/graphs/contributors) page to
+know who helped.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['typefit']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.22,<2.0.0', 'pendulum<3.0.0', 'pygments<3.0.0']
-
-setup_kwargs = {
-    'name': 'typefit',
-    'version': '0.4.2',
-    'description': 'Fits JSON values into Python type-anotated objects',
-    'long_description': '# TypeFit\n\n[![Read the Docs](https://img.shields.io/readthedocs/typefit)](http://typefit.rtfd.io/)\n[![Build Status](https://img.shields.io/travis/Xowap/typefit)](https://travis-ci.org/Xowap/typefit)\n[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/Xowap/typefit)](https://lgtm.com/projects/g/Xowap/typefit/)\n\nTyping annotations make Python awesome, however it\'s complicated to keep your\ndata annotated when it comes from external sources like APIs. The goal of\nTypefit is to help you map that external data into type-annotated native Python\nobjects.\n\n```python\nfrom typefit import api\nfrom typing import NamedTuple, Text\n\n\nclass Item(NamedTuple):\n    id: int\n    title: Text\n\n\nclass HackerNews(api.SyncClient):\n    BASE_URL = "https://hacker-news.firebaseio.com/v0/"\n\n    @api.get("item/{item_id}.json")\n    def get_item(self, item_id: int) -> Item:\n        pass\n\nstory = HackerNews().get_item(42)\nprint(story.title)\n# An alternative to VC: &#34;Selling In&#34;\n```\n\nThis is the full example of a Hacker News API client. Its functionality is\nlimited but in 14 lines counting white space you can build a type-safe client\nfor Hacker News. You\'ll find a [full example](example/typefit_hn) attached if\nyou\'re interested.\n\n\n## Documentation\n\n[✨ **Documentation is there** ✨](http://typefit.rtfd.io/)\n\n## Licence\n\nThis library is provided under the terms of the [WTFPL](./LICENSE).\n\nIf you find it useful, you can have a look at the\n[contributors](https://github.com/Xowap/typefit/graphs/contributors) page to\nknow who helped.\n',
-    'author': 'Rémy Sanchez',
-    'author_email': 'remy.sanchez@hyperthese.net',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Xowap/typefit/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

