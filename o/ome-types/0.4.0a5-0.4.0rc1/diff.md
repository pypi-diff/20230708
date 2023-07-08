# Comparing `tmp/ome_types-0.4.0a5.tar.gz` & `tmp/ome_types-0.4.0rc1.tar.gz`

## Comparing `ome_types-0.4.0a5.tar` & `ome_types-0.4.0rc1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/_config.py
--rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_autogen/main.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/__init__.py
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_conversion.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/units.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_bin_data.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_kinded.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_pixels.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/_structured_annotations.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/LICENSE
--rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/hatch_build.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/pyproject.toml
--rw-r--r--   0        0        0    11376 2020-02-02 00:00:00.000000 ome_types-0.4.0a5/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/main.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/__init__.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/units.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_bin_data.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_pixels.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/hatch_build.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 ome_types-0.4.0rc1/PKG-INFO
```

### Comparing `ome_types-0.4.0a5/CHANGELOG.md` & `ome_types-0.4.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_autogen/_config.py` & `ome_types-0.4.0rc1/src/ome_autogen/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 from xsdata.codegen.writer import CodeWriter
 from xsdata.models import config as cfg
 from xsdata.utils import text
 
 from ome_autogen._generator import OmeGenerator
 from ome_autogen._util import camel_to_snake
 
