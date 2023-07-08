# Comparing `tmp/langsmith-0.0.1.tar.gz` & `tmp/langsmith-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.1.tar", max compression
+gzip compressed data, was "langsmith-0.0.2.tar", max compression
```

## Comparing `langsmith-0.0.1.tar` & `langsmith-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     8006 2023-06-26 21:49:14.459291 langsmith-0.0.1/README.md
--rw-r--r--   0        0        0      479 2023-06-26 21:47:00.744671 langsmith-0.0.1/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 22:33:42.162840 langsmith-0.0.1/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-06 22:33:42.162946 langsmith-0.0.1/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-06 22:33:42.163009 langsmith-0.0.1/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1061 2023-06-14 13:47:41.867397 langsmith-0.0.1/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14097 2023-06-26 21:46:06.630189 langsmith-0.0.1/langsmith/cli/main.py
--rw-r--r--   0        0        0    27732 2023-06-26 21:47:00.748635 langsmith-0.0.1/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-06-26 21:42:08.517344 langsmith-0.0.1/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-06-26 21:42:08.531755 langsmith-0.0.1/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-06-26 21:42:08.531868 langsmith-0.0.1/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-06-26 21:42:08.517144 langsmith-0.0.1/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6120 2023-06-26 21:49:42.954134 langsmith-0.0.1/langsmith/run_trees.py
--rw-r--r--   0        0        0     6575 2023-06-23 09:42:59.404625 langsmith-0.0.1/langsmith/schemas.py
--rw-r--r--   0        0        0     3688 2023-06-26 21:48:34.873509 langsmith-0.0.1/langsmith/utils.py
--rw-r--r--   0        0        0      878 2023-06-26 22:59:57.421302 langsmith-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8006 2023-07-05 17:54:45.352295 langsmith-0.0.2/README.md
+-rw-r--r--   0        0        0      479 2023-07-05 17:54:45.352708 langsmith-0.0.2/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.2/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.2/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.2/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1198 2023-07-05 17:54:45.353810 langsmith-0.0.2/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14054 2023-07-05 17:54:45.354144 langsmith-0.0.2/langsmith/cli/main.py
+-rw-r--r--   0        0        0    27679 2023-07-05 17:54:45.354525 langsmith-0.0.2/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.2/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.2/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.2/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.2/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6120 2023-07-05 17:54:45.356170 langsmith-0.0.2/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6452 2023-07-05 18:01:48.582191 langsmith-0.0.2/langsmith/schemas.py
+-rw-r--r--   0        0        0     3688 2023-07-05 17:54:45.356784 langsmith-0.0.2/langsmith/utils.py
+-rw-r--r--   0        0        0      878 2023-07-05 18:01:48.582953 langsmith-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.2/PKG-INFO
```

### Comparing `langsmith-0.0.1/README.md` & `langsmith-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.2/langsmith/cli/docker-compose.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 version: '3'
 services:
+  langchain-playground:
+    image: langchain/${_LANGCHAINPLUS_IMAGE_PREFIX-}langchainplus-playground:latest
   langchain-frontend:
     image: langchain/${_LANGCHAINPLUS_IMAGE_PREFIX-}langchainplus-frontend:latest
     ports:
       - 80:80
     environment:
       - REACT_APP_BACKEND_URL=http://localhost:1984
     depends_on:
       - langchain-backend
+      - langchain-playground
     volumes:
       - ./conf/nginx.conf:/etc/nginx/default.conf:ro
   langchain-backend:
     image: langchain/${_LANGCHAINPLUS_IMAGE_PREFIX-}langchainplus-backend:latest
     environment:
       - PORT=1984
       - LANGCHAIN_ENV=local_docker
```

### Comparing `langsmith-0.0.1/langsmith/cli/main.py` & `langsmith-0.0.2/langsmith/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,14 @@
             "-f",
             str(self.docker_compose_file),
         ]
         subprocess.run(
             [
                 *command,
                 "up",
-                "--pull=always",
                 "--quiet-pull",
                 "--wait",
             ]
         )
         logger.info(
             "langchain plus server is running at http://localhost:1984.  To connect"
             " locally, set the following environment variable"
@@ -205,15 +204,14 @@
                 "-f",
                 str(self.ngrok_path),
             ]
             subprocess.run(
                 [
                     *command,
                     "up",
-                    "--pull=always",
                     "--quiet-pull",
                     "--wait",
                 ]
             )
         logger.info(
             "ngrok is running. You can view the dashboard at http://0.0.0.0:4040"
         )
