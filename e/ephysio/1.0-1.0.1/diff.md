# Comparing `tmp/ephysio-1.0.tar.gz` & `tmp/ephysio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysio-1.0.tar", last modified: Fri Jul  7 19:41:27 2023, max compression
+gzip compressed data, was "ephysio-1.0.1.tar", last modified: Fri Jul  7 23:10:54 2023, max compression
```

## Comparing `ephysio-1.0.tar` & `ephysio-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 19:41:27.371508 ephysio-1.0/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1401 2023-07-07 19:41:27.371508 ephysio-1.0/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 19:41:27.371508 ephysio-1.0/ephysio/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 19:41:15.000000 ephysio-1.0/ephysio/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12693 2023-01-11 21:50:43.000000 ephysio-1.0/ephysio/kilosortIO.py
--rw-------   0 wagenaar  (1000) wagenaar  (1000)    56917 2023-01-16 18:21:33.000000 ephysio-1.0/ephysio/openEphysIO.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17453 2023-01-11 21:50:43.000000 ephysio-1.0/ephysio/vizio.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 19:41:27.371508 ephysio-1.0/ephysio.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1401 2023-07-07 19:41:27.000000 ephysio-1.0/ephysio.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      268 2023-07-07 19:41:27.000000 ephysio-1.0/ephysio.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-07 19:41:27.000000 ephysio-1.0/ephysio.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       12 2023-07-07 19:41:27.000000 ephysio-1.0/ephysio.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-07 19:41:27.000000 ephysio-1.0/ephysio.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      303 2023-07-07 19:40:43.000000 ephysio-1.0/pyproject.toml
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-07 19:41:27.371508 ephysio-1.0/setup.cfg
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 23:10:54.699027 ephysio-1.0.1/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.1/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-07 23:10:54.699027 ephysio-1.0.1/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.1/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 23:10:54.699027 ephysio-1.0.1/ephysio/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.1/ephysio/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12693 2023-01-11 21:50:43.000000 ephysio-1.0.1/ephysio/kilosortIO.py
+-rw-------   0 wagenaar  (1000) wagenaar  (1000)    58530 2023-07-07 20:15:35.000000 ephysio-1.0.1/ephysio/openEphysIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17453 2023-01-11 21:50:43.000000 ephysio-1.0.1/ephysio/vizio.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-07 23:10:54.699027 ephysio-1.0.1/ephysio.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-07 23:10:54.000000 ephysio-1.0.1/ephysio.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      268 2023-07-07 23:10:54.000000 ephysio-1.0.1/ephysio.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-07 23:10:54.000000 ephysio-1.0.1/ephysio.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       12 2023-07-07 23:10:54.000000 ephysio-1.0.1/ephysio.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-07 23:10:54.000000 ephysio-1.0.1/ephysio.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      306 2023-07-07 23:10:42.000000 ephysio-1.0.1/pyproject.toml
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-07 23:10:54.699027 ephysio-1.0.1/setup.cfg
```

### Comparing `ephysio-1.0/LICENSE` & `ephysio-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysio-1.0/PKG-INFO` & `ephysio-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0
+Version: 1.0.1
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

### Comparing `ephysio-1.0/README.md` & `ephysio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ephysio-1.0/ephysio/kilosortIO.py` & `ephysio-1.0.1/ephysio/kilosortIO.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0/ephysio/openEphysIO.py` & `ephysio-1.0.1/ephysio/openEphysIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -966,14 +966,18 @@
         self._ss0 = {}  # node->expt->rec->stream
         self._barcodes = {}  # node->expt->rec->stream->(times, ids)
         self.cntlbarcodes = cntlbarcodes
         if not os.path.exists(root):
             raise ValueError(f"No data at {root}")
 
     def _oebin(self, node, expt, rec):
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         _populate(self._oebins, node, expt)
         if rec not in self._oebins[node][expt]:
             self._oebins[node][expt][rec] = loadoebin(self.root,
                                                       expt, rec, node)
         return self._oebins[node][expt][rec]
 
     def _oebinsection(self, expt, rec, stream, section='continuous', node=None):
@@ -1091,49 +1095,75 @@
 
     def nodes(self):
         '''NODES - List of recording nodes
         NODES() returns a simple list of recording nodes, or [None] for
         older versions of OpenEphys that did not keep track.'''
         return list(self.nodemap().keys())
 
