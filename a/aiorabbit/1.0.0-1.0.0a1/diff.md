# Comparing `tmp/aiorabbit-1.0.0.tar.gz` & `tmp/aiorabbit-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorabbit-1.0.0.tar", last modified: Sat Jul  8 17:41:20 2023, max compression
+gzip compressed data, was "dist/aiorabbit-1.0.0a1.tar", last modified: Thu Mar 26 23:40:23 2020, max compression
```

## Comparing `aiorabbit-1.0.0.tar` & `aiorabbit-1.0.0a1.tar`

### file list

```diff
@@ -1,38 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:41:20.448769 aiorabbit-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5532 2023-07-08 17:41:20.448769 aiorabbit-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4439 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:41:20.440769 aiorabbit-1.0.0/aiorabbit/
--rw-r--r--   0 root         (0) root         (0)     2064 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/__version__.py
--rw-r--r--   0 root         (0) root         (0)    12232 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/channel0.py
--rw-r--r--   0 root         (0) root         (0)    74235 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/client.py
--rw-r--r--   0 root         (0) root         (0)     6122 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5891 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/message.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/protocol.py
--rw-r--r--   0 root         (0) root         (0)     4752 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/state.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/aiorabbit/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:41:20.444769 aiorabbit-1.0.0/aiorabbit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5532 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      725 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:41:20.000000 aiorabbit-1.0.0/aiorabbit.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-08 17:41:20.452769 aiorabbit-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:41:20.448769 aiorabbit-1.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)    10519 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_basic.py
--rw-r--r--   0 root         (0) root         (0)     8679 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_channel0.py
--rw-r--r--   0 root         (0) root         (0)     5675 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_client_edge_cases.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_exchange.py
--rw-r--r--   0 root         (0) root         (0)     8088 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_protocol.py
--rw-r--r--   0 root         (0) root         (0)     7478 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_publish.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_queue.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_state.py
--rw-r--r--   0 root         (0) root         (0)      912 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_tx.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/test_validation.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-07-08 17:41:08.000000 aiorabbit-1.0.0/tests/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-26 23:40:23.961623 aiorabbit-1.0.0a1/
+-rw-r--r--   0 root         (0) root         (0)     1500 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       35 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6257 2020-03-26 23:40:23.961623 aiorabbit-1.0.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4439 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-26 23:40:23.961623 aiorabbit-1.0.0a1/aiorabbit/
+-rw-r--r--   0 root         (0) root         (0)     1609 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       36 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/__version__.py
+-rw-r--r--   0 root         (0) root         (0)    11956 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/channel0.py
+-rw-r--r--   0 root         (0) root         (0)    73496 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/client.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5891 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/message.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/state.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-26 23:40:23.961623 aiorabbit-1.0.0a1/aiorabbit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6257 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      193 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/aiorabbit.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1974 2020-03-26 23:40:23.961623 aiorabbit-1.0.0a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2020-03-26 23:40:23.000000 aiorabbit-1.0.0a1/setup.py
```

### Comparing `aiorabbit-1.0.0/LICENSE` & `aiorabbit-1.0.0a1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019-2023 Gavin M. Roy
+Copyright (c) 2019-2020 Gavin M. Roy
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `aiorabbit-1.0.0/PKG-INFO` & `aiorabbit-1.0.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,126 @@
 Metadata-Version: 2.1
 Name: aiorabbit
-Version: 1.0.0
+Version: 1.0.0a1
 Summary: An AsyncIO RabbitMQ Client Library
 Home-page: https://github.com/gmr/aiorabbit
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/aiorabbit/issues
 Project-URL: Documentation, https://aiorabbit.readthedocs.io
 Project-URL: Source Code, https://github.com/gmr/aiorabbit/
+Description: aiorabbit
+        =========
+        aiorabbit is an opinionated AsyncIO RabbitMQ client for `Python 3 <https://www.python.org/>`_ (3.7+).
+        
+        |Version| |Status| |Coverage| |License|
+        
+        Project Goals
+        -------------
+        - To create a simple, robust `RabbitMQ <https://rabbitmq.com>`_ client library for `AsyncIO <https://docs.python.org/3/library/asyncio.html>`_ development in Python 3.
+        - To make use of new features and capabilities in Python 3.7+.
+        - Remove some complexity in using an `AMQP <https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol>`_ client by:
+           - Abstracting away the AMQP channel and use it only as a protocol coordination mechanism inside the client.
+           - Remove the `nowait <https://www.rabbitmq.com/amqp-0-9-1-reference.html#domain.no-wait>`_ keyword to ensure a single round-trip pattern of behavior for client usage.
+        - To automatically reconnect when a connection is closed due to an AMQP exception/error.
+        
+          *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
+        - To automatically create a new channel when the channel is closed due to an AMQP exception/error.
+        
+          *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
+        - To ensure correctness of API usage, including values passed to RabbitMQ in AMQ method calls.
+        
+        Example Use
+        -----------
+        The following demonstrates an example of using the library to publish a message with publisher confirmations enabled:
+        
+        .. code-block:: python
+        
+            import asyncio
+            import datetime
+            import uuid
+        
+            import aiorabbit
+        
+            RABBITMQ_URL = 'amqps://guest:guest@localhost:5672/%2f'
+        
+        
+            async def main():
+                async with aiorabbit.connect(RABBITMQ_URL) as client:
+                    await client.confirm_select()
+                    if not await client.publish(
+                            'exchange',
+                            'routing-key',
+                            'message-body',
+                            app_id='example',
+                            message_id=str(uuid.uuid4()),
+                            timestamp=datetime.datetime.utcnow()):
+                        print('Publishing failure')
+        
+            if __name__ == '__main__':
+                asyncio.get_event_loop().run_until_complete(main())
+        
+        Documentation
+        -------------
+        http://aiorabbit.readthedocs.org
+        
+        License
+        -------
+        Copyright (c) 2019-2020 Gavin M. Roy
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification,
+        are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        * Neither the name of the copyright holder nor the names of its contributors may
+          be used to endorse or promote products derived from this software without
+          specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+        IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+        INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+        BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+        DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+        LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+        OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+        ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+        Python Versions Supported
+        -------------------------
+        3.7+
+        
+        .. |Version| image:: https://img.shields.io/pypi/v/aiorabbit.svg?
+           :target: https://pypi.python.org/pypi/aiorabbit
+        
+        .. |Status| image:: https://github.com/gmr/aiorabbit/workflows/Testing/badge.svg?
+           :target: https://github.com/gmr/aiorabbit/actions?workflow=Testing
+           :alt: Build Status
+        
+        .. |Coverage| image:: https://img.shields.io/codecov/c/github/gmr/aiorabbit.svg?
+           :target: https://codecov.io/github/gmr/aiorabbit?branch=master
+        
+        .. |License| image:: https://img.shields.io/pypi/l/aiorabbit.svg?
+           :target: https://aiorabbit.readthedocs.org
+        
 Keywords: amqp,rabbitmq
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: test
-License-File: LICENSE
-
-aiorabbit
-=========
-aiorabbit is an opinionated AsyncIO RabbitMQ client for `Python 3 <https://www.python.org/>`_ (3.7+).
-
-|Version| |Status| |Coverage| |License|
-
-Project Goals
--------------
-- To create a simple, robust `RabbitMQ <https://rabbitmq.com>`_ client library for `AsyncIO <https://docs.python.org/3/library/asyncio.html>`_ development in Python 3.
-- To make use of new features and capabilities in Python 3.7+.
-- Remove some complexity in using an `AMQP <https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol>`_ client by:
-   - Abstracting away the AMQP channel and use it only as a protocol coordination mechanism inside the client.
-   - Remove the `nowait <https://www.rabbitmq.com/amqp-0-9-1-reference.html#domain.no-wait>`_ keyword to ensure a single round-trip pattern of behavior for client usage.
-- To automatically reconnect when a connection is closed due to an AMQP exception/error.
-
-  *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
-- To automatically create a new channel when the channel is closed due to an AMQP exception/error.
-
-  *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
-- To ensure correctness of API usage, including values passed to RabbitMQ in AMQ method calls.
-
-Example Use
------------
-The following demonstrates an example of using the library to publish a message with publisher confirmations enabled:
-
-.. code-block:: python
-
-    import asyncio
-    import datetime
-    import uuid
-
-    import aiorabbit
-
-    RABBITMQ_URL = 'amqps://guest:guest@localhost:5672/%2f'
-
-
-    async def main():
-        async with aiorabbit.connect(RABBITMQ_URL) as client:
-            await client.confirm_select()
-            if not await client.publish(
-                    'exchange',
-                    'routing-key',
-                    'message-body',
-                    app_id='example',
-                    message_id=str(uuid.uuid4()),
-                    timestamp=datetime.datetime.utcnow()):
-                print('Publishing failure')
-
-    if __name__ == '__main__':
-        asyncio.get_event_loop().run_until_complete(main())
-
-Documentation
--------------
-http://aiorabbit.readthedocs.org
-
-License
--------
-Copyright (c) 2019-2023 Gavin M. Roy
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-* Neither the name of the copyright holder nor the names of its contributors may
-  be used to endorse or promote products derived from this software without
-  specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-Python Versions Supported
--------------------------
-3.7+
-
-.. |Version| image:: https://img.shields.io/pypi/v/aiorabbit.svg?
-   :target: https://pypi.python.org/pypi/aiorabbit
-
-.. |Status| image:: https://github.com/gmr/aiorabbit/workflows/Testing/badge.svg?
-   :target: https://github.com/gmr/aiorabbit/actions?workflow=Testing
-   :alt: Build Status
-
-.. |Coverage| image:: https://img.shields.io/codecov/c/github/gmr/aiorabbit.svg?
-   :target: https://codecov.io/github/gmr/aiorabbit?branch=master
-
-.. |License| image:: https://img.shields.io/pypi/l/aiorabbit.svg?
-   :target: https://aiorabbit.readthedocs.org
```

### Comparing `aiorabbit-1.0.0/README.rst` & `aiorabbit-1.0.0a1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 Documentation
 -------------
 http://aiorabbit.readthedocs.org
 
 License
 -------
