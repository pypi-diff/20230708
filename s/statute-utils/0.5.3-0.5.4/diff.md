# Comparing `tmp/statute_utils-0.5.3.tar.gz` & `tmp/statute_utils-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.3.tar", max compression
+gzip compressed data, was "statute_utils-0.5.4.tar", max compression
```

## Comparing `statute_utils-0.5.3.tar` & `statute_utils-0.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.3/LICENSE
--rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.3/README.md
--rw-r--r--   0        0        0     1380 2023-07-01 12:33:52.669248 statute_utils-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      457 2023-07-01 06:23:31.949055 statute_utils-0.5.3/statute_utils/__init__.py
--rw-r--r--   0        0        0      275 2023-07-01 05:31:15.495445 statute_utils-0.5.3/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     8971 2023-07-01 07:26:53.216138 statute_utils-0.5.3/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.3/statute_utils/components/short.py
--rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.3/statute_utils/components/utils.py
--rw-r--r--   0        0        0    10136 2023-07-01 12:36:21.497674 statute_utils-0.5.3/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-01 06:44:19.410593 statute_utils-0.5.3/statute_utils/models.py
--rw-r--r--   0        0        0     9880 2023-07-01 07:26:41.687325 statute_utils-0.5.3/statute_utils/models_names.py
--rw-r--r--   0        0        0     6682 2023-07-01 06:21:01.765608 statute_utils-0.5.3/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.3/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.3/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.3/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.3/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.3/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     4709 2023-07-01 06:20:32.418706 statute_utils-0.5.3/statute_utils/tree.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.4/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.4/README.md
+-rw-r--r--   0        0        0     1380 2023-07-08 02:35:12.669952 statute_utils-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      505 2023-07-08 03:56:43.843992 statute_utils-0.5.4/statute_utils/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-08 03:56:36.059597 statute_utils-0.5.4/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0    10002 2023-07-08 02:39:06.841639 statute_utils-0.5.4/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.4/statute_utils/components/short.py
+-rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.4/statute_utils/components/utils.py
+-rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.4/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.4/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.4/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.4/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.4/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.4/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.4/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.4/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.4/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6098 2023-07-08 04:17:18.808301 statute_utils-0.5.4/statute_utils/tree.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.4/PKG-INFO
```

### Comparing `statute_utils-0.5.3/LICENSE` & `statute_utils-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.3/README.md` & `statute_utils-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.3/pyproject.toml` & `statute_utils-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.3"
+version = "0.5.4"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.5.3/statute_utils/components/category.py` & `statute_utils-0.5.4/statute_utils/components/category.py`

 * *Files 15% similar despite different names*

```diff
@@ -124,14 +124,36 @@
             'ra'
 
         Returns:
             str: The value of the Enum member
         """
         return str.__repr__(self.value)
 
+    @classmethod
+    def shorten(cls, text: str):
+        """Replace the item's long form keyword with its shorthand format, if
+        possible."""
+        if "Republic Act" in text:
+            return re.sub(r"Republic\s+Act\s+No\.", "RA", text)
+        if "Presidential Decree" in text:
+            return re.sub(r"Presidential\s+Decree\s+No\.", "PD", text)
+        if "Batas Pambansa" in text:
+            return re.sub(r"Batas\s+Pambansa\s+Blg\.", "BP", text)
+        if "Executive Order" in text:
+            return re.sub(r"Executive\s+Order\s+No\.", "EO", text)
+        if "Commonwealth Act" in text:
+            return re.sub(r"Commonwealth\s+Act\s+No\.", "CA", text)
+        if "Administrative Matter" in text:
+            return re.sub(r"Administrative\s+Matter\s+No\.", "AM", text)
+        if "Bar Matter" in text:
+            return re.sub(r"Bar\s+Matter\s+No\.", "BM", text)
+        if "Administrative Circular" in text:
+            return re.sub(r"Administrative\s+Circular\s+No\.", "AC", text)
+        return text
+
     def serialize(self, idx: str) -> str | None:
         """Given a member item and a valid serialized identifier, create a serial title.
 
         Note that the identifier must be upper-cased to make this consistent
         with the textual convention, e.g.
 
         Examples:
```

### Comparing `statute_utils-0.5.3/statute_utils/components/short.py` & `statute_utils-0.5.4/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.3/statute_utils/main.py` & `statute_utils-0.5.4/statute_utils/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 from collections import Counter
 from collections.abc import Iterator
 from operator import attrgetter
 from typing import NamedTuple, Self
 
 from .components import StatuteSerialCategory
 from .models import NamedPattern, Rule, SerialPattern
