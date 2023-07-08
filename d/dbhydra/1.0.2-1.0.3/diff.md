# Comparing `tmp/dbhydra-1.0.2.tar.gz` & `tmp/dbhydra-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.0.2.tar", last modified: Tue May 30 18:30:18 2023, max compression
+gzip compressed data, was "dbhydra-1.0.3.tar", last modified: Sat Jul  8 14:39:47 2023, max compression
```

## Comparing `dbhydra-1.0.2.tar` & `dbhydra-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.860805 dbhydra-1.0.2/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-05-30 18:30:18.859805 dbhydra-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.826894 dbhydra-1.0.2/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.2/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_builder.py
--rw-rw-rw-   0        0        0    67310 2023-05-30 18:29:17.000000 dbhydra-1.0.2/dbhydra/dbhydra_core.py
--rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_liquibase.py
--rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_model.py
--rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.2/dbhydra/dbhydra_mysql_example - kopie.py
--rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_mysql_example.py
--rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_pandas_framework.py
--rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/migrator_example.py
--rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.2/dbhydra/mongo.py
--rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.2/dbhydra/test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.857811 dbhydra-1.0.2/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.851827 dbhydra-1.0.2/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-05-30 18:30:17.000000 dbhydra-1.0.2/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 18:30:18.860805 dbhydra-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-05-30 18:29:50.000000 dbhydra-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:39:47.993871 dbhydra-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-07-08 14:39:47.993871 dbhydra-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 14:39:47.954975 dbhydra-1.0.3/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.3/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.3/dbhydra/dbhydra_builder.py
+-rw-rw-rw-   0        0        0    67814 2023-07-08 14:27:23.000000 dbhydra-1.0.3/dbhydra/dbhydra_core.py
+-rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.3/dbhydra/dbhydra_liquibase.py
+-rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.3/dbhydra/dbhydra_model.py
+-rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.3/dbhydra/dbhydra_mysql_example - kopie.py
+-rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.3/dbhydra/dbhydra_pandas_framework.py
+-rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.3/dbhydra/mongo.py
+-rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.3/dbhydra/test.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:39:47.992874 dbhydra-1.0.3/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.3/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.3/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.3/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.3/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:39:47.975139 dbhydra-1.0.3/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-07-08 14:39:47.000000 dbhydra-1.0.3/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-07-08 14:39:47.000000 dbhydra-1.0.3/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:39:47.000000 dbhydra-1.0.3/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-08 14:39:47.000000 dbhydra-1.0.3/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 14:39:47.000000 dbhydra-1.0.3/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:39:47.993871 dbhydra-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-07-08 14:39:44.000000 dbhydra-1.0.3/setup.py
```

### Comparing `dbhydra-1.0.2/LICENSE` & `dbhydra-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/PKG-INFO` & `dbhydra-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.2
+Version: 1.0.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.2/README.md` & `dbhydra-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/dbhydra_builder.py` & `dbhydra-1.0.3/dbhydra/dbhydra_builder.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/dbhydra_core.py` & `dbhydra-1.0.3/dbhydra/dbhydra_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """DB Hydra ORM"""
+import abc
+import ast
+import json
+import math
 import sys
+import threading
+from contextlib import contextmanager
+from sys import platform
+
+import numpy as np
+import pandas as pd
 import pymongo
+import pymysql as MySQLdb
+from google.cloud import bigquery
+from google.oauth2 import service_account
+from pydantic import BaseModel
 
 #! Disabled on macOS --> problematic import
 if sys.platform != "darwin":
     import pyodbc
-    
-import pandas as pd
-import numpy as np
-import pymysql as MySQLdb
-from sys import platform
+
 if platform != "linux" and platform != "linux2":
     # linux
     import psycopg2 # disable dependency for server (Temporary)
 
 
-import math
-import json
-import ast
-
-from google.cloud import bigquery
-from google.oauth2 import service_account
-
-import abc
-from contextlib import contextmanager
-
 MONGO_OPERATOR_DICT = {"=": "$eq", ">": "$gt", ">=": "$gte", " IN ": "$in", "<": "$lt", "<=": "$lte", "<>": "$ne"}
 
 POSTGRES_TO_MYSQL_DATA_MAPPING = {
     "int": "int",
     "integer": "int",
     "bigint": "bigint",
     "smallint": "smallint",
     "character varying": "varchar",
     "text": "longtext",
-    "boolean": "bit",
+    "boolean": "tinyint",
     "double precision": "double",
     "real": "float",
     "numeric": "decimal",
     "date": "date",
     "timestamp": "timestamp"
 }
 
@@ -282,14 +282,16 @@
             self.DB_PORT = None
 
         if "DB_DRIVER" in db_details.keys():
             self.DB_DRIVER = db_details["DB_DRIVER"]
         else:
             self.DB_DRIVER = "ODBC Driver 13 for SQL Server"
 
+        self.lock = threading.Lock()
+
         self.connect_to_db()
 
     @abc.abstractmethod
     def connect_locally(self):
         pass
 
     @abc.abstractmethod
