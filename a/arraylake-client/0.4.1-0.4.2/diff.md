# Comparing `tmp/arraylake_client-0.4.1.tar.gz` & `tmp/arraylake_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake_client-0.4.1.tar", max compression
+gzip compressed data, was "arraylake_client-0.4.2.tar", max compression
```

## Comparing `arraylake_client-0.4.1.tar` & `arraylake_client-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      654 2023-06-13 15:51:53.886016 arraylake_client-0.4.1/README.md
--rw-r--r--   0        0        0      357 2023-06-07 16:41:28.210985 arraylake_client-0.4.1/arraylake_client/__init__.py
--rw-r--r--   0        0        0       70 2023-06-07 16:41:28.212174 arraylake_client-0.4.1/arraylake_client/__main__.py
--rw-r--r--   0        0        0    15114 2023-06-15 22:59:38.849767 arraylake_client-0.4.1/arraylake_client/api_utils.py
--rw-r--r--   0        0        0      630 2023-06-07 16:41:28.212923 arraylake_client-0.4.1/arraylake_client/chunkstore/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-07 16:41:28.213251 arraylake_client-0.4.1/arraylake_client/chunkstore/abc.py
--rw-r--r--   0        0        0     5201 2023-06-07 16:41:28.213373 arraylake_client-0.4.1/arraylake_client/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2023-06-07 16:41:28.213456 arraylake_client-0.4.1/arraylake_client/cli/__init__.py
--rw-r--r--   0        0        0     3822 2023-06-07 16:41:28.213758 arraylake_client-0.4.1/arraylake_client/cli/auth.py
--rw-r--r--   0        0        0     4762 2023-06-07 16:41:28.213838 arraylake_client-0.4.1/arraylake_client/cli/config.py
--rw-r--r--   0        0        0     1155 2023-06-07 16:41:28.213908 arraylake_client-0.4.1/arraylake_client/cli/main.py
--rw-r--r--   0        0        0     3568 2023-06-13 00:03:11.754464 arraylake_client-0.4.1/arraylake_client/cli/repo.py
--rw-r--r--   0        0        0     3390 2023-06-07 16:41:28.214762 arraylake_client-0.4.1/arraylake_client/cli/utils.py
--rw-r--r--   0        0        0     6402 2023-06-15 22:59:33.395642 arraylake_client-0.4.1/arraylake_client/client.py
--rw-r--r--   0        0        0     7098 2023-06-13 00:03:11.755118 arraylake_client-0.4.1/arraylake_client/commits.py
--rw-r--r--   0        0        0      538 2023-06-07 16:41:28.215453 arraylake_client-0.4.1/arraylake_client/config.py
--rw-r--r--   0        0        0      105 2023-06-07 16:41:28.215671 arraylake_client-0.4.1/arraylake_client/config.yaml
--rw-r--r--   0        0        0      192 2023-06-07 18:29:47.978531 arraylake_client-0.4.1/arraylake_client/exceptions.py
--rw-r--r--   0        0        0     1110 2023-06-13 00:03:11.755253 arraylake_client-0.4.1/arraylake_client/log_util.py
--rw-r--r--   0        0        0      282 2023-06-13 00:03:11.755626 arraylake_client-0.4.1/arraylake_client/metastore/__init__.py
--rw-r--r--   0        0        0     8187 2023-06-07 18:29:47.979860 arraylake_client-0.4.1/arraylake_client/metastore/abc.py
--rw-r--r--   0        0        0    12463 2023-06-15 22:59:38.850066 arraylake_client-0.4.1/arraylake_client/metastore/http_metastore.py
--rw-r--r--   0        0        0    50310 2023-06-15 22:59:38.850335 arraylake_client-0.4.1/arraylake_client/repo.py
--rw-r--r--   0        0        0     1227 2023-06-15 22:59:38.850457 arraylake_client-0.4.1/arraylake_client/spec.py
--rw-r--r--   0        0        0     4166 2023-06-07 16:41:28.218150 arraylake_client-0.4.1/arraylake_client/token.py
--rw-r--r--   0        0        0     9753 2023-06-15 22:59:38.850797 arraylake_client-0.4.1/arraylake_client/types.py
--rw-r--r--   0        0        0    10315 2023-06-15 22:59:38.851157 arraylake_client-0.4.1/arraylake_client/virtual.py
--rw-r--r--   0        0        0      851 2023-06-15 22:59:38.851694 arraylake_client-0.4.1/arraylake_client/zarr_util.py
--rw-r--r--   0        0        0     2362 2023-06-15 23:13:13.671835 arraylake_client-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2043 1970-01-01 00:00:00.000000 arraylake_client-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-06-22 20:23:42.538357 arraylake_client-0.4.2/README.md
+-rw-r--r--   0        0        0      357 2023-06-07 16:41:28.210985 arraylake_client-0.4.2/arraylake_client/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-07 16:41:28.212174 arraylake_client-0.4.2/arraylake_client/__main__.py
+-rw-r--r--   0        0        0    15359 2023-06-27 00:27:20.947227 arraylake_client-0.4.2/arraylake_client/api_utils.py
+-rw-r--r--   0        0        0     2381 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/async_utils.py
+-rw-r--r--   0        0        0      630 2023-06-07 16:41:28.212923 arraylake_client-0.4.2/arraylake_client/chunkstore/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-07 16:41:28.213251 arraylake_client-0.4.2/arraylake_client/chunkstore/abc.py
+-rw-r--r--   0        0        0     5201 2023-06-07 16:41:28.213373 arraylake_client-0.4.2/arraylake_client/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:41:28.213456 arraylake_client-0.4.2/arraylake_client/cli/__init__.py
+-rw-r--r--   0        0        0     3822 2023-06-07 16:41:28.213758 arraylake_client-0.4.2/arraylake_client/cli/auth.py
+-rw-r--r--   0        0        0     4762 2023-06-07 16:41:28.213838 arraylake_client-0.4.2/arraylake_client/cli/config.py
+-rw-r--r--   0        0        0     1155 2023-06-07 16:41:28.213908 arraylake_client-0.4.2/arraylake_client/cli/main.py
+-rw-r--r--   0        0        0     3568 2023-06-22 20:23:42.539238 arraylake_client-0.4.2/arraylake_client/cli/repo.py
+-rw-r--r--   0        0        0     3390 2023-06-07 16:41:28.214762 arraylake_client-0.4.2/arraylake_client/cli/utils.py
+-rw-r--r--   0        0        0     7327 2023-07-08 00:39:33.338130 arraylake_client-0.4.2/arraylake_client/client.py
+-rw-r--r--   0        0        0     7098 2023-06-13 00:03:11.755118 arraylake_client-0.4.2/arraylake_client/commits.py
+-rw-r--r--   0        0        0      538 2023-06-07 16:41:28.215453 arraylake_client-0.4.2/arraylake_client/config.py
+-rw-r--r--   0        0        0      105 2023-06-07 16:41:28.215671 arraylake_client-0.4.2/arraylake_client/config.yaml
+-rw-r--r--   0        0        0      192 2023-06-07 18:29:47.978531 arraylake_client-0.4.2/arraylake_client/exceptions.py
+-rw-r--r--   0        0        0     1110 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/log_util.py
+-rw-r--r--   0        0        0      282 2023-06-22 20:23:42.540028 arraylake_client-0.4.2/arraylake_client/metastore/__init__.py
+-rw-r--r--   0        0        0     8188 2023-07-08 00:39:33.338322 arraylake_client-0.4.2/arraylake_client/metastore/abc.py
+-rw-r--r--   0        0        0    12464 2023-07-08 00:39:33.338491 arraylake_client-0.4.2/arraylake_client/metastore/http_metastore.py
+-rw-r--r--   0        0        0    51546 2023-07-08 00:40:14.647940 arraylake_client-0.4.2/arraylake_client/repo.py
+-rw-r--r--   0        0        0     1227 2023-06-22 20:23:42.540945 arraylake_client-0.4.2/arraylake_client/spec.py
+-rw-r--r--   0        0        0     4166 2023-06-07 16:41:28.218150 arraylake_client-0.4.2/arraylake_client/token.py
+-rw-r--r--   0        0        0     9753 2023-06-22 20:23:42.541106 arraylake_client-0.4.2/arraylake_client/types.py
+-rw-r--r--   0        0        0    10315 2023-06-27 00:27:16.448369 arraylake_client-0.4.2/arraylake_client/virtual.py
+-rw-r--r--   0        0        0      851 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/zarr_util.py
+-rw-r--r--   0        0        0     2337 2023-07-08 00:43:08.120935 arraylake_client-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2043 1970-01-01 00:00:00.000000 arraylake_client-0.4.2/PKG-INFO
```

### Comparing `arraylake_client-0.4.1/README.md` & `arraylake_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/api_utils.py` & `arraylake_client-0.4.2/arraylake_client/api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Optional,
     Union,
 )
 
 import httpx
 from dateutil.parser import isoparse
 
