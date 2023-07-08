# Comparing `tmp/telnetlib3-2.0.2.tar.gz` & `tmp/telnetlib3-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/telnetlib3-2.0.2.tar", last modified: Fri Mar 31 17:50:36 2023, max compression
+gzip compressed data, was "telnetlib3-2.0.3.tar", last modified: Sat Jul  8 15:08:13 2023, max compression
```

## Comparing `telnetlib3-2.0.2.tar` & `telnetlib3-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/
--rw-r--r--   0 jq         (501) staff       (20)      169 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/.coveragerc
--rw-r--r--   0 jq         (501) staff       (20)     2343 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/LICENSE.txt
--rw-r--r--   0 jq         (501) staff       (20)       38 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/MANIFEST.in
--rw-r--r--   0 jq         (501) staff       (20)     8435 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/PKG-INFO
--rw-r--r--   0 jq         (501) staff       (20)     6146 2023-03-28 16:48:37.000000 telnetlib3-2.0.2/README.rst
-drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/docs/
--rw-r--r--   0 jq         (501) staff       (20)       58 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/docs/api.rst
--rw-r--r--   0 jq         (501) staff       (20)     2058 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/docs/contributing.rst
--rw-r--r--   0 jq         (501) staff       (20)     3631 2023-03-31 17:49:32.000000 telnetlib3-2.0.2/docs/history.rst
--rw-r--r--   0 jq         (501) staff       (20)      259 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/docs/index.rst
--rw-r--r--   0 jq         (501) staff       (20)     6146 2023-03-28 16:48:37.000000 telnetlib3-2.0.2/docs/intro.rst
--rw-r--r--   0 jq         (501) staff       (20)     6729 2020-07-03 00:14:03.000000 telnetlib3-2.0.2/docs/rfcs.rst
--rw-r--r--   0 jq         (501) staff       (20)       49 2022-11-28 21:50:53.000000 telnetlib3-2.0.2/requirements-analysis.txt
--rw-r--r--   0 jq         (501) staff       (20)       86 2022-11-28 22:32:25.000000 telnetlib3-2.0.2/requirements-docs.txt
--rw-r--r--   0 jq         (501) staff       (20)       84 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/requirements-tests.txt
--rw-r--r--   0 jq         (501) staff       (20)      179 2022-11-29 16:16:26.000000 telnetlib3-2.0.2/requirements.txt
--rw-r--r--   0 jq         (501) staff       (20)       38 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/setup.cfg
--rw-r--r--   0 jq         (501) staff       (20)     1943 2023-03-31 17:49:35.000000 telnetlib3-2.0.2/setup.py
-drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3/
--rw-r--r--   0 jq         (501) staff       (20)      990 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/__init__.py
--rw-r--r--   0 jq         (501) staff       (20)     2756 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/accessories.py
--rwxr-xr-x   0 jq         (501) staff       (20)    16453 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/client.py
--rw-r--r--   0 jq         (501) staff       (20)    12293 2023-03-20 18:26:59.000000 telnetlib3-2.0.2/telnetlib3/client_base.py
--rw-r--r--   0 jq         (501) staff       (20)     9360 2023-03-20 18:26:17.000000 telnetlib3-2.0.2/telnetlib3/client_shell.py
--rw-r--r--   0 jq         (501) staff       (20)     3091 2022-11-28 21:50:53.000000 telnetlib3-2.0.2/telnetlib3/relay_server.py
--rwxr-xr-x   0 jq         (501) staff       (20)    22716 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/server.py
--rw-r--r--   0 jq         (501) staff       (20)    11981 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/server_base.py
--rw-r--r--   0 jq         (501) staff       (20)     6625 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/server_shell.py
--rw-r--r--   0 jq         (501) staff       (20)    14936 2022-01-30 19:27:08.000000 telnetlib3-2.0.2/telnetlib3/slc.py
--rw-r--r--   0 jq         (501) staff       (20)    21191 2023-03-28 22:26:35.000000 telnetlib3-2.0.2/telnetlib3/stream_reader.py
--rw-r--r--   0 jq         (501) staff       (20)   103507 2023-03-31 17:48:21.000000 telnetlib3-2.0.2/telnetlib3/stream_writer.py
--rw-r--r--   0 jq         (501) staff       (20)     5348 2023-03-28 16:48:37.000000 telnetlib3-2.0.2/telnetlib3/telopt.py
-drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/
--rw-r--r--   0 jq         (501) staff       (20)     8435 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/PKG-INFO
--rw-r--r--   0 jq         (501) staff       (20)      760 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/SOURCES.txt
--rw-r--r--   0 jq         (501) staff       (20)        1 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/dependency_links.txt
--rw-r--r--   0 jq         (501) staff       (20)      105 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/entry_points.txt
--rw-r--r--   0 jq         (501) staff       (20)       11 2023-03-31 17:50:36.000000 telnetlib3-2.0.2/telnetlib3.egg-info/top_level.txt
--rw-r--r--   0 jq         (501) staff       (20)        1 2020-07-03 00:14:32.000000 telnetlib3-2.0.2/telnetlib3.egg-info/zip-safe
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-07-08 15:08:13.956769 telnetlib3-2.0.3/
+-rw-r--r--   0 jq         (501) staff       (20)      169 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/.coveragerc
+-rw-r--r--   0 jq         (501) staff       (20)     2343 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/LICENSE.txt
+-rw-r--r--   0 jq         (501) staff       (20)       38 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/MANIFEST.in
+-rw-r--r--   0 jq         (501) staff       (20)     7064 2023-07-08 15:08:13.956638 telnetlib3-2.0.3/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)     6146 2023-03-28 16:48:37.000000 telnetlib3-2.0.3/README.rst
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-07-08 15:08:13.952051 telnetlib3-2.0.3/docs/
+-rw-r--r--   0 jq         (501) staff       (20)       58 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/docs/api.rst
+-rw-r--r--   0 jq         (501) staff       (20)     2058 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/docs/contributing.rst
+-rw-r--r--   0 jq         (501) staff       (20)     3711 2023-07-08 15:06:29.000000 telnetlib3-2.0.3/docs/history.rst
+-rw-r--r--   0 jq         (501) staff       (20)      259 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/docs/index.rst
+-rw-r--r--   0 jq         (501) staff       (20)     6146 2023-03-28 16:48:37.000000 telnetlib3-2.0.3/docs/intro.rst
+-rw-r--r--   0 jq         (501) staff       (20)     6729 2020-07-03 00:14:03.000000 telnetlib3-2.0.3/docs/rfcs.rst
+-rw-r--r--   0 jq         (501) staff       (20)       49 2022-11-28 21:50:53.000000 telnetlib3-2.0.3/requirements-analysis.txt
+-rw-r--r--   0 jq         (501) staff       (20)       86 2022-11-28 22:32:25.000000 telnetlib3-2.0.3/requirements-docs.txt
+-rw-r--r--   0 jq         (501) staff       (20)       84 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/requirements-tests.txt
+-rw-r--r--   0 jq         (501) staff       (20)      179 2022-11-29 16:16:26.000000 telnetlib3-2.0.3/requirements.txt
+-rw-r--r--   0 jq         (501) staff       (20)       38 2023-07-08 15:08:13.956805 telnetlib3-2.0.3/setup.cfg
+-rw-r--r--   0 jq         (501) staff       (20)     1943 2023-07-08 15:06:42.000000 telnetlib3-2.0.3/setup.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-07-08 15:08:13.955595 telnetlib3-2.0.3/telnetlib3/
+-rw-r--r--   0 jq         (501) staff       (20)      990 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/telnetlib3/__init__.py
+-rw-r--r--   0 jq         (501) staff       (20)     2756 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/telnetlib3/accessories.py
+-rwxr-xr-x   0 jq         (501) staff       (20)    16453 2023-07-08 15:03:26.000000 telnetlib3-2.0.3/telnetlib3/client.py
+-rw-r--r--   0 jq         (501) staff       (20)    12293 2023-03-20 18:26:59.000000 telnetlib3-2.0.3/telnetlib3/client_base.py
+-rw-r--r--   0 jq         (501) staff       (20)     9360 2023-03-20 18:26:17.000000 telnetlib3-2.0.3/telnetlib3/client_shell.py
+-rw-r--r--   0 jq         (501) staff       (20)     3091 2022-11-28 21:50:53.000000 telnetlib3-2.0.3/telnetlib3/relay_server.py
+-rwxr-xr-x   0 jq         (501) staff       (20)    22716 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/telnetlib3/server.py
+-rw-r--r--   0 jq         (501) staff       (20)    11981 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/telnetlib3/server_base.py
+-rw-r--r--   0 jq         (501) staff       (20)     6625 2023-03-28 22:26:35.000000 telnetlib3-2.0.3/telnetlib3/server_shell.py
+-rw-r--r--   0 jq         (501) staff       (20)    14974 2023-07-08 15:04:07.000000 telnetlib3-2.0.3/telnetlib3/slc.py
+-rw-r--r--   0 jq         (501) staff       (20)    21202 2023-07-08 15:04:04.000000 telnetlib3-2.0.3/telnetlib3/stream_reader.py
+-rw-r--r--   0 jq         (501) staff       (20)   103507 2023-03-31 17:48:21.000000 telnetlib3-2.0.3/telnetlib3/stream_writer.py
+-rw-r--r--   0 jq         (501) staff       (20)     5348 2023-03-28 16:48:37.000000 telnetlib3-2.0.3/telnetlib3/telopt.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-07-08 15:08:13.956373 telnetlib3-2.0.3/telnetlib3.egg-info/
+-rw-r--r--   0 jq         (501) staff       (20)     7064 2023-07-08 15:08:13.000000 telnetlib3-2.0.3/telnetlib3.egg-info/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)      760 2023-07-08 15:08:13.000000 telnetlib3-2.0.3/telnetlib3.egg-info/SOURCES.txt
+-rw-r--r--   0 jq         (501) staff       (20)        1 2023-07-08 15:08:13.000000 telnetlib3-2.0.3/telnetlib3.egg-info/dependency_links.txt
+-rw-r--r--   0 jq         (501) staff       (20)      104 2023-07-08 15:08:13.000000 telnetlib3-2.0.3/telnetlib3.egg-info/entry_points.txt
+-rw-r--r--   0 jq         (501) staff       (20)       11 2023-07-08 15:08:13.000000 telnetlib3-2.0.3/telnetlib3.egg-info/top_level.txt
+-rw-r--r--   0 jq         (501) staff       (20)        1 2020-07-03 00:14:32.000000 telnetlib3-2.0.3/telnetlib3.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `telnetlib3-2.0.2/LICENSE.txt` & `telnetlib3-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/PKG-INFO` & `telnetlib3-2.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: telnetlib3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python 3 asyncio Telnet server and client Protocol library
 Home-page: http://telnetlib3.rtfd.org/
 Author: Jeff Quast
 Author-email: contact@jeffquast.com
 License: ISC
-Description: .. image:: https://coveralls.io/repos/jquast/telnetlib3/badge.svg?branch=master&service=github
-            :alt: Coveralls Code Coverage
-            :target: https://coveralls.io/github/jquast/telnetlib3?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/telnetlib3.svg
-            :alt: Latest Version
-            :target: https://pypi.python.org/pypi/telnetlib3
-        
-        .. image:: https://img.shields.io/pypi/dm/telnetlib3.svg
-            :alt: Downloads
-            :target: https://pypi.python.org/pypi/telnetlib3
-        
-        
-        Introduction
-        ============
-        
-        telnetlib3 is a Telnet Client and Server library for python.  This project
-        requires python 3.7 and later, using the asyncio_ module.
-        
-        .. _asyncio: http://docs.python.org/3.11/library/asyncio.html
-        
-        Quick Example
-        -------------
-        
-        Authoring a Telnet Server using Streams interface that offers a basic war game:
-        
-        .. code-block:: python
-        
-            import asyncio, telnetlib3
-        
-            async def shell(reader, writer):
-                writer.write('\r\nWould you like to play a game? ')
-                inp = await reader.read(1)
-                if inp:
-                    writer.echo(inp)
-                    writer.write('\r\nThey say the only way to win '
-                                 'is to not play at all.\r\n')
-                    await writer.drain()
-                writer.close()
-        
-            loop = asyncio.get_event_loop()
-            coro = telnetlib3.create_server(port=6023, shell=shell)
-            server = loop.run_until_complete(coro)
-            loop.run_until_complete(server.wait_closed())
-        
-        Authoring a Telnet Client that plays the war game with this server:
-        
-        .. code-block:: python
-        
-            import asyncio, telnetlib3
-        
-            async def shell(reader, writer):
-                while True:
-                    # read stream until '?' mark is found
-                    outp = await reader.read(1024)
-                    if not outp:
-                        # End of File
-                        break
-                    elif '?' in outp:
-                        # reply all questions with 'y'.
-                        writer.write('y')
-        
-                    # display all server output
-                    print(outp, flush=True)
-        
-                # EOF
-                print()
-        
-            loop = asyncio.get_event_loop()
-            coro = telnetlib3.open_connection('localhost', 6023, shell=shell)
-            reader, writer = loop.run_until_complete(coro)
-            loop.run_until_complete(writer.protocol.waiter_closed)
-        
-        Command-line
-        ------------
-        
-        Two command-line scripts are distributed with this package.
-        
-        ``telnetlib3-client``
-        
-          Small terminal telnet client.  Some example destinations and options::
-        
-            telnetlib3-client nethack.alt.org
-            telnetlib3-client --encoding=cp437 --force-binary blackflag.acid.org
-            telnetlib3-client htc.zapto.org
-        
-        
-        ``telnetlib3-server``
-        
-          Telnet server providing the default debugging shell.  This provides a simple
-          shell server that allows introspection of the session's values, for example::
-        
-             tel:sh> help
-             quit, writer, slc, toggle [option|all], reader, proto
-        
-             tel:sh> writer
-             <TelnetWriter server mode:kludge +lineflow -xon_any +slc_sim server-will:BINARY,ECHO,SGA client-will:BINARY,NAWS,NEW_ENVIRON,TTYPE>
-        
-             tel:sh> reader
-             <TelnetReaderUnicode encoding='utf8' limit=65536 buflen=0 eof=False>
-        
-             tel:sh> toggle all
-             wont echo.
-             wont suppress go-ahead.
-             wont outbinary.
-             dont inbinary.
-             xon-any enabled.
-             lineflow disabled.
-        
-             tel:sh> reader
-             <TelnetReaderUnicode encoding='US-ASCII' limit=65536 buflen=1 eof=False>
-        
-             tel:sh> writer
-             <TelnetWriter server mode:local -lineflow +xon_any +slc_sim client-will:NAWS,NEW_ENVIRON,TTYPE>
-        
-        
-        Both command-line scripts accept argument ``--shell=my_module.fn_shell``
-        describing a python module path to a coroutine of signature
-        ``shell(reader, writer)``, just as the above examples.
-        
-        Features
-        --------
-        
-        The following RFC specifications are implemented:
-        
-        * `rfc-727`_, "Telnet Logout Option," Apr 1977.
-        * `rfc-779`_, "Telnet Send-Location Option", Apr 1981.
-        * `rfc-854`_, "Telnet Protocol Specification", May 1983.
-        * `rfc-855`_, "Telnet Option Specifications", May 1983.
-        * `rfc-856`_, "Telnet Binary Transmission", May 1983.
-        * `rfc-857`_, "Telnet Echo Option", May 1983.
-        * `rfc-858`_, "Telnet Suppress Go Ahead Option", May 1983.
-        * `rfc-859`_, "Telnet Status Option", May 1983.
-        * `rfc-860`_, "Telnet Timing mark Option", May 1983.
-        * `rfc-885`_, "Telnet End of Record Option", Dec 1983.
-        * `rfc-1073`_, "Telnet Window Size Option", Oct 1988.
-        * `rfc-1079`_, "Telnet Terminal Speed Option", Dec 1988.
-        * `rfc-1091`_, "Telnet Terminal-Type Option", Feb 1989.
-        * `rfc-1096`_, "Telnet X Display Location Option", Mar 1989.
-        * `rfc-1123`_, "Requirements for Internet Hosts", Oct 1989.
-        * `rfc-1184`_, "Telnet Linemode Option (extended options)", Oct 1990.
-        * `rfc-1372`_, "Telnet Remote Flow Control Option", Oct 1992.
-        * `rfc-1408`_, "Telnet Environment Option", Jan 1993.
-        * `rfc-1571`_, "Telnet Environment Option Interoperability Issues", Jan 1994.
-        * `rfc-1572`_, "Telnet Environment Option", Jan 1994.
-        * `rfc-2066`_, "Telnet Charset Option", Jan 1997.
-        
-        .. _rfc-727: https://www.rfc-editor.org/rfc/rfc727.txt
-        .. _rfc-779: https://www.rfc-editor.org/rfc/rfc779.txt
-        .. _rfc-854: https://www.rfc-editor.org/rfc/rfc854.txt
-        .. _rfc-855: https://www.rfc-editor.org/rfc/rfc855.txt
-        .. _rfc-856: https://www.rfc-editor.org/rfc/rfc856.txt
-        .. _rfc-857: https://www.rfc-editor.org/rfc/rfc857.txt
-        .. _rfc-858: https://www.rfc-editor.org/rfc/rfc858.txt
-        .. _rfc-859: https://www.rfc-editor.org/rfc/rfc859.txt
-        .. _rfc-860: https://www.rfc-editor.org/rfc/rfc860.txt
-        .. _rfc-885: https://www.rfc-editor.org/rfc/rfc885.txt
-        .. _rfc-1073: https://www.rfc-editor.org/rfc/rfc1073.txt
-        .. _rfc-1079: https://www.rfc-editor.org/rfc/rfc1079.txt
-        .. _rfc-1091: https://www.rfc-editor.org/rfc/rfc1091.txt
-        .. _rfc-1096: https://www.rfc-editor.org/rfc/rfc1096.txt
-        .. _rfc-1123: https://www.rfc-editor.org/rfc/rfc1123.txt
-        .. _rfc-1184: https://www.rfc-editor.org/rfc/rfc1184.txt
-        .. _rfc-1372: https://www.rfc-editor.org/rfc/rfc1372.txt
-        .. _rfc-1408: https://www.rfc-editor.org/rfc/rfc1408.txt
-        .. _rfc-1571: https://www.rfc-editor.org/rfc/rfc1571.txt
-        .. _rfc-1572: https://www.rfc-editor.org/rfc/rfc1572.txt
-        .. _rfc-2066: https://www.rfc-editor.org/rfc/rfc2066.txt
-        
-        Further Reading
-        ---------------
-        
-        Further documentation available at https://telnetlib3.readthedocs.org/
-        
 Keywords: telnet,server,client,bbs,mud,utf8,cp437,api,library,asyncio,talker
 Platform: any
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -191,7 +17,182 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Terminals :: Telnet
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+
+.. image:: https://coveralls.io/repos/jquast/telnetlib3/badge.svg?branch=master&service=github
+    :alt: Coveralls Code Coverage
+    :target: https://coveralls.io/github/jquast/telnetlib3?branch=master
+
+.. image:: https://img.shields.io/pypi/v/telnetlib3.svg
+    :alt: Latest Version
+    :target: https://pypi.python.org/pypi/telnetlib3
+
+.. image:: https://img.shields.io/pypi/dm/telnetlib3.svg
+    :alt: Downloads
+    :target: https://pypi.python.org/pypi/telnetlib3
+
+
+Introduction
+============
+
+telnetlib3 is a Telnet Client and Server library for python.  This project
+requires python 3.7 and later, using the asyncio_ module.
+
+.. _asyncio: http://docs.python.org/3.11/library/asyncio.html
+
+Quick Example
+-------------
+
+Authoring a Telnet Server using Streams interface that offers a basic war game:
+
+.. code-block:: python
+
+    import asyncio, telnetlib3
+
+    async def shell(reader, writer):
+        writer.write('\r\nWould you like to play a game? ')
+        inp = await reader.read(1)
+        if inp:
+            writer.echo(inp)
+            writer.write('\r\nThey say the only way to win '
+                         'is to not play at all.\r\n')
+            await writer.drain()
+        writer.close()
+
+    loop = asyncio.get_event_loop()
+    coro = telnetlib3.create_server(port=6023, shell=shell)
+    server = loop.run_until_complete(coro)
+    loop.run_until_complete(server.wait_closed())
+
+Authoring a Telnet Client that plays the war game with this server:
+
+.. code-block:: python
+
+    import asyncio, telnetlib3
+
+    async def shell(reader, writer):
+        while True:
+            # read stream until '?' mark is found
+            outp = await reader.read(1024)
+            if not outp:
+                # End of File
+                break
+            elif '?' in outp:
+                # reply all questions with 'y'.
+                writer.write('y')
+
+            # display all server output
+            print(outp, flush=True)
+
+        # EOF
+        print()
+
+    loop = asyncio.get_event_loop()
+    coro = telnetlib3.open_connection('localhost', 6023, shell=shell)
+    reader, writer = loop.run_until_complete(coro)
+    loop.run_until_complete(writer.protocol.waiter_closed)
+
+Command-line
+------------
+
+Two command-line scripts are distributed with this package.
+
+``telnetlib3-client``
+
+  Small terminal telnet client.  Some example destinations and options::
+
+    telnetlib3-client nethack.alt.org
+    telnetlib3-client --encoding=cp437 --force-binary blackflag.acid.org
+    telnetlib3-client htc.zapto.org
+
+
+``telnetlib3-server``
+
+  Telnet server providing the default debugging shell.  This provides a simple
+  shell server that allows introspection of the session's values, for example::
+
+     tel:sh> help
+     quit, writer, slc, toggle [option|all], reader, proto
+
+     tel:sh> writer
+     <TelnetWriter server mode:kludge +lineflow -xon_any +slc_sim server-will:BINARY,ECHO,SGA client-will:BINARY,NAWS,NEW_ENVIRON,TTYPE>
+
+     tel:sh> reader
+     <TelnetReaderUnicode encoding='utf8' limit=65536 buflen=0 eof=False>
+
+     tel:sh> toggle all
+     wont echo.
+     wont suppress go-ahead.
+     wont outbinary.
+     dont inbinary.
+     xon-any enabled.
+     lineflow disabled.
+
+     tel:sh> reader
+     <TelnetReaderUnicode encoding='US-ASCII' limit=65536 buflen=1 eof=False>
+
+     tel:sh> writer
+     <TelnetWriter server mode:local -lineflow +xon_any +slc_sim client-will:NAWS,NEW_ENVIRON,TTYPE>
+
+
+Both command-line scripts accept argument ``--shell=my_module.fn_shell``
+describing a python module path to a coroutine of signature
+``shell(reader, writer)``, just as the above examples.
+
+Features
+--------
+
+The following RFC specifications are implemented:
+
+* `rfc-727`_, "Telnet Logout Option," Apr 1977.
+* `rfc-779`_, "Telnet Send-Location Option", Apr 1981.
+* `rfc-854`_, "Telnet Protocol Specification", May 1983.
+* `rfc-855`_, "Telnet Option Specifications", May 1983.
+* `rfc-856`_, "Telnet Binary Transmission", May 1983.
+* `rfc-857`_, "Telnet Echo Option", May 1983.
+* `rfc-858`_, "Telnet Suppress Go Ahead Option", May 1983.
+* `rfc-859`_, "Telnet Status Option", May 1983.
+* `rfc-860`_, "Telnet Timing mark Option", May 1983.
+* `rfc-885`_, "Telnet End of Record Option", Dec 1983.
+* `rfc-1073`_, "Telnet Window Size Option", Oct 1988.
+* `rfc-1079`_, "Telnet Terminal Speed Option", Dec 1988.
+* `rfc-1091`_, "Telnet Terminal-Type Option", Feb 1989.
+* `rfc-1096`_, "Telnet X Display Location Option", Mar 1989.
+* `rfc-1123`_, "Requirements for Internet Hosts", Oct 1989.
+* `rfc-1184`_, "Telnet Linemode Option (extended options)", Oct 1990.
+* `rfc-1372`_, "Telnet Remote Flow Control Option", Oct 1992.
+* `rfc-1408`_, "Telnet Environment Option", Jan 1993.
+* `rfc-1571`_, "Telnet Environment Option Interoperability Issues", Jan 1994.
+* `rfc-1572`_, "Telnet Environment Option", Jan 1994.
+* `rfc-2066`_, "Telnet Charset Option", Jan 1997.
+
+.. _rfc-727: https://www.rfc-editor.org/rfc/rfc727.txt
+.. _rfc-779: https://www.rfc-editor.org/rfc/rfc779.txt
+.. _rfc-854: https://www.rfc-editor.org/rfc/rfc854.txt
+.. _rfc-855: https://www.rfc-editor.org/rfc/rfc855.txt
+.. _rfc-856: https://www.rfc-editor.org/rfc/rfc856.txt
+.. _rfc-857: https://www.rfc-editor.org/rfc/rfc857.txt
+.. _rfc-858: https://www.rfc-editor.org/rfc/rfc858.txt
+.. _rfc-859: https://www.rfc-editor.org/rfc/rfc859.txt
+.. _rfc-860: https://www.rfc-editor.org/rfc/rfc860.txt
+.. _rfc-885: https://www.rfc-editor.org/rfc/rfc885.txt
+.. _rfc-1073: https://www.rfc-editor.org/rfc/rfc1073.txt
+.. _rfc-1079: https://www.rfc-editor.org/rfc/rfc1079.txt
+.. _rfc-1091: https://www.rfc-editor.org/rfc/rfc1091.txt
+.. _rfc-1096: https://www.rfc-editor.org/rfc/rfc1096.txt
+.. _rfc-1123: https://www.rfc-editor.org/rfc/rfc1123.txt
+.. _rfc-1184: https://www.rfc-editor.org/rfc/rfc1184.txt
+.. _rfc-1372: https://www.rfc-editor.org/rfc/rfc1372.txt
+.. _rfc-1408: https://www.rfc-editor.org/rfc/rfc1408.txt
+.. _rfc-1571: https://www.rfc-editor.org/rfc/rfc1571.txt
+.. _rfc-1572: https://www.rfc-editor.org/rfc/rfc1572.txt
+.. _rfc-2066: https://www.rfc-editor.org/rfc/rfc2066.txt
+
+Further Reading
+---------------
+
+Further documentation available at https://telnetlib3.readthedocs.org/
```

