# Comparing `tmp/hrequests-0.1.2.tar.gz` & `tmp/hrequests-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.1.2.tar", max compression
+gzip compressed data, was "hrequests-0.2.0.tar", max compression
```

## Comparing `hrequests-0.1.2.tar` & `hrequests-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      252 2023-07-07 02:29:04.973494 hrequests-0.1.2/hrequests/__init__.py
--rw-r--r--   0        0        0      141 2023-07-07 17:13:40.743171 hrequests-0.1.2/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.1.2/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.1.2/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    23319 2023-07-07 18:53:43.892054 hrequests-0.1.2/hrequests/browser.py
--rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.1.2/hrequests/cffi.py
--rw-r--r--   0        0        0    15818 2023-07-05 21:16:15.840628 hrequests-0.1.2/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.1.2/hrequests/cookies.py
--rw-r--r--   0        0        0      582 2023-07-07 01:06:44.367224 hrequests-0.1.2/hrequests/exceptions.py
--rw-r--r--   0        0        0    17506 2023-07-03 02:11:52.031572 hrequests-0.1.2/hrequests/parser.py
--rw-r--r--   0        0        0      372 2023-07-02 09:40:33.648986 hrequests-0.1.2/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.1.2/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.1.2/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2220 2023-07-07 17:33:52.582265 hrequests-0.1.2/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    13787 2023-06-17 22:56:39.628341 hrequests-0.1.2/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.1.2/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.1.2/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.1.2/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.1.2/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.1.2/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.1.2/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1951 2023-07-07 18:21:58.114844 hrequests-0.1.2/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-06-24 01:37:41.576954 hrequests-0.1.2/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    12333 2023-07-06 00:09:40.164591 hrequests-0.1.2/hrequests/reqs.py
--rw-r--r--   0        0        0     7505 2023-07-06 04:15:41.650723 hrequests-0.1.2/hrequests/response.py
--rw-r--r--   0        0        0     9576 2023-07-07 02:19:53.457218 hrequests-0.1.2/hrequests/session.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.1.2/LICENSE
--rw-r--r--   0        0        0     1022 2023-07-07 17:13:53.198053 hrequests-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    29663 2023-07-07 18:50:35.573726 hrequests-0.1.2/README.md
--rw-r--r--   0        0        0    30154 1970-01-01 00:00:00.000000 hrequests-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.2.0/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-08 02:07:11.575795 hrequests-0.2.0/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.2.0/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.2.0/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.2.0/hrequests/browser.py
+-rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.2.0/hrequests/cffi.py
+-rw-r--r--   0        0        0    15622 2023-07-08 00:43:33.012698 hrequests-0.2.0/hrequests/client.py
+-rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.2.0/hrequests/cookies.py
+-rw-r--r--   0        0        0      582 2023-07-07 01:06:44.367224 hrequests-0.2.0/hrequests/exceptions.py
+-rw-r--r--   0        0        0    17489 2023-07-08 03:00:50.611004 hrequests-0.2.0/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.2.0/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.2.0/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.2.0/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.2.0/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.2.0/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.2.0/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.2.0/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.2.0/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.2.0/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.2.0/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.2.0/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.2.0/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.2.0/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13464 2023-07-08 02:07:11.860477 hrequests-0.2.0/hrequests/reqs.py
+-rw-r--r--   0        0        0     7501 2023-07-08 02:07:11.851360 hrequests-0.2.0/hrequests/response.py
+-rw-r--r--   0        0        0    11715 2023-07-08 02:54:30.797972 hrequests-0.2.0/hrequests/session.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1022 2023-07-08 01:14:18.341560 hrequests-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    31376 2023-07-08 03:26:00.777238 hrequests-0.2.0/README.md
+-rw-r--r--   0        0        0    31848 1970-01-01 00:00:00.000000 hrequests-0.2.0/PKG-INFO
```

### Comparing `hrequests-0.1.2/hrequests/bin/LICENSE.txt` & `hrequests-0.2.0/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/browser.py` & `hrequests-0.2.0/hrequests/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,27 +81,23 @@
         self._in: Queue = Queue()
         # _out is for responses from the asyncio loop
         self._out: Queue = Queue()
         # remember session and resp to clone cookies back to when closing
         self.session: Optional[hrequests.session.TLSSession] = session
         self.resp: Optional[hrequests.response.Response] = resp
         # generating headers
-        if browser or os:
-            # if a browser or os was provided, generate a user-agent and IGNORE session/resp headers
-            # only meant to be used when using BrowserSession as a standalone
-            self.browser: str = browser or choice(('firefox', 'chrome', 'opera'))
-            self.ua: str = Headers(browser=self.browser, os=os).generate()['User-Agent']
-        elif session:
+        if session:
             # if a session was provided, use the session user-agent
             self.browser: str = session.browser
             self.ua: str = session.headers.get('User-Agent')
         else:
-            # else if nothing else was provided, generate a firefox user-agent
-            self.browser: str = 'firefox'
-            self.ua: str = Headers(browser='firefox').generate()['User-Agent']
+            # if a browser or os was provided, generate a user-agent and IGNORE session/resp headers
+            # only meant to be used when using BrowserSession as a standalone
+            self.browser: str = browser or choice(('firefox', 'chrome', 'opera'))
+            self.ua: str = Headers(browser=self.browser, os=os).generate()['User-Agent']
         # proxy variables
         self.proxy_ip: Optional[str] = proxy_ip
         # browser config
         self.mock_human: bool = mock_human
         self.headless: bool = headless
         # bool to indicate browser was closed
         self._closed: bool = False
@@ -239,48 +235,50 @@
             timeout (float, optional): Timeout in seconds. Defaults to 30.
         '''
         return await self.page.wait_for_function(
             "selector => !!document.querySelector(selector)",
             arg=selector,
             timeout=int(timeout * 1e3),
         )
-    
+
     async def _awaitEnabled(self, selector, *, timeout: float = 30):
         '''
         Wait for a selector to be enabled
 
         Parameters:
             selector (str): Selector to wait for
             timeout (float, optional): Timeout in seconds. Defaults to 30.
         '''
         return await self.page.wait_for_function(
             "selector => !document.querySelector(selector).disabled",
             arg=selector,
             timeout=int(timeout * 1e3),
         )
-    
+
     async def _isVisible(self, selector: str) -> bool:
         '''
         Check if a selector is visible
 
         Parameters:
             selector (str): Selector to check
         '''
         return await self.page.is_visible(selector)
 
     async def _isEnabled(self, selector: str) -> bool:
         '''
         Check if a selector is enabled
-        
+
         Parameters:
             selector (str): Selector to check
         '''
         if not await self.page.is_visible(selector):
             return False
-        return await self.page.evaluate("selector => !document.querySelector(selector).disabled", arg=selector)
+        return await self.page.evaluate(
+            "selector => !document.querySelector(selector).disabled", arg=selector
+        )
 
     async def _awaitUrl(
         self, url: Union[str, Pattern[str], Callable[[str], bool]], *, timeout: float = 30
     ):
         '''
         Wait for the url to match a string, regex, or a python function to return True
 
@@ -309,15 +307,15 @@
             wait_after (bool, optional): Wait for a page event before continuing. Defaults to False.
             check (bool, optional): Check if an element is draggable before running. Defaults to False.
         '''
         return await self.page.drag_and_drop(
             source, target, no_wait_after=not wait_after, timeout=int(timeout * 1e3), check=check
         )
 
-    async def _type(self, selector: str, text: str, delay: int=50, *, timeout: float = 30):
+    async def _type(self, selector: str, text: str, delay: int = 50, *, timeout: float = 30):
         '''
         Type text into a selector
 
         Parameters:
             selector (str): CSS selector to type in
             text (str): Text to type
             delay (int, optional): Delay between keypresses in ms. On mock_human, this is randomized by 50%. Defaults to 50.
```

### Comparing `hrequests-0.1.2/hrequests/cffi.py` & `hrequests-0.2.0/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/client.py` & `hrequests-0.2.0/hrequests/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,14 @@
         # Example:
         # {
         #     "http": "http://user:pass@ip:port",
         #     "https": "http://user:pass@ip:port"
         # }
         self.proxies: dict = {}
 
-        # Dictionary of querystring data to attach to each request. The dictionary values may be lists for representing
-        # multivalued query parameters.
-        self.params: dict = {}
-
         # CookieJar containing all currently outstanding cookies set on this session
         self.cookies: RequestsCookieJar = RequestsCookieJar()
 
         # - Advanced Settings
 
         # Examples:
         # Chrome > chrome_103, chrome_104, chrome_105, chrome_106
@@ -290,19 +286,19 @@
         # Prepare URL - add params to url
         if params is not None:
             url = f'{url}?{urllib.parse.urlencode(params, doseq=True)}'
 
         # Prepare request body - build request body
         # Data has priority. JSON is only used if data is None.
         if data is None and json is not None:
-            if type(json) in [dict, list]:
+            if type(json) in (dict, list):
                 json = dumps(json).decode('utf-8')
             request_body = json
             content_type = 'application/json'
-        elif data is not None and type(data) not in [str, bytes]:
+        elif data is not None and type(data) not in (str, bytes):
             request_body = urllib.parse.urlencode(data, doseq=True)
             content_type = 'application/x-www-form-urlencoded'
         else:
             request_body = data
             content_type = None
         # set content type if it isn't set
         if content_type is not None and 'content-type' not in self.headers:
```

### Comparing `hrequests-0.1.2/hrequests/cookies.py` & `hrequests-0.2.0/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/exceptions.py` & `hrequests-0.2.0/hrequests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/parser.py` & `hrequests-0.2.0/hrequests/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import contextlib
-from typing import List, MutableMapping, Set, Union
+from typing import List, MutableMapping, Optional, Set, Union
 from urllib.parse import urljoin, urlparse, urlunparse
 
 import lxml
 from lxml import etree
 from lxml.html import HtmlElement
 from lxml.html import tostring as lxml_html_tostring
 from lxml.html.clean import Cleaner