+import arraylake_client
 from arraylake_client.log_util import get_logger
 from arraylake_client.token import TokenHandler
 from arraylake_client.types import ApiTokenInfo, OauthTokensResponse, UserInfo
 
 HTTP_TIMEOUT = int(os.environ.get("ARRAYLAKE_CLIENT_HTTP_TIMEOUT", 90))
 
 logger = get_logger(__name__)
@@ -76,25 +77,29 @@
     _client: Optional[httpx.AsyncClient]  # set in __aenter__
     _OPEN: bool
 
     def __init__(self, api_url: str, token: str = None):
         self.api_url = api_url
         self.token = token
 
-        self._default_headers = {"accept": "application/vnd.earthmover+json"}
+        self._default_headers = {
+            "accept": "application/vnd.earthmover+json",
+            # technically we don't enforce this, for now it's for debugging purposes
+            "client-name": "arraylake-python-client",
+            "client-version": arraylake_client.__version__,
+        }
 
         self._client = None
         self._OPEN = False
 
     @retry_on_exception(httpx.RemoteProtocolError, 3)
     async def _request(self, method: str, path: str, **kwargs) -> httpx.Response:
         """Convenience method to make a standard request with retry on RemoteProtocolError"""
         if not self._OPEN:
             raise ValueError("must be in async context to make requests")
