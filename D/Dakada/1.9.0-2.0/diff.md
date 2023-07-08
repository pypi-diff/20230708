# Comparing `tmp/Dakada-1.9.0.tar.gz` & `tmp/Dakada-2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dakada-1.9.0.tar", last modified: Fri Jun 23 08:01:05 2023, max compression
+gzip compressed data, was "dist\Dakada-2.0.tar", last modified: Sat Jul  8 03:11:43 2023, max compression
```

## Comparing `Dakada-1.9.0.tar` & `Dakada-2.0-py3-none-any.whl.zip-content`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/
-drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/Dakada.egg-info/
--rw-rw-rw-   0        0        0      678 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      678 2023-06-23 08:01:05.000000 Dakada-1.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/dakada/
--rw-rw-rw-   0        0        0     9005 2023-06-23 01:50:45.000000 Dakada-1.9.0/dakada/Dakada.py
--rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-1.9.0/dakada/User.py
--rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-1.9.0/dakada/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-1.9.0/dakada/admin.py
--rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-1.9.0/dakada/cookie.py
--rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-1.9.0/dakada/render.py
--rw-rw-rw-   0        0        0      256 2023-06-23 01:46:12.000000 Dakada-1.9.0/dakada/startproject.py
--rw-rw-rw-   0        0        0       42 2023-06-23 08:01:05.000000 Dakada-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     3821 2023-06-23 01:51:10.000000 Dakada-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:11:43.000000 Dakada-2.0/
+drwxrwxrwx   0        0        0        0 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:11:43.000000 Dakada-2.0/Dakada.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      646 2023-07-08 03:11:43.000000 Dakada-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8226 2023-07-08 03:10:59.000000 Dakada-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 03:11:43.000000 Dakada-2.0/dakada/
+-rw-rw-rw-   0        0        0    11086 2023-07-08 03:09:03.000000 Dakada-2.0/dakada/Dakada.py
+-rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-2.0/dakada/User.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-2.0/dakada/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-2.0/dakada/admin.py
+-rw-rw-rw-   0        0        0      119 2023-07-08 02:24:49.000000 Dakada-2.0/dakada/blueprint.py
+-rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-2.0/dakada/cookie.py
+-rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-2.0/dakada/render.py
+-rw-rw-rw-   0        0        0      256 2023-07-08 02:24:11.000000 Dakada-2.0/dakada/startproject.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:11:43.000000 Dakada-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3828 2023-07-08 03:11:21.000000 Dakada-2.0/setup.py
```

### Comparing `Dakada-1.9.0/Dakada.egg-info/PKG-INFO` & `Dakada-2.0/Dakada.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.9.0
+Version: 2.0
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
-Description: A web framework by Dakada CN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+A web framework by Dakada CN
```

### Comparing `Dakada-1.9.0/PKG-INFO` & `Dakada-2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.9.0
+Version: 2.0
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
-Description: A web framework by Dakada CN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+A web framework by Dakada CN
```

### Comparing `Dakada-1.9.0/dakada/Dakada.py` & `Dakada-2.0/dakada/Dakada.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from wsgiref.simple_server import make_server
 import os
 import re
 import json
 import datetime
 import threading
+import random
+
 html3=''
+tmp=[]
 def cookie():
     while True:
         with open(".\\cookies.txt","r",encoding="UTF-8") as f2:
             newlist2=[]
             for i in f2.readlines():
                 nowtime=datetime.datetime.now()
                 every_cookie=eval(i.split("\n")[0])
@@ -32,40 +35,42 @@
     req_json=None
     try:
         req_body = env['wsgi.input'].read(int(env['CONTENT_LENGTH']))
         req_json = json.loads(req_body)
     except:
         pass
     HTTPdict["req_json"]=req_json
+    HTTPdict["QUERY_STRING"]=env["QUERY_STRING"]
     return HTTPdict
 def load_staic(link="."):
     link+="\\staic"        
     list1=[]
     for staicname in os.listdir(link):
         global staic_header
         staic_header="text/plain"
         with open(link+"\\"+staicname, "r", encoding="UTF8") as f:
             houzhui=staicname.split(".")[-1]
             if houzhui=="js":
