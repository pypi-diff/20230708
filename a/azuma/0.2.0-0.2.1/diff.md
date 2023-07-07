# Comparing `tmp/azuma-0.2.0.tar.gz` & `tmp/azuma-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuma-0.2.0.tar", max compression
+gzip compressed data, was "azuma-0.2.1.tar", max compression
```

## Comparing `azuma-0.2.0.tar` & `azuma-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-06-24 05:28:08.865208 azuma-0.2.0/LICENSE
--rw-r--r--   0        0        0      560 2023-06-24 05:28:08.865208 azuma-0.2.0/README.md
--rw-r--r--   0        0        0      128 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/__init__.py
--rw-r--r--   0        0        0     1483 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/cli.py
--rw-r--r--   0        0        0      212 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/exceptions.py
--rw-r--r--   0        0        0     5226 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/matchers.py
--rw-r--r--   0        0        0      129 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/parsers/__init__.py
--rw-r--r--   0        0        0     4631 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/parsers/condition.py
--rw-r--r--   0        0        0     5337 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/parsers/detection.py
--rw-r--r--   0        0        0      144 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/__init__.py
--rw-r--r--   0        0        0     1860 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/detection.py
--rw-r--r--   0        0        0      256 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/log_source.py
--rw-r--r--   0        0        0      206 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/related.py
--rw-r--r--   0        0        0     4027 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/rule.py
--rw-r--r--   0        0        0     1098 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/rule_set.py
--rw-r--r--   0        0        0     1956 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/schemas/yaml_model.py
--rw-r--r--   0        0        0      318 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/types.py
--rw-r--r--   0        0        0      638 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/utils.py
--rw-r--r--   0        0        0      182 2023-06-24 05:28:08.865208 azuma-0.2.0/azuma/validators.py
--rw-r--r--   0        0        0     1351 2023-06-24 05:28:27.237481 azuma-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 azuma-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-07 23:02:32.195212 azuma-0.2.1/LICENSE
+-rw-r--r--   0        0        0      560 2023-07-07 23:02:32.195212 azuma-0.2.1/README.md
+-rw-r--r--   0        0        0      128 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/cli.py
+-rw-r--r--   0        0        0      212 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/exceptions.py
+-rw-r--r--   0        0        0      952 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/grammar.lark
+-rw-r--r--   0        0        0     5226 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/matchers.py
+-rw-r--r--   0        0        0      129 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/__init__.py
+-rw-r--r--   0        0        0     3452 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/condition.py
+-rw-r--r--   0        0        0     5451 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/detection.py
+-rw-r--r--   0        0        0      144 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/__init__.py
+-rw-r--r--   0        0        0     1882 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/detection.py
+-rw-r--r--   0        0        0      256 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/log_source.py
+-rw-r--r--   0        0        0      206 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/related.py
+-rw-r--r--   0        0        0     3937 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/rule.py
+-rw-r--r--   0        0        0     1098 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/rule_set.py
+-rw-r--r--   0        0        0     1249 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/yaml_model.py
+-rw-r--r--   0        0        0      318 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/types.py
+-rw-r--r--   0        0        0      638 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/utils.py
+-rw-r--r--   0        0        0      182 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/validators.py
+-rw-r--r--   0        0        0     1351 2023-07-07 23:02:52.367235 azuma-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 azuma-0.2.1/PKG-INFO
```

### Comparing `azuma-0.2.0/LICENSE` & `azuma-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/README.md` & `azuma-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/azuma/cli.py` & `azuma-0.2.1/azuma/cli.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/azuma/matchers.py` & `azuma-0.2.1/azuma/matchers.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/azuma/parsers/detection.py` & `azuma-0.2.1/azuma/parsers/detection.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,39 +67,52 @@
         match = UPTO_WILDCARD.match(value)
 
         if match:
             # The non regex content in the sigma string, may have characters special to regex
             matched = match.group(0)
             full_content.append(re.escape(matched))
             value = value[len(matched) :]
-        elif value.startswith("*"):
+            continue
+
+        if value.startswith("*"):
             full_content.append(".*")
             value = value[1:]
-        elif value.startswith("\\*"):
+            continue
+
+        if value.startswith("\\*"):
             full_content.append(re.escape("*"))
             value = value[2:]
-        elif value.startswith("?"):
+            continue
+
+        if value.startswith("?"):
             full_content.append(".")
             value = value[1:]
-        elif value.startswith("\\?"):
+            continue
+
+        if value.startswith("\\?"):
             full_content.append(re.escape("?"))
             value = value[2:]
