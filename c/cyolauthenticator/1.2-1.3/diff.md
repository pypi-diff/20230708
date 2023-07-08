# Comparing `tmp/cyolauthenticator-1.2.tar.gz` & `tmp/cyolauthenticator-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyolauthenticator-1.2.tar", last modified: Wed Aug 11 20:01:58 2021, max compression
+gzip compressed data, was "dist/cyolauthenticator-1.3.tar", last modified: Sat Jul  8 02:46:58 2023, max compression
```

## Comparing `cyolauthenticator-1.2.tar` & `cyolauthenticator-1.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/
-drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator.egg-info/
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      251 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       18 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator.egg-info/top_level.txt
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      403 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)        1 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       38 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/setup.cfg
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      478 2021-08-11 19:15:10.000000 cyolauthenticator-1.2/README.md
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      403 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/PKG-INFO
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      485 2021-08-11 20:01:52.000000 cyolauthenticator-1.2/setup.py
-drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2021-08-11 20:01:58.000000 cyolauthenticator-1.2/cyolauthenticator/
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)     4590 2021-08-11 20:01:46.000000 cyolauthenticator-1.2/cyolauthenticator/cyolauthenticator.py
--rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       97 2021-08-11 19:15:10.000000 cyolauthenticator-1.2/cyolauthenticator/__init__.py
+drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2023-07-08 02:46:58.000000 cyolauthenticator-1.3/
+drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2023-07-08 02:46:58.000000 cyolauthenticator-1.3/cyolauthenticator.egg-info/
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      341 2023-07-08 02:46:57.000000 cyolauthenticator-1.3/cyolauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       18 2023-07-08 02:46:57.000000 cyolauthenticator-1.3/cyolauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      403 2023-07-08 02:46:57.000000 cyolauthenticator-1.3/cyolauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)        1 2023-07-08 02:46:57.000000 cyolauthenticator-1.3/cyolauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       38 2023-07-08 02:46:58.000000 cyolauthenticator-1.3/setup.cfg
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      478 2020-10-14 02:15:48.000000 cyolauthenticator-1.3/README.md
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      403 2023-07-08 02:46:58.000000 cyolauthenticator-1.3/PKG-INFO
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      485 2023-07-08 02:43:54.000000 cyolauthenticator-1.3/setup.py
+drwxr-xr-x   0 sbrandt   (1168) internalusers  (1000)        0 2023-07-08 02:46:58.000000 cyolauthenticator-1.3/cyolauthenticator/
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)     5458 2023-07-07 23:42:18.000000 cyolauthenticator-1.3/cyolauthenticator/cyolauthenticator.py
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)       97 2020-10-14 02:15:48.000000 cyolauthenticator-1.3/cyolauthenticator/__init__.py
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      813 2023-07-07 23:40:55.000000 cyolauthenticator-1.3/cyolauthenticator/chkpasswd.py
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)     2628 2023-07-08 02:41:44.000000 cyolauthenticator-1.3/cyolauthenticator/useradd.py
+-rw-r--r--   0 sbrandt   (1168) internalusers  (1000)      940 2023-07-07 23:41:10.000000 cyolauthenticator-1.3/cyolauthenticator/chpasswd.py
```

### Comparing `cyolauthenticator-1.2/cyolauthenticator/cyolauthenticator.py` & `cyolauthenticator-1.3/cyolauthenticator/cyolauthenticator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from traitlets import Unicode
 
 from jupyterhub.auth import Authenticator
 
+from traceback import print_exc
 from subprocess import call, Popen, PIPE
 from tornado.httpclient import HTTPError
 from tornado import gen
 from os import stat
 import os
 import sys
 import re
-import pwd
 from hmac import compare_digest
 from crypt import crypt
+from .useradd import user_add, get_user_data
+from .chpasswd import change_passwd
+from .chkpasswd import check_passwd
 
 # Attempt to authenticate using PAM
 def authuser(user, passw):
-    with open("/etc/shadow", "r") as fd:
-        for line in fd.readlines():
-            cols = line.split(':')
-            if cols[0] == user:
-                if compare_digest(crypt(passw, cols[1]), cols[1]):
-                  return True
-                else:
-                  break
+#    with open("/etc/shadow", "r") as fd:
+#        for line in fd.readlines():
+#            cols = line.split(':')
+#            if cols[0] == user:
+#                if passw is None or cols[1] is None:
+#                    e = HTTPError(403)
+#                    e.my_message = f"No password for account {user}"
+#                    raise e
+#                crypt_result = crypt(passw, cols[1])
+#                if crypt_result is None:
+#                    e = HTTPError(403)
+#                    e.my_message = f"No password for account {user}"
+#                    raise e
+#                if compare_digest(crypt_result , cols[1]):
+#                  return True
+#                else:
+#                  break
+    r = check_passwd(user, passw)
+    if r == 0:
+        return True
     e = HTTPError(403)
     e.my_message = "Incorrect password"
     raise e
 
 def mkuser(user, passw, passw2, code_check):
     if user == None or len(user.strip())=="":
       e = HTTPError(403)
