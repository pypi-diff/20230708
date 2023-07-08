# Comparing `tmp/ku_proxy-0.2.0-py3-none-any.whl.zip` & `tmp/ku_proxy-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10546 bytes, number of entries: 10
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-01 19:41 ku/__init__.py
--rw-r--r--  2.0 unx    11923 b- defN 23-Jul-01 19:41 ku/ku.py
--rw-r--r--  2.0 unx     9453 b- defN 23-Jul-01 19:41 ku/kun.py
--rw-r--r--  2.0 unx      943 b- defN 23-Jul-01 19:41 ku/util.py
--rw-rw-rw-  2.0 unx     1064 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3462 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        3 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      753 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/RECORD
-10 files, 27779 bytes uncompressed, 9272 bytes compressed:  66.6%
+Zip file size: 10563 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-08 13:23 ku/__init__.py
+-rw-r--r--  2.0 unx    12013 b- defN 23-Jul-08 13:23 ku/ku.py
+-rw-r--r--  2.0 unx     9453 b- defN 23-Jul-08 13:23 ku/kun.py
+-rw-r--r--  2.0 unx      943 b- defN 23-Jul-08 13:23 ku/util.py
+-rw-rw-rw-  2.0 unx     1064 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3462 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      753 b- defN 23-Jul-08 13:23 ku_proxy-0.2.1.dist-info/RECORD
+10 files, 27869 bytes uncompressed, 9289 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: ku/kun.py
 Comment: 
 
 Filename: ku/util.py
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/LICENSE
+Filename: ku_proxy-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/METADATA
+Filename: ku_proxy-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/WHEEL
+Filename: ku_proxy-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/entry_points.txt
+Filename: ku_proxy-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/top_level.txt
+Filename: ku_proxy-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ku_proxy-0.2.0.dist-info/RECORD
+Filename: ku_proxy-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .ku import * # NOQA
-version = '0.2.0'
+version = '0.2.1'
```

## ku/ku.py

```diff
@@ -29,15 +29,15 @@
 class state(Enum):
     DISCONNECTED = 0
     CLIENT_W_U = 1 # client waiting for upstream
     CONNECTED = 2
 
 class tcpsession(object):
 
-    state: state = state.DISCONNECTED
+    _state: state = state.DISCONNECTED
 
     client: socket
     server: socket
 
     client_total: int
     server_total: int
 
@@ -55,22 +55,22 @@
     def connection_lost(self, side: Union[socket, None], err: Union[Exception, None]) -> None:
         pass
     
     def shutdown(self) -> None:
         pass
 
     def _change_state(self, new_state: state) -> None:
-        self.proxy.logger.debug(f"#{id(self)} {self.state} -> {new_state}")
-        self.state = new_state
+        self.proxy._logger.debug(f"#{id(self)} {self._state} -> {new_state}")
+        self._state = new_state
 
     def terminate(self) -> None:
         self.proxy.terminate(self)
 
     def __repr__(self):        
-        if self.state != state.CONNECTED:
+        if self._state != state.CONNECTED:
             return super().__repr__()
         return f"<#{id(self)}[{round((time() - self.estab_time), 2)}] {self.client.getpeername()}->{self.client.getsockname()}::{self.server.getsockname()}->{self.server.getpeername()}>"
 
 class ku(object):
 
     fd: List[socket]  # tracked file descriptors
     wai: List[socket] # wa
@@ -105,57 +105,58 @@
 
                 elif pattern is IPv4:
                     return AF_INET
 
                 elif pattern is TLD:
                     return -1
 
-    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, session_args: tuple = (), maxcon: int = -1, upstream_6: bool = False):
+    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, session_args: tuple = (), maxcon: int = -1, upstream_6: bool = False, loglevel = logging.ERROR):
 
         self.fd: list = []
         self.wai: list = []
         self.ss: list = []
 
-        self.logger = logging.getLogger("ku.devel")
+        self._logger = logging.getLogger("ku.devel")
+        self._logger.setLevel(loglevel)
 
         proto = self._resolve_proto(upstream[0])
         self.upstream = (AF_INET6 if upstream_6 else AF_INET if proto == -1 else proto, upstream[0], upstream[1])