-    def _recfolder(self, node, expt=1, rec=1):
+    def _firstexpt(self, node):
         fldr = self.root
         if node is not None:
             fldr += f"/{node}"
-        fldr += f"/experiment{expt}/recording{rec}"
+        xpts = [x for x in os.listdir(fldr) if x.startswith("experiment")]
+        if not xpts:
+            raise Exception("No experiments")
+        xpts.sort()
+        return int(xpts[0][10:])
+
+    def _firstrec(self, node, expt):
+        fldr = self.root
+        if node is not None:
+            fldr += f"/{node}"
+        fldr += f"/experiment{expt}"
+        recs = [x for x in os.listdir(fldr) if x.startswith("recording")]
+        if not recs:
+            raise Exception("No recordings")
+        recs.sort()
+        return int(recs[0][9:])
+    
+    def _recfolder(self, node, expt=None, rec=None):
+        fldr = self.root
+        if node is not None:
+            fldr += f"/{node}"
+        if expt is None:
+            expt = self._firstexpt(node)
+        fldr += f"/experiment{expt}"
+        if rec is None:
+            rec = self._firstrec(node, expt)
+        fldr += f"/recording{rec}"
         return fldr
 
-    def contfolder(self, stream, expt=1, rec=1, node=None):
+    def contfolder(self, stream, expt=None, rec=None, node=None):
         '''CONTFOLDER - Folder name where continuous data is stored
         p = CONTFOLDER(stream) returns the full path of the "continuous" folder for the given stream.
         Optional expt, rec, and node further specify.'''
         node = self._autonode(stream, node)
         return self._recfolder(node, expt, rec) + f"/continuous/{stream}"
 
-    def _contsamplestampfile(self, stream, expt=1, rec=1, node=None):
+    def _contsamplestampfile(self, stream, expt=None, rec=None, node=None):
         fldr = self.contfolder(stream, expt, rec, node)
         for fn in ["sample_numbers", "timestamps"]:
             if os.path.exists(f"{fldr}/{fn}.npy"):
                 return f"{fldr}/{fn}.npy"
         raise Exception(f"No sample stamp file found for {stream} {expt}:{rec}")
 
-    def _eventfolder(self, stream, expt=1, rec=1, node=None):
+    def _eventfolder(self, stream, expt=None, rec=None, node=None):
         node = self._autonode(stream, node)
         fldr = self._recfolder(node, expt, rec) + f"/events/{stream}"
         ttl = _quickglob(f"{fldr}/TTL*")
         return f"{fldr}/{ttl[0]}"
 
-    def _eventsamplestampfile(self, stream, expt=1, rec=1, node=None):
+    def _eventsamplestampfile(self, stream, expt=None, rec=None, node=None):
         fldr = self._eventfolder(stream, expt, rec, node)
         for fn in ["sample_numbers", "timestamps"]:
             if os.path.exists(f"{fldr}/{fn}.npy"):
                 return f"{fldr}/{fn}.npy"
         raise Exception(f"No sample stamp file found for {stream} {expt}:{rec}")
 
-    def _eventstatesfile(self, stream, expt=1, rec=1, node=None):
+    def _eventstatesfile(self, stream, expt=None, rec=None, node=None):
         fldr = self._eventfolder(stream, expt, rec, node)
         for fn in ["states", "channel_states"]:
             if os.path.exists(f"{fldr}/{fn}.npy"):
                 return f"{fldr}/{fn}.npy"
         raise Exception(f"No sample stamp file found for {stream} {expt}:{rec}")
 
     def nodemap(self):
@@ -1150,17 +1180,18 @@
             nodes = _quickglob(f"{self.root}/*")
             nodemap = {}
             if any([node.startswith("experiment") for node in nodes]):
                 # Old style without explicit nodes
                 nodemap[None] = explorenodes(None)
             else:
                 for node in nodes:
-                    probes = explorenodes(node)
-                    if len(probes):
-                        nodemap[node] = probes
+                    if os.path.exists(f"{self.root}/{node}/settings.xml"):
+                        probes = explorenodes(node)
+                        if len(probes):
+                            nodemap[node] = probes
             streammap = {}
             for node, streams in nodemap.items():
                 for stream in streams:
                     if stream not in streammap:
                         streammap[stream] = []
                     streammap[stream].append(node)
             self._nodemap = nodemap
