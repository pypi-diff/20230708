# Comparing `tmp/serial_packets-0.1.8.tar.gz` & `tmp/serial_packets-0.1.9.tar.gz`

## Comparing `serial_packets-0.1.8.tar` & `serial_packets-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/client.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packet_decoder.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packet_encoder.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.8/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.8/LICENSE
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.8/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packet_decoder.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packet_encoder.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.9/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.9/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.9/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.9/PKG-INFO
```

### Comparing `serial_packets-0.1.8/src/serial_packets/_packets.py` & `serial_packets-0.1.9/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/src/serial_packets/client.py` & `serial_packets-0.1.9/src/serial_packets/client.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/src/serial_packets/packet_decoder.py` & `serial_packets-0.1.9/src/serial_packets/packet_decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 
     def __init__(self):
         # assert (decoded_packet_callback is not None)
         self.__crc_calc = CRCCCITT("FFFF")
         self.__packet_bfr = bytearray()
         self.__in_packet = False
         self.__pending_escape = False
-        # self.__decoded_packet_callback = decoded_packet_callback
+        # Used to filter warnings before first packet.
+        self.__encountered_start_flag = False
 
     def __str__(self):
         return f"In_packet ={self.__in_packet}, pending_escape={self.__pending_escape}, len={len(self.__packet_bytes)}"
 
     def __reset_packet(self, in_packet: bool):
         self.__in_packet = in_packet
         self.__pending_escape = False
@@ -79,18 +80,21 @@
                   | DecodedMessagePacket):
         """ Returns a decoded packet or None."""
         # If not already in a packet, wait for next flag.
         if not self.__in_packet:
             if b == PACKET_START_FLAG:
                 # Start collecting a packet.
                 self.__reset_packet(True)
+                self.__encountered_start_flag = True
             else:
                 # Here we drop bytes until next packet start. Should not
-                # happen in normal operation.
-                logger.error(f"Dropping byte {b:02x}")
+                # happen in normal operation, except when connecting to 
+                # and on going communication.
+                if self.__encountered_start_flag:
+                  logger.error(f"Dropping byte {b:02x}")
                 pass
             return None
 
         # Here collecting packet bytes.
         assert (self.__in_packet)
 
         if b == PACKET_START_FLAG:
@@ -148,23 +152,25 @@
     def __process_packet(self):
         """Returns a packet or None."""
         rx_bfr = self.__packet_bfr
 
         # Check for minimum length. A minimum we should
         # have a type byte and two CRC bytes.
         n = len(rx_bfr)
+        # logger.info(f"Packet candidate: len={n}")
+        # logger.info(f"Packet: {rx_bfr.hex(sep=' ')}")
         if n < MIN_PACKET_LEN:
             logger.error("Packet too short (%d), dropping", n)
             return None
 
         # Check CRC
         packet_crc = int.from_bytes(rx_bfr[-2:], byteorder='big', signed=False)
         computed_crc = self.__crc_calc.calculate(bytes(rx_bfr[:-2]))
         if computed_crc != packet_crc:
-            logger.error("Packet CRC error %04x vs %04x, dropping", packet_crc,
+            logger.error("Packet CRC error, packet: %04x vs computed: %04x, dropping", packet_crc,
                          computed_crc)
             return None
 
         # Construct decoded packet
         type_value = rx_bfr[0]
         if type_value == PacketType.COMMAND.value:
             cmd_id = int.from_bytes(rx_bfr[1:5], byteorder='big', signed=False)
@@ -189,12 +195,12 @@
             return None
 
         if data.size() > MAX_DATA_LEN:
             logger.error("Packet data too long (type=%d, len=%d), dropping",
                          type_value, data.size())
             return None
 
-        # Inform the user about the new packet.
-        # self.__decoded_packet_callback(decoded_packet)
+        # A new packet is available.
+        # logger.info("A packet is available.")
         return decoded_packet
 
         # self.__packets_queue.put_nowait(decoded_packet)
```

### Comparing `serial_packets-0.1.8/src/serial_packets/packet_encoder.py` & `serial_packets-0.1.9/src/serial_packets/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/src/serial_packets/packets.py` & `serial_packets-0.1.9/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/LICENSE` & `serial_packets-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/README.md` & `serial_packets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.8/pyproject.toml` & `serial_packets-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.8/PKG-INFO` & `serial_packets-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

