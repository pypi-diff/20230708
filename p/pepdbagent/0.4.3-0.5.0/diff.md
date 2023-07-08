# Comparing `tmp/pepdbagent-0.4.3.tar.gz` & `tmp/pepdbagent-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.4.3.tar", last modified: Fri Jun 30 21:55:04 2023, max compression
+gzip compressed data, was "pepdbagent-0.5.0.tar", last modified: Sat Jul  8 17:13:21 2023, max compression
```

## Comparing `pepdbagent-0.4.3.tar` & `pepdbagent-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 21:55:04.000000 pepdbagent-0.4.3/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:55:04.262874 pepdbagent-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-30 21:54:54.000000 pepdbagent-0.4.3/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.352859 pepdbagent-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 17:13:21.000000 pepdbagent-0.5.0/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:13:21.352859 pepdbagent-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:21.348859 pepdbagent-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-08 17:13:11.000000 pepdbagent-0.5.0/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.4.3/LICENSE.txt` & `pepdbagent-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/PKG-INFO` & `pepdbagent-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.3
+Version: 0.5.0
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.3/README.md` & `pepdbagent-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/pepdbagent/db_utils.py` & `pepdbagent-0.5.0/pepdbagent/db_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import datetime
 import logging
-from typing import Any, Optional
+from typing import Any, Optional, List
 
 from sqlalchemy import (
     BigInteger,
     FetchedValue,
     PrimaryKeyConstraint,
     Result,
     Select,
     String,
     event,
     select,
     TIMESTAMP,
+    ForeignKey,
+    ForeignKeyConstraint,
+    UniqueConstraint,
 )
 from sqlalchemy.dialects.postgresql import JSON
 from sqlalchemy.engine import URL, create_engine
 from sqlalchemy.exc import ProgrammingError
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.orm import (
     DeclarativeBase,
     Mapped,
     Session,
     mapped_column,
+    relationship,
 )
 
 from pepdbagent.const import POSTGRES_DIALECT, PKG_NAME
 from pepdbagent.exceptions import SchemaError
 
 _LOGGER = logging.getLogger(PKG_NAME)
 
@@ -57,38 +61,83 @@
         _LOGGER.info("A table was created")
     else:
         _LOGGER.info("A table was not created")
 
 
 def deliver_description(context):
     try:
-        return context.get_current_parameters()["project_value"]["_config"]["description"]
+        return context.get_current_parameters()["config"]["description"]
     except KeyError:
         return ""
 
 
+def deliver_update_date(context):
+    return datetime.datetime.now(datetime.timezone.utc)
+
+
 class Projects(Base):
+    """
+    Projects table representation in the database
+    """
+
     __tablename__ = "projects"
 
-    id: Mapped[int] = mapped_column(BIGSERIAL, server_default=FetchedValue())
-    namespace: Mapped[str] = mapped_column(primary_key=True)
-    name: Mapped[str] = mapped_column(primary_key=True)
-    tag: Mapped[str] = mapped_column(primary_key=True)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    namespace: Mapped[str] = mapped_column()
+    name: Mapped[str] = mapped_column()
+    tag: Mapped[str] = mapped_column()
     digest: Mapped[str] = mapped_column(String(32))
     description: Mapped[Optional[str]] = mapped_column(
         default=deliver_description, onupdate=deliver_description
     )
-    project_value: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
+    config: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
     private: Mapped[bool]
     number_of_samples: Mapped[int]
     submission_date: Mapped[datetime.datetime]
-    last_update_date: Mapped[datetime.datetime]
+    last_update_date: Mapped[Optional[datetime.datetime]] = mapped_column(
+        onupdate=deliver_update_date,
+    )
     pep_schema: Mapped[Optional[str]]
+    samples_mapping: Mapped[List["Samples"]] = relationship(
+        back_populates="sample_mapping", cascade="all, delete-orphan"
+    )
+    subsamples_mapping: Mapped[List["Subsamples"]] = relationship(
+        back_populates="subsample_mapping", cascade="all, delete-orphan"
+    )
+
+    __table_args__ = (UniqueConstraint("namespace", "name", "tag"),)
+
+
+class Samples(Base):
+    """
+    Samples table representation in the database
+    """
+
+    __tablename__ = "samples"
+
+    id: Mapped[int] = mapped_column(primary_key=True)
+    sample: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
+    row_number: Mapped[int]
+    project_id = mapped_column(ForeignKey("projects.id", ondelete="CASCADE"))
+    sample_mapping: Mapped["Projects"] = relationship(back_populates="samples_mapping")
+
+
+class Subsamples(Base):
+    """
+    Subsamples table representation in the database
+    """
+
+    __tablename__ = "subsamples"
 