@@ -1171,29 +1202,33 @@
         '''STREAMMAP - Map of stream names to recording nodes
         STREAMMAP() returns a dict mapping stream names to lists of
         recording names that contain that stream.'''
         if self._streammap is None:
             self.nodemap()
         return self._streammap
 
-    def samplingrate(self, stream, expt=1, rec=1, node=None):
+    def samplingrate(self, stream, expt=None, rec=None, node=None):
         '''SAMPLINGRATE - Sampling rate of a stream
         SIMPLINGRATE(stream), where STREAM is one of the items returned
         by STREAMS() or its friends, returns the sampling rate of that
         stream in Hertz. Optional experiments EXPT and REC specify the
         "experiment" and "recording", but those can usually be left out,
         as the sampling rate is generally consistent for a whole session.'''
         node = self._autonode(stream, node)
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         _populate(self._sfreqs, node, expt, rec)
         if stream not in self._sfreqs[node][expt][rec]:
             info = self._oebinsection(expt, rec, stream=stream, node=node)
             self._sfreqs[node][expt][rec][stream] = info['sample_rate']
         return self._sfreqs[node][expt][rec][stream]
 
-    def data(self, stream, expt=1, rec=1, node=None, stage='continuous'):
+    def data(self, stream, expt=None, rec=None, node=None, stage='continuous'):
         '''DATA - Data for a stream
         DATA(stream) returns the data for the first recording from the
         given stream as a TxC array. Optional arguments EXPT, REC, and
         NODE further specify.
         By default, the file "continuous.dat" is loaded. Use optional
         argument STAGE to specify an alternative. (E.g., stage='salpa'
         for "salpa.dat".)'''
@@ -1201,32 +1236,32 @@
         contfn += f"/{stage}.dat"
         mm = np.memmap(contfn, dtype=np.int16, mode='r')
         info = self._oebinsection(expt, rec, stream=stream, node=node)
         C = info['num_channels']
         T = len(mm) // C
         return np.reshape(mm, [T, C])
 
-    def bitvolts(self, stream, expt=1, rec=1, node=None):
+    def bitvolts(self, stream, expt=None, rec=None, node=None):
         '''BITVOLTS - Scale factor for all the channels for a data stream
         BITVOLTS(stream) returns the scale factors to convert DATA from
         binary scale to volts as a C-length array. Optional arguments EXPT, REC, and
         NODE further specify.'''
         info = self._oebinsection(expt, rec, stream=stream, node=node)
         return [ch['bit_volts'] for ch in info['channels']]
 
-    def channellist(self, stream, expt=1, rec=1, node=None):
+    def channellist(self, stream, expt=None, rec=None, node=None):
         '''CHANNELLIST - List of channels for a stream
         CHANNELLIST(stream) returns the list of channels for that stream.
         Each entry in the list is a dict with channel name and other
         information straight from the OEBIN file.
         Optional arguments EXPT, REC, and NODE further specify.'''
         info = self._oebinsection(expt, rec, stream=stream, node=node)
         return info['channels']
 
