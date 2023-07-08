# Comparing `tmp/MCRP-0.1.9-py3-none-any.whl.zip` & `tmp/MCRP-0.2.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 24513 bytes, number of entries: 12
--rw-r--r--  2.0 unx       80 b- defN 23-Mar-20 20:43 MCRP/__init__.py
--rw-r--r--  2.0 unx      611 b- defN 23-Mar-20 20:43 MCRP/iautil.py
--rw-r--r--  2.0 unx    14614 b- defN 23-Mar-20 20:43 MCRP/mcrp.py
--rw-r--r--  2.0 unx     5931 b- defN 23-Mar-20 20:43 MCRP/mcwp.py
--rw-r--r--  2.0 unx     4157 b- defN 23-Mar-20 20:43 MCRP/tcproxy.py
--rw-r--r--  2.0 unx      882 b- defN 23-Mar-20 20:43 MCRP/util.py
--rw-rw-rw-  2.0 unx    35060 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     7314 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 23-Mar-20 20:44 MCRP-0.1.9.dist-info/RECORD
-12 files, 69670 bytes uncompressed, 23055 bytes compressed:  66.9%
+Zip file size: 28524 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-08 16:48 MCRP/__init__.py
+-rw-r--r--  2.0 unx     6142 b- defN 23-Jul-08 16:48 MCRP/dgi.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jul-08 16:48 MCRP/iautil.py
+-rw-r--r--  2.0 unx     1370 b- defN 23-Jul-08 16:48 MCRP/mcdj.py
+-rw-r--r--  2.0 unx     1927 b- defN 23-Jul-08 16:48 MCRP/mcenc.py
+-rw-r--r--  2.0 unx     4070 b- defN 23-Jul-08 16:48 MCRP/mcrp.py
+-rw-r--r--  2.0 unx    12606 b- defN 23-Jul-08 16:48 MCRP/mcsession.py
+-rw-r--r--  2.0 unx     8627 b- defN 23-Jul-08 16:48 MCRP/mcwp.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Jul-08 16:48 MCRP/util.py
+-rw-rw-rw-  2.0 unx    35060 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8286 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1112 b- defN 23-Jul-08 16:48 MCRP-0.2.0rc1.dist-info/RECORD
+15 files, 81531 bytes uncompressed, 26726 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,37 +1,46 @@
 Filename: MCRP/__init__.py
 Comment: 
 
+Filename: MCRP/dgi.py
+Comment: 
+
 Filename: MCRP/iautil.py
 Comment: 
 
+Filename: MCRP/mcdj.py
+Comment: 
+
+Filename: MCRP/mcenc.py
+Comment: 
+
 Filename: MCRP/mcrp.py
 Comment: 
 
-Filename: MCRP/mcwp.py
+Filename: MCRP/mcsession.py
 Comment: 
 
-Filename: MCRP/tcproxy.py
+Filename: MCRP/mcwp.py
 Comment: 
 
 Filename: MCRP/util.py
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/LICENSE
+Filename: MCRP-0.2.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/METADATA
+Filename: MCRP-0.2.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/WHEEL
+Filename: MCRP-0.2.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/entry_points.txt
+Filename: MCRP-0.2.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/top_level.txt
+Filename: MCRP-0.2.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: MCRP-0.1.9.dist-info/RECORD
+Filename: MCRP-0.2.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MCRP/__init__.py

```diff
@@ -1,3 +1,4 @@
-from .mcrp import MCRewriteProxy, Relative, ProtocolDecryptor
+from .mcrp import MCRewriteProxy, Relative
+from .mcenc import ProtocolDecryptor
 
-version = '0.1.9'
+version = '0.2.0-pre1'
```

## MCRP/iautil.py

```diff
@@ -1,28 +1,39 @@
-import re
-
-IPv6_PORT = r"^(\[[\d\D]{1,}\]):([0-9]{1,5})$"
-IPv6 = r"^(\[[\d\D]{1,}\])$"
-
-IPv4_PORT = r"^([0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}):([0-9]{1,5})$"
-IPv4 = r"^[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}$"
+"""
+    iautil
+    ======
+    Internet addresses transforming utilities
+"""
 
-TLD_PORT = r"^(.*):([0-9]{1,5})$"
-TLD = r"^(.*)$"
-
-PATTERNS = [
-    IPv6_PORT,
-    IPv6,
-    IPv4_PORT,
-    IPv4,
-    TLD_PORT,
-    TLD
-]
+import re
+from typing import Tuple
 
-def addr_parser(addr: str, default_port: int):
+def addr_parser(addr: str, default_port: int) -> Tuple[str, int]:
+    """        
+        Parse internet address into Tuple[host: str, port: int]
+        with default port support...
+    """
+
+    IPv6_PORT = r"^(\[[\d\D]{1,}\]):([0-9]{1,5})$" # [::1]:65535 -> Tuple["[::1]", 65535]
+    IPv6 = r"^(\[[\d\D]{1,}\])$" # [::1] -> Tuple["[::1]", default_port]
+
+    IPv4_PORT = r"^([0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}):([0-9]{1,5})$" # 1.1.1.1:80 -> Tuple["1.1.1.1", 80]
+    IPv4 = r"^[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}$" # 1.1.1.1 -> Tuple["1.1.1.1", default_port]
+
+    TLD_PORT = r"^(.*):([0-9]{1,5})$" # yt.be:80 -> Tuple["yt.be", 80]
+    TLD = r"^(.*)$" # yt.be -> Tuple["yt.be", default_port]
+
+    PATTERNS = [
+        IPv6_PORT,
+        IPv6,
+        IPv4_PORT,
+        IPv4,
+        TLD_PORT,
+        TLD
+    ]
 
     for pattern in PATTERNS:
         i = re.findall(pattern, addr)
         if i:
             if isinstance(i[0], str):
                 return i[0], default_port
```

## MCRP/mcrp.py

