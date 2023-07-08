# Comparing `tmp/qmp-1.0.0.tar.gz` & `tmp/qmp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmp-1.0.0.tar", last modified: Sun Jul  2 20:45:45 2023, max compression
+gzip compressed data, was "qmp-1.1.0.tar", last modified: Sat Jul  8 14:10:11 2023, max compression
```

## Comparing `qmp-1.0.0.tar` & `qmp-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-02 20:45:45.177517 qmp-1.0.0/
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)    18092 2023-07-02 20:10:38.000000 qmp-1.0.0/LICENSE
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1954 2023-07-02 20:45:45.177517 qmp-1.0.0/PKG-INFO
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      984 2023-07-02 20:10:18.000000 qmp-1.0.0/README.md
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1038 2023-07-02 20:44:14.000000 qmp-1.0.0/pyproject.toml
-drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-02 20:45:45.177517 qmp-1.0.0/qmp.egg-info/
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1954 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/PKG-INFO
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      147 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/SOURCES.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        1 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/dependency_links.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        4 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/top_level.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     8244 2023-07-02 12:55:24.000000 qmp-1.0.0/qmp.py
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)       38 2023-07-02 20:45:45.177517 qmp-1.0.0/setup.cfg
+drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-08 14:10:11.022662 qmp-1.1.0/
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)    18092 2023-07-02 20:10:38.000000 qmp-1.1.0/LICENSE
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1950 2023-07-08 14:10:11.022662 qmp-1.1.0/PKG-INFO
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      980 2023-07-08 14:04:18.000000 qmp-1.1.0/README.md
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1040 2023-07-08 14:07:01.000000 qmp-1.1.0/pyproject.toml
+drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-08 14:10:11.022662 qmp-1.1.0/qmp.egg-info/
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1950 2023-07-08 14:10:11.000000 qmp-1.1.0/qmp.egg-info/PKG-INFO
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      147 2023-07-08 14:10:11.000000 qmp-1.1.0/qmp.egg-info/SOURCES.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        1 2023-07-08 14:10:11.000000 qmp-1.1.0/qmp.egg-info/dependency_links.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        4 2023-07-08 14:10:11.000000 qmp-1.1.0/qmp.egg-info/top_level.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     9789 2023-07-08 14:04:18.000000 qmp-1.1.0/qmp.py
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)       38 2023-07-08 14:10:11.022662 qmp-1.1.0/setup.cfg
```

### Comparing `qmp-1.0.0/LICENSE` & `qmp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qmp-1.0.0/PKG-INFO` & `qmp-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmp
-Version: 1.0.0
+Version: 1.1.0
 Summary: QEMU Machine Protocol client
 Author-email: QEMU Project <qemu-devel@nongnu.org>
 Maintainer-email: Alexey Bogdanenko <alexey@bogdanenko.com>
 Project-URL: Homepage, https://gitlab.com/abogdanenko/qmp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -38,13 +38,13 @@
 For the full list of commands supported by QMP see
 [QEMU QMP Reference Manual — QEMU documentation](https://qemu-project.gitlab.io/qemu/interop/qemu-qmp-ref.html).
 
 About the project
 -----------------
 
 This PyPI project packages a single file `qmp.py` from the QEMU source tree:
-<https://github.com/qemu/qemu/blob/v4.0.0-rc0/python/qemu/qmp.py>.
+<https://github.com/qemu/qemu/blob/v5.0.0/python/qemu/qmp.py>.
 
 This PyPI project was created in 2019.
 
 A different project offering a solution to the same problem (and more) has been
 created in 2021: <https://pypi.org/project/qemu.qmp/>. You may want to use it.
```

### Comparing `qmp-1.0.0/README.md` & `qmp-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 For the full list of commands supported by QMP see
 [QEMU QMP Reference Manual — QEMU documentation](https://qemu-project.gitlab.io/qemu/interop/qemu-qmp-ref.html).
 
 About the project
 -----------------
 
 This PyPI project packages a single file `qmp.py` from the QEMU source tree:
-<https://github.com/qemu/qemu/blob/v4.0.0-rc0/python/qemu/qmp.py>.
+<https://github.com/qemu/qemu/blob/v5.0.0/python/qemu/qmp.py>.
 
 This PyPI project was created in 2019.
 
 A different project offering a solution to the same problem (and more) has been
 created in 2021: <https://pypi.org/project/qemu.qmp/>. You may want to use it.
```

### Comparing `qmp-1.0.0/pyproject.toml` & `qmp-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 description = "QEMU Machine Protocol client"
 name = "qmp"
 readme = "README.md"
 requires-python = ">=3.6"
-version="1.0.0"
+version = "1.1.0"
 
 [project.urls]
 Homepage = "https://gitlab.com/abogdanenko/qmp"
 
 [[project.authors]]
 email = "qemu-devel@nongnu.org"
 name = "QEMU Project"
```

### Comparing `qmp-1.0.0/qmp.egg-info/PKG-INFO` & `qmp-1.1.0/qmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmp
-Version: 1.0.0
+Version: 1.1.0
 Summary: QEMU Machine Protocol client
 Author-email: QEMU Project <qemu-devel@nongnu.org>
 Maintainer-email: Alexey Bogdanenko <alexey@bogdanenko.com>
 Project-URL: Homepage, https://gitlab.com/abogdanenko/qmp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -38,13 +38,13 @@
 For the full list of commands supported by QMP see
 [QEMU QMP Reference Manual — QEMU documentation](https://qemu-project.gitlab.io/qemu/interop/qemu-qmp-ref.html).
 
 About the project
 -----------------
 
 This PyPI project packages a single file `qmp.py` from the QEMU source tree:
-<https://github.com/qemu/qemu/blob/v4.0.0-rc0/python/qemu/qmp.py>.
+<https://github.com/qemu/qemu/blob/v5.0.0/python/qemu/qmp.py>.
 
 This PyPI project was created in 2019.
 
 A different project offering a solution to the same problem (and more) has been
 created in 2021: <https://pypi.org/project/qemu.qmp/>. You may want to use it.
```

### Comparing `qmp-1.0.0/qmp.py` & `qmp-1.1.0/qmp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# QEMU Monitor Protocol Python class
-#
+""" QEMU Monitor Protocol Python class """
 # Copyright (C) 2009, 2010 Red Hat Inc.
 #
 # Authors:
 #  Luiz Capitulino <lcapitulino@redhat.com>
 #
 # This work is licensed under the terms of the GNU GPL, version 2.  See
 # the COPYING file in the top-level directory.
@@ -11,54 +10,65 @@
 import json
 import errno
 import socket
 import logging
 
 
 class QMPError(Exception):
-    pass
+    """
+    QMP base exception
+    """
 
 
 class QMPConnectError(QMPError):
-    pass
+    """
+    QMP connection exception
+    """
 
 
 class QMPCapabilitiesError(QMPError):
-    pass
+    """
+    QMP negotiate capabilities exception
+    """
 
 
 class QMPTimeoutError(QMPError):
-    pass
+    """
+    QMP timeout exception
+    """
 
 
-class QEMUMonitorProtocol(object):
+class QEMUMonitorProtocol:
+    """
+    Provide an API to connect to QEMU via QEMU Monitor Protocol (QMP) and then
+    allow to handle commands and events.
+    """
 
     #: Logger object for debugging messages
     logger = logging.getLogger('QMP')
-    #: Socket's error class
-    error = socket.error
-    #: Socket's timeout
-    timeout = socket.timeout
 
-    def __init__(self, address, server=False):
+    def __init__(self, address, server=False, nickname=None):
         """
         Create a QEMUMonitorProtocol class.
 
         @param address: QEMU address, can be either a unix socket path (string)
                         or a tuple in the form ( address, port ) for a TCP
                         connection
         @param server: server mode listens on the socket (bool)
-        @raise socket.error on socket connection errors
+        @raise OSError on socket connection errors
         @note No connection is established, this is done by the connect() or
               accept() methods
         """
         self.__events = []
         self.__address = address
         self.__sock = self.__get_sock()
         self.__sockfile = None
+        self._nickname = nickname
+        if self._nickname:
+            self.logger = logging.getLogger('QMP').getChild(self._nickname)
         if server:
             self.__sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             self.__sock.bind(self.__address)
             self.__sock.listen(1)
 
     def __get_sock(self):
         if isinstance(self.__address, tuple):
@@ -69,23 +79,23 @@
 
     def __negotiate_capabilities(self):
         greeting = self.__json_read()
         if greeting is None or "QMP" not in greeting:
             raise QMPConnectError
         # Greeting seems ok, negotiate capabilities
         resp = self.cmd('qmp_capabilities')
-        if "return" in resp:
+        if resp and "return" in resp:
             return greeting
         raise QMPCapabilitiesError
 
     def __json_read(self, only_event=False):
         while True:
             data = self.__sockfile.readline()
             if not data:
-                return
+                return None
             resp = json.loads(data)
             if 'event' in resp:
                 self.logger.debug("<<< %s", resp)
                 self.__events.append(resp)
                 if not only_event:
                     continue
             return resp
@@ -103,16 +113,16 @@
                                 retrieved or if some other error occurred.
         """
 
         # Check for new events regardless and pull them into the cache:
         self.__sock.setblocking(0)
         try:
             self.__json_read()
-        except socket.error as err:
-            if err[0] == errno.EAGAIN:
+        except OSError as err:
+            if err.errno == errno.EAGAIN:
                 # No data available
                 pass
         self.__sock.setblocking(1)
 
         # Wait for new events, if needed.
         # if wait is 0.0, this means "no wait" and is also implicitly false.
         if not self.__events and wait:
@@ -124,38 +134,55 @@
                 raise QMPTimeoutError("Timeout waiting for event")
             except:
                 raise QMPConnectError("Error while reading from socket")
             if ret is None:
                 raise QMPConnectError("Error while reading from socket")
             self.__sock.settimeout(None)
 
+    def __enter__(self):
+        # Implement context manager enter function.
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        # Implement context manager exit function.
+        self.close()
+        return False
+
     def connect(self, negotiate=True):
         """
         Connect to the QMP Monitor and perform capabilities negotiation.
 
-        @return QMP greeting dict
-        @raise socket.error on socket connection errors
+        @return QMP greeting dict, or None if negotiate is false
+        @raise OSError on socket connection errors
         @raise QMPConnectError if the greeting is not received
         @raise QMPCapabilitiesError if fails to negotiate capabilities
         """
         self.__sock.connect(self.__address)
         self.__sockfile = self.__sock.makefile()
         if negotiate:
             return self.__negotiate_capabilities()
+        return None
 
-    def accept(self):
+    def accept(self, timeout=15.0):
         """
         Await connection from QMP Monitor and perform capabilities negotiation.
 
+        @param timeout: timeout in seconds (nonnegative float number, or
+                        None). The value passed will set the behavior of the
+                        underneath QMP socket as described in [1]. Default value
+                        is set to 15.0.
         @return QMP greeting dict
-        @raise socket.error on socket connection errors
+        @raise OSError on socket connection errors
         @raise QMPConnectError if the greeting is not received
         @raise QMPCapabilitiesError if fails to negotiate capabilities
+
+        [1]
+        https://docs.python.org/3/library/socket.html#socket.socket.settimeout
         """
-        self.__sock.settimeout(15)
+        self.__sock.settimeout(timeout)
         self.__sock, _ = self.__sock.accept()
         self.__sockfile = self.__sock.makefile()
         return self.__negotiate_capabilities()
 
     def cmd_obj(self, qmp_cmd):
         """
         Send a QMP command to the QMP Monitor.
@@ -163,18 +190,18 @@
         @param qmp_cmd: QMP command to be sent as a Python dict
         @return QMP response as a Python dict or None if the connection has
                 been closed
         """
         self.logger.debug(">>> %s", qmp_cmd)
         try:
             self.__sock.sendall(json.dumps(qmp_cmd).encode('utf-8'))
-        except socket.error as err:
-            if err[0] == errno.EPIPE:
-                return
-            raise socket.error(err)
+        except OSError as err:
+            if err.errno == errno.EPIPE:
+                return None
+            raise err
         resp = self.__json_read()
         self.logger.debug("<<< %s", resp)
         return resp
 
     def cmd(self, name, args=None, cmd_id=None):
         """
         Build a QMP command and send it to the QMP Monitor.
@@ -239,18 +266,39 @@
     def clear_events(self):
         """
         Clear current list of pending events.
         """
         self.__events = []
 
     def close(self):
-        self.__sock.close()
-        self.__sockfile.close()
+        """
+        Close the socket and socket file.
+        """
+        if self.__sock:
+            self.__sock.close()
+        if self.__sockfile:
+            self.__sockfile.close()
 
     def settimeout(self, timeout):
+        """
+        Set the socket timeout.
+
+        @param timeout (float): timeout in seconds, or None.
+        @note This is a wrap around socket.settimeout
+        """
         self.__sock.settimeout(timeout)
 
     def get_sock_fd(self):
+        """
+        Get the socket file descriptor.
+
+        @return The file descriptor number.
+        """
         return self.__sock.fileno()
 
     def is_scm_available(self):
+        """
+        Check if the socket allows for SCM_RIGHTS.
+
+        @return True if SCM_RIGHTS is available, otherwise False.
+        """
         return self.__sock.family == socket.AF_UNIX
```