-KindedTypes = "(Shape|ManufacturerSpec|Annotation)"
-
-
 MIXIN_MODULE = "ome_types._mixins"
 MIXINS: list[tuple[str, str, bool]] = [
     (".*", f"{MIXIN_MODULE}._base_type.OMEType", False),  # base type on every class
     ("OME", f"{MIXIN_MODULE}._ome.OMEMixin", True),
     ("Instrument", f"{MIXIN_MODULE}._instrument.InstrumentMixin", False),
     ("Reference", f"{MIXIN_MODULE}._reference.ReferenceMixin", True),
     ("BinData", f"{MIXIN_MODULE}._bin_data.BinDataMixin", True),
     ("Pixels", f"{MIXIN_MODULE}._pixels.PixelsMixin", True),
-    (KindedTypes, f"{MIXIN_MODULE}._kinded.KindMixin", True),
 ]
 
 ALLOW_RESERVED_NAMES = {"type", "Type", "Union"}
 OME_FORMAT = "OME"
 
 
 def get_config(
```

### Comparing `ome_types-0.4.0a5/src/ome_autogen/_generator.py` & `ome_types-0.4.0rc1/src/ome_autogen/_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, NamedTuple
+import sys
+from contextlib import contextmanager
+from pathlib import Path
+from typing import TYPE_CHECKING, Iterator, NamedTuple, cast
 
 from xsdata.formats.dataclass.filters import Filters
 from xsdata.formats.dataclass.generator import DataclassGenerator
 
 from ome_autogen import _util
 from xsdata_pydantic_basemodel.generator import PydanticBaseFilters
 
 if TYPE_CHECKING:
+    from jinja2 import Environment, FileSystemLoader
     from xsdata.codegen.models import Attr, Class
     from xsdata.codegen.resolver import DependenciesResolver
     from xsdata.models.config import GeneratorConfig
 
 
 # from ome_types._mixins._base_type import AUTO_SEQUENCE
 # avoiding import to avoid build-time dependency on the ome-types package
@@ -87,22 +91,70 @@
         if aliases:
             mod += "\n\n" + "\n".join(aliases) + "\n"
 
         return mod
 
 
 class OmeFilters(PydanticBaseFilters):
+    def register(self, env: Environment) -> None:
+        # add our own templates dir to the search path
+        tpl_dir = Path(__file__).parent.joinpath("templates")
+        cast("FileSystemLoader", env.loader).searchpath.insert(0, str(tpl_dir))
+        return super().register(env)
+
     def __init__(self, config: GeneratorConfig):
         super().__init__(config)
 
         # TODO: it would be nice to know how to get the schema we're processing from
         # the config.  For now, we just assume it's the OME schema and that's the
         # hardcoded default in _util.get_appinfo
         self.appinfo = _util.get_appinfo()
 
+    @contextmanager
+    def _modern_typing(self) -> Iterator[None]:
+        """Context manager to use modern typing syntax."""
+        prev_u, self.union_type = self.union_type, True
+        prev_s, self.subscriptable_types = self.subscriptable_types, True
+        try:
+            yield
+        finally:
+            self.union_type = prev_u
+            self.subscriptable_types = prev_s
+
+    def class_params(self, obj: Class) -> Iterator[tuple[str, str, str]]:
+        # This method override goes along with the docstring jinja template override
+        # to fixup the numpy docstring format.
+        # https://github.com/tefra/xsdata/issues/818
+
+        if sys.version_info < (3, 8):  # pragma: no cover
+            # i don't know why, but in python 3.7, it's not picking up our
+            # template ... so this method yields too many values to unpack
+            # xsdata/formats/dataclass/templates/docstrings.numpy.jinja2", line 6
+            #   {%- for var_name, var_doc in obj | class_params %}
+            #       ValueError: too many values to unpack (expected 2)
+            # however, it's not at all important that we be able to build docs correctly
+            # on python 3.7.  The built wheel will still work fine (and won't be built
+            # on python 3.7 anyway)
+            yield from super().class_params(obj)
+            return
+
+        for attr in obj.attrs:
+            name = attr.name
+            name = (
+                self.constant_name(name, obj.name)
+                if obj.is_enumeration
+                else self.field_name(name, obj.name)
+            )
+            with self._modern_typing():
+                type_ = self.field_type(attr, [obj.name])
+            help_ = attr.help
+            if not help_:
+                help_ = f"(The {obj.name} {attr.name})."
+            yield name, type_, self.clean_docstring(help_)
+
     def class_bases(self, obj: Class, class_name: str) -> list[str]:
         # we don't need PydanticBaseFilters to add the Base class
         # because we add it in the config.extensions
         # This could go once PydanticBaseFilters is better about deduping
         return Filters.class_bases(self, obj, class_name)
 
     def _attr_is_optional(self, attr: Attr) -> bool:
@@ -114,22 +166,23 @@
 
     def _format_type(self, attr: Attr, result: str) -> str:
         if self._attr_is_optional(attr):
             return f"None | {result}" if self.union_type else f"Optional[{result}]"
         return result
 
     def field_type(self, attr: Attr, parents: list[str]) -> str:
-        if attr.is_list:
+        if attr.is_list and not getattr(attr, "_plural_set", False):
             # HACK
             # It would be nicer to put this in the self.field_name method...but that
             # method only receives the attr name, not the attr object, and so we
             # don't know at that point whether it belongs to a list or not.
             # This hack works only because this method is called BEFORE self.field_name
             # in the class.jinja2 template, so we directly modify the attr object here.
             attr.name = self.appinfo.plurals.get(attr.name, f"{attr.name}s")
+            attr._plural_set = True  # type: ignore
 
         if attr.name in OVERRIDE_ELEM_TO_CLASS:
             return self._format_type(attr, OVERRIDE_ELEM_TO_CLASS[attr.name])
 
         type_name = super().field_type(attr, parents)
         # we want to use datetime.datetime instead of XmlDateTime
         return type_name.replace("XmlDateTime", "datetime")
```

### Comparing `ome_types-0.4.0a5/src/ome_autogen/_util.py` & `ome_types-0.4.0rc1/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_autogen/main.py` & `ome_types-0.4.0rc1/src/ome_autogen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 def _check_mypy(package_dir: str) -> None:
     _print_gray("Running mypy ...")
 
     mypy = ["mypy", package_dir, "--strict"]
     try:
         subprocess.check_output(mypy, stderr=subprocess.STDOUT)  # noqa S
-    except subprocess.CalledProcessError as e:
+    except subprocess.CalledProcessError as e:  # pragma: no cover
         raise RuntimeError(f"mypy errors:\n\n{e.output.decode()}") from e
 
 
 def _print_gray(text: str) -> None:
     if os.name != "nt":
         # UnicodeEncodeError: 'charmap' codec can't encode character '\u2713'
         text = f"\033[90m\033[1m{text}\033[0m"
```

### Comparing `ome_types-0.4.0a5/src/ome_types/__init__.py` & `ome_types-0.4.0rc1/src/ome_types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 try:
     from importlib.metadata import PackageNotFoundError, version
-except ImportError:
+except ImportError:  # pragma: no cover
     from importlib_metadata import PackageNotFoundError, version  # type: ignore
 
 try:
     __version__ = version("ome-types")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 
+from typing import Any
+
 from ome_types import model
 from ome_types._conversion import from_tiff, from_xml, to_dict, to_xml
 from ome_types.model import OME
-from ome_types.units import ureg
 from ome_types.validation import validate_xml
 
 __all__ = [
     "__version__",
     "from_tiff",
     "from_xml",
     "model",
     "OME",
     "to_dict",
     "to_xml",
     "ureg",
     "validate_xml",
 ]
+
+
+def __getattr__(name: str) -> Any:
+    if name == "ureg":
+        from ome_types.units import ureg
+
+        return ureg
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_conversion.py` & `ome_types-0.4.0rc1/src/ome_types/_conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,14 +71,26 @@
     except AttributeError as e:  # pragma: no cover
         raise ValueError(
             f"Could not find a class for {localname!r} in {mod.__name__}"
         ) from e
 
 
 def to_dict(source: OME | Path | str | bytes) -> dict[str, Any]:
+    """Return a dictionary representation of an OME or XML document.
+
+    Parameters
+    ----------
+    source : OME | Path | str | bytes
+        An OME object, or a path to an XML file, or a string or bytes containing XML.
+
+    Returns
+    -------
+    dict[str, Any]
+        A dictionary representation of the OME object or XML document.
+    """
     if is_dataclass(source):  # pragma: no cover
         raise NotImplementedError("dataclass -> dict is not supported yet")
 
     if isinstance(source, BaseModel):
         return source.dict(exclude_defaults=True)
 
     return from_xml(  # type: ignore[return-value]
@@ -92,14 +104,35 @@
 def from_xml(
     xml: Path | str | bytes,
     *,
     validate: bool | None = None,
     parser: Any = None,
     parser_kwargs: ParserKwargs | None = None,
 ) -> OME:
+    """Generate an OME object from an XML document.
+
+    Parameters
+    ----------
+    xml : Path | str | bytes
+        Path to an XML file, or a string or bytes containing XML.
+    validate : bool | None
+        Whether to validate the XML document against the OME schema.
+        If None, validation will be skipped if lxml is not available,
+        and will be performed otherwise.
+    parser : Any
+        Ignored, but kept for backwards compatibility.
+    parser_kwargs : ParserKwargs | None
+        Passed to the XmlParser constructor. If None, a default parser
+        will be used.
+
+    Returns
+    -------
+    OME
+        The OME object parsed from the XML document.
+    """
     if parser is not None:  # pragma: no cover
         warnings.warn(
             "As of version 0.4.0, the parser argument is ignored. "
             "lxml will be used if available in the environment, but you can "
             "drop this keyword argument.",
             DeprecationWarning,
             stacklevel=2,
@@ -124,15 +157,15 @@
         return parser_.parse(xml, OME_type)
     return parser_.from_string(xml, OME_type)
 
 
 def to_xml(
     ome: OME,
     *,
-    # exclude_defaults takes precendence over exclude_unset
+    # exclude_defaults takes precedence over exclude_unset
     # if a value equals the default, it will be excluded
     exclude_defaults: bool = False,
     # exclude_unset will exclude any value that is not explicitly set
     # but will INCLUDE values that are set to their default
     exclude_unset: bool = True,
     indent: int = 2,
     include_namespace: bool | None = None,
@@ -174,14 +207,28 @@
 
 def from_tiff(
     path: Path | str,
     *,
     validate: bool | None = None,
     parser_kwargs: ParserKwargs | None = None,
 ) -> OME:
+    """Generate an OME object from a TIFF file.
+
+    Parameters
+    ----------
+    path : Path | str
+        Path to a TIFF file.
+    validate : bool | None
+        Whether to validate the XML document against the OME schema before parsing.
+        If None, validation will be skipped if lxml is not available,
+        and will be performed otherwise.
+    parser_kwargs : ParserKwargs | None
+        Passed to the XmlParser constructor. If None, a default parser
+        will be used.
+    """
     xml = tiff2xml(path)
     return from_xml(xml, validate=validate, parser_kwargs=parser_kwargs)
 
 
 TIFF_TYPES: dict[bytes, tuple[Struct, Struct, int, Struct]] = {
     b"II*\0": (Struct("<I"), Struct("<H"), 12, Struct("<H")),
     b"MM\0*": (Struct(">I"), Struct(">H"), 12, Struct(">H")),
```

### Comparing `ome_types-0.4.0a5/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0rc1/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/validation.py` & `ome_types-0.4.0rc1/src/ome_types/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from typing import IO, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     import xmlschema
 
     XMLSourceType = Union[str, bytes, Path, IO[str], IO[bytes]]
 
-NS_OME = r"{http://www.openmicroscopy.org/Schemas/OME/2016-06}"
+OME_URI = "http://www.openmicroscopy.org/Schemas/OME/2016-06"
+OME_NS = f"{{{OME_URI}}}"
 OME_2016_06_XSD = str(Path(__file__).parent / "ome-2016-06.xsd")
 
 
 class ValidationError(ValueError):
     ...
 
 
@@ -75,11 +76,11 @@
 @lru_cache(maxsize=None)
 def _get_XMLSchema(schema: Path | str) -> xmlschema.XMLSchema:
     import xmlschema
 
     xml_schema = xmlschema.XMLSchema(schema)
     # FIXME Hack to work around xmlschema poor support for keyrefs to
     # substitution groups
-    ls_sgs = xml_schema.maps.substitution_groups[f"{NS_OME}LightSourceGroup"]
-    ls_id_maps = xml_schema.maps.identities[f"{NS_OME}LightSourceIDKey"]
+    ls_sgs = xml_schema.maps.substitution_groups[f"{OME_NS}LightSourceGroup"]
+    ls_id_maps = xml_schema.maps.identities[f"{OME_NS}LightSourceIDKey"]
     ls_id_maps.elements = {e: None for e in ls_sgs}
     return xml_schema
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_base_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import warnings
 from datetime import datetime
 from enum import Enum
 from textwrap import indent
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Sequence, Set, Tuple, cast
+from typing import Any, ClassVar, Dict, Optional, Sequence, Set, Tuple
 
 from pydantic import BaseModel, validator
 
 from ome_types._mixins._ids import validate_id
-from ome_types.units import ureg
-
-if TYPE_CHECKING:
-    import pint
 
+try:
+    from ome_types.units import add_quantity_properties
+except ImportError:
+    add_quantity_properties = lambda cls: None  # noqa: E731
 
 # Default value to support automatic numbering for id field values.
 AUTO_SEQUENCE = "__auto_sequence__"
 
 
-_UNIT_FIELD = "{}_unit"
-_QUANTITY_FIELD = "{}_quantity"
 DEPRECATED_NAMES = {
     "annotation_ref": "annotation_refs",
     "bin_data": "bin_data_blocks",
     "dataset_ref": "dataset_refs",
     "emission_filter_ref": "emission_filters",
     "excitation_filter_ref": "excitation_filters",
     "experimenter_ref": "experimenter_refs",
@@ -34,22 +32,36 @@
     "microbeam_manipulation_ref": "microbeam_manipulation_refs",
     "plate_ref": "plate_refs",
     "roi_ref": "roi_refs",
     "well_sample_ref": "well_sample_refs",
 }
 
 
+def _move_deprecated_fields(data: Dict[str, Any], field_names: Set[str]) -> None:
+    for key in list(data):
+        if (
+            key not in field_names
+            and key in DEPRECATED_NAMES
+            and DEPRECATED_NAMES[key] in field_names
+        ):
+            warnings.warn(
+                f"Field {key!r} is deprecated. Use {DEPRECATED_NAMES[key]!r} instead.",
+                stacklevel=2,
+            )
+            data[DEPRECATED_NAMES[key]] = data.pop(key)
+
+
 class OMEType(BaseModel):
     """The base class that all OME Types inherit from.
 
     This provides some global conveniences around auto-setting ids. (i.e., making them
-    optional in the class constructor, but never ``None`` after initialization.).
-    It provides a nice __repr__ that hides things that haven't been changed from
+    optional in the class constructor, but never `None` after initialization.).
+    It provides a nice `__repr__` that hides things that haven't been changed from
     defaults.  It adds ``*_quantity`` property for fields that have both a value and a
-    unit, where ``*_quantity`` is a pint ``Quantity``.  It also provides pickling
+    unit, where `*_quantity` is a [`pint.Quantity`][].  It also provides pickling
     support.
     """
 
     # pydantic BaseModel configuration.
     # see: https://pydantic-docs.helpmanual.io/usage/model_config/
     class Config:
         arbitrary_types_allowed = False
@@ -60,37 +72,38 @@
 
     # allow use with weakref
     __slots__: ClassVar[Set[str]] = {"__weakref__"}  # type: ignore
 
     _v = validator("id", pre=True, always=True, check_fields=False)(validate_id)
 
     def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
         field_names = set(self.__fields__.keys())
+        _move_deprecated_fields(data, field_names)
+        super().__init__(**data)
         kwargs = set(data.keys())
         if kwargs - field_names:
             warnings.warn(
                 f"Unrecognized fields for type {type(self)}: {kwargs - field_names}",
                 stacklevel=2,
             )
 
     def __init_subclass__(cls) -> None:
         """Add `*_quantity` property for fields that have both a value and a unit.
 
         where `*_quantity` is a pint `Quantity`.
         """
-        for field in cls.__fields__:
-            if _UNIT_FIELD.format(field) in cls.__fields__:
-                setattr(cls, _QUANTITY_FIELD.format(field), _quantity_property(field))
+        add_quantity_properties(cls)
 
     def __repr_args__(self) -> Sequence[Tuple[Optional[str], Any]]:
         """Repr with only set values, and truncated sequences."""
         args = []
         for k, v in self._iter(exclude_defaults=True):
             if isinstance(v, Sequence) and not isinstance(v, str):
+                if v == []:  # skip empty lists
+                    continue
                 # if this is a sequence with a long repr, just show the length
                 # and type
                 if len(repr(v).split(",")) > 5:
                     type_name = self.__fields__[k].type_.__name__
                     v = _RawRepr(f"[<{len(v)} {type_name}>]")
             elif isinstance(v, Enum):
                 v = v.value
@@ -119,28 +132,14 @@
                 DeprecationWarning,
                 stacklevel=2,
             )
             return getattr(self, new_key)
         raise AttributeError(f"{cls_name} object has no attribute {key!r}")
 
 
-def _quantity_property(field_name: str) -> property:
-    """Create property that returns a ``pint.Quantity`` combining value and unit."""
-
-    def quantity(self: Any) -> Optional["pint.Quantity"]:
-        value = getattr(self, field_name)
-        if value is None:
-            return None
-
-        unit = cast("Enum", getattr(self, _UNIT_FIELD.format(field_name)))
-        return ureg.Quantity(value, unit.value.replace(" ", "_"))
-
-    return property(quantity)
-
-
 class _RawRepr:
     """Helper class to allow repr to show raw values for fields that are sequences."""
 
     def __init__(self, raw: str) -> None:
         self.raw = raw
 
     def __repr__(self) -> str:
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_bin_data.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_bin_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     @root_validator(pre=True)
     def _v(cls, values: dict) -> Dict[str, Any]:
         # This catches the case of <BinData Length="0"/>, where the parser may have
         # omitted value from the dict, and sets value to b""
         # seems like it could be done in a default_factory, but that would
         # require more modification of xsdata I think
         if "value" not in values:
-            if values.get("length") != 0:
+            if values.get("length") != 0:  # pragma: no cover
                 warnings.warn(
                     "BinData length is non-zero but value is missing", stacklevel=2
                 )
             values["value"] = b""
         return values
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,13 +73,13 @@
         # store the converted ID so we can use it elsewhere
         CONVERTED_IDS[(id_name, value)] = newname
 
         # warn the user
         msg = f"Casting invalid {id_name}ID {value!r} to {newname!r}"
         warnings.warn(msg, stacklevel=2)
         return newname
-    elif not isinstance(value, int):
+    elif not isinstance(value, int):  # pragma: no cover
         raise ValueError(f"Invalid ID value: {value!r}, {type(value)}")
 
     # update the counter to be at least this value
     ID_COUNTER[id_name] = max(current_count, value)
     return f"{id_name}:{value}"
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         GenericExcitationSource, LightEmittingDiode, Filament, Arc, Laser
     ]
 
 
 class InstrumentMixin:
     @property
     def light_source_group(self) -> List["LightSource"]:
+        # here for backwards compatibility
         slf = cast("Instrument", self)
         return [
             *slf.arcs,
             *slf.filaments,
             *slf.generic_excitation_sources,
             *slf.lasers,
             *slf.light_emitting_diodes,
```

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_ome.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_pixels.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_pixels.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0rc1/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/model/__init__.py` & `ome_types-0.4.0rc1/src/ome_types/model/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 from ome_types._autogenerated.ome_2016_06 import *  # noqa
 
 # these are here mostly to make mypy happy in pre-commit
 # even when the model isn't built
 from ome_types._autogenerated.ome_2016_06 import OME as OME
 from ome_types._autogenerated.ome_2016_06 import Reference as Reference
+from ome_types.model._color import Color as Color
+from ome_types.model._shape_union import ShapeUnion as ShapeUnion
+from ome_types.model._structured_annotations import (
+    StructuredAnnotationList as StructuredAnnotationList,
+)
 
 if TYPE_CHECKING:
     from importlib.machinery import ModuleSpec
     from types import ModuleType
 
 # ---------------------------------------------------------------------
 # Below here is logic to allow importing from ome_types._autogenerated.ome_2016_06
```

### Comparing `ome_types-0.4.0a5/src/ome_types/model/_color.py` & `ome_types-0.4.0rc1/src/ome_types/model/_color.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 __all__ = ["Color"]
 
 RGBA = Tuple[int, int, int, float]
 ColorType = Union[Tuple[int, int, int], RGBA, str, int]
 
 
 class Color(color.Color):
+    """A Pydantic Color subclass that converts to and from OME int32 types."""
+
     def __init__(self, val: ColorType = -1) -> None:
         with suppress(ValueError, TypeError):
             val = self._int2tuple(int(val))  # type: ignore
         super().__init__(val)  # type: ignore [arg-type]
 
     @classmethod
     def _int2tuple(cls, val: int) -> RGBA:
```

### Comparing `ome_types-0.4.0a5/src/ome_types/model/_converters.py` & `ome_types-0.4.0rc1/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/model/_structured_annotations.py` & `ome_types-0.4.0rc1/src/ome_types/model/_structured_annotations.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,18 +29,34 @@
     CommentAnnotation,
     BooleanAnnotation,
     TimestampAnnotation,
     TagAnnotation,
     TermAnnotation,
     MapAnnotation,
 )
-_KINDS = {cls.__name__.lower(): cls for cls in AnnotationTypes}
 
 
 class StructuredAnnotationList(OMEType, UserSequence[Annotation]):  # type: ignore[misc]
+    """A mutable sequence of [`ome_types.model.Annotation`][].
+
+    Members of this sequence must be one of the following types:
+
+    - [`ome_types.model.XMLAnnotation`][]
+    - [`ome_types.model.FileAnnotation`][]
+    - [`ome_types.model.ListAnnotation`][]
+    - [`ome_types.model.LongAnnotation`][]
+    - [`ome_types.model.DoubleAnnotation`][]
+    - [`ome_types.model.CommentAnnotation`][]
+    - [`ome_types.model.BooleanAnnotation`][]
+    - [`ome_types.model.TimestampAnnotation`][]
+    - [`ome_types.model.TagAnnotation`][]
+    - [`ome_types.model.TermAnnotation`][]
+    - [`ome_types.model.MapAnnotation`][]
+    """
+
     # NOTE: in reality, this is List[StructuredAnnotationTypes]... but
     # for some reason that messes up xsdata data binding
     __root__: List[object] = Field(
         default_factory=list,
         metadata={
             "type": "Elements",
             "choices": tuple(
@@ -50,16 +66,14 @@
     )
 
     @validator("__root__", each_item=True)
     def _validate_root(cls, v: Annotation) -> Annotation:
         if isinstance(v, AnnotationTypes):
             return v
         if isinstance(v, dict):
-            if "kind" in v:
-                return _KINDS[v.pop("kind")](**v)
             for cls_ in AnnotationTypes:
                 with suppress(ValidationError):
                     return cls_(**v)
         raise ValueError(f"Invalid Annotation: {v} of type {type(v)}")
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.__root__!r})"
```

### Comparing `ome_types-0.4.0a5/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.0rc1/src/ome_types/model/_user_sequence.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/ome_types/model/simple_types.py` & `ome_types-0.4.0rc1/src/ome_types/model/simple_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""This module is only here for backwards compatibility.
+"""This module is only here for backwards compatibility with v<0.4.0 of ome-types.
 
-Should add a deprecation warning.
+Most of the types defined here are also exported from `ome_types.model`.  But for
+now, you can also import them from here.
 """
 from enum import Enum
 
 from ome_types._autogenerated.ome_2016_06 import (
     Binning,
     Marker,
     NamingConvention,
```

### Comparing `ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.0rc1/src/xsdata_pydantic_basemodel/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         # add BaseModel to the class bases
         # FIXME ... need to dedupe superclasses
         bases = super().class_bases(obj, class_name)
         return unique_sequence([*bases, "BaseModel"])
 
     def move_metadata_to_pydantic_field(self, kwargs: dict, pop: bool = False) -> None:
         """Move metadata from the metadata dict to the pydantic Field kwargs."""
-        # XXX: can we pop them?  or does xsdata need them in the metdata dict as well?
+        # XXX: can we pop them?  or does xsdata need them in the metadata dict as well?
         if "metadata" not in kwargs:  # pragma: no cover
             return
 
         metadata: dict = kwargs["metadata"]
         getitem = metadata.pop if pop else metadata.get
         for from_, to_ in [
             ("min_inclusive", "ge"),
```

### Comparing `ome_types-0.4.0a5/.gitignore` & `ome_types-0.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/LICENSE` & `ome_types-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a5/README.md` & `ome_types-0.4.0rc1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,46 +3,58 @@
 [![License](https://img.shields.io/github/license/tlambert03/ome-types)](LICENSE)
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/ome-types.svg)](https://python.org)
 [![Tests](https://github.com/tlambert03/ome-types/workflows/tests/badge.svg)](https://github.com/tlambert03/ome-types/actions)
 [![Docs](https://readthedocs.org/projects/ome-types/badge/?version=latest)](https://ome-types.readthedocs.io/en/latest/?badge=latest)
-<!-- [![conda-forge](https://img.shields.io/conda/vn/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types) -->
+[![codecov](https://codecov.io/gh/tlambert03/ome-types/branch/main/graph/badge.svg?token=GocY9y8A32)](https://codecov.io/gh/tlambert03/ome-types)
 
 ## A pure-python implementation of the OME data model
 
 `ome_types` provides a set of python dataclasses and utility functions for
 parsing the [OME-XML
 format](https://docs.openmicroscopy.org/ome-model/latest/ome-xml/) into
 fully-typed python objects for interactive or programmatic access in python. It
 can also take these python objects and output them into valid OME-XML.
 `ome_types` is a **pure python** library and does not require a Java virtual
 machine.
 
 > Note: The generated python code can be seen in the [`built`
-branch](https://github.com/tlambert03/ome-types/tree/built).
-(Read the [code generation](#code-generation) section for details).
+> branch](https://github.com/tlambert03/ome-types/tree/built).
+> (Read the [code generation](#code-generation) section for details).
 
-### 📖  &nbsp;&nbsp;[documentation](https://ome-types.readthedocs.io/)
+### 📖 &nbsp;&nbsp;[documentation](https://ome-types.readthedocs.io/)
 
 ## Installation
 
 ### from pip
 
 ```shell
 pip install ome-types
 ```
 
-### from source
+With all optional dependencies:
 
 ```shell
-git clone https://github.com/tlambert03/ome-types.git
-cd ome-types
-pip install -e .
+# lxml => if you want to use lxml as the XML parser
+# pint => if you want to use object.<field>_quantity properties
+pip install ome-types[lxml,pint]
+```
+
+### from conda
+
+```shell
+conda install -c conda-forge ome-types
+```
+
+### from github (bleeding edge dev version)
+
+```shell
+pip install git+https://github.com/tlambert03/ome-types.git
 ```
 
 ## Usage
 
 ### convert an XML string or filepath into an instance of `ome_types.model.OME`
 
 (The XML string/file will be validated against the [ome.xsd
@@ -168,15 +180,15 @@
     microscope=Microscope(
        manufacturer='OME Instruments',
        model='Lab Mk4',
        serial_number='L4-5678',
     ),
     objectives=[<1 Objectives>],
  )]
- ```
+```
 
 ### export to an OME-XML string
 
 Finally, you can generate the OME-XML representation of the OME model object,
 for writing to a standalone `.ome.xml` file or inserting into the header of an
 OME-TIFF file:
 
@@ -203,104 +215,61 @@
         </Pixels>
     </Image>
 </OME>
 ```
 
 ## Code generation
 
-The bulk of this library (namely, the `ome_types.model` module) is generated
-at install time, and is therefore not checked into source (or visible in the main
-branch of this repo).
+The bulk of this library (namely, modules inside `ome_types._autogenerated`) is
+generated at install time, and is therefore not checked into source (or visible
+in the main branch of this repo).
 
 You can see the code generated by the main branch in the [built
 branch](https://github.com/tlambert03/ome-types/tree/built)
 
-
-The script at `src/ome_autogen.py` converts the [ome.xsd
+The package at `src/ome_autogen` converts the [ome.xsd
 schema](https://www.openmicroscopy.org/Schemas/OME/2016-06/ome.xsd) into valid
 python code. To run the code generation script in a development environment,
 clone this repository and run:
 
 ```sh
-python src/ome_autogen.py
+python -m src.ome_autogen
 ```
 
-As an example, the
-[`OME/Image`](https://www.openmicroscopy.org/Schemas/Documentation/Generated/OME-2016-06/ome_xsd.html#Image)
-model will be rendered as the following dataclass in `ome_types/model/image.py`
-
-```python
-from datetime import datetime
-from typing import List, Optional
-
-from pydantic import Field
-
-from ome_types._base_type import OMEType
-
-from .annotation_ref import AnnotationRef
-from .experiment_ref import ExperimentRef
-from .experimenter_group_ref import ExperimenterGroupRef
-from .experimenter_ref import ExperimenterRef
-from .imaging_environment import ImagingEnvironment
-from .instrument_ref import InstrumentRef
-from .microbeam_manipulation_ref import MicrobeamManipulationRef
-from .objective_settings import ObjectiveSettings
-from .pixels import Pixels
-from .roi_ref import ROIRef
-from .simple_types import ImageID
-from .stage_label import StageLabel
-
-
-class Image(OMEType):
-    id: ImageID
-    pixels: Pixels
-    acquisition_date: Optional[datetime] = None
-    annotation_ref: List[AnnotationRef] = Field(default_factory=list)
-    description: Optional[str] = None
-    experiment_ref: Optional[ExperimentRef] = None
-    experimenter_group_ref: Optional[ExperimenterGroupRef] = None
-    experimenter_ref: Optional[ExperimenterRef] = None
-    imaging_environment: Optional[ImagingEnvironment] = None
-    instrument_ref: Optional[InstrumentRef] = None
-    microbeam_manipulation_ref: List[MicrobeamManipulationRef] = Field(
-        default_factory=list
-    )
-    name: Optional[str] = None
-    objective_settings: Optional[ObjectiveSettings] = None
-    roi_ref: List[ROIRef] = Field(default_factory=list)
-    stage_label: Optional[StageLabel] = None
-```
 
 The documentation and types for the full model can be in the [API Reference](https://ome-types.readthedocs.io/en/latest/ome_types.model.html)
 
 ## Contributing
 
-To clone and install this repository locally (this will also build the model at
-`src/ome_types/model`)
+To clone and install this repository locally:
 
 ```shell
 git clone https://github.com/tlambert03/ome-types.git
 cd ome-types
-pip install -e .[autogen]
+pip install -e .[test,dev]
 ```
 
-We use `pre-commit` to run various code-quality checks (isort, black, mypy,
-flake8) during continuous integration.  If you'd like to make sure that your
-code will pass these checks before you commit your code, you should install
-`pre-commit` after cloning this repository:
+We use `pre-commit` to run various code-quality checks  during continuous
+integration. If you'd like to make sure that your code will pass these checks
+before you commit your code, you should install `pre-commit` after cloning this
+repository:
 
 ```shell
-pip install pre-commit
 pre-commit install
 ```
 
-If you modify `src/ome_autogen.py`, you may need to regenerate the model with:
+### regenerating the models
+
+If you modify anything in `src/ome_autogen`, you may need to
+regenerate the model with:
 
 ```shell
-python src/ome_autogen.py
+python -m src.ome_autogen
 ```
 
 ### Running tests
 
-To run tests quickly, just install and run `pytest`.  Note, however, that this
-requires that the `ome_types.model` module has already been built with `python
-src/ome_autogen.py`.
+To run tests:
+
+```
+pytest
+```
```

### Comparing `ome_types-0.4.0a5/pyproject.toml` & `ome_types-0.4.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,48 +25,49 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
-  "Pint >=0.15",
-  "lxml >=4.8.0",
-  "pydantic[email] <2.0",
-  "xsdata",
+  "pydantic <2.0",
+  "xsdata >=23.5",                              # 23.6 necessary for codegen, but not for runtime
   "importlib_metadata; python_version < '3.8'",
 ]
 
 [project.urls]
 Source = "https://github.com/tlambert03/ome-types"
 Tracker = "https://github.com/tlambert03/ome-types/issues"
 Documentation = "https://ome-types.readthedocs.io/en/latest/"
 
 [project.entry-points."napari.plugin"]
 ome-types = "ome_types._napari_plugin"
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
+pint = ["Pint >=0.15"]
+lxml = ["lxml >=4.8.0"]
 dev = [
   "black",
   "ruff",
   "xsdata[cli]>=23.6",
   "mypy",
   "pre-commit",
   "types-lxml; python_version >= '3.8'",
 ]
-docs = [
-  "numpydoc",
-  "pygments",
-  "sphinx==5.3.0",
-  "sphinx-rtd-theme==1.1.1",
-  "ipython",
+docs = ["mkdocs-material", "mkdocstrings-python"]
+test = [
+  "pint",
+  "lxml",
+  "pytest",
+  "pytest-cov",
+  "xmlschema",
+  "pytest-mypy-plugins",
 ]
-test = ["pytest", "pytest-cov", "xmlschema", "pytest-mypy-plugins"]
 
 # https://hatch.pypa.io/latest/plugins/build-hook/custom/
 [tool.hatch.build.targets.wheel.hooks.custom]
 # requirements to run the autogen script in hatch_build.py
 require-runtime-dependencies = true
 dependencies = ["black", "ruff", "xsdata[cli]>=23.6"]
 
@@ -136,14 +137,15 @@
 
 [tool.check-manifest]
 ignore = [
   "coverage.yml",
   ".pre-commit-config.yaml",
   ".github_changelog_generator",
   ".readthedocs.yml",
+  "mkdocs.yml",
   "docs/**/*",
   "tests/**/*",
   "typesafety/**/*",
 ]
 
 
 [tool.isort]
@@ -201,16 +203,17 @@
   "@overload",
   "except ImportError",
   "\\.\\.\\.",
   "raise NotImplementedError()",
 ]
 
 [tool.coverage.run]
-source = ["src/ome_types", "src/ome_autogen"]
-omit = ["src/ome_types/_autogenerated/*"]
+source = ["ome_types", "ome_autogen"]
+omit = ["src/ome_types/_autogenerated/*", "/private/var/folders/*"]
+
 
 # Entry points -- REMOVE ONCE XSDATA-PYDANTIC-BASEMODEL IS SEPARATE
 [project.entry-points."xsdata.plugins.class_types"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.class_type"
 
 [project.entry-points."xsdata.plugins.cli"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.cli"
```

### Comparing `ome_types-0.4.0a5/PKG-INFO` & `ome_types-0.4.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0a5
+Version: 0.4.0rc1
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -20,32 +20,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
-Requires-Dist: lxml>=4.8.0
-Requires-Dist: pint>=0.15
-Requires-Dist: pydantic[email]<2.0
-Requires-Dist: xsdata
+Requires-Dist: pydantic<2.0
+Requires-Dist: xsdata>=23.5
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-lxml; python_version >= '3.8' and extra == 'dev'
 Requires-Dist: xsdata[cli]>=23.6; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: ipython; extra == 'docs'
-Requires-Dist: numpydoc; extra == 'docs'
-Requires-Dist: pygments; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme==1.1.1; extra == 'docs'
-Requires-Dist: sphinx==5.3.0; extra == 'docs'
+Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: mkdocstrings-python; extra == 'docs'
+Provides-Extra: lxml
+Requires-Dist: lxml>=4.8.0; extra == 'lxml'
+Provides-Extra: pint
+Requires-Dist: pint>=0.15; extra == 'pint'
 Provides-Extra: test
+Requires-Dist: lxml; extra == 'test'
+Requires-Dist: pint; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mypy-plugins; extra == 'test'
 Requires-Dist: xmlschema; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ome-types
@@ -53,46 +54,58 @@
 [![License](https://img.shields.io/github/license/tlambert03/ome-types)](LICENSE)
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
 [![Python
 Version](https://img.shields.io/pypi/pyversions/ome-types.svg)](https://python.org)
 [![Tests](https://github.com/tlambert03/ome-types/workflows/tests/badge.svg)](https://github.com/tlambert03/ome-types/actions)
 [![Docs](https://readthedocs.org/projects/ome-types/badge/?version=latest)](https://ome-types.readthedocs.io/en/latest/?badge=latest)
-<!-- [![conda-forge](https://img.shields.io/conda/vn/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types) -->
+[![codecov](https://codecov.io/gh/tlambert03/ome-types/branch/main/graph/badge.svg?token=GocY9y8A32)](https://codecov.io/gh/tlambert03/ome-types)
 
 ## A pure-python implementation of the OME data model
 
 `ome_types` provides a set of python dataclasses and utility functions for
 parsing the [OME-XML
 format](https://docs.openmicroscopy.org/ome-model/latest/ome-xml/) into
 fully-typed python objects for interactive or programmatic access in python. It
 can also take these python objects and output them into valid OME-XML.
 `ome_types` is a **pure python** library and does not require a Java virtual
 machine.
 
 > Note: The generated python code can be seen in the [`built`
-branch](https://github.com/tlambert03/ome-types/tree/built).
-(Read the [code generation](#code-generation) section for details).
+> branch](https://github.com/tlambert03/ome-types/tree/built).
+> (Read the [code generation](#code-generation) section for details).
 
-### 📖  &nbsp;&nbsp;[documentation](https://ome-types.readthedocs.io/)
+### 📖 &nbsp;&nbsp;[documentation](https://ome-types.readthedocs.io/)
 
 ## Installation
 
 ### from pip
 
 ```shell
 pip install ome-types
 ```
 
-### from source
+With all optional dependencies:
 
 ```shell
-git clone https://github.com/tlambert03/ome-types.git
-cd ome-types
-pip install -e .
+# lxml => if you want to use lxml as the XML parser
+# pint => if you want to use object.<field>_quantity properties
+pip install ome-types[lxml,pint]
+```
+
+### from conda
+
+```shell
+conda install -c conda-forge ome-types
+```
+
+### from github (bleeding edge dev version)
+
+```shell
+pip install git+https://github.com/tlambert03/ome-types.git
 ```
 
 ## Usage
 
 ### convert an XML string or filepath into an instance of `ome_types.model.OME`
 
 (The XML string/file will be validated against the [ome.xsd
@@ -218,15 +231,15 @@
     microscope=Microscope(
        manufacturer='OME Instruments',
        model='Lab Mk4',
        serial_number='L4-5678',
     ),
     objectives=[<1 Objectives>],
  )]
- ```
+```
 
 ### export to an OME-XML string
 
 Finally, you can generate the OME-XML representation of the OME model object,
 for writing to a standalone `.ome.xml` file or inserting into the header of an
 OME-TIFF file:
 
@@ -253,104 +266,61 @@
         </Pixels>
     </Image>
 </OME>
 ```
 
 ## Code generation
 
-The bulk of this library (namely, the `ome_types.model` module) is generated
-at install time, and is therefore not checked into source (or visible in the main
-branch of this repo).
+The bulk of this library (namely, modules inside `ome_types._autogenerated`) is
+generated at install time, and is therefore not checked into source (or visible
+in the main branch of this repo).
 
 You can see the code generated by the main branch in the [built
 branch](https://github.com/tlambert03/ome-types/tree/built)
 
-
-The script at `src/ome_autogen.py` converts the [ome.xsd
+The package at `src/ome_autogen` converts the [ome.xsd
 schema](https://www.openmicroscopy.org/Schemas/OME/2016-06/ome.xsd) into valid
 python code. To run the code generation script in a development environment,
 clone this repository and run:
 
 ```sh
-python src/ome_autogen.py
+python -m src.ome_autogen
 ```
 
-As an example, the
-[`OME/Image`](https://www.openmicroscopy.org/Schemas/Documentation/Generated/OME-2016-06/ome_xsd.html#Image)
-model will be rendered as the following dataclass in `ome_types/model/image.py`
-
-```python
-from datetime import datetime
-from typing import List, Optional
-
-from pydantic import Field
-
-from ome_types._base_type import OMEType
-
-from .annotation_ref import AnnotationRef
-from .experiment_ref import ExperimentRef
-from .experimenter_group_ref import ExperimenterGroupRef
-from .experimenter_ref import ExperimenterRef
-from .imaging_environment import ImagingEnvironment
-from .instrument_ref import InstrumentRef
-from .microbeam_manipulation_ref import MicrobeamManipulationRef
-from .objective_settings import ObjectiveSettings
-from .pixels import Pixels
-from .roi_ref import ROIRef
-from .simple_types import ImageID
-from .stage_label import StageLabel
-
-
-class Image(OMEType):
-    id: ImageID
-    pixels: Pixels
-    acquisition_date: Optional[datetime] = None
-    annotation_ref: List[AnnotationRef] = Field(default_factory=list)
-    description: Optional[str] = None
-    experiment_ref: Optional[ExperimentRef] = None
-    experimenter_group_ref: Optional[ExperimenterGroupRef] = None
-    experimenter_ref: Optional[ExperimenterRef] = None
-    imaging_environment: Optional[ImagingEnvironment] = None
-    instrument_ref: Optional[InstrumentRef] = None
-    microbeam_manipulation_ref: List[MicrobeamManipulationRef] = Field(
-        default_factory=list
-    )
-    name: Optional[str] = None
-    objective_settings: Optional[ObjectiveSettings] = None
-    roi_ref: List[ROIRef] = Field(default_factory=list)
-    stage_label: Optional[StageLabel] = None
-```
 
 The documentation and types for the full model can be in the [API Reference](https://ome-types.readthedocs.io/en/latest/ome_types.model.html)
 
 ## Contributing
 
-To clone and install this repository locally (this will also build the model at
-`src/ome_types/model`)
+To clone and install this repository locally:
 
 ```shell
 git clone https://github.com/tlambert03/ome-types.git
 cd ome-types
-pip install -e .[autogen]
+pip install -e .[test,dev]
 ```
 
-We use `pre-commit` to run various code-quality checks (isort, black, mypy,
-flake8) during continuous integration.  If you'd like to make sure that your
-code will pass these checks before you commit your code, you should install
-`pre-commit` after cloning this repository:
+We use `pre-commit` to run various code-quality checks  during continuous
+integration. If you'd like to make sure that your code will pass these checks
+before you commit your code, you should install `pre-commit` after cloning this
+repository:
 
 ```shell
-pip install pre-commit
 pre-commit install
 ```
 
-If you modify `src/ome_autogen.py`, you may need to regenerate the model with:
+### regenerating the models
+
+If you modify anything in `src/ome_autogen`, you may need to
+regenerate the model with:
 
 ```shell
-python src/ome_autogen.py
+python -m src.ome_autogen
 ```
 
 ### Running tests
 
-To run tests quickly, just install and run `pytest`.  Note, however, that this
-requires that the `ome_types.model` module has already been built with `python
-src/ome_autogen.py`.
+To run tests:
+
+```
+pytest
+```
```