```diff
@@ -3,381 +3,116 @@
     =======================
 """
 
 import traceback
 import logging
 from importlib import import_module
 from unittest.mock import MagicMock
-from time import sleep
-from Crypto.Cipher import AES
+from time import time, sleep
+
 import datetime
 
 import cubelib
 import MCRP
 
-from .tcproxy import tcproxy
+from ku import ku
 
-from typing import Optional, List, Callable, Tuple
+from typing import Optional, List, Callable, Union
 from types import ModuleType
 
-Relative = MagicMock()
-
-class DebugJournal:
+from copy import copy
+import json
 
-    def __init__(self, file_path: str):
-        self.file = open(file_path, "wb")
-    
-    def append_clientbound(self, packet: bytes):
-        self.add_record(type=0x01, data=packet)
-    
-    def append_serverbound(self, packet: bytes):
-        self.add_record(type=0x02, data=packet)
-    
-    def set_enckey(self, key: bytes):
-        self.add_record(type=0x03, data=key)
+Relative = MagicMock()
 
-    def add_record(self, type: int, data: bytes):
+from .mcenc import ProtocolDecryptor
+from .mcsession import MinecraftSession
 
-        self.file.write(cubelib.types.VarInt.build(type))
-        self.file.write(cubelib.types.VarInt.build(len(data)))
-        self.file.write(data)
-    
-    def close(self):
-        self.file.close()
-
-class ProtocolDecryptor:
-    """
-        Protocol Decryptor Prototype
+class MCRewriteProxy(ku):
+    """    
+        Ku-proxy with mcsession, join() ja cross-session handlers.
     """
-
-    name: str
-    version: str
-
-    def __init__(self, logger):
-        pass
-
-    def EncryptionRequest(self, server_id: str, public_key: bytes, verify_token: str) -> Tuple[bytes, str, str]:
-        """
-        External Encryption Request handler for decryption setup purposes
-
-        Args:
-            server_id (str): EncryptionRequest.ServerID
-            public_key (bytes): EncryptionRequest.PublicKey
-            verify_token (bytes): EncryptionRequest.VerifyToken
-        
-        Returns:
-            server_id (str): New server id
-            public_key (bytes): New public key
-            verify_token (bytes): New verify token
-        """        
-        pass
     
-    def EncryptionResponse(self, shared_secret: bytes, verify_token: bytes) -> Tuple[bytes, bytes, bytes]:
-        """
-        External Encryption Response handler for decryption setup purposes
-
-        Args:
-            shared_secret (bytes): EncryptionResponse.SharedSecret
-            verify_token (bytes): EncryptionResponse.VerifyToken
-        
-        Returns:
-            shared_secret (bytes): Plain shared secret
-            shared_secret (bytes): Encrypted shared secret
-            verify_token (bytes): Encrypted verify token
-        """          
-        pass
+    handlers: dict
+    relative_handlers: dict
+    PSM = 0 # broken timings on compression establishment issue[cubelib #3] (don't stop! don't stop!)
+
+    def __init__(self, listen: tuple, upstream: tuple,
+        loglevel = logging.INFO, session: MinecraftSession = MinecraftSession,
+        decryptor: Optional[ProtocolDecryptor] = None,
+        leave_debug_journals: bool = False, maxcon: int = -1,
+        upstream_6: bool = False, ku_loglevel = logging.ERROR):
 
-class AESCipher:
-    
-    Encryptor: AES
-    Decryptor: AES
-
-    def __init__(self, secret: bytes):
-        self.Encryptor = AES.new(secret, AES.MODE_CFB, iv=secret)
-        self.Decryptor = AES.new(secret, AES.MODE_CFB, iv=secret)
-
-class AESComplex:
-
-    ClientCipher: AESCipher
-    ServerCipher: AESCipher
-
-    def __init__(self, secret):
-        self.ClientCipher = AESCipher(secret)
-        self.ServerCipher = AESCipher(secret)
-
-class MCRewriteProxy(tcproxy):    
-
-    ServerBoundBuff: List[bytes]
-    ClientBoundBuff: List[bytes]
-
-    PROTOCOL: ModuleType = cubelib.proto
-    STATE: cubelib.state = cubelib.state.Handshaking
-    COMPRESSION_THR: int = -1
-
-    PASS_THROUGH: bool = False
-    decryptor: Optional[ProtocolDecryptor] = None
-    cipher: AESComplex
-
-    HANDLERS: dict # {cubelib.proto.v47.ServerBound.ChatMessage: [False, <function handler at 0x00000...>]}
-    REL_HANDLERS: dict
-
-    ServerBoundHandler: Optional[Callable] = None
-    ClientBoundHandler: Optional[Callable] = None
-    IntersessionHandler: Optional[Callable] = None
-    
-    def __init__(self, listen_addr: tuple, upstream_addr: tuple,
-        loglevel = logging.ERROR, decryptor: Optional[ProtocolDecryptor] = None,
-            leave_debug_journals: bool = False):
+        self.version_string = f"MCRP/{MCRP.version} (cubelib version {cubelib.version})"
         
-        self.ServerBoundBuff = [b""] # it's a little trick to make immutable type (bytes)
-        self.ClientBoundBuff = [b""] # mutable to pass reference to it
-        self.HANDLERS = {}
-        self.REL_HANDLERS = {}
-        self.leave_debug_journals = leave_debug_journals
-
         self.logger = logging.getLogger("MCRP")
         self.logger.setLevel(loglevel)
-        super().__init__(listen_addr, upstream_addr)
-        self.logger.info(f"Running MCRP v{MCRP.version} (cubelib version {cubelib.version})")
-        self.logger.info(f"Proxying config is: \u001b[97m{':'.join([str(a) for a in listen_addr])} \u001b[92m-> \u001b[97m{':'.join([str(a) for a in upstream_addr])}")
+        self.logger.info(f"Running {self.version_string}")
+        self.logger.info(f"Proxying config is: \u001b[97m{listen[0]}:{listen[1]} \u001b[92m-> \u001b[97m{':'.join([str(a) for a in upstream])}")
         self.logger.info(f"Using protocol decryptor: {decryptor.name}/{decryptor.version}") if decryptor else None
-        self.logger.info(f"Debug journals enabled!") if leave_debug_journals else None
+        self.logger.info(f"Debug journaling enabled!") if leave_debug_journals else None
+
         if decryptor:
             crlogger = logging.getLogger("MCRP/CRYPTO")
             crlogger.setLevel(loglevel)
             self.decryptor = decryptor(crlogger)              
-    
-    def _waiting_for_client(self):
-        
-        self.IntersessionHandler() if self.IntersessionHandler else None
-        self.logger.info(f"Waiting for client connection...")
-
-    def _new_client(self):
-
-        self.logger.info(f"New client, creating connection to the server")
-            
-    def _new_server(self):
-
-        self.logger.info(f"Connected to the server")
-        self.logger.info("Reseting state to Handshaking")
-        self.STATE = cubelib.state.Handshaking
-        self.PROTOCOL = cubelib.proto
-        self.COMPRESSION_THR = -1
-        self.ServerBoundBuff = [b""]
-        self.ClientBoundBuff = [b""]
-        self.PASS_THROUGH = False        
-        self.cipher = None
-        if self.leave_debug_journals:
-            dt = datetime.datetime.now()
-            m = dt.strftime("%B")[:3]
-            ts = dt.strftime(f"%d {m} %Y %H-%M-%S")
-            self.logger.info(f"Starting debug journaling in file [{ts}.mcdj]")
-            self.journal = DebugJournal(f"{ts}.mcdj")            
-
-        # Remove relative handlers for old protocol
-        for handler in dict(self.HANDLERS):
-            if self.HANDLERS[handler][0] == True:
-                del self.HANDLERS[handler]        
-    
-    def _client_lost(self):
-
-        self.logger.info(f"Client disconnected")
-    
-    def _server_lost(self):
-
-        if self.leave_debug_journals:
-            self.journal.close()
-        self.logger.info(f"Server disconnected")
-    
-    def _server_error(self, error):
-        
-        self.logger.error(f"Failed to connect to the server due to an error: {error}")
-    
-    def _from_client(self, data):
-
-        return self._handle_bytes(data, self.ServerBoundBuff, cubelib.bound.Server)
-
-    def _from_server(self, data):
 
-        return self._handle_bytes(data, self.ClientBoundBuff, cubelib.bound.Client)
+        self.listen = listen
+        self.upstream = upstream
 
-    def _client_error(self, error):
-        
-        self.logger.critical(f"Failed to bind socket to local addr due to an error: {error}")
-        exit()
-
-    def _handle_bytes(self, data, buff, bound):
-        
-        if self.leave_debug_journals:
-            (self.journal.append_clientbound if bound is cubelib.bound.Client else self.journal.append_serverbound)(data)
-
-        was_encrypted = False
-        if self.cipher:
-            if bound is cubelib.bound.Server:
-                data = self.cipher.ServerCipher.Decryptor.decrypt(data)
-            elif bound is cubelib.bound.Client:
-                data = self.cipher.ClientCipher.Decryptor.decrypt(data)
-            was_encrypted = True
-
-        if data[:3] == b"\xFE\x01\xFA" and self.STATE == cubelib.state.Handshaking:
-            self.logger.warn("Client sent legacy MC|PingHost! Unsupported! Enabling pass-trough!")
-            self.PASS_THROUGH = True
-
-        if self.PASS_THROUGH:
-            r = b""
-            if buff[0]:
-                r += buff[0]
-                buff[0] = b""
-            r += data
-            return r
-
-        try:
-            packs = []
-            buff[0] += data
-            buff[0] = cubelib.readPacketsStream(buff[0], self.COMPRESSION_THR, bound, packs)            
-
-            ret = b""
-            for p in packs:
-                if self.PASS_THROUGH:
-                    ret += p.build(self.COMPRESSION_THR if p.compressed else -1)
-                    continue # if the Handshake is sent in one buffer with LoginStart
-                             # but proto is unsupported, we need to skip it right there
-                try:
-                    hr = self._handle_packet(p)
-                    if isinstance(hr, bytes):
-                        ret += hr
-                    elif isinstance(hr, cubelib.p.Night):
-                        ret += hr.build(self.COMPRESSION_THR if p.compressed else -1)
-                    elif hr is False:
-                        ret += b""
-                    else:
-                        ret += p.build(self.COMPRESSION_THR if p.compressed else -1)
-                        if hr is  not None:
-                            self.logger.warn(f'обработчик сделал хуйню (вернул {hr})')                    
-
-                except Exception as e:
-                    self.logger.warn(f"Exception in {bound.name}Bound Handler: {e}")                    
-                    self.logger.warn(traceback.format_exc())
-                    ret += p.build(self.COMPRESSION_THR if p.compressed else -1)
-            
-            if self.cipher and was_encrypted:
-                return self.cipher.ServerCipher.Encryptor.encrypt(ret) if bound is cubelib.bound.Server else self.cipher.ClientCipher.Encryptor.encrypt(data)            
-            return ret
-
-        except Exception as e:
-            self.logger.error(f"Exception in {bound.name}Bound: {e}")
-            self.logger.error(traceback.format_exc())            
-
-    def _handle_packet(self, pack):
-        
-        p = pack.resolve(self.STATE, self.PROTOCOL)
-        t = p.__class__
+        self.session = session
+        self.maxcon = maxcon
+        self.upstream_6 = upstream_6
+        self.leave_debug_journals = leave_debug_journals
+        self.loglevel = loglevel
+        self.ku_loglevel = ku_loglevel
 
-        # Global bound handlers
-        if pack.bound == cubelib.bound.Client:
-            self.ClientBoundHandler(p) if self.ClientBoundHandler else None
-        else:
-            self.ServerBoundHandler(p) if self.ServerBoundHandler else None                
-
-        # Handle handshake
-        if t is cubelib.proto.ServerBound.Handshaking.Handshake:
-            self._handle_handshake(p)
-            # Call a handler if exists, prematurely to prevent state check if proto not loaded
-            return self.HANDLERS[t][1](p) if t in self.HANDLERS else None
-
-        if self.STATE is cubelib.state.Login:
-            
-            # Handle SetCompression
-            if t is self.PROTOCOL.ClientBound.Login.SetCompression:
-                self.logger.info(f"Point of switching-on compression with threshold {p.Threshold}")
-                self.COMPRESSION_THR = p.Threshold
-
-            # Handle LoginSuccess
-            if t is self.PROTOCOL.ClientBound.Login.LoginSuccess:
-                self.STATE = cubelib.state.Play
-                self.logger.info(f"State changed to {self.STATE}")
-            
-            # Handle EncryptionRequest
-            if t is self.PROTOCOL.ClientBound.Login.EncryptionRequest:
-                if self.decryptor:
-                    hr = self.decryptor.EncryptionRequest(p.ServerID, p.PublicKey, p.VerifyToken)
-                    return self.PROTOCOL.ClientBound.Login.EncryptionRequest(*hr)
-                return
-
-            # Handle EncryptionResponse
-            if t is self.PROTOCOL.ServerBound.Login.EncryptionResponse:
-                if self.decryptor:
-                    hr = self.decryptor.EncryptionResponse(p.SharedSecret, p.VerifyToken)
-                    self.cipher = AESComplex(hr[0])
-                    self.logger.info(f"Protocol encryption is set, but you provided a shared secret")
-                    self.logger.info(f"Shared secret: {hr[0].hex()}")
-                    if self.leave_debug_journals:
-                        self.journal.set_enckey(hr[0])
-                    return self.PROTOCOL.ServerBound.Login.EncryptionResponse(*hr[1:])
-                self.logger.warn(f"Minecraft client sent EncryptionResponse! That mean full symmetric encryption enabling, so we can't proceed with protocol analyzing. Just proxying!")
-                self.PASS_THROUGH = True
-                return
+        self.handlers: dict = {}
+        self.relative_handlers: dict = {}
 
-        # Call a handler if exists        
-        return self.HANDLERS[t][1](p) if t in self.HANDLERS else None
+    def join(self):
         
-    def _handle_handshake(self, p):
+        self.logger.info(f'Registred direct handlers list[{len(self.handlers)}]:')
+        for name, handlers in self.handlers.items():
+            self.logger.info(f"[{len(handlers[1])}]    {name}")
+
+        self.logger.info(f'Registred relative handlers list[{len(self.relative_handlers)}]:')
+        for name, handlers in self.relative_handlers.items():
+            self.logger.info(f"[{len(handlers)}]    {'.'.join(name._extract_mock_name().split('.')[1:])}")
+
+        args = (self.logger, self.handlers, self.relative_handlers, self.leave_debug_journals)
+        super().__init__(self.listen, self.upstream, self.session, args, self.maxcon, self.upstream_6, self.ku_loglevel)
+
+        self.logger.debug("Entering mainloop")
+        while self.alive:
+            try:
+                sleep(0.017)
+            except KeyboardInterrupt:
+                self.logger.debug("Shutting down...")
+                self.shutdown()
+                break
 
-        if p.NextState == cubelib.NextState.Status:
-            self.STATE = cubelib.state.Status
-            return
-        
-        self.STATE = cubelib.state.Login
-        self.logger.info(f"State changed to {self.STATE}, trying to load protocol v{p.ProtoVer}")
-        if p.ProtoVer in cubelib.supported_versions:        
-            self.PROTOCOL = import_module(f"cubelib.proto.v{p.ProtoVer}")
-        else:
-            self.logger.warn(f"Failed to load protocol v{p.ProtoVer}, looks like it's unsupported! Enabling enabling pass-through")
-            self.PASS_THROUGH = True
-            return
-
-        self.logger.info(f"Successfuly loaded protovol v{p.ProtoVer}" + (f", compiling {len(self.REL_HANDLERS)} handlers..." if self.REL_HANDLERS else ""))
-
-        for handler in self.REL_HANDLERS:
-            attrs = handler._extract_mock_name().split('.')[1:]
-            obj = self.PROTOCOL
-            for attr in attrs:
-                obj = getattr(obj, attr, None)
-                if not obj:
-                    self.logger.warn(f'Failed to resolve handler {self.PROTOCOL.__name__}.{".".join(attrs)}')
-                    break
-            if obj:
-                self.logger.debug(f"Successfully resolved {handler} into {obj}")
-                self.HANDLERS[obj] = [True, self.REL_HANDLERS[handler]]
+        self.logger.debug("Exiting...")
 
     def on(self, type_):
         def no(fun):
             if isinstance(type_, MagicMock):
-                self.REL_HANDLERS[type_] = fun
+                if type_ in self.relative_handlers:
+                    self.relative_handlers[type_].append(fun)
+                else:
+                    self.relative_handlers[type_] = [fun]
             else:
-                self.HANDLERS[type_] = [False, fun]
+                if type_ in self.handlers:
+                    self.handlers[type_][1].append(fun)
+                else:
+                    self.handlers[type_] = [False, [fun]]
+            return fun
         return no
     
-    def ClientBound(self, handler):
-        self.ClientBoundHandler = handler
-    
-    def ServerBound(self, handler):
-        self.ServerBoundHandler = handler
-    
-    def Intersession(self, handler):
-        self.IntersessionHandler = handler
+    def purge_rel_handlers(self):
+        """Remove active relative handlers"""
 
-    def join(self):
-        
-        self.logger.info(f'Registred direct handlers list[{len(self.HANDLERS)}]:')
-        for handler in self.HANDLERS:
-            self.logger.info(f"    {handler}")
-
-        self.logger.info(f'Registred relative handlers list[{len(self.REL_HANDLERS)}]:')
-        for handler in self.REL_HANDLERS:            
-            self.logger.info(f"    {'.'.join(handler._extract_mock_name().split('.')[1:])}")
-
-        self.logger.debug('Entering mainloop')
-        super().join()    
-        #p = self.PROTOCOL.ClientBound.Play.Disconnect('proxy_closed').build(self.COMPRESSION_THR)
-        #self.Client.send(p)
-        self.logger.debug('Exiting')
+        for handler in dict(self.handlers):
+            if self.handlers[handler][0] == True: # if relative
+                del self.handlers[handler]
+
+        self.relative_handlers.clear() # remove relative handlers from all sessions
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## MCRP/mcwp.py

```diff
@@ -1,43 +1,53 @@
 """
     MineCraft Watching Proxy
     ========================
 """
 
