# Comparing `tmp/atomic_counter-0.1.1.tar.gz` & `tmp/atomic_counter-0.1.2.tar.gz`

## Comparing `atomic_counter-0.1.1.tar` & `atomic_counter-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 atomic_counter-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123      410 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.bumpversion.cfg
--rw-r--r--   0     1001      123      147 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.gitattributes
--rw-r--r--   0     1001      123     3352 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123      206 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/dependabot.yml
--rw-r--r--   0     1001      123     1690 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/workflows/build.yml
--rw-r--r--   0     1001      123     4134 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/workflows/deploy.yml
--rw-r--r--   0     1001      123     1817 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.gitignore
--rw-r--r--   0     1001      123    11352 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/LICENSE
--rw-r--r--   0     1001      123      284 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/MANIFEST.in
--rw-r--r--   0     1001      123     2266 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/Makefile
--rw-r--r--   0     1001      123     1730 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/README.md
--rw-r--r--   0     1001      123      545 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/__init__.py
--rw-r--r--   0     1001      123      454 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_daily.py
--rw-r--r--   0     1001      123       78 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_exports.py
--rw-r--r--   0     1001      123      930 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_offset.py
--rw-r--r--   0     1001      123     1130 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     1166 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123       10 2023-04-11 00:03:00.000000 atomic_counter-0.1.1/wheelhouse/atomic_counter-0.1.1.tar.gz
--rw-r--r--   0     1001      123    18299 2023-04-11 00:02:58.000000 atomic_counter-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 atomic_counter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 atomic_counter-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123      410 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.bumpversion.cfg
+-rw-r--r--   0     1001      123      147 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.gitattributes
+-rw-r--r--   0     1001      123     3352 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123      206 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1690 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0     1001      123     4134 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     1817 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/.gitignore
+-rw-r--r--   0     1001      123    11352 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/LICENSE
+-rw-r--r--   0     1001      123      284 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/MANIFEST.in
+-rw-r--r--   0     1001      123     2266 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/Makefile
+-rw-r--r--   0     1001      123     1730 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/README.md
+-rw-r--r--   0     1001      123      545 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/atomic_counter/__init__.py
+-rw-r--r--   0     1001      123      454 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/atomic_counter/tests/test_daily.py
+-rw-r--r--   0     1001      123       78 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/atomic_counter/tests/test_exports.py
+-rw-r--r--   0     1001      123      930 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/atomic_counter/tests/test_offset.py
+-rw-r--r--   0     1001      123     1402 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     1166 2023-07-08 01:19:25.000000 atomic_counter-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123    17799 2023-07-08 01:19:51.000000 atomic_counter-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 atomic_counter-0.1.2/PKG-INFO
```

### Comparing `atomic_counter-0.1.1/.github/CODE_OF_CONDUCT.md` & `atomic_counter-0.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/.github/workflows/build.yml` & `atomic_counter-0.1.2/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Rust
       uses: actions-rs/toolchain@v1
       with:
         profile: minimal
-        toolchain: nightly
+        toolchain: stable 
         components: clippy
         override: true
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `atomic_counter-0.1.1/.github/workflows/deploy.yml` & `atomic_counter-0.1.2/.github/workflows/deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         cache: 'pip'
         cache-dependency-path: 'pyproject.toml'
 
     - name: Setup Rust
       uses: actions-rs/toolchain@v1
       with:
         profile: minimal
-        toolchain: nightly
+        toolchain: stable 
         components: clippy
         override: true
 
     - name: Setup Rust cache
       uses: Swatinem/rust-cache@v2
       with:
         key: ${{ matrix.alt_arch_name }}
```

### Comparing `atomic_counter-0.1.1/.gitignore` & `atomic_counter-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/LICENSE` & `atomic_counter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/Makefile` & `atomic_counter-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/README.md` & `atomic_counter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/atomic_counter/__init__.py` & `atomic_counter-0.1.2/atomic_counter/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from functools import lru_cache
 from datetime import datetime
 from dateutil import tz
 
 from .atomic_counter import Counter
