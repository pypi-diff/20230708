# Comparing `tmp/smtpdfix-0.5.0.tar.gz` & `tmp/smtpdfix-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smtpdfix-0.5.0.tar", last modified: Tue May  2 17:47:10 2023, max compression
+gzip compressed data, was "smtpdfix-0.5.1.tar", last modified: Sat Jul  8 01:18:38 2023, max compression
```

## Comparing `smtpdfix-0.5.0.tar` & `smtpdfix-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/
--rw-r--r--   0 james     (1000) james     (1000)     1089 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/LICENSE
--rw-r--r--   0 james     (1000) james     (1000)    10715 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)     9715 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/README.md
--rw-r--r--   0 james     (1000) james     (1000)       90 2023-01-05 22:40:35.000000 smtpdfix-0.5.0/pyproject.toml
--rw-r--r--   0 james     (1000) james     (1000)     2113 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/setup.cfg
--rw-r--r--   0 james     (1000) james     (1000)       41 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/setup.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.721994 smtpdfix-0.5.0/smtpdfix/
--rw-r--r--   0 james     (1000) james     (1000)      342 2023-05-02 17:45:20.000000 smtpdfix-0.5.0/smtpdfix/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)     1041 2022-11-12 12:17:37.000000 smtpdfix-0.5.0/smtpdfix/authenticator.py
--rw-r--r--   0 james     (1000) james     (1000)     3063 2022-09-05 11:25:36.000000 smtpdfix-0.5.0/smtpdfix/certs.py
--rw-r--r--   0 james     (1000) james     (1000)     5027 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/smtpdfix/configuration.py
--rw-r--r--   0 james     (1000) james     (1000)     8008 2023-05-02 16:10:16.000000 smtpdfix-0.5.0/smtpdfix/controller.py
--rw-r--r--   0 james     (1000) james     (1000)      640 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/event_handler.py
--rw-r--r--   0 james     (1000) james     (1000)     2606 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/smtpdfix/fixture.py
--rw-r--r--   0 james     (1000) james     (1000)     3400 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/handlers.py
--rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/py.typed
--rw-r--r--   0 james     (1000) james     (1000)     1660 2023-04-10 17:16:42.000000 smtpdfix-0.5.0/smtpdfix/smtp.py
--rw-r--r--   0 james     (1000) james     (1000)      673 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/typing.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.731994 smtpdfix-0.5.0/smtpdfix.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)    10715 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      633 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/SOURCES.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/dependency_links.txt
--rw-r--r--   0 james     (1000) james     (1000)       36 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/entry_points.txt
--rw-r--r--   0 james     (1000) james     (1000)      239 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/requires.txt
--rw-r--r--   0 james     (1000) james     (1000)       15 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/top_level.txt
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/tests/
--rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/tests/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)     1191 2022-12-03 17:17:56.000000 smtpdfix-0.5.0/tests/conftest.py
--rw-r--r--   0 james     (1000) james     (1000)     3016 2023-04-03 11:16:42.000000 smtpdfix-0.5.0/tests/test_configuration.py
--rw-r--r--   0 james     (1000) james     (1000)     4789 2023-04-03 11:16:42.000000 smtpdfix-0.5.0/tests/test_controller.py
--rw-r--r--   0 james     (1000) james     (1000)     7914 2023-04-01 17:11:44.000000 smtpdfix-0.5.0/tests/test_fixture.py
--rw-r--r--   0 james     (1000) james     (1000)     3057 2023-04-10 17:11:14.000000 smtpdfix-0.5.0/tests/test_smtp.py
--rw-r--r--   0 james     (1000) james     (1000)     1068 2023-04-08 16:47:14.000000 smtpdfix-0.5.0/tests/test_smtpdfix.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.648136 smtpdfix-0.5.1/
+-rw-r--r--   0 james      (501) staff       (20)     1089 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    10715 2023-07-08 01:18:38.648217 smtpdfix-0.5.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     9715 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/README.md
+-rw-r--r--   0 james      (501) staff       (20)       90 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)     2085 2023-07-08 01:18:38.648595 smtpdfix-0.5.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.646337 smtpdfix-0.5.1/smtpdfix/
+-rw-r--r--   0 james      (501) staff       (20)      342 2023-07-08 01:17:28.000000 smtpdfix-0.5.1/smtpdfix/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1041 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/authenticator.py
+-rw-r--r--   0 james      (501) staff       (20)     3063 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/certs.py
+-rw-r--r--   0 james      (501) staff       (20)     5034 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/configuration.py
+-rw-r--r--   0 james      (501) staff       (20)     8078 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/smtpdfix/controller.py
+-rw-r--r--   0 james      (501) staff       (20)      688 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/event_handler.py
+-rw-r--r--   0 james      (501) staff       (20)     2577 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/fixture.py
+-rw-r--r--   0 james      (501) staff       (20)     3400 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/smtpdfix/handlers.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/py.typed
+-rw-r--r--   0 james      (501) staff       (20)     1660 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/smtp.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.647215 smtpdfix-0.5.1/smtpdfix.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    10715 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      614 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       36 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      120 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        9 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.648024 smtpdfix-0.5.1/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1191 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/conftest.py
+-rw-r--r--   0 james      (501) staff       (20)     3016 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/test_configuration.py
+-rw-r--r--   0 james      (501) staff       (20)     4789 2023-06-23 13:43:39.000000 smtpdfix-0.5.1/tests/test_controller.py
+-rw-r--r--   0 james      (501) staff       (20)     7914 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/test_fixture.py
+-rw-r--r--   0 james      (501) staff       (20)     3057 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/tests/test_smtp.py
+-rw-r--r--   0 james      (501) staff       (20)     1068 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/tests/test_smtpdfix.py
```

### Comparing `smtpdfix-0.5.0/LICENSE` & `smtpdfix-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/PKG-INFO` & `smtpdfix-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.5.0
+Version: 0.5.1
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
```

### Comparing `smtpdfix-0.5.0/README.md` & `smtpdfix-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/setup.cfg` & `smtpdfix-0.5.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 	Issues = https://github.com/bebleo/smtpdfix/issues
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	aiosmtpd
-	cryptography;python_implementation!="PyPy"
-	cryptography >= 39.0.1, < 40.0.0;python_implementation=="PyPy"
+	cryptography
 	portpicker
 	pytest
 python_requires = >=3.7
 
 [options.entry_points]
 pytest11 = 
 	smtpd = smtpdfix.fixture