-from MCRP import MCRewriteProxy, Relative, version
+from MCRP import MCRewriteProxy, version
+from .dgi import DeepGameInteractionMachine
 from .util import CustomFormatter
 from .iautil import addr_parser
 
 import cubelib
 
 from ruamel.yaml import YAML
 import argparse
 import logging
 from importlib.machinery import SourceFileLoader
+import traceback
+from .mcsession import MinecraftSession
 
 BANNER = \
 f"""
  __  __   ____  ____   ____       __        __ ____
 |  \/  | / ___||  _ \ |  _ \  _   \ \      / /|  _ \\
 | |\/| || |    | |_) || |_) |(_)   \ \ /\ / / | |_) |
 | |  | || |___ |  _ < |  __/  _     \ V  V /  |  __/
 |_|  |_| \____||_| \_\|_|    (_)     \_/\_/   |_| v{version}
 """
 
+class WatchingSession(MinecraftSession):
+    """Watching session"""
+
 def main():
 
     print(BANNER[1:])
     parser = argparse.ArgumentParser(description="Minecraft Watching Proxy")
     parser.add_argument("-c", type=argparse.FileType("r", encoding="utf-8"), help="Path to the YAML config file", metavar="config.yaml")
     parser.add_argument("-v", action="store_true", help="If passed, enables verbose logging")
     parser.add_argument("-l", help="Proxy listen addr [localhost:25565] (enclose ipv6 like [::])", default="127.0.0.1:25565", metavar="addr")
     parser.add_argument("-u", help="Proxy upstream server addr [localhost:25575]", default="127.0.0.1:25575", metavar="addr")
     parser.add_argument("-d", help="Protocol decryption module", metavar="decmod")