-    __table_args__ = (PrimaryKeyConstraint("namespace", "name", "tag", name="id"),)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    subsample: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
+    subsample_number: Mapped[int]
+    row_number: Mapped[int]
+    project_id = mapped_column(ForeignKey("projects.id", ondelete="CASCADE"))
+    subsample_mapping: Mapped["Projects"] = relationship(back_populates="subsamples_mapping")
 
 
 class BaseEngine:
     """
     A class with base methods, that are used in several classes. e.g. fetch_one or fetch_all
     """
```

### Comparing `pepdbagent-0.4.3/pepdbagent/exceptions.py` & `pepdbagent-0.5.0/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/pepdbagent/models.py` & `pepdbagent-0.5.0/pepdbagent/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # file with pydantic models
 import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import peppy
 from pydantic import BaseModel, Extra, Field, validator
 
 
 class AnnotationModel(BaseModel):
     """
@@ -67,41 +67,49 @@
 
 
 class UpdateItems(BaseModel):
     """
     Model used for updating individual items in db
     """
 
-    project_value: Optional[peppy.Project] = Field(alias="project")
+    name: Optional[str]
+    description: Optional[str]
     tag: Optional[str]
     is_private: Optional[bool]
-    name: Optional[str]
     pep_schema: Optional[str]
+    digest: Optional[str]
+    config: Optional[dict]
+    samples: Optional[List[dict]]
+    subsamples: Optional[List[List[dict]]]
 
     class Config:
         arbitrary_types_allowed = True
+        extra = Extra.forbid
 
-    #     extra = Extra.forbid
+    @property
+    def number_of_samples(self) -> Union[int, None]:
+        if self.samples:
+            return len(self.samples)
+        return None
 
 
 class UpdateModel(BaseModel):
     """
     !! is Used only by pepdbagent. Don't use it outside
     Model used for updating individual items and creating sql string in the code
     """
 
-    project_value: Optional[dict]
+    config: Optional[dict]
     name: Optional[str] = None
     tag: Optional[str] = None
     private: Optional[bool] = Field(alias="is_private")
     digest: Optional[str]
-    last_update_date: Optional[datetime.datetime]
     number_of_samples: Optional[int]
     pep_schema: Optional[str]
-    description: Optional[str]
+    # last_update_date: Optional[datetime.datetime] = datetime.datetime.now(datetime.timezone.utc)
 
     @validator("tag", "name")
     def value_must_not_be_empty(cls, v):
         if "" == v:
             return None
         return v
```

### Comparing `pepdbagent-0.4.3/pepdbagent/modules/annotation.py` & `pepdbagent-0.5.0/pepdbagent/modules/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,16 @@
         admin: Union[str, List[str]] = None,
         limit: int = DEFAULT_LIMIT,
         offset: int = DEFAULT_OFFSET,
         order_by: str = "update_date",
         order_desc: bool = False,
     ) -> List[AnnotationModel]:
         """
-        Get project by providing search string.
+        Get projects by providing search string.
+
         :param namespace: namespace where to search for a project
         :param search_str: search string that has to be found in the name or tag
         :param admin: True, if user is admin of the namespace [Default: False]
         :param limit: limit of return results
         :param offset: number of results off set (that were already showed)
         :param order_by: sort the result-set by the information
             Options: ["name", "update_date", "submission_date"]
@@ -363,15 +364,15 @@
 
     def get_project_number_in_namespace(
         self,
         namespace: str,
         admin: Union[str, List[str]] = None,
     ) -> int:
         """
-        Get project by providing search string.
+        Get number of found projects by providing search string.
 
         :param namespace: namespace where to search for a project
         :param admin: True, if user is admin of the namespace [Default: False]
         :return Integer: number of projects in the namepsace
         """
         if admin is None:
             admin = []
```

### Comparing `pepdbagent-0.4.3/pepdbagent/modules/namespace.py` & `pepdbagent-0.5.0/pepdbagent/modules/namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import List, Union
 
 from sqlalchemy import distinct, func, or_, select
 from sqlalchemy.sql.selectable import Select
