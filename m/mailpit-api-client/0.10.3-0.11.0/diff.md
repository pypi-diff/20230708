# Comparing `tmp/mailpit-api-client-0.10.3.tar.gz` & `tmp/mailpit-api-client-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.10.3.tar", last modified: Fri Jun 30 13:32:46 2023, max compression
+gzip compressed data, was "mailpit-api-client-0.11.0.tar", last modified: Sat Jul  8 15:48:08 2023, max compression
```

## Comparing `mailpit-api-client-0.10.3.tar` & `mailpit-api-client-0.11.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 15:48:08.000000 mailpit-api-client-0.11.0/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-08 15:47:57.000000 mailpit-api-client-0.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:48:08.113917 mailpit-api-client-0.11.0/setup.cfg
```

### Comparing `mailpit-api-client-0.10.3/LICENSE` & `mailpit-api-client-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.3/PKG-INFO` & `mailpit-api-client-0.11.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.10.3
+Version: 0.11.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -195,26 +195,41 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <corvan@gmx.de>
+    Lars Liedtke <lars@familie-liedtke.net>
 :Version:
-    0.10.3
+    0.11.0
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
 Searching for an alternative, I found Mailpit - for which I decided to write an API-client in my free time.
 
+-------
+Install
+-------
+If you want to use the library with ``unittest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client
+
+If you want to use the library with ``pytest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client[pytest]
+
 -----
 Usage
 -----
 
 this library - as is Mailpit - is mostly meant for testing. Giving the url of Mailpit to a tool to send e-mail messages to and then use this client to check on the API if the mail was sent.
 
 ------
@@ -239,18 +254,37 @@
     messages = api.get_messages()
 
 messages will be an instance of ``mailpit.client.models.Messages`` , which you can find in link:mailpit/client/models/messages.py[mailpit/client/models.py]. +
 The model-classes' attributes are named the same as Mailpit's responses, as documented in the API's `README.md <https://github.com/axllent/mailpit/blob/develop/docs/apiv1/README.md>`_, but as is convention in Python in Snakecase.
 
 For examples have a look at the link:tests[tests]
 
-== Testing
+-------
+Testing
+-------
 
-To make testing easier I plan to provide testhelpers like TestCase-classes of ``unittest`` and ``pytest``-fixtures.
+To make testing easier there are test-helpers inside the ``mailpit.testing`` package.
 
-=== unittest
-tbd
+________
+unittest
+________
+
+In order to provide some convenience a test-case class has been created with the name ``EMailTestCase`` deriving from ``unittest.TestCase``, which is meant to be inherited from, as you would do from ``TestCase``:
+
+.. code-block:: python
+
+    from mailpit.testing.unittest import EMailTestCase
+
+    class MyTest(EMailTestCase):
+
+         def test_sending_email():
+            ...
+
+The class adds a few methods and attributes, so that you are able to assert, if your message has been sent, or if two messages are equal.
+
+______
+pytest
+______
 
-=== pytest
 tbd
 
 .. [1] If you have it running differently, you have to adjust the URL you pass.
```

### Comparing `mailpit-api-client-0.10.3/README.rst` & `mailpit-api-client-0.11.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,41 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <corvan@gmx.de>
+    Lars Liedtke <lars@familie-liedtke.net>
 :Version:
-    0.10.3
+    0.11.0
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
 Searching for an alternative, I found Mailpit - for which I decided to write an API-client in my free time.
 
+-------
+Install
+-------
+If you want to use the library with ``unittest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client
+
+If you want to use the library with ``pytest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client[pytest]
+
 -----
 Usage
 -----
 
 this library - as is Mailpit - is mostly meant for testing. Giving the url of Mailpit to a tool to send e-mail messages to and then use this client to check on the API if the mail was sent.
 
 ------
@@ -46,18 +61,37 @@
     messages = api.get_messages()
 
 messages will be an instance of ``mailpit.client.models.Messages`` , which you can find in link:mailpit/client/models/messages.py[mailpit/client/models.py]. +
 The model-classes' attributes are named the same as Mailpit's responses, as documented in the API's `README.md <https://github.com/axllent/mailpit/blob/develop/docs/apiv1/README.md>`_, but as is convention in Python in Snakecase.
 
 For examples have a look at the link:tests[tests]
 
-== Testing
+-------
+Testing
+-------
 