@@ -457,27 +459,32 @@
 
 class Mysqldb(AbstractDB):
 
     python_database_type_mapping = PYTHON_TO_MYSQL_DATA_MAPPING = \
     {
     'int': "int",
     'float': "double",
-    'str': "nvarchar(255)",
-    'list': "nvarchar(255)",
-    'dict': "nvarchar(255)",
-    'bool': "bit",
+    'str': "varchar(255)",
+    'list': "varchar(255)",
+    'dict': "varchar(255)",
+    'bool': "tinyint",
     'datetime': "datetime"
     }
 
+    def connect_to_db(self):
+        self.connection = MySQLdb.connect(host=self.DB_SERVER, port=self.DB_PORT, user=self.DB_USERNAME, password=self.DB_PASSWORD, database=self.DB_DATABASE)
+        self.cursor = self.connection.cursor()
+
+    # NOT USED, BUT FORCED BY ABSTRACT CLASS
     def connect_locally(self):
         self.connection = MySQLdb.connect(host=self.DB_SERVER, user=self.DB_USERNAME, password=self.DB_PASSWORD,
                                           database=self.DB_DATABASE)
         self.cursor = self.connection.cursor()
         print("DB connection established")
-
+    # NOT USED, BUT FORCED BY ABSTRACT CLASS
     def connect_remotely(self):
         if self.DB_PORT is not None:
             self.connection = MySQLdb.connect(host=self.DB_SERVER, port=self.DB_PORT, user=self.DB_USERNAME,
                                               password=self.DB_PASSWORD, database=self.DB_DATABASE)
         else:
             self.connection = MySQLdb.connect(host=self.DB_SERVER, user=self.DB_USERNAME, password=self.DB_PASSWORD,
                                               database=self.DB_DATABASE)
@@ -663,15 +670,14 @@
 class AbstractSelectable:
     def __init__(self, db1, name, columns=None):
         self.db1 = db1
         self.name = name
         self.columns = columns
 
     def select(self, query):
-
         """given SELECT query returns Python list"""
         """Columns give the number of selected columns"""
         print(query)
         self.db1.cursor.execute(query)
         column_string = query.lower().split("from")[0]
         if "*" in column_string:
             columns = len(self.columns)
@@ -700,15 +706,14 @@
         for col in self.columns:
             all_cols_query = all_cols_query + col + ","
         if all_cols_query[-1] == ",":
             all_cols_query = all_cols_query[:-1]
         list1 = self.select(f"SELECT {all_cols_query} FROM " + self.name)
         return (list1)
 
-
     def select_to_df(self):
         rows = self.select_all()
         table_columns = self.columns
         demands_df = pd.DataFrame(rows, columns=table_columns)
         return (demands_df)
 
     def export_to_xlsx(self):
@@ -741,33 +746,35 @@
         return (new_joinable)
 
 
 class Joinable(Selectable):
     pass
 
 
-class AbstractTable(AbstractJoinable):
+class AbstractTable(AbstractJoinable, abc.ABC):
     def __init__(self, db1, name, columns=None, types=None):
         super().__init__(db1, name, columns)
         self.types = types
 
-    # @save_migration
+    @abc.abstractmethod
+    def init_from_column_type_dict(db1, name, column_type_dict):
+        pass
 
     def drop(self):
         query = "DROP TABLE " + self.name
         print(query)
         self.db1.execute(query)
 
     def update(self, variable_assign, where=None):
         if where is None:
             query = "UPDATE " + self.name + " SET " + variable_assign
         else:
             query = "UPDATE " + self.name + " SET " + variable_assign + " WHERE " + where
         print(query)