-Copyright (c) 2019-2023 Gavin M. Roy
+Copyright (c) 2019-2020 Gavin M. Roy
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `aiorabbit-1.0.0/aiorabbit/__init__.py` & `aiorabbit-1.0.0a1/aiorabbit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 # coding: utf-8
 import asyncio
 import contextlib
 import logging
-import ssl
 import typing
 
 from aiorabbit import exceptions
 from aiorabbit.__version__ import version
 
 DEFAULT_LOCALE = 'en-US'
 DEFAULT_PRODUCT = 'aiorabbit/{}'.format(version)
-DEFAULT_URL = 'amqp://guest:guest@localhost'
+DEFAULT_URL = 'amqp://guest:guest@localhost:5672/%2f'
 
 LOGGER = logging.getLogger('aiorabbit')
 
 
 @contextlib.asynccontextmanager
 async def connect(url: str = DEFAULT_URL,
                   locale: str = DEFAULT_LOCALE,
                   product: str = DEFAULT_PRODUCT,
-                  loop: typing.Optional[asyncio.AbstractEventLoop] = None,
-                  on_return: typing.Optional[typing.Callable] = None,
-                  ssl_context: typing.Optional[ssl.SSLContext] = None):
+                  loop: typing.Optional[asyncio.AbstractEventLoop] = None):
     """Asynchronous :ref:`context-manager <python:typecontextmanager>` that
     connects to RabbitMQ, returning a connected
     :class:`~aiorabbit.client.Client` as the target.
 
     .. code-block:: python3
        :caption: Example Usage
 
        async with aiorabbit.connect(RABBITMQ_URL) as client:
             await client.exchange_declare('test', 'topic')
 
     :param url: The URL to connect to RabbitMQ with
     :param locale: The locale for the connection, default `en-US`
     :param product: The product name for the connection, default `aiorabbit`
     :param loop: Optional :mod:`asyncio` event loop to use
-    :param on_return: An optional callback method to be invoked if the server
-        returns a published method. Can also be set using the
-        :meth:`~Client.register_basic_return_callback` method.
-    :param ssl_context: Optional :class:`ssl.SSLContext` for the connection
 
     """
     from aiorabbit import client
 
-    rmq_client = client.Client(
-        url, locale, product, loop, on_return, ssl_context)
+    rmq_client = client.Client(url, locale, product, loop)
     await rmq_client.connect()
     try:
         yield rmq_client
     finally:
         if not rmq_client.is_closed:
             await rmq_client.close()
```