-    parser.add_argument("-ll", action="store_true", help="If passed, enables low level debug logging")
-    parser.add_argument("--leave-debug-journals", action="store_true", help="If passed, leaves debug journals", dest="ldj")
+    parser.add_argument("-ll", action="store_true", help="If passed, enables network debug logging")
+    parser.add_argument("--leave-debug-journals", action="store_true", help="If passed, leaves debug journals", dest="ldj")    
+    parser.add_argument("--ext", help="Module with register() containing external handlers", metavar="handlers")
+    parser.add_argument("-derf", action="store_true", help="Disable entities resolving and following")
+    parser.add_argument("--ext-sore", action="store_true", help="Show rejected packets", dest="sore")
+    parser.add_argument("--devel", action="store_true")
     args = parser.parse_args()
     
     decryptor = SourceFileLoader("", f"{args.d}.py").load_module().MCWPDecryptor if args.d else None
 
     if args.c:
         yaml = YAML(typ="safe")
         conf = yaml.load(args.c)
@@ -47,53 +57,73 @@
     logger = logging.getLogger("")
     logger.setLevel(logging.DEBUG if args.v else logging.INFO)
     stdout_handler = logging.StreamHandler()
     stdout_handler.setLevel(logging.DEBUG)
     stdout_handler.setFormatter(CustomFormatter('[%(asctime)s] [%(levelname)s] %(name)s:  %(message)s'))
     logger.addHandler(stdout_handler)
 
