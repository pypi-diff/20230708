# Comparing `tmp/sockets-communication-1.4.0.tar.gz` & `tmp/sockets-communication-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.4.0.tar", last modified: Sat Jul  8 10:38:09 2023, max compression
+gzip compressed data, was "sockets-communication-1.4.1.tar", last modified: Sat Jul  8 15:51:08 2023, max compression
```

## Comparing `sockets-communication-1.4.0.tar` & `sockets-communication-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.537481 sockets-communication-1.4.0/
--rw-rw-rw-   0        0        0       98 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-08 10:38:09.536514 sockets-communication-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.4.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.4.0/build.py
--rw-rw-rw-   0        0        0      708 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 10:38:09.537481 sockets-communication-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-08 10:38:00.000000 sockets-communication-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.519479 sockets-communication-1.4.0/sockets_communication/
--rw-rw-rw-   0        0        0      364 2023-07-08 10:32:37.000000 sockets-communication-1.4.0/sockets_communication/bluetooth.py
--rw-rw-rw-   0        0        0     5793 2023-07-08 10:35:48.000000 sockets-communication-1.4.0/sockets_communication/client.py
--rw-rw-rw-   0        0        0     3766 2023-07-08 10:29:31.000000 sockets-communication-1.4.0/sockets_communication/communication.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.4.0/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.4.0/sockets_communication/process.py
--rw-rw-rw-   0        0        0    14757 2023-07-08 10:37:45.000000 sockets-communication-1.4.0/sockets_communication/server.py
--rw-rw-rw-   0        0        0     7899 2023-07-07 15:47:06.000000 sockets-communication-1.4.0/sockets_communication/service.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.536514 sockets-communication-1.4.0/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 15:51:08.226224 sockets-communication-1.4.1/
+-rw-rw-rw-   0        0        0       98 2023-07-08 15:51:06.000000 sockets-communication-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-08 15:51:08.226224 sockets-communication-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.4.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.4.1/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-08 15:51:06.000000 sockets-communication-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.4.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:51:08.226224 sockets-communication-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-08 15:50:53.000000 sockets-communication-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:51:08.211224 sockets-communication-1.4.1/sockets_communication/
+-rw-rw-rw-   0        0        0      364 2023-07-08 10:32:37.000000 sockets-communication-1.4.1/sockets_communication/bluetooth.py
+-rw-rw-rw-   0        0        0     5786 2023-07-08 15:47:06.000000 sockets-communication-1.4.1/sockets_communication/client.py
+-rw-rw-rw-   0        0        0     3624 2023-07-08 15:47:46.000000 sockets-communication-1.4.1/sockets_communication/communication.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.4.1/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.4.1/sockets_communication/process.py
+-rw-rw-rw-   0        0        0    14999 2023-07-08 15:50:44.000000 sockets-communication-1.4.1/sockets_communication/server.py
+-rw-rw-rw-   0        0        0     8013 2023-07-08 15:50:44.000000 sockets-communication-1.4.1/sockets_communication/service.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:51:08.225255 sockets-communication-1.4.1/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-08 15:51:08.000000 sockets-communication-1.4.1/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-07-08 15:51:08.000000 sockets-communication-1.4.1/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:51:08.000000 sockets-communication-1.4.1/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-08 15:51:08.000000 sockets-communication-1.4.1/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 15:51:08.000000 sockets-communication-1.4.1/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.4.0/PKG-INFO` & `sockets-communication-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.4.0
+Version: 1.4.1
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.4.0/README.md` & `sockets-communication-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.0/build.py` & `sockets-communication-1.4.1/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.0/pyproject.toml` & `sockets-communication-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.4.0'
+version = '1.4.1'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.4.0/setup.py` & `sockets-communication-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.4.0',
+        version='1.4.1',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.4.0/sockets_communication/client.py` & `sockets-communication-1.4.1/sockets_communication/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Defines the server address and creates the client object.
 
         :param connection: The connection socket.
         :param host: The ip address of the server.
         :param port: The port for the server connection.
         """
 
-        self.connection: Optional[socket.socket] = connection
+        self.connection: Optional[Socket] = connection
 
         self.host: Optional[str] = host
         self.port: Optional[int] = port
     # end __init__
 
     def validate_connection(self) -> None:
         """Validates the connection object."""
```

### Comparing `sockets-communication-1.4.0/sockets_communication/communication.py` & `sockets-communication-1.4.1/sockets_communication/communication.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # communication.py
 
 from abc import ABCMeta
 import socket
-from typing import Union, Tuple
 
 __all__ = [
     "Components",
     "Communication"
 ]
 
 Socket = socket.socket
-Host = str
-Port = Union[str, int]
-Address = Tuple[Host, Port]
-Number = Union[int, float]
 
 class Components(metaclass=ABCMeta):
     """Defines the basic parameters for the communication."""
 
     HEADER = 64
 
     ENCODING = 'utf-8'
@@ -99,21 +94,21 @@
         :param connection: The sockets' connection object.
         """
 
         message_len = len(message)
 
         connection.send(
             (
-                    str(message_len) + " " *
-                    (self.HEADER - len(str(message_len)))
+                str(message_len) + " " *
+                (self.HEADER - len(str(message_len)))
             ).encode(self.ENCODING)
         )
 
         iterations = (
-                message_len // self.SIZE + 1 + message_len % self.SIZE
+            message_len // self.SIZE + 1 + message_len % self.SIZE
         )
 
         for i in range(0, iterations, self.SIZE):
             if len(message[i:]) >= self.SIZE:
                 connection.send(message[i:self.SIZE])
 
             else:
@@ -138,15 +133,15 @@
                 replace(" ", "")
             )
         )
 
         message = b''
 
         iterations = (
-                message_len // self.SIZE + 1 + message_len % self.SIZE
+            message_len // self.SIZE + 1 + message_len % self.SIZE
         )
 
         for i in range(0, iterations, self.SIZE):
             if (i < iterations - 1) or (message_len % self.SIZE == 0):
                 message += connection.recv(self.SIZE)
 
             else:
```

### Comparing `sockets-communication-1.4.0/sockets_communication/exceptions.py` & `sockets-communication-1.4.1/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.0/sockets_communication/process.py` & `sockets-communication-1.4.1/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.0/sockets_communication/server.py` & `sockets-communication-1.4.1/sockets_communication/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,28 @@
 Address = Tuple[Host, Port]
 Number = Union[int, float]
 
 @represent
 class ClientsCollection:
     """A data class to contain clients within the server data."""
 
+    __slots__ = "clients",
+
     def __init__(self, clients: Optional[dict] = None) -> None:
         """
         Defines the base data class to contain the clients.
 
         :param clients: The base dictionary to contain the clients' data.
         """
 
-        self.clients = clients or {}
+        if clients is None:
+            clients = {}
+        # end if
+
+        self.clients = clients
     # end __init__
 
     # defines a method to set a client
     def set_client(
             self, address: Address, connection: Optional[Socket] = None
     ) -> None:
         """
@@ -88,14 +94,19 @@
         self.pop_client(address)
     # end remove_client
 # end ClientsCollection
 
 class SocketServer(Communication, ServiceInterface):
     """The server object to control the communication ith multiple clients."""
 
+    __slots__ = (
+        "connection", "host", "port", "_serving_process",
+        "_running_parameters", "_connected", "_serving", "clients"
+    )
+
     def __init__(
             self,
             connection: Optional[Socket] = None, *,
             host: Optional[Host] = None,
             port: Optional[Port] = None
     ) -> None:
         """
@@ -109,15 +120,15 @@
         ServiceInterface.__init__(self)
 
         self.connection: Optional[socket.socket] = connection
 
         self.host: Optional[str] = host
         self.port: Optional[int] = port
 
-        self._listening_process: Optional[threading.Thread] = None
+        self._serving_process: Optional[threading.Thread] = None
 
         self._running_parameters: Optional[Dict[str, Any]] = None
 
         self._connected = False
         self._serving = False
 
         self.clients = ClientsCollection()
@@ -138,15 +149,15 @@
     def created(self) -> bool:
         """
         Checks if the service was created.
 
         :return: The value for the service being created.
         """
 
-        return isinstance(self._listening_process, threading.Thread)
+        return isinstance(self._serving_process, threading.Thread)
     # end created
 
     @property
     def serving(self) -> bool:
         """
         Checks if the service is currently serving.
 
@@ -253,15 +264,15 @@
         :param daemon: The value to set the process as daemon.
         """
 
         if not self.connected:
             self.connect(connection=connection, host=host, port=port)
         # end if
 
-        self._listening_process = threading.Thread(
+        self._serving_process = threading.Thread(
             target=self.listen, daemon=daemon
         )
     # end create
 
     def start_serving(
             self,
             connection: Optional[Socket] = None,
@@ -287,15 +298,15 @@
         if not self.created:
             self.create(
                 connection=connection, host=host,
                 port=port, daemon=daemon
             )
         # end if
 
-        self._listening_process.start()
+        self._serving_process.start()
     # end start_serving
 
     def run(
             self,
             connection: Optional[Socket] = None,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
@@ -392,16 +403,16 @@
     def stop_serving(self) -> None:
         """Stops the serving process."""
 
         if self.serving:
             self._serving = False
         # end if
 
-        if self.created and self._listening_process.is_alive():
-            self._listening_process = None
+        if self.created and self._serving_process.is_alive():
+            self._serving_process = None
         # end if
     # end stop_serving
 
     def terminate(self) -> None:
         """Pauses the process of service."""
 
         super().terminate()
```

### Comparing `sockets-communication-1.4.0/sockets_communication/service.py` & `sockets-communication-1.4.1/sockets_communication/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 import warnings
 import time
 import datetime as dt
 from typing import Optional, Union
 
 from represent import represent
 
-Number = Union[int, float]
-Host = str
-Port = Union[str, int]
-
 __all__ = [
     "ServiceInterface"
 ]
 
+Number = Union[int, float]
+
 @represent
 class ServiceInterface:
     """The server object to control the communication ith multiple clients."""
 
     SLEEP = 0.01
 
+    __slots__ = (
+        "_timeout_process", "_updating_process", "_refreshing_process",
+        "_blocking", "_updating", "_refreshing"
+    )
+
     def __init__(self) -> None:
         """Defines the server datasets for clients and client commands."""
 
         self._timeout_process: Optional[threading.Thread] = None
         self._updating_process: Optional[threading.Thread] = None
         self._refreshing_process: Optional[threading.Thread] = None
```

### Comparing `sockets-communication-1.4.0/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.4.1/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.4.0
+Version: 1.4.1
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.4.0/sockets_communication.egg-info/SOURCES.txt` & `sockets-communication-1.4.1/sockets_communication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