-
         return await self._client.request(method, path, **kwargs)
 
     async def __aenter__(self):
         transport = AsyncRetryTransport()
 
         if self.token:
             # if a token is presented, just use that token for all all Authentication headers
```

### Comparing `arraylake_client-0.4.1/arraylake_client/chunkstore/__init__.py` & `arraylake_client-0.4.2/arraylake_client/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/chunkstore/abc.py` & `arraylake_client-0.4.2/arraylake_client/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/chunkstore/s3chunkstore.py` & `arraylake_client-0.4.2/arraylake_client/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/cli/auth.py` & `arraylake_client-0.4.2/arraylake_client/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/cli/config.py` & `arraylake_client-0.4.2/arraylake_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/cli/main.py` & `arraylake_client-0.4.2/arraylake_client/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/cli/repo.py` & `arraylake_client-0.4.2/arraylake_client/cli/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/cli/utils.py` & `arraylake_client-0.4.2/arraylake_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/client.py` & `arraylake_client-0.4.2/arraylake_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ```
 """
 
 import re
 from dataclasses import dataclass, field
 from typing import Optional, Sequence, Tuple
 
-from anyio import start_blocking_portal
-
+from arraylake_client.async_utils import cached_portal
 from arraylake_client.chunkstore import chunkstore
 from arraylake_client.config import config
 from arraylake_client.log_util import get_logger
 from arraylake_client.metastore import HttpMetastore, HttpMetastoreConfig
 from arraylake_client.repo import AsyncRepo, Repo
 from arraylake_client.types import Author
 
@@ -55,15 +54,16 @@
     service_uri: Optional[str] = None
     token: Optional[str] = field(default=None, repr=False)
 
     def __post_init__(self):
         if self.service_uri is None:
             self.service_uri = config.get("service.uri")
 
-    async def list_repos(self, org: str) -> Sequence[str]:
+    # TODO: replace the return type with a stricted type around repo listing object
+    async def list_repos(self, org: str) -> Sequence[dict]:
         """List all repositories for the specified org
 
         Args:
             org: Name of the org
         """
 
         _validate_org(org)
@@ -88,14 +88,27 @@
 
         async with mstore:
             user = await mstore.get_user()
 
         author: Author = user.as_author()
         return AsyncRepo(db, cstore, name, author)
 
+    async def get_or_create_repo(self, name: str) -> AsyncRepo:
+        """Get a repo by name. Create the repo if it doesn't already exist.
+
+        Args:
+            name: Full name of the repo (of the form {ORG}/{REPO})
+        """
+        org, repo_name = _parse_org_and_repo(name)
+        all_repos = [result["name"] for result in await self.list_repos(org)]
+        if repo_name in all_repos:
+            return await self.get_repo(name)
+        else:
+            return await self.create_repo(name)
+
     async def create_repo(self, name: str) -> AsyncRepo:
         """Create a new repo
 
         Args:
             name: Full name of the repo to create (of the form {ORG}/{REPO})
         """
 
@@ -124,24 +137,24 @@
 
         org, repo_name = _parse_org_and_repo(name)
         mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token))
         await mstore.delete_database(repo_name, imsure=imsure, imreallysure=imreallysure)
 
 
 # This version of synchronize is different from the one in repo.py.
-# That version creates a single blocking portal for the lifetime of a Repo object.
-# This version creates a new portal every time an async method is needed.
+# That version stores the global portal on the Repo object itself.
+# This version also uses the global portal but enters and exits the context for each call.
 # This is undoubtedly slower (a new thread is started and stopped on each call.)
 # But it is also simpler, with no need to explicitly .close() the client.
 def _synchronize(func, *args, **kwargs):
     # we have to wrap the method because portal.call doesn't support kwargs
     def wrapped():
         return func(*args, **kwargs)
 
-    with start_blocking_portal() as portal:
+    with cached_portal.acquire() as portal:
         result = portal.call(wrapped)
     return result
 
 
 @dataclass
 class Client:
     """Client for interacting with ArrayLake.
@@ -176,14 +189,23 @@
         Args:
             name: Full name of the repo (of the form {ORG}/{REPO})
         """
 
         arepo = _synchronize(self.aclient.get_repo, name)
         return Repo(arepo)
 
+    def get_or_create_repo(self, name: str) -> Repo:
+        """Get a repo by name. Create the repo if it doesn't already exist.
+
+        Args:
+            name: Full name of the repo (of the form {ORG}/{REPO})
+        """
+        arepo = _synchronize(self.aclient.get_or_create_repo, name)
+        return Repo(arepo)
+
     def create_repo(self, name: str) -> Repo:
         """Create a new repo
 
         Args:
             name: Full name of the repo to create (of the form {ORG}/{REPO})
         """
```

