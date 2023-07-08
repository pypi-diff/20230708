# Comparing `tmp/mathpad-2.0.1.tar.gz` & `tmp/mathpad-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpad-2.0.1.tar", max compression
+gzip compressed data, was "mathpad-2.1.0.tar", max compression
```

## Comparing `mathpad-2.0.1.tar` & `mathpad-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1095 2023-07-02 13:23:36.640679 mathpad-2.0.1/LICENSE
--rw-r--r--   0        0        0     6921 2023-07-02 13:23:36.640679 mathpad-2.0.1/README.md
--rw-r--r--   0        0        0      826 2023-07-02 13:23:38.324701 mathpad-2.0.1/mathpad/__init__.py
--rw-r--r--   0        0        0      435 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/_global_options.py
--rw-r--r--   0        0        0     2045 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/codegen.py
--rw-r--r--   0        0        0      449 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/__init__.py
--rw-r--r--   0        0        0     2424 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/_generate_units_py.py
--rw-r--r--   0        0        0      786 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/common_vals.py
--rw-r--r--   0        0        0     6352 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/dimensions.py
--rw-r--r--   0        0        0     5489 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/equation.py
--rw-r--r--   0        0        0     8319 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/frame.py
--rw-r--r--   0        0        0    12173 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/matrix.py
--rw-r--r--   0        0        0    11562 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/units.py
--rw-r--r--   0        0        0    18813 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/val.py
--rw-r--r--   0        0        0    13291 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/vector.py
--rw-r--r--   0        0        0     7775 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/core/vector_space.py
--rw-r--r--   0        0        0      950 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/library/constants.py
--rw-r--r--   0        0        0     1913 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/library/electrical.py
--rw-r--r--   0        0        0     2282 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/library/mathpad_constructor.py
--rw-r--r--   0        0        0     1878 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/library/mechanic.py
--rw-r--r--   0        0        0      730 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/library/trigonometry.py
--rw-r--r--   0        0        0      266 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/__init__.py
--rw-r--r--   0        0        0     3930 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/algebra.py
--rw-r--r--   0        0        0     3411 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/calculus.py
--rw-r--r--   0        0        0     1229 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/functions.py
--rw-r--r--   0        0        0     3409 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/solve.py
--rw-r--r--   0        0        0      414 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/maths/trigonometry.py
--rw-r--r--   0        0        0     9648 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/simulate_dynamic_system.py
--rw-r--r--   0        0        0    12032 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/SymbolicMatrixFunction.py
--rw-r--r--   0        0        0      284 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/__init__.py
--rw-r--r--   0        0        0      267 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch.py
--rw-r--r--   0        0        0     1756 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_ArrayDerivative___len__and__iter__.py
--rw-r--r--   0        0        0      924 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_MatrixOperations_subs.py
--rw-r--r--   0        0        0     1522 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_VectorLatexPrinter_print_Derivative.py
--rw-r--r--   0        0        0        0 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/viz/viz2d.py
--rw-r--r--   0        0        0     4901 2023-07-02 13:23:36.700679 mathpad-2.0.1/mathpad/viz/viz3d.py
--rw-r--r--   0        0        0     1619 2023-07-02 13:23:38.340701 mathpad-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     8180 1970-01-01 00:00:00.000000 mathpad-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-07-08 07:41:38.595680 mathpad-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6921 2023-07-08 07:41:38.595680 mathpad-2.1.0/README.md
+-rw-r--r--   0        0        0      826 2023-07-08 07:41:39.651756 mathpad-2.1.0/mathpad/__init__.py
+-rw-r--r--   0        0        0      435 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/_global_options.py
+-rw-r--r--   0        0        0     2045 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/codegen.py
+-rw-r--r--   0        0        0      449 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/__init__.py
+-rw-r--r--   0        0        0     2424 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/_generate_units_py.py
+-rw-r--r--   0        0        0      786 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/common_vals.py
+-rw-r--r--   0        0        0     6352 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/dimensions.py
+-rw-r--r--   0        0        0     5489 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/equation.py
+-rw-r--r--   0        0        0     8319 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/frame.py
+-rw-r--r--   0        0        0    12173 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/matrix.py
+-rw-r--r--   0        0        0    11562 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/units.py
+-rw-r--r--   0        0        0    18813 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/val.py
+-rw-r--r--   0        0        0    13291 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/vector.py
+-rw-r--r--   0        0        0     7775 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/core/vector_space.py
+-rw-r--r--   0        0        0      950 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/library/constants.py
+-rw-r--r--   0        0        0     1913 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/library/electrical.py
+-rw-r--r--   0        0        0     2282 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/library/mathpad_constructor.py
+-rw-r--r--   0        0        0     1878 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/library/mechanic.py
+-rw-r--r--   0        0        0      730 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/library/trigonometry.py
+-rw-r--r--   0        0        0      266 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/__init__.py
+-rw-r--r--   0        0        0     3930 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/algebra.py
+-rw-r--r--   0        0        0     3411 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/calculus.py
+-rw-r--r--   0        0        0     1229 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/functions.py
+-rw-r--r--   0        0        0     3409 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/solve.py
+-rw-r--r--   0        0        0      414 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/maths/trigonometry.py
+-rw-r--r--   0        0        0     9648 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/simulate_dynamic_system.py
+-rw-r--r--   0        0        0    12032 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/SymbolicMatrixFunction.py
+-rw-r--r--   0        0        0      284 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch.py
+-rw-r--r--   0        0        0     1756 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_ArrayDerivative___len__and__iter__.py
+-rw-r--r--   0        0        0      924 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_MatrixOperations_subs.py
+-rw-r--r--   0        0        0     1522 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_VectorLatexPrinter_print_Derivative.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/viz/viz2d.py
+-rw-r--r--   0        0        0     4901 2023-07-08 07:41:38.679686 mathpad-2.1.0/mathpad/viz/viz3d.py
+-rw-r--r--   0        0        0     1619 2023-07-08 07:41:39.675758 mathpad-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8231 1970-01-01 00:00:00.000000 mathpad-2.1.0/PKG-INFO
```

### Comparing `mathpad-2.0.1/LICENSE` & `mathpad-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/README.md` & `mathpad-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/__init__.py` & `mathpad-2.1.0/mathpad/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 except ImportError:
     pass
 
 
 sympy.init_printing()  # type: ignore
 sympy.printing.printer.Printer.set_global_settings(min=-3, max=4)  # type: ignore
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
```

### Comparing `mathpad-2.0.1/mathpad/codegen.py` & `mathpad-2.1.0/mathpad/codegen.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/_generate_units_py.py` & `mathpad-2.1.0/mathpad/core/_generate_units_py.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/common_vals.py` & `mathpad-2.1.0/mathpad/core/common_vals.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/dimensions.py` & `mathpad-2.1.0/mathpad/core/dimensions.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/equation.py` & `mathpad-2.1.0/mathpad/core/equation.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/frame.py` & `mathpad-2.1.0/mathpad/core/frame.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/matrix.py` & `mathpad-2.1.0/mathpad/core/matrix.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/units.py` & `mathpad-2.1.0/mathpad/core/units.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/val.py` & `mathpad-2.1.0/mathpad/core/val.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/vector.py` & `mathpad-2.1.0/mathpad/core/vector.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/core/vector_space.py` & `mathpad-2.1.0/mathpad/core/vector_space.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/library/constants.py` & `mathpad-2.1.0/mathpad/library/constants.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/library/electrical.py` & `mathpad-2.1.0/mathpad/library/electrical.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/library/mathpad_constructor.py` & `mathpad-2.1.0/mathpad/library/mathpad_constructor.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/library/mechanic.py` & `mathpad-2.1.0/mathpad/library/mechanic.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/library/trigonometry.py` & `mathpad-2.1.0/mathpad/library/trigonometry.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/maths/algebra.py` & `mathpad-2.1.0/mathpad/maths/algebra.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/maths/calculus.py` & `mathpad-2.1.0/mathpad/maths/calculus.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/maths/functions.py` & `mathpad-2.1.0/mathpad/maths/functions.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/maths/solve.py` & `mathpad-2.1.0/mathpad/maths/solve.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/simulate_dynamic_system.py` & `mathpad-2.1.0/mathpad/simulate_dynamic_system.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/sympy_extensions/SymbolicMatrixFunction.py` & `mathpad-2.1.0/mathpad/sympy_extensions/SymbolicMatrixFunction.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_ArrayDerivative___len__and__iter__.py` & `mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_ArrayDerivative___len__and__iter__.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_MatrixOperations_subs.py` & `mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_MatrixOperations_subs.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/sympy_extensions/monkeypatch_VectorLatexPrinter_print_Derivative.py` & `mathpad-2.1.0/mathpad/sympy_extensions/monkeypatch_VectorLatexPrinter_print_Derivative.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/mathpad/viz/viz3d.py` & `mathpad-2.1.0/mathpad/viz/viz3d.py`

 * *Files identical despite different names*

### Comparing `mathpad-2.0.1/pyproject.toml` & `mathpad-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mathpad"
-version = "2.0.1"
+version = "2.1.0"
 description = "Simplified interface to Sympy for solving physics, engineering and maths problems"
 authors = ["Callum J Hays <callumjhays@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CallumJHays/mathpad"
 documentation = "https://mathpad.readthedocs.io"
 classifiers = [
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/CallumJHays/mathpad/issues"
 "Changelog" = "https://mathpad.readthedocs.io/changelog.html"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10" # < 3.10 required by scipy currently
+python = ">=3.7,<3.11" # < 3.10 required by scipy currently
 typing-extensions = "^4.0.0"
 numpy = "^1.20"
 sympy = "^1.8"
 scipy = "^1.7.1"
 
 [tool.poetry.extras]
 viz = ["plotly", "k3d", "tqdm"]
```

### Comparing `mathpad-2.0.1/PKG-INFO` & `mathpad-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mathpad
-Version: 2.0.1
+Version: 2.1.0
 Summary: Simplified interface to Sympy for solving physics, engineering and maths problems
 Home-page: https://github.com/CallumJHays/mathpad
 License: MIT
 Author: Callum J Hays
 Author-email: callumjhays@gmail.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: viz
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: sympy (>=1.8,<2.0)
 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/CallumJHays/mathpad/issues
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: mathpad Version: 2.0.1 Summary: Simplified
+Metadata-Version: 2.1 Name: mathpad Version: 2.1.0 Summary: Simplified
 interface to Sympy for solving physics, engineering and maths problems Home-
 page: https://github.com/CallumJHays/mathpad License: MIT Author: Callum J Hays
-Author-email: callumjhays@gmail.com Requires-Python: >=3.7,<3.10 Classifier:
+Author-email: callumjhays@gmail.com Requires-Python: >=3.7,<3.11 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
-:: Libraries Provides-Extra: viz Requires-Dist: numpy (>=1.20,<2.0) Requires-
-Dist: scipy (>=1.7.1,<2.0.0) Requires-Dist: sympy (>=1.8,<2.0) Requires-Dist:
-typing-extensions (>=4.0.0,<5.0.0) Project-URL: Bug Tracker, https://
-github.com/CallumJHays/mathpad/issues Project-URL: Changelog, https://
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Software Development :: Libraries Provides-
+Extra: viz Requires-Dist: numpy (>=1.20,<2.0) Requires-Dist: scipy
+(>=1.7.1,<2.0.0) Requires-Dist: sympy (>=1.8,<2.0) Requires-Dist: typing-
+extensions (>=4.0.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/
+CallumJHays/mathpad/issues Project-URL: Changelog, https://
 mathpad.readthedocs.io/changelog.html Project-URL: Documentation, https://
 mathpad.readthedocs.io Project-URL: Repository, https://github.com/CallumJHays/
 mathpad Description-Content-Type: text/markdown # mathpad   `mathpad` is a
 robust Computer Algebra System (CAS) library built on top of `SymPy`, providing
 a simple and intuitive way to solve engineering, science, and math problems
 using Python. ## Quickstart 1. Install using package manager of choice. For
 example, `pip`: ```bash pip install mathpad ``` 2. Import and use the library
```