### Comparing `aiorabbit-1.0.0/aiorabbit/channel0.py` & `aiorabbit-1.0.0a1/aiorabbit/channel0.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     state.STATE_UNINITIALIZED: [STATE_PROTOCOL_HEADER_SENT],
     state.STATE_EXCEPTION: [STATE_CLOSE_SENT],
     STATE_PROTOCOL_HEADER_SENT: [STATE_START_RECEIVED],
     STATE_START_RECEIVED: [STATE_STARTOK_SENT],
     STATE_STARTOK_SENT: [STATE_TUNE_RECEIVED, STATE_CLOSE_RECEIVED],
     STATE_TUNE_RECEIVED: [STATE_TUNEOK_SENT],
     STATE_TUNEOK_SENT: [STATE_OPEN_SENT, STATE_CLOSE_RECEIVED],
-    STATE_OPEN_SENT: [STATE_OPENOK_RECEIVED, STATE_CLOSE_RECEIVED],
+    STATE_OPEN_SENT: [STATE_OPENOK_RECEIVED],
     STATE_OPENOK_RECEIVED: [
         STATE_BLOCKED_RECEIVED,
         STATE_HEARTBEAT_RECEIVED,
         STATE_CLOSE_RECEIVED,
         STATE_CLOSE_SENT],
     STATE_CLOSE_RECEIVED: [STATE_CLOSEOK_SENT],
     STATE_CLOSE_SENT: [STATE_CLOSEOK_RECEIVED],
@@ -124,15 +124,15 @@
         self.blocked = blocked
         self.max_channels = max_channels
         self.max_frame_size = constants.FRAME_MAX_SIZE
         self.properties: dict = {}
         self._heartbeat_interval = heartbeat_interval
         self._heartbeat_timer: typing.Optional[asyncio.TimerHandle] = None
         self._last_error: typing.Tuple[int, typing.Optional[str]] = (0, None)