### Comparing `telnetlib3-2.0.2/README.rst` & `telnetlib3-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/docs/contributing.rst` & `telnetlib3-2.0.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/docs/history.rst` & `telnetlib3-2.0.3/docs/history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 History
 =======
+2.0.3
+ * bugfix: NameError: when debug=True is with asyncio.run, :ghissue:`75`
+
 2.0.2
  * bugfix: NameError: name 'sleep' is not defined in stream_writer.py
 
 2.0.1
  * bugfix: "write after close" is disregarded, caused many errors logged in socket.send()
  * bugfix: in accessories.repr_mapping() about using shlex.quote on non-str,
    `TypeError: expected string or bytes-like object, got 'int'`
```

### Comparing `telnetlib3-2.0.2/docs/intro.rst` & `telnetlib3-2.0.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/docs/rfcs.rst` & `telnetlib3-2.0.3/docs/rfcs.rst`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/setup.py` & `telnetlib3-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def _get_long_description(fname, encoding="utf8"):
     return open(fname, "r", encoding=encoding).read()
 
 
 setup(
     name="telnetlib3",
     # keep in sync w/docs/conf.py manually for now, please!
-    version="2.0.2",
+    version="2.0.3",
     url="http://telnetlib3.rtfd.org/",
     license="ISC",
     author="Jeff Quast",
     description="Python 3 asyncio Telnet server and client Protocol library",
     long_description=_get_long_description(fname=_get_here("README.rst")),
     # requires python 3.7 and greater beginning with 2.0.0 release
     python_requires=">=3.7",
```

