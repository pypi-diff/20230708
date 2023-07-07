# Comparing `tmp/django_spreadsheet_serializer-0.1.0a0.tar.gz` & `tmp/django_spreadsheet_serializer-0.1.0rc1.tar.gz`

## Comparing `django_spreadsheet_serializer-0.1.0a0.tar` & `django_spreadsheet_serializer-0.1.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/.DS_Store
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/.editorconfig
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/requirements-dev.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tox.ini
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/apps.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/core.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/serializers/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/serializers/ods_serializer.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/serializers/xlsx_serializer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tests/models.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tests/settings.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tests/test_deserialization.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/tests/test_utils.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/.DS_Store
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/.editorconfig
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/requirements-dev.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tox.ini
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/__init__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/apps.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/core.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/serializers/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/serializers/ods_serializer.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/serializers/xlsx_serializer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tests/models.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tests/settings.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tests/test_deserialization.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/tests/test_utils.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 django_spreadsheet_serializer-0.1.0rc1/PKG-INFO
```

### Comparing `django_spreadsheet_serializer-0.1.0a0/.DS_Store` & `django_spreadsheet_serializer-0.1.0rc1/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/.pre-commit-config.yaml` & `django_spreadsheet_serializer-0.1.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/tox.ini` & `django_spreadsheet_serializer-0.1.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/.github/workflows/ci.yaml` & `django_spreadsheet_serializer-0.1.0rc1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/apps.py` & `django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/apps.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/spreadsheet_serializer/core.py` & `django_spreadsheet_serializer-0.1.0rc1/spreadsheet_serializer/core.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/tests/models.py` & `django_spreadsheet_serializer-0.1.0rc1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/tests/settings.py` & `django_spreadsheet_serializer-0.1.0rc1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/tests/test_deserialization.py` & `django_spreadsheet_serializer-0.1.0rc1/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/tests/test_utils.py` & `django_spreadsheet_serializer-0.1.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/.gitignore` & `django_spreadsheet_serializer-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/LICENSE` & `django_spreadsheet_serializer-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/README.md` & `django_spreadsheet_serializer-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `django_spreadsheet_serializer-0.1.0a0/pyproject.toml` & `django_spreadsheet_serializer-0.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-spreadsheet-serializer"
-version = "0.1.0-alpha"
+version = "0.1.0-rc1"
 description = "Manage Django models using spreadsheets!"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">= 3.8"
-license = {file = "LICENSE"}
+license = {text = "MIT License"}
 authors = [
   {name = "Kamil Paduszyński", email = "paduszyk@gmail.com"},
 ]
 maintainers = [
   {name = "Kamil Paduszyński", email = "paduszyk@gmail.com"},
 ]
 keywords = ["python", "django", "spreadsheet", "Excel", "xlsx", "ods"]
```

### Comparing `django_spreadsheet_serializer-0.1.0a0/PKG-INFO` & `django_spreadsheet_serializer-0.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,17 @@
 Metadata-Version: 2.1
 Name: django-spreadsheet-serializer
-Version: 0.1.0a0
+Version: 0.1.0rc1
 Summary: Manage Django models using spreadsheets!
 Project-URL: Homepage, https://github.com/paduszyk/django-spreadsheet-serializer
 Project-URL: Documentation, https://github.com/paduszyk/django-spreadsheet-serializer#readme
 Project-URL: Repository, https://github.com/paduszyk/django-spreadsheet-serializer
 Author-email: Kamil Paduszyński <paduszyk@gmail.com>
 Maintainer-email: Kamil Paduszyński <paduszyk@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2023 Kamil Paduszyński
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
 License-File: LICENSE
 Keywords: Excel,django,ods,python,spreadsheet,xlsx
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
```

