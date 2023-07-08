# Comparing `tmp/iam_actions-1.2.20230707.tar.gz` & `tmp/iam_actions-1.2.20230708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230707.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230708.tar", max compression
```

## Comparing `iam_actions-1.2.20230707.tar` & `iam_actions-1.2.20230708.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/README.md
--rw-r--r--   0        0        0      228 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/__init__.py
--rw-r--r--   0        0        0  4363235 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560956 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544073 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-07 02:53:43.110682 iam_actions-1.2.20230707/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230707/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230707/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/README.md
+-rw-r--r--   0        0        0      228 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4363235 2023-07-08 02:53:56.795212 iam_actions-1.2.20230708/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-08 02:52:40.983953 iam_actions-1.2.20230708/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560950 2023-07-08 02:53:56.795212 iam_actions-1.2.20230708/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-08 02:53:56.795212 iam_actions-1.2.20230708/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544067 2023-07-08 02:53:56.795212 iam_actions-1.2.20230708/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-08 02:53:57.631204 iam_actions-1.2.20230708/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230708/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230708/PKG-INFO
```

### Comparing `iam_actions-1.2.20230707/LICENSE` & `iam_actions-1.2.20230708/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/README.md` & `iam_actions-1.2.20230708/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/actions.json` & `iam_actions-1.2.20230708/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4135,217 +4135,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "StartIngestion": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAppBundles": {
             "access_level": "Undocumented",
             "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -17622,305 +17622,305 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "ListConfiguredTables": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -25323,129 +25323,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "DeleteScansByCategory": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -33019,25 +33019,25 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
@@ -33481,25 +33481,25 @@
             "access_level": "Undocumented",
             "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationEligibility": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
@@ -35151,41 +35151,41 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "GetProjectConfiguration": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProjectCredentials": {
             "access_level": "Undocumented",
             "action": "GetProjectCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListUserProjects": {
             "access_level": "Undocumented",
@@ -35193,241 +35193,241 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "datazonecontrol": {
-        "ListMetadataCollectorRuns": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectorRuns",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "ListMetadataCollectors": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssociatedDomain": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "GetAssociatedDomain",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "ListEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceByEnvironment": {
+        "ListMetadataCollectorRuns": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceByEnvironment",
+            "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllAssociatedAccountsForEnvironment": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListAllAssociatedAccountsForEnvironment",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectors": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectors",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "GetAssociatedDomain": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -57160,225 +57160,225 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "DeleteRule": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -63936,25 +63936,25 @@
             "access_level": "Undocumented",
             "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -72425,1377 +72425,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "ListServerCertificateTags": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateAccessKey": {
             "access_level": "Undocumented",
             "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -75636,25 +75636,25 @@
             "access_level": "Undocumented",
             "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInvoiceSummaries": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -81561,889 +81561,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "DisassociateWirelessGatewayFromThing": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteDeviceProfile": {
             "access_level": "Undocumented",
             "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -85251,315 +85251,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "UpdateRescoreExecutionPlan": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
             "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "EnableEnhancedMonitoring": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateStream": {
             "access_level": "Undocumented",
             "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListStreamConsumers": {
             "access_level": "Undocumented",
             "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -88145,169 +88145,169 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "CreateSettingsSet": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeProvisionedApp": {
             "access_level": "Undocumented",
             "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -96971,225 +96971,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "DeleteChannel": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -104269,251 +104269,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "ListEventRules": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "GetNotificationEvent",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeregisterNotificationHub": {
+            "access_level": "Undocumented",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNotificationConfigurations": {
             "access_level": "Undocumented",
             "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
             "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AssociateChannel": {
             "access_level": "Undocumented",
             "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNotificationEvents": {
             "access_level": "Undocumented",
             "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
-            "access_level": "Undocumented",
-            "action": "DisassociateChannel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "DeleteEventRule": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "ListEmailContacts": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -106886,49 +106886,49 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "ValidatePipeline": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StopPipeline": {
             "access_level": "Undocumented",
@@ -106942,73 +106942,73 @@
             "access_level": "Undocumented",
             "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -107623,315 +107623,315 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payment-cryptography": {
-        "DeleteKey": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateAlias": {
             "access_level": "Undocumented",
             "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "GetPaymentInstrument": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeletePaymentInstrument": {
             "access_level": "Undocumented",
             "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -113368,281 +113368,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "DeletePermission": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131219,113 +131219,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "ListAdminUsers": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSSOApplication": {
             "access_level": "Undocumented",
             "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -146323,273 +146323,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "ListSolFunctionPackages": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
             "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -148424,201 +148424,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "CreatePolicyTemplate": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSchema": {
             "access_level": "Undocumented",
             "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
             "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPolicies": {
             "access_level": "Undocumented",
             "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
```

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230708/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230708/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/generate.py` & `iam_actions-1.2.20230708/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230708/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230708/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/generate/services.py` & `iam_actions-1.2.20230708/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/policies.json` & `iam_actions-1.2.20230708/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999890350877193%*

 * *Differences: {"'serviceMap'": "{'AWS Outposts': {'ARNRegex': '^arn:aws:outposts:.+'}}"}*

```diff
@@ -7194,15 +7194,15 @@
                 "aws:TagKeys",
                 "organizations:PolicyType",
                 "organizations:ServicePrincipal"
             ]
         },
         "AWS Outposts": {
             "ARNFormat": "arn:aws:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}",
-            "ARNRegex": "^arn:aws:outposts:.+:.+:.+",
+            "ARNRegex": "^arn:aws:outposts:.+",
             "Actions": [
                 "CancelOrder",
                 "CreateOrder",
                 "CreateOutpost",
                 "CreatePrivateConnectivityConfig",
                 "CreateSite",
                 "DeleteOutpost",
```

### Comparing `iam_actions-1.2.20230707/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230708/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230707/iam_actions/services.json` & `iam_actions-1.2.20230708/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998852157943067%*

 * *Differences: {"'outposts'": "{'ARNRegexes': ['^arn:aws:outposts:.+']}"}*

```diff
@@ -14975,15 +14975,15 @@
         ]
     },
     "outposts": {
         "ARNFormats": [
             "arn:aws:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
-            "^arn:aws:outposts:.+:.+:.+"
+            "^arn:aws:outposts:.+"
         ],
         "Actions": [
             "CancelOrder",
             "CreateOrder",
             "CreateOutpost",
             "CreatePrivateConnectivityConfig",
             "CreateSite",
```

### Comparing `iam_actions-1.2.20230707/pyproject.toml` & `iam_actions-1.2.20230708/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230707"
+version = "1.2.20230708"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230707/setup.py` & `iam_actions-1.2.20230708/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230707',
+    'version': '1.2.20230708',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230707/PKG-INFO` & `iam_actions-1.2.20230708/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230707
+Version: 1.2.20230708
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

