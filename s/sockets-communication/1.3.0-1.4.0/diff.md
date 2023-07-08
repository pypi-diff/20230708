# Comparing `tmp/sockets-communication-1.3.0.tar.gz` & `tmp/sockets-communication-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.3.0.tar", last modified: Fri Jul  7 16:04:58 2023, max compression
+gzip compressed data, was "sockets-communication-1.4.0.tar", last modified: Sat Jul  8 10:38:09 2023, max compression
```

## Comparing `sockets-communication-1.3.0.tar` & `sockets-communication-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:58.884920 sockets-communication-1.3.0/
--rw-rw-rw-   0        0        0       98 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-07 16:04:58.883887 sockets-communication-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.3.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.3.0/build.py
--rw-rw-rw-   0        0        0      708 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 16:04:58.884920 sockets-communication-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-07 16:04:50.000000 sockets-communication-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:58.873569 sockets-communication-1.3.0/sockets_communication/
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.3.0/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.3.0/sockets_communication/process.py
--rw-rw-rw-   0        0        0     7899 2023-07-07 15:47:06.000000 sockets-communication-1.3.0/sockets_communication/service.py
--rw-rw-rw-   0        0        0    23253 2023-07-07 16:04:42.000000 sockets-communication-1.3.0/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:04:58.882886 sockets-communication-1.3.0/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 16:04:58.000000 sockets-communication-1.3.0/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.537481 sockets-communication-1.4.0/
+-rw-rw-rw-   0        0        0       98 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-08 10:38:09.536514 sockets-communication-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.4.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.4.0/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:38:09.537481 sockets-communication-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-08 10:38:00.000000 sockets-communication-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.519479 sockets-communication-1.4.0/sockets_communication/
+-rw-rw-rw-   0        0        0      364 2023-07-08 10:32:37.000000 sockets-communication-1.4.0/sockets_communication/bluetooth.py
+-rw-rw-rw-   0        0        0     5793 2023-07-08 10:35:48.000000 sockets-communication-1.4.0/sockets_communication/client.py
+-rw-rw-rw-   0        0        0     3766 2023-07-08 10:29:31.000000 sockets-communication-1.4.0/sockets_communication/communication.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.4.0/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.4.0/sockets_communication/process.py
+-rw-rw-rw-   0        0        0    14757 2023-07-08 10:37:45.000000 sockets-communication-1.4.0/sockets_communication/server.py
+-rw-rw-rw-   0        0        0     7899 2023-07-07 15:47:06.000000 sockets-communication-1.4.0/sockets_communication/service.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:38:09.536514 sockets-communication-1.4.0/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 10:38:09.000000 sockets-communication-1.4.0/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.3.0/PKG-INFO` & `sockets-communication-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.3.0
+Version: 1.4.0
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.3.0/README.md` & `sockets-communication-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.3.0/build.py` & `sockets-communication-1.4.0/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.3.0/pyproject.toml` & `sockets-communication-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.3.0'
+version = '1.4.0'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.3.0/setup.py` & `sockets-communication-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.3.0',
+        version='1.4.0',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.3.0/sockets_communication/exceptions.py` & `sockets-communication-1.4.0/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.3.0/sockets_communication/process.py` & `sockets-communication-1.4.0/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.3.0/sockets_communication/service.py` & `sockets-communication-1.4.0/sockets_communication/service.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.3.0/sockets_communication/sockets.py` & `sockets-communication-1.4.0/sockets_communication/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,303 +1,35 @@
 # sockets.py
 
 import warnings
-from abc import ABCMeta
 import datetime as dt
 import socket
 import threading
 from typing import (
     Optional, Union, Tuple, Dict, Any
 )
 
-from requests.models import PreparedRequest
 
 from represent import represent
 
-from sockets_communication.process import decode
 from sockets_communication.service import ServiceInterface
+from sockets_communication.communication import Communication
 
 __all__ = [
-    "Components",
-    "Communication",
-    "SocketClient",
     "SocketServer",
-    "ClientsCollection",
-    "bluetooth_socket_request",
-    "bluetooth_socket"
+    "ClientsCollection"
+
 ]
 
 Socket = socket.socket
 Host = str
 Port = Union[str, int]
 Address = Tuple[Host, Port]
 Number = Union[int, float]
 