+    # External handlers area
+    if args.ext:
+        try:
+            external_handlers = SourceFileLoader("", f"{args.ext}.py").load_module().register
+        except Exception as e:
+            logger.error("Failed to load external handlers! There is no module with name given or it doesn't have register()")
+            logger.error("\n" + traceback.format_exc())
+            return
+
     limit = conf["loglimit"] if "loglimit" in conf else None
     if "mode" in conf:
         cbmode = conf["mode"]
         sbmode = conf["mode"]
     elif "ClientBoundMode" in conf and "ServerBoundMode" in conf:
         cbmode = conf["ClientBoundMode"]
         sbmode = conf["ServerBoundMode"]
         conf["mode"] = f"ClB: {cbmode} / SvB: {sbmode}"
     else:
-        logger.error(f"Failed to read configuration! please declate 'mode' or 'ClientBoundMode' and 'ServerBoundMode'")
+        logger.error(f"Failed to read configuration! please declare 'mode' or 'ClientBoundMode' and 'ServerBoundMode'")
         exit()
 
+    if args.devel:
+        logger.error(("/stop"*7)[1:])
+        conf = {"mode": "whitelist"}
+
     proxy = MCRewriteProxy(addr_parser(args.l, 25565), addr_parser(args.u, 25565),
-        logging.DEBUG if args.ll else logging.INFO if args.v else logging.WARNING,
-            decryptor=decryptor, leave_debug_journals=args.ldj)
+        logging.DEBUG if args.v else logging.INFO,
+        WatchingSession, decryptor=decryptor, leave_debug_journals=args.ldj,
+        maxcon=1 if not args.devel else 7, ku_loglevel=logging.DEBUG if args.ll else logging.ERROR)
+
+    if args.ext:
+        external_handlers(proxy)
+
+    if args.derf:
+        logger.info("Entities resolving and following are disabled!")
 
     ClientBoundFilterList = []
     ServerBoundFilterList = []
 
     @proxy.on(cubelib.proto.ServerBound.Handshaking.Handshake)
-    def handler(packet):
+    def handler(sess, packet):
         nonlocal ClientBoundFilterList, ServerBoundFilterList
 
         if packet.NextState != cubelib.NextState.Login:
             return cubelib.proto.ServerBound.Handshaking.Handshake(packet.ProtoVer, *addr_parser(args.u, 25565), packet.NextState)
 
         logger.debug(f'Selected proto version is: {packet.ProtoVer}, building filter...')
-        proto = proxy.PROTOCOL
+        proto = sess.protocol
 
         def find_ap_by_path(proto, path):
             obj = proto
             attrs = path.split('.')
             if attrs[-1] == "NotImplementedPacket":
                 return cubelib.p.NotImplementedPacket
 
             for attr in attrs:
                 obj = getattr(obj, attr, None)
                 if not obj:
-                    logger.debug(f'\x1b[38;5;226mFailed to resolve filter packet {proxy.PROTOCOL.__name__}.{".".join(attrs)}')
+                    logger.warning(f'Failed to resolve filter packet {sess.protocol.__name__}.{".".join(attrs)}')
                     break
             return obj
         
         ClientBoundFilterList = [find_ap_by_path(proto, "ClientBound.Play." + packet) for packet in conf["ClientBound"]] if "ClientBound" in conf else []
         ServerBoundFilterList = [find_ap_by_path(proto, "ServerBound.Play." + packet) for packet in conf["ServerBound"]] if "ServerBound" in conf else []
         ClientBoundFilterList = [i for i in ClientBoundFilterList if i is not None]
         ServerBoundFilterList = [i for i in ServerBoundFilterList if i is not None]
@@ -111,37 +141,75 @@
         return cubelib.proto.ServerBound.Handshaking.Handshake(packet.ProtoVer, *addr_parser(args.u, 25565), packet.NextState)
 
     def log_clientbound(*args):
         logger.info(f'\u001b[96mClientBound   {" ".join([str(a) for a in args])}\u001b[0m')
 
     def log_serverbound(*args):
         logger.info(f'\u001b[95mServerBound   {" ".join([str(a) for a in args])}\u001b[0m')
+    
+    def log_rewrite(*args):
+        logger.info(f'\x1b[38;2;186;220;88m{" ".join([str(a) for a in args])}\u001b[0m')
 
     def filter_(packet, mode, list_):
         if mode == "blacklist":
             if packet.__class__ in list_:
                 return False
             return True
 
         elif mode == "whitelist":
             if packet.__class__ in list_:
                 return True
             return False
 
