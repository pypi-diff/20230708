# Comparing `tmp/pbipy-2.3.4.tar.gz` & `tmp/pbipy-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.3.4.tar", last modified: Tue Jul  4 08:10:01 2023, max compression
+gzip compressed data, was "pbipy-2.4.5.tar", last modified: Sat Jul  8 17:45:28 2023, max compression
```

## Comparing `pbipy-2.3.4.tar` & `pbipy-2.4.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.427516 pbipy-2.3.4/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.3.4/LICENSE
--rw-rw-rw-   0        0        0    11017 2023-07-04 08:10:01.426513 pbipy-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    10233 2023-07-04 08:02:15.000000 pbipy-2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.412516 pbipy-2.3.4/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.3.4/pbipy/__init__.py
--rw-rw-rw-   0        0        0      335 2023-07-04 08:07:00.000000 pbipy-2.3.4/pbipy/__version__.py
--rw-rw-rw-   0        0        0     4932 2023-07-03 17:56:42.000000 pbipy-2.3.4/pbipy/apps.py
--rw-rw-rw-   0        0        0     1630 2023-07-03 09:18:23.000000 pbipy-2.3.4/pbipy/dashboards.py
--rw-rw-rw-   0        0        0    19984 2023-06-20 20:08:48.000000 pbipy-2.3.4/pbipy/datasets.py
--rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.3.4/pbipy/groups.py
--rw-rw-rw-   0        0        0    12471 2023-07-02 19:39:59.000000 pbipy-2.3.4/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    12848 2023-06-30 01:50:56.000000 pbipy-2.3.4/pbipy/reports.py
--rw-rw-rw-   0        0        0     1312 2023-06-19 20:24:41.000000 pbipy-2.3.4/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.3.4/pbipy/settings.py
--rw-rw-rw-   0        0        0    11125 2023-06-29 21:51:58.000000 pbipy-2.3.4/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:10:01.423517 pbipy-2.3.4/pbipy.egg-info/
--rw-rw-rw-   0        0        0    11017 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 08:10:01.000000 pbipy-2.3.4/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:10:01.427516 pbipy-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.953789 pbipy-2.4.5/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0    11056 2023-07-08 17:45:28.953789 pbipy-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10272 2023-07-08 17:41:53.000000 pbipy-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.945788 pbipy-2.4.5/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.4.5/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-07-08 17:44:27.000000 pbipy-2.4.5/pbipy/__version__.py
+-rw-rw-rw-   0        0        0     4932 2023-07-03 17:56:42.000000 pbipy-2.4.5/pbipy/apps.py
+-rw-rw-rw-   0        0        0     1630 2023-07-03 09:18:23.000000 pbipy-2.4.5/pbipy/dashboards.py
+-rw-rw-rw-   0        0        0     5782 2023-07-08 17:35:27.000000 pbipy-2.4.5/pbipy/dataflows.py
+-rw-rw-rw-   0        0        0    19984 2023-07-08 17:28:25.000000 pbipy-2.4.5/pbipy/datasets.py
+-rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.4.5/pbipy/groups.py
+-rw-rw-rw-   0        0        0    16707 2023-07-08 17:29:44.000000 pbipy-2.4.5/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    12848 2023-06-30 01:50:56.000000 pbipy-2.4.5/pbipy/reports.py
+-rw-rw-rw-   0        0        0     1367 2023-07-06 17:22:30.000000 pbipy-2.4.5/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.4.5/pbipy/settings.py
+-rw-rw-rw-   0        0        0    11724 2023-07-08 01:16:07.000000 pbipy-2.4.5/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.953789 pbipy-2.4.5/pbipy.egg-info/
+-rw-rw-rw-   0        0        0    11056 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:45:28.953789 pbipy-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.4.5/setup.py
```

### Comparing `pbipy-2.3.4/LICENSE` & `pbipy-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.3.4/PKG-INFO` & `pbipy-2.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.3.4
+Version: 2.4.5
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -142,24 +142,24 @@
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
 First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
 
 ```python
 sales = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 ```
@@ -272,16 +272,16 @@
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
 | Apps                	| Done   	|       	|
-| Dataflows           	| Doing    	|       	|
-| Admin Operations     	| Todo     	|       	|
+| Dataflows           	| Done    	|       	|
+| Admin Operations     	| Doing    	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.3.4/README.md` & `pbipy-2.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -122,24 +122,24 @@
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
 First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
 
 ```python
 sales = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 ```
@@ -252,16 +252,16 @@
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
 | Apps                	| Done   	|       	|
-| Dataflows           	| Doing    	|       	|
-| Admin Operations     	| Todo     	|       	|
+| Dataflows           	| Done    	|       	|
+| Admin Operations     	| Doing    	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.3.4/pbipy/apps.py` & `pbipy-2.4.5/pbipy/apps.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.3.4/pbipy/dashboards.py` & `pbipy-2.4.5/pbipy/dashboards.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.3.4/pbipy/datasets.py` & `pbipy-2.4.5/pbipy/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
         
         Providing `direct_query=True` targets the Direct Query
         Refresh Schedule.
         
         Parameters
         ----------
         `notify_option` : `str`
