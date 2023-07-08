# Comparing `tmp/Ruster-2.0.0.tar.gz` & `tmp/Ruster-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-2.0.0.tar", last modified: Fri Jul  7 17:26:26 2023, max compression
+gzip compressed data, was "Ruster-2.0.1.tar", last modified: Sat Jul  8 21:03:04 2023, max compression
```

## Comparing `Ruster-2.0.0.tar` & `Ruster-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.566744 Ruster-2.0.0/
--rw-rw-rw-   0        0        0      904 2023-07-07 17:26:26.566744 Ruster-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.454893 Ruster-2.0.0/Ruster/
--rw-rw-rw-   0        0        0       20 2023-07-07 17:25:59.000000 Ruster-2.0.0/Ruster/__init__.py
--rw-rw-rw-   0        0        0    13111 2023-07-07 17:25:53.000000 Ruster-2.0.0/Ruster/app.py
--rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-2.0.0/Ruster/blueprints.py
--rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-2.0.0/Ruster/exceptions.py
--rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-2.0.0/Ruster/hasher.py
--rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-2.0.0/Ruster/jwt.py
--rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-2.0.0/Ruster/limiter.py
--rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-2.0.0/Ruster/mailer.py
--rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-2.0.0/Ruster/sanitizer.py
--rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-2.0.0/Ruster/session.py
--rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-2.0.0/Ruster/wtf.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.558743 Ruster-2.0.0/Ruster.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:26:26.566744 Ruster-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-07-07 17:26:14.000000 Ruster-2.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-08 21:03:04.828704 Ruster-2.0.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/Ruster.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      383 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/ruster/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-07 17:26:00.000000 Ruster-2.0.1/ruster/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13358 2023-07-08 20:55:05.000000 Ruster-2.0.1/ruster/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1345 2023-07-06 08:52:08.000000 Ruster-2.0.1/ruster/blueprints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-07-04 18:04:16.000000 Ruster-2.0.1/ruster/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3761 2023-07-06 17:39:42.000000 Ruster-2.0.1/ruster/hasher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7955 2023-07-06 17:40:00.000000 Ruster-2.0.1/ruster/jwt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-06 08:37:16.000000 Ruster-2.0.1/ruster/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2023-07-06 17:39:06.000000 Ruster-2.0.1/ruster/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2023-07-08 20:35:21.000000 Ruster-2.0.1/ruster/sanitizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 18:45:58.000000 Ruster-2.0.1/ruster/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2679 2023-07-06 17:40:22.000000 Ruster-2.0.1/ruster/wtf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 21:03:04.828704 Ruster-2.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-08 21:00:20.000000 Ruster-2.0.1/setup.py
```

### Comparing `Ruster-2.0.0/Ruster/app.py` & `Ruster-2.0.1/ruster/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
 import asyncio
+import traceback
+import os
+import importlib.util
 from werkzeug.wrappers import Request, Response
 from werkzeug.routing import Map, Rule
 from jinja2 import Environment, FileSystemLoader
-from .exceptions import HTTPException
-from .blueprints import Blueprint
-from werkzeug.exceptions import NotFound, MethodNotAllowed, BadRequest, Unauthorized, Forbidden
+from werkzeug.exceptions import NotFound, MethodNotAllowed, BadRequest, Unauthorized, Forbidden, HTTPException
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from itsdangerous import URLSafeTimedSerializer, BadSignature
 from werkzeug.serving import run_simple
 from werkzeug.urls import url_encode
-import asyncio
 from .session import session_manager
 from .limiter import Limiter
-import traceback
-import os
-import importlib.util
+
 
 class Rust:
     def __init__(self):
         self.url_map = Map()
         self.error_handlers = {}
         self.before_request_funcs = []
         self.after_request_funcs = []
@@ -32,42 +30,45 @@
         self.middlewares = []
         self.flash_messages = {}
         self.request_context = None
         self.static_folder = 'public'
         self.template_folder = 'templates'
         self.limiter = Limiter()
         self.config = {}