-    @proxy.ClientBound
-    def handler(packet):
+    def handler(sess, packet):
+        packet = sess.dgim(packet) if sess.dgim else packet
         if filter_(packet, cbmode, ClientBoundFilterList):
             log_clientbound(packet) if not limit else log_clientbound(str(packet)[:limit])
+    WatchingSession.ClientBoundHandler = handler
 
-    @proxy.ServerBound
-    def handler(packet):
+    def handler(sess, packet):
+        packet = sess.dgim(packet) if sess.dgim else packet
         if filter_(packet, sbmode, ServerBoundFilterList):
             log_serverbound(packet) if not limit else log_serverbound(str(packet)[:limit])
+    WatchingSession.ServerBoundHandler = handler
 
-    @proxy.Intersession
-    def handler():
+    def handler(sess):        
+        if not args.derf:
+            sess.dgim = DeepGameInteractionMachine(sess)
+        else:
+            sess.dgim = None
         print()
+    WatchingSession.IntersessionHandler = handler
+    
+    def handler(sess, source, replace):
+        if replace != False:
+            log_rewrite(source, "->", replace)
+        else:
+            if args.sore:
+                log_rewrite(source, "was rejected")
+    WatchingSession.RewriteHandler = handler
+
+    def reload(sess):
+        """Re-load external handlers into the proxy instance"""
+        proxy.purge_rel_handlers()
+
+        if args.ext:
+            try:
+                external_handlers = SourceFileLoader("", f"{args.ext}.py").load_module().register
+            except Exception as e:
+                logger.error("Failed to reload external handlers! There is no module with name given or it doesn't have register()")
+                logger.error("\n" + traceback.format_exc())
+        else:
+            logger.error("You can't reload external handlers 'cause they are not used!")
+            return
+
+        external_handlers(proxy)
+        sess.resolve_handlers()
+    
+    proxy.reload = reload
 
     proxy.join()
 
+    logger.info("Finalizing")
+
 if __name__ == "__main__":
     main()
```

## MCRP/util.py

```diff
@@ -1,7 +1,13 @@
+"""
+    util
+    ====
+    Just my colored logging preset
+"""
+
 import logging, os
 os.system('color')
 
 class CustomFormatter(logging.Formatter):    
     
     grey = '\u001b[34m'
     blue = '\x1b[38;5;39m'
```

## Comparing `MCRP-0.1.9.dist-info/LICENSE` & `MCRP-0.2.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MCRP-0.1.9.dist-info/METADATA` & `MCRP-0.2.0rc1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCRP
-Version: 0.1.9
+Version: 0.2.0rc1
 Summary: Minecraft MITM proxy with function of rewriting packets, written in pure Python 3
 Home-page: https://gitlab.com/seeklay/MCRP
 Author: seeklay
 Author-email: rudeboy@seeklay.icu
 License: GNU General Public License v3.0
 Download-URL: https://gitlab.com/seeklay/MCRP
 Platform: OS Independent
@@ -17,25 +17,42 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
 Requires-Dist: cubelib (>=1.0.3-pre.1)
 Requires-Dist: ruamel.yaml (==0.17.21)