@@ -433,18 +433,15 @@
     Attributes:
         session (Union[hrequests.session.TLSSession, hrequests.browser.BrowserSession]): The session used for the HTML request.
     """
 
     def __init__(
         self,
         *,
-        session: Union[
-            hrequests.session.TLSSession,
-            hrequests.browser.BrowserSession
-        ] = None,
+        session: Optional[Union[hrequests.session.TLSSession, hrequests.browser.BrowserSession]] = None,
         url: str = DEFAULT_URL,
         html: _HTML,
         default_encoding: str = DEFAULT_ENCODING,
     ) -> None:
         # Convert incoming unicode HTML into bytes.
         if isinstance(html, str):
             html = html.encode(DEFAULT_ENCODING)
```

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/context.py` & `hrequests-0.2.0/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/element_handle.py` & `hrequests-0.2.0/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/faker.py` & `hrequests-0.2.0/hrequests/playwright_mock/faker.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,14 @@
             self.height: int = 720
             self.avail_width: int = 1280
             self.avail_height: int = 720
 
     async def locale(self, proxy) -> None:
         with open(join(dirname(__file__), "locale.json"), "r") as f:
             language_dict = json.load(f)
-            
+
         country_code = proxy.country_code
 
         if country_code in language_dict:
             self.locale, self.language_code = language_dict[country_code]
         else:
             raise ValueError("Proxy Country not supported")
```

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/frame.py` & `hrequests-0.2.0/hrequests/playwright_mock/locator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,299 +1,404 @@
 import typing
 
-from . import element_handle, frame_locator, js_handle, locator
+from . import element_handle, frame, frame_locator, js_handle
 
 
-def mock_frame(frame) -> None:
-    if not frame:
-        return
+def attach_dyn_propr(instance, prop_name, propr):
+    """Attach property proper to instance with name prop_name.
 