-        self.logger.debug(f"Upstreaming to - {'v6' if self.upstream[0] is AF_INET6 else 'v4'} {upstream[0]}:{upstream[1]}")
+        self._logger.debug(f"Upstreaming to - {'v6' if self.upstream[0] is AF_INET6 else 'v4'} {upstream[0]}:{upstream[1]}")
 
         self.session = session
         self.maxcon = maxcon
         self.session_args = session_args
 
         self.sockets = ()
         for i in range(0, len(listen), 2):
             proto, host, port = self._resolve_proto(listen[i]), *listen[i:i+2]
 
             sock = socket(proto, 1)
-            self.logger.debug(f"Listening at - {'v6' if proto is AF_INET6 else 'v4'} {host}:{port}")
+            self._logger.debug(f"Listening at - {'v6' if proto is AF_INET6 else 'v4'} {host}:{port}")
             sock.bind((host, port))
             if system() == "Windows":
                 sock.setsockopt(SOL_SOCKET, SO_CONDITIONAL_ACCEPT, 1)
             sock.listen()
             self.fd.append(sock)
             self.sockets = (*self.sockets, sock)
 
-        self.thread = Thread(target=self.poll, name=f"Ku poller #{currentThread().ident}", daemon=True)
+        self.thread = Thread(target=self.poll, name=f"Ku poller #{id(self)}", daemon=True)
         self.thread.start()
 
     def shutdown(self):
         # can't be called from handler!)
         if currentThread() is self.thread:
             raise RuntimeError(f"People stuck at {currentThread()}")
 
         self.alive = False
         while self.thread.is_alive():
             pass
 
         for s in self.ss:
-            if s.state == state.CONNECTED:
+            if s._state == state.CONNECTED:
                 s.shutdown()
 
             s.client.shutdown(1)
             s.server.shutdown(1)
             s._change_state(state.DISCONNECTED)
 
         del self.fd
@@ -173,15 +174,15 @@
         self.fd.remove(session.client)
         self.fd.remove(session.server)
         # Shutdown sockets
         session.client.shutdown(2)
         session.server.shutdown(2)
         # Delete session
         self.ss.remove(session)
-        self.logger.debug(f"#{id(session)} terminated [ITR]")
+        self._logger.debug(f"#{id(session)} terminated [ITR]")
 
     def _handle_socket_disconnect(self, fd, err):            
         s = self.lookup_session(fd)        
         if not s:
             # ITR
             return
 
@@ -195,85 +196,85 @@
 
         # Destroy session instance
         self.ss.remove(s)
 
         s._change_state(state.DISCONNECTED)
         s.connection_lost(fd, err)
 
-        self.logger.debug(f"#{id(s)} terminated")
+        self._logger.debug(f"#{id(s)} terminated")
 
     def lookup_session(self, fd: socket):
         for s in self.ss:
             if s.client == fd or s.server == fd:
                 return s
 
     def send(self, fd: socket, data: bytes) -> None:
         try:
             fd.sendall(data)
         except Exception as e:
-            self.logger.debug(f"Failed to send data to the fd, initiating session termination...")
-            self._handle_socket_disconnect(fd)
+            self._logger.debug(f"Failed to send data to the fd, initiating session termination...")
+            self._handle_socket_disconnect(fd, e)
 
     def _accept(self, fd: socket):
         # check limitations
         if len(self.ss) == self.maxcon:
             try:
                 c, addr = fd.accept()
                 c.close()
             except:
                 pass
             return
         
         # create new instance of tcpsession class
         s = object.__new__(self.session)
         s.proxy = self
-        self.logger.debug(f"#{id(s)} Begin new connection request processing")
+        self._logger.debug(f"#{id(s)} Begin new connection request processing")
 
         # new client
         try:
             c, addr = fd.accept()
         except Exception as e:
-            self.logger.warning(f"Failed to accept new client: {e}")
-            self.logger.debug(f"#{id(s)} terminated")
+            self._logger.warning(f"Failed to accept new client: {e}")
+            self._logger.debug(f"#{id(s)} terminated")
             return
             
-        self.logger.debug(f"#{id(s)} client: {addr}")
+        self._logger.debug(f"#{id(s)} client: {addr}")
         s.client = c
 
         s._change_state(state.CLIENT_W_U)
 
         # new upstream
         u = socket(self.upstream[0], 1)
         u.settimeout(0)
         s.server = u
 
         try:                        
             u.connect(self.upstream[1:])
         except BlockingIOError:
             pass
 