-            Mail notification options, e.g., "MailOnCompletion", "MailOnFailure",
+            Email notification options, e.g., "MailOnCompletion", "MailOnFailure",
             or "NoNotification".
         `direct_query` : bool, optional
             Target the Direct Query Refresh Schedule (if there is one) of the
             dataset.
         `days` : list[str], optional
             The full name of days on which to execute the refresh,e.g, "Monday",
             "Tuesday", "Wednesday", etc.
@@ -538,15 +538,15 @@
         `frequency` : int, optional
             Applies to Direct Query Refresh Schedule only. The interval in minutes
             between successive refreshes. Supported values are 15, 30, 60, 120,
             and 180.
             If `frequency` is supplied and `direct_query` is `false`, then `frequency`
             will be ignored.
         `local_time_zone_id` : `str`, optional
-            _The ID of the time zone to use, e.g, "UTC".
+            The ID of the time zone to use, e.g, "UTC".
         `times` : list[str], optional
             The times of day to execute the refresh expressed as hh:mm, e.g.,
             "07:00", "16:00", etc.
         
         Raises
         ------
         `ValueError`
```

### Comparing `pbipy-2.3.4/pbipy/groups.py` & `pbipy-2.4.5/pbipy/groups.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.3.4/pbipy/powerbi.py` & `pbipy-2.4.5/pbipy/powerbi.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import requests
 from requests.exceptions import HTTPError
 
 from pbipy import settings
 from pbipy.apps import App
+from pbipy.dataflows import Dataflow
 from pbipy.groups import Group
 from pbipy.datasets import Dataset
 from pbipy.reports import Report
 from pbipy.utils import RequestsMixin, remove_no_values
 
 
 class PowerBI(RequestsMixin):
@@ -97,14 +98,171 @@
                 raw=app_js,
             )
             for app_js in raw
         ]
 
         return apps
 
+    def cancel_transaction(
+        self,
+        transaction_id: str,
+        group: str | Group,
+    ) -> dict:
+        """
+        Attempt to cancel the specified Dataflow Transaction.
+
+        Parameters
+        ----------
+        `transaction_id` : `str`
+            Id of the Transaction to cancel.
+        `group` : `str | Group`
+            Group Id or `Group` object where the Transaction originated. 
+            Should match the Group of the Dataflow that generated the 
+            transaction.
+
+        Returns
+        -------
+        `dict`
+            Dataflow transaction status.
+
+        """
+
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+
+        resource = (
+            self.BASE_URL
+            + f"/groups/{group_id}/dataflows/transactions/{transaction_id}/cancel"
+        )
+        raw = self.post_raw(resource, self.session)
+
+        return raw
+
+    def dataflow(
+        self,
+        dataflow: str | Dataflow,
+        group: str | Group,
+    ) -> Dataflow:
+        """
+        Get and load the specified dataflow.
+
+        Parameters
+        ----------
+        `dataflow` : `str | Dataflow`
+            The Dataflow Id of the Dataflow to retrieve.
+        `group` : `str | Group`
+            The Group Id or `Group` object where the Dataflow resides.
+
+        Returns
+        -------
+        `Dataflow`
+            The specified Dataflow.
+
+        Notes
+        -----
+        The Get Dataflow endpoint returns a json file. For consistency
+        with the rest of pbipy, this method returns a `Dataflow` object instead
+        of the file itself. To access the json file, use the `Dataflow.raw`
+        property.
+
+        """
+
+        if isinstance(dataflow, Dataflow):
+            return Dataflow
+
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+
+        resource = self.BASE_URL + f"/groups/{group_id}/dataflows/{dataflow}"
+        raw = self.get_raw(resource, self.session)
+
+        dataflow = Dataflow(
+            raw.get("objectId"),
+            self.session,
+            group_id=group_id,
+            raw=raw,
+        )
+
+        return dataflow
+
+    def dataflows(
+        self,
+        group: str | Group,
+    ) -> list[Dataflow]:
+        """
+        Returns a list of all dataflows from the specified Workspace.
+
+        Parameters
+        ----------
+        `group` : `str | Group`
+            Group Id or `Group` object where the Dataflow resides.
+
+        Returns
+        -------
+        `list[Dataflow]`
+            List of `Dataflow` objects from the specified Workspace.
+
+        """
+
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+
+        resource = self.BASE_URL + f"/groups/{group_id}/dataflows"
+        raw = self.get_raw(resource, self.session)
+
+        dataflows = [
+            Dataflow(
+                dataflow_js.get("objectId"),
+                self.session,
+                group_id=group_id,
+                raw=dataflow_js,
+            )
+            for dataflow_js in raw
+        ]
+
+        return dataflows
+
+    def delete_dataflow(
+        self,
+        dataflow: str | Dataflow,
+        group: str | Group,
+    ) -> None:
+        """
+        Deletes a dataflow from Power BI data prep storage, including its 
+        definition file and model.
+
+        Parameters
+        ----------
+        `dataflow` : `str | Dataflow`
+            Dataflow Id or `Dataflow` object to delete.
+        `group` : `str | Group`
+            Group Id or `Group` object where the Dataflow resides.
+        
+        """
+
+        if isinstance(dataflow, Dataflow):
+            dataflow_id = dataflow.id
+        else:
+            dataflow_id = dataflow
+        
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+        
+        resource = self.BASE_URL + f"/groups/{group_id}/dataflows/{dataflow_id}"
+
+        self.delete(resource, self.session)
+
     # TODO: Add support for passing in a group obj
     def dataset(
         self,
         dataset: str | Dataset,
         group: str = None,
     ) -> Dataset:
         """
```

### Comparing `pbipy-2.3.4/pbipy/reports.py` & `pbipy-2.4.5/pbipy/reports.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.3.4/pbipy/resources.py` & `pbipy-2.4.5/pbipy/resources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import Session
 
 from pbipy import settings
-from pbipy.utils import RequestsMixin, to_snake_case
+from pbipy.utils import RequestsMixin, to_identifier, to_snake_case
 
 
 class Resource(RequestsMixin):
     BASE_URL = settings.BASE_URL
 
     def __init__(
         self,
@@ -40,15 +40,16 @@
 
         return f"<{name} {', '.join(attrs)}>"
 
     def _load_from_raw(self, raw):
         self.raw = raw
 
         for k, v in raw.items():
-            attr = to_snake_case(k)
+            attr = to_identifier(k)
+            attr = to_snake_case(attr)
             setattr(self, attr, v)
 
         return self
 
     def load(self):
         raw = self.get_raw(self.base_path, self.session)
         self._load_from_raw(raw)
```

### Comparing `pbipy-2.3.4/pbipy/utils.py` & `pbipy-2.4.5/pbipy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,24 +79,52 @@
 
     if isinstance(directory, str):
         f_dir = Path(directory)
     elif directory is None:
         f_dir = Path()  # cwd
     else:
         f_dir = directory
-    
+
     # Be a bit more flexible and accept .ext
     if extension[0] == ".":
         f_ext = extension[1:]
     else:
         f_ext = extension
 
     return f_dir / f"{file_name}.{f_ext}"
 
 
+def to_identifier(
+    s: str,
+) -> str:
+    """
+    Convert a string into a valid Python identifier, e.g., variable or
+    attribute name.
+
+    Parameters
+    ----------
+    `s` : `str`
+        String to convert.
+
+    Returns
+    -------
+    `str`
+        Converted string.
+
+    """
+
+    # Remove leading characters until letter or underscore
+    s = re.sub("^[^a-zA-Z_]+", "", s)
+
+    # Replace invalid characters
+    s = re.sub("[^0-9a-zA-Z_]", "_", s)
+
+    return s
+
+
 class RequestsMixin:
     """
     Mixin class for http requests and response handling.
 
     Lets the PowerBI client and Resources use the same functionality for
     making requests and handling the response.
 