### Comparing `telnetlib3-2.0.2/telnetlib3/__init__.py` & `telnetlib3-2.0.3/telnetlib3/__init__.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/accessories.py` & `telnetlib3-2.0.3/telnetlib3/accessories.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/client.py` & `telnetlib3-2.0.3/telnetlib3/client.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/client_base.py` & `telnetlib3-2.0.3/telnetlib3/client_base.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/client_shell.py` & `telnetlib3-2.0.3/telnetlib3/client_shell.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/relay_server.py` & `telnetlib3-2.0.3/telnetlib3/relay_server.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/server.py` & `telnetlib3-2.0.3/telnetlib3/server.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/server_base.py` & `telnetlib3-2.0.3/telnetlib3/server_base.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/server_shell.py` & `telnetlib3-2.0.3/telnetlib3/server_shell.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/slc.py` & `telnetlib3-2.0.3/telnetlib3/slc.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,18 +230,20 @@
     # no default value for break, sync, end-of-record,
     SLC_BRK: SLC(),
     SLC_SYNCH: SLC(),
     SLC_EOR: SLC(),
 }
 
 
-def generate_slctab(tabset=BSD_SLC_TAB):
+def generate_slctab(tabset=None):
     """Returns full 'SLC Tab' for definitions found using ``tabset``.
     Functions not listed in ``tabset`` are set as SLC_NOSUPPORT.
     """