-                staic_header="application/x-javascript"
+                staic_header="application/x-javascript;charset=utf-8"
             elif houzhui=="css":
-                staic_header="text/css"
+                staic_header="text/css;charset=utf-8"
+            elif houzhui=="html":
+                staic_header="text/html;charset=utf-8"
             try:
                 list1.append(("/"+staicname,f.read(),staic_header,"text"))
             except UnicodeDecodeError:
                 f.close()
                 with open(link+"\\"+staicname,"rb") as f:
                     staic_header="application/octet-stream"
                     houzhui=staicname.split(".")[-1]
                     if houzhui=="ico":
                         staic_header="application/x-ico"
                     elif houzhui=="icon":
                         staic_header="application/x-icon"
-                    list1.append(("/"+staicname,f.read(),staic_header,"byte"))
-            
+                    list1.append(("/"+staicname,f.read(),staic_header,"byte"))          
     return list1
 def errorhandle(status,status2,start_response,env):
     global err
     global url
     try:
         start_response(status2, [('Content-Type', 'text/html;charset=utf-8')])
     except:
@@ -75,34 +80,58 @@
     HTTP_req_dict=makedict(env)
     return str(err(status))
 def app(environ,start_response):
     global html3
     global url
     global staic
     try:
-        global staic
+        global tmp
+        global staic  #???
         for url1 in url:
             if url1[0]==environ['PATH_INFO'] or (url1[4]=="RE" and not re.match(url1[0],environ['PATH_INFO'])==None):
                 if environ['REQUEST_METHOD'] in url1[2]:
                     start_response('200 OK', url1[3])
                     match=None
                     if url1[0]==environ['PATH_INFO']:
                         pass
                     else:
                         match=re.findall(url1[0],environ['PATH_INFO'])
                     HTTP_req_dict= makedict(environ,match)
-                    return [str(url1[1](HTTP_req_dict)).encode()]
+                    if not url1[5]=="websocket":
+                        return [str(url1[1](HTTP_req_dict)).encode()]
+                    else:
+                        global Htmlcode
+                        name=random.randint(1,999999)
+                        global tmp
+                        newtmp=[eve for eve in tmp if not eve[0]=="/"+str(name)]
+                        tmp=list(newtmp)
+                        tname="/"+str(name)
+                        tmp.append(tname)
+                        print("==========================")
+                        print("Websocket is running at:%s"%(tname))
+                        print("==========================")
+                        code="""<script>var recv=0;function send(msg,fuc){var xmlhttp;if (window.XMLHttpRequest){xmlhttp=new XMLHttpRequest();}else{xmlhttp=new ActiveXObject("Microsoft.XMLHTTP");}xmlhttp.onreadystatechange=function(){fuc(xmlhttp.status,JSON.parse(xmlhttp.responseText).msg)};xmlhttp.open("POST","%s",true);xmlhttp.setRequestHeader("Content-Type", "application/json;charset=UTF-8");xmlhttp.send(JSON.stringify({"msg":msg}));}</script>"""%(tname)+str(url1[1](HTTP_req_dict))
+                        return [code.encode()]
                 else:
                     return [str(errorhandle("405","405 Method Not Allowed",start_response,environ)).encode()]
         for staicdata in staic:
             if staicdata[0]==environ['PATH_INFO']:
                 start_response('200 OK', [("Content-Type",staicdata[2])])
                 if staicdata[3]=="byte":
                     return [staicdata[1]]
                 return [staicdata[1].encode()]
+        for tmphtml in tmp:
+            if tmphtml==environ['PATH_INFO']:
+                start_response('200 OK', [("Content-Type","application/json;chatset=utf-8")])
+                try:
+                    msg=makedict(environ,None)["req_json"]["msg"]
+                    ret=str(json.dumps({"msg":webs(msg)}))
+                except Exception as e:
+                    ret=str(json.dumps({"msg":{"err":str(e)}}))
+                return [ret.encode()]
         return [errorhandle("404","404 Not Found",start_response,environ).encode()]
     except Exception as e:
         print("==========================")
         print("Found a bug!")
         with open(".\\debug.txt", "a", encoding="UTF8") as f:
             if os.path.getsize(".\\debug.txt"):
                 f.write("\n")