@@ -64,75 +79,82 @@
       raise e
 
     if re.search(r'\W',passw):
       e = HTTPError(403)
       e.my_message = "Illegal character in password. Only letters, numbers and the underscore are allowed."
       raise e
 
-    home = "/home/%s" % user
-    cmd = ["useradd",user,"-s","/bin/bash"]
+    #home = "/home/%s" % user
+    #cmd = ["useradd",user,"-s","/bin/bash"]
     check_pass2 = False
-    if os.path.exists(home):
-      uid = stat(home).st_uid
-      try:
-        pwd.getpwuid(uid)
-        return authuser(user, passw)
-        # The user already exists, nothing to do
-        #return uid
-      except KeyError:
-        check_pass2 = True
-      cmd += ["-u",str(uid)]
+    udata = get_user_data(user)
+    if udata is not None:
+      if len(udata.pw_passwd)==1:
+            user_add(user)
+            change_passwd(user, passw)
+      print(f"get_user_data({user}) succeeded")
+      return authuser(user, passw)
+      # The user already exists, nothing to do
+      #return uid
     else:
-
-      if not os.path.exists("/usr/enable_mkuser"):
-        e = HTTPError(403)
-        e.my_message = "MkUser disabled"
-        raise e
-      if not code_check:
-         e = HTTPError(403)
-         e.my_message = "Code check failed"
-         raise e
+      print("No user data")
       check_pass2 = True
-      if passw != passw2:
-        e = HTTPError(403)
-        e.my_message = "Password and Password2 do not match."
-        raise e
-      cmd += ["-m"]
-      uids = set()
-      for path in os.listdir("/home"):
-        u = stat("/home/%s" % path).st_uid
-        uids.add(u)
-      for u in range(1000,100000):
-        if u in uids:
-          continue
-        try:
-          pwd.getpwuid(u)
-        except KeyError:
-          uid = u
-          cmd += ["-u",str(uid)]
-          break
+
+    if not os.path.exists("/usr/enable_mkuser"):
+      e = HTTPError(403)
+      e.my_message = "MkUser disabled"
+      raise e
+    if not code_check:
+       e = HTTPError(403)
+       e.my_message = "Code check failed"
+       raise e
+    check_pass2 = True
+    if passw != passw2:
+      e = HTTPError(403)
+      e.my_message = "Password and Password2 do not match."
+      raise e
+    #cmd += ["-m"]
 
     if check_pass2:
       if passw != passw2:
         e = HTTPError(403)
         e.my_message = "Password and Password2 do not match."
         raise e
-    call(cmd)
-    call(["su","-",user,"-c","bash /inituser.sh"])
-
-    pipe = Popen(["chpasswd"],stdin=PIPE,universal_newlines=True)
-    pipe.stdin.write("%s:%s\n" % (user, passw))
-    pipe.stdin.close()
-    pipe.wait()
-    print("Chpasswd called with %s:%s" % (user, passw))
-    call(["cp","/etc/shadow","/home/shadow"])
-    call(["cp","/etc/passwd","/home/passwd"])
+    try:
+        #call(cmd)
+        user_add(user)
+        if os.path.exists("/inituser.sh"):
+            call(["su","-",user,"-c","bash /inituser.sh"])
+
+        #pipe = Popen(["chpasswd"],stdin=PIPE,universal_newlines=True)
+        #pipe.stdin.write("%s:%s\n" % (user, passw))
+        #pipe.stdin.close()
+        #pipe.wait()
+        r  = change_passwd(user, passw)
+        #print("Chpasswd called with %s:%s" % (user, passw))
+        #call(["cp","/etc/shadow","/home/shadow"])
+        #call(["cp","/etc/passwd","/home/passwd"])
+        #call(["cp","/etc/group","/home/group"])
+    except:
+        print("An exception occurred")
+        print_exc()
+        return False
     return True
 
 class CYOLAuthenticator(Authenticator):
+
+    @staticmethod
+    def _getpwnam(name):
+        """Wrapper function to protect against `pwd` not being available
+        on Windows
+        """
+        import pwd
+
+        return get_user_data(name)
+
     password = Unicode(
         None,
         allow_none=True,
         config=True,
         help="""
         Set a global password for all users wanting to log in.
```