-        self._last_heartbeat: int = 0
+        self._last_heartbeat = 0
         self._locale = locale
         self._on_remote_close = on_remote_close
         self._password = password
         self._product = product
         self._transport: typing.Optional[asyncio.Transport] = None
         self._username = username
         self._virtual_host = virtual_host
@@ -202,29 +202,23 @@
 
     @property
     def is_closed(self) -> bool:
         return self._state in [STATE_CLOSEOK_RECEIVED,
                                STATE_CLOSEOK_SENT,
                                state.STATE_EXCEPTION]
 
-    def update_last_heartbeat(self) -> None:
-        """Invoked by the client whenever traffic is received"""
-        self._last_heartbeat = self._loop.time()
-
     def _heartbeat_check(self):
         threshold = self._loop.time() - (self._heartbeat_interval * 2)
-        if 0 < self._last_heartbeat < threshold:
+        if self._last_heartbeat < threshold:
             msg = 'No heartbeat in {:2f} seconds'.format(
                 self._loop.time() - self._last_heartbeat)
             self._logger.critical(msg)
             self._heartbeat_timer = None
             self._on_remote_close(599, 'Too many missed heartbeats')
         else:
-            if self._heartbeat_timer:
-                self._heartbeat_timer.cancel()
             self._heartbeat_timer = self._loop.call_later(
                 self._heartbeat_interval, self._heartbeat_check)
 
     @staticmethod
     def _negotiate(client: int, server: int) -> int:
         """Return the negotiated value between what the client has requested
         and the server has requested for how the two will communicate.
```

### Comparing `aiorabbit-1.0.0/aiorabbit/client.py` & `aiorabbit-1.0.0a1/aiorabbit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import asyncio
 import collections
 import dataclasses
 import datetime
 import math
 import re
 import socket
-import ssl
 import typing
 from urllib import parse
 
 from pamqp import base, body, commands, frame, header
 import yarl
 
 from aiorabbit import (channel0, DEFAULT_LOCALE, DEFAULT_PRODUCT, DEFAULT_URL,
@@ -309,24 +308,24 @@
 
 class Client(state.StateManager):
     """AsyncIO RabbitMQ Client
 
     This client provides a streamlined interface for interacting with RabbitMQ.
 
     Instead of manually managing your channels, the client will do so for you.
-    In addition, if you are disconnected remotely due to an error, it will
+    In addition if you are disconnected remotely due to an error, it will
     attempt to automatically reconnect. Any non-connection related exception
     should leave you in a state where you can continue working with RabbitMQ,
     even if it disconnected the client as part of the exception.
 
     .. note:: AMQ Methods vs Opinionated Methods
 
         For the most part, the client directly implements the AMQ model
         combining class and method RPC calls as a function. For example,
-        ``Basic.Ack`` is implemented as :meth:`Client.basic_ack`. However, some
+        ``Basic.Ack`` is implemented as :meth:`Client.basic_ack`. However some
         methods, such as :meth:`Client.consume`, :meth:`Client.publish`, and
         :meth:`Client.qos_prefetch` provide a higher-level and more opinionated
         implementation than their respected AMQ RPC methods.
 
     :param url: The URL to connect to RabbitMQ with
     :param locale: The locale to specify for the RabbitMQ connection
     :param product: The project name to specify for the RabbitMQ connection
@@ -343,25 +342,23 @@
 
         client = Client(RABBITMQ_URL)
         await client.connect()
         await client.exchange_declare('test', 'topic')
         await client.close()
 
     """
-    CONNECTING_EXCEPTIONS = (exceptions.AccessRefused, exceptions.NotAllowed)
     STATE_MAP = _STATE_MAP
     STATE_TRANSITIONS = _STATE_TRANSITIONS
 
     def __init__(self,
                  url: str = DEFAULT_URL,
                  locale: str = DEFAULT_LOCALE,
                  product: str = DEFAULT_PRODUCT,
                  loop: typing.Optional[asyncio.AbstractEventLoop] = None,
-                 on_return: typing.Optional[typing.Callable] = None,
-                 ssl_context: typing.Optional[ssl.SSLContext] = None):
+                 on_return: typing.Optional[typing.Callable] = None):
         super().__init__(loop or asyncio.get_running_loop())
         self._blocked = asyncio.Event()
         self._block_write = asyncio.Event()
         self._channel: int = 0
         self._channel0: typing.Optional[channel0.Channel0] = None
         self._channel_open = asyncio.Event()
         self._confirmation_result: typing.Dict[int, bool] = {}
@@ -378,16 +375,14 @@
         self._on_channel_close: typing.Optional[typing.Callable] = None
         self._on_message_return: typing.Optional[typing.Callable] = on_return
         self._pending_consumers: typing.Deque[
             (asyncio.Future, typing.Callable)] = collections.deque([])
         self._protocol: typing.Optional[asyncio.Protocol] = None
         self._publisher_confirms = False
         self._rpc_lock = asyncio.Lock()
-        self._close_lock = asyncio.Lock()
-        self._ssl_context = ssl_context
         self._transactional = False
         self._transport: typing.Optional[asyncio.Transport] = None
         self._url = yarl.URL(url)
         self._set_state(STATE_DISCONNECTED)
 
     async def connect(self) -> None:
         """Connect to the RabbitMQ Server
