# Comparing `tmp/typeid_python-0.2.0.tar.gz` & `tmp/typeid_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid_python-0.2.0.tar", max compression
+gzip compressed data, was "typeid_python-0.2.1.tar", max compression
```

## Comparing `typeid_python-0.2.0.tar` & `typeid_python-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-02 21:35:38.940939 typeid_python-0.2.0/LICENSE
--rw-r--r--   0        0        0     2469 2023-06-30 11:13:15.292795 typeid_python-0.2.0/README.md
--rw-r--r--   0        0        0     1450 2023-07-06 12:47:21.595852 typeid_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-29 20:43:34.998392 typeid_python-0.2.0/typeid/__init__.py
--rw-r--r--   0        0        0     6469 2023-07-06 12:42:30.775952 typeid_python-0.2.0/typeid/base32.py
--rw-r--r--   0        0        0       37 2023-06-30 09:52:48.383251 typeid_python-0.2.0/typeid/constants.py
--rw-r--r--   0        0        0      207 2023-06-29 20:16:47.263968 typeid_python-0.2.0/typeid/errors.py
--rw-r--r--   0        0        0     1660 2023-06-30 19:03:52.462137 typeid_python-0.2.0/typeid/typeid.py
--rw-r--r--   0        0        0      899 2023-07-06 12:44:57.757807 typeid_python-0.2.0/typeid/validation.py
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 typeid_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 21:35:38.940939 typeid_python-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3131 2023-07-08 11:34:21.324936 typeid_python-0.2.1/README.md
+-rw-r--r--   0        0        0     1489 2023-07-08 11:29:32.917101 typeid_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-08 11:29:24.849230 typeid_python-0.2.1/typeid/__init__.py
+-rw-r--r--   0        0        0     6504 2023-07-08 11:29:24.849230 typeid_python-0.2.1/typeid/base32.py
+-rw-r--r--   0        0        0      872 2023-07-08 11:29:24.849230 typeid_python-0.2.1/typeid/cli.py
+-rw-r--r--   0        0        0       37 2023-06-30 09:52:48.383251 typeid_python-0.2.1/typeid/constants.py
+-rw-r--r--   0        0        0      207 2023-06-29 20:16:47.263968 typeid_python-0.2.1/typeid/errors.py
+-rw-r--r--   0        0        0     1862 2023-07-08 11:29:24.849230 typeid_python-0.2.1/typeid/typeid.py
+-rw-r--r--   0        0        0      899 2023-07-06 12:44:57.757807 typeid_python-0.2.1/typeid/validation.py
+-rw-r--r--   0        0        0     4067 1970-01-01 00:00:00.000000 typeid_python-0.2.1/PKG-INFO
```

### Comparing `typeid_python-0.2.0/LICENSE` & `typeid_python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.0/README.md` & `typeid_python-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 
 This particular implementation provides an pip package that can be used by any Python project.
 
 ## Installation
 
 - PyPI:
 
-    ```bash
+    ```console
     pip install typeid-python
     ```
 
 - Poetry:
 
-    ```bash
+    ```console
     poetry add typeid-python
     ```
 
 ## Usage
 
+### Basic
+
 - Create TypeID Instance:
 
     ```python
     from typeid import TypeID
 
     typeid = TypeID()
 
@@ -73,7 +75,37 @@
     uuid = uuid7()  # UUID('01890bf0-846f-7762-8605-5a3abb40e0e5')
     prefix = "user"
 
     typeid = from_uuid(prefix=prefix, suffix=uuid)
 
     print(str(typeid))  # "user_01h45z113fexh8c1at7axm1r75"
     ```