-To make testing easier I plan to provide testhelpers like TestCase-classes of ``unittest`` and ``pytest``-fixtures.
+To make testing easier there are test-helpers inside the ``mailpit.testing`` package.
 
-=== unittest
-tbd
+________
+unittest
+________
+
+In order to provide some convenience a test-case class has been created with the name ``EMailTestCase`` deriving from ``unittest.TestCase``, which is meant to be inherited from, as you would do from ``TestCase``:
+
+.. code-block:: python
+
+    from mailpit.testing.unittest import EMailTestCase
+
+    class MyTest(EMailTestCase):
+
+         def test_sending_email():
+            ...
+
+The class adds a few methods and attributes, so that you are able to assert, if your message has been sent, or if two messages are equal.
+
+______
+pytest
+______
 
-=== pytest
 tbd
 
 .. [1] If you have it running differently, you have to adjust the URL you pass.
```

### Comparing `mailpit-api-client-0.10.3/mailpit/client/api.py` & `mailpit-api-client-0.11.0/mailpit/client/api.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.3/mailpit/client/models.py` & `mailpit-api-client-0.11.0/mailpit/client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Definitions of model classes, that wrap Mailpit's API data-structures. Defined with 
+:py:mod:`dataclasses` and :py:mod:`dataclasses_json`, in order to use them as json over 
+the API and be used as objects in the Python domain."""
 import dataclasses as _dc
 import datetime as _dt
 import decimal as _d
 import email.utils as _email
 import logging
 import re as _re
 from typing import Optional, Iterable
@@ -12,46 +15,48 @@
 
 _log = logging.getLogger("mailpit_client")
 
 
 @_dj.dataclass_json
 @_dc.dataclass(init=True)
 class Contact:
-    """
-    class representing a mail contact splitting 'Test User <test@example.com> into
-    its name and address parts
-    """
+    """Represents a mail contact splitting 'Test User <test@example.com> into
+    its name and address parts"""
 
     # pylint: disable=too-few-public-methods
 
     name: str = _dc.field(init=True, metadata=_dj.config(field_name="Name"))
+    """Contact's Name"""
     address: str = _dc.field(init=True, metadata=_dj.config(field_name="Address"))
+    """Contact's E-Mail address"""
 
     def __lt__(self, other):
         return f"{other.name} {other.address}".__lt__(f"{self.name} {self.address}")
 
     def __hash__(self):
         return f"{self.name} {self.address}".__hash__()
 
 
 @_dc.dataclass(init=True)
 class Attachment(_dj.DataClassJsonMixin):
-    """
-    class representing an attachment of a message
-    """
+    """Represents an attachment of a :py:class:`Message`"""
 
     # pylint: disable=too-few-public-methods
 
     part_id: str = _dc.field(init=True, metadata=_dj.config(field_name="PartID"))
+    """Attachment's part ID"""
     file_name: str = _dc.field(init=True, metadata=_dj.config(field_name="FileName"))
+    """Attachment's file name"""
     content_type: str = _dc.field(
         init=True, metadata=_dj.config(field_name="ContentType")
     )
+    """Attachment's MIME content-type"""
     content_id: str = _dc.field(init=True, metadata=_dj.config(field_name="ContentID"))
     size: int = _dc.field(init=True, metadata=_dj.config(field_name="Size"))