-    def events(self, stream, expt=1, rec=1, node=None):
+    def events(self, stream, expt=None, rec=None, node=None):
         '''EVENTS - Events for a stream
         EVENTS(stream) returns the events associated with the given
         stream as a dict of event channel numbers (typically counted 1
         to 8) to Nx2 arrays of on and off sample times, measured from
         the beginning of the recording, so that they can be used
         directly as indices into the corresponding DATA().
         Ab initio, only conventional digital events are returned, but
@@ -1262,36 +1297,45 @@
                 if np.any(np.diff(mydelta) == 0):
                     raise Exception("Event edges should alternate")
                 N = len(myss)
                 myss = myss.reshape(N // 2, 2)
                 self._events[node][expt][rec][stream][c] = myss
         return self._events[node][expt][rec][stream]
 
-    def analogevents(self, stream, channel="A0", expt=1, rec=1, node=None):
+    def analogevents(self, stream, channel="A0", expt=None, rec=None, node=None):
         '''ANALOGEVENTS - Return virtual events from analog channel
         ss = ANALOGEVENTS(stream, channel) treats the given channel (specified
         in string form, e.g., "A0", or "A1", etc.) as if it were a digital
         channel and returns an Nx2 array of on/off event time stamps.
         '''
+        node = self._autonode(stream, node)
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         self.events(stream, expt, rec, node)  # just to populate the dict
         if channel not in self._events[node][expt][rec][stream]:
             ss, cc, st = loadanalogevents(self.root, expt, rec, stream, node, int(channel[1:]))
             N = len(ss)
             self._events[node][expt][rec][stream][channel] = np.reshape(ss, (N // 2, 2))
         return self._events[node][expt][rec][stream]
 
-    def barcodes(self, stream, expt=1, rec=1, node=None, channel=1):
+    def barcodes(self, stream, expt=None, rec=None, node=None, channel=1):
         '''BARCODES - Extract bar codes from a given stream
         times, codes = BARCODES(stream) returns the time stamps and codes of the
         bar codes associated with the given stream. Optional arguments EXPT, REC,
         NODE further specify.
         Optional argument CHANNEL specifies the digital channel from which the
         bar codes are to be read. If CHANNEL is a string like "A0", the bar codes
         are read from the given analog channel.'''
         node = self._autonode(stream, node)
+        if expt is None:
+            expt = self._firstexpt(node)
+        if rec is None:
+            rec = self._firstrec(node, expt)
         _populate(self._barcodes, node, expt, rec)
         if stream not in self._barcodes[node][expt][rec]:
             if type(channel) == str:
                 self.analogevents(stream, channel, expt, rec, node)
             evts = self.events(stream, expt, rec, node)[channel]
             fs = self.samplingrate(stream, expt, rec, node)
             ss_on = evts[:, 0]
@@ -1305,15 +1349,15 @@
             if self.cntlbarcodes:
                 tt, vv = _cntlbarcodes(sss, uds)
             else:
                 tt, vv = _openephysbarcodes(sss, uds, fs)
             self._barcodes[node][expt][rec][stream] = (tt, vv)
         return self._barcodes[node][expt][rec][stream]
 
-    def shifttime(self, times, sourcestream, deststream, expt=1, rec=1,
+    def shifttime(self, times, sourcestream, deststream, expt=None, rec=None,
                   sourcenode=None, destnode=None,
                   sourcebarcode=1, destbarcode=1):
         '''SHIFTTIME - Translate event time stamps to other stream
         SHIFTTIME(times, source, dest) translates event time stamps
         defined relative to the SOURCE stream for use as indices in
         the DEST stream. Operates on the first experiment/recording
         unless EXPT and REC are specified.
@@ -1346,15 +1390,16 @@
         if len(isafter):
             print(f"Caution: Extrapolation {len(isafter)} event(s) after end of bar codes")
             a_after, b_after = np.polyfit(ss1[-2:], ss2[-2:], 1)
             result[isafter] = a_after * result[isafter] + b_after
 
         return result
 
-    def translatedata(self, data, t0, sourcestream, deststream, expt=1, rec=1,
+    def translatedata(self, data, t0, sourcestream, deststream,
+                      expt=None, rec=None,
                       sourcenode=None, destnode=None,
                       sourcebarcode=1, destbarcode=1):
         '''TRANSLATEDATA - Translate a chunk of data from one timezone to another.
         datad, t0d = TRANSLATEDATA(data, t0, source, dest) takes a chunk of data (vector of
         arbitrary length N) that lives in the timezone of the SOURCE stream with time stamps
         T0 up to T1 = T0+N, and reinterpolates it to the timezone of the DEST stream. The
         function figures out the translations of T0 and T1 in the DEST stream. We call those T0D
@@ -1375,15 +1420,15 @@
         # Note backward translation
         tts = self.shifttime(ttd, deststream, sourcestream, expt, rec,
                              destnode, sourcenode, destbarcode, sourcebarcode)
         # Interpolate the data
         datad = np.interp(tts, np.arange(t0, t1), data)
         return datad, t0d
 
-    def nidaqevents(self, stream, expt=1, rec=1, node=None,
+    def nidaqevents(self, stream, expt=None, rec=None, node=None,
                     nidaqstream=None, nidaqbarcode=1, destbarcode=1,
                     glitch_ms=None):
         '''NIDAQEVENTS - NIDAQ events translated to given stream
         NIDAQEVENTS is a convenience function that first calls EVENTS
         on the NIDAQ stream, then SHIFTTIME to convert those events
         to the time base of the given STREAM.
         NIDAQBARCODE and DESTBARCODE are the digital (or analog)
```

### Comparing `ephysio-1.0/ephysio/vizio.py` & `ephysio-1.0.1/ephysio/vizio.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0/ephysio.egg-info/PKG-INFO` & `ephysio-1.0.1/ephysio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0
+Version: 1.0.1
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