+
+### CLI-tool
+
+- Install dependencies:
+
+    ```console
+    pip install typeid-python[cli]
+    ```
+
+- To generate a new TypeID, run:
+
+    ```console
+    $ python3 -m typeid.cli new -p prefix
+    prefix_01h2xcejqtf2nbrexx3vqjhp41
+    ```
+
+- To decode an existing TypeID into a UUID run:
+
+    ```console
+    $ python3 -m typeid.cli decode prefix_01h2xcejqtf2nbrexx3vqjhp41
+    type: prefix
+    uuid: 0188bac7-4afa-78aa-bc3b-bd1eef28d881
+    ```
+
+- And to encode an existing UUID into a TypeID run:
+
+    ```console
+    $ python3 -m typeid.cli encode 0188bac7-4afa-78aa-bc3b-bd1eef28d881 --prefix prefix
+    prefix_01h2xcejqtf2nbrexx3vqjhp41
+    ```
```

#### html2text {}

```diff
@@ -2,20 +2,28 @@
 versions] ## A Python implementation of [TypeIDs](https://github.com/jetpack-
 io/typeid) using Python TypeIDs are a modern, **type-safe**, globally unique
 identifier based on the upcoming UUIDv7 standard. They provide a ton of nice
 properties that make them a great choice as the primary identifiers for your
 data in a database, APIs, and distributed systems. Read more about TypeIDs in
 their [spec](https://github.com/jetpack-io/typeid). This particular
 implementation provides an pip package that can be used by any Python project.
-## Installation - PyPI: ```bash pip install typeid-python ``` - Poetry: ```bash
-poetry add typeid-python ``` ## Usage - Create TypeID Instance: ```python from
-typeid import TypeID typeid = TypeID() print(typeid.prefix) # "" print
-(typeid.suffix) # "01h45ytscbebyvny4gc8cr8ma2" (encoded uuid7 instance) typeid
-= TypeID(prefix="user") print(typeid.prefix) # "user" print(str(typeid)) #
-"user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create TypeID from string: ```python
-from typeid import from_string typeid = from_string
-("user_01h45ytscbebyvny4gc8cr8ma2") print(str(typeid)) #
+## Installation - PyPI: ```console pip install typeid-python ``` - Poetry:
+```console poetry add typeid-python ``` ## Usage ### Basic - Create TypeID
+Instance: ```python from typeid import TypeID typeid = TypeID() print
+(typeid.prefix) # "" print(typeid.suffix) # "01h45ytscbebyvny4gc8cr8ma2"
+(encoded uuid7 instance) typeid = TypeID(prefix="user") print(typeid.prefix) #
+"user" print(str(typeid)) # "user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create
+TypeID from string: ```python from typeid import from_string typeid =
+from_string("user_01h45ytscbebyvny4gc8cr8ma2") print(str(typeid)) #
 "user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create TypeID from uuid7: ```python
 from typeid import from_uuid from uuid6 import uuid7 uuid = uuid7() # UUID
 ('01890bf0-846f-7762-8605-5a3abb40e0e5') prefix = "user" typeid = from_uuid
 (prefix=prefix, suffix=uuid) print(str(typeid)) #
-"user_01h45z113fexh8c1at7axm1r75" ```
+"user_01h45z113fexh8c1at7axm1r75" ``` ### CLI-tool - Install dependencies:
+```console pip install typeid-python[cli] ``` - To generate a new TypeID, run:
+```console $ python3 -m typeid.cli new -p prefix
+prefix_01h2xcejqtf2nbrexx3vqjhp41 ``` - To decode an existing TypeID into a
+UUID run: ```console $ python3 -m typeid.cli decode
+prefix_01h2xcejqtf2nbrexx3vqjhp41 type: prefix uuid: 0188bac7-4afa-78aa-bc3b-
+bd1eef28d881 ``` - And to encode an existing UUID into a TypeID run: ```console
+$ python3 -m typeid.cli encode 0188bac7-4afa-78aa-bc3b-bd1eef28d881 --prefix
+prefix prefix_01h2xcejqtf2nbrexx3vqjhp41 ```
```

### Comparing `typeid_python-0.2.0/pyproject.toml` & `typeid_python-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typeid-python"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs"
 authors = ["Murad Akhundov <akhundov1murad@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/akhundMurad/typeid-python"
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -53,14 +53,18 @@
 flake8 = "^5.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 requests = "^2.31.0"
 pyyaml = "^6.0"
 
 
+[tool.poetry.extras]
+cli = ["click"]
+
+
 [tool.pylint]
 disable = ["C0111", "C0116", "C0114", "R0903"]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typeid_python-0.2.0/typeid/base32.py` & `typeid_python-0.2.1/typeid/base32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from typeid.constants import SUFFIX_LEN
 
 ALPHABET = "0123456789abcdefghjkmnpqrstvwxyz"
 
 
 TABLE = [
     0xFF,
@@ -259,15 +261,15 @@
     0xFF,
     0xFF,
     0xFF,
     0xFF,
 ]
 
 
-def encode(src: list) -> str:
+def encode(src: List[int]) -> str:
     dst = [""] * SUFFIX_LEN
 
     if len(src) != 16:
         raise RuntimeError("Invalid length.")
 
     # 10 byte timestamp
     dst[0] = ALPHABET[(src[0] & 224) >> 5]
@@ -298,15 +300,15 @@
     dst[23] = ALPHABET[(src[14] & 124) >> 2]
     dst[24] = ALPHABET[((src[14] & 3) << 3) | ((src[15] & 224) >> 5)]
     dst[25] = ALPHABET[src[15] & 31]
 
     return "".join(dst)
 
 
-def decode(s: str) -> list:
+def decode(s: str) -> List[int]:
     v = bytes(s, encoding="utf-8")
 
     if (
         TABLE[v[0]] == 0xFF
         and TABLE[v[1]] == 0xFF
         and TABLE[v[2]] == 0xFF
         and TABLE[v[3]] == 0xFF
```

### Comparing `typeid_python-0.2.0/typeid/typeid.py` & `typeid_python-0.2.1/typeid/typeid.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,24 +36,33 @@
     def __eq__(self, value: object) -> bool:
         if not isinstance(value, TypeID):
             return False
         return value.prefix == self.prefix and value.suffix == self.suffix
 
 
 def from_string(string: str) -> TypeID:
-    parts = string.split("_")
+    prefix, suffix = get_prefix_and_suffix(string=string)
+    return TypeID(suffix=suffix, prefix=prefix)
+
+
+def from_uuid(suffix: UUID, prefix: Optional[str] = None) -> TypeID:
+    suffix_str = _convert_uuid_to_b32(suffix)
+    return TypeID(suffix=suffix_str, prefix=prefix)
 
+
+def get_prefix_and_suffix(string: str) -> tuple:
+    parts = string.split("_")
+    suffix = None
+    prefix = None
     if len(parts) == 1:
-        return TypeID(suffix=parts[0])
+        suffix = parts[0]
     elif len(parts) == 2 and parts[0] != "":
-        return TypeID(suffix=parts[1], prefix=parts[0])
+        suffix = parts[1]
+        prefix = parts[0]
     else:
         raise InvalidTypeIDStringException(f"Invalid TypeID: {string}")
 
-
-def from_uuid(suffix: UUID, prefix: Optional[str] = None) -> TypeID:
-    suffix_str = _convert_uuid_to_b32(suffix)
-    return TypeID(suffix=suffix_str, prefix=prefix)
+    return prefix, suffix
 
 
 def _convert_uuid_to_b32(uuid_instance: UUID) -> str:
     return base32.encode(list(uuid_instance.bytes))
```

### Comparing `typeid_python-0.2.0/typeid/validation.py` & `typeid_python-0.2.1/typeid/validation.py`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.0/PKG-INFO` & `typeid_python-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs
 Home-page: https://github.com/akhundMurad/typeid-python
 License: MIT
 Keywords: typeid,uuid,uuid6,guid
 Author: Murad Akhundov
 Author-email: akhundov1murad@gmail.com
 Requires-Python: >=3.8,<4
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cli
 Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0)
 Project-URL: Repository, https://github.com/akhundMurad/typeid-python
 Description-Content-Type: text/markdown
 
 # TypeID Python
 
 <a href="https://github.com/akhundMurad/typeid-python/actions?query=setup%3ACI%2FCD+event%3Apush+branch%3Amain" target="_blank">
@@ -44,26 +45,28 @@
 
 This particular implementation provides an pip package that can be used by any Python project.
 
 ## Installation
 
 - PyPI:
 
-    ```bash
+    ```console
     pip install typeid-python
     ```
 
 - Poetry:
 
-    ```bash
+    ```console
     poetry add typeid-python
     ```
 
 ## Usage
 
+### Basic
+
 - Create TypeID Instance:
 
     ```python
     from typeid import TypeID
 
     typeid = TypeID()
 
@@ -96,7 +99,37 @@
     prefix = "user"
 
     typeid = from_uuid(prefix=prefix, suffix=uuid)
 
     print(str(typeid))  # "user_01h45z113fexh8c1at7axm1r75"
     ```
 
+### CLI-tool
+
+- Install dependencies:
+
+    ```console
+    pip install typeid-python[cli]
+    ```
+
+- To generate a new TypeID, run:
+
+    ```console
+    $ python3 -m typeid.cli new -p prefix
+    prefix_01h2xcejqtf2nbrexx3vqjhp41
+    ```
+
+- To decode an existing TypeID into a UUID run:
+
+    ```console
+    $ python3 -m typeid.cli decode prefix_01h2xcejqtf2nbrexx3vqjhp41
+    type: prefix
+    uuid: 0188bac7-4afa-78aa-bc3b-bd1eef28d881
+    ```
+
+- And to encode an existing UUID into a TypeID run:
+
+    ```console
+    $ python3 -m typeid.cli encode 0188bac7-4afa-78aa-bc3b-bd1eef28d881 --prefix prefix
+    prefix_01h2xcejqtf2nbrexx3vqjhp41
+    ```
+
```

#### html2text {}

```diff
@@ -1,33 +1,42 @@
-Metadata-Version: 2.1 Name: typeid-python Version: 0.2.0 Summary: Python
+Metadata-Version: 2.1 Name: typeid-python Version: 0.2.1 Summary: Python
 implementation of TypeIDs: type-safe, K-sortable, and globally unique
 identifiers inspired by Stripe IDs Home-page: https://github.com/akhundMurad/
 typeid-python License: MIT Keywords: typeid,uuid,uuid6,guid Author: Murad
 Akhundov Author-email: akhundov1murad@gmail.com Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0) Project-URL:
-Repository, https://github.com/akhundMurad/typeid-python Description-Content-
-Type: text/markdown # TypeID Python [Test] [Downloads] [Package_version]
-[Supported_Python_versions] ## A Python implementation of [TypeIDs](https://
-github.com/jetpack-io/typeid) using Python TypeIDs are a modern, **type-safe**,
-globally unique identifier based on the upcoming UUIDv7 standard. They provide
-a ton of nice properties that make them a great choice as the primary
-identifiers for your data in a database, APIs, and distributed systems. Read
-more about TypeIDs in their [spec](https://github.com/jetpack-io/typeid). This
-particular implementation provides an pip package that can be used by any
-Python project. ## Installation - PyPI: ```bash pip install typeid-python ``` -
-Poetry: ```bash poetry add typeid-python ``` ## Usage - Create TypeID Instance:
-```python from typeid import TypeID typeid = TypeID() print(typeid.prefix) # ""
-print(typeid.suffix) # "01h45ytscbebyvny4gc8cr8ma2" (encoded uuid7 instance)
-typeid = TypeID(prefix="user") print(typeid.prefix) # "user" print(str(typeid))
-# "user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create TypeID from string: ```python
+Python :: 3.11 Provides-Extra: cli Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0)
+Project-URL: Repository, https://github.com/akhundMurad/typeid-python
+Description-Content-Type: text/markdown # TypeID Python [Test] [Downloads]
+[Package_version] [Supported_Python_versions] ## A Python implementation of
+[TypeIDs](https://github.com/jetpack-io/typeid) using Python TypeIDs are a
+modern, **type-safe**, globally unique identifier based on the upcoming UUIDv7
+standard. They provide a ton of nice properties that make them a great choice
+as the primary identifiers for your data in a database, APIs, and distributed
+systems. Read more about TypeIDs in their [spec](https://github.com/jetpack-io/
+typeid). This particular implementation provides an pip package that can be
+used by any Python project. ## Installation - PyPI: ```console pip install
+typeid-python ``` - Poetry: ```console poetry add typeid-python ``` ## Usage
+### Basic - Create TypeID Instance: ```python from typeid import TypeID typeid
+= TypeID() print(typeid.prefix) # "" print(typeid.suffix) #
+"01h45ytscbebyvny4gc8cr8ma2" (encoded uuid7 instance) typeid = TypeID
+(prefix="user") print(typeid.prefix) # "user" print(str(typeid)) #
+"user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create TypeID from string: ```python
 from typeid import from_string typeid = from_string
 ("user_01h45ytscbebyvny4gc8cr8ma2") print(str(typeid)) #
 "user_01h45ytscbebyvny4gc8cr8ma2" ``` - Create TypeID from uuid7: ```python
 from typeid import from_uuid from uuid6 import uuid7 uuid = uuid7() # UUID
 ('01890bf0-846f-7762-8605-5a3abb40e0e5') prefix = "user" typeid = from_uuid
 (prefix=prefix, suffix=uuid) print(str(typeid)) #
-"user_01h45z113fexh8c1at7axm1r75" ```
+"user_01h45z113fexh8c1at7axm1r75" ``` ### CLI-tool - Install dependencies:
+```console pip install typeid-python[cli] ``` - To generate a new TypeID, run:
+```console $ python3 -m typeid.cli new -p prefix
+prefix_01h2xcejqtf2nbrexx3vqjhp41 ``` - To decode an existing TypeID into a
+UUID run: ```console $ python3 -m typeid.cli decode
+prefix_01h2xcejqtf2nbrexx3vqjhp41 type: prefix uuid: 0188bac7-4afa-78aa-bc3b-
+bd1eef28d881 ``` - And to encode an existing UUID into a TypeID run: ```console
+$ python3 -m typeid.cli encode 0188bac7-4afa-78aa-bc3b-bd1eef28d881 --prefix
+prefix prefix_01h2xcejqtf2nbrexx3vqjhp41 ```
```