-from .models_names import NAMED_COLLECTION
-from .models_serials import SERIAL_COLLECTION
+from .models_names import STYLES_NAMED
+from .models_serials import STYLES_SERIAL
 from .recipes import split_digits
 
 
-def create_pattern(collection: list[SerialPattern] | list[NamedPattern]) -> re.Pattern:
-    return re.compile("|".join([style.regex for style in collection]), re.X)
+def create_single_pattern_styles(
+    styles: list[SerialPattern] | list[NamedPattern],
+) -> re.Pattern:
+    """Regex strings from either a `SerialPattern` list or a `NamedPattern` list are
+    combined into a single regex string so that `finditer()` can used."""  # noqa: E501
+    return re.compile("|".join([style.regex for style in styles]), re.X)
 
 
-COLLECTED_SERIALS = create_pattern(collection=SERIAL_COLLECTION)
-"""Each serial regex string is combined into a single regex string so that `finditer()` can used."""  # noqa: E501
-COLLECTED_NAMES = create_pattern(collection=NAMED_COLLECTION)
-"""Each named regex string is combined into a single regex string so that `finditer()` can used."""  # noqa: E501
+SERIALS = create_single_pattern_styles(styles=STYLES_SERIAL)
+"""All of the Serial Pattern objects combined into a single pattern object."""
+
+NAMES = create_single_pattern_styles(styles=STYLES_NAMED)
+"""All of the Named Pattern objects combined into a single pattern object."""
 
 
 def extract_serial_rules(text: str) -> Iterator[Rule]:
     """Each `m`, a python Match object, represents a
     serial pattern category with possible ambiguous identifier found.
 
     So running `m.group(0)` should yield the entire text of the
@@ -34,16 +39,16 @@
     The identifier is ambiguous because it may be a compound one,
     e.g. 'Presidential Decree No. 1 and 2'. In this case, there
     should be 2 matches produced not just one.
 
     This function splits the identifier by commas `,` and the
     word `and` to get the individual component identifiers.
     """