+from sqlalchemy.orm import Session
 
 from pepdbagent.const import DEFAULT_LIMIT, DEFAULT_OFFSET, PKG_NAME
 from pepdbagent.db_utils import Projects, BaseEngine
 from pepdbagent.models import Namespace, NamespaceList
 from pepdbagent.utils import tuple_converter
 
 _LOGGER = logging.getLogger(PKG_NAME)
@@ -92,16 +93,19 @@
         )
 
         statement = self._add_condition(
             statement=statement,
             search_str=search_str,
             admin_list=admin_nsp,
         )
+
         statement = statement.limit(limit).offset(offset)
-        query_results = self._pep_db_engine.session_execute(statement).all()
+
+        with Session(self._sa_engine) as session:
+            query_results = session.execute(statement).all()
 
         results_list = []
         for res in query_results:
             results_list.append(
                 Namespace(
                     namespace=res.namespace,
                     number_of_projects=res.number_of_projects,
@@ -122,16 +126,16 @@
             func.count(distinct(Projects.namespace)).label("number_of_namespaces")
         ).select_from(Projects)
         statement = self._add_condition(
             statement=statement,
             search_str=search_str,
             admin_list=admin_nsp,
         )
-
-        query_results = self._pep_db_engine.session_execute(statement).first()
+        with Session(self._sa_engine) as session:
+            query_results = session.execute(statement).one()
 
         return query_results.number_of_namespaces
 
     @staticmethod
     def _add_condition(
         statement: Select,
         search_str: str = None,
```

### Comparing `pepdbagent-0.4.3/pepdbagent/pepdbagent.py` & `pepdbagent-0.5.0/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/pepdbagent/utils.py` & `pepdbagent-0.5.0/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.5.0/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.4.3
+Version: 0.5.0
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.4.3/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.5.0/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/setup.py` & `pepdbagent-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.4.3/tests/conftest.py` & `pepdbagent-0.5.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,16 +32,18 @@
 
 @pytest.fixture(scope="function")
 def initiate_pepdb_con(
     list_of_available_peps,
 ):
     sa_engine = create_engine(DNS)
     with sa_engine.begin() as conn:
-        conn.execute(text("DROP table IF EXISTS projects"))
-    pepdb_con = PEPDatabaseAgent(dsn=DNS, echo=False)
+        conn.execute(text("DROP table IF EXISTS projects CASCADE"))
+        conn.execute(text("DROP table IF EXISTS samples CASCADE"))
+        conn.execute(text("DROP table IF EXISTS subsamples CASCADE"))
+    pepdb_con = PEPDatabaseAgent(dsn=DNS, echo=True)
     for namespace, item in list_of_available_peps.items():
         if namespace == "private_test":
             private = True
         else:
             private = False
         for name, path in item.items():
             prj = peppy.Project(path)
@@ -52,7 +54,25 @@
                 is_private=private,
                 project=prj,
                 overwrite=True,
                 pep_schema="random_schema_name",
             )
 
     yield pepdb_con
+
+
+@pytest.fixture(scope="function")
+def initiate_empty_pepdb_con(
+    list_of_available_peps,
+):
+    """
+    create connection without adding peps to the db
+    """
+    # sa_engine = create_engine(DNS)
+    # with sa_engine.begin() as conn:
+    #     conn.execute(text("DROP table IF EXISTS projects CASCADE"))
+    #     conn.execute(text("DROP table IF EXISTS samples CASCADE"))
+    #     conn.execute(text("DROP table IF EXISTS subsamples CASCADE"))
+
+    pepdb_con = PEPDatabaseAgent(dsn=DNS, echo=False)
+
+    yield pepdb_con
```

### Comparing `pepdbagent-0.4.3/tests/test_pepagent.py` & `pepdbagent-0.5.0/tests/test_pepagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,24 @@
 
 def get_path_to_example_file(namespace, project_name):
     return os.path.join(DATA_PATH, namespace, project_name, "project_config.yaml")
 
 
 class TestProject:
     """
-    Test project C
+    Test project methods
     """
 
+    def test_create_project(self, initiate_empty_pepdb_con, list_of_available_peps):
+        prj = peppy.Project(list_of_available_peps["namespace3"]["subtables"])
+        initiate_empty_pepdb_con.project.create(
+            prj, namespace="test", name="imply", overwrite=True
+        )
+        assert True
+
     @pytest.mark.parametrize(
         "namespace, name",
         [
             ["namespace1", "amendments1"],
             ["namespace1", "amendments2"],
             ["namespace1", "basic"],
             ["namespace2", "derive"],
@@ -51,14 +58,53 @@
         ],
     )
     def test_get_project_error(self, initiate_pepdb_con, namespace, name, tag):
         with pytest.raises(ProjectNotFoundError, match="Project does not exist."):
             kk = initiate_pepdb_con.project.get(namespace=namespace, name=name, tag=tag)
 
     @pytest.mark.parametrize(
+        "namespace, name",
+        [
+            ["namespace1", "amendments1"],
+            ["namespace1", "amendments2"],
+            ["namespace2", "derive"],
+            ["namespace2", "imply"],
+        ],
+    )
+    def test_overwrite_project(self, initiate_pepdb_con, namespace, name):
+        new_prj = initiate_pepdb_con.project.get(namespace="namespace1", name="basic")
+
+        initiate_pepdb_con.project.create(
+            project=new_prj,
+            namespace=namespace,
+            name=name,
+            tag="default",
+            overwrite=True,
+        )
+
+        assert initiate_pepdb_con.project.get(namespace=namespace, name=name) == new_prj
+
+    @pytest.mark.parametrize(
+        "namespace, name",
+        [
+            ["namespace1", "amendments1"],
+            ["namespace1", "amendments2"],
+            ["namespace2", "derive"],
+            ["namespace2", "imply"],
+        ],
+    )
+    def test_delete_project(self, initiate_pepdb_con, namespace, name):
+        initiate_pepdb_con.project.delete(namespace=namespace, name=name, tag="default")
+
+        with pytest.raises(ProjectNotFoundError, match="Project does not exist."):
+            kk = initiate_pepdb_con.project.get(namespace=namespace, name=name, tag="default")
+
+
+class TestProjectUpdate:
+    @pytest.mark.parametrize(
         "namespace, name,new_name",
         [
             ["namespace1", "amendments1", "name1"],
             ["namespace1", "amendments2", "name2"],
             ["namespace2", "derive", "name3"],
             ["namespace1", "basic", "name4"],
             ["namespace2", "derive", "name5"],
@@ -161,46 +207,32 @@
         res = initiate_pepdb_con.annotation.get(namespace, name, "default")
         assert res.results[0].pep_schema == pep_schema
 
     @pytest.mark.parametrize(
         "namespace, name",
         [
             ["namespace1", "amendments1"],
-            ["namespace1", "amendments2"],
-            ["namespace2", "derive"],
-            ["namespace2", "imply"],
         ],
     )
-    def test_overwrite_project(self, initiate_pepdb_con, namespace, name):
-        new_prj = initiate_pepdb_con.project.get(namespace="namespace1", name="basic")
-
-        initiate_pepdb_con.project.create(
-            project=new_prj,
+    def test_update_project_private(self, initiate_pepdb_con, namespace, name):
+        initiate_pepdb_con.project.update(
             namespace=namespace,
             name=name,
             tag="default",
-            overwrite=True,
+            update_dict={"is_private": True},
         )
 
-        assert initiate_pepdb_con.project.get(namespace=namespace, name=name) == new_prj
-
-    @pytest.mark.parametrize(
-        "namespace, name",
-        [
-            ["namespace1", "amendments1"],
-            ["namespace1", "amendments2"],
-            ["namespace2", "derive"],
-            ["namespace2", "imply"],
-        ],
-    )
-    def test_delete_project(self, initiate_pepdb_con, namespace, name):
-        initiate_pepdb_con.project.delete(namespace=namespace, name=name, tag="default")
-
-        with pytest.raises(ProjectNotFoundError, match="Project does not exist."):
-            kk = initiate_pepdb_con.project.get(namespace=namespace, name=name, tag="default")
+        is_private = (
+            initiate_pepdb_con.annotation.get(
+                namespace=namespace, name=name, tag="default", admin=[namespace]
+            )
+            .results[0]
+            .is_private
+        )
+        assert is_private is True
 
 
 class TestAnnotation:
     """
     Test function within annotation class
     """
```