```

### Comparing `atomic_counter-0.1.1/atomic_counter/tests/test_offset.py` & `atomic_counter-0.1.2/atomic_counter/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/pyproject.toml` & `atomic_counter-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 [build-system]
-requires = ["maturin>=0.13,<0.14"]
+requires = [
+  "maturin>=1.1,<2"
+]
 build-backend = "maturin"
 
 [project]
 name = "atomic-counter"
 authors = [{name = "Tim Paine"}]
 description="Atomic Counters"
 readme = "README.md"
-version = "0.1.1"
-requires-python = ">=3.7"
+version = "0.1.2"
+requires-python = ">=3.8"
 dependencies = [
   "python-dateutil",
 ]
 classifiers = [
+    "Development Status :: 3 - Alpha",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 develop = [
   "check-manifest",
-  "maturin",
+  "maturin>=1.1,<2",
   "pytest",
   "pytest-cov",
   "ruff",
   "twine",
   "wheel",
 ]
```

### Comparing `atomic_counter-0.1.1/src/lib.rs` & `atomic_counter-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.1/Cargo.lock` & `atomic_counter-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,17 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "atomic-counter"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62f447d68cfa5a9ab0c1c862a703da2a65b5ed1b7ce1153c9eb0169506d56019"
-
-[[package]]
 name = "atomic-counter-py"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
- "atomic-counter",
  "chrono",
  "pyo3",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -84,24 +77,14 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
-name = "ctor"
-version = "0.1.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
-dependencies = [
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "cxx"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
@@ -138,25 +121,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.13",
 ]
 
 [[package]]
-name = "ghost"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "iana-time-zone"
 version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -180,21 +152,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.2.3"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84344c6e0b90a9e2b6f3f9abe5cc74402684e348df7b32adca28747e0cef091a"
-dependencies = [
- "ctor",
- "ghost",
-]
+checksum = "c38a87a1e0e2752433cd4b26019a469112a25fb43b30f5ee9b3b898925c5a0f9"
 
 [[package]]
 name = "js-sys"
 version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
@@ -232,14 +200,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
@@ -290,66 +267,67 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.16.6"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0220c44442c9b239dd4357aa856ac468a4f5e1f0df19ddb89b2522952eb4c6ca"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.16.6"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c819d397859445928609d0ec5afc2da5204e0d0f73d6bf9e153b04e83c9cdc2"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.16.6"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca882703ab55f54702d7bfe1189b41b0af10272389f04cae38fe4cd56c65f75f"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.16.6"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "568749402955ad7be7bad9a09b8593851cd36e549ac90bfd44079cea500f3f21"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.16.6"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "611f64e82d98f447787e82b8e7b0ebc681e1eb78fc1252668b2c605ffb4e1eb8"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
```

### Comparing `atomic_counter-0.1.1/PKG-INFO` & `atomic_counter-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: atomic-counter
-Version: 0.1.1
+Version: 0.1.2
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dateutil
-Requires-Dist: check-manifest; extra == 'develop'
-Requires-Dist: maturin; extra == 'develop'
-Requires-Dist: pytest; extra == 'develop'
-Requires-Dist: pytest-cov; extra == 'develop'
-Requires-Dist: ruff; extra == 'develop'
-Requires-Dist: twine; extra == 'develop'
-Requires-Dist: wheel; extra == 'develop'
+Requires-Dist: check-manifest ; extra == 'develop'
+Requires-Dist: maturin >=1.1, <2 ; extra == 'develop'
+Requires-Dist: pytest ; extra == 'develop'
+Requires-Dist: pytest-cov ; extra == 'develop'
+Requires-Dist: ruff ; extra == 'develop'
+Requires-Dist: twine ; extra == 'develop'
+Requires-Dist: wheel ; extra == 'develop'
 Provides-Extra: develop
 License-File: LICENSE
 Summary: Atomic Counters
 Author: Tim Paine
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/timkpaine/atomic-counter
 Project-URL: homepage, https://github.com/timkpaine/atomic-counter
 
 # Atomic Counter
 
 [![Build Status](https://github.com/timkpaine/atomic-counter/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/atomic-counter/actions?query=workflow%3A%22Build+Status%22)
```