-        self.configure_app()
+        self.load_config()
 
     def route(self, rule, methods=['GET'], strict_slashes=False, secure=False):
         def decorator(f):
             endpoint = f.__name__
             self.url_map.add(Rule(rule, methods=methods, endpoint=endpoint, strict_slashes=strict_slashes))
             self.view_functions[endpoint] = f
 
             if secure:
                 self.view_functions[endpoint] = self._secure_wrapper(self.view_functions[endpoint])
 
             return f
+
         return decorator
 
     def _secure_wrapper(self, view_func):
         async def secure_view(request, *args, **kwargs):
             if not request.is_secure:
-                return Response('403 Forbidden - This route requires a secure (HTTPS) connection.', status=403)
+                return self.handle_forbidden("")
             return await view_func(request, *args, **kwargs)
+
         return secure_view
 
     def errorhandler(self, code):
         def decorator(f):
             self.error_handlers[code] = f
             return f
+
         return decorator
 
-    def configure_app(self):
+    def load_config(self):
         for key, value in self.config.items():
             setattr(self.jwt_manager, key, value)
 
     def before_request(self, f):
         self.before_request_funcs.append(f)
         return f
 
@@ -135,85 +136,89 @@
         except Forbidden as e:
             return self.handle_forbidden(request, e)
         except Unauthorized as e:
             return self.handle_unauthorized(request, e)
         except HTTPException as e:
             response = await self.handle_exception(e)
         return response
-    
+
     def serve_static(self, path):
         static_path = os.path.join(self.static_folder, path)
         if os.path.exists(static_path):
             with open(static_path, 'rb') as f:
                 response = self.response(f.read())
                 response.headers['Content-Type'] = 'text/css' if path.endswith('.css') else 'text/javascript'
                 return response
         return self.handle_not_found()
 
     def handle_not_found(self, request):
