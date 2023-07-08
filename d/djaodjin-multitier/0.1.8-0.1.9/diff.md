# Comparing `tmp/djaodjin-multitier-0.1.8.tar.gz` & `tmp/djaodjin-multitier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djaodjin-multitier-0.1.8.tar", last modified: Sun Feb  3 08:04:07 2019, max compression
+gzip compressed data, was "dist/djaodjin-multitier-0.1.9.tar", last modified: Thu Feb 14 06:29:13 2019, max compression
```

## Comparing `djaodjin-multitier-0.1.8.tar` & `djaodjin-multitier-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-03 08:04:07.000000 djaodjin-multitier-0.1.8/
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-03 08:04:07.000000 djaodjin-multitier-0.1.8/multitier/
--rw-r--r--   0 smirolo    (502) staff       (20)     1438 2019-02-03 07:57:44.000000 djaodjin-multitier-0.1.8/multitier/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3850 2018-10-16 19:54:35.000000 djaodjin-multitier-0.1.8/multitier/compat.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1653 2016-12-24 22:30:27.000000 djaodjin-multitier-0.1.8/multitier/context_processors.py
--rw-r--r--   0 smirolo    (502) staff       (20)     5691 2017-02-04 05:46:00.000000 djaodjin-multitier-0.1.8/multitier/finders.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-03 08:04:07.000000 djaodjin-multitier-0.1.8/multitier/loaders/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2016-10-08 01:11:54.000000 djaodjin-multitier-0.1.8/multitier/loaders/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3791 2017-02-04 05:45:18.000000 djaodjin-multitier-0.1.8/multitier/loaders/django.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3584 2019-01-31 04:08:10.000000 djaodjin-multitier-0.1.8/multitier/loaders/jinja2.py
--rw-r--r--   0 smirolo    (502) staff       (20)     6267 2019-01-11 07:53:37.000000 djaodjin-multitier-0.1.8/multitier/middleware.py
--rw-r--r--   0 smirolo    (502) staff       (20)     4896 2019-02-02 09:29:24.000000 djaodjin-multitier-0.1.8/multitier/mixins.py
--rw-r--r--   0 smirolo    (502) staff       (20)     8621 2019-02-03 07:26:11.000000 djaodjin-multitier-0.1.8/multitier/models.py
--rw-r--r--   0 smirolo    (502) staff       (20)     4002 2019-01-02 18:07:04.000000 djaodjin-multitier-0.1.8/multitier/routers.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3069 2019-02-03 07:45:34.000000 djaodjin-multitier-0.1.8/multitier/settings.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-03 08:04:07.000000 djaodjin-multitier-0.1.8/multitier/templatetags/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2016-10-08 01:11:54.000000 djaodjin-multitier-0.1.8/multitier/templatetags/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3170 2018-06-20 15:35:09.000000 djaodjin-multitier-0.1.8/multitier/templatetags/multitier_tags.py
--rw-r--r--   0 smirolo    (502) staff       (20)     6496 2018-06-20 15:35:09.000000 djaodjin-multitier-0.1.8/multitier/thread_locals.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9427 2018-08-22 22:12:51.000000 djaodjin-multitier-0.1.8/multitier/urlresolvers.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2126 2019-02-03 08:01:11.000000 djaodjin-multitier-0.1.8/multitier/utils.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1474 2019-02-03 08:04:07.000000 djaodjin-multitier-0.1.8/PKG-INFO
--rw-r--r--   0 smirolo    (502) staff       (20)      921 2019-02-03 07:23:11.000000 djaodjin-multitier-0.1.8/README.md
--rw-r--r--   0 smirolo    (502) staff       (20)       40 2019-02-03 07:20:32.000000 djaodjin-multitier-0.1.8/requirements.txt
--rw-r--r--   0 smirolo    (502) staff       (20)     2153 2019-02-03 08:02:13.000000 djaodjin-multitier-0.1.8/setup.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-14 06:29:13.000000 djaodjin-multitier-0.1.9/
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-14 06:29:13.000000 djaodjin-multitier-0.1.9/multitier/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1438 2019-02-14 06:27:24.000000 djaodjin-multitier-0.1.9/multitier/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3850 2019-02-14 06:27:54.000000 djaodjin-multitier-0.1.9/multitier/compat.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1653 2016-12-24 22:30:27.000000 djaodjin-multitier-0.1.9/multitier/context_processors.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     5691 2017-02-04 05:46:00.000000 djaodjin-multitier-0.1.9/multitier/finders.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-14 06:29:13.000000 djaodjin-multitier-0.1.9/multitier/loaders/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2016-10-08 01:11:54.000000 djaodjin-multitier-0.1.9/multitier/loaders/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3791 2017-02-04 05:45:18.000000 djaodjin-multitier-0.1.9/multitier/loaders/django.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3584 2019-01-31 04:08:10.000000 djaodjin-multitier-0.1.9/multitier/loaders/jinja2.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     6267 2019-02-14 06:28:00.000000 djaodjin-multitier-0.1.9/multitier/middleware.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     4896 2019-02-02 09:29:24.000000 djaodjin-multitier-0.1.9/multitier/mixins.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9060 2019-02-13 01:39:30.000000 djaodjin-multitier-0.1.9/multitier/models.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     4028 2019-02-07 05:00:38.000000 djaodjin-multitier-0.1.9/multitier/routers.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3069 2019-02-07 05:00:38.000000 djaodjin-multitier-0.1.9/multitier/settings.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2019-02-14 06:29:13.000000 djaodjin-multitier-0.1.9/multitier/templatetags/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2016-10-08 01:11:54.000000 djaodjin-multitier-0.1.9/multitier/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3170 2019-02-14 06:28:07.000000 djaodjin-multitier-0.1.9/multitier/templatetags/multitier_tags.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     6496 2019-02-14 06:28:17.000000 djaodjin-multitier-0.1.9/multitier/thread_locals.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9427 2019-02-14 06:28:22.000000 djaodjin-multitier-0.1.9/multitier/urlresolvers.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2126 2019-02-07 05:00:38.000000 djaodjin-multitier-0.1.9/multitier/utils.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1474 2019-02-14 06:29:13.000000 djaodjin-multitier-0.1.9/PKG-INFO
+-rw-r--r--   0 smirolo    (502) staff       (20)      921 2019-02-07 05:00:38.000000 djaodjin-multitier-0.1.9/README.md
+-rw-r--r--   0 smirolo    (502) staff       (20)       40 2019-02-07 05:00:38.000000 djaodjin-multitier-0.1.9/requirements.txt
+-rw-r--r--   0 smirolo    (502) staff       (20)     2153 2019-02-03 08:02:13.000000 djaodjin-multitier-0.1.9/setup.py
```

### Comparing `djaodjin-multitier-0.1.8/multitier/__init__.py` & `djaodjin-multitier-0.1.9/multitier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the multitier django app.
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
```

### Comparing `djaodjin-multitier-0.1.8/multitier/compat.py` & `djaodjin-multitier-0.1.9/multitier/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018, DjaoDjin inc.
+# Copyright (c) 2019, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `djaodjin-multitier-0.1.8/multitier/context_processors.py` & `djaodjin-multitier-0.1.9/multitier/context_processors.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/finders.py` & `djaodjin-multitier-0.1.9/multitier/finders.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/loaders/django.py` & `djaodjin-multitier-0.1.9/multitier/loaders/django.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/loaders/jinja2.py` & `djaodjin-multitier-0.1.9/multitier/loaders/jinja2.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/middleware.py` & `djaodjin-multitier-0.1.9/multitier/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018, Djaodjin Inc.
+# Copyright (c) 2019, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `djaodjin-multitier-0.1.8/multitier/mixins.py` & `djaodjin-multitier-0.1.9/multitier/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/models.py` & `djaodjin-multitier-0.1.9/multitier/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 """
 Models for the multi-tier application.
 """
 
 import re, string
 
+from django.core.mail import get_connection as get_connection_base
 from django.core.validators import (_lazy_re_compile, RegexValidator,
     URLValidator)
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils._os import safe_join
 from django.utils.encoding import python_2_unicode_compatible
 from django.utils.translation import ugettext_lazy as _
@@ -79,16 +80,16 @@
 
     # Since most DNS provider limit subdomain length to 25 characters,
     # we do here too. `django.contrib.Site` limits the domain length
     # to 100 characters so we also do the same. Though 100 characters
     # is often not enough for 3rd part db/email host names (ex: AWS RDS,
     # AWS SES) so we bumped the limit to 255 for those.
     slug = models.SlugField(unique=True, max_length=25,
-        validators=[SUBDOMAIN_SLUG],
-        help_text="unique identifier for the site (also serves as subdomain)")
+        validators=[SUBDOMAIN_SLUG], help_text=_(
+            "unique identifier for the site (also serves as subdomain)"))
 
     domain = models.CharField(max_length=100, null=True, blank=True,
         validators=[domain_name_validator, RegexValidator(
             URLValidator.host_re,
             _("Enter a valid 'domain', ex: example.com"), 'invalid')],
         help_text=_(
             _("fully qualified domain name at which the site is available")))
@@ -105,51 +106,47 @@
     tag = models.CharField(null=True, max_length=255,
         help_text=_("Tags can be used by the project to filter sites"))
     base = models.ForeignKey('self',
         null=True, on_delete=models.CASCADE,
         help_text=_("The site is a derivative of this parent."))
 
     # Database connection
-    db_name = models.SlugField(null=True,
+    db_name = models.SlugField(max_length=255, null=True,
         help_text=_("name of database to connect to for the site"))
     db_host = models.CharField(max_length=255, null=True, blank=True,
         validators=[HOST_VALIDATOR],
         help_text=_("host to connect to the database"))
     db_port = models.IntegerField(null=True, blank=True,
         help_text=_("port to connect to the database host"))
     db_host_user = models.CharField(max_length=128, null=True, blank=True,
         help_text=_("username authorized to connect to the database"))
-    db_host_password = models.CharField(_('Password'),  max_length=128,
+    db_host_password = models.CharField(_('Password'), max_length=128,
         null=True, blank=True,
         help_text=_("password to authenticate user connecting to the database"))
 
     # SMTP connection
     email_default_from = models.EmailField(null=True, blank=True)
     email_host = models.CharField(max_length=255, null=True, blank=True,
         validators=[HOST_VALIDATOR],
         help_text=_("host to connect to the SMTP server"))
     email_port = models.IntegerField(null=True, blank=True,
         help_text=_("port to connect to the SMTP server"))
     email_host_user = models.CharField(max_length=128, null=True, blank=True,
         help_text=_("username authorized to send e-mails on the SMTP server"))
-    email_host_password = models.CharField(_('Password'),  max_length=128,
+    email_host_password = models.CharField(_('Password'), max_length=128,
         null=True, blank=True,
         help_text=_("password to authenticate the user with the SMTP server"))
 
     class Meta:
         swappable = 'MULTITIER_SITE_MODEL'
         abstract = True
 
     def __str__(self): #pylint: disable=super-on-old-class
         return self.slug
 
-
-    def __str__(self): #pylint: disable=super-on-old-class
-        return self.slug
-
     def as_base(self):
         """
         Returns either the base site or ``self`` if no base exists.
         """
         if self.base_id:
             return self.base
         return self
@@ -183,14 +180,26 @@
                 tags = [rec for rec in tags if rec != tag]
         self.tag += ','.join(tags)
 
     def remove_tags(self, tags):
         self.tag = ','.join([
             tag for tag in self.tag.split(',') if tag not in tags])
 
+    def get_email_connection(self):
+        kwargs = {}
+        if self.email_host:
+            kwargs['host'] = self.email_host
+        if self.email_port:
+            kwargs['port'] = self.email_port
+        if self.email_host_user:
+            kwargs['username'] = self.email_host_user
+        if self.email_host_password:
+            kwargs['password'] = self.get_email_host_password()
+        return get_connection_base(**kwargs)
+
     def get_from_email(self):
         if self.email_default_from:
             return self.email_default_from
         if self.email_host_user and '@' in self.email_host_user:
             return self.email_host_user
         return settings.DEFAULT_FROM_EMAIL
```

### Comparing `djaodjin-multitier-0.1.8/multitier/routers.py` & `djaodjin-multitier-0.1.9/multitier/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017, Djaodjin Inc.
+# Copyright (c) 2019, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -88,17 +88,18 @@
     # XXX Note here running tests with Django <1.7 will call
     #     allow_syncdb instead.
     def allow_migrate(self, database, app_label, model_name=None, **hints):
         """
         Make sure the apps only appears in the current provider
         database.
         """
+        result = True
         model = hints.get('model')
         if model is None:
             if model_name is not None:
                 model = get_app_model_class(app_label, model_name)
             else:
                 # Django 1.7 prototype is allow_migrate(self, db, model)
                 model = app_label
         if database != DEFAULT_DB_ALIAS:
-            return self.includes(model)
-        return True
+            result = self.includes(model)
+        return result
```

### Comparing `djaodjin-multitier-0.1.8/multitier/settings.py` & `djaodjin-multitier-0.1.9/multitier/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/multitier/templatetags/multitier_tags.py` & `djaodjin-multitier-0.1.9/multitier/templatetags/multitier_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018, DjaoDjin inc.
+# Copyright (c) 2019, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `djaodjin-multitier-0.1.8/multitier/thread_locals.py` & `djaodjin-multitier-0.1.9/multitier/thread_locals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018, Djaodjin Inc.
+# Copyright (c) 2019, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `djaodjin-multitier-0.1.8/multitier/urlresolvers.py` & `djaodjin-multitier-0.1.9/multitier/urlresolvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018, Djaodjin Inc.
+# Copyright (c) 2019, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `djaodjin-multitier-0.1.8/multitier/utils.py` & `djaodjin-multitier-0.1.9/multitier/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/PKG-INFO` & `djaodjin-multitier-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: djaodjin-multitier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Multi-tier Django app
 Home-page: https://github.com/djaodjin/djaodjin-multitier/
 Author: DjaoDjin inc.
 Author-email: support@djaodjin.com
 License: BSD
-Download-URL: https://github.com/djaodjin/djaodjin-multitier/tarball/0.1.8
+Download-URL: https://github.com/djaodjin/djaodjin-multitier/tarball/0.1.9
 Description: djaodjin-multitier is a Django application that implements shared tenancy.
         
         Major Features:
         
           - Dynamically select the following based on subdomain or path prefix:
               * Database connection
               * SMTP connection
```

### Comparing `djaodjin-multitier-0.1.8/README.md` & `djaodjin-multitier-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `djaodjin-multitier-0.1.8/setup.py` & `djaodjin-multitier-0.1.9/setup.py`

 * *Files identical despite different names*

