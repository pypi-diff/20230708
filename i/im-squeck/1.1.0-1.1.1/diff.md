# Comparing `tmp/im-squeck-1.1.0.tar.gz` & `tmp/im-squeck-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-squeck-1.1.0.tar", last modified: Tue May 23 18:14:23 2023, max compression
+gzip compressed data, was "im-squeck-1.1.1.tar", last modified: Sat Jul  8 09:22:37 2023, max compression
```

## Comparing `im-squeck-1.1.0.tar` & `im-squeck-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:23.147401 im-squeck-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 18:14:11.000000 im-squeck-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 18:14:11.000000 im-squeck-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-23 18:14:23.147401 im-squeck-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-23 18:14:11.000000 im-squeck-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 18:14:11.000000 im-squeck-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 18:14:11.000000 im-squeck-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:14:23.147401 im-squeck-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-05-23 18:14:11.000000 im-squeck-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:23.143401 im-squeck-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:23.147401 im-squeck-1.1.0/src/im_squeck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:14:22.000000 im-squeck-1.1.0/src/im_squeck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 18:14:23.000000 im-squeck-1.1.0/src/im_squeck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:23.147401 im-squeck-1.1.0/src/squeck/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 18:14:16.000000 im-squeck-1.1.0/src/squeck/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/squeck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:23.147401 im-squeck-1.1.0/src/squeck/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-23 18:14:11.000000 im-squeck-1.1.0/src/squeck/widgets/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:37.936191 im-squeck-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-08 09:22:23.000000 im-squeck-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-08 09:22:23.000000 im-squeck-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-08 09:22:37.936191 im-squeck-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-08 09:22:23.000000 im-squeck-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-08 09:22:23.000000 im-squeck-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-08 09:22:23.000000 im-squeck-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:22:37.936191 im-squeck-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-07-08 09:22:23.000000 im-squeck-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:37.928192 im-squeck-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:37.932191 im-squeck-1.1.1/src/im_squeck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 09:22:37.000000 im-squeck-1.1.1/src/im_squeck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:37.932191 im-squeck-1.1.1/src/squeck/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 09:22:28.000000 im-squeck-1.1.1/src/squeck/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/squeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:37.936191 im-squeck-1.1.1/src/squeck/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-08 09:22:23.000000 im-squeck-1.1.1/src/squeck/widgets/env.py
```

### Comparing `im-squeck-1.1.0/LICENSE` & `im-squeck-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/PKG-INFO` & `im-squeck-1.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squeck
-Version: 1.1.0
+Version: 1.1.1
 Summary: The IM Squonk2 Deck (Squeck)
 Home-page: https://github.com/informaticsmatters/squonk2-deck
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
@@ -38,14 +38,20 @@
 .. image:: docs/images/screenshot.png
 
 **Squeck** uses the `squonk2-python-client`_ to create a **Deck** displaying
 summary information for multiple Squonk2 environments and uses Will McGugan's
 `textual`_ framework to provide the user with a simple,
 text-based user interface modelled on the popular `k9s`_ Kubernetes monitor.
 
+It displays a summary of the environments, where: -
+
+- A green tick indicates that the authenticator service has issued a token for the service
+- The service version is displayed for those that are running
+- A **NO RESPONSE** banner is displayed for services that are not responding
+
 .. _k9s: https://k9scli.io
 .. _squonk2-python-client: https://github.com/InformaticsMatters/squonk2-python-client
 .. _textual: https://github.com/Textualize/textual
 
 ************
 Installation
 ************
```

### Comparing `im-squeck-1.1.0/README.rst` & `im-squeck-1.1.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 .. image:: docs/images/screenshot.png
 
 **Squeck** uses the `squonk2-python-client`_ to create a **Deck** displaying
 summary information for multiple Squonk2 environments and uses Will McGugan's
 `textual`_ framework to provide the user with a simple,
 text-based user interface modelled on the popular `k9s`_ Kubernetes monitor.
 
+It displays a summary of the environments, where: -
+
+- A green tick indicates that the authenticator service has issued a token for the service
+- The service version is displayed for those that are running
+- A **NO RESPONSE** banner is displayed for services that are not responding
+
 .. _k9s: https://k9scli.io
 .. _squonk2-python-client: https://github.com/InformaticsMatters/squonk2-python-client
 .. _textual: https://github.com/Textualize/textual
 
 ************
 Installation
 ************
```

### Comparing `im-squeck-1.1.0/setup.py` & `im-squeck-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/src/im_squeck.egg-info/PKG-INFO` & `im-squeck-1.1.1/src/im_squeck.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squeck
-Version: 1.1.0
+Version: 1.1.1
 Summary: The IM Squonk2 Deck (Squeck)
 Home-page: https://github.com/informaticsmatters/squonk2-deck
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
@@ -38,14 +38,20 @@
 .. image:: docs/images/screenshot.png
 
 **Squeck** uses the `squonk2-python-client`_ to create a **Deck** displaying
 summary information for multiple Squonk2 environments and uses Will McGugan's
 `textual`_ framework to provide the user with a simple,
 text-based user interface modelled on the popular `k9s`_ Kubernetes monitor.
 
+It displays a summary of the environments, where: -
+
+- A green tick indicates that the authenticator service has issued a token for the service
+- The service version is displayed for those that are running
+- A **NO RESPONSE** banner is displayed for services that are not responding
+
 .. _k9s: https://k9scli.io
 .. _squonk2-python-client: https://github.com/InformaticsMatters/squonk2-python-client
 .. _textual: https://github.com/Textualize/textual
 
 ************
 Installation
 ************
```

### Comparing `im-squeck-1.1.0/src/im_squeck.egg-info/SOURCES.txt` & `im-squeck-1.1.1/src/im_squeck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/src/squeck/access_token.py` & `im-squeck-1.1.1/src/squeck/access_token.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/src/squeck/common.py` & `im-squeck-1.1.1/src/squeck/common.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/src/squeck/squeck.py` & `im-squeck-1.1.1/src/squeck/squeck.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.1.0/src/squeck/widgets/env.py` & `im-squeck-1.1.1/src/squeck/widgets/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 _KEY_STYLE: Style = Style(color="orange_red1", bold=True)
 _KEY_VALUE_STYLE: Style = Style(color="bright_white")
 _VALUE_ERROR_STYLE: Style = Style(
     color="bright_yellow", bgcolor="bright_red", bold=True
 )
 
 _NO_RESPONSE_TEXT: str = "- NO RESPONSE -"
+_UI_HOSTNAME_POSTFIX: str = "/data-manager-ui"
 
 
 class EnvWidget(Widget):  # type: ignore
     """Displays the environment."""
 
     as_access_token: Optional[str] = None
     dm_access_token: Optional[str] = None
@@ -143,15 +144,17 @@
             else:
                 dm_hostname_text.append(common.CROSS)
         else:
             dm_hostname_text = Text("Undefined", style=_VALUE_ERROR_STYLE)
 
         ui_hostname: Optional[str] = self.environment.ui_hostname
         if ui_hostname:
-            ui_hostname_text: Text = Text(ui_hostname + " ", style=_KEY_VALUE_STYLE)
+            ui_hostname_text: Text = Text(
+                ui_hostname + _UI_HOSTNAME_POSTFIX + " ", style=_KEY_VALUE_STYLE
+            )
             if ui_api_version == _NO_RESPONSE_TEXT:
                 ui_hostname_text.append(common.CROSS)
             else:
                 ui_hostname_text.append(common.TICK)
         else:
             ui_hostname_text = Text("Undefined", style=_VALUE_ERROR_STYLE)
```