-    for match in COLLECTED_SERIALS.finditer(text):
-        for style in SERIAL_COLLECTION:
+    for match in SERIALS.finditer(text):
+        for style in STYLES_SERIAL:
             if match.lastgroup == style.group_name:
                 if candidates := style.digits_in_match.search(match.group(0)):
                     for d in split_digits(candidates.group(0)):
                         yield Rule(cat=style.cat, num=d.lower())
 
 
 def extract_named_rules(
@@ -55,16 +60,16 @@
     Args:
         text (str): The text to extract named patterns from.
         document_date (datetime.date | None, optional): When present, will use the `named.options`. Defaults to None.
 
     Yields:
         Iterator[Rule]: The applicable rule found
     """  # noqa: E501
-    for m in COLLECTED_NAMES.finditer(text):
-        for named in NAMED_COLLECTION:
+    for m in NAMES.finditer(text):
+        for named in STYLES_NAMED:
             if m.lastgroup == named.group_name:
                 if named.options and document_date:
                     # sorts the options in descending order
                     options = sorted(
                         named.options, key=attrgetter("date"), reverse=True
                     )
                     for option in options:
```

### Comparing `statute_utils-0.5.3/statute_utils/models.py` & `statute_utils-0.5.4/statute_utils/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         return StatuteSerialCategory(self.cat.value).serialize(self.num)
 
     @cached_property
     def date(self) -> datetime.date | None:
         try:
             date_str = STATUTE_DB.execute_returning_dicts(
                 """--sql
-                    select max(s.date) max_date
+                    select min(s.date) min_date
                     from statutes s
                     where s.cat = :cat and s.num = :num
                     group by s.cat, s.num;
                     """,
                 params={"cat": self.cat.value.lower(), "num": self.num.lower()},
-            )[0]["max_date"]
+            )[0]["min_date"]
             return datetime.date.fromisoformat(date_str)
         except Exception:
             return None
 
 
 class NamedPattern(NamedTuple):
     name: str
```

### Comparing `statute_utils-0.5.3/statute_utils/models_names.py` & `statute_utils-0.5.4/statute_utils/models_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,15 +392,15 @@
                 \\s+
                 and
                 \\s+
                 Accountability|ACCOUNTABILITY
             )?
 """
 
-NAMED_COLLECTION = [
+STYLES_NAMED: list[NamedPattern] = [
     admin,
     civ,
     rpc,
     corp,
     labor,
     locgov,
     prof_responsibility,
@@ -408,12 +408,12 @@
     roc,
     tax,
     insurance,
     election,
     cooperative,
 ] + spain_codes
 """
-Each named legal title, not falling under `SERIAL_COLLECTION`,
+Each named legal title, not falling under `STYLES_SERIAL`,
 will also have its own manually crafted regex string. Examples include
 'the Spanish Civil Code' or the '1987 Constitution' or the
 'Code of Professional Responsibility'.
 """
```

### Comparing `statute_utils-0.5.3/statute_utils/models_serials.py` & `statute_utils-0.5.4/statute_utils/models_serials.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     regex_serials=[r"10-15-1991"],
     matches=["Resolution of the Court En Banc dated 10-15-1991"],
 )
 """
 ## Resolution of the Court Rule Pattern
 """
 
-SERIAL_COLLECTION = [
+STYLES_SERIAL: list[SerialPattern] = [
     ra,
     ca,
     act,
     eo,
     pd,
     bp,
     loi,
```

### Comparing `statute_utils-0.5.3/statute_utils/recipes/digits.py` & `statute_utils-0.5.4/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.3/statute_utils/recipes/spain.py` & `statute_utils-0.5.4/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.3/statute_utils/tree.py` & `statute_utils-0.5.4/statute_utils/tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import datetime
 from collections.abc import Iterator
+from copy import deepcopy
 from pathlib import Path
-from typing import NamedTuple
+from typing import Any, NamedTuple
 
 import yaml
 
-from .components import StatuteSerialCategory, StatuteTitle, set_node_ids, walk
+from .components import (
+    StatuteSerialCategory,
+    StatuteTitle,
+    create_fts_snippet_column,
+    create_unit_heading,
+    set_node_ids,
+    walk,
+)
 from .models import STATUTE_DIR, Rule
 
 
 class Statute(NamedTuple):
     """A instance is dependent on a statute path from a fixed
     `STATUTE_DIR`. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
@@ -57,21 +65,48 @@
         set_node_ids(self.units)
         return {
             "id": self.slug,
             "cat": self.rule.cat.value,
             "num": self.rule.num,
             "date": self.date,
             "variant": self.variant,
-            "units": [{"num": "1.", "units": self.units}],
+            "units": [{"id": "1.", "units": self.units}],
         }
 
+    @classmethod
+    def flatten_units(
+        cls, statute_id: str, units: list[dict[str, Any]], heading: str = ""
+    ) -> Iterator[dict[str, str | None]]:
+        """Recursive flattening of tree structure where each material path
+        gets its own item, caption, and content fields with extracted heading / snippetable
+        columns from such fields. Use cases:
+
+        1. Material path with individual fields reconstructs subtrees
+        2. Snippetable column becomes a searchable FTS summary of caption + content
+        3. Heading column makes identifable the subtree involved with item + caption
+
+        """  # noqa: E501
+        for unit in units:
+            present_heading = create_unit_heading(unit, heading)
+            yield {
+                "statute_id": statute_id,
+                "material_path": unit["id"],  # enable subtree
+                "heading": present_heading,  # identify subtree
+                "item": unit.get("item"),
+                "caption": unit.get("caption"),
+                "content": unit.get("content"),
+                "snippetable": create_fts_snippet_column(unit),  # enable searchability
+            }
+            if subunits := unit.get("units"):
+                yield from cls.flatten_units(statute_id, subunits, present_heading)
+
     def to_file(self) -> Path:
-        """Orders the different key, value pairs for a yaml dump operation.
-        Ensures that each node in the tree is properly (rather than alphabetically)
-        ordered."""
+        """Orders different key, value pairs for a yaml dump operation.
+        Ensures each node in the tree is properly (rather than alphabetically) ordered.
+        """
         f = STATUTE_DIR.joinpath(self.__repr__())
         f.parent.mkdir(parents=True, exist_ok=True)
         data: dict = self._asdict()
         data["units"] = walk(data["units"])
         text = yaml.dump(data, width=60)  # see representer added in walk
         f.write_text(text)
         return f
```

### Comparing `statute_utils-0.5.3/PKG-INFO` & `statute_utils-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.5.3
+Version: 0.5.4
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