-        self.db1.execute(query)
+        return self.db1.execute(query)
 
     def _adjust_df(self, df: pd.DataFrame, debug_mode=False) -> pd.DataFrame:
         """
         Adjust DataFrame in case number of its columns differs from number of columns in DB table.
         :param df: original DF
         :param debug_mode: in debug mode a warning will be printed to console
         :return: adjusted DF
@@ -794,14 +801,15 @@
 
         # Ensure the same order of columns in DF as in DB table
         cols_order = [x for x in self.columns if x != 'id']
         df_copy = df_copy[cols_order]
 
         return df_copy
 
+
     def insert_from_df(self, df, batch=1, try_mode=False, debug_mode=False, adjust_df=False, insert_id=False):
 
         if adjust_df:
             df = self._adjust_df(df, debug_mode)
 
         if insert_id:
             assert len(df.columns) == len(self.columns)
@@ -838,28 +846,27 @@
         # rows = df.values.tolist()
         # for i, row in enumerate(rows):
         #     for j, record in enumerate(row):
         #         if type(record) == str:
         #             rows[i][j] = "'" + record + "'"
         #print(rows)
         rows = df.values.tolist()
-        self.insert(rows, batch=batch, try_mode=try_mode, debug_mode=False, insert_id=insert_id)
+        return self.insert(rows, batch=batch, try_mode=try_mode, debug_mode=False, insert_id=insert_id)
 
     #TODO: need to solve inserting in different column_order
     #check df column names, permute if needed
     def insert_from_column_value_dict(self, dict, insert_id=False):
         df = pd.DataFrame(dict, index=[0])
-        self.insert_from_df(df, insert_id=insert_id)
+        return self.insert_from_df(df, insert_id=insert_id)
 
     def insert_from_column_value_dict_list(self, list, insert_id=False):
         df = pd.DataFrame(list)
         self.insert_from_df(df, insert_id=insert_id)
 
 
-
     def delete(self, where=None):
 
         if where is None:
             query = "DELETE FROM " + self.name
         else:
             query = "DELETE FROM " + self.name + " WHERE " + where
         self.db1.execute(query)
@@ -1011,18 +1018,18 @@
             if k % batch == batch - 1 or k == len(rows) - 1:
                 query = query[:-1]
 
                 if debug_mode:
                     print(query)
 
                 if not try_mode:
-                    self.db1.execute(query)
+                    return self.db1.execute(query)
                 else:
                     try:
-                        self.db1.execute(query)
+                        return self.db1.execute(query)
                     except Exception as e:
 
                         print("Query", query, "Could not be inserted:", e)
 
                         # Write to logs only in debug mode
                         if debug_mode:
                             with open("log.txt", "a") as file:
@@ -1494,20 +1501,20 @@
         self.db1.execute(query)
 
     # @save_migration #TODO: Uncomment
     def create(self, foreign_keys=None):
         assert len(self.columns) == len(self.types)
         assert self.columns[0] == "id"
         assert self.types[0].lower() == "int"
-        query = "CREATE TABLE " + self.name + "(id INT UNSIGNED AUTO_INCREMENT PRIMARY KEY,"
-        for i in range(1, len(self.columns)):
-            query += self.columns[i] + " " + self.types[i] + ","
 
-        query = query[:-1]
-        query += ")"
+        column_type_pairs = list(zip(self.columns, self.types))[1:]
+        fields = ", ".join(
+            [f"{column} {type_.upper()}" for column, type_ in column_type_pairs]
+        )
+        query = f"CREATE TABLE {self.name} (id INT UNSIGNED AUTO_INCREMENT PRIMARY KEY, {fields})"
 
         print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
@@ -1775,28 +1782,26 @@
     return (dictionary)
 
 
 def dict_to_df(dictionary, column1, column2):
     df = pd.DataFrame(list(dictionary.items()), columns=[column1, column2])
     return (df)
 
-from pydantic import BaseModel
-from typing import List, Dict
 
 class AbstractModel(abc.ABC, BaseModel):
-    def generate_dbhydra_table(self, db1, name):
-        structure_dict = create_table_structure_dict(self)
-        #TODO: what type of table, TEST
-        dbhydra_table = MysqlTable(db1, name, list(structure_dict.keys()), list(structure_dict.values()))
+    @classmethod
+    def generate_dbhydra_table(cls, table_class: AbstractTable, db1, name):
+        column_type_dict = create_table_structure_dict(cls)
+        dbhydra_table = table_class.init_from_column_type_dict(db1, name, column_type_dict)
         return dbhydra_table
 
-
+ 
 
 def create_table_structure_dict(api_class_instance):
     """
     Accepts instance of API data class (e.g. APIDatabase) and converts it to dictionary {attribute_name: attribute_type}
     """
     table_structure_dict = {"id": "int"}
     table_structure_dict = {**table_structure_dict,
                             **{attribute_name: attribute_type.__name__ for attribute_name, attribute_type in api_class_instance.__annotations__.items()}}
 
-    return table_structure_dict
+    return table_structure_dict
```

### Comparing `dbhydra-1.0.2/dbhydra/dbhydra_liquibase.py` & `dbhydra-1.0.3/dbhydra/dbhydra_liquibase.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/dbhydra_model.py` & `dbhydra-1.0.3/dbhydra/dbhydra_model.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/dbhydra_pandas_framework.py` & `dbhydra-1.0.3/dbhydra/dbhydra_pandas_framework.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/mongo.py` & `dbhydra-1.0.3/dbhydra/mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/tests/test_mongo.py` & `dbhydra-1.0.3/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra/tests/test_sql.py` & `dbhydra-1.0.3/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.2/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.0.3/dbhydra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.2
+Version: 1.0.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.2/dbhydra.egg-info/SOURCES.txt` & `dbhydra-1.0.3/dbhydra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 setup.py
 dbhydra/__init__.py
 dbhydra/dbhydra_builder.py
 dbhydra/dbhydra_core.py
 dbhydra/dbhydra_liquibase.py
 dbhydra/dbhydra_model.py
 dbhydra/dbhydra_mysql_example - kopie.py
-dbhydra/dbhydra_mysql_example.py
 dbhydra/dbhydra_pandas_framework.py
-dbhydra/migrator_example.py
 dbhydra/mongo.py
 dbhydra/test.py
 dbhydra.egg-info/PKG-INFO
 dbhydra.egg-info/SOURCES.txt
 dbhydra.egg-info/dependency_links.txt
 dbhydra.egg-info/requires.txt
 dbhydra.egg-info/top_level.txt
```

### Comparing `dbhydra-1.0.2/setup.py` & `dbhydra-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.0.2',
+    version='1.0.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