@@ -180,14 +208,15 @@
         return response
 
     def post(
         self,
         resource: str,
         session: Session,
         payload: dict = None,
+        params: dict = None,
         success_codes: list[int] = [200, 201, 202],
     ) -> Response:
         """
         Post data to an api endpoint.
 
         Parameters
         ----------
@@ -208,28 +237,32 @@
 
         Raises
         ------
         `HTTPError`
             If the response status code was not found in `success_codes`.
         """
 
-        response = session.post(resource, json=payload)
+        response = session.post(
+            resource,
+            params=params,
+            json=payload,
+        )
 
         if response.status_code not in success_codes:
             raise HTTPError(
                 f"Encountered api error. Response: {json.dumps(response.json(), indent=True)})"
             )
 
         return response
 
     def post_raw(
         self,
         resource: str,
         session: Session,
-        payload: dict,
+        payload: dict = None,
         **kwargs: dict,
     ) -> dict:
         """
         Make a post request and return any resulting json.
 
         Parameters
         ----------
```

### Comparing `pbipy-2.3.4/pbipy.egg-info/PKG-INFO` & `pbipy-2.4.5/pbipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.3.4
+Version: 2.4.5
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-`pbipy` supports operations for Apps, Datasets, Groups (Workspaces) and Reports, allowing users to perform actions on their PowerBI instance using Python.
+`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
 
 See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
@@ -142,24 +142,24 @@
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
 First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
 
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a group argument.
+The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
 
 ```python
 sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 print(sales)
 
 # <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the `group_id` when we call the `dataset()` method.
+But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
 
 ```python
 sales = pbi.dataset(
     "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
 ```
@@ -272,16 +272,16 @@
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
 | Reports             	| Done      |       	|
 | Apps                	| Done   	|       	|
-| Dataflows           	| Doing    	|       	|
-| Admin Operations     	| Todo     	|       	|
+| Dataflows           	| Done    	|       	|
+| Admin Operations     	| Doing    	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.3.4/setup.py` & `pbipy-2.4.5/setup.py`

 * *Files identical despite different names*