@@ -422,32 +417,25 @@
             self._reset()
             self._logger.critical('Failed to connect to RabbitMQ: %s', exc)
             raise exc
         await self._open_channel()
 
     async def close(self) -> None:
         """Close the client connection to the server"""
-        async with self._close_lock:
-            if self.is_closed or not self._channel0 or not self._transport:
-                self._logger.warning(
-                    'Close called when connection is not open')
-                if self._state != STATE_CLOSED:
-                    self._set_state(STATE_CLOSED)
-                return
-            if self._channel_open.is_set():
-                await self._send_rpc(
-                    commands.Channel.Close(200, 'Client Requested', 0, 0),
-                    STATE_CHANNEL_CLOSE_SENT,
-                    STATE_CHANNEL_CLOSEOK_RECEIVED)
-            await self._close()
-
-    @property
-    def is_connected(self) -> bool:
-        """Indicates if the connection is available"""
-        return not self.is_closed
+        if self.is_closed or not self._channel0 or not self._transport:
+            self._logger.warning('Close called when connection is not open')
+            if self._state != STATE_CLOSED:
+                self._set_state(STATE_CLOSED)
+            return
+        if self._channel_open.is_set():
+            await self._send_rpc(
+                commands.Channel.Close(200, 'Client Requested', 0, 0),
+                STATE_CHANNEL_CLOSE_SENT,
+                STATE_CHANNEL_CLOSEOK_RECEIVED)
+        await self._close()
 
     @property
     def is_closed(self) -> bool:
         """Indicates if the connection is closed or closing"""
         return (not self._channel0
                 or (self._channel0 and self._channel0.is_closed)
                 or self._state in [STATE_CLOSING,
@@ -662,15 +650,15 @@
             elif not 0 < priority < 256:
                 raise ValueError('priority must be between 0 and 256')
         if message_type:
             self._validate_short_str('message_type', message_type)
         if reply_to:
             self._validate_short_str('reply_to', reply_to)
         if timestamp and not isinstance(timestamp, datetime.datetime):
-            raise TypeError('timestamp must be of type datetime.datetime')
+            raise TypeError('reply_to must be of type datetime.datetime')
         if user_id:
             self._validate_short_str('user_id', user_id)
 
         if isinstance(message_body, str):
             message_body = message_body.encode('utf-8')
         self._delivery_tag += 1
         if self._publisher_confirms:
@@ -1394,44 +1382,43 @@
         await self._channel0.close()
         self._transport.close()
         self._set_state(STATE_CLOSED)
         self._reset()
 
     async def _connect(self) -> None:
         self._set_state(STATE_CONNECTING)
-        port = self._url.port
-        if port is None:
-            port = 5671 if self._url.scheme == 'amqps' else 5672
-        self._logger.info(
-            'Connecting to %s://%s:%s@%s:%s/%s',
-            self._url.scheme, self._url.user,
-            ''.ljust(len(self._url.password), '*'),
-            self._url.host, port, parse.quote(self._url.path[1:], ''))
+        self._logger.info('Connecting to %s://%s:%s@%s:%s/%s',
+                          self._url.scheme, self._url.user,
+                          ''.ljust(len(self._url.password), '*'),
+                          self._url.host, self._url.port,
+                          parse.quote(self._url.path[1:], ''))
         heartbeat = self._url.query.get('heartbeat')
         self._channel0 = channel0.Channel0(
             self._blocked,
             self._url.user,
             self._url.password,
-            self._url.path[1:] if self._url.path[1:] else '/',
+            self._url.path[1:],
             int(heartbeat) if heartbeat else None,
             self._defaults.locale,
             self._loop,
             int(self._url.query.get('channel_max', '32768')),
             self._defaults.product,
             self._on_remote_close)
         self._max_frame_size = float(self._channel0.max_frame_size)
-        ssl_enabled = self._url.scheme == 'amqps'
+
+        ssl = self._url.scheme == 'amqps'
+
         future = self._loop.create_connection(
             lambda: protocol.AMQP(
                 self._on_connected,
                 self._on_disconnected,
                 self._on_frame,
-            ), self._url.host, port,
-            server_hostname=self._url.host if ssl_enabled else None,
-            ssl=self._ssl_context or ssl_enabled)
+            ), self._url.host, self._url.port,
+            server_hostname=self._url.host if ssl else None,
+            ssl=ssl)
         self._transport, self._protocol = await asyncio.wait_for(
             future, timeout=self._connect_timeout)
         self._max_frame_size = float(self._channel0.max_frame_size)
         if await self._channel0.open(self._transport):
             return self._set_state(STATE_OPENED)
         await self._wait_on_state(STATE_OPENED)  # To catch connection errors
 