### Comparing `arraylake_client-0.4.1/arraylake_client/commits.py` & `arraylake_client-0.4.2/arraylake_client/commits.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/config.py` & `arraylake_client-0.4.2/arraylake_client/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/log_util.py` & `arraylake_client-0.4.2/arraylake_client/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/metastore/abc.py` & `arraylake_client-0.4.2/arraylake_client/metastore/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class Metastore(ABC):  # pragma: no cover
     @abstractmethod
     async def ping(self) -> dict:
         """Verify that the metastore is accessible and responsive to the client."""
         ...
 
     @abstractmethod
-    async def list_databases(self) -> Sequence[str]:
+    async def list_databases(self) -> Sequence[dict]:
         ...
 
     @abstractmethod
     async def create_database(self, name: str) -> MetastoreDatabase:
         """Create a new metastore database.
 
         Parameters
```

### Comparing `arraylake_client-0.4.1/arraylake_client/metastore/http_metastore.py` & `arraylake_client-0.4.2/arraylake_client/metastore/http_metastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     async def ping(self) -> dict:
         async with self:
             response = await self._request("GET", "user")
         handle_response(response)
 
         return dict(**response.json())
 
-    async def list_databases(self) -> Sequence[str]:
+    async def list_databases(self) -> Sequence[dict]:
         async with self:
             response = await self._request("GET", f"/orgs/{self._config.org}/repos")
         handle_response(response)
         # TODO: use a response model for stricter typing here
         return [repo for repo in response.json()]
 
     async def create_database(self, name: str):
```

### Comparing `arraylake_client-0.4.1/arraylake_client/repo.py` & `arraylake_client-0.4.2/arraylake_client/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,34 +23,40 @@
 import warnings
 from dataclasses import dataclass
 from html import escape
 from typing import (
     AsyncGenerator,
     Awaitable,
     Callable,
+    Generator,
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
 )
 
 import zarr
-from anyio import start_blocking_portal
 from zarr._storage.store import StoreV3
 from zarr.util import normalize_storage_path
 
+from arraylake_client.async_utils import (
+    BlockingPortal,
+    BlockingPortalGenerator,
+    cached_portal,
+)
 from arraylake_client.chunkstore import Chunkstore
 from arraylake_client.commits import CommitData, CommitLog, CommitTree
 from arraylake_client.exceptions import (
     CommitFailedError,
     DocumentNotFoundError,
     InvalidPrefixError,
 )
+from arraylake_client.log_util import get_logger
 from arraylake_client.metastore import MetastoreDatabase
 from arraylake_client.types import (
     Author,
     BranchName,
     CollectionName,
     CommitID,
     NewCommit,
@@ -66,14 +72,16 @@
     ENTRY_POINT_METADATA,
     data_root,
     is_chunk_key,
     is_meta_key,
     meta_root,
 )
 
+logger = get_logger(__name__)
+
 metadata_collection = CollectionName("metadata")
 chunks_collection = CollectionName("chunks")
 
 
 def _write_op(func):
     """
     Decorator for write operations. Ensures that the repo is in a writable state.