-        self.logger.debug(f"#{id(s)} upstreaming initiated, waiting...")        
+        self._logger.debug(f"#{id(s)} upstreaming initiated, waiting...")        
 
         self.ss.append(s)                    
         self.wai.append(u)
 
     def poll(self):
-        self.logger.debug("Begin polling")
+        self._logger.debug("Begin polling")
 
         while self.alive:
             # select()
             fds, puo, puf = select(self.fd, self.wai, self.wai, 0)
             if not (fds or puo or puf) or self.pause:
                 if self.PSM:
                     sleep(self.PSM)
                 continue
 
             for fd in puo:                
                 s = self.lookup_session(fd)
-                self.logger.debug(f"#{id(s)} upstreamed, initiating trasmisson")
+                self._logger.debug(f"#{id(s)} upstreamed, initiating trasmisson")
 
                 # Remove upstream from waiting list
                 self.wai.remove(fd)
 
                 # Add client & upstream to watging list
                 self.fd.append(fd)
                 self.fd.append(s.client)
@@ -284,29 +285,29 @@
                 s.estab_time = time()
 
                 # Init session
                 s.__init__(s.client, fd, self, *self.session_args)
 
             for fd in puf:
                 s = self.lookup_session(fd)
-                self.logger.debug(f"#{id(s)} Failed to upstream")
+                self._logger.debug(f"#{id(s)} Failed to upstream")
 
                 # Remove upstream from waiting list
                 self.wai.remove(fd)
 
                 # Close associated client & upstream descriptors
                 s.client.close()
                 fd.close()
 
                 # Change session state
                 s._change_state(state.DISCONNECTED)
 
                 self.ss.remove(s)
 
-                self.logger.debug(f"#{id(s)} terminated")
+                self._logger.debug(f"#{id(s)} terminated")
 
             for sock in self.sockets:
                 if sock in fds:
                     self._accept(sock)
                     fds.remove(sock)
 
             for fd in fds:
@@ -315,65 +316,65 @@
 
                 s = self.lookup_session(fd)
                 bname = 'client' if fd is s.client else 'upstream'
 
                 try:
                     data = fd.recv(65535)
                 except Exception as e:
-                    self.logger.debug(f"#{id(s)}, {bname} lost connection: {e}")
+                    self._logger.debug(f"#{id(s)}, {bname} lost connection: {e}")
                     self._handle_socket_disconnect(fd, e)
                     continue
 
                 if len(data) < 1:
-                    self.logger.debug(f"#{id(s)}, {bname} disconnected")
+                    self._logger.debug(f"#{id(s)}, {bname} disconnected")
                     self._handle_socket_disconnect(fd, None)
                     continue
 
                 if fd is s.client:
-                    self.logger.debug(f"#{id(s)} client -> server {round(len(data) / 1000, 2)}Kb")
+                    #self._logger.debug(f"#{id(s)} client -> server {round(len(data) / 1000, 2)}Kb")
                     hr = None
 
                     try:
                         hr = s.serverbound(data)
                     except Exception as e:
-                        self.logger.error(f"Exception in {s.serverbound}: {e}")
+                        self._logger.error(f"Exception in {s.serverbound}: {e}")
 
                     if isinstance(hr, bytes):
                         data = hr
 
                     elif hr is Reject:
                             continue
 
                     elif hr is not Pass and hr is not None:
-                        self.logger.error(F"#{id(s)} ServerBound handler returned unidentified type! {hr.__class__}")
+                        self._logger.error(F"#{id(s)} ServerBound handler returned unidentified type! {hr.__class__}")
 
                     try:
                         s.server.sendall(data)
                     except Exception as e:
-                        self.logger.debug(f"#{id(s)} Upstream dropped connection in the middle of data transmission process")
+                        self._logger.debug(f"#{id(s)} Upstream dropped connection in the middle of data transmission process")
                         self._handle_socket_disconnect(s.server, e)
 
                 else:
-                    self.logger.debug(f"#{id(s)} server -> client {round(len(data) / 1000, 2)}Kb")
+                    #self._logger.debug(f"#{id(s)} server -> client {round(len(data) / 1000, 2)}Kb")
                     hr = None
 
                     try:
                         hr = s.clientbound(data)
                     except Exception as e:
-                        self.logger.error(f"Exception in {s.clientbound}: {e}")                        
+                        self._logger.error(f"Exception in {s.clientbound}: {e}")                        
 
                     if isinstance(hr, bytes):
                         data = hr
 
                     elif hr is Reject:
                             continue
 
                     elif hr is not Pass and hr is not None:
-                        self.logger.error(F"#{id(s)} ClientBound handler returned unidentified type! {hr.__class__}")
+                        self._logger.error(F"#{id(s)} ClientBound handler returned unidentified type! {hr.__class__}")
 
                     try:
                         s.client.sendall(data)
                     except Exception as e:
-                        self.logger.debug(f"#{id(s)} Client dropped connection in the middle of data transmission process")
+                        self._logger.debug(f"#{id(s)} Client dropped connection in the middle of data transmission process")
                         self._handle_socket_disconnect(s.client, e)
 
-        self.logger.debug(f"Stop polling")
+        self._logger.debug(f"Stop polling")
```

## Comparing `ku_proxy-0.2.0.dist-info/LICENSE` & `ku_proxy-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_proxy-0.2.0.dist-info/METADATA` & `ku_proxy-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku-proxy
-Version: 0.2.0
+Version: 0.2.1
 Summary: ku is fast, async, modern, little tcp man-in-the-middle proxy library, written in pure Python 3
 Home-page: https://gitlab.com/seeklay/ku
 Author: seeklay
 Author-email: rudeboy@seeklay.icu
 License: MIT
 Download-URL: https://gitlab.com/seeklay/ku
 Platform: OS Independent
```

## Comparing `ku_proxy-0.2.0.dist-info/RECORD` & `ku_proxy-0.2.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ku/__init__.py,sha256=KggOrEo8YVeVqw8fY_lTdtGNG5cSYs36b-5W0-f_2bk,42
-ku/ku.py,sha256=mndg1dneX3_oYmlqEC15167kEiBE9nf-3UYk9bRS7KY,11923
+ku/__init__.py,sha256=7BWmX8baxVvui8ac10RenlhFlTonxrvn4LrrkumLw8c,42
+ku/ku.py,sha256=eoxSoxgw1tVoG4cjIsMiowKyG-W7ZbATyTNB7t6LF2o,12013
 ku/kun.py,sha256=5bkXVoqodobCWv-EceAnU3URISa9OFurS1E93nAyGqQ,9453
 ku/util.py,sha256=6DFb7NfA9-4vEmxY5LCp8bKOu5vn1WuyikiWBsvkSzc,943
-ku_proxy-0.2.0.dist-info/LICENSE,sha256=Lnu_C3NpvP-wrunHvh58jopFspHBRekQJPd5zjD7siU,1064
-ku_proxy-0.2.0.dist-info/METADATA,sha256=JRwXbcRa9oQvOLersG852Gyeo1hTQAkv6q-xHRAkyz4,3462
-ku_proxy-0.2.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-ku_proxy-0.2.0.dist-info/entry_points.txt,sha256=shidVH2jY_HIiEn6ULD-AqBzB-Bpv6SKIkGc4qTVI34,44
-ku_proxy-0.2.0.dist-info/top_level.txt,sha256=QTrN_uqQ-epFQrRU-dU5X8HF4Z0_dPXPQT9RBKwFJV0,3
-ku_proxy-0.2.0.dist-info/RECORD,,
+ku_proxy-0.2.1.dist-info/LICENSE,sha256=Lnu_C3NpvP-wrunHvh58jopFspHBRekQJPd5zjD7siU,1064
+ku_proxy-0.2.1.dist-info/METADATA,sha256=T900DF0K9G_D3Xpn2kBGd6bGkm1KXTdit-i5zdV0REw,3462
+ku_proxy-0.2.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+ku_proxy-0.2.1.dist-info/entry_points.txt,sha256=shidVH2jY_HIiEn6ULD-AqBzB-Bpv6SKIkGc4qTVI34,44
+ku_proxy-0.2.1.dist-info/top_level.txt,sha256=QTrN_uqQ-epFQrRU-dU5X8HF4Z0_dPXPQT9RBKwFJV0,3
+ku_proxy-0.2.1.dist-info/RECORD,,
```