@@ -1464,20 +1451,16 @@
                 STATE_CLOSED,
                 exceptions.ConnectionClosedException(
                     'Socket closed' if not exc else str(exc)))
 
     def _on_frame(self, channel: int, value: frame.FrameTypes) -> None:
         self._last_frame = value
         if channel == 0:
-            return self._channel0.process(value)
-
-        # Reset last heartbeat timestamp since a frame was received
-        self._channel0.update_last_heartbeat()
-
-        if isinstance(value, commands.Basic.Ack):
+            self._channel0.process(value)
+        elif isinstance(value, commands.Basic.Ack):
             self._set_delivery_tag_result(value.delivery_tag, True)
             self._set_state(STATE_BASIC_ACK_RECEIVED)
         elif isinstance(value, commands.Basic.CancelOk):
             del self._consumers[value.consumer_tag]
             self._set_state(STATE_BASIC_CANCELOK_RECEIVED)
         elif isinstance(value, commands.Basic.ConsumeOk):
             future, callback = self._pending_consumers.popleft()
@@ -1601,17 +1584,18 @@
 
     async def _post_wait_on_state(
             self, result: int = 0,
             exc: typing.Optional[exceptions.AIORabbitException] = None,
             raise_on_channel_close: bool = False) -> int:
         """Process results from Client._send_rpc and Client._wait_on_state"""
         if exc:
-            await asyncio.sleep(0.001)  # Let pending things happen
-            await self._reconnect()
             err = self._get_last_error()
+            if not isinstance(exc, exceptions.AccessRefused):
+                await asyncio.sleep(0.001)  # Let pending things happen
+                await self._reconnect()
             raise exceptions.CLASS_MAPPING[err[0]](err[1])
         if result == STATE_CHANNEL_CLOSE_RECEIVED and self._last_error[0] > 0:
             await self._open_channel()
             await asyncio.sleep(0.001)  # Sleep to let pending things happen
             if raise_on_channel_close:
                 err = self._get_last_error()
                 raise exceptions.CLASS_MAPPING[err[0]](err[1])
@@ -1702,12 +1686,10 @@
             self._transport.write(frame.marshal(value, self._channel))
 
     async def _wait_on_state(self, *args: int) -> int:
         args = list(args) + [STATE_CHANNEL_CLOSE_RECEIVED]
         try:
             result = await super()._wait_on_state(*args)
         except exceptions.AIORabbitException as exc:
-            if isinstance(exc, self.CONNECTING_EXCEPTIONS):
-                raise
             await self._post_wait_on_state(exc=exc)
         else:
             return await self._post_wait_on_state(result)
```

### Comparing `aiorabbit-1.0.0/aiorabbit/exceptions.py` & `aiorabbit-1.0.0a1/aiorabbit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiorabbit-1.0.0/aiorabbit/message.py` & `aiorabbit-1.0.0a1/aiorabbit/message.py`

 * *Files identical despite different names*

### Comparing `aiorabbit-1.0.0/aiorabbit/protocol.py` & `aiorabbit-1.0.0a1/aiorabbit/protocol.py`

 * *Files identical despite different names*

### Comparing `aiorabbit-1.0.0/aiorabbit/state.py` & `aiorabbit-1.0.0a1/aiorabbit/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,57 +70,54 @@
         self._state_start = self._loop.time()
         self._exc = None
         self._waits = {}
 
     def _set_state(self, value: int,
                    exc: typing.Optional[Exception] = None) -> None:
         self._logger.debug(
-            'Set state to 0x%x: %s while state is 0x%x: %s - %r [%r]',
+            'Set state to %i: %s while state is %i: %s - %r [%r]',
             value, self.state_description(value), self._state, self.state,
             self._waits, exc)
         if value == self._state and exc == self._exception:
             return
         elif value != STATE_EXCEPTION \
                 and value not in self.STATE_TRANSITIONS[self._state]:
-            exc = exceptions.StateTransitionError(
+            raise exceptions.StateTransitionError(
                 'Invalid state transition from {!r} to {!r}'.format(
                     self.state, self.state_description(value)))
-            self._exception = exc
-            raise exc
         self._logger.debug(
-            'Transition to 0x%x: %s from 0x%x: %s after %.4f seconds',
+            'Transition to %i: %s from %i: %s after %.4f seconds',
             value, self.state_description(value),
             self._state, self.state, self.time_in_state)
         self._exception = exc
         self._state = value
         self._state_start = self._loop.time()
         if self._state in self._waits:
             [self._loop.call_soon(event.set)
              for event in self._waits[self._state].values()]
 
     async def _wait_on_state(self, *args) -> int:
         """Wait on a specific state value to transition"""
         wait_id, waits = time.monotonic_ns(), []
         self._logger.debug(
-            'Waiter %i waiting on (%s) while in 0x%x: %s',
+            'Waiter %i waiting on (%s) while in %i: %s',
             wait_id, ' || '.join(
                 '{}: {}'.format(s, self.state_description(s))
                 for s in args), self._state, self.state)
         for state in args:
             if state not in self._waits:
                 self._waits[state] = {}
             self._waits[state][wait_id] = asyncio.Event()
             waits.append((state, self._waits[state][wait_id]))
         while not self._exception:
             for state, event in waits:
                 if event.is_set():
                     self._logger.debug(
-                        'Waiter %r wait on 0x%x: %s has finished [%r]',
-                        wait_id, state, self.state_description(state),
-                        self._exception)
+                        'Waiter %r wait on %i: %s has finished [%r]', wait_id,
+                        state, self.state_description(state), self._exception)
                     self._clear_waits(wait_id)
                     return state
             await asyncio.sleep(0.001)
         self._clear_waits(wait_id)
         exc = self._exception
         self._exception = None
         raise exc
```

### Comparing `aiorabbit-1.0.0/aiorabbit/types.py` & `aiorabbit-1.0.0a1/aiorabbit/types.py`

 * *Files identical despite different names*

### Comparing `aiorabbit-1.0.0/aiorabbit.egg-info/PKG-INFO` & `aiorabbit-1.0.0a1/aiorabbit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,126 @@
 Metadata-Version: 2.1
 Name: aiorabbit
-Version: 1.0.0
+Version: 1.0.0a1
 Summary: An AsyncIO RabbitMQ Client Library
 Home-page: https://github.com/gmr/aiorabbit
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/aiorabbit/issues
 Project-URL: Documentation, https://aiorabbit.readthedocs.io
 Project-URL: Source Code, https://github.com/gmr/aiorabbit/