@@ -53,14 +52,20 @@
 	tox
 typing = 
 	mypy
 
 [options.package_data]
 smtpdfix = py.typed
 
+[options.packages.find]
+exclude = 
+	docs*
+	requirements*
+	tests*
+
 [tool:pytest]
 testpaths = tests
 
 [coverage:run]
 branch = True
 source = smtpdfix
```

### Comparing `smtpdfix-0.5.0/smtpdfix/authenticator.py` & `smtpdfix-0.5.1/smtpdfix/authenticator.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/smtpdfix/certs.py` & `smtpdfix-0.5.1/smtpdfix/certs.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/smtpdfix/configuration.py` & `smtpdfix-0.5.1/smtpdfix/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from pathlib import Path
 from typing import Any, Optional, Tuple, Union
 
 import portpicker
 
 from .event_handler import EventHandler
-from .typing import PathType
+
+PathType = Union[str, os.PathLike]
 
 _current_dir = Path(__file__).parent
 
 
 def _strtobool(val: str) -> bool:
     """Convert a string representation of truth to true (1) or false (0).
```

### Comparing `smtpdfix-0.5.0/smtpdfix/controller.py` & `smtpdfix-0.5.1/smtpdfix/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import errno
 import logging
 from contextlib import ExitStack
 from os import strerror
 from pathlib import Path
 from socket import create_connection
 from ssl import CERT_OPTIONAL, Purpose, SSLContext, create_default_context
-from typing import Any, List, Optional
+from typing import Any, Coroutine, List, Optional
 
 from aiosmtpd.controller import Controller, get_localhost
 
 from .authenticator import Authenticator
-from .configuration import Config
+from .configuration import Config, PathType
 from .handlers import AuthMessage
 from .smtp import _SMTP
-from .typing import AsyncServer, PathType, ServerCoroutine
+
+AsyncServer = asyncio.base_events.Server
+ServerCoroutine = Coroutine[Any, Any, asyncio.base_events.Server]
 
 log = logging.getLogger(__name__)
 
 
 class AuthController(Controller):
     def __init__(self,
                  loop: Optional[asyncio.AbstractEventLoop] = None,
```

### Comparing `smtpdfix-0.5.0/smtpdfix/fixture.py` & `smtpdfix-0.5.1/smtpdfix/fixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import portpicker
 import pytest
 
 from .authenticator import Authenticator
 from .certs import _generate_certs
 from .configuration import Config
 from .controller import AuthController
-from .typing import TempPathFactory
 
 log = logging.getLogger(__name__)
 
 
 class _Authenticator(Authenticator):
     def __init__(self, config: Config) -> None:
         self.config = config
@@ -61,15 +60,15 @@
 
     def __exit__(self, type: Any, value: Any, traceback: Any) -> None:
         self.controller.stop()
 
 
 @pytest.fixture
 def smtpd(
-    tmp_path_factory: TempPathFactory
+    tmp_path_factory: pytest.TempPathFactory
 ) -> Generator[AuthController, None, None]:
     """A small SMTP server for use when testing applications that send email
     messages. To access the messages call `smtpd.messages` which returns a copy
     of the list of messages sent to the server.
 
     Example:
         def test_mail(smtpd):
```

### Comparing `smtpdfix-0.5.0/smtpdfix/handlers.py` & `smtpdfix-0.5.1/smtpdfix/handlers.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/smtpdfix/smtp.py` & `smtpdfix-0.5.1/smtpdfix/smtp.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/smtpdfix.egg-info/PKG-INFO` & `smtpdfix-0.5.1/smtpdfix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.5.0
+Version: 0.5.1
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
```

### Comparing `smtpdfix-0.5.0/smtpdfix.egg-info/SOURCES.txt` & `smtpdfix-0.5.1/smtpdfix.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 smtpdfix/configuration.py
 smtpdfix/controller.py
 smtpdfix/event_handler.py
 smtpdfix/fixture.py
 smtpdfix/handlers.py
 smtpdfix/py.typed
 smtpdfix/smtp.py
-smtpdfix/typing.py
 smtpdfix.egg-info/PKG-INFO
 smtpdfix.egg-info/SOURCES.txt
 smtpdfix.egg-info/dependency_links.txt
 smtpdfix.egg-info/entry_points.txt
 smtpdfix.egg-info/requires.txt
 smtpdfix.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `smtpdfix-0.5.0/tests/conftest.py` & `smtpdfix-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/tests/test_configuration.py` & `smtpdfix-0.5.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/tests/test_controller.py` & `smtpdfix-0.5.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/tests/test_fixture.py` & `smtpdfix-0.5.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/tests/test_smtp.py` & `smtpdfix-0.5.1/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.0/tests/test_smtpdfix.py` & `smtpdfix-0.5.1/tests/test_smtpdfix.py`

 * *Files identical despite different names*