+    if tabset is None:
+        tabset = BSD_SLC_TAB
     #   ``slctab`` is a dictionary of SLC functions, such as SLC_IP,
     #   to a tuple of the handling character and support level.
     _slctab = {}
     for slc in [bytes([const]) for const in range(1, NSLC + 1)]:
         _slctab[slc] = tabset.get(slc, SLC_nosupport())
     return _slctab
 
@@ -249,16 +251,16 @@
 def generate_forwardmask(binary_mode, tabset, ack=False):
     """
     Generate a :class:`~.Forwardmask` instance.
 
     Generate a 32-byte (``binary_mode`` is True) or 16-byte (False) Forwardmask
     instance appropriate for the specified ``slctab``.  A Forwardmask is formed
     by a bitmask of all 256 possible 8-bit keyboard ascii input, or, when not
-    'outbinary', a 16-byte 7-bit representation of each value, and whether or
-    not they should be "forwarded" by the client on the transport stream
+    'outbinary', a 16-byte 7-bit representation of each value, and whether
+    they should be "forwarded" by the client on the transport stream
     """
     num_bytes, msb = (32, 256) if binary_mode else (16, 127)
     mask32 = [theNULL] * num_bytes
     for mask in range(msb // 8):
         start = mask * 8
         last = start + 7
         byte = theNULL
```

### Comparing `telnetlib3-2.0.2/telnetlib3/stream_reader.py` & `telnetlib3-2.0.3/telnetlib3/stream_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module provides class TelnetReader and TelnetReaderUnicode."""
 # std imports
+import sys
 import codecs
 import asyncio
 import logging
 import warnings
 import asyncio
 
 from asyncio import events
```

### Comparing `telnetlib3-2.0.2/telnetlib3/stream_writer.py` & `telnetlib3-2.0.3/telnetlib3/stream_writer.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3/telopt.py` & `telnetlib3-2.0.3/telnetlib3/telopt.py`

 * *Files identical despite different names*

### Comparing `telnetlib3-2.0.2/telnetlib3.egg-info/PKG-INFO` & `telnetlib3-2.0.3/telnetlib3.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: telnetlib3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python 3 asyncio Telnet server and client Protocol library
 Home-page: http://telnetlib3.rtfd.org/
 Author: Jeff Quast
 Author-email: contact@jeffquast.com
 License: ISC
-Description: .. image:: https://coveralls.io/repos/jquast/telnetlib3/badge.svg?branch=master&service=github
-            :alt: Coveralls Code Coverage
-            :target: https://coveralls.io/github/jquast/telnetlib3?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/telnetlib3.svg
-            :alt: Latest Version
-            :target: https://pypi.python.org/pypi/telnetlib3
-        
-        .. image:: https://img.shields.io/pypi/dm/telnetlib3.svg
-            :alt: Downloads
-            :target: https://pypi.python.org/pypi/telnetlib3
-        
-        
-        Introduction
-        ============
-        
-        telnetlib3 is a Telnet Client and Server library for python.  This project
-        requires python 3.7 and later, using the asyncio_ module.
-        
-        .. _asyncio: http://docs.python.org/3.11/library/asyncio.html
-        
-        Quick Example
-        -------------
-        
-        Authoring a Telnet Server using Streams interface that offers a basic war game:
-        
-        .. code-block:: python
-        
-            import asyncio, telnetlib3
-        
-            async def shell(reader, writer):
-                writer.write('\r\nWould you like to play a game? ')
-                inp = await reader.read(1)
-                if inp:
-                    writer.echo(inp)
-                    writer.write('\r\nThey say the only way to win '
-                                 'is to not play at all.\r\n')
-                    await writer.drain()
-                writer.close()
-        
-            loop = asyncio.get_event_loop()
-            coro = telnetlib3.create_server(port=6023, shell=shell)
-            server = loop.run_until_complete(coro)
-            loop.run_until_complete(server.wait_closed())
-        
-        Authoring a Telnet Client that plays the war game with this server:
-        
-        .. code-block:: python
-        
-            import asyncio, telnetlib3
-        
-            async def shell(reader, writer):
-                while True:
-                    # read stream until '?' mark is found
-                    outp = await reader.read(1024)
-                    if not outp:
-                        # End of File
-                        break
-                    elif '?' in outp:
-                        # reply all questions with 'y'.
-                        writer.write('y')
-        
-                    # display all server output
-                    print(outp, flush=True)
-        
-                # EOF
-                print()
-        
-            loop = asyncio.get_event_loop()
-            coro = telnetlib3.open_connection('localhost', 6023, shell=shell)
-            reader, writer = loop.run_until_complete(coro)
-            loop.run_until_complete(writer.protocol.waiter_closed)
-        
-        Command-line
-        ------------
-        
-        Two command-line scripts are distributed with this package.
-        
-        ``telnetlib3-client``
-        
-          Small terminal telnet client.  Some example destinations and options::
-        
-            telnetlib3-client nethack.alt.org
-            telnetlib3-client --encoding=cp437 --force-binary blackflag.acid.org
-            telnetlib3-client htc.zapto.org
-        
-        
-        ``telnetlib3-server``
-        
-          Telnet server providing the default debugging shell.  This provides a simple
-          shell server that allows introspection of the session's values, for example::
-        
-             tel:sh> help
-             quit, writer, slc, toggle [option|all], reader, proto
-        
-             tel:sh> writer
-             <TelnetWriter server mode:kludge +lineflow -xon_any +slc_sim server-will:BINARY,ECHO,SGA client-will:BINARY,NAWS,NEW_ENVIRON,TTYPE>
-        
-             tel:sh> reader
-             <TelnetReaderUnicode encoding='utf8' limit=65536 buflen=0 eof=False>
-        
-             tel:sh> toggle all
-             wont echo.
-             wont suppress go-ahead.
-             wont outbinary.
-             dont inbinary.
-             xon-any enabled.
-             lineflow disabled.
-        
-             tel:sh> reader
-             <TelnetReaderUnicode encoding='US-ASCII' limit=65536 buflen=1 eof=False>
-        
-             tel:sh> writer
-             <TelnetWriter server mode:local -lineflow +xon_any +slc_sim client-will:NAWS,NEW_ENVIRON,TTYPE>
-        
-        
-        Both command-line scripts accept argument ``--shell=my_module.fn_shell``
-        describing a python module path to a coroutine of signature
-        ``shell(reader, writer)``, just as the above examples.
-        
-        Features
-        --------
-        
-        The following RFC specifications are implemented:
-        
-        * `rfc-727`_, "Telnet Logout Option," Apr 1977.
-        * `rfc-779`_, "Telnet Send-Location Option", Apr 1981.
-        * `rfc-854`_, "Telnet Protocol Specification", May 1983.
-        * `rfc-855`_, "Telnet Option Specifications", May 1983.
-        * `rfc-856`_, "Telnet Binary Transmission", May 1983.
-        * `rfc-857`_, "Telnet Echo Option", May 1983.
-        * `rfc-858`_, "Telnet Suppress Go Ahead Option", May 1983.
-        * `rfc-859`_, "Telnet Status Option", May 1983.
-        * `rfc-860`_, "Telnet Timing mark Option", May 1983.
-        * `rfc-885`_, "Telnet End of Record Option", Dec 1983.
-        * `rfc-1073`_, "Telnet Window Size Option", Oct 1988.
-        * `rfc-1079`_, "Telnet Terminal Speed Option", Dec 1988.
-        * `rfc-1091`_, "Telnet Terminal-Type Option", Feb 1989.
-        * `rfc-1096`_, "Telnet X Display Location Option", Mar 1989.
-        * `rfc-1123`_, "Requirements for Internet Hosts", Oct 1989.
-        * `rfc-1184`_, "Telnet Linemode Option (extended options)", Oct 1990.
-        * `rfc-1372`_, "Telnet Remote Flow Control Option", Oct 1992.
-        * `rfc-1408`_, "Telnet Environment Option", Jan 1993.
-        * `rfc-1571`_, "Telnet Environment Option Interoperability Issues", Jan 1994.
-        * `rfc-1572`_, "Telnet Environment Option", Jan 1994.
-        * `rfc-2066`_, "Telnet Charset Option", Jan 1997.
-        
-        .. _rfc-727: https://www.rfc-editor.org/rfc/rfc727.txt
-        .. _rfc-779: https://www.rfc-editor.org/rfc/rfc779.txt
-        .. _rfc-854: https://www.rfc-editor.org/rfc/rfc854.txt
-        .. _rfc-855: https://www.rfc-editor.org/rfc/rfc855.txt
-        .. _rfc-856: https://www.rfc-editor.org/rfc/rfc856.txt
-        .. _rfc-857: https://www.rfc-editor.org/rfc/rfc857.txt
-        .. _rfc-858: https://www.rfc-editor.org/rfc/rfc858.txt
-        .. _rfc-859: https://www.rfc-editor.org/rfc/rfc859.txt
-        .. _rfc-860: https://www.rfc-editor.org/rfc/rfc860.txt
-        .. _rfc-885: https://www.rfc-editor.org/rfc/rfc885.txt
-        .. _rfc-1073: https://www.rfc-editor.org/rfc/rfc1073.txt
-        .. _rfc-1079: https://www.rfc-editor.org/rfc/rfc1079.txt
-        .. _rfc-1091: https://www.rfc-editor.org/rfc/rfc1091.txt
-        .. _rfc-1096: https://www.rfc-editor.org/rfc/rfc1096.txt
-        .. _rfc-1123: https://www.rfc-editor.org/rfc/rfc1123.txt
-        .. _rfc-1184: https://www.rfc-editor.org/rfc/rfc1184.txt
-        .. _rfc-1372: https://www.rfc-editor.org/rfc/rfc1372.txt
-        .. _rfc-1408: https://www.rfc-editor.org/rfc/rfc1408.txt
-        .. _rfc-1571: https://www.rfc-editor.org/rfc/rfc1571.txt
-        .. _rfc-1572: https://www.rfc-editor.org/rfc/rfc1572.txt
-        .. _rfc-2066: https://www.rfc-editor.org/rfc/rfc2066.txt
-        
-        Further Reading
-        ---------------
-        
-        Further documentation available at https://telnetlib3.readthedocs.org/
-        
 Keywords: telnet,server,client,bbs,mud,utf8,cp437,api,library,asyncio,talker
 Platform: any
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -191,7 +17,182 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Terminals :: Telnet
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+
+.. image:: https://coveralls.io/repos/jquast/telnetlib3/badge.svg?branch=master&service=github
+    :alt: Coveralls Code Coverage
+    :target: https://coveralls.io/github/jquast/telnetlib3?branch=master
+
+.. image:: https://img.shields.io/pypi/v/telnetlib3.svg
+    :alt: Latest Version
+    :target: https://pypi.python.org/pypi/telnetlib3
+
+.. image:: https://img.shields.io/pypi/dm/telnetlib3.svg
+    :alt: Downloads
+    :target: https://pypi.python.org/pypi/telnetlib3
+
+
+Introduction
+============
+
+telnetlib3 is a Telnet Client and Server library for python.  This project
+requires python 3.7 and later, using the asyncio_ module.
+
+.. _asyncio: http://docs.python.org/3.11/library/asyncio.html
+
+Quick Example
+-------------
+
+Authoring a Telnet Server using Streams interface that offers a basic war game:
+
+.. code-block:: python
+
+    import asyncio, telnetlib3
+
+    async def shell(reader, writer):
+        writer.write('\r\nWould you like to play a game? ')
+        inp = await reader.read(1)
+        if inp:
+            writer.echo(inp)
+            writer.write('\r\nThey say the only way to win '
+                         'is to not play at all.\r\n')
+            await writer.drain()
+        writer.close()
+
+    loop = asyncio.get_event_loop()
+    coro = telnetlib3.create_server(port=6023, shell=shell)
+    server = loop.run_until_complete(coro)
+    loop.run_until_complete(server.wait_closed())
+
+Authoring a Telnet Client that plays the war game with this server:
+
+.. code-block:: python
+
+    import asyncio, telnetlib3
+
+    async def shell(reader, writer):
+        while True:
+            # read stream until '?' mark is found
+            outp = await reader.read(1024)
+            if not outp:
+                # End of File
+                break
+            elif '?' in outp:
+                # reply all questions with 'y'.
+                writer.write('y')
+
+            # display all server output
+            print(outp, flush=True)
+
+        # EOF
+        print()
+
+    loop = asyncio.get_event_loop()
+    coro = telnetlib3.open_connection('localhost', 6023, shell=shell)
+    reader, writer = loop.run_until_complete(coro)
+    loop.run_until_complete(writer.protocol.waiter_closed)
+
+Command-line
+------------
+
+Two command-line scripts are distributed with this package.
+
+``telnetlib3-client``
+
+  Small terminal telnet client.  Some example destinations and options::
+
+    telnetlib3-client nethack.alt.org
+    telnetlib3-client --encoding=cp437 --force-binary blackflag.acid.org
+    telnetlib3-client htc.zapto.org
+
+
+``telnetlib3-server``
+
+  Telnet server providing the default debugging shell.  This provides a simple
+  shell server that allows introspection of the session's values, for example::
+
+     tel:sh> help
+     quit, writer, slc, toggle [option|all], reader, proto
+
+     tel:sh> writer
+     <TelnetWriter server mode:kludge +lineflow -xon_any +slc_sim server-will:BINARY,ECHO,SGA client-will:BINARY,NAWS,NEW_ENVIRON,TTYPE>
+
+     tel:sh> reader
+     <TelnetReaderUnicode encoding='utf8' limit=65536 buflen=0 eof=False>
+
+     tel:sh> toggle all
+     wont echo.
+     wont suppress go-ahead.
+     wont outbinary.
+     dont inbinary.
+     xon-any enabled.
+     lineflow disabled.
+
+     tel:sh> reader
+     <TelnetReaderUnicode encoding='US-ASCII' limit=65536 buflen=1 eof=False>
+
+     tel:sh> writer
+     <TelnetWriter server mode:local -lineflow +xon_any +slc_sim client-will:NAWS,NEW_ENVIRON,TTYPE>
+
+
+Both command-line scripts accept argument ``--shell=my_module.fn_shell``
+describing a python module path to a coroutine of signature
+``shell(reader, writer)``, just as the above examples.
+
+Features
+--------
+
+The following RFC specifications are implemented:
+
+* `rfc-727`_, "Telnet Logout Option," Apr 1977.
+* `rfc-779`_, "Telnet Send-Location Option", Apr 1981.
+* `rfc-854`_, "Telnet Protocol Specification", May 1983.
+* `rfc-855`_, "Telnet Option Specifications", May 1983.
+* `rfc-856`_, "Telnet Binary Transmission", May 1983.
+* `rfc-857`_, "Telnet Echo Option", May 1983.
+* `rfc-858`_, "Telnet Suppress Go Ahead Option", May 1983.
+* `rfc-859`_, "Telnet Status Option", May 1983.
+* `rfc-860`_, "Telnet Timing mark Option", May 1983.
+* `rfc-885`_, "Telnet End of Record Option", Dec 1983.
+* `rfc-1073`_, "Telnet Window Size Option", Oct 1988.
+* `rfc-1079`_, "Telnet Terminal Speed Option", Dec 1988.
+* `rfc-1091`_, "Telnet Terminal-Type Option", Feb 1989.
+* `rfc-1096`_, "Telnet X Display Location Option", Mar 1989.
+* `rfc-1123`_, "Requirements for Internet Hosts", Oct 1989.
+* `rfc-1184`_, "Telnet Linemode Option (extended options)", Oct 1990.
+* `rfc-1372`_, "Telnet Remote Flow Control Option", Oct 1992.
+* `rfc-1408`_, "Telnet Environment Option", Jan 1993.
+* `rfc-1571`_, "Telnet Environment Option Interoperability Issues", Jan 1994.
+* `rfc-1572`_, "Telnet Environment Option", Jan 1994.
+* `rfc-2066`_, "Telnet Charset Option", Jan 1997.
+
+.. _rfc-727: https://www.rfc-editor.org/rfc/rfc727.txt
+.. _rfc-779: https://www.rfc-editor.org/rfc/rfc779.txt
+.. _rfc-854: https://www.rfc-editor.org/rfc/rfc854.txt
+.. _rfc-855: https://www.rfc-editor.org/rfc/rfc855.txt
+.. _rfc-856: https://www.rfc-editor.org/rfc/rfc856.txt
+.. _rfc-857: https://www.rfc-editor.org/rfc/rfc857.txt
+.. _rfc-858: https://www.rfc-editor.org/rfc/rfc858.txt
+.. _rfc-859: https://www.rfc-editor.org/rfc/rfc859.txt
+.. _rfc-860: https://www.rfc-editor.org/rfc/rfc860.txt
+.. _rfc-885: https://www.rfc-editor.org/rfc/rfc885.txt
+.. _rfc-1073: https://www.rfc-editor.org/rfc/rfc1073.txt
+.. _rfc-1079: https://www.rfc-editor.org/rfc/rfc1079.txt
+.. _rfc-1091: https://www.rfc-editor.org/rfc/rfc1091.txt
+.. _rfc-1096: https://www.rfc-editor.org/rfc/rfc1096.txt
+.. _rfc-1123: https://www.rfc-editor.org/rfc/rfc1123.txt
+.. _rfc-1184: https://www.rfc-editor.org/rfc/rfc1184.txt
+.. _rfc-1372: https://www.rfc-editor.org/rfc/rfc1372.txt
+.. _rfc-1408: https://www.rfc-editor.org/rfc/rfc1408.txt
+.. _rfc-1571: https://www.rfc-editor.org/rfc/rfc1571.txt
+.. _rfc-1572: https://www.rfc-editor.org/rfc/rfc1572.txt
+.. _rfc-2066: https://www.rfc-editor.org/rfc/rfc2066.txt
+
+Further Reading
+---------------
+
+Further documentation available at https://telnetlib3.readthedocs.org/
```

### Comparing `telnetlib3-2.0.2/telnetlib3.egg-info/SOURCES.txt` & `telnetlib3-2.0.3/telnetlib3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