@@ -110,55 +139,61 @@
             f.write("\n")
             f.write(str(e))
             f.write("\n")
             f.write("==========================")
         print("see .\\debug.txt for more information")
         print("==========================")
         return [errorhandle("500","500 Internal Server Error",start_response,environ).encode()]
+   
 
 class _Dakada:
     def __init__(self,link=".",host='',port=8000):
         self.link=link
         self.host=host
         self.port=port
         self.url1=[]
         self.err1=0
+        self.websocket=0
         return 
-    def addpath(self,path,URL_type="URL",method=['GET'],req_header=[('Content-Type', 'text/html;charset=utf-8')]):
+    def addpath(self,path,URL_type="URL",method=['GET'],req_header=[('Content-Type', 'text/html;charset=utf-8')],mode="staic"):
         def returnfuc(fuc):
-            self.url1.append((path,fuc,method,req_header,URL_type))
+            self.url1.append((path,fuc,method,req_header,URL_type,mode))
         return returnfuc
     def run(self):
         try:
             global url
             global err
             global p_link
             global staic
+            global webs
             err=self.err1
             url=self.url1
             p_link=self.link
+            webs=self.websocket
             print("making server...")
             staic=load_staic(p_link)
             http=make_server(str(self.host),self.port,app)
             print("OK")
             print("starting cookiehandler...")
             t=threading.Thread(target=cookie)
             t.setDaemon(True)
             t.start()
             print("OK")
-            print("Dakada(ver 1.9.0) is running!")
+            print("Dakada(ver 2.0) is running!")
             if self.host=='':
                 print("View at:http://localhost:"+str(self.port))
             else:
                 print("View at:http://"+self.host+":"+str(self.port))
             http.serve_forever()
         except KeyboardInterrupt:
             print("server exit")
     def seterr(self,fuc):
         self.err1=fuc
+    def register_blueprint(self,blueprint):
+        self.url1+=blueprint.url1
     class db:
         def __init__(self,link=".",cookie=False):
             self.link=link
             self.dangerstr=["\n"]
             if not cookie:
                 self.link+="\\db"
         def adddangerstr(self,dangerlist):
@@ -220,9 +255,11 @@
                 except:
                     pass
             with open(self.link+"\\"+dblink,"w", encoding="UTF8") as f:
                 f.writelines(newlist)
         def clear(self,dblink):
             with open(self.link+"\\"+dblink,"w", encoding="UTF8") as f:
                 f.writelines([])
+    def newwebsocket(self,fuc):
+        self.websocket=fuc
 import sys
 sys.modules[__name__]=_Dakada
```

### Comparing `Dakada-1.9.0/dakada/User.py` & `Dakada-2.0/dakada/User.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.9.0/dakada/admin.py` & `Dakada-2.0/dakada/admin.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.9.0/dakada/cookie.py` & `Dakada-2.0/dakada/cookie.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.9.0/setup.py` & `Dakada-2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'Dakada'
 DESCRIPTION = 'A web framework by Dakada CN'
 URL = 'https://github.com/dakadayyds/dakadaWeb'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.9.0'
+VERSION = '2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'jinja2'
 ]
 
 # What packages are optional?
@@ -30,15 +30,15 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+    with io.open(".\\dakada\\README.md", encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
@@ -73,19 +73,19 @@
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
+        os.system('python -m twine upload dist/*')
 
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        # self.status('Pushing git tags…')
+        # os.system('git tag v{0}'.format(about['__version__']))
+        # os.system('git push --tags')
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
@@ -103,15 +103,15 @@
     #   'User'
     #   'admin'
     #    'cookie'
     #   'render'
     #],
 
      entry_points={
-         'console_scripts': ['startproject=dakada:startproject'],
+         # 'console_scripts': ['startproject=dakada:startproject'],
      },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
```