@@ -716,21 +724,28 @@
                 yield prefix
             return
         elif path_query == "data":
             yield "root"
             return
 
         start = len(path_query) + 1
+        groups_seen = set()
         async for path in self._list(path_query, all_subdirs=False):
+            # a group may end with .group.json (explicit) or have no
+            # suffix (implicit). in the group
+            # (in progress) should this logic be tweaked to find items without a suffix too (i.e a dir?)
             if path.endswith(".group.json"):
-                # the presence of a group.json indicates that there is a subdirectory
-                # NOTE: it is ambiguous whether we should append a trailing slash
-                # The spec suggests yes, but zarr-python doesn't seem to like this
-                yield path[start:-11]  # + "/"
-            yield path[start:]
+                p = path[start:-11]
+                if p not in groups_seen:
+                    yield path[start:]
+                    groups_seen.add(p)
+            else:
+                # trim the start of the path off, we only want what's in the dir
+                # e.g. meta/root/baz.array.json -> baz.array.json
+                yield path[start:]
 
     async def _list_prefix(self, prefix: str) -> AsyncGenerator[str, None]:
         """List a prefix in the metastore
 
         Parameters
         ----------
         prefix : str
@@ -859,24 +874,33 @@
     return meta_keys, chunk_keys
 
 
 class Repo:
     """Synchronous interface to Arraylake repo."""
 
     _arepo: AsyncRepo
+    _OPEN: bool
+    _cached_portal_context: Optional[BlockingPortalGenerator]
+    _portal: Optional[BlockingPortal]
+    _arepo_context: Optional[Generator]
 
     def __init__(self, arepo: AsyncRepo):
         """
         Initialize a Repo from an initialized AsyncRepo
 
         Args:
             arepo: An existing AsyncRepo
         """
         self._arepo = arepo
+
+        # default / unset attributes used to wrap AsyncRepo
         self._OPEN = False
+        self._cached_portal_context = None
+        self._portal = None
+        self._arepo_context = None
 
     @classmethod
     def from_metastore_and_chunkstore(cls, metastore_db: MetastoreDatabase, chunkstore: Chunkstore, name: str, author: Author) -> Repo:
         """
         Initialize a Repo from an initialized metastore database and chunkstore
 
         Args:
@@ -889,29 +913,31 @@
         return cls(arepo)
 
     @property
     def repo_name(self) -> str:
         return self._arepo.repo_name
 
     def _open(self):
-        self._blocking_portal = start_blocking_portal()
-        self._portal = self._blocking_portal.__enter__()
+        """using a AnyIO blocking portal, enter the AsyncRepo's async context"""
+
+        # Acquire the blocking portal .acquire() returns a context manager that when entered, provisions a BlockingPortal.
+        # and when exited, deprovisions the BlockingPortal (provided there are no other active references, e.g. from
+        # other repo objects).
+        self._cached_portal_context = cached_portal.acquire()
+        self._portal = self._cached_portal_context.__enter__()
+        # wrap_async_context_manager wraps the AsyncRepo object and .__enter__() enters the async context (synchronously)
         self._arepo_context = self._portal.wrap_async_context_manager(self._arepo)
         self._arepo_context.__enter__()
-        self._portal._check_running()
+
+        # _OPEN signals that the portal and async context are ready for use
         self._OPEN = True
 
     def _synchronize(self, method, *args, **kwargs):
         if not self._OPEN:
             self._open()
-        try:
-            # TODO: understand why this is necessary
-            self._portal._check_running()
-        except RuntimeError:
-            self._open()
 
         # we have to wrap the method because portal.call doesn't support kwargs
         def wrapped_method():
             return method(*args, **kwargs)
 
         @functools.wraps(method)
         def wrap(*args, **kwargs):
@@ -921,31 +947,34 @@
 
     def _wrap_async_iter(self, func, *args, **kwargs):
         async def iter_to_list():
             # TODO: replace with generators so we don't load massive lists into memory
             # (e.g. list_prefix(""))
             return [item async for item in func(*args, **kwargs)]
 
-        return self._portal.call(iter_to_list)
+        return self._synchronize(iter_to_list)
 
     def __getstate__(self):
         return self._arepo
 
     def __setstate__(self, state):
         self._arepo = state
         self._open()
 
     def close(self):
         if self._OPEN:
             try:
                 self._arepo_context.__exit__(None, None, None)
-                self._blocking_portal.__exit__(None, None, None)
             except RuntimeError:
-                # the portal is not running
                 pass
+            self._arepo_context = None
+            self._portal = None
+            self._cached_portal_context.__exit__(None, None, None)
+            self._cached_portal_context = None
+            self._OPEN = False
 
     def __del__(self):
         self.close()
 
     def __repr__(self):
         repo_name = self._arepo.repo_name
         return f"<arraylake_client.repo.Repo '{repo_name}'>"
```

### Comparing `arraylake_client-0.4.1/arraylake_client/spec.py` & `arraylake_client-0.4.2/arraylake_client/spec.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/token.py` & `arraylake_client-0.4.2/arraylake_client/token.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/types.py` & `arraylake_client-0.4.2/arraylake_client/types.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/virtual.py` & `arraylake_client-0.4.2/arraylake_client/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/arraylake_client/zarr_util.py` & `arraylake_client-0.4.2/arraylake_client/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.1/pyproject.toml` & `arraylake_client-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake-client"
-version = "0.4.1"  # placeholder
+version = "0.4.2"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake_client"}]
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -37,15 +37,14 @@
 cachetools = "^5.3.0"
 structlog = "^23.1.0"
 ipytree = { version = ">=0.2.2,<1.0", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
-pytest-asyncio = "^0.19"
 pytest-cov = "^4.0.0"
 pytest-click = "^1.1.0"
 pooch = "^1.6.0"
 netCDF4 = "^1.6.1"
 xarray = ">=2022.12.0"
 pandas = "^1.3"
 dask = "^2022.10.2"
```

### Comparing `arraylake_client-0.4.1/PKG-INFO` & `arraylake_client-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylake-client
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.1 Summary: Python
+Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.2 Summary: Python
 client for ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cli Provides-Extra: virtual Provides-Extra: widgets Requires-
 Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: anyio (>=3.6.1,<4.0.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0) Requires-Dist: donfig (>=0.7,<1.0)
```

