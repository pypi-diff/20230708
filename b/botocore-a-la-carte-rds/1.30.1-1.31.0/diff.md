# Comparing `tmp/botocore-a-la-carte-rds-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-rds-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-rds-1.30.1.tar", last modified: Thu Jul  6 01:45:23 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-rds-1.31.0.tar", last modified: Fri Jul  7 01:44:15 2023, max compression
```

## Comparing `botocore-a-la-carte-rds-1.30.1.tar` & `botocore-a-la-carte-rds-1.31.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.203088 botocore-a-la-carte-rds-1.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:23.203088 botocore-a-la-carte-rds-1.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   326067 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    57903 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   968789 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/service-2.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-06 01:44:40.000000 botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:23.199088 botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:23.203088 botocore-a-la-carte-rds-1.30.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-06 01:45:23.000000 botocore-a-la-carte-rds-1.30.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.595611 botocore-a-la-carte-rds-1.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 01:44:15.595611 botocore-a-la-carte-rds-1.31.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.591611 botocore-a-la-carte-rds-1.31.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.591611 botocore-a-la-carte-rds-1.31.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.591611 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.591611 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   326067 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.595611 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57903 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   969933 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/service-2.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-07 01:43:28.000000 botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:15.595611 botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:44:15.595611 botocore-a-la-carte-rds-1.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 01:44:15.000000 botocore-a-la-carte-rds-1.31.0/setup.py
```

### Comparing `botocore-a-la-carte-rds-1.30.1/LICENSE.txt` & `botocore-a-la-carte-rds-1.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/PKG-INFO` & `botocore-a-la-carte-rds-1.31.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rds
-Version: 1.30.1
+Version: 1.31.0
 Summary: rds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/paginators-1.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/service-2.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-09-01/waiters-2.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/examples-1.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/paginators-1.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/service-2.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999662281883358%*

 * *Differences: {"'operations'": "{'CreateGlobalCluster': {'documentation': '<p>Creates an Aurora global database "*

 * *                 'spread across multiple Amazon Web Services Regions. The global database contains '*

 * *                 'a single primary cluster with read-write capability, and a read-only secondary '*

 * *                 'cluster that receives data from the primary cluster through high-speed '*

 * *                 'replication performed by the Aurora storage subsystem.</p> <p>You can create a '*

 * *                 'glob […]*

```diff
@@ -974,15 +974,15 @@
             "name": "CreateEventSubscription",
             "output": {
                 "resultWrapper": "CreateEventSubscriptionResult",
                 "shape": "CreateEventSubscriptionResult"
             }
         },
         "CreateGlobalCluster": {
-            "documentation": "<p>Creates an Aurora global database spread across multiple Amazon Web Services Regions. The global database contains a single primary cluster with read-write capability, and a read-only secondary cluster that receives data from the primary cluster through high-speed replication performed by the Aurora storage subsystem.</p> <p>You can create a global database that is initially empty, and then add a primary cluster and a secondary cluster to it. Or you can specify an existing Aurora cluster during the create operation, and this cluster becomes the primary cluster of the global database.</p> <note> <p>This action applies only to Aurora DB clusters.</p> </note>",
+            "documentation": "<p>Creates an Aurora global database spread across multiple Amazon Web Services Regions. The global database contains a single primary cluster with read-write capability, and a read-only secondary cluster that receives data from the primary cluster through high-speed replication performed by the Aurora storage subsystem.</p> <p>You can create a global database that is initially empty, and then add a primary cluster and a secondary cluster to it. Or you can specify an existing Aurora cluster during the create operation, and this cluster becomes the primary cluster of the global database.</p> <note> <p>This operation applies only to Aurora DB clusters.</p> </note>",
             "errors": [
                 {
                     "shape": "GlobalClusterAlreadyExistsFault"
                 },
                 {
                     "shape": "GlobalClusterQuotaExceededFault"
                 },
@@ -5423,15 +5423,15 @@
             },
             "type": "structure"
         },
         "CreateDBInstanceMessage": {
             "documentation": "<p/>",
             "members": {
                 "AllocatedStorage": {
-                    "documentation": "<p>The amount of storage in gibibytes (GiB) to allocate for the DB instance.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. Aurora cluster volumes automatically grow as the amount of data in your database increases, though you are only charged for the space that you use in an Aurora cluster volume.</p> <dl> <dt>Amazon RDS Custom</dt> <dt>RDS for MariaDB</dt> <dt>RDS for MySQL</dt> <dt>RDS for Oracle</dt> <dt>RDS for PostgreSQL</dt> <dt>RDS for SQL Server</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 40 to 65536 for RDS Custom for Oracle, 16384 for RDS Custom for SQL Server.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 40 to 65536 for RDS Custom for Oracle, 16384 for RDS Custom for SQL Server.</p> </li> </ul> </dd> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 10 to 3072.</p> </li> </ul> </dd> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 20 to 16384.</p> </li> <li> <p>Web and Express editions: Must be an integer from 20 to 16384.</p> </li> </ul> </li> <li> <p>Provisioned IOPS storage (io1):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 100 to 16384.</p> </li> <li> <p>Web and Express editions: Must be an integer from 100 to 16384.</p> </li> </ul> </li> <li> <p>Magnetic storage (standard):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 20 to 1024.</p> </li> <li> <p>Web and Express editions: Must be an integer from 20 to 1024.</p> </li> </ul> </li> </ul> </dd> </dl>",
+                    "documentation": "<p>The amount of storage in gibibytes (GiB) to allocate for the DB instance.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. Aurora cluster volumes automatically grow as the amount of data in your database increases, though you are only charged for the space that you use in an Aurora cluster volume.</p> <dl> <dt>Amazon RDS Custom</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 40 to 65536 for RDS Custom for Oracle, 16384 for RDS Custom for SQL Server.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 40 to 65536 for RDS Custom for Oracle, 16384 for RDS Custom for SQL Server.</p> </li> </ul> </dd> <dt>RDS for MariaDB</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dt>RDS for MySQL</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dt>RDS for Oracle</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 10 to 3072.</p> </li> </ul> </dd> <dt>RDS for PostgreSQL</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3): Must be an integer from 20 to 65536.</p> </li> <li> <p>Provisioned IOPS storage (io1): Must be an integer from 100 to 65536.</p> </li> <li> <p>Magnetic storage (standard): Must be an integer from 5 to 3072.</p> </li> </ul> </dd> <dt>RDS for SQL Server</dt> <dd> <p>Constraints to the amount of storage for each storage type are the following:</p> <ul> <li> <p>General Purpose (SSD) storage (gp2, gp3):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 20 to 16384.</p> </li> <li> <p>Web and Express editions: Must be an integer from 20 to 16384.</p> </li> </ul> </li> <li> <p>Provisioned IOPS storage (io1):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 100 to 16384.</p> </li> <li> <p>Web and Express editions: Must be an integer from 100 to 16384.</p> </li> </ul> </li> <li> <p>Magnetic storage (standard):</p> <ul> <li> <p>Enterprise and Standard editions: Must be an integer from 20 to 1024.</p> </li> <li> <p>Web and Express editions: Must be an integer from 20 to 1024.</p> </li> </ul> </li> </ul> </dd> </dl>",
                     "shape": "IntegerOptional"
                 },
                 "AutoMinorVersionUpgrade": {
                     "documentation": "<p>Specifies whether minor engine upgrades are applied automatically to the DB instance during the maintenance window. By default, minor engine upgrades are applied automatically.</p> <p>If you create an RDS Custom DB instance, you must set <code>AutoMinorVersionUpgrade</code> to <code>false</code>.</p>",
                     "shape": "BooleanOptional"
                 },
                 "AvailabilityZone": {
@@ -5451,15 +5451,15 @@
                     "shape": "String"
                 },
                 "CharacterSetName": {
                     "documentation": "<p>For supported engines, the character set (<code>CharacterSet</code>) to associate the DB instance with.</p> <p>This setting doesn't apply to the following DB instances:</p> <ul> <li> <p>Amazon Aurora - The character set is managed by the DB cluster. For more information, see <code>CreateDBCluster</code>.</p> </li> <li> <p>RDS Custom - However, if you need to change the character set, you can change it on the database itself.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "CopyTagsToSnapshot": {
-                    "documentation": "<p>Spcifies whether to copy tags from the DB instance to snapshots of the DB instance. By default, tags are not copied.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. Copying tags to snapshots is managed by the DB cluster. Setting this value for an Aurora DB instance has no effect on the DB cluster setting.</p>",
+                    "documentation": "<p>Specifies whether to copy tags from the DB instance to snapshots of the DB instance. By default, tags are not copied.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. Copying tags to snapshots is managed by the DB cluster. Setting this value for an Aurora DB instance has no effect on the DB cluster setting.</p>",
                     "shape": "BooleanOptional"
                 },
                 "CustomIamInstanceProfile": {
                     "documentation": "<p>The instance profile associated with the underlying Amazon EC2 instance of an RDS Custom DB instance.</p> <p>This setting is required for RDS Custom.</p> <p>Constraints:</p> <ul> <li> <p>The profile must exist in your account.</p> </li> <li> <p>The profile must have an IAM role that Amazon EC2 has permissions to assume.</p> </li> <li> <p>The instance profile name and the associated IAM role name must start with the prefix <code>AWSRDSCustom</code>.</p> </li> </ul> <p>For the list of permissions required for the IAM role, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/custom-setup-orcl.html#custom-setup-orcl.iam-vpc\"> Configure IAM and your VPC</a> in the <i>Amazon RDS User Guide</i>.</p>",
                     "shape": "String"
                 },
                 "DBClusterIdentifier": {
@@ -5471,15 +5471,15 @@
                     "shape": "String"
                 },
                 "DBInstanceIdentifier": {
                     "documentation": "<p>The identifier for this DB instance. This parameter is stored as a lowercase string.</p> <p>Constraints:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>First character must be a letter.</p> </li> <li> <p>Can't end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p>Example: <code>mydbinstance</code> </p>",
                     "shape": "String"
                 },
                 "DBName": {
-                    "documentation": "<p>The meaning of this parameter differs depending on the database engine.</p> <dl> <dt>Amazon Aurora MySQL</dt> <dt>Amazon Aurora PostgreSQL</dt> <dt>Amazon RDS Custom for Oracle</dt> <dt>Amazon RDS Custom for SQL Server</dt> <dt>RDS for MariaDB</dt> <dt>RDS for MySQL</dt> <dt>RDS for Oracle</dt> <dt>RDS for PostgreSQL</dt> <dt>RDS for SQL Server</dt> <dd> <p>The name of the database to create when the primary DB instance of the Aurora MySQL DB cluster is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 alphanumeric characters.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>The name of the database to create when the primary DB instance of the Aurora PostgreSQL DB cluster is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 alphanumeric characters.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0 to 9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>The Oracle System ID (SID) of the created RDS Custom DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 8 alphanumeric characters.</p> </li> <li> <p>Must contain a letter.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>Not applicable. Must be null.</p> </dd> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>The Oracle System ID (SID) of the created DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 8 characters.</p> </li> <li> <p>Can't be a word reserved by the database engine, such as the string <code>NULL</code>.</p> </li> </ul> </dd> <dd> <p>The name of the database to create when the DB instance is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 letters, numbers, or underscores.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dd> <p>Not applicable. Must be null.</p> </dd> </dl>",
+                    "documentation": "<p>The meaning of this parameter differs depending on the database engine.</p> <dl> <dt>Amazon Aurora MySQL</dt> <dd> <p>The name of the database to create when the primary DB instance of the Aurora MySQL DB cluster is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 alphanumeric characters.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon Aurora PostgreSQL</dt> <dd> <p>The name of the database to create when the primary DB instance of the Aurora PostgreSQL DB cluster is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 alphanumeric characters.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0 to 9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon RDS Custom for Oracle</dt> <dd> <p>The Oracle System ID (SID) of the created RDS Custom DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 8 alphanumeric characters.</p> </li> <li> <p>Must contain a letter.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon RDS Custom for SQL Server</dt> <dd> <p>Not applicable. Must be null.</p> </dd> <dt>RDS for MariaDB</dt> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for MySQL</dt> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for Oracle</dt> <dd> <p>The Oracle System ID (SID) of the created DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 8 characters.</p> </li> <li> <p>Can't be a word reserved by the database engine, such as the string <code>NULL</code>.</p> </li> </ul> </dd> <dt>RDS for PostgreSQL</dt> <dd> <p>The name of the database to create when the DB instance is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 letters, numbers, or underscores.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for SQL Server</dt> <dd> <p>Not applicable. Must be null.</p> </dd> </dl>",
                     "shape": "String"
                 },
                 "DBParameterGroupName": {
                     "documentation": "<p>The name of the DB parameter group to associate with this DB instance. If you don't specify a value, then Amazon RDS uses the default DB parameter group for the specified DB engine and version.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p> <p>Constraints:</p> <ul> <li> <p>Must be 1 to 255 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Can't end with a hyphen or contain two consecutive hyphens.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DBSecurityGroups": {
@@ -5495,31 +5495,31 @@
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>The Active Directory directory ID to create the DB instance in. Currently, only Microsoft SQL Server, MySQL, Oracle, and PostgreSQL DB instances can be created in an Active Directory Domain.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to the following DB instances:</p> <ul> <li> <p>Amazon Aurora (The domain is managed by the DB cluster.)</p> </li> <li> <p>RDS Custom</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DomainAuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user joining the domain.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
                     "shape": "String"
                 },
                 "DomainDnsIps": {
                     "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p> <p>Constraints:</p> <ul> <li> <p>Two IP addresses must be provided. If there isn't a secondary domain controller, use the IP address of the primary domain controller for both entries in the list.</p> </li> </ul> <p>Example: <code>123.124.125.126,234.235.236.237</code> </p>",
                     "shape": "StringList"
                 },
                 "DomainFqdn": {
-                    "documentation": "<p>Specifies the fully qualified domain name of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
+                    "documentation": "<p>The fully qualified domain name (FQDN) of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
                     "shape": "String"
                 },
                 "DomainIAMRoleName": {
                     "documentation": "<p>The name of the IAM role to use when making API calls to the Directory Service.</p> <p>This setting doesn't apply to the following DB instances:</p> <ul> <li> <p>Amazon Aurora (The domain is managed by the DB cluster.)</p> </li> <li> <p>RDS Custom</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DomainOu": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
+                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
                     "shape": "String"
                 },
                 "EnableCloudwatchLogsExports": {
                     "documentation": "<p>The list of log types that need to be enabled for exporting to CloudWatch Logs. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_LogAccess.html#USER_LogAccess.Procedural.UploadtoCloudWatch\"> Publishing Database Logs to Amazon CloudWatch Logs</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to the following DB instances:</p> <ul> <li> <p>Amazon Aurora (CloudWatch Logs exports are managed by the DB cluster.)</p> </li> <li> <p>RDS Custom</p> </li> </ul> <p>The following values are valid for each DB engine:</p> <ul> <li> <p>RDS for MariaDB - <code>audit | error | general | slowquery</code> </p> </li> <li> <p>RDS for Microsoft SQL Server - <code>agent | error</code> </p> </li> <li> <p>RDS for MySQL - <code>audit | error | general | slowquery</code> </p> </li> <li> <p>RDS for Oracle - <code>alert | audit | listener | trace | oemagent</code> </p> </li> <li> <p>RDS for PostgreSQL - <code>postgresql | upgrade</code> </p> </li> </ul>",
                     "shape": "LogTypeList"
                 },
                 "EnableCustomerOwnedIp": {
@@ -5535,15 +5535,15 @@
                     "shape": "BooleanOptional"
                 },
                 "Engine": {
                     "documentation": "<p>The database engine to use for this DB instance.</p> <p>Not every database engine is available in every Amazon Web Services Region.</p> <p>Valid Values:</p> <ul> <li> <p> <code>aurora-mysql</code> (for Aurora MySQL DB instances)</p> </li> <li> <p> <code>aurora-postgresql</code> (for Aurora PostgreSQL DB instances)</p> </li> <li> <p> <code>custom-oracle-ee</code> (for RDS Custom for Oracle DB instances)</p> </li> <li> <p> <code>custom-oracle-ee-cdb</code> (for RDS Custom for Oracle DB instances)</p> </li> <li> <p> <code>custom-sqlserver-ee</code> (for RDS Custom for SQL Server DB instances)</p> </li> <li> <p> <code>custom-sqlserver-se</code> (for RDS Custom for SQL Server DB instances)</p> </li> <li> <p> <code>custom-sqlserver-web</code> (for RDS Custom for SQL Server DB instances)</p> </li> <li> <p> <code>mariadb</code> </p> </li> <li> <p> <code>mysql</code> </p> </li> <li> <p> <code>oracle-ee</code> </p> </li> <li> <p> <code>oracle-ee-cdb</code> </p> </li> <li> <p> <code>oracle-se2</code> </p> </li> <li> <p> <code>oracle-se2-cdb</code> </p> </li> <li> <p> <code>postgres</code> </p> </li> <li> <p> <code>sqlserver-ee</code> </p> </li> <li> <p> <code>sqlserver-se</code> </p> </li> <li> <p> <code>sqlserver-ex</code> </p> </li> <li> <p> <code>sqlserver-web</code> </p> </li> </ul>",
                     "shape": "String"
                 },
                 "EngineVersion": {
-                    "documentation": "<p>The version number of the database engine to use.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. The version number of the database engine the DB instance uses is managed by the DB cluster.</p> <p>For a list of valid engine versions, use the <code>DescribeDBEngineVersions</code> operation.</p> <p>The following are the database engines and links to information about the major and minor versions that are available with Amazon RDS. Not every database engine is available for every Amazon Web Services Region.</p> <dl> <dt>Amazon RDS Custom for Oracle</dt> <dt>Amazon RDS Custom for SQL Server</dt> <dt>RDS for MariaDB</dt> <dt>RDS for Microsoft SQL Server</dt> <dt>RDS for MySQL</dt> <dt>RDS for Oracle</dt> <dt>RDS for PostgreSQL</dt> <dd> <p>A custom engine version (CEV) that you have previously created. This setting is required for RDS Custom for Oracle. The CEV name has the following format: 19.<i>customized_string</i>. A valid CEV name is <code>19.my_cev1</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/custom-creating.html#custom-creating.create\"> Creating an RDS Custom for Oracle DB instance</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>See <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/custom-reqs-limits-MS.html\">RDS Custom for SQL Server general requirements</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MariaDB.html#MariaDB.Concepts.VersionMgmt\">MariaDB on Amazon RDS versions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SQLServer.html#SQLServer.Concepts.General.VersionSupport\">Microsoft SQL Server versions on Amazon RDS</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MySQL.html#MySQL.Concepts.VersionMgmt\">MySQL on Amazon RDS versions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Appendix.Oracle.PatchComposition.html\">Oracle Database Engine release notes</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html#PostgreSQL.Concepts\">Amazon RDS for PostgreSQL versions and extensions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> </dl>",
+                    "documentation": "<p>The version number of the database engine to use.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. The version number of the database engine the DB instance uses is managed by the DB cluster.</p> <p>For a list of valid engine versions, use the <code>DescribeDBEngineVersions</code> operation.</p> <p>The following are the database engines and links to information about the major and minor versions that are available with Amazon RDS. Not every database engine is available for every Amazon Web Services Region.</p> <dl> <dt>Amazon RDS Custom for Oracle</dt> <dd> <p>A custom engine version (CEV) that you have previously created. This setting is required for RDS Custom for Oracle. The CEV name has the following format: 19.<i>customized_string</i>. A valid CEV name is <code>19.my_cev1</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/custom-creating.html#custom-creating.create\"> Creating an RDS Custom for Oracle DB instance</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>Amazon RDS Custom for SQL Server</dt> <dd> <p>See <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/custom-reqs-limits-MS.html\">RDS Custom for SQL Server general requirements</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>RDS for MariaDB</dt> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MariaDB.html#MariaDB.Concepts.VersionMgmt\">MariaDB on Amazon RDS versions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>RDS for Microsoft SQL Server</dt> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SQLServer.html#SQLServer.Concepts.General.VersionSupport\">Microsoft SQL Server versions on Amazon RDS</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>RDS for MySQL</dt> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_MySQL.html#MySQL.Concepts.VersionMgmt\">MySQL on Amazon RDS versions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>RDS for Oracle</dt> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Appendix.Oracle.PatchComposition.html\">Oracle Database Engine release notes</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> <dt>RDS for PostgreSQL</dt> <dd> <p>For information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html#PostgreSQL.Concepts\">Amazon RDS for PostgreSQL versions and extensions</a> in the <i>Amazon RDS User Guide</i>.</p> </dd> </dl>",
                     "shape": "String"
                 },
                 "Iops": {
                     "documentation": "<p>The amount of Provisioned IOPS (input/output operations per second) to initially allocate for the DB instance. For information about valid IOPS values, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_Storage.html\">Amazon RDS DB instance storage</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. Storage is managed by the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>For RDS for MariaDB, MySQL, Oracle, and PostgreSQL - Must be a multiple between .5 and 50 of the storage amount for the DB instance.</p> </li> <li> <p>For RDS for SQL Server - Must be a multiple between 1 and 50 of the storage amount for the DB instance.</p> </li> </ul>",
                     "shape": "IntegerOptional"
                 },
                 "KmsKeyId": {
@@ -5713,31 +5713,31 @@
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>The Active Directory directory ID to create the DB instance in. Currently, only MySQL, Microsoft SQL Server, Oracle, and PostgreSQL DB instances can be created in an Active Directory Domain.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "String"
                 },
                 "DomainAuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user joining the domain.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
                     "shape": "String"
                 },
                 "DomainDnsIps": {
                     "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p> <p>Constraints:</p> <ul> <li> <p>Two IP addresses must be provided. If there isn't a secondary domain controller, use the IP address of the primary domain controller for both entries in the list.</p> </li> </ul> <p>Example: <code>123.124.125.126,234.235.236.237</code> </p>",
                     "shape": "StringList"
                 },
                 "DomainFqdn": {
-                    "documentation": "<p>Specifies the fully qualified domain name of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
+                    "documentation": "<p>The fully qualified domain name (FQDN) of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
                     "shape": "String"
                 },
                 "DomainIAMRoleName": {
                     "documentation": "<p>The name of the IAM role to be used when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "String"
                 },
                 "DomainOu": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
+                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
                     "shape": "String"
                 },
                 "EnableCloudwatchLogsExports": {
                     "documentation": "<p>The list of logs that the new DB instance is to export to CloudWatch Logs. The values in the list depend on the DB engine being used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_LogAccess.html#USER_LogAccess.Procedural.UploadtoCloudWatch\">Publishing Database Logs to Amazon CloudWatch Logs </a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "LogTypeList"
                 },
                 "EnableCustomerOwnedIp": {
@@ -6137,39 +6137,39 @@
                 }
             },
             "type": "structure"
         },
         "CreateGlobalClusterMessage": {
             "members": {
                 "DatabaseName": {
-                    "documentation": "<p>The name for your database of up to 64 alphanumeric characters. If you do not provide a name, Amazon Aurora will not create a database in the global database cluster you are creating.</p>",
+                    "documentation": "<p>The name for your database of up to 64 alphanumeric characters. If you don't specify a name, Amazon Aurora doesn't create a database in the global database cluster.</p> <p>Constraints:</p> <ul> <li> <p>Can't be specified if <code>SourceDBClusterIdentifier</code> is specified. In this case, Amazon Aurora uses the database name from the source DB cluster.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DeletionProtection": {
-                    "documentation": "<p>The deletion protection setting for the new global database. The global database can't be deleted when deletion protection is enabled.</p>",
+                    "documentation": "<p>Specifies whether to enable deletion protection for the new global database cluster. The global database can't be deleted when deletion protection is enabled.</p>",
                     "shape": "BooleanOptional"
                 },
                 "Engine": {
-                    "documentation": "<p>The name of the database engine to be used for this DB cluster.</p>",
+                    "documentation": "<p>The database engine to use for this global database cluster.</p> <p>Valid Values: <code>aurora-mysql | aurora-postgresql</code> </p> <p>Constraints:</p> <ul> <li> <p>Can't be specified if <code>SourceDBClusterIdentifier</code> is specified. In this case, Amazon Aurora uses the engine of the source DB cluster.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "EngineVersion": {
-                    "documentation": "<p>The engine version of the Aurora global database.</p>",
+                    "documentation": "<p>The engine version to use for this global database cluster.</p> <p>Constraints:</p> <ul> <li> <p>Can't be specified if <code>SourceDBClusterIdentifier</code> is specified. In this case, Amazon Aurora uses the engine version of the source DB cluster.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "GlobalClusterIdentifier": {
-                    "documentation": "<p>The cluster identifier of the new global database cluster. This parameter is stored as a lowercase string.</p>",
+                    "documentation": "<p>The cluster identifier for this global database cluster. This parameter is stored as a lowercase string.</p>",
                     "shape": "String"
                 },
                 "SourceDBClusterIdentifier": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) to use as the primary cluster of the global database. This parameter is optional.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) to use as the primary cluster of the global database.</p> <p>If you provide a value for this parameter, don't specify values for the following settings because Amazon Aurora uses the values from the specified source DB cluster:</p> <ul> <li> <p> <code>DatabaseName</code> </p> </li> <li> <p> <code>Engine</code> </p> </li> <li> <p> <code>EngineVersion</code> </p> </li> <li> <p> <code>StorageEncrypted</code> </p> </li> </ul>",
                     "shape": "String"
                 },
                 "StorageEncrypted": {
-                    "documentation": "<p>The storage encryption setting for the new global database cluster.</p>",
+                    "documentation": "<p>Specifies whether to enable storage encryption for the new global database cluster.</p> <p>Constraints:</p> <ul> <li> <p>Can't be specified if <code>SourceDBClusterIdentifier</code> is specified. In this case, Amazon Aurora uses the setting from the source DB cluster.</p> </li> </ul>",
                     "shape": "BooleanOptional"
                 }
             },
             "type": "structure"
         },
         "CreateGlobalClusterResult": {
             "members": {
@@ -10515,39 +10515,39 @@
             "pattern": ".*",
             "type": "string"
         },
         "DomainMembership": {
             "documentation": "<p>An Active Directory Domain membership record associated with the DB instance or cluster.</p>",
             "members": {
                 "AuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user that's a member of the domain.</p>",
                     "shape": "String"
                 },
                 "DnsIps": {
-                    "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p>",
+                    "documentation": "<p>The IPv4 DNS IP addresses of the primary and secondary Active Directory domain controllers.</p>",
                     "shape": "StringList"
                 },
                 "Domain": {
                     "documentation": "<p>The identifier of the Active Directory Domain.</p>",
                     "shape": "String"
                 },
                 "FQDN": {
                     "documentation": "<p>The fully qualified domain name (FQDN) of the Active Directory Domain.</p>",
                     "shape": "String"
                 },
                 "IAMRoleName": {
-                    "documentation": "<p>The name of the IAM role to be used when making API calls to the Directory Service.</p>",
+                    "documentation": "<p>The name of the IAM role used when making API calls to the Directory Service.</p>",
                     "shape": "String"
                 },
                 "OU": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p>",
+                    "documentation": "<p>The Active Directory organizational unit for the DB instance or cluster.</p>",
                     "shape": "String"
                 },
                 "Status": {
-                    "documentation": "<p>The status of the Active Directory Domain membership for the DB instance or cluster. Values include joined, pending-join, failed, and so on.</p>",
+                    "documentation": "<p>The status of the Active Directory Domain membership for the DB instance or cluster. Values include <code>joined</code>, <code>pending-join</code>, <code>failed</code>, and so on.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "DomainMembershipList": {
             "member": {
@@ -12206,39 +12206,39 @@
                     "shape": "String"
                 },
                 "DeletionProtection": {
                     "documentation": "<p>Specifies whether the DB instance has deletion protection enabled. The database can't be deleted when deletion protection is enabled. By default, deletion protection isn't enabled. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_DeleteInstance.html\"> Deleting a DB Instance</a>.</p>",
                     "shape": "BooleanOptional"
                 },
                 "DisableDomain": {
-                    "documentation": "<p>Boolean. If present, removes the instance from the Active Directory domain.</p>",
+                    "documentation": "<p>Specifies whether to remove the DB instance from the Active Directory domain.</p>",
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>The Active Directory directory ID to move the DB instance to. Specify <code>none</code> to remove the instance from its current domain. You must create the domain before this operation. Currently, you can create only MySQL, Microsoft SQL Server, Oracle, and PostgreSQL DB instances in an Active Directory Domain.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p>",
                     "shape": "String"
                 },
                 "DomainAuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user joining the domain.</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
                     "shape": "String"
                 },
                 "DomainDnsIps": {
                     "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p> <p>Constraints:</p> <ul> <li> <p>Two IP addresses must be provided. If there isn't a secondary domain controller, use the IP address of the primary domain controller for both entries in the list.</p> </li> </ul> <p>Example: <code>123.124.125.126,234.235.236.237</code> </p>",
                     "shape": "StringList"
                 },
                 "DomainFqdn": {
-                    "documentation": "<p>Specifies the fully qualified domain name of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
+                    "documentation": "<p>The fully qualified domain name (FQDN) of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
                     "shape": "String"
                 },
                 "DomainIAMRoleName": {
                     "documentation": "<p>The name of the IAM role to use when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p>",
                     "shape": "String"
                 },
                 "DomainOu": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
+                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
                     "shape": "String"
                 },
                 "EnableCustomerOwnedIp": {
                     "documentation": "<p>Specifies whether to enable a customer-owned IP address (CoIP) for an RDS on Outposts DB instance.</p> <p>A <i>CoIP</i> provides local or external connectivity to resources in your Outpost subnets through your on-premises network. For some use cases, a CoIP can provide lower latency for connections to the DB instance from outside of its virtual private cloud (VPC) on your local network.</p> <p>For more information about RDS on Outposts, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/rds-on-outposts.html\">Working with Amazon RDS on Amazon Web Services Outposts</a> in the <i>Amazon RDS User Guide</i>.</p> <p>For more information about CoIPs, see <a href=\"https://docs.aws.amazon.com/outposts/latest/userguide/routing.html#ip-addressing\">Customer-owned IP addresses</a> in the <i>Amazon Web Services Outposts User Guide</i>.</p>",
                     "shape": "BooleanOptional"
                 },
                 "EnableIAMDatabaseAuthentication": {
@@ -14705,31 +14705,31 @@
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>Specify the Active Directory directory ID to restore the DB instance in. The domain/ must be created prior to this operation. Currently, you can create only MySQL, Microsoft SQL Server, Oracle, and PostgreSQL DB instances in an Active Directory Domain.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "String"
                 },
                 "DomainAuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p> <p>Constraints:</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user joining the domain.</p> <p>Constraints:</p> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
                     "shape": "String"
                 },
                 "DomainDnsIps": {
                     "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p> <p>Constraints:</p> <ul> <li> <p>Two IP addresses must be provided. If there isn't a secondary domain controller, use the IP address of the primary domain controller for both entries in the list.</p> </li> </ul> <p>Example: <code>123.124.125.126,234.235.236.237</code> </p>",
                     "shape": "StringList"
                 },
                 "DomainFqdn": {
-                    "documentation": "<p>Specifies the fully qualified domain name of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
+                    "documentation": "<p>The fully qualified domain name (FQDN) of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
                     "shape": "String"
                 },
                 "DomainIAMRoleName": {
-                    "documentation": "<p>Specify the name of the IAM role to be used when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom.</p>",
+                    "documentation": "<p>The name of the IAM role to use when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p>",
                     "shape": "String"
                 },
                 "DomainOu": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
+                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
                     "shape": "String"
                 },
                 "EnableCloudwatchLogsExports": {
                     "documentation": "<p>The list of logs that the restored DB instance is to export to CloudWatch Logs. The values in the list depend on the DB engine being used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_LogAccess.html#USER_LogAccess.Procedural.UploadtoCloudWatch\">Publishing Database Logs to Amazon CloudWatch Logs</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "LogTypeList"
                 },
                 "EnableCustomerOwnedIp": {
@@ -15079,31 +15079,31 @@
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>Specify the Active Directory directory ID to restore the DB instance in. Create the domain before running this command. Currently, you can create only the MySQL, Microsoft SQL Server, Oracle, and PostgreSQL DB instances in an Active Directory Domain.</p> <p>This setting doesn't apply to RDS Custom.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p>",
                     "shape": "String"
                 },
                 "DomainAuthSecretArn": {
-                    "documentation": "<p>The ARN for the Secrets Manager secret that contains the credentials for the user performing the domain join.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
+                    "documentation": "<p>The ARN for the Secrets Manager secret with the credentials for the user joining the domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>arn:aws:secretsmanager:region:account-number:secret:myselfmanagedADtestsecret-123456</code> </p>",
                     "shape": "String"
                 },
                 "DomainDnsIps": {
                     "documentation": "<p>The IPv4 DNS IP addresses of your primary and secondary Active Directory domain controllers.</p> <p>Constraints:</p> <ul> <li> <p>Two IP addresses must be provided. If there isn't a secondary domain controller, use the IP address of the primary domain controller for both entries in the list.</p> </li> </ul> <p>Example: <code>123.124.125.126,234.235.236.237</code> </p>",
                     "shape": "StringList"
                 },
                 "DomainFqdn": {
-                    "documentation": "<p>Specifies the fully qualified domain name of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
+                    "documentation": "<p>The fully qualified domain name (FQDN) of an Active Directory domain.</p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>mymanagedADtest.mymanagedAD.mydomain</code> </p>",
                     "shape": "String"
                 },
                 "DomainIAMRoleName": {
-                    "documentation": "<p>Specify the name of the IAM role to be used when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom.</p>",
+                    "documentation": "<p>The name of the IAM role to use when making API calls to the Directory Service.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p>",
                     "shape": "String"
                 },
                 "DomainOu": {
-                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Cannot be greater than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
+                    "documentation": "<p>The Active Directory organizational unit for your DB instance to join.</p> <p>Constraints:</p> <ul> <li> <p>Must be in the distinguished name format.</p> </li> <li> <p>Can't be longer than 64 characters.</p> </li> </ul> <p>Example: <code>OU=mymanagedADtestOU,DC=mymanagedADtest,DC=mymanagedAD,DC=mydomain</code> </p>",
                     "shape": "String"
                 },
                 "EnableCloudwatchLogsExports": {
                     "documentation": "<p>The list of logs that the restored DB instance is to export to CloudWatch Logs. The values in the list depend on the DB engine being used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_LogAccess.html#USER_LogAccess.Procedural.UploadtoCloudWatch\">Publishing Database Logs to Amazon CloudWatch Logs</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to RDS Custom.</p>",
                     "shape": "LogTypeList"
                 },
                 "EnableCustomerOwnedIp": {
```

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/service-2.sdk-extras.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/service-2.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore/data/rds/2014-10-31/waiters-2.json` & `botocore-a-la-carte-rds-1.31.0/botocore/data/rds/2014-10-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/PKG-INFO` & `botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rds
-Version: 1.30.1
+Version: 1.31.0
 Summary: rds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rds-1.30.1/botocore_a_la_carte_rds.egg-info/SOURCES.txt` & `botocore-a-la-carte-rds-1.31.0/botocore_a_la_carte_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.30.1/setup.py` & `botocore-a-la-carte-rds-1.31.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-rds',
-    version="1.30.1",
+    version="1.31.0",
     description='rds data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/rds/*/*.json'],
```

