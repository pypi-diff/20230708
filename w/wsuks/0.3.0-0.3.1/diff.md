# Comparing `tmp/wsuks-0.3.0.tar.gz` & `tmp/wsuks-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.3.0.tar", max compression
+gzip compressed data, was "wsuks-0.3.1.tar", max compression
```

## Comparing `wsuks-0.3.0.tar` & `wsuks-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.3.0/LICENSE
--rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.3.0/README.md
--rw-r--r--   0        0        0      507 2023-07-07 23:35:53.932318 wsuks-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.3.0/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.3.0/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.3.0/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.3.0/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.3.0/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.3.0/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.3.0/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3361 2023-07-07 23:08:04.680283 wsuks-0.3.0/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.3.0/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     3603 2023-07-07 23:34:44.580316 wsuks-0.3.0/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.3.0/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.3.0/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.3.0/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.3.0/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.3.0/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.3.0/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.3.0/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.3.0/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 wsuks-0.3.0/setup.py
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 wsuks-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.3.1/README.md
+-rw-r--r--   0        0        0      523 2023-07-08 10:37:14.955366 wsuks-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.3.1/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.3.1/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.3.1/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.3.1/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.3.1/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3306 2023-07-07 23:08:04.680283 wsuks-0.3.1/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     2628 2023-07-07 23:26:14.448306 wsuks-0.3.1/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     3361 2023-07-07 23:08:04.680283 wsuks-0.3.1/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10323 2023-07-07 23:20:30.360298 wsuks-0.3.1/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     3603 2023-07-07 23:34:44.580316 wsuks-0.3.1/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.3.1/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.3.1/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.3.1/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.3.1/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.3.1/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.3.1/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.3.1/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.3.1/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 wsuks-0.3.1/setup.py
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 wsuks-0.3.1/PKG-INFO
```

### Comparing `wsuks-0.3.0/LICENSE` & `wsuks-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/README.md` & `wsuks-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/executables/PsExec.exe` & `wsuks-0.3.1/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/executables/PsExec64.exe` & `wsuks-0.3.1/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/helpers/argparser.py` & `wsuks-0.3.1/wsuks/helpers/argparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/helpers/arpspoofer.py` & `wsuks-0.3.1/wsuks/helpers/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/helpers/logger.py` & `wsuks-0.3.1/wsuks/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/helpers/sysvolparser.py` & `wsuks-0.3.1/wsuks/helpers/sysvolparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/helpers/wsusserver.py` & `wsuks-0.3.1/wsuks/helpers/wsusserver.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/wsuks.py` & `wsuks-0.3.1/wsuks/wsuks.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.3.1/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/xml_files/get-config.xml` & `wsuks-0.3.1/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/xml_files/get-cookie.xml` & `wsuks-0.3.1/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.3.1/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/wsuks/xml_files/sync-updates.xml` & `wsuks-0.3.1/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.3.0/setup.py` & `wsuks-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
 package_data = \
 {'': ['*'], 'wsuks': ['executables/*', 'xml_files/*']}
 
 install_requires = \
 ['bs4>=0.0.1,<0.0.2',
  'impacket>=0.10.0,<0.11.0',
+ 'lxml>=4.9.3,<5.0.0',
  'scapy>=2.5.0,<3.0.0',
  'termcolor>=2.2.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wsuks = wsuks.wsuks:main']}
 
 setup_kwargs = {
     'name': 'wsuks',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A Tool for automating the MITM attack on the WSUS connection',
     'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nGaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.\nBy default, a Windows client requests updates every 24 hours. \n\nBoth the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.\n\nPrerequisits:\n- The target Client must be on the local network\n- The Windows Server Update Service (WSUS) must be configured using HTTP\n\nResult:\n- After successful execution a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created and added to the local admin group\n\n## Installation\nUsing pipx:\n```\nsudo apt install python3-pipx\npipx ensurepath\npipx install wsuks\nsudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nWith pipx:\n```\nsudo wsuks\nsuso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\nWith poetry:\n```\nsudo poetry run wsuks\nsudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
     'author': 'Alexander Neff',
     'author_email': 'alex99.neff@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wsuks-0.3.0/PKG-INFO` & `wsuks-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: wsuks
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Tool for automating the MITM attack on the WSUS connection
 License: MIT
 Author: Alexander Neff
 Author-email: alex99.neff@gmx.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: impacket (>=0.10.0,<0.11.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)
 # wsuks
 _Weaponizing the WSUS Attack_
```