-    async def click_mocker(selector, button="left", click_count=1, strict=False, delay=20, force=False, modifiers=[], no_wait_after=False, position={}, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.click(frame, selector, button=button, click_count=click_count, strict=strict, delay=delay, force=force, modifiers=modifiers, no_wait_after=no_wait_after, position=position, timeout=timeout, trial=trial)
+    Reference:
+      * https://stackoverflow.com/a/1355444/509706
+      * https://stackoverflow.com/questions/48448074
+    """
+    class_name = instance.__class__.__name__ + "Child"
+    child_class = type(class_name, (instance.__class__,), {prop_name: propr})
+
+    instance.__class__ = child_class
+
+
+def mock_locator(locator) -> None:
+    async def click_mocker(
+        button="left",
+        click_count=1,
+        delay=20,
+        force=False,
+        modifiers=[],
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ):
+        await Locator.click(
+            locator,
+            button=button,
+            click_count=click_count,
+            delay=delay,
+            force=force,
+            modifiers=modifiers,
+            no_wait_after=no_wait_after,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.click = click_mocker
+
+    async def dblclick_mocker(
+        button="left",
+        delay=20,
+        force=False,
+        modifiers=[],
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ):
+        await Locator.dblclick(
+            locator,
+            button=button,
+            delay=delay,
+            force=force,
+            modifiers=modifiers,
+            no_wait_after=no_wait_after,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.dblclick = dblclick_mocker
+
+    async def check_mocker(
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ):
+        await Locator.check(
+            locator,
+            force=force,
+            no_wait_after=no_wait_after,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.check = check_mocker
+
+    async def uncheck_mocker(
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ):
+        await Locator.uncheck(
+            locator,
+            force=force,
+            no_wait_after=no_wait_after,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.uncheck = uncheck_mocker
+
+    async def set_checked_mocker(
+        checked=False,
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ):
+        await Locator.set_checked(
+            locator,
+            checked=checked,
+            force=force,
+            no_wait_after=no_wait_after,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.set_checked = set_checked_mocker
+
+    async def hover_mocker(
+        force=False, modifiers=[], position={}, timeout: typing.Optional[float] = None, trial=False
+    ):
+        await Locator.hover(
+            locator,
+            force=force,
+            modifiers=modifiers,
+            position=position,
+            timeout=timeout,
+            trial=trial,
+        )
+
+    locator.hover = hover_mocker
+
+    async def type_mocker(
+        text, delay=200, no_wait_after=False, timeout: typing.Optional[float] = None
+    ):
+        await Locator.type(locator, text, delay=delay, no_wait_after=no_wait_after, timeout=timeout)
 
-    frame.click = click_mocker
-
-    async def dblclick_mocker(selector, button="left", strict=False, delay=20, force=False, modifiers=[], no_wait_after=False, position={}, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.dblclick(frame, selector, button=button, strict=strict, delay=delay, force=force, modifiers=modifiers, no_wait_after=no_wait_after, position=position, timeout=timeout, trial=trial)
-
-    frame.dblclick = dblclick_mocker
-
-    async def check_mocker(selector, force=False, no_wait_after=False, position={}, strict=False, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.check(frame, selector, force=force, no_wait_after=no_wait_after, position=position, strict=strict, timeout=timeout, trial=trial)
-
-    frame.check = check_mocker
-
-    async def uncheck_mocker(selector, force=False, no_wait_after=False, position={}, strict=False, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.uncheck(frame, selector, force=force, no_wait_after=no_wait_after, position=position, strict=strict, timeout=timeout, trial=trial)
-
-    frame.uncheck = uncheck_mocker
-
-    async def set_checked_mocker(selector, checked=False, force=False, no_wait_after=False, position={}, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.set_checked(frame, selector, checked=checked, force=force, no_wait_after=no_wait_after, position=position, timeout=timeout, trial=trial)
-
-    frame.set_checked = set_checked_mocker
-
-    async def hover_mocker(selector, force=False, modifiers=[], position={}, strict=False, timeout: typing.Optional[float] = None, trial=False):
-        await Frame.hover(frame, selector, force=force, modifiers=modifiers, position=position, strict=strict, timeout=timeout, trial=trial)
-
-    frame.hover = hover_mocker
-
-    async def type_mocker(selector, text, delay=200, no_wait_after=False, strict=False, timeout: typing.Optional[float] = None):
-        await Frame.type(frame, selector, text, delay=delay, no_wait_after=no_wait_after, strict=strict, timeout=timeout)
-
-    frame.type = type_mocker
-
-    for frame in frame.child_frames:
-        mock_frame(frame)
-
-    # ElementHandle
-    async def mock_query_selector(selector, strict=False) -> typing.Optional["ElementHandle"]:
-        element = await frame._query_selector(selector, strict=strict)
-        if element:
-            await element_handle.mock_element_handle(element, frame.page)
-        return element
-
-    frame._query_selector = frame.query_selector
-    frame.query_selector = mock_query_selector
-
-    async def mock_query_selector_all(selector) -> typing.List["ElementHandle"]:
-        elements = await frame._query_selector_all(selector)
-        for element in elements:
-            await element_handle.mock_element_handle(element, frame.page)
-        return elements
-
-    frame._query_selector_all = frame.query_selector_all
-    frame.query_selector_all = mock_query_selector_all
-
-    async def mock_wait_for_selector(selector, state=[], strict=False, timeout: typing.Optional[float] = None) -> typing.Optional["ElementHandle"]:
-        element = await frame.__wait_for_selector(selector, state=state, strict=strict, timeout=timeout)
-        if element:
-            await element_handle.mock_element_handle(element, frame.page)
-        return element
-
-    frame.__wait_for_selector = frame.wait_for_selector
-    frame.wait_for_selector = mock_wait_for_selector
-
-    async def mock_add_script_tag(content="", path="", type="", url="") -> "ElementHandle":
-        element = await frame._add_script_tag(content=content, path=path, type=type, url=url)
-        await element_handle.mock_element_handle(element, frame.page)
-        return element
-
-    frame._add_script_tag = frame.add_script_tag
-    frame.add_script_tag = mock_add_script_tag
-
-    async def mock_add_style_tag(content="", path="", type="", url="") -> "ElementHandle":
-        element = await frame._add_script_tag(content=content, path=path, type=type, url=url)
-        await element_handle.mock_element_handle(element, frame.page)
-        return element
-
-    frame._add_script_tag = frame.add_script_tag
-    frame.add_script_tag = mock_add_style_tag
-
-    async def frame_element() -> "ElementHandle":
-        element = await frame._frame_element()
-        await element_handle.mock_element_handle(element, frame.page)
-        return element
-
-    frame._frame_element = frame.frame_element
-    frame.frame_element = frame_element
+    locator.type = type_mocker
 
     # JsHandle
     async def mock_evaluate_handle(expression, arg=None) -> "JSHandle":
-        _js_handle = await frame._evaluate_handle(expression, arg=arg)
-        await js_handle.mock_js_handle(_js_handle, frame.page)
-        return _js_handle
-
-    frame._evaluate_handle = frame.evaluate_handle
-    frame.evaluate_handle = mock_evaluate_handle
-
-    async def mock_wait_for_function(expression, arg=None, polling="raf", timeout: typing.Optional[float] = None) -> "JSHandle":
-        _js_handle = await frame._wait_for_function(expression, arg=arg, polling=polling, timeout=timeout)
-        await js_handle.mock_js_handle(_js_handle, frame.page)
+        _js_handle = await locator._evaluate_handle(expression, arg=arg)
+        await js_handle.mock_js_handle(_js_handle, locator.page)
         return _js_handle
 
-    frame._wait_for_function = frame.wait_for_function
-    frame.wait_for_function = mock_wait_for_function
+    locator._evaluate_handle = locator.evaluate_handle
+    locator.evaluate_handle = mock_evaluate_handle
 
     # FrameLocator
-    async def frame_locator_mocker(selector) -> "JSHandle":
-        _frame_locator = await frame._frame_locator(selector)
+    async def mock_frame_locator_func(selector) -> "JSHandle":
+        _frame_locator = await locator._frame_locator(selector)
         await frame_locator.mock_frame_locator(_frame_locator)
         return _frame_locator
 
-    frame._frame_locator = frame.frame_locator
-    frame.frame_locator = frame_locator_mocker
+    locator._frame_locator = locator.frame_locator
+    locator.frame_locator = mock_frame_locator_func
+
+    # ElementHandle
+    def element_handle_mocker(timeout: typing.Optional[float] = None):
+        element = locator._element_handle(timeout=timeout)
+        element_handle.mock_element_handle(element, locator.page)
+        return element
+
+    locator._element_handle = locator.element_handle
+    locator.element_handle = element_handle_mocker
 
     # Locator
-    async def locator_mocker(selector, has=None, has_text="") -> "JSHandle":
-        _locator = await frame._locator(selector, has=has, has_text=has_text)
-        locator.mock_locator(_locator)
+    def nth_mocker(index):
+        _locator = locator._nth(index)
+        mock_locator(_locator)
         return _locator
 
-    frame._locator = frame.locator
-    frame.locator = locator_mocker
+    locator._nth = locator.nth
+    locator.nth = nth_mocker
 
+    @property
+    def first_mocker(self):
+        _locator = locator._first
+        mock_locator(_locator)
+        return _locator
+
+    @property
+    def last_mocker(self):
+        _locator = locator._last
+        mock_locator(_locator)
+        return _locator
 
-class Frame:
-    async def click(frame, selector, button="left", click_count=1, strict=False, delay=20, force=False, modifiers=[], no_wait_after=False, position={}, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+    locator._first = locator.first
+    locator._last = locator.last
 
+    attach_dyn_propr(locator, "first", first_mocker)
+    attach_dyn_propr(locator, "last", last_mocker)
+
+
+class Locator:
+    async def click(
+        locator,
+        button="left",
+        click_count=1,
+        delay=20,
+        force=False,
+        modifiers=[],
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
+
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
             for modifier in modifiers:
-                await frame.page.keyboard.down(modifier)
+                await locator.page.keyboard.down(modifier)
 
-            await frame.page.mouse.click(x, y, button, click_count, delay)
+            await locator.page.mouse.click(x, y, button, click_count, delay)
 
             for modifier in modifiers:
-                await frame.page.keyboard.up(modifier)
-
-    async def dblclick(frame, selector, button="left", strict=False, delay=20, force=False, modifiers=[], no_wait_after=False, position={}, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+                await locator.page.keyboard.up(modifier)
 
+    async def dblclick(
+        locator,
+        button="left",
+        delay=20,
+        force=False,
+        modifiers=[],
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
             for modifier in modifiers:
-                await frame.page.keyboard.down(modifier)
+                await locator.page.keyboard.down(modifier)
 
-            await frame.page.mouse.dblclick(x, y, button, delay)
+            await locator.page.mouse.dblclick(x, y, button, delay)
 
             for modifier in modifiers:
-                await frame.page.keyboard.up(modifier)
-
-    async def check(frame, selector, force=False, no_wait_after=False, position={}, strict=False, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+                await locator.page.keyboard.up(modifier)
 
+    async def check(
+        locator,
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
-        if await element.is_checked():
+        if await locator.is_checked():
             return
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
-            await frame.page.mouse.click(x, y, button="left", click_count=1, delay=20)
-
-            assert await element.is_checked()
+            await locator.page.mouse.click(x, y, button="left", click_count=1, delay=20)
 
-    async def uncheck(frame, selector, force=False, no_wait_after=False, position={}, strict=False, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+            assert await locator.is_checked()
 
+    async def uncheck(
+        locator,
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
-        if not await element.is_checked():
+        if not await locator.is_checked():
             return
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
-            await frame.page.mouse.click(x, y, button="left", click_count=1, delay=20)
+            await locator.page.mouse.click(x, y, button="left", click_count=1, delay=20)
 
-            assert not await element.is_checked()
-
-    async def set_checked(frame, selector, checked=False, force=False, no_wait_after=False, position={}, strict=False, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+            assert not await locator.is_checked()
 
+    async def set_checked(
+        locator,
+        checked=False,
+        force=False,
+        no_wait_after=False,
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
-        if await element.is_checked() == checked:
+        if await locator.is_checked() == checked:
             return
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
-            await frame.page.mouse.click(x, y, button="left", click_count=1, delay=20)
-
-            assert await element.is_checked()
+            await locator.page.mouse.click(x, y, button="left", click_count=1, delay=20)
 
-    async def hover(frame, selector, force=False, modifiers=[], position={}, strict=False, timeout: typing.Optional[float] = None, trial=False) -> None:
-        element = await frame.wait_for_selector(selector, state="visible" if not force else "hidden", strict=strict, timeout=timeout)
+            assert await locator.is_checked()
 
+    async def hover(
+        locator,
+        force=False,
+        modifiers=[],
+        position={},
+        timeout: typing.Optional[float] = None,
+        trial=False,
+    ) -> None:
         if not force:
-            await element.wait_for_element_state("editable", timeout=timeout)
+            await locator.wait_for(state="visible", timeout=timeout)
 
         if not trial:
-            if frame.page.scroll_into_view:
+            if locator.page.scroll_into_view:
                 await locator.scroll_into_view_if_needed(timeout=timeout)
 
-            boundings = await element.bounding_box()
+            boundings = await locator.bounding_box()
             x, y, width, height = boundings.values()
             if not position:
                 x, y = x + width // 2, y + height // 2
             else:
                 x, y = x + position["x"], y + position["y"]
 
             for modifier in modifiers:
-                await frame.page.keyboard.down(modifier)
+                await locator.page.keyboard.down(modifier)
 
-            await frame.page.mouse.move(x, y)
+            await locator.page.mouse.move(x, y)
 
             for modifier in modifiers:
-                await frame.page.keyboard.up(modifier)
-
-    async def type(frame, selector, text, delay=200, no_wait_after=False, strict=False, timeout: typing.Optional[float] = None) -> None:
-        element = await frame.wait_for_selector(selector, state="visible", strict=strict, timeout=timeout)
+                await locator.page.keyboard.up(modifier)
 
-        await element.wait_for_element_state("editable", timeout=timeout)
+    async def type(
+        locator, text, delay=200, no_wait_after=False, timeout: typing.Optional[float] = None
+    ) -> None:
+        await locator.wait_for(state="visible", timeout=timeout)
 
-        if frame.page.scroll_into_view:
+        if locator.page.scroll_into_view:
             await locator.scroll_into_view_if_needed(timeout=timeout)
 
-        boundings = await element.bounding_box()
+        boundings = await locator.bounding_box()
         x, y, width, height = boundings.values()
 
         x, y = x + width // 2, y + height // 2
 
-        await frame.page.mouse.click(x, y, "left", 1, delay)
+        await locator.page.mouse.click(x, y, "left", 1, delay)
 
-        await frame.page.keyboard.type(text, delay=delay)
+        await locator.page.keyboard.type(text, delay=delay)
```

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.2.0/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/locale.json` & `hrequests-0.2.0/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/mouse.py` & `hrequests-0.2.0/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/page.py` & `hrequests-0.2.0/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.2.0/hrequests/playwright_mock/playwright_mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,51 +6,43 @@
 class PlaywrightMock(AsyncObject):
     async def __ainit__(self, headless=False, scroll_into_view=True):
         # setting values
         self.scroll_into_view = scroll_into_view
         # starting Playwright
         self.playwright = await async_playwright().start()
         # launching chromium
-        self.main_browser = await self.launch_browser(
-            client=self.playwright,
-            headless=headless
-        )
-    
+        self.main_browser = await self.launch_browser(client=self.playwright, headless=headless)
+
     args = [
         '--disable-blink-features=AutomationControlled',
         '--disable-web-security',
         '--disable-site-isolation-trials',
         '--disable-features=CrossSiteDocumentBlockingIfIsolating,'
-            'CrossSiteDocumentBlockingAlways,'
-            'IsolateOrigins,'
-            'site-per-process,'
-            'SharedArrayBuffer',
+        'CrossSiteDocumentBlockingAlways,'
+        'IsolateOrigins,'
+        'site-per-process,'
+        'SharedArrayBuffer',
     ]
-    
+
     @staticmethod
     async def launch_browser(client, headless=False):
         return await client.chromium.launch(
             headless=headless,
             args=PlaywrightMock.args + (['--headless=new'] if headless else []),
         )
-    
+
     async def stop(self):
         await self.main_browser.close()
         await self.playwright.stop()
 
     async def new_context(self, browser_name: str, user_agent: str, proxy=None, **launch_args):
         # calling proxyManager and faker
         _proxy = await ProxyManager(self, proxy)
         _faker = await Faker(self, _proxy, browser_name, user_agent)
         # create context with human emulation
         _browser = await context.new_context(
-            self,
-            _proxy,
-            _faker,
-            bypass_csp=True,
-            user_agent=user_agent,
-            **launch_args
+            self, _proxy, _faker, bypass_csp=True, user_agent=user_agent, **launch_args
         )
         _browser.proxy = _proxy
         _browser.faker = _faker
 
-        return _browser
+        return _browser
```

### Comparing `hrequests-0.1.2/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.2.0/hrequests/playwright_mock/proxy_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,20 @@
         elif len(splitted) == 4:
             self.split_helper(splitted)
         else:
             raise SplitError(f"Proxy Format ({self.proxy}) isnt supported")
 
     async def check_proxy(self) -> None:
         try:
-            ip_request = await self.phttpx.get("https://api.ipify.org?format=json", timeout=self.timeout)
+            ip_request = await self.phttpx.get(
+                "https://api.ipify.org?format=json", timeout=self.timeout
+            )
             ip = ip_request.json().get("ip")
         except Exception:
-            raise ProxyCheckError(
-                "Could not get IP-Address of Proxy (Proxy is Invalid/Timed Out)"
-            )
+            raise ProxyCheckError("Could not get IP-Address of Proxy (Proxy is Invalid/Timed Out)")
         try:
             r = await self.httpx.get(f"http://ip-api.com/json/{ip}", timeout=self.timeout)
             data = r.json()
             self.country = data.get("country")
             self.country_code = data.get("countryCode")
             self.region = data.get("regionName")
             self.city = data.get("city")
```

### Comparing `hrequests-0.1.2/hrequests/reqs.py` & `hrequests-0.2.0/hrequests/reqs.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,42 +32,73 @@
 
     Methods:
         send(**kwargs): Prepares request based on parameter passed to constructor and optional ``kwargs```.
                         Then sends request and saves response to :attr:`response`.
                         Returns: ``Response``.
     '''
 
+    session_kwargs = {
+        'browser',
+        'version',
+        'headers',
+        'os',
+        'ja3_string',
+        'h2_settings',
+        'additional_decode',
+        'pseudo_header_order',
+        'priority_frames',
+        'header_order',
+        'force_http1',
+        'catch_panics',
+        'debug',
+    }
+
     def __init__(
         self,
         method: str,
         url: str,
         session: Optional['hrequests.session.TLSSession'] = None,
         raise_exception: bool = True,
         **kwargs,
     ):
         # Request method
-        self.method = method
+        self.method: str = method
         # Raise exceptions (default FALSE for async, TRUE for sync)
-        self.raise_exception = raise_exception
+        self.raise_exception: bool = raise_exception
         # URL to request
-        self.url = url
-        # Create TLSSession if not provided
-        self._build_session(session)
+        self.url: str = url
+
+        # Session kwargs
+        self.sess_kwargs: dict | None = None
+        if kwargs:
+            sess_kwargs = set(kwargs.keys()) & TLSRequest.session_kwargs
+            if session and sess_kwargs:
+                # If session is already provided, raise TypeError if session-only kwargs are passed
+                raise TypeError(f'Cannot pass parameter(s) to an existing session: {sess_kwargs}')
+            else:
+                self.sess_kwargs = {k: kwargs.pop(k) for k in sess_kwargs}
 
         if callback := kwargs.pop('callback', None):
             kwargs['hooks'] = {'response': callback}
 
-        # The rest arguments for ``Session.request``
+        # The rest of the arguments for `Session.request`
         self.kwargs = kwargs
-        # Resulting ``Response``
+        # Resulting Response
         self.response = None
+        # Create TLSSession if not provided
+        self._build_session(session)
 
     def _build_session(self, session=None):
         if session is None:
-            self.session = hrequests.firefox.Session(temp=True)
+            if self.sess_kwargs:
+                # if session kwargs are passed, configure a new session with them
+                self.session = hrequests.Session(temp=True, **self.sess_kwargs)
+            else:
+                # else use a preconfigured session
+                self.session = hrequests.chrome.Session(temp=True)
             self._close = True
         else:
             # don't close adapters after each request if the user provided the session
             self.session = session
             self._close = False
 
     def send(self, **kwargs):
```

### Comparing `hrequests-0.1.2/hrequests/response.py` & `hrequests-0.2.0/hrequests/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     url: str
     status_code: int
     headers: 'hrequests.client.CaseInsensitiveDict'
     cookies: RequestsCookieJar
     _text: Optional[str] = None
     _content: Optional[Union[str, bytes]] = None
-    
+
     # set by ProcessResponse
     history: Optional[List['Response']] = None
     session: Optional[
         Union['hrequests.session.TLSSession', 'hrequests.browser.BrowserSession']
     ] = None
     elapsed: timedelta | None = None
```

### Comparing `hrequests-0.1.2/hrequests/session.py` & `hrequests-0.2.0/hrequests/session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import partial
 from random import choice as rchoice
-from typing import Literal, Optional, Union
+from typing import Literal, Optional, Tuple, Union
 
 from fake_headers import Headers
 
 import hrequests
 from hrequests.reqs import *
 from hrequests.response import ProcessResponse
 
@@ -16,105 +16,116 @@
 class TLSSession(TLSClient):
     """
     Session object that sends requests with TLS client.
 
     Args:
         browser (str): Browser to use [firefox, chrome, opera]
         client_identifier (str): Identifier for the client
-        os (str): OS to use in header [win, mac, lin]
+        os (Literal['win', 'mac', 'lin'], optional): OS to use in header [win, mac, lin]
         headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
         temp (bool, optional): Indicates if session is temporary. Defaults to False.
         verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
         ja3_string (str, optional): JA3 string. Defaults to None.
         h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
         additional_decode (str, optional): Additional decode. Defaults to None.
         pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
         priority_frames (list, optional): Priority frames. Defaults to None.
         header_order (list, optional): Header order. Defaults to None.
         force_http1 (bool, optional): Force HTTP/1. Defaults to False.
         catch_panics (bool, optional): Catch panics. Defaults to False.
         debug (bool, optional): Debug mode. Defaults to False.
-    
+
     Methods:
-        get(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        get(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a GET request
-        post(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        post(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a POST request
-        options(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        options(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a OPTIONS request
-        head(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        head(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a HEAD request
-        put(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        put(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a PUT request
-        patch(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        patch(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a PATCH request
-        delete(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None): 
+        delete(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a DELETE request
-        render(url, headless, proxy, response, mock_human): 
+        render(url, headless, proxy, response, mock_human):
             Render a page with playwright
     """
+
     def __init__(
         self,
-        browser: str,
         client_identifier: str,
-        os: str,
+        browser: Literal['firefox', 'chrome', 'opera'],
+        os: Optional[Literal['win', 'mac', 'lin']] = None,
         headers: Optional[dict] = None,
         temp: bool = False,
         verify: bool = True,
         *args,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(client_identifier=client_identifier, *args, **kwargs)
 
         # sync network methods
         self.get: partial = partial(get, session=self)
         self.post: partial = partial(post, session=self)
         self.options: partial = partial(options, session=self)
         self.head: partial = partial(head, session=self)
         self.put: partial = partial(put, session=self)
         self.patch: partial = partial(patch, session=self)
         self.delete: partial = partial(delete, session=self)
-        
+
         # async network methods
         self.async_get: partial = partial(async_get, session=self)
         self.async_post: partial = partial(async_post, session=self)
         self.async_options: partial = partial(async_options, session=self)
         self.async_head: partial = partial(async_head, session=self)
         self.async_put: partial = partial(async_put, session=self)
         self.async_patch: partial = partial(async_patch, session=self)
         self.async_delete: partial = partial(async_delete, session=self)
-        
+
         # shortcut to render method
         self.render: partial = partial(hrequests.browser.render, session=self)
 
         self.temp: bool = temp  # indicate if session is temporary
         self._closed: bool = False  # indicate if session is closed
         self.browser: str = browser  # browser name
-        self.os: str = os  # os name
+        self._os: str = os or rchoice(('win', 'mac', 'lin'))  # os name
         self.verify: bool = verify  # default to verifying certs
 
         # set headers
         if headers:
             self.headers = CaseInsensitiveDict(headers)
         else:
             self.resetHeaders(os=os)
 
     def resetHeaders(
         self,
-        os: Optional[Literal['random', 'win', 'mac', 'lin']] = None,
+        os: Optional[Literal['win', 'mac', 'lin']] = None,
     ):
         """
         Rotates the headers of the session
         "OS" can be one of the following:
-          'random', 'win', 'mac', 'lin'
+          ['win', 'mac', 'lin']
         Default is what it was initialized with, or the last value set
         """
         if os:
-            self.os = os
-        self.headers = Headers(browser=self.browser, os=os or self.os, headers=True).generate()
+            self._os = os
+        self.headers = Headers(browser=self.browser, os=self._os, headers=True).generate()
+
+    @property
+    def os(self) -> str:
+        return self._os
+
+    @os.setter
+    def os(self, os: Literal['win', 'mac', 'lin']):
+        if os not in _os_set:
+            raise ValueError(f'`{os}` is not a valid OS: (win, mac, lin)')
+        self.resetHeaders(os=os)
 
     def request(
         self,
         method: str,
         url: str,
         *,
         params: Optional[dict] = None,
@@ -163,83 +174,113 @@
             chain=history,
             insecure_skip_verify=not verify,
             timeout_seconds=timeout,
             proxy=proxies,
         )
         proc.send()
         return proc.response
-    
+
     def close(self):
         if not self._closed:
             self._closed = True
             freeMemory(self._session_id.encode('utf-8'))
-    
+
     def __enter__(self):
         return self
-    
+
     def __exit__(self, *_):
         self.close()
 
     def __del__(self):
         self.close()
 
 
 class Session(TLSSession):
     def __init__(
         self,
         browser: Literal['firefox', 'chrome', 'opera'] = 'firefox',
-        client_identifier: Optional[str] = None,
-        os: Literal['random', 'win', 'mac', 'lin'] = 'random',
+        version: Optional[int] = None,
+        os: Optional[Literal['win', 'mac', 'lin']] = None,
         headers: Optional[dict] = None,
         *args,
-        **kwargs
+        **kwargs,
     ):
+        '''
+        Parameters:
+            browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+            version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
+            os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
+            headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
+            verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+            ja3_string (str, optional): JA3 string. Defaults to None.
+            h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
+            additional_decode (str, optional): Additional decode. Defaults to None.
+            pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
+            priority_frames (list, optional): Priority frames. Defaults to None.
+            header_order (list, optional): Header order. Defaults to None.
+            force_http1 (bool, optional): Force HTTP/1. Defaults to False.
+            catch_panics (bool, optional): Catch panics. Defaults to False.
+            debug (bool, optional): Debug mode. Defaults to False.
+        '''
+        # random version if not specified
+        if not version:
+            version = _browsers[browser].version
+        # if version is specified, check if it is supported
+        elif version not in _browsers[browser].versions:
+            raise ValueError(
+                f'`{version}` is not a supported {browser} version: {_browsers[browser].versions}'
+            )
+        self.version = version
+
         super().__init__(
-            client_identifier=client_identifier or firefox.tls,
+            client_identifier=f'{browser}_{version}',
             browser=browser,
             headers=headers,
             os=os,
             *args,
-            **kwargs
+            **kwargs,
         )
 
 
 class SessionShortcut:
     name: str
-    tls_clients: tuple
-    
+    versions: Tuple[int]
+
     @classmethod
     @property
-    def tls(cls) -> str:
-        return rchoice(cls.tls_clients)
-    
+    def version(cls) -> int:
+        return rchoice(cls.versions)
+
     @classmethod
-    def Session(cls, os='random', *args, **kwargs) -> Session:
+    def Session(
+        cls,
+        version: Optional[int] = None,
+        os: Optional[Literal['win', 'mac', 'lin']] = None,
+        *args,
+        **kwargs,
+    ) -> Session:
         return Session(
-            browser=cls.name, client_identifier=cls.tls, os=os, *args, **kwargs
+            browser=cls.name,
+            version=version or cls.version,
+            os=os,
+            *args,
+            **kwargs,
         )
 
 
 class firefox(SessionShortcut):
     name: str = 'firefox'
-    tls_clients: tuple = ('firefox_102', 'firefox_104', 'firefox108', 'firefox110')
+    versions: Tuple[int] = (102, 104, 105, 106, 108, 110)
 
 
 class chrome(SessionShortcut):
     name: str = 'chrome'
-    tls_clients: tuple = (
-        'chrome_103',
-        'chrome_104',
-        'chrome_105',
-        'chrome_106',
-        'chrome_107',
-        'chrome_108',
-        'chrome109',
-        'chrome110',
-        'chrome111',
-        'chrome112',
-    )
+    versions: Tuple[int] = (103, 104, 105, 106, 107, 108, 109, 110, 111, 112)
 
 
 class opera(SessionShortcut):
     name: str = 'opera'
-    tls_clients: tuple = ('opera_89', 'opera_90')
+    versions: Tuple[int] = (89, 90)
+
+
+_browsers = {'firefox': firefox, 'chrome': chrome, 'opera': opera}
+_os_set = {'win', 'mac', 'lin'}
```

### Comparing `hrequests-0.1.2/LICENSE` & `hrequests-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.2/pyproject.toml` & `hrequests-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.1.2"
+version = "0.2.0"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
```

### Comparing `hrequests-0.1.2/README.md` & `hrequests-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,38 +67,38 @@
 
 Here is an example of a simple `get` request:
 
 ```py
 >>> resp = hrequests.get('https://www.google.com/')
 ```
 
-Requests are sent through [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof the TLS Client Fingerprint. This is done automatically, and is completely transparent to the user.
+Requests are sent through [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof the TLS client fingerprint. This is done automatically, and is completely transparent to the user.
 
 Other request methods include `post`, `put`, `delete`, `head`, `options`, and `patch`.
 
 The `Response` object is a near 1:1 replica of the `requests.Response` object, with some additional attributes.
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
     url (str): URL to send request to
     params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     data (Union[str, dict], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
     no_pause (bool, optional): Run the request in the background. Defaults to False.
+    <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
 
@@ -165,55 +165,91 @@
 <hr width=50>
 
 ## Sessions
 
 Creating a new Firefox Session object:
 
 ```py
->>> session = hrequests.Session()
+>>> session = hrequests.Session()  # version randomized by default
+>>> session = hrequests.Session('firefox', version=110)
 ```
 
-Or other browsers:
+<details>
+<summary>Parameters</summary>
 
-"`os`" can be `'win'`, `'mac'`, `'lin'`, or `'random'`. Default is `'random'`.
+```
+Parameters:
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+    version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
+    os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
+    headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
+    verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+    ja3_string (str, optional): JA3 string. Defaults to None.
+    h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
+    additional_decode (str, optional): Additional decode. Defaults to None.
+    pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
+    priority_frames (list, optional): Priority frames. Defaults to None.
+    header_order (list, optional): Header order. Defaults to None.
+    force_http1 (bool, optional): Force HTTP/1. Defaults to False.
+    catch_panics (bool, optional): Catch panics. Defaults to False.
+    debug (bool, optional): Debug mode. Defaults to False.
+```
+</details>
+
+Browsers can also be created through the `firefox`, `chrome`, and `opera` shortcuts:
 
 ```py
->>> session = hrequests.firefox.Session(os='win')
->>> session = hrequests.chrome.Session(os='lin')
->>> session = hrequests.opera.Session(os='mac')
+>>> session = hrequests.firefox.Session()
+>>> session = hrequests.chrome.Session()
+>>> session = hrequests.opera.Session()
 ```
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    browser (str): Browser to use [firefox, chrome, opera]
-    os (str): OS to use in header [win, mac, lin]
+    version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
+    os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
     pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
     priority_frames (list, optional): Priority frames. Defaults to None.
     header_order (list, optional): Header order. Defaults to None.
     force_http1 (bool, optional): Force HTTP/1. Defaults to False.
     catch_panics (bool, optional): Catch panics. Defaults to False.
     debug (bool, optional): Debug mode. Defaults to False.
 ```
 </details>
 
-This will automatically generate headers based on the browser name and OS.
+`os` can be `'win'`, `'mac'`, or `'lin'`. Default is randomized.
+
+```py
+>>> session = hrequests.firefox.Session(os='mac')
+```
+
+This will automatically generate headers based on the browser name and OS:
 
 ```py
 >>> session.headers
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'}
+{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_4; rv:60.2.2) Gecko/20100101 Firefox/60.2.2', 'Accept-Encoding': 'gzip, deflate, br', 'Pragma': 'no-cache'}
 ```
 
+<details>
+<summary>Why is the browser version in the header different than the TLS browser version?</summary>
+
+Website bot detection systems typically do not correlate the TLS fingerprint browser version with the browser header.
+
+By adding more randomization to our headers, we can make our requests appear to be coming from a larger number of clients. We can make it seem like our requests are coming from a larger number of clients. This makes it harder for websites to identify and block our requests based on a consistent browser version.
+
+</details>
+
 
 ### Properties
 
 Here is a simple get request. This is a wraper around `hrequests.get`. The only difference is that the session cookies are updated with each request. Creating sessions are recommended for making multiple requests to the same domain.
 
 ```py
 >>> resp = session.get('https://www.google.com/')
@@ -222,36 +258,31 @@
 Session cookies update with each request:
 
 ```py
 >>> session.cookies: RequestsCookieJar
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.google.com', domain_specified=True...
 ```
 
-Get headers:
+Regenerate headers for a different OS:
 
 ```py
+>>> session.os = 'win'
 >>> session.headers: CaseInsensitiveDict
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:52.7.0) Gecko/20100101 Firefox/52.7.0', 'Accept-Encoding': 'gzip, deflate, br', 'Upgrade-Insecure-Requests': '1', 'Referer': 'https://google.com', 'Pragma': 'no-cache'}
+{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0.3) Gecko/20100101 Firefox/66.0.3', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-Language': 'en-US;q=0.5,en;q=0.3', 'Cache-Control': 'max-age=0', 'DNT': '1', 'Upgrade-Insecure-Requests': '1', 'Pragma': 'no-cache'}
 ```
 
-Regenerate headers for a different OS:
-
-```py
->>> session.resetHeaders(os='mac')
->>> session.headers
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'}
-```
+### Closing Sessions
 
 Sessions can also be closed to free memory:
 
 ```py
 >>> session.close()
 ```
 
-Additionally, sessions can be used as context managers:
+Alternatively, sessions can be used as context managers:
 
 ```py
 with hrequests.Session() as session:
     resp = session.get('https://www.google.com/')
     print(resp)
 ```
 
@@ -285,26 +316,26 @@
 The method `async_get` will create an unsent request.
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
     url (str): URL to send request to
     params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     data (Union[str, dict], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
+    <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
 
@@ -632,15 +663,15 @@
 ```
 
 Toggle loading unnessecary resources such as images, fonts, styles, etc:
 ```py
 page.allow_styling: bool = False
 ```
 
-#### Pulling page data
+### Pulling page data
 
 
 Get current page url:
 
 ```py
 >>> page.url: str
 https://www.somewebsite.com/
@@ -672,15 +703,15 @@
 ```
 Parameters:
     path (str): Path to save screenshot to
     full_page (bool): Whether to take a screenshot of the full scrollable page
 ```
 </details>
 
-#### Navigate the browser
+### Navigate the browser
 
 Navigate to a url:
 
 ```py
 >>> page.url = 'https://bing.com'  # navigate to a url
 >>> page.goto('https://bing.com')  # or use goto
 ```
@@ -688,15 +719,15 @@
 Navigate through page history:
 
 ```py
 >>> page.back()
 >>> page.forward()
 ```
 
-#### Controlling elements
+### Controlling elements
 Click an element:
 ```py
 >>> page.click('#my-button')
 ```
 <details>
 <summary>Parameters</summary>
 
@@ -742,31 +773,19 @@
     check (bool, optional): Check if an element is draggable before running. Defaults to False.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
-#### Check page elements
+### Check page elements
 
-Check if a selector is visible:
+Check if a selector is visible and enabled:
 ```py
 >>> page.isVisible('#my-selector'): bool
-```
-<details>
-<summary>Parameters</summary>
-
-```
-Parameters:
-    selector (str): Selector to check
-```
-</details>
-
-Check if a selector is enabled:
-```py
 >>> page.isEnabled('#my-selector'): bool
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
@@ -784,15 +803,15 @@
 ```
 Parameters:
     script (str): Javascript to evaluate in the page
     arg (str, optional): Argument to pass into the javascript function
 ```
 </details>
 
-#### Awaiting events
+### Awaiting events
 
 ```py
 >>> page.awaitNavigation()
 ```
 
 <details>
 <summary>Parameters</summary>
@@ -876,15 +895,15 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
-#### Requests & Responses
+### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
 
 This returns a normal `Response` object:
 ```py
 >>> resp = page.get('https://duckduckgo.com')
 ```
@@ -910,15 +929,15 @@
 Returns:
     hrequests.response.Response: Response object
 ```
 </details>
 
 Other methods include `post`, `put`, `delete`, `head`, and `patch`.
 
-#### Closing the page
+### Closing the page
 
 The `BrowserSession` object must be closed when finished. This will close the browser, update the response data, and merge new cookies with the session cookies.
 
 ```py
 >>> page.close()
 ```
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_9mxok84c_/tmpnrxcngt9_TarContainer/0/28.md", line 966, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_9mxok84c_/tmpnrxcngt9_TarContainer/0/28.md", line 966, column 3: CDATA terminal not found*

```diff
@@ -17,124 +17,149 @@
 daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://
 github.com/daijro/hrequests#html-parsing) 5. [Page Rendering](https://
 github.com/daijro/hrequests#page-rendering)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
-the TLS Client Fingerprint. This is done automatically, and is completely
+the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
 the `requests.Response` object, with some additional attributes.  Parameters
-``` Parameters: method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT,
-PATCH, DELETE) url (str): URL to send request to params (dict, optional):
+``` Parameters: url (str): URL to send request to params (dict, optional):
 Dictionary of URL parameters to append to the URL. Defaults to None. data
 (Union[str, dict], optional): Data to send to request. Defaults to None.
 headers (dict, optional): Dictionary of HTTP headers to send with the request.
 Defaults to None. cookies (Union[RequestsCookieJar, dict, list], optional):
 Dict or CookieJar to send. Defaults to None. json (dict, optional): Json to
 send in the request body. Defaults to None. allow_redirects (bool, optional):
 Allow request to redirect. Defaults to True. history (bool, optional): Remember
 request history. Defaults to False. verify (bool, optional): Verify the
 server's TLS certificate. Defaults to True. timeout (int, optional): Timeout in
 seconds. Defaults to 30. proxies (dict, optional): Dictionary of proxies.
 Defaults to None. no_pause (bool, optional): Run the request in the background.
-Defaults to False. Returns: hrequests.response.Response: Response object ```
-### Properties Get the response url: ```py >>> resp.url: str 'https://
-www.google.com/' ``` Check if the request was successful: ```py >>>
-resp.status_code: int 200 >>> resp.reason: str 'OK' >>> resp.ok: bool True >>>
-bool(resp) True ``` Getting the response body: ```py >>> resp.text: str '
+Defaults to False.
+hrequests.Session` if a session was not specified> Returns:
+hrequests.response.Response: Response object ```  ### Properties Get the
+response url: ```py >>> resp.url: str 'https://www.google.com/' ``` Check if
+the request was successful: ```py >>> resp.status_code: int 200 >>>
+resp.reason: str 'OK' >>> resp.ok: bool True >>> bool(resp) True ``` Getting
+the response body: ```py >>> resp.text: str '
 ..' >>> resp.content: Union[bytes, str] '
 ..' ``` Parse the response body as JSON: ```py >>> resp.json(): Union[dict,
 list] {'somedata': True} ``` Get the elapsed time of the request: ```py >>>
 resp.elapsed: datetime.timedelta datetime.timedelta(microseconds=77768) ``` Get
 the response cookies: ```py >>> resp.cookies: RequestsCookieJar
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
 port_specified=False, domain='.google.com', domain_specified=True... ``` Get
 the response headers: ```py >>> resp.headers: CaseInsensitiveDict {'Alt-Svc':
 'h3=":443"; ma=2592000,h3-29=":443"; ma=2592000', 'Cache-Control': 'private,
 max-age=0', 'Content-Encoding': 'br', 'Content-Length': '51288', 'Content-
 Security-Policy-Report-Only': "object-src 'none';base-uri 'se ```
 ===============================================================================
 ## Sessions Creating a new Firefox Session object: ```py >>> session =
-hrequests.Session() ``` Or other browsers: "`os`" can be `'win'`, `'mac'`,
-`'lin'`, or `'random'`. Default is `'random'`. ```py >>> session =
-hrequests.firefox.Session(os='win') >>> session = hrequests.chrome.Session
-(os='lin') >>> session = hrequests.opera.Session(os='mac') ```  Parameters ```
-Parameters: browser (str): Browser to use [firefox, chrome, opera] os (str): OS
-to use in header [win, mac, lin] headers (dict, optional): Dictionary of HTTP
-headers to send with the request. Default is generated from `browser` and `os`.
-verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+hrequests.Session() # version randomized by default >>> session =
+hrequests.Session('firefox', version=110) ```  Parameters ``` Parameters:
+browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
+Default is 'firefox'. version (int, optional): Version of the browser to use.
+Browser must be specified. Default is randomized. os (Literal['win', 'mac',
+'lin'], optional): OS to use in header. Default is randomized. headers (dict,
+optional): Dictionary of HTTP headers to send with the request. Default is
+generated from `browser` and `os`. verify (bool, optional): Verify the server's
+TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
+Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
+None. additional_decode (str, optional): Additional decode. Defaults to None.
+pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
+priority_frames (list, optional): Priority frames. Defaults to None.
+header_order (list, optional): Header order. Defaults to None. force_http1
+(bool, optional): Force HTTP/1. Defaults to False. catch_panics (bool,
+optional): Catch panics. Defaults to False. debug (bool, optional): Debug mode.
+Defaults to False. ```  Browsers can also be created through the `firefox`,
+`chrome`, and `opera` shortcuts: ```py >>> session = hrequests.firefox.Session
+() >>> session = hrequests.chrome.Session() >>> session =
+hrequests.opera.Session() ```  Parameters ``` Parameters: version (int,
+optional): Version of the browser to use. Browser must be specified. Default is
+randomized. os (Literal['win', 'mac', 'lin'], optional): OS to use in header.
+Default is randomized. headers (dict, optional): Dictionary of HTTP headers to
+send with the request. Default is generated from `browser` and `os`. verify
+(bool, optional): Verify the server's TLS certificate. Defaults to True.
 ja3_string (str, optional): JA3 string. Defaults to None. h2_settings (dict,
 optional): HTTP/2 settings. Defaults to None. additional_decode (str,
 optional): Additional decode. Defaults to None. pseudo_header_order (list,
 optional): Pseudo header order. Defaults to None. priority_frames (list,
 optional): Priority frames. Defaults to None. header_order (list, optional):
 Header order. Defaults to None. force_http1 (bool, optional): Force HTTP/1.
 Defaults to False. catch_panics (bool, optional): Catch panics. Defaults to
-False. debug (bool, optional): Debug mode. Defaults to False. ```  This will
-automatically generate headers based on the browser name and OS. ```py >>>
-session.headers {'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent':
-'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101
-Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-
-age=0', 'DNT': '1'} ``` ### Properties Here is a simple get request. This is a
-wraper around `hrequests.get`. The only difference is that the session cookies
-are updated with each request. Creating sessions are recommended for making
+False. debug (bool, optional): Debug mode. Defaults to False. ```  `os` can be
+`'win'`, `'mac'`, or `'lin'`. Default is randomized. ```py >>> session =
+hrequests.firefox.Session(os='mac') ``` This will automatically generate
+headers based on the browser name and OS: ```py >>> session.headers {'Accept':
+'*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel
+Mac OS X 10_12_4; rv:60.2.2) Gecko/20100101 Firefox/60.2.2', 'Accept-Encoding':
+'gzip, deflate, br', 'Pragma': 'no-cache'} ```  Why is the browser version in
+the header different than the TLS browser version? Website bot detection
+systems typically do not correlate the TLS fingerprint browser version with the
+browser header. By adding more randomization to our headers, we can make our
+requests appear to be coming from a larger number of clients. We can make it
+seem like our requests are coming from a larger number of clients. This makes
+it harder for websites to identify and block our requests based on a consistent
+browser version.  ### Properties Here is a simple get request. This is a wraper
+around `hrequests.get`. The only difference is that the session cookies are
+updated with each request. Creating sessions are recommended for making
 multiple requests to the same domain. ```py >>> resp = session.get('https://
 www.google.com/') ``` Session cookies update with each request: ```py >>>
 session.cookies: RequestsCookieJar
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
-port_specified=False, domain='.google.com', domain_specified=True... ``` Get
-headers: ```py >>> session.headers: CaseInsensitiveDict {'Accept': '*/*',
-'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64;
-rv:52.7.0) Gecko/20100101 Firefox/52.7.0', 'Accept-Encoding': 'gzip, deflate,
-br', 'Upgrade-Insecure-Requests': '1', 'Referer': 'https://google.com',
-'Pragma': 'no-cache'} ``` Regenerate headers for a different OS: ```py >>>
-session.resetHeaders(os='mac') >>> session.headers {'Accept': '*/*',
-'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS
-X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip,
-deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'} ``` Sessions can also
-be closed to free memory: ```py >>> session.close() ``` Additionally, sessions
-can be used as context managers: ```py with hrequests.Session() as session:
-resp = session.get('https://www.google.com/') print(resp) ```
+port_specified=False, domain='.google.com', domain_specified=True... ```
+Regenerate headers for a different OS: ```py >>> session.os = 'win' >>>
+session.headers: CaseInsensitiveDict {'Accept': '*/*', 'Connection': 'keep-
+alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0.3)
+Gecko/20100101 Firefox/66.0.3', 'Accept-Encoding': 'gzip, deflate, br',
+'Accept-Language': 'en-US;q=0.5,en;q=0.3', 'Cache-Control': 'max-age=0', 'DNT':
+'1', 'Upgrade-Insecure-Requests': '1', 'Pragma': 'no-cache'} ``` ### Closing
+Sessions Sessions can also be closed to free memory: ```py >>> session.close()
+``` Alternatively, sessions can be used as context managers: ```py with
+hrequests.Session() as session: resp = session.get('https://www.google.com/')
+print(resp) ```
 ===============================================================================
 ## Concurrent & Lazy Requests ### "Lazy" Requests Adding the `no_pause=True`
 keyword argument will return a `LazyTLSRequest` object. This will send the
 request immediately, but doesn't wait for the response to be ready until an
 attribute of the response is accessed. ```py resp1 = hrequests.get('https://
 www.google.com/', no_pause=True) resp2 = hrequests.get('https://www.google.com/
 ', no_pause=True) # resp1 and resp2 are sent concurrently print('Resp 1:',
 resp1.reason) # will pause for resp1 to finish, if it hasn't already print
 ('Resp 2:', resp2.reason) # will pause for resp2 to finish, if it hasn't
 already ``` This is useful for sending multiple requests concurrently, but only
 waiting for the response when it is needed. Note that `no_pause` uses gevent as
 it's backend. Use `no_pause_threadsafe` when running across multiple threads.
 ### Grequests-style Async Requests The method `async_get` will create an unsent
-request.  Parameters ``` Parameters: method (str): Method of request (GET,
-POST, OPTIONS, HEAD, PUT, PATCH, DELETE) url (str): URL to send request to
-params (dict, optional): Dictionary of URL parameters to append to the URL.
-Defaults to None. data (Union[str, dict], optional): Data to send to request.
-Defaults to None. headers (dict, optional): Dictionary of HTTP headers to send
-with the request. Defaults to None. cookies (Union[RequestsCookieJar, dict,
-list], optional): Dict or CookieJar to send. Defaults to None. json (dict,
-optional): Json to send in the request body. Defaults to None. allow_redirects
-(bool, optional): Allow request to redirect. Defaults to True. history (bool,
+request.  Parameters ``` Parameters: url (str): URL to send request to params
+(dict, optional): Dictionary of URL parameters to append to the URL. Defaults
+to None. data (Union[str, dict], optional): Data to send to request. Defaults
+to None. headers (dict, optional): Dictionary of HTTP headers to send with the
+request. Defaults to None. cookies (Union[RequestsCookieJar, dict, list],
+optional): Dict or CookieJar to send. Defaults to None. json (dict, optional):
+Json to send in the request body. Defaults to None. allow_redirects (bool,
+optional): Allow request to redirect. Defaults to True. history (bool,
 optional): Remember request history. Defaults to False. verify (bool,
 optional): Verify the server's TLS certificate. Defaults to True. timeout (int,
 optional): Timeout in seconds. Defaults to 30. proxies (dict, optional):
-Dictionary of proxies. Defaults to None. Returns: hrequests.response.Response:
-Response object ```  Async requests are evaluated on `hrequests.map`,
-`hrequests.imap`, or `hrequests.imap_enum`. This functionality is similar to
-[grequests](https://github.com/spyoungtech/grequests). Unlike grequests,
-[monkey patching](https://www.gevent.org/api/gevent.monkey.html) is not
-required because this does not rely on the standard python SSL library. Create
-a set of unsent Requests: ```py reqs = [ hrequests.async_get('https://
-www.google.com/'), hrequests.async_get('https://www.duckduckgo.com/'),
-hrequests.async_get('https://www.yahoo.com/') ] ``` #### map Send them all at
-the same time using map: ```py >>> hrequests.map(reqs, size=3) [
+Dictionary of proxies. Defaults to None.
+hrequests.Session` if a session was not specified> Returns:
+hrequests.response.Response: Response object ```  Async requests are evaluated
+on `hrequests.map`, `hrequests.imap`, or `hrequests.imap_enum`. This
+functionality is similar to [grequests](https://github.com/spyoungtech/
+grequests). Unlike grequests, [monkey patching](https://www.gevent.org/api/
+gevent.monkey.html) is not required because this does not rely on the standard
+python SSL library. Create a set of unsent Requests: ```py reqs =
+[ hrequests.async_get('https://www.google.com/'), hrequests.async_get('https://
+www.duckduckgo.com/'), hrequests.async_get('https://www.yahoo.com/') ] ``` ####
+map Send them all at the same time using map: ```py >>> hrequests.map(reqs,
+size=3) [
 200]>,
 200]>,
 200]>] ```  Parameters ``` Concurrently converts a list of Requests to
 Responses. Parameters: requests - a collection of Request objects. size -
 Specifies the number of requests to make at a time. If None, no throttling
 occurs. exception_handler - Callback function, called when exception occured.
 Params: Request, Exception timeout - Gevent joinall timeout in seconds. (Note:
```

### Comparing `hrequests-0.1.2/PKG-INFO` & `hrequests-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.1.2
+Version: 0.2.0
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -106,38 +106,38 @@
 
 Here is an example of a simple `get` request:
 
 ```py
 >>> resp = hrequests.get('https://www.google.com/')
 ```
 
-Requests are sent through [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof the TLS Client Fingerprint. This is done automatically, and is completely transparent to the user.
+Requests are sent through [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof the TLS client fingerprint. This is done automatically, and is completely transparent to the user.
 
 Other request methods include `post`, `put`, `delete`, `head`, `options`, and `patch`.
 
 The `Response` object is a near 1:1 replica of the `requests.Response` object, with some additional attributes.
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
     url (str): URL to send request to
     params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     data (Union[str, dict], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
     no_pause (bool, optional): Run the request in the background. Defaults to False.
+    <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
 
@@ -204,55 +204,91 @@
 <hr width=50>
 
 ## Sessions
 
 Creating a new Firefox Session object:
 
 ```py
->>> session = hrequests.Session()
+>>> session = hrequests.Session()  # version randomized by default
+>>> session = hrequests.Session('firefox', version=110)
 ```
 
-Or other browsers:
+<details>
+<summary>Parameters</summary>
 
-"`os`" can be `'win'`, `'mac'`, `'lin'`, or `'random'`. Default is `'random'`.
+```
+Parameters:
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+    version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
+    os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
+    headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
+    verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+    ja3_string (str, optional): JA3 string. Defaults to None.
+    h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
+    additional_decode (str, optional): Additional decode. Defaults to None.
+    pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
+    priority_frames (list, optional): Priority frames. Defaults to None.
+    header_order (list, optional): Header order. Defaults to None.
+    force_http1 (bool, optional): Force HTTP/1. Defaults to False.
+    catch_panics (bool, optional): Catch panics. Defaults to False.
+    debug (bool, optional): Debug mode. Defaults to False.
+```
+</details>
+
+Browsers can also be created through the `firefox`, `chrome`, and `opera` shortcuts:
 
 ```py
->>> session = hrequests.firefox.Session(os='win')
->>> session = hrequests.chrome.Session(os='lin')
->>> session = hrequests.opera.Session(os='mac')
+>>> session = hrequests.firefox.Session()
+>>> session = hrequests.chrome.Session()
+>>> session = hrequests.opera.Session()
 ```
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    browser (str): Browser to use [firefox, chrome, opera]
-    os (str): OS to use in header [win, mac, lin]
+    version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
+    os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
     pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
     priority_frames (list, optional): Priority frames. Defaults to None.
     header_order (list, optional): Header order. Defaults to None.
     force_http1 (bool, optional): Force HTTP/1. Defaults to False.
     catch_panics (bool, optional): Catch panics. Defaults to False.
     debug (bool, optional): Debug mode. Defaults to False.
 ```
 </details>
 
-This will automatically generate headers based on the browser name and OS.
+`os` can be `'win'`, `'mac'`, or `'lin'`. Default is randomized.
+
+```py
+>>> session = hrequests.firefox.Session(os='mac')
+```
+
+This will automatically generate headers based on the browser name and OS:
 
 ```py
 >>> session.headers
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'}
+{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_4; rv:60.2.2) Gecko/20100101 Firefox/60.2.2', 'Accept-Encoding': 'gzip, deflate, br', 'Pragma': 'no-cache'}
 ```
 
+<details>
+<summary>Why is the browser version in the header different than the TLS browser version?</summary>
+
+Website bot detection systems typically do not correlate the TLS fingerprint browser version with the browser header.
+
+By adding more randomization to our headers, we can make our requests appear to be coming from a larger number of clients. We can make it seem like our requests are coming from a larger number of clients. This makes it harder for websites to identify and block our requests based on a consistent browser version.
+
+</details>
+
 
 ### Properties
 
 Here is a simple get request. This is a wraper around `hrequests.get`. The only difference is that the session cookies are updated with each request. Creating sessions are recommended for making multiple requests to the same domain.
 
 ```py
 >>> resp = session.get('https://www.google.com/')
@@ -261,36 +297,31 @@
 Session cookies update with each request:
 
 ```py
 >>> session.cookies: RequestsCookieJar
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.google.com', domain_specified=True...
 ```
 
-Get headers:
+Regenerate headers for a different OS:
 
 ```py
+>>> session.os = 'win'
 >>> session.headers: CaseInsensitiveDict
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:52.7.0) Gecko/20100101 Firefox/52.7.0', 'Accept-Encoding': 'gzip, deflate, br', 'Upgrade-Insecure-Requests': '1', 'Referer': 'https://google.com', 'Pragma': 'no-cache'}
+{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0.3) Gecko/20100101 Firefox/66.0.3', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-Language': 'en-US;q=0.5,en;q=0.3', 'Cache-Control': 'max-age=0', 'DNT': '1', 'Upgrade-Insecure-Requests': '1', 'Pragma': 'no-cache'}
 ```
 
-Regenerate headers for a different OS:
-
-```py
->>> session.resetHeaders(os='mac')
->>> session.headers
-{'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'}
-```
+### Closing Sessions
 
 Sessions can also be closed to free memory:
 
 ```py
 >>> session.close()
 ```
 
-Additionally, sessions can be used as context managers:
+Alternatively, sessions can be used as context managers:
 
 ```py
 with hrequests.Session() as session:
     resp = session.get('https://www.google.com/')
     print(resp)
 ```
 
@@ -324,26 +355,26 @@
 The method `async_get` will create an unsent request.
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
     url (str): URL to send request to
     params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     data (Union[str, dict], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
+    <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
 
@@ -671,15 +702,15 @@
 ```
 
 Toggle loading unnessecary resources such as images, fonts, styles, etc:
 ```py
 page.allow_styling: bool = False
 ```
 
-#### Pulling page data
+### Pulling page data
 
 
 Get current page url:
 
 ```py
 >>> page.url: str
 https://www.somewebsite.com/
@@ -711,15 +742,15 @@
 ```
 Parameters:
     path (str): Path to save screenshot to
     full_page (bool): Whether to take a screenshot of the full scrollable page
 ```
 </details>
 
-#### Navigate the browser
+### Navigate the browser
 
 Navigate to a url:
 
 ```py
 >>> page.url = 'https://bing.com'  # navigate to a url
 >>> page.goto('https://bing.com')  # or use goto
 ```
@@ -727,15 +758,15 @@
 Navigate through page history:
 
 ```py
 >>> page.back()
 >>> page.forward()
 ```
 
-#### Controlling elements
+### Controlling elements
 Click an element:
 ```py
 >>> page.click('#my-button')
 ```
 <details>
 <summary>Parameters</summary>
 
@@ -781,31 +812,19 @@
     check (bool, optional): Check if an element is draggable before running. Defaults to False.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
-#### Check page elements
+### Check page elements
 
-Check if a selector is visible:
+Check if a selector is visible and enabled:
 ```py
 >>> page.isVisible('#my-selector'): bool
-```
-<details>
-<summary>Parameters</summary>
-
-```
-Parameters:
-    selector (str): Selector to check
-```
-</details>
-
-Check if a selector is enabled:
-```py
 >>> page.isEnabled('#my-selector'): bool
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
@@ -823,15 +842,15 @@
 ```
 Parameters:
     script (str): Javascript to evaluate in the page
     arg (str, optional): Argument to pass into the javascript function
 ```
 </details>
 
-#### Awaiting events
+### Awaiting events
 
 ```py
 >>> page.awaitNavigation()
 ```
 
 <details>
 <summary>Parameters</summary>
@@ -915,15 +934,15 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
-#### Requests & Responses
+### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
 
 This returns a normal `Response` object:
 ```py
 >>> resp = page.get('https://duckduckgo.com')
 ```
@@ -949,15 +968,15 @@
 Returns:
     hrequests.response.Response: Response object
 ```
 </details>
 
 Other methods include `post`, `put`, `delete`, `head`, and `patch`.
 
-#### Closing the page
+### Closing the page
 
 The `BrowserSession` object must be closed when finished. This will close the browser, update the response data, and merge new cookies with the session cookies.
 
 ```py
 >>> page.close()
 ```
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_9mxok84c_/tmpnrxcngt9_TarContainer/0/29", line 1006, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_9mxok84c_/tmpnrxcngt9_TarContainer/0/29", line 1006, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.1.2 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.2.0 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -36,124 +36,149 @@
 daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://
 github.com/daijro/hrequests#html-parsing) 5. [Page Rendering](https://
 github.com/daijro/hrequests#page-rendering)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
-the TLS Client Fingerprint. This is done automatically, and is completely
+the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
 the `requests.Response` object, with some additional attributes.  Parameters
-``` Parameters: method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT,
-PATCH, DELETE) url (str): URL to send request to params (dict, optional):
+``` Parameters: url (str): URL to send request to params (dict, optional):
 Dictionary of URL parameters to append to the URL. Defaults to None. data
 (Union[str, dict], optional): Data to send to request. Defaults to None.
 headers (dict, optional): Dictionary of HTTP headers to send with the request.
 Defaults to None. cookies (Union[RequestsCookieJar, dict, list], optional):
 Dict or CookieJar to send. Defaults to None. json (dict, optional): Json to
 send in the request body. Defaults to None. allow_redirects (bool, optional):
 Allow request to redirect. Defaults to True. history (bool, optional): Remember
 request history. Defaults to False. verify (bool, optional): Verify the
 server's TLS certificate. Defaults to True. timeout (int, optional): Timeout in
 seconds. Defaults to 30. proxies (dict, optional): Dictionary of proxies.
 Defaults to None. no_pause (bool, optional): Run the request in the background.
-Defaults to False. Returns: hrequests.response.Response: Response object ```
-### Properties Get the response url: ```py >>> resp.url: str 'https://
-www.google.com/' ``` Check if the request was successful: ```py >>>
-resp.status_code: int 200 >>> resp.reason: str 'OK' >>> resp.ok: bool True >>>
-bool(resp) True ``` Getting the response body: ```py >>> resp.text: str '
+Defaults to False.
+hrequests.Session` if a session was not specified> Returns:
+hrequests.response.Response: Response object ```  ### Properties Get the
+response url: ```py >>> resp.url: str 'https://www.google.com/' ``` Check if
+the request was successful: ```py >>> resp.status_code: int 200 >>>
+resp.reason: str 'OK' >>> resp.ok: bool True >>> bool(resp) True ``` Getting
+the response body: ```py >>> resp.text: str '
 ..' >>> resp.content: Union[bytes, str] '
 ..' ``` Parse the response body as JSON: ```py >>> resp.json(): Union[dict,
 list] {'somedata': True} ``` Get the elapsed time of the request: ```py >>>
 resp.elapsed: datetime.timedelta datetime.timedelta(microseconds=77768) ``` Get
 the response cookies: ```py >>> resp.cookies: RequestsCookieJar
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
 port_specified=False, domain='.google.com', domain_specified=True... ``` Get
 the response headers: ```py >>> resp.headers: CaseInsensitiveDict {'Alt-Svc':
 'h3=":443"; ma=2592000,h3-29=":443"; ma=2592000', 'Cache-Control': 'private,
 max-age=0', 'Content-Encoding': 'br', 'Content-Length': '51288', 'Content-
 Security-Policy-Report-Only': "object-src 'none';base-uri 'se ```
 ===============================================================================
 ## Sessions Creating a new Firefox Session object: ```py >>> session =
-hrequests.Session() ``` Or other browsers: "`os`" can be `'win'`, `'mac'`,
-`'lin'`, or `'random'`. Default is `'random'`. ```py >>> session =
-hrequests.firefox.Session(os='win') >>> session = hrequests.chrome.Session
-(os='lin') >>> session = hrequests.opera.Session(os='mac') ```  Parameters ```
-Parameters: browser (str): Browser to use [firefox, chrome, opera] os (str): OS
-to use in header [win, mac, lin] headers (dict, optional): Dictionary of HTTP
-headers to send with the request. Default is generated from `browser` and `os`.
-verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+hrequests.Session() # version randomized by default >>> session =
+hrequests.Session('firefox', version=110) ```  Parameters ``` Parameters:
+browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
+Default is 'firefox'. version (int, optional): Version of the browser to use.
+Browser must be specified. Default is randomized. os (Literal['win', 'mac',
+'lin'], optional): OS to use in header. Default is randomized. headers (dict,
+optional): Dictionary of HTTP headers to send with the request. Default is
+generated from `browser` and `os`. verify (bool, optional): Verify the server's
+TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
+Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
+None. additional_decode (str, optional): Additional decode. Defaults to None.
+pseudo_header_order (list, optional): Pseudo header order. Defaults to None.
+priority_frames (list, optional): Priority frames. Defaults to None.
+header_order (list, optional): Header order. Defaults to None. force_http1
+(bool, optional): Force HTTP/1. Defaults to False. catch_panics (bool,
+optional): Catch panics. Defaults to False. debug (bool, optional): Debug mode.
+Defaults to False. ```  Browsers can also be created through the `firefox`,
+`chrome`, and `opera` shortcuts: ```py >>> session = hrequests.firefox.Session
+() >>> session = hrequests.chrome.Session() >>> session =
+hrequests.opera.Session() ```  Parameters ``` Parameters: version (int,
+optional): Version of the browser to use. Browser must be specified. Default is
+randomized. os (Literal['win', 'mac', 'lin'], optional): OS to use in header.
+Default is randomized. headers (dict, optional): Dictionary of HTTP headers to
+send with the request. Default is generated from `browser` and `os`. verify
+(bool, optional): Verify the server's TLS certificate. Defaults to True.
 ja3_string (str, optional): JA3 string. Defaults to None. h2_settings (dict,
 optional): HTTP/2 settings. Defaults to None. additional_decode (str,
 optional): Additional decode. Defaults to None. pseudo_header_order (list,
 optional): Pseudo header order. Defaults to None. priority_frames (list,
 optional): Priority frames. Defaults to None. header_order (list, optional):
 Header order. Defaults to None. force_http1 (bool, optional): Force HTTP/1.
 Defaults to False. catch_panics (bool, optional): Catch panics. Defaults to
-False. debug (bool, optional): Debug mode. Defaults to False. ```  This will
-automatically generate headers based on the browser name and OS. ```py >>>
-session.headers {'Accept': '*/*', 'Connection': 'keep-alive', 'User-Agent':
-'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5; rv:52.8.0) Gecko/20100101
-Firefox/52.8.0', 'Accept-Encoding': 'gzip, deflate, br', 'Cache-Control': 'max-
-age=0', 'DNT': '1'} ``` ### Properties Here is a simple get request. This is a
-wraper around `hrequests.get`. The only difference is that the session cookies
-are updated with each request. Creating sessions are recommended for making
+False. debug (bool, optional): Debug mode. Defaults to False. ```  `os` can be
+`'win'`, `'mac'`, or `'lin'`. Default is randomized. ```py >>> session =
+hrequests.firefox.Session(os='mac') ``` This will automatically generate
+headers based on the browser name and OS: ```py >>> session.headers {'Accept':
+'*/*', 'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel
+Mac OS X 10_12_4; rv:60.2.2) Gecko/20100101 Firefox/60.2.2', 'Accept-Encoding':
+'gzip, deflate, br', 'Pragma': 'no-cache'} ```  Why is the browser version in
+the header different than the TLS browser version? Website bot detection
+systems typically do not correlate the TLS fingerprint browser version with the
+browser header. By adding more randomization to our headers, we can make our
+requests appear to be coming from a larger number of clients. We can make it
+seem like our requests are coming from a larger number of clients. This makes
+it harder for websites to identify and block our requests based on a consistent
+browser version.  ### Properties Here is a simple get request. This is a wraper
+around `hrequests.get`. The only difference is that the session cookies are
+updated with each request. Creating sessions are recommended for making
 multiple requests to the same domain. ```py >>> resp = session.get('https://
 www.google.com/') ``` Session cookies update with each request: ```py >>>
 session.cookies: RequestsCookieJar
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
-port_specified=False, domain='.google.com', domain_specified=True... ``` Get
-headers: ```py >>> session.headers: CaseInsensitiveDict {'Accept': '*/*',
-'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64;
-rv:52.7.0) Gecko/20100101 Firefox/52.7.0', 'Accept-Encoding': 'gzip, deflate,
-br', 'Upgrade-Insecure-Requests': '1', 'Referer': 'https://google.com',
-'Pragma': 'no-cache'} ``` Regenerate headers for a different OS: ```py >>>
-session.resetHeaders(os='mac') >>> session.headers {'Accept': '*/*',
-'Connection': 'keep-alive', 'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS
-X 10_10_5; rv:52.8.0) Gecko/20100101 Firefox/52.8.0', 'Accept-Encoding': 'gzip,
-deflate, br', 'Cache-Control': 'max-age=0', 'DNT': '1'} ``` Sessions can also
-be closed to free memory: ```py >>> session.close() ``` Additionally, sessions
-can be used as context managers: ```py with hrequests.Session() as session:
-resp = session.get('https://www.google.com/') print(resp) ```
+port_specified=False, domain='.google.com', domain_specified=True... ```
+Regenerate headers for a different OS: ```py >>> session.os = 'win' >>>
+session.headers: CaseInsensitiveDict {'Accept': '*/*', 'Connection': 'keep-
+alive', 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0.3)
+Gecko/20100101 Firefox/66.0.3', 'Accept-Encoding': 'gzip, deflate, br',
+'Accept-Language': 'en-US;q=0.5,en;q=0.3', 'Cache-Control': 'max-age=0', 'DNT':
+'1', 'Upgrade-Insecure-Requests': '1', 'Pragma': 'no-cache'} ``` ### Closing
+Sessions Sessions can also be closed to free memory: ```py >>> session.close()
+``` Alternatively, sessions can be used as context managers: ```py with
+hrequests.Session() as session: resp = session.get('https://www.google.com/')
+print(resp) ```
 ===============================================================================
 ## Concurrent & Lazy Requests ### "Lazy" Requests Adding the `no_pause=True`
 keyword argument will return a `LazyTLSRequest` object. This will send the
 request immediately, but doesn't wait for the response to be ready until an
 attribute of the response is accessed. ```py resp1 = hrequests.get('https://
 www.google.com/', no_pause=True) resp2 = hrequests.get('https://www.google.com/
 ', no_pause=True) # resp1 and resp2 are sent concurrently print('Resp 1:',
 resp1.reason) # will pause for resp1 to finish, if it hasn't already print
 ('Resp 2:', resp2.reason) # will pause for resp2 to finish, if it hasn't
 already ``` This is useful for sending multiple requests concurrently, but only
 waiting for the response when it is needed. Note that `no_pause` uses gevent as
 it's backend. Use `no_pause_threadsafe` when running across multiple threads.
 ### Grequests-style Async Requests The method `async_get` will create an unsent
-request.  Parameters ``` Parameters: method (str): Method of request (GET,
-POST, OPTIONS, HEAD, PUT, PATCH, DELETE) url (str): URL to send request to
-params (dict, optional): Dictionary of URL parameters to append to the URL.
-Defaults to None. data (Union[str, dict], optional): Data to send to request.
-Defaults to None. headers (dict, optional): Dictionary of HTTP headers to send
-with the request. Defaults to None. cookies (Union[RequestsCookieJar, dict,
-list], optional): Dict or CookieJar to send. Defaults to None. json (dict,
-optional): Json to send in the request body. Defaults to None. allow_redirects
-(bool, optional): Allow request to redirect. Defaults to True. history (bool,
+request.  Parameters ``` Parameters: url (str): URL to send request to params
+(dict, optional): Dictionary of URL parameters to append to the URL. Defaults
+to None. data (Union[str, dict], optional): Data to send to request. Defaults
+to None. headers (dict, optional): Dictionary of HTTP headers to send with the
+request. Defaults to None. cookies (Union[RequestsCookieJar, dict, list],
+optional): Dict or CookieJar to send. Defaults to None. json (dict, optional):
+Json to send in the request body. Defaults to None. allow_redirects (bool,
+optional): Allow request to redirect. Defaults to True. history (bool,
 optional): Remember request history. Defaults to False. verify (bool,
 optional): Verify the server's TLS certificate. Defaults to True. timeout (int,
 optional): Timeout in seconds. Defaults to 30. proxies (dict, optional):
-Dictionary of proxies. Defaults to None. Returns: hrequests.response.Response:
-Response object ```  Async requests are evaluated on `hrequests.map`,
-`hrequests.imap`, or `hrequests.imap_enum`. This functionality is similar to
-[grequests](https://github.com/spyoungtech/grequests). Unlike grequests,
-[monkey patching](https://www.gevent.org/api/gevent.monkey.html) is not
-required because this does not rely on the standard python SSL library. Create
-a set of unsent Requests: ```py reqs = [ hrequests.async_get('https://
-www.google.com/'), hrequests.async_get('https://www.duckduckgo.com/'),
-hrequests.async_get('https://www.yahoo.com/') ] ``` #### map Send them all at
-the same time using map: ```py >>> hrequests.map(reqs, size=3) [
+Dictionary of proxies. Defaults to None.
+hrequests.Session` if a session was not specified> Returns:
+hrequests.response.Response: Response object ```  Async requests are evaluated
+on `hrequests.map`, `hrequests.imap`, or `hrequests.imap_enum`. This
+functionality is similar to [grequests](https://github.com/spyoungtech/
+grequests). Unlike grequests, [monkey patching](https://www.gevent.org/api/
+gevent.monkey.html) is not required because this does not rely on the standard
+python SSL library. Create a set of unsent Requests: ```py reqs =
+[ hrequests.async_get('https://www.google.com/'), hrequests.async_get('https://
+www.duckduckgo.com/'), hrequests.async_get('https://www.yahoo.com/') ] ``` ####
+map Send them all at the same time using map: ```py >>> hrequests.map(reqs,
+size=3) [
 200]>,
 200]>,
 200]>] ```  Parameters ``` Concurrently converts a list of Requests to
 Responses. Parameters: requests - a collection of Request objects. size -
 Specifies the number of requests to make at a time. If None, no throttling
 occurs. exception_handler - Callback function, called when exception occured.
 Params: Request, Exception timeout - Gevent joinall timeout in seconds. (Note:
```