+Requires-Dist: ku-proxy (>=0.2.1)
+Requires-Dist: pycryptodome
 
 # MCRP: Minecraft Rewrite Proxy
 
 Minecraft MITM proxy with function of rewriting packets, written in pure [Python 3](https://www.python.org/).
 
-![](https://img.shields.io/badge/Made%20with-Python-1f425f.svg) ![](https://img.shields.io/gitlab/license/seeklay/MCRP.svg) ![](https://tokei.rs/b1/gitlab/seeklay/MCRP) ![](https://badgen.net/gitlab/release/seeklay/MCRP) ![](https://badgen.net/pypi/v/MCRP) ![](https://img.shields.io/pypi/dw/MCRP?style=flat&logo=pypi)
+[![](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![](https://img.shields.io/gitlab/license/seeklay/MCRP.svg)](LICENSE/) [![](https://tokei.rs/b1/gitlab/seeklay/MCRP)](#) [![](https://badgen.net/pypi/v/MCRP) ![](https://img.shields.io/pypi/dw/MCRP?style=flat&logo=pypi)](https://pypi.org/project/cubelib/) [![](https://badgen.net/gitlab/release/seeklay/MCRP)](https://gitlab.com/seeklay/MCRP/-/releases)
 
 ## About
 
 **MCRP** provides cool interface to interact with minecraft packets goes via proxy.
 
+# What's new in v0.2.0
+* powered by ku-proxy backend
+* add session-based multiclient support
+* split single file into  separate modules
+* rework logging levels, bind network logging with -ll
+* add --ext-sore
+* add&fix bug when LoginSuccess was read as uncompressed (cubelib issue #3)
+
+## Announce
+No new features will be released on base of `v0.1`.
+Only security/bugfixes if needed.
+Now the project will develop in the direction of replacing network engine with `ku`.
+Release `v0.2` will have same functionality but written around ku.
+https://gitlab.com/seeklay/ku
+
 ## Supported versions
 
 >This note about **Play** state only! **Handshaking**, **Status**, **Login** fully supported and version-independent.
 
 Absolutely Supported: Minecraft 1.8-1.8.9
 Chat supported: Minecraft 1.12.2
 For more information on supported protocols, visit the [cubelib](https://gitlab.com/seeklay/cubelib) page on gitlab, because protocol support lies with it.
@@ -50,89 +67,90 @@
 
 ```bash
 $> mcwp -h
  __  __   ____  ____   ____       __        __ ____
 |  \/  | / ___||  _ \ |  _ \  _   \ \      / /|  _ \
 | |\/| || |    | |_) || |_) |(_)   \ \ /\ / / | |_) |
 | |  | || |___ |  _ < |  __/  _     \ V  V /  |  __/
-|_|  |_| \____||_| \_\|_|    (_)     \_/\_/   |_| v0.1.8
+|_|  |_| \____||_| \_\|_|    (_)     \_/\_/   |_| v0.2.0-pre1
 
-usage: mcwp [-h] [-c config.yaml] [-v] [-l addr] [-u addr] [-d decmod] [-ll]
-            [--leave-debug-journals]
+usage: mcwp.py [-h] [-c config.yaml] [-v] [-l addr] [-u addr] [-d decmod]
+               [-ll] [--leave-debug-journals] [--ext handlers] [-derf]
+               [--ext-sore] [--devel]
 
 Minecraft Watching Proxy
 
 optional arguments:
   -h, --help            show this help message and exit
   -c config.yaml        Path to the YAML config file
   -v                    If passed, enables verbose logging
   -l addr               Proxy listen addr [localhost:25565] (enclose ipv6 like
                         [::])
   -u addr               Proxy upstream server addr [localhost:25575]
   -d decmod             Protocol decryption module
-  -ll                   If passed, enables low level debug logging
+  -ll                   If passed, enables network debug logging
   --leave-debug-journals
                         If passed, leaves debug journals
+  --ext handlers        Module with register() containing external handlers
+  -derf                 Disable entities resolving and following
+  --ext-sore            Show rejected packets
+  --devel
 ```
 ## Requirements
 
-* Python 3 (tested and developed under `Python 3.7.9`)
+* Python 3.7 and above (tested and developed under `Python 3.7.9`)
 * [cubelib](https://gitlab.com/seeklay/cubelib) >= 1.0.3-pre.1
 * [ruamel.yaml](https://pypi.org/project/ruamel.yaml/) == 0.17.21
 * [pycryptodome](https://pypi.org/project/pycryptodome/)
+* [ku](https://gitlab.com/seeklay/ku-proxy) >= 0.2.1
+
 ## Installation
 
 MCRP is published in [PyPI](https://pypi.org/project/cubelib/), so latest release can be installed with one simple command:
 ```bash
 pip install -U mcrp
 ```
 
 or bleeding edge from git sources (unstable) (may not work at all!):
 
 ```bash
 git clone https://gitlab.com/seeklay/MCRP.git
 cd mcrp/
 pip3 install .
 ```
+## Docs
+# Check out our new cool pretty terrifying amazing documentation [HERE](https://mcrp.seeklay.pp.ua)
 
 ## Usage examples
-*if you set a domain name as a listen or an upstream address, ipv4 will used, ipv6 works only with addresses in this notation: [::1]. if the port is not specified, the default will be 25565*
+*if you set a domain name as a listen or an upstream address, ipv4 will used, ipv6 works only with addresses in this notation: [::1]. if the port is not specified, the default will be 25565. if upstream/listen addr not specified 25565->25575 at localhost will be used by default*
+> default configured mcwp and normal ping sequence (mcsr used)
 ```bash
-$> mcwp -c examples\conf_blacklist.yaml -v -ll -d md --leave-debug-journals -l localhost
+$> mcwp -c examples\conf_blacklist.yaml
  __  __   ____  ____   ____       __        __ ____
 |  \/  | / ___||  _ \ |  _ \  _   \ \      / /|  _ \
 | |\/| || |    | |_) || |_) |(_)   \ \ /\ / / | |_) |
 | |  | || |___ |  _ < |  __/  _     \ V  V /  |  __/
-|_|  |_| \____||_| \_\|_|    (_)     \_/\_/   |_| v0.1.8
-
-[03/19/2023 04:08:39 AM] [INFO] MCRP:  Running MCRP v0.1.8 (cubelib version 1.0.5-pre1)
-[03/19/2023 04:08:39 AM] [INFO] MCRP:  Proxying config is: localhost:25565 -> 127.0.0.1:25575
-[03/19/2023 04:08:39 AM] [INFO] MCRP:  Using protocol decryptor: Yggdrasil-Server-DecMod/v0.1.1
-[03/19/2023 04:08:39 AM] [INFO] MCRP:  Debug journals enabled!
-[03/19/2023 04:08:39 AM] [DEBUG] MCRP/CRYPTO:  Generating 1024 RSA key...
-[03/19/2023 04:08:40 AM] [INFO] MCRP:  Registred direct handlers list[1]:
-[03/19/2023 04:08:40 AM] [INFO] MCRP:      <class 'cubelib.proto.version_independent.ServerBound.Handshaking.Handshake'>
-[03/19/2023 04:08:40 AM] [INFO] MCRP:  Registred relative handlers list[0]:
-[03/19/2023 04:08:40 AM] [DEBUG] MCRP:  Entering mainloop
-
-[03/19/2023 04:08:40 AM] [INFO] MCRP:  Waiting for client connection...
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  New client, creating connection to the server
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  Connected to the server
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  Reseting state to Handshaking
-[02/20/2023 09:33:02 PM] [INFO] root:  ServerBound   Handshaking.Handshake(ProtoVer=47, ServerName='lc', ServerPort=25565, NextState=NextState.Status)
-[02/20/2023 09:33:02 PM] [INFO] root:  ServerBound   Status.Request()
-[02/20/2023 09:33:02 PM] [INFO] root:  ClientBound   Status.Response(JsonRsp='{"description":"A Minecraft Server","players":{"max":20,"online":0},"version":{"name":"Spigot 1.8.8","protocol":47}}')
-[02/20/2023 09:33:02 PM] [INFO] root:  ServerBound   Status.Ping(Uniq=133772128)
-[02/20/2023 09:33:02 PM] [INFO] root:  ClientBound   Status.Pong(Uniq=133772128)
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  Client disconnected
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  Server disconnected
+|_|  |_| \____||_| \_\|_|    (_)     \_/\_/   |_| v0.2.0-pre1
 
-[02/20/2023 09:33:02 PM] [INFO] MCRP:  Waiting for client connection...
+[07/08/2023 11:18:42 PM] [INFO] MCRP:  Running MCRP/0.2.0-pre1 (cubelib version 1.0.9)
+[07/08/2023 11:18:42 PM] [INFO] MCRP:  Proxying config is: 127.0.0.1:25565 -> 127.0.0.1:25575
+[07/08/2023 11:18:42 PM] [INFO] MCRP:  Registred direct handlers list[1]:
+[07/08/2023 11:18:42 PM] [INFO] MCRP:  [1]    <class 'cubelib.proto.version_independent.ServerBound.Handshaking.Handshake'>
+[07/08/2023 11:18:42 PM] [INFO] MCRP:  Registred relative handlers list[0]:
+
+[07/08/2023 11:18:44 PM] [INFO] MCRP:  #2006377812680 ready for trasmission
+[07/08/2023 11:18:44 PM] [INFO] root:  ServerBound   Handshaking.Handshake(ProtoVer=-1, ServerName='localhost', ServerPort=25565, NextState=state.Status)
+[07/08/2023 11:18:44 PM] [INFO] root:  Handshaking.Handshake(ProtoVer=-1, ServerName='localhost', ServerPort=25565, NextState=state.Status) -> Handshaking.Handshake(ProtoVer=-1, ServerName='127.0.0.1', ServerPort=25575, NextState=state.Status)
+[07/08/2023 11:18:44 PM] [INFO] root:  ServerBound   Status.Request()
+[07/08/2023 11:18:44 PM] [INFO] root:  ClientBound   Status.Response(JsonRsp='{"description":"A Minecraft Server","players":{"max":20,"online":0},"version":{"name":"Spigot 1.8.8","protocol":47}}')
+[07/08/2023 11:18:44 PM] [INFO] root:  ServerBound   Status.Ping(Uniq=1337)
+[07/08/2023 11:18:44 PM] [INFO] root:  ClientBound   Status.Pong(Uniq=1337)
+[07/08/2023 11:18:44 PM] [INFO] MCRP:  #2006377812680 connection_lost by server due to None
 ```
-See [**examples/**](examples/) for MCRP usage details
+See [**examples/**](examples/) for MCRP and MCWP external handlers usage details
 
 ## Protocol decryption
 ### MCWP
 For protocol decryption enabling you need user to use your instance of [yggdrasil-server](https://gitlab.com/seeklay/yggdrasil-server) 
 Add `-d md` arg to mcwp command to use standard yggdrasil server decryption module
 This module will spoof server publickey, read shared secret and spoof session on sessionserver.
 Then you will see decrypted packets.
@@ -143,15 +161,15 @@
 ```python
 proxy = MCRewriteProxy(("localhost", 25565), ("localhost", 25575), logging.INFO,
 	decryptor=decryptor_class)
 ```
 where decryptor_class is heir of `MCRP.ProtocolDecryptor` like `MCWPDecryptor` in md.py, oh yes you can import `MCWPDecryptor` from md.py and use it here too
 
 ## TODO
-- [ ] Rewrite networking with [ku](https://gitlab.com/seeklay/ku)
+- [x] Rewrite networking with [ku](https://gitlab.com/seeklay/ku)
 - [ ] еще ченить можно добавить =P
 
 ## Author
 **[seeklay](https://gitlab.com/seeklay)**
 
 ## License
 **[GNU GPL 3.0](LICENSE)**
```

## Comparing `MCRP-0.1.9.dist-info/RECORD` & `MCRP-0.2.0rc1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-MCRP/__init__.py,sha256=fUcvnFtsWtCv7i4lmZuPeOJQU4KVzc5pjFBTMEkYR0E,80
-MCRP/iautil.py,sha256=SdQwcfsYuSG4JFMR1NrfcVHDLZQF4WYmG1FpfI3ysbw,611
-MCRP/mcrp.py,sha256=E0xsn0-ycDLyQAjjiycOVOb5rblbVkRZaov8mkK1AKc,14614
-MCRP/mcwp.py,sha256=vbWBnHxV0TMbvQHde_fGbpUROT20tcs5cZ-z_BiHrOs,5931
-MCRP/tcproxy.py,sha256=-H3Z9gk5X-sofDfie1dXJjvY0LP4mpLXtYt3I0eXT_M,4157
-MCRP/util.py,sha256=QPWzVMO4ulHkSA9v3nPUqKfLecPa68uc03zz-rI-8MM,882
-MCRP-0.1.9.dist-info/LICENSE,sha256=5o3klq1LXYOQ7ZW15SETGFku4Z3oV9VOELnettdwfLU,35060
-MCRP-0.1.9.dist-info/METADATA,sha256=elZ6wjtk8is6chSrmydZXI3QyBqrpAFbPQWZyki9WfI,7314
-MCRP-0.1.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-MCRP-0.1.9.dist-info/entry_points.txt,sha256=8HjEjIsVMm6kdV9S1GqsjK9ICk_iAvrb3W6S2Zzfre4,41
-MCRP-0.1.9.dist-info/top_level.txt,sha256=kiBJB9iCobyqf3IxllWZAGupoBPqi7nHCNXQevMrEpc,5
-MCRP-0.1.9.dist-info/RECORD,,
+MCRP/__init__.py,sha256=Yn9PvA7g_DfLeeKYS_yobPsp-_hWKqE_-t1BbKHhYmw,103
+MCRP/dgi.py,sha256=-0qQGQKuK3hHdgM0ymfs00u6TwDuVH0T8zNbTECXKtc,6142
+MCRP/iautil.py,sha256=CsAYNfv6at2omdJTnKxzWmLJ0JdwTNVDnr24Jwr9vF8,1146
+MCRP/mcdj.py,sha256=9sf7KneAjFDIPxA8kVaJ_38hiWQSClkkq_jtY-a8K-8,1370
+MCRP/mcenc.py,sha256=G62tDqgzbw8ae9p5-UkG1v6Xd9NqhfhdoJ1yptgbZjc,1927
+MCRP/mcrp.py,sha256=H-Whk--WGTSyCeCVp8v9YGu-ZvHukrP8sv_v5K8Naos,4070
+MCRP/mcsession.py,sha256=OMQXAzO4_0_Xa19K_XWCCTK_nMx2dcsGrJKcKjOPoBc,12606
+MCRP/mcwp.py,sha256=veWMp4_SjWsB1D4950oyzHezNXXmB3lsiUWtEYw_FCo,8627
+MCRP/util.py,sha256=cMm2-bBJgn0OnGszRKdHnz-pg_sobEWR_K0FFdzPeB4,944
+MCRP-0.2.0rc1.dist-info/LICENSE,sha256=5o3klq1LXYOQ7ZW15SETGFku4Z3oV9VOELnettdwfLU,35060
+MCRP-0.2.0rc1.dist-info/METADATA,sha256=mptqlhWftGtw0cKj5nSTKD0Zf37vPHGmSfkCPyBbM2I,8286
+MCRP-0.2.0rc1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+MCRP-0.2.0rc1.dist-info/entry_points.txt,sha256=8HjEjIsVMm6kdV9S1GqsjK9ICk_iAvrb3W6S2Zzfre4,41
+MCRP-0.2.0rc1.dist-info/top_level.txt,sha256=kiBJB9iCobyqf3IxllWZAGupoBPqi7nHCNXQevMrEpc,5
+MCRP-0.2.0rc1.dist-info/RECORD,,
```