-        error_template_path = os.path.join('errors', '404.html')
+        error_template_path = os.path.join(self.template_folder, 'errors', '404.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=404, content_type='text/html')
         else:
             return Response('404 Page not found', status=404)
-        
+
     def handle_method_not_allowed(self, request):
-        error_template_path = os.path.join('errors', '405.html')
+        error_template_path = os.path.join(self.template_folder, 'errors', '405.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=405, content_type='text/html')
         else:
             return Response('405 Method Not Allowed', status=405)
 
     def handle_error(self, error):
         traceback_message = traceback.format_exc()
         response = Response(traceback_message, status=500)
         return response
 
-    def handle_bad_request(self, error):
-        error_template_path = os.path.join('errors', '400.html')
+    def handle_bad_request(self, request):
+        error_template_path = os.path.join(self.template_folder, 'errors', '400.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=400, content_type='text/html')
         else:
             return Response('400 Bad Request', status=400)
 
-    def handle_unauthorized(self, error):
-        error_template_path = os.path.join('errors', '401.html')
+    def handle_unauthorized(self, request):
+        error_template_path = os.path.join(self.template_folder, 'errors', '401.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=401, content_type='text/html')
         else:
             return Response('401 Unauthorized', status=401)
 
-    def handle_forbidden(self, error):
-        error_template_path = os.path.join('errors', '403.html')
+    def handle_forbidden(self, request):
+        error_template_path = os.path.join(self.template_folder, 'errors', '403.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=403, content_type='text/html')
         else:
             return Response('403 Forbidden', status=403)
 
     async def process_request(self, request):
         response = None  # Initialize the response variable
         for func in self.before_request_funcs:
             response = await func(request)
             if response is not None:
-                return response
+                break  # Exit the loop if a response is generated
 
-        # Add session handling
         session_id = request.cookies.get('session_id')
         if session_id:
             session = session_manager.get_session(session_id)
+            if session is None:
+                session_id = session_manager.create_session()
+                session = session_manager.get_session(session_id)
+                response = Response()  # Initialize the response for new session
+                response.set_cookie('session_id', session_id)
         else:
             session_id = session_manager.create_session()
             session = session_manager.get_session(session_id)
             response = Response()  # Initialize the response for new session
             response.set_cookie('session_id', session_id)
 
         request.session = session
@@ -229,36 +234,39 @@
     async def handle_exception(self, e):
         if e.code in self.error_handlers:
             return await self.error_handlers[e.code](e)
         else:
             return Response('An error occurred.', status=500)
 
     def __call__(self, environ, start_response):
+        session_manager.set_secret_key('your_secret_key')  # Replace 'your_secret_key' with your actual secret key
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
         return loop.run_until_complete(self.wsgi_app(environ, start_response))
 
 
 class VeloRequest(Request):
     @property
     def session(self):
         return session_manager.get_session(self.cookies.get('session_id'))
 
+
 crust = Rust()
 request = VeloRequest
 
 
 def jsonify(data):
     return Response(json.dumps(data), mimetype='application/json')
 
 
 def render_template(template_name, **context):
     template = crust.template_env.get_template(template_name)
     return Response(template.render(**context), mimetype='text/html')
 
+
 def make_response(response):
     if isinstance(response, str):
         return Response(response)
     return response
 
 
 def redirect(location):
@@ -279,24 +287,21 @@
     response = Response()
     response.headers['Content-Disposition'] = f'attachment; filename="{filename}"' if as_attachment else f'inline; filename="{filename}"'
     if mimetype is not None:
         response.headers['Content-Type'] = mimetype
     return response
 
 
-def redirect_args(location, *args, **kwargs):
-    location = url_for(location, *args, **kwargs)
-    return redirect(location)
-
-def redirect_args(self, location, **kwargs):
-        url = location
-        if kwargs:
-            query_params = url_encode(kwargs)
-            url += f'?{query_params}'
-        return Response(status=302, headers={'Location': url})
+def redirect_args(location, **kwargs):
+    url = location
+    if kwargs:
+        query_params = url_encode(kwargs)
+        url += f'?{query_params}'
+    return Response(status=302, headers={'Location': url})
+
 
 def send_from_directory(directory, filename):
     root = os.path.join(crust.static_folder, directory)
     return send_file(os.path.join(root, filename))
 
 
 def url_rule(rule, view_func, **options):
@@ -328,24 +333,28 @@
     crust.static_folder = static_folder
 
 
 def set_template_folder(template_folder):
     crust.template_folder = template_folder
     crust.template_env = Environment(loader=FileSystemLoader(template_folder))
 
-def make_secure_token(self, salt=None, key=None):
-        if salt is None:
-            salt = self.config.get('SECRET_KEY', os.urandom(24))
-        if key is None:
-            key = os.urandom(16)
-        serializer = URLSafeTimedSerializer(salt)
-        return serializer.dumps(key)
 
-def check_secure_token(self, token, salt=None):
+@staticmethod
+def make_secure_token(salt=None, key=None):
+    if salt is None:
+        salt = crust.config.get('SECRET_KEY', os.urandom(24))
+    if key is None:
+        key = os.urandom(16)
+    serializer = URLSafeTimedSerializer(salt)
+    return serializer.dumps(key)
+
+
+@staticmethod
+def check_secure_token(token, salt=None):
     if salt is None:
-        salt = self.config.get('SECRET_KEY', os.urandom(24))
+        salt = crust.config.get('SECRET_KEY', os.urandom(24))
     serializer = URLSafeTimedSerializer(salt)
     try:
         key = serializer.loads(token)
         return key
     except BadSignature:
-        return None
+        return None
```

### Comparing `Ruster-2.0.0/Ruster/blueprints.py` & `Ruster-2.0.1/ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/hasher.py` & `Ruster-2.0.1/ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/jwt.py` & `Ruster-2.0.1/ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/limiter.py` & `Ruster-2.0.1/ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/mailer.py` & `Ruster-2.0.1/ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/sanitizer.py` & `Ruster-2.0.1/ruster/sanitizer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     if not any(char.isdigit() for char in password):
         return False
 
     # Check for special characters
     if not any(char in "!@#$%^&*()-_=+{}[]|;:,<.>/?`~" for char in password):
         return False
 
-    return True
+    return True
```

### Comparing `Ruster-2.0.0/Ruster/session.py` & `Ruster-2.0.1/ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.0/Ruster/wtf.py` & `Ruster-2.0.1/ruster/wtf.py`

 * *Files identical despite different names*