-        elif value.startswith(r"\\*"):
+            continue
+
+        if value.startswith(r"\\*"):
             full_content.append(re.escape("\\") + ".*")
             value = value[3:]
-        elif value.startswith(r"\\?"):
+            continue
+
+        if value.startswith(r"\\?"):
             full_content.append(re.escape("\\") + ".")
             value = value[3:]
-        elif value.startswith("\\"):
+            continue
+
+        if value.startswith("\\"):
             full_content.append(re.escape("\\"))
             value = value[1:]
-        else:
-            raise ValueError(
-                f"Could not parse string matching pattern: {original_value}"
-            )
+            continue
+
+        raise ValueError(f"Could not parse string matching pattern: {original_value}")
 
     return "".join(full_content)  # Sigma strings are case insensitive
 
 
 def get_modified_value(value: str, modifiers: list[str] | None) -> str:
     if not modifiers:
         # If there are no modifiers, we assume exact match
```

### Comparing `azuma-0.2.0/azuma/schemas/detection.py` & `azuma-0.2.1/azuma/schemas/detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from pydantic import BaseModel, Field, root_validator
+from pydantic import BaseModel, Field, model_validator
 
 from azuma import types
 from azuma.parsers import apply_modifiers, normalize_field_map, prepare_condition
 
 
 class DetectionField(BaseModel):
     list_search: list[types.Query] = Field(default_factory=list)
@@ -31,24 +31,23 @@
 
 
 class Detection(BaseModel):
     detection: dict[str, DetectionField] = Field(...)
     timeframe: str | None = Field(default=None)
     condition: types.Condition = Field(...)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def transform(cls, values: Any):
         timeframe: str | None = None
         if "timeframe" in values:
             timeframe = values.pop("timeframe")
 
         condition = prepare_condition(values.pop("condition"))
-
         detection = normalize_detection(values)
-
         return {"condition": condition, "detection": detection, "timeframe": timeframe}
 
     def get_search_fields(self, search_id: str) -> DetectionField | None:
         return self.detection.get(search_id)
 
     @property
     def all_searches(self) -> dict[str, DetectionField]:
```

### Comparing `azuma-0.2.0/azuma/schemas/rule.py` & `azuma-0.2.1/azuma/schemas/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Literal
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 
 from azuma.validators import is_valid_date_format
 
 from .detection import Detection
 from .log_source import LogSource
 from .related import Related
 from .yaml_model import YAMLBaseModel
@@ -72,19 +72,16 @@
     fields: list[str] | None = Field(
         default=None,
         description="A list of log fields that could be interesting in further analysis of the event and should be displayed to the analyst.",
     )
 
     related: list[Related] | None = Field(default=None)
 
-    @validator("detection", pre=True)
-    def transform_detection(cls, v: Any):
-        return Detection.parse_obj(v)
-
-    @validator("date", "modified")
+    @field_validator("date", "modified")
+    @classmethod
     def validate_date_format(cls, v: str | None):
         if v is None:
             return v
 
         if not is_valid_date_format(v):
             raise ValueError("Use YYYY/MM/DD format")
```

### Comparing `azuma-0.2.0/azuma/schemas/rule_set.py` & `azuma-0.2.1/azuma/schemas/rule_set.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/azuma/utils.py` & `azuma-0.2.1/azuma/utils.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.0/pyproject.toml` & `azuma-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "azuma"
-version = "0.2.0"
+version = "0.2.1"
 description = "Yet another Sigma library for Python"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ninoseki/azuma"
 repository = "https://github.com/ninoseki/azuma"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 lark-parser = ">=0.12,<1.0"
 loguru = ">=0.7,<1.0"
-pydantic = ">=1.8,<2.0"
+pydantic = ">=2.0,<3.0"
 pyyaml = ">=6.0,<7.0"
 regex = ">=2022"
 typer = ">=0.9,<1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
 ci-py = "^1.0.0"
```

### Comparing `azuma-0.2.0/PKG-INFO` & `azuma-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: azuma
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yet another Sigma library for Python
 Home-page: https://github.com/ninoseki/azuma
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lark-parser (>=0.12,<1.0)
 Requires-Dist: loguru (>=0.7,<1.0)
-Requires-Dist: pydantic (>=1.8,<2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: regex (>=2022)
 Requires-Dist: typer (>=0.9,<1.0)
 Project-URL: Repository, https://github.com/ninoseki/azuma
 Description-Content-Type: text/markdown
 
 # azuma
```

