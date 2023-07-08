# Comparing `tmp/lantrane-0.0.4.tar.gz` & `tmp/lantrane-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantrane-0.0.4.tar", last modified: Fri Jul  7 23:19:49 2023, max compression
+gzip compressed data, was "lantrane-0.0.5.tar", last modified: Sat Jul  8 00:28:18 2023, max compression
```

## Comparing `lantrane-0.0.4.tar` & `lantrane-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 23:19:49.509068 lantrane-0.0.4/
--rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.4/LICENSE.md
--rw-rw-r--   0 ace       (1000) ace       (1000)     1430 2023-07-07 23:19:49.509068 lantrane-0.0.4/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      975 2023-07-07 23:19:10.000000 lantrane-0.0.4/README.md
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 23:19:49.509068 lantrane-0.0.4/lantrane/
--rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.4/lantrane/__init__.py
--rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-07 19:56:09.000000 lantrane-0.0.4/lantrane/data.py
--rw-rw-r--   0 ace       (1000) ace       (1000)      826 2023-07-07 22:19:22.000000 lantrane-0.0.4/lantrane/eventmanager.py
--rw-rw-r--   0 ace       (1000) ace       (1000)     1595 2023-07-07 22:20:24.000000 lantrane-0.0.4/lantrane/lantrane.py
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 23:19:49.509068 lantrane-0.0.4/lantrane.egg-info/
--rw-rw-r--   0 ace       (1000) ace       (1000)     1430 2023-07-07 23:19:49.000000 lantrane-0.0.4/lantrane.egg-info/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      241 2023-07-07 23:19:49.000000 lantrane-0.0.4/lantrane.egg-info/SOURCES.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-07 23:19:49.000000 lantrane-0.0.4/lantrane.egg-info/dependency_links.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-07 23:19:49.000000 lantrane-0.0.4/lantrane.egg-info/top_level.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-07 23:19:49.509068 lantrane-0.0.4/setup.cfg
--rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-07 23:17:03.000000 lantrane-0.0.4/setup.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-08 00:28:18.182883 lantrane-0.0.5/
+-rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.5/LICENSE.md
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1194 2023-07-08 00:28:18.182883 lantrane-0.0.5/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      739 2023-07-08 00:14:35.000000 lantrane-0.0.5/README.md
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-08 00:28:18.182883 lantrane-0.0.5/lantrane/
+-rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.5/lantrane/__init__.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-07 19:56:09.000000 lantrane-0.0.5/lantrane/data.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)      826 2023-07-07 22:19:22.000000 lantrane-0.0.5/lantrane/eventmanager.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1546 2023-07-08 00:13:50.000000 lantrane-0.0.5/lantrane/lantrane.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-08 00:28:18.182883 lantrane-0.0.5/lantrane.egg-info/
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1194 2023-07-08 00:28:18.000000 lantrane-0.0.5/lantrane.egg-info/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      241 2023-07-08 00:28:18.000000 lantrane-0.0.5/lantrane.egg-info/SOURCES.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-08 00:28:18.000000 lantrane-0.0.5/lantrane.egg-info/dependency_links.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-08 00:28:18.000000 lantrane-0.0.5/lantrane.egg-info/top_level.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-08 00:28:18.182883 lantrane-0.0.5/setup.cfg
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-08 00:27:56.000000 lantrane-0.0.5/setup.py
```

### Comparing `lantrane-0.0.4/LICENSE.md` & `lantrane-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.4/PKG-INFO` & `lantrane-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -21,27 +21,14 @@
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 import asyncio
 
-async def read_async():
-	async for data in Trane(args.ip, args.port).listen():
-	print(data)
-
-asyncio.run(read_async())
-```
-
-you can also subscribe to data using a callback (i think)
-
-```python
-from lantrane import Trane
-import asyncio
-
 trane = Trane(args.ip, args.port)
 
 def read(data):
 	print(data)
 
 trane.on_data(read)
```

### Comparing `lantrane-0.0.4/README.md` & `lantrane-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,14 @@
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 import asyncio
 
-async def read_async():
-	async for data in Trane(args.ip, args.port).listen():
-	print(data)
-
-asyncio.run(read_async())
-```
-
-you can also subscribe to data using a callback (i think)
-
-```python
-from lantrane import Trane
-import asyncio
-
 trane = Trane(args.ip, args.port)
 
 def read(data):
 	print(data)
 
 trane.on_data(read)
```

### Comparing `lantrane-0.0.4/lantrane/data.py` & `lantrane-0.0.5/lantrane/data.py`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.4/lantrane/eventmanager.py` & `lantrane-0.0.5/lantrane/eventmanager.py`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.4/lantrane/lantrane.py` & `lantrane-0.0.5/lantrane/lantrane.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,17 +41,15 @@
 		try:
 			while True:
 				data = await reader.read(bufsize)
 				if not data:
 					break
 				# strip newline and trailing null
 				data = data[:-2]
-				returnData = ThermostatData.from_data(data)
-				self.emit("incoming_data", returnData)
-				yield returnData
+				self.emit("incoming_data", ThermostatData.from_data(data))
 		except (TimeoutError, ConnectionAbortedError, ConnectionResetError) as e:
 			# sockets generally either time out, close, or reset.
 			# https://stackoverflow.com/a/15175067/
 			print("Connection Error")
 			print(e)
 		finally:
 			writer.close()
```

### Comparing `lantrane-0.0.4/lantrane.egg-info/PKG-INFO` & `lantrane-0.0.5/lantrane.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -21,27 +21,14 @@
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 import asyncio
 
-async def read_async():
-	async for data in Trane(args.ip, args.port).listen():
-	print(data)
-
-asyncio.run(read_async())
-```
-
-you can also subscribe to data using a callback (i think)
-
-```python
-from lantrane import Trane
-import asyncio
-
 trane = Trane(args.ip, args.port)
 
 def read(data):
 	print(data)
 
 trane.on_data(read)
```

### Comparing `lantrane-0.0.4/setup.py` & `lantrane-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=[],      								  # Dependencies
      python_requires='>=3',                                   # Minimum Python version
      name='lantrane',                                  # Package name
-     version="0.0.4",                                     # Version
+     version="0.0.5",                                     # Version
      author="Adrian Edwards",                                 # Author name
      author_email="adrian@adriancedwards.com",                           # Author mail
      description="Python package for interacting with Trane thermostats locally.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/MoralCode/lantrane",       # Url to your Git Repo
     #  download_url = 'https://github.com/MoralCode/lantrane/archive/'+new_version+'.tar.gz',
```