+    """Attachment's size in bytes"""
 
     def __lt__(self, other: "Attachment"):
         return (
             f"{other.part_id} {other.file_name} {other.content_type} "
             f"{other.content_id} {other.size}".__lt__(
                 f"{self.part_id} {self.file_name} {self.content_type} "
                 f"{self.content_id} {self.size}"
@@ -63,45 +68,43 @@
             f"{self.part_id} {self.file_name} {self.content_type} "
             f"{self.content_id} {self.size}"
         ).__hash__()
 
 
 @_dc.dataclass(init=True)
 class Message(_dj.DataClassJsonMixin):
-    """
-    class representing a Message returned by the message-endpoint
-    """
+    """Represents a message returned by the message-endpoint"""
 
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-few-public-methods
     # pylint: disable=invalid-name
 
     id: str = _dc.field(init=True, metadata=_dj.config(field_name="ID"))
-    """The message's database ID, of Mailpit's message-database"""
+    """Message's database ID, of Mailpit's message-database"""
     message_id: str = _dc.field(init=True, metadata=_dj.config(field_name="MessageID"))
-    """The message's RFC-5322 message-id"""
+    """Message's RFC-5322 message-id"""
     read: bool = _dc.field(init=True, metadata=_dj.config(field_name="Read"))
-    """always true (message marked read on open)"""
+    """Always true (message marked read on open)"""
     from_: Optional[Contact] = _dc.field(
         init=True, metadata=_dj.config(field_name="From")
     )
-    """The :Contact: the message is from"""
+    """The :py:class`Contact`: the message is from"""
     to: list[Contact] = _dc.field(init=True, metadata=_dj.config(field_name="To"))
-    """Message To-Header, the list of :Contact: the message is addressed to"""
+    """Message's To-Header, the list of :Contact: the message is addressed to"""
     cc: Optional[list[Contact]] = _dc.field(
         init=True, metadata=_dj.config(field_name="Cc")
     )
-    """Message CC-Header, the list of :Contact: that the message is coal-copied to"""
+    """Message's CC-Header, the list of :Contact: that the message is coal-copied to"""
     bcc: Optional[list[Contact]] = _dc.field(
         init=True, metadata=_dj.config(field_name="Bcc")
     )
-    """Message BCC-Header, the list of :Contact:, that the message is blindly 
+    """Message's BCC-Header, the list of :Contact:, that the message is blindly 
     coal-copied to"""
     subject: str = _dc.field(init=True, metadata=_dj.config(field_name="Subject"))
-    """Message subject"""
+    """Message's subject"""
     date: _dt.date = _dc.field(
         init=True,
         metadata=_dj.config(
             field_name="Date",
             encoder=_dt.datetime.isoformat,
             decoder=_dt.datetime.fromisoformat,
             mm_field=marshmallow.fields.DateTime("iso"),
@@ -109,15 +112,15 @@
     )
     """Parsed email local date & time from headers"""
     text: Optional[str] = _dc.field(init=True, metadata=_dj.config(field_name="Text"))
     """Plain text MIME part of the email"""
     html: Optional[str] = _dc.field(init=True, metadata=_dj.config(field_name="HTML"))
     """HTML MIME part (if exists)"""
     size: int = _dc.field(init=True, metadata=_dj.config(field_name="Size"))
-    """Total size of raw email"""
+    """Total size of raw email in bytes"""
     inline: list[Attachment] = _dc.field(
         init=True, metadata=_dj.config(field_name="Inline")
     )
     """Inline Attachments"""
     attachments: list[Attachment] = _dc.field(
         init=True, metadata=_dj.config(field_name="Attachments")
     )
@@ -250,17 +253,16 @@
     result = zulu_to_utc_shift(millis_to_3_digit(isoformat))
     _log.debug(f"new isoformat: {result}")
     return _dt.datetime.fromisoformat(result)
 
 
 @_dc.dataclass(init=True)
 class MessageSummary(_dj.DataClassJsonMixin):
-    """
-    class representing a single message that has been returned by the messages endpoint
-    """
+    """class representing a single message that has been returned by the messages
+    endpoint"""
 
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-few-public-methods
     # pylint: disable=invalid-name
 
     id: str = _dc.field(init=True, metadata=_dj.config(field_name="ID"))
     message_id: str = _dc.field(init=True, metadata=_dj.config(field_name="MessageID"))
@@ -292,17 +294,15 @@
         init=True, metadata=_dj.config(field_name="Attachments")
     )
 
 
 @_dc.dataclass(init=True)
 class Messages(_dj.DataClassJsonMixin):
     # pylint: disable=too-few-public-methods
-    """
-    class representing the returns of the messages endpoint
-    """
+    """class representing the returns of the messages endpoint"""
 
     total: int = _dc.field(init=True)
     """Total messages in mailbox"""
     unread: int = _dc.field(init=True)
     """Total unread messages in mailbox"""
     count: int = _dc.field(init=True)
     """Number of messages returned in request"""
```

### Comparing `mailpit-api-client-0.10.3/mailpit/testing/unittest.py` & `mailpit-api-client-0.11.0/mailpit/testing/unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Module providing helpers for :py:module:`unittest` kind of testing against the
+"""Provides helpers for :py:mod:`unittest` kind of testing against the
 Mailpit-API"""
 from typing import Optional
 import unittest as _unittest
 
 import mailpit.client.models as _models
 import mailpit.client.api as _api
 
 
 class EMailTestCase(_unittest.TestCase):
-    """:py:class:`unittest.TestCase` derived class with added test-helper methods and
+    """:py:class:`unittest.TestCase`-derived class with added test-helper methods and
     attributes, in order to test against the Mailpit-API. Simply derive from this class,
     as you would from :py:class:`unittest.TestCase` and write your tests as you are used
     to.
 
 
     e.g.::
 
         class ExampleTestCase(EMailTestCase):
 
             def test_api_object(self):
-            messages: mailpit.client.models.Messages = self.api.get_messages()
-            self.assertEqual(0, len(messages.messages))
+                messages: mailpit.client.models.Messages = self.api.get_messages()
+                self.assertEqual(0, len(messages.messages))
     """
 
     api_url: str = "http://localhost:8025"
     """URL pointing to the Mailpit-API to test, if you need to use another url,
     override this attribute in your derived class"""
     api: Optional[_api.API] = None
     """API object created on class setup for testing against Mailpit's API, access this
```

### Comparing `mailpit-api-client-0.10.3/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-0.11.0/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.10.3
+Version: 0.11.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -195,26 +195,41 @@
 mailpit-api-client
 ==================
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
-    Lars Liedtke <corvan@gmx.de>
+    Lars Liedtke <lars@familie-liedtke.net>
 :Version:
-    0.10.3
+    0.11.0
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
 Searching for an alternative, I found Mailpit - for which I decided to write an API-client in my free time.
 
+-------
+Install
+-------
+If you want to use the library with ``unittest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client
+
+If you want to use the library with ``pytest``:
+
+.. code-block:: bash
+
+    pip install mailpit-api-client[pytest]
+
 -----
 Usage
 -----
 
 this library - as is Mailpit - is mostly meant for testing. Giving the url of Mailpit to a tool to send e-mail messages to and then use this client to check on the API if the mail was sent.
 
 ------
@@ -239,18 +254,37 @@
     messages = api.get_messages()
 
 messages will be an instance of ``mailpit.client.models.Messages`` , which you can find in link:mailpit/client/models/messages.py[mailpit/client/models.py]. +
 The model-classes' attributes are named the same as Mailpit's responses, as documented in the API's `README.md <https://github.com/axllent/mailpit/blob/develop/docs/apiv1/README.md>`_, but as is convention in Python in Snakecase.
 
 For examples have a look at the link:tests[tests]
 
-== Testing
+-------
+Testing
+-------
 
-To make testing easier I plan to provide testhelpers like TestCase-classes of ``unittest`` and ``pytest``-fixtures.
+To make testing easier there are test-helpers inside the ``mailpit.testing`` package.
 
-=== unittest
-tbd
+________
+unittest
+________
+
+In order to provide some convenience a test-case class has been created with the name ``EMailTestCase`` deriving from ``unittest.TestCase``, which is meant to be inherited from, as you would do from ``TestCase``:
+
+.. code-block:: python
+
+    from mailpit.testing.unittest import EMailTestCase
+
+    class MyTest(EMailTestCase):
+
+         def test_sending_email():
+            ...
+
+The class adds a few methods and attributes, so that you are able to assert, if your message has been sent, or if two messages are equal.
+
+______
+pytest
+______
 
-=== pytest
 tbd
 
 .. [1] If you have it running differently, you have to adjust the URL you pass.
```

### Comparing `mailpit-api-client-0.10.3/pyproject.toml` & `mailpit-api-client-0.11.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.10.3"
+version = "0.11.0"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -18,25 +18,22 @@
     "Topic :: Communications :: Email",
     "Topic :: Communications :: Email :: Mail Transport Agents",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
 
-
-
 dependencies = [
     "dataclasses_json",
     "httpx",
     "ruff",
     "invoke >= 2.0.0",
     "logging518 >= 1.0.0",
 ]
 
-
 [project.optional-dependencies]
 docs = [
     "sphinx",
 ]
 test = [
     "black",
     "mypy>=1.1.1",
@@ -54,15 +51,15 @@
 
 [project.urls]
 repository = "https://github.com/Corvan/mailpit-api-client"
 
 
 [tool.poetry]
 name = "mailpit-api-client"
-version = "0.10.1"
+version = "0.11.0"
 description = ""
 authors = ["Lars Liedtke <lars@familie-liedtke.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dataclasses_json = "*"
 httpx = "*"
```