-class Components(metaclass=ABCMeta):
-    """Defines the basic parameters for the communication."""
-
-    HEADER = 64
-
-    ENCODING = 'utf-8'
-
-    @property
-    def encoding(self) -> str:
-        """
-        Returns the encoding string.
-
-        :return: The encoding string.
-        """
-
-        return self.ENCODING
-    # end encoding
-
-    @property
-    def header(self) -> int:
-        """
-        Returns the header number.
-
-        :return: The header-number.
-        """
-
-        return self.HEADER
-    # end header
-
-    @encoding.setter
-    def encoding(self, value: str) -> None:
-        """
-        Sets the encoding value.
-
-        :param value: The encoding value
-        """
-
-        try:
-            if not isinstance(value, str):
-                raise LookupError
-            # end if
-
-            "".encode(value)
-
-        except LookupError:
-            raise LookupError(f"Unknown encoding: {value}")
-        # end try
-
-        Components.ENCODING = value
-    # end encoding
-
-    @header.setter
-    def header(self, value: int) -> None:
-        """
-        Sets the header value.
-
-        :param value: The header value
-        """
-
-        if not (isinstance(value, str) and value % 2 == 0):
-            raise ValueError(f"Invalid header: {value}")
-        # end if
-
-        Components.HEADER = value
-    # end header
-# end Components
-
-class Communication(Components, metaclass=ABCMeta):
-    """Defines the base methods for the server and clients communication."""
-
-    SIZE = 1024
-
-    def send(self, message: bytes, connection: Socket) -> None:
-        """
-        Sends a message to the client or server by its connection.
-
-        :param message: The message to send to the client.
-        :param connection: The sockets' connection object.
-        """
-
-        message_len = len(message)
-
-        connection.send(
-            (
-                str(message_len) + " " *
-                (self.HEADER - len(str(message_len)))
-            ).encode(self.ENCODING)
-        )
-
-        iterations = (
-            message_len // self.SIZE + 1 + message_len % self.SIZE
-        )
-
-        for i in range(0, iterations, self.SIZE):
-            if len(message[i:]) >= self.SIZE:
-                connection.send(message[i:self.SIZE])
-
-            else:
-                connection.send(message[i:])
-            # end if
-        # end for
-    # end send
-
-    def receive(self, connection: Socket) -> bytes:
-        """
-        Receive a message from the client or server by its connection.
-
-        :param connection: The sockets' connection object.
-
-        :return: The received message from the server.
-        """
-
-        message_len = (
-            int(
-                connection.recv(self.HEADER).
-                decode(self.ENCODING).
-                replace(" ", "")
-            )
-        )
-
-        message = b''
-
-        iterations = (
-            message_len // self.SIZE + 1 + message_len % self.SIZE
-        )
-
-        for i in range(0, iterations, self.SIZE):
-            if (i < iterations - 1) or (message_len % self.SIZE == 0):
-                message += connection.recv(self.SIZE)
-
-            else:
-                message += connection.recv(message_len % self.SIZE)
-            # end if
-        # end for
-
-        return message
-    # end receive
-# end Communication
-
-@represent
-class SocketClient(Communication):
-    """Creates the client to communicate with the server."""
-
-    def __init__(
-            self,
-            connection: Optional[Socket] = None, *,
-            host: Optional[Host] = None,
-            port: Optional[Port] = None
-    ) -> None:
-        """
-        Defines the server address and creates the client object.
-
-        :param connection: The connection socket.
-        :param host: The ip address of the server.
-        :param port: The port for the server connection.
-        """
-
-        self.connection: Optional[socket.socket] = connection
-
-        self.host: Optional[str] = host
-        self.port: Optional[int] = port
-    # end __init__
-
-    def validate_connection(self) -> None:
-        """Validates the connection object."""
-
-        if not isinstance(self.connection, socket.socket):
-            raise ValueError(
-                f"Connection object must be {socket.socket}, "
-                f"not: {self.connection}."
-            )
-        # end if
-    # end validate_connection
-
-    def send(self, message: bytes, connection: Optional[Socket] = None) -> None:
-        """
-        Sends a message to the client or server by its connection.
-
-        :param message: The message to send to the client.
-        :param connection: The sockets' connection object.
-        """
-
-        if connection is None:
-            self.validate_connection()
-
-            connection = self.connection
-        # end if
-
-        super().send(message=message, connection=connection)
-    # end send
-
-    def receive(self, connection: Optional[Socket] = None) -> bytes:
-        """
-        Receive a message from the client or server by its connection.
-
-        :param connection: The sockets' connection object.
-
-        :return: The received message from the server.
-        """
-
-        if connection is None:
-            self.validate_connection()
-
-            connection = self.connection
-        # end if
-
-        return super().receive(connection=connection)
-    # end receive
-
-    def connect(
-            self,
-            connection: Optional[Socket] = None, *,
-            host: Optional[Host] = None,
-            port: Optional[Port] = None
-    ) -> None:
-        """
-        Creates the sockets' connection for the client object with the server.
-
-        :param connection: The connection socket.
-        :param host: The ip address of the server.
-        :param port: The port for the server connection.
-        """
-
-        if connection is not None:
-            self.connection = connection
-        # end if
-
-        if host is not None:
-            self.host = host
-        # end if
-
-        if port is not None:
-            self.port = port
-        # end if
-
-        self.validate_connection()
-
-        self.connection.connect((self.host, self.port))
-    # end connect
-
-    def send_message_to_server(self, message: bytes) -> None:
-        """
-        Sends a message to the server through the sockets' connection.
-
-        :param message: The message to send to the server.
-        """
-
-        return self.send(connection=self.connection, message=message)
-    # end send_message_to_server
-
-    # defines a method to receive a message form hte server
-    def receive_message_from_server(self) -> bytes:
-        """
-        Gets the received message from the server.
-
-        :return: The received response from the server.
-        """
-
-        return self.receive(connection=self.connection)
-    # end receive_message_from_server
-# end SocketClient
-
 @represent
 class ClientsCollection:
     """A data class to contain clients within the server data."""
 
     def __init__(self, clients: Optional[dict] = None) -> None:
         """
         Defines the base data class to contain the clients.
@@ -388,23 +120,23 @@
         self._connected = False
         self._serving = False
 
         self.clients = ClientsCollection()
     # end __init__
 
     @property
-    def built(self) -> bool:
+    def connected(self) -> bool:
         """
         Checks if the service was built.
 
         :return: The value for the service being built.
         """
 
         return self._connected
-    # end built
+    # end connected
 
     @property
     def created(self) -> bool:
         """
         Checks if the service was created.
 
         :return: The value for the service being created.