@@ -269,14 +267,15 @@
                 OPENAI_API_KEY environment variable. If neither are provided,
                 some features of LangSmith will not be available.
         """
         if dev:
             os.environ["_LANGCHAINPLUS_IMAGE_PREFIX"] = "rc-"
         if openai_api_key is not None:
             os.environ["OPENAI_API_KEY"] = openai_api_key
+        self.pull(dev=dev)
         if expose:
             self._start_and_expose(auth_token=auth_token)
         else:
             self._start_local()
 
     def stop(self) -> None:
         """Stop the LangSmith server."""
```

### Comparing `langsmith-0.0.1/langsmith/client.py` & `langsmith-0.0.2/langsmith/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     FeedbackCreate,
     FeedbackSourceBase,
     FeedbackSourceType,
     ModelFeedbackSource,
     Run,
     RunBase,
     RunTypeEnum,
-    RunUpdate,
     TracerSession,
     TracerSessionResult,
 )
 from langsmith.utils import (
     LangChainPlusAPIError,
     LangChainPlusError,
     LangChainPlusUserError,
@@ -290,23 +289,20 @@
 
     def update_run(
         self,
         run_id: ID_TYPE,
         **kwargs: Any,
     ) -> None:
         """Update a run to the LangChain+ API."""
-        run_update = RunUpdate(
-            **kwargs,
-        )
         headers = {**self._headers, "Accept": "application/json"}
         request_with_retries(
             "patch",
             f"{self.api_url}/runs/{run_id}",
             request_kwargs={
-                "data": run_update.json(),
+                "data": json.dumps(kwargs, default=_serialize_json),
                 "headers": headers,
                 "timeout": self.timeout_ms / 1000,
             },
             retry_config=self.retry_config,
         )
 
     def _load_child_runs(self, run: Run) -> Run:
```

### Comparing `langsmith-0.0.1/langsmith/evaluation/evaluator.py` & `langsmith-0.0.2/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.2/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/langsmith/run_helpers.py` & `langsmith-0.0.2/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/langsmith/run_trees.py` & `langsmith-0.0.2/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/langsmith/schemas.py` & `langsmith-0.0.2/langsmith/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,23 +78,25 @@
 
 class RunTypeEnum(str, Enum):
     """Enum for run types."""
 
     tool = "tool"
     chain = "chain"
     llm = "llm"
+    retriever = "retriever"
+    embedding = "embedding"
 
 
 class RunBase(BaseModel):
     """Base Run schema."""
 
     id: UUID
     name: str
     start_time: datetime
-    run_type: RunTypeEnum
+    run_type: Union[RunTypeEnum, str]
     end_time: Optional[datetime] = None
     extra: Optional[dict] = None
     error: Optional[str] = None
     serialized: Optional[dict]
     events: Optional[List[Dict]] = None
     inputs: dict
     outputs: Optional[dict] = None
@@ -109,22 +111,14 @@
     execution_order: int
     session_id: Optional[UUID] = None
     child_run_ids: Optional[List[UUID]] = None
     child_runs: Optional[List[Run]] = None
     feedback_stats: Optional[Dict[str, Any]] = None
 
 
-class RunUpdate(BaseModel):
-    end_time: Optional[datetime]
-    error: Optional[str]
-    outputs: Optional[dict]
-    parent_run_id: Optional[UUID]
-    reference_example_id: Optional[UUID]
-
-
 class FeedbackSourceBase(BaseModel):
     type: str
     metadata: Optional[Dict[str, Any]] = None
 
     class Config:
         frozen = True
```

### Comparing `langsmith-0.0.1/langsmith/utils.py` & `langsmith-0.0.2/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.1/pyproject.toml` & `langsmith-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.1"
+version = "0.0.2"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.1/PKG-INFO` & `langsmith-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

