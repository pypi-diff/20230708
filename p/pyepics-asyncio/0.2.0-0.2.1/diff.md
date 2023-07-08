# Comparing `tmp/pyepics-asyncio-0.2.0.tar.gz` & `tmp/pyepics_asyncio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepics-asyncio-0.2.0.tar", max compression
+gzip compressed data, was "pyepics_asyncio-0.2.1.tar", max compression
```

## Comparing `pyepics-asyncio-0.2.0.tar` & `pyepics_asyncio-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      664 2022-04-06 12:17:54.769183 pyepics-asyncio-0.2.0/README.md
--rw-r--r--   0        0        0     4053 2022-10-07 04:56:36.162117 pyepics-asyncio-0.2.0/pyepics_asyncio/__init__.py
--rw-r--r--   0        0        0        0 2022-04-06 12:17:54.769183 pyepics-asyncio-0.2.0/pyepics_asyncio/py.typed
--rw-r--r--   0        0        0      855 2022-10-07 02:25:36.142088 pyepics-asyncio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1383 2022-10-07 04:59:45.742431 pyepics-asyncio-0.2.0/setup.py
--rw-r--r--   0        0        0     1501 2022-10-07 04:59:45.742697 pyepics-asyncio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      638 2023-07-08 06:53:40.401654 pyepics_asyncio-0.2.1/README.md
+-rw-r--r--   0        0        0     4037 2023-07-08 06:57:01.373994 pyepics_asyncio-0.2.1/pyepics_asyncio/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-06 12:17:54.769183 pyepics_asyncio-0.2.1/pyepics_asyncio/py.typed
+-rw-r--r--   0        0        0      837 2023-07-08 06:59:14.374240 pyepics_asyncio-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.1/setup.py
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.1/PKG-INFO
```

### Comparing `pyepics-asyncio-0.2.0/pyepics_asyncio/__init__.py` & `pyepics_asyncio-0.2.1/pyepics_asyncio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             loop.call_soon_threadsafe(self._complete)
 
     def __init__(self, pv: PvBase, value: Any) -> None:
         super().__init__()
         pv.raw.put(value, wait=False, callback=self._callback)
 
 
-T = TypeVar("T", bound=PvBase, covariant=True)
+T = TypeVar("T", bound=PvBase)
 
 
 class _ConnectBase(Future[T]):
     def _cancel(self) -> None:
         self.raw.disconnect()
 
     def _complete(self) -> None:
```

### Comparing `pyepics-asyncio-0.2.0/pyproject.toml` & `pyepics_asyncio-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyepics-asyncio"
-version = "0.2.0"
+version = "0.2.1"
 description = "Async/await wrapper for PyEpics"
 homepage = "https://github.com/agerasev/pyepics-asyncio"
 repository = "https://github.com/agerasev/pyepics-asyncio"
 authors = ["Alexey Gerasev <alexey.gerasev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pyepics", "epics", "asyncio", "async", "await"]
@@ -16,17 +16,16 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyepics = "^3.5.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
-mypy = "^0.942"
-numpy = "^1.22.3"
+mypy = "^1.4.1"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 128
```

### Comparing `pyepics-asyncio-0.2.0/setup.py` & `pyepics_asyncio-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['pyepics>=3.5.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'pyepics-asyncio',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Async/await wrapper for PyEpics',
-    'long_description': '# pyepics-asyncio\n\nSimple `async`/`await` wrapper for [PyEpics](https://github.com/pyepics/pyepics).\n\nCurrently there is a wrapper only for `PV` class.\n\n## Usage\n\n### Import\n\n```python\nfrom pyepics_asyncio import Pv\n```\n\n### Connect to PV\n\n```python\npv = await Pv.connect("pvname")\n```\n\n### Read PV value\n\n```python\nprint(await pv.get())\n```\n\n### Write value to PV\n\n```python\nawait pv.put(3.1415)\n```\n\n### Monitor PV\n\n```python\nasync with pv.monitor() as mon:\n    async for value in mon:\n        print(value)\n```\n\n*NOTE: By default values are yielded only on PV update.*\n*If you need monitor to also provide current value on start use `pv.monitor(current=True)`.*\n',
+    'long_description': '# pyepics-asyncio\n\nSimple `async`/`await` wrapper for [PyEpics](https://github.com/pyepics/pyepics).\n\n## Overview\n\nThere are two main types:\n+ `PvMonitor` - subscribed to PV updates, `get` returns last received value.\n+ `Pv` - connected but not subscribed, each `get` requests PV value over network.\n\n## Usage\n\n### Read PV value\n\n```python\nfrom pyepics_asyncio import Pv\n\npv = await Pv.connect("pvname")\nprint(await pv.get())\n```\n\n### Monitor PV\n\n```python\nfrom pyepics_asyncio import PvMonitor\n\npv = await PvMonitor.connect("pvname")\nasync for value in pv:\n    print(value)\n```\n\n### Write value to PV\n\n```python\nawait pv.put(3.1415)\n```\n',
     'author': 'Alexey Gerasev',
     'author_email': 'alexey.gerasev@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/agerasev/pyepics-asyncio',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `pyepics-asyncio-0.2.0/PKG-INFO` & `pyepics_asyncio-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 Metadata-Version: 2.1
 Name: pyepics-asyncio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Async/await wrapper for PyEpics
 Home-page: https://github.com/agerasev/pyepics-asyncio
 License: MIT
 Keywords: pyepics,epics,asyncio,async,await
 Author: Alexey Gerasev
 Author-email: alexey.gerasev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: pyepics (>=3.5.1,<4.0.0)
 Project-URL: Repository, https://github.com/agerasev/pyepics-asyncio
 Description-Content-Type: text/markdown
 
 # pyepics-asyncio
 
 Simple `async`/`await` wrapper for [PyEpics](https://github.com/pyepics/pyepics).
 
-Currently there is a wrapper only for `PV` class.
+## Overview
+
+There are two main types:
++ `PvMonitor` - subscribed to PV updates, `get` returns last received value.
++ `Pv` - connected but not subscribed, each `get` requests PV value over network.
 
 ## Usage
 
-### Import
+### Read PV value
 
 ```python
 from pyepics_asyncio import Pv
-```
 
-### Connect to PV
-
-```python
 pv = await Pv.connect("pvname")
+print(await pv.get())
 ```
 
-### Read PV value
+### Monitor PV
 
 ```python
-print(await pv.get())
+from pyepics_asyncio import PvMonitor
+
+pv = await PvMonitor.connect("pvname")
+async for value in pv:
+    print(value)
 ```
 
 ### Write value to PV
 
 ```python
 await pv.put(3.1415)
 ```
 
-### Monitor PV
-
-```python
-async with pv.monitor() as mon:
-    async for value in mon:
-        print(value)
-```
-
-*NOTE: By default values are yielded only on PV update.*
-*If you need monitor to also provide current value on start use `pv.monitor(current=True)`.*
-
```