@@ -457,16 +189,14 @@
             self.host = host
         # end if
 
         if port is not None:
             self.port = port
         # end if
 
-        self.connection = connection
-
         self.validate_connection()
 
         self.connection.bind((host, port))
 
         self._connected = True
     # end connect
 
@@ -519,15 +249,15 @@
 
         :param connection: The connection socket.
         :param host: The host of the server.
         :param port: The port of the server.
         :param daemon: The value to set the process as daemon.
         """
 
-        if not self.built:
+        if not self.connected:
             self.connect(connection=connection, host=host, port=port)
         # end if
 
         self._listening_process = threading.Thread(
             target=self.listen, daemon=daemon
         )
     # end create
@@ -602,16 +332,16 @@
         if listen:
             self.start_serving(
                 connection=connection, host=host,
                 port=port, daemon=daemon
             )
         # end if
 
-        super().run(
-            update=update, refresh=refresh,
+        ServiceInterface.run(
+            self, update=update, refresh=refresh,
             block=block, wait=wait, timeout=timeout
         )
     # end run
 
     def rerun(
             self,
             connection: Optional[Socket] = None,
@@ -754,59 +484,8 @@
         Removes the client object from the data class.
 
         :param address: The tuple of the ip address and the port of the connection
         """
 
         self.clients.remove_client(address)
     # end remove_client
-# end SocketServer
-
-def bluetooth_socket() -> socket:
-    """
-    Sends a request through the bluetooth sockets.
-
-    :return: The client object..
-    """
-
-    return socket.socket(
-        socket.AF_BLUETOOTH, socket.SOCK_STREAM,
-        socket.BTPROTO_RFCOMM
-    )
-# end bluetooth_socket
-
-def bluetooth_socket_request(
-        host: Host,
-        port: Port,
-        endpoint: Optional[str] = None,
-        parameters: Optional[Dict[str, Any]] = None
-) -> Any:
-    """
-    Sends a request through the bluetooth sockets.
-
-    :param host: The request host.
-    :param endpoint: The path to the endpoint.
-    :param port: The sending port.
-    :param parameters: The request parameters.
-
-    :return: The returned value.
-    """
-
-    client = SocketClient()
-
-    connection = bluetooth_socket()
-
-    client.connect(connection=connection, host=host, port=port)
-
-    req = PreparedRequest()
-    # noinspection HttpUrlsUsage
-    req.prepare_url(
-        f"http://{host}:{port}/{endpoint or ''}",
-        parameters or {}
-    )
-
-    client.send(message=req.url.encode())
-    content = client.receive()
-
-    client.connection.close()
-
-    return decode(content.decode())
-# end bluetooth_socket_request
+# end SocketServer
```

### Comparing `sockets-communication-1.3.0/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.4.0/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.3.0
+Version: 1.4.0
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