+Description: aiorabbit
+        =========
+        aiorabbit is an opinionated AsyncIO RabbitMQ client for `Python 3 <https://www.python.org/>`_ (3.7+).
+        
+        |Version| |Status| |Coverage| |License|
+        
+        Project Goals
+        -------------
+        - To create a simple, robust `RabbitMQ <https://rabbitmq.com>`_ client library for `AsyncIO <https://docs.python.org/3/library/asyncio.html>`_ development in Python 3.
+        - To make use of new features and capabilities in Python 3.7+.
+        - Remove some complexity in using an `AMQP <https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol>`_ client by:
+           - Abstracting away the AMQP channel and use it only as a protocol coordination mechanism inside the client.
+           - Remove the `nowait <https://www.rabbitmq.com/amqp-0-9-1-reference.html#domain.no-wait>`_ keyword to ensure a single round-trip pattern of behavior for client usage.
+        - To automatically reconnect when a connection is closed due to an AMQP exception/error.
+        
+          *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
+        - To automatically create a new channel when the channel is closed due to an AMQP exception/error.
+        
+          *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
+        - To ensure correctness of API usage, including values passed to RabbitMQ in AMQ method calls.
+        
+        Example Use
+        -----------
+        The following demonstrates an example of using the library to publish a message with publisher confirmations enabled:
+        
+        .. code-block:: python
+        
+            import asyncio
+            import datetime
+            import uuid
+        
+            import aiorabbit
+        
+            RABBITMQ_URL = 'amqps://guest:guest@localhost:5672/%2f'
+        
+        
+            async def main():
+                async with aiorabbit.connect(RABBITMQ_URL) as client:
+                    await client.confirm_select()
+                    if not await client.publish(
+                            'exchange',
+                            'routing-key',
+                            'message-body',
+                            app_id='example',
+                            message_id=str(uuid.uuid4()),
+                            timestamp=datetime.datetime.utcnow()):
+                        print('Publishing failure')
+        
+            if __name__ == '__main__':
+                asyncio.get_event_loop().run_until_complete(main())
+        
+        Documentation
+        -------------
+        http://aiorabbit.readthedocs.org
+        
+        License
+        -------
+        Copyright (c) 2019-2020 Gavin M. Roy
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification,
+        are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        * Neither the name of the copyright holder nor the names of its contributors may
+          be used to endorse or promote products derived from this software without
+          specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+        IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+        INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+        BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+        DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+        LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+        OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+        ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+        Python Versions Supported
+        -------------------------
+        3.7+
+        
+        .. |Version| image:: https://img.shields.io/pypi/v/aiorabbit.svg?
+           :target: https://pypi.python.org/pypi/aiorabbit
+        
+        .. |Status| image:: https://github.com/gmr/aiorabbit/workflows/Testing/badge.svg?
+           :target: https://github.com/gmr/aiorabbit/actions?workflow=Testing
+           :alt: Build Status
+        
+        .. |Coverage| image:: https://img.shields.io/codecov/c/github/gmr/aiorabbit.svg?
+           :target: https://codecov.io/github/gmr/aiorabbit?branch=master
+        
+        .. |License| image:: https://img.shields.io/pypi/l/aiorabbit.svg?
+           :target: https://aiorabbit.readthedocs.org
+        
 Keywords: amqp,rabbitmq
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: test
-License-File: LICENSE
-
-aiorabbit
-=========
-aiorabbit is an opinionated AsyncIO RabbitMQ client for `Python 3 <https://www.python.org/>`_ (3.7+).
-
-|Version| |Status| |Coverage| |License|
-
-Project Goals
--------------
-- To create a simple, robust `RabbitMQ <https://rabbitmq.com>`_ client library for `AsyncIO <https://docs.python.org/3/library/asyncio.html>`_ development in Python 3.
-- To make use of new features and capabilities in Python 3.7+.
-- Remove some complexity in using an `AMQP <https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol>`_ client by:
-   - Abstracting away the AMQP channel and use it only as a protocol coordination mechanism inside the client.
-   - Remove the `nowait <https://www.rabbitmq.com/amqp-0-9-1-reference.html#domain.no-wait>`_ keyword to ensure a single round-trip pattern of behavior for client usage.
-- To automatically reconnect when a connection is closed due to an AMQP exception/error.
-
-  *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
-- To automatically create a new channel when the channel is closed due to an AMQP exception/error.
-
-  *When such a behavior is encountered, the exception is raised, but the client continues to operate if the user catches and logs the error.*
-- To ensure correctness of API usage, including values passed to RabbitMQ in AMQ method calls.
-
-Example Use
------------
-The following demonstrates an example of using the library to publish a message with publisher confirmations enabled:
-
-.. code-block:: python
-
-    import asyncio
-    import datetime
-    import uuid
-
-    import aiorabbit
-
-    RABBITMQ_URL = 'amqps://guest:guest@localhost:5672/%2f'
-
-
-    async def main():
-        async with aiorabbit.connect(RABBITMQ_URL) as client:
-            await client.confirm_select()
-            if not await client.publish(
-                    'exchange',
-                    'routing-key',
-                    'message-body',
-                    app_id='example',
-                    message_id=str(uuid.uuid4()),
-                    timestamp=datetime.datetime.utcnow()):
-                print('Publishing failure')
-
-    if __name__ == '__main__':
-        asyncio.get_event_loop().run_until_complete(main())
-
-Documentation
--------------
-http://aiorabbit.readthedocs.org
-
-License
--------
-Copyright (c) 2019-2023 Gavin M. Roy
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-* Neither the name of the copyright holder nor the names of its contributors may
-  be used to endorse or promote products derived from this software without
-  specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-Python Versions Supported
--------------------------
-3.7+
-
-.. |Version| image:: https://img.shields.io/pypi/v/aiorabbit.svg?
-   :target: https://pypi.python.org/pypi/aiorabbit
-
-.. |Status| image:: https://github.com/gmr/aiorabbit/workflows/Testing/badge.svg?
-   :target: https://github.com/gmr/aiorabbit/actions?workflow=Testing
-   :alt: Build Status
-
-.. |Coverage| image:: https://img.shields.io/codecov/c/github/gmr/aiorabbit.svg?
-   :target: https://codecov.io/github/gmr/aiorabbit?branch=master
-
-.. |License| image:: https://img.shields.io/pypi/l/aiorabbit.svg?
-   :target: https://aiorabbit.readthedocs.org
```

### Comparing `aiorabbit-1.0.0/setup.cfg` & `aiorabbit-1.0.0a1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Topic :: Communications
 	Topic :: Internet
 	Topic :: Software Development
-	Typing :: Typed
 requires-dist = setuptools
 keywords = 
 	amqp
 	rabbitmq
 
 [options]
 include_package_data = True
@@ -50,15 +48,14 @@
 	flake8-import-order
 	flake8-print
 	flake8-quotes
 	flake8-rst-docstrings
 	flake8-tuple
 	mypy
 	pygments
-	pytest
 
 [coverage:run]
 branch = True
 command_line = -m unittest discover --verbose
 data_file = build/.coverage
 
 [coverage:report]
@@ -71,15 +68,15 @@
 
 [coverage:xml]
 output = build/coverage.xml
 
 [flake8]
 application-import-names = aiorabbit, tests
 exclude = build,docs,env
-ignore = RST306,RST307,RST399,W503
+ignore = RST306,RST399,W503
 import-order-style = google
 rst-directives = seealso
 rst-roles = attr,class,const,data,exc,func,meth,mod,obj,ref,yields
 
 [mypy]
 check_untyped_defs = True
 disallow_incomplete_defs = True
```

