# Comparing `tmp/nl2ltl-0.0.3.tar.gz` & `tmp/nl2ltl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl2ltl-0.0.3.tar", last modified: Tue Jun 13 20:18:16 2023, max compression
+gzip compressed data, was "nl2ltl-0.0.4.tar", last modified: Fri Jul  7 22:02:11 2023, max compression
```

## Comparing `nl2ltl-0.0.3.tar` & `nl2ltl-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.392397 nl2ltl-0.0.3/nl2ltl/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl/declare/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/engines/gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/grounding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/engines/rasa/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/simple_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/filters/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/subsumptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/tests/test_gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/tests/test_rasa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.903442 nl2ltl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-07 22:02:11.903442 nl2ltl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.891441 nl2ltl-0.0.4/nl2ltl/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.895441 nl2ltl-0.0.4/nl2ltl/declare/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/declare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/declare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/declare/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/declare/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.895441 nl2ltl-0.0.4/nl2ltl/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.899442 nl2ltl-0.0.4/nl2ltl/engines/gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/gpt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/gpt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/grounding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.899442 nl2ltl-0.0.4/nl2ltl/engines/rasa/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/rasa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/rasa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-07 22:02:01.000000 nl2ltl-0.0.4/nl2ltl/engines/rasa/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/engines/rasa/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.899442 nl2ltl-0.0.4/nl2ltl/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/simple_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.899442 nl2ltl-0.0.4/nl2ltl/filters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/utils/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/nl2ltl/filters/utils/subsumptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.895441 nl2ltl-0.0.4/nl2ltl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 22:02:11.000000 nl2ltl-0.0.4/nl2ltl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 22:02:11.903442 nl2ltl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:02:11.903442 nl2ltl-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/tests/test_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 22:02:02.000000 nl2ltl-0.0.4/tests/test_rasa.py
```

### Comparing `nl2ltl-0.0.3/LICENSE` & `nl2ltl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/PKG-INFO` & `nl2ltl-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nl2ltl
-Version: 0.0.3
+Version: 0.0.4
 Summary: From Natural Language to Linear-time Temporal Logic
 Author: Tathagata Chakraborti, Francesco Fuggitti
 Author-email: tathagata.chakraborti1@ibm.com, francesco.fuggitti@ibm.com
 License: MIT
 Keywords: natural language nlu ltl temporal logic
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
@@ -164,14 +164,25 @@
   title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
   booktitle    = {{AAAI}},
   year         = {2023},
   note         = {System Demonstration.},
   url_code     = {https://github.com/IBM/nl2ltl},
 }
 ```
+and
+```
+@inproceedings{icaps2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{ICAPS}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
 
 
 MIT License
 
 Copyright (c) 2022 International Business Machines
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nl2ltl-0.0.3/README.md` & `nl2ltl-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -140,8 +140,19 @@
   title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
   booktitle    = {{AAAI}},
   year         = {2023},
   note         = {System Demonstration.},
   url_code     = {https://github.com/IBM/nl2ltl},
 }
 ```
+and
+```
+@inproceedings{icaps2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{ICAPS}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
```

### Comparing `nl2ltl-0.0.3/nl2ltl/core.py` & `nl2ltl-0.0.4/nl2ltl/core.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/declare/base.py` & `nl2ltl-0.0.4/nl2ltl/declare/base.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/declare/declare.py` & `nl2ltl-0.0.4/nl2ltl/declare/declare.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def to_ltlf(self) -> Formula:
         """Translate Response to LTLf."""
         return Always(Implies(self.operands[0], Eventually(self.operands[1])))
 
     def to_english(self) -> str:
         """English meaning."""
         return (
-            f"Whenever activity {self.operands[0]} happens, activity {self.operands[1]} has to happen "
+            f"Whenever  {self.operands[0]} happens,  {self.operands[1]} has to happen "
             f"eventually afterward."
         )
 
     def to_ppltl(self) -> Formula:
         """Translate Response to PPLTL."""
         return Not(
             Since(Not(self.operands[1]), And(self.operands[0], Not(self.operands[1])))
@@ -148,15 +148,15 @@
             Until(Not(self.operands[1]), self.operands[0]),
             Always(Not(self.operands[1])),
         )
 
     def to_english(self) -> str:
         """English meaning."""
         return (
-            f"Whenever activity {self.operands[1]} happens, activity {self.operands[0]} has to have happened "
+            f"Whenever  {self.operands[1]} happens,  {self.operands[0]} has to have happened "
             f"before it."
         )
 
     def to_ppltl(self) -> Formula:
         """Translate Precedence to PPLTL."""
         return Or(
             Once(
@@ -182,16 +182,16 @@
     def to_ltlf(self) -> Formula:
         """Translate ChainResponse to LTLf."""
         return Always(Implies(self.operands[0], Next(self.operands[1])))
 
     def to_english(self) -> str:
         """English meaning."""
         return (
-            f"Every time activity {self.operands[0]} happens, it must be directly followed by activity "
-            f"{self.operands[1]} (activity {self.operands[1]} can also follow other activities)."
+            f"Every time  {self.operands[0]} happens, it must be directly followed by  "
+            f"{self.operands[1]} ( {self.operands[1]} can also follow other activities)."
         )
 
     def to_ppltl(self) -> Formula:
         """Translate ChainResponse to PPLTL."""
         return And(
             Historically(Implies(Before(self.operands[0]), self.operands[1])),
             Not(self.operands[0]),
@@ -210,12 +210,12 @@
 
     def to_ltlf(self) -> Formula:
         """Translate NotCoExistence to LTLf."""
         return Implies(Eventually(self.operands[0]), Not(Eventually(self.operands[1])))
 
     def to_english(self) -> str:
         """English meaning."""
-        return f"Either activity {self.operands[0]} or {self.operands[1]} can happen, but not both."
+        return f"Either  {self.operands[0]} or {self.operands[1]} can happen, but not both."
 
     def to_ppltl(self) -> Formula:
         """Translate NotCoExistence to PPLTL."""
         return Implies(Once(self.operands[0]), Not(Once(self.operands[1])))
```

### Comparing `nl2ltl-0.0.3/nl2ltl/declare/misc.py` & `nl2ltl-0.0.4/nl2ltl/declare/misc.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/base.py` & `nl2ltl-0.0.4/nl2ltl/engines/base.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/gpt/core.py` & `nl2ltl-0.0.4/nl2ltl/engines/gpt/core.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/gpt/output.py` & `nl2ltl-0.0.4/nl2ltl/engines/gpt/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 @dataclass
 class GPTOutput:
     """Dataclass to represent the GPT output."""
 
     pattern: str
-    entities: Tuple[str]
+    entities: Tuple[str, ...]
 
     def __post_init__(self):
         """Do consistency checks after initialization."""
         assert self.pattern is not None
         assert self.entities is not None
```

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/grounding.py` & `nl2ltl-0.0.4/nl2ltl/engines/grounding.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,115 +13,121 @@
     Existence,
     ExistenceTwo,
     NotCoExistence,
     Precedence,
     RespondedExistence,
     Response,
 )
+from nl2ltl.engines.utils import decapitalize
 
 
 def ground_existence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Existence."""
     if len(list(connectors)) > 0:
-        return {Existence(Atomic(list(connectors)[0].lower()))}
+        return {Existence(Atomic(decapitalize(list(connectors)[0])))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate Existence with < 1 connectors."
         )
         return set()
 
 
 def ground_existencetwo(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for ExistenceTwo."""
     if len(list(connectors)) > 0:
-        return {ExistenceTwo(Atomic(list(connectors)[0].lower()))}
+        return {ExistenceTwo(Atomic(decapitalize(list(connectors)[0])))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate ExistenceTwo with < 1 connectors."
         )
         return set()
 
 
 def ground_absence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Absence."""
     if len(list(connectors)) > 0:
-        return {Absence(Atomic(list(connectors)[0].lower()))}
+        return {Absence(Atomic(decapitalize(list(connectors)[0])))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate Absence with < 1 connectors."
         )
         return set()
 
 
 def ground_respondedexistence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for RespondedExistence."""
     if len(list(connectors)) >= 2:
         return {
             RespondedExistence(
-                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+                Atomic(decapitalize(list(connectors)[0])),
+                Atomic(decapitalize(list(connectors)[1])),
             )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate RespondedExistence with < 2 connectors."
         )
         return set()
 
 
 def ground_response(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Response."""
     if len(list(connectors)) >= 2:
         return {
             Response(
-                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+                Atomic(decapitalize(list(connectors)[0])),
+                Atomic(decapitalize(list(connectors)[1])),
             )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate Response with < 2 connectors."
         )
         return set()
 
 
 def ground_precedence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Precedence."""
     if len(list(connectors)) >= 2:
         return {
             Precedence(
-                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+                Atomic(decapitalize(list(connectors)[0])),
+                Atomic(decapitalize(list(connectors)[1])),
             )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate Precedence with < 2 connectors."
         )
         return set()
 
 
 def ground_chainresponse(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for ChainResponse."""
     if len(list(connectors)) >= 2:
         return {
             ChainResponse(
-                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+                Atomic(decapitalize(list(connectors)[0])),
+                Atomic(decapitalize(list(connectors)[1])),
             )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate ChainResponse with < 2 connectors."
         )
         return set()
 
 
 def ground_notcoexistence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for NotCoExistence."""
     if len(list(connectors)) >= 2:
         return {
             NotCoExistence(
-                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+                Atomic(decapitalize(list(connectors)[1])),
+                Atomic(decapitalize(list(connectors)[1])),
             )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate NotCoExistence with < 2 connectors."
         )
         return set()
```

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/rasa/core.py` & `nl2ltl-0.0.4/nl2ltl/engines/rasa/core.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/rasa/output.py` & `nl2ltl-0.0.4/nl2ltl/engines/rasa/output.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/engines/utils.py` & `nl2ltl-0.0.4/nl2ltl/engines/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Engines utils."""
 import difflib
-from typing import Callable, Dict, Set
+from typing import Callable, Dict, Set, Union
 
-from pylogics.syntax.base import Formula
+from pylogics.syntax.base import AtomName, Formula
 
 from nl2ltl.declare.base import TemplateEnum
 
 
 def _get_formulas(name: str, args: Dict[str, float]) -> Set[Formula]:
     """Instantiate matching formulas based on intent name and entities."""
     import nl2ltl.declare.declare
@@ -43,7 +43,12 @@
 
     This function is useful to avoid the use of the built-in assert statement, which is removed
         when the code is compiled in optimized mode. For more information, see
         https://bandit.readthedocs.io/en/1.7.5/plugins/b101_assert_used.html
     """
     if not condition:
         raise AssertionError(message)
+
+
+def decapitalize(s: Union[str, AtomName]) -> str:
+    """Decapitalize a string."""
+    return s[:1].lower() + s[1:] if s else ""
```

### Comparing `nl2ltl-0.0.3/nl2ltl/exceptions.py` & `nl2ltl-0.0.4/nl2ltl/exceptions.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/filters/simple_filters.py` & `nl2ltl-0.0.4/nl2ltl/filters/simple_filters.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/filters/utils/conflicts.py` & `nl2ltl-0.0.4/nl2ltl/filters/utils/conflicts.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl/filters/utils/subsumptions.py` & `nl2ltl-0.0.4/nl2ltl/filters/utils/subsumptions.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/nl2ltl.egg-info/PKG-INFO` & `nl2ltl-0.0.4/nl2ltl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nl2ltl
-Version: 0.0.3
+Version: 0.0.4
 Summary: From Natural Language to Linear-time Temporal Logic
 Author: Tathagata Chakraborti, Francesco Fuggitti
 Author-email: tathagata.chakraborti1@ibm.com, francesco.fuggitti@ibm.com
 License: MIT
 Keywords: natural language nlu ltl temporal logic
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
@@ -164,14 +164,25 @@
   title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
   booktitle    = {{AAAI}},
   year         = {2023},
   note         = {System Demonstration.},
   url_code     = {https://github.com/IBM/nl2ltl},
 }
 ```
+and
+```
+@inproceedings{icaps2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{ICAPS}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
 
 
 MIT License
 
 Copyright (c) 2022 International Business Machines
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nl2ltl-0.0.3/nl2ltl.egg-info/SOURCES.txt` & `nl2ltl-0.0.4/nl2ltl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/setup.cfg` & `nl2ltl-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/tests/test_gpt.py` & `nl2ltl-0.0.4/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.3/tests/test_rasa.py` & `nl2ltl-0.0.4/tests/test_rasa.py`

 * *Files identical despite different names*

