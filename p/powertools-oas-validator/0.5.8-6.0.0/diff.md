# Comparing `tmp/powertools_oas_validator-0.5.8.tar.gz` & `tmp/powertools_oas_validator-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.8.tar", max compression
+gzip compressed data, was "powertools_oas_validator-6.0.0.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.8.tar` & `powertools_oas_validator-6.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/LICENSE
--rw-r--r--   0        0        0     2666 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/README.md
--rw-r--r--   0        0        0       13 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      252 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4933 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     1884 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1909 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.8/setup.py
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/LICENSE
+-rw-r--r--   0        0        0     2790 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/README.md
+-rw-r--r--   0        0        0       13 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1326 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4243 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     1884 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1843 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-08 11:49:19.464485 powertools_oas_validator-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 powertools_oas_validator-6.0.0/setup.py
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 powertools_oas_validator-6.0.0/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.8/LICENSE` & `powertools_oas_validator-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/README.md` & `powertools_oas_validator-6.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,19 @@
 Example of a `SchemaValidatonError`:
 ```python
 from aws_lambda_powertools.utilities.validation import SchemaValidationError
 
 SchemaValidatonError(
   name="test-path.test-endpoint.requestBody[param_1]",
   path=["test-path", "test-endpoint", "requestBody", "param_1"],
-  validation_message="'not an integer' is not of type 'integer'"
+  validation_message="'not an integer' is not of type 'integer'.",
+  message="'not an integer' is not of type 'integer'",
+  rule="int",
+  rule_definition="type",
+  value="'not an integer'"
 )
 ```
 
 ## Know Issues
 While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
 (same as the Powertools validator would), with as much of the optional attributes as possible.
```

#### html2text {}

```diff
@@ -21,14 +21,15 @@
 app.resolve(event, context) return response ``` ## Error Handling If the
 validation fails, the decorator throws a `SchemaValidatonError` with relevant
 information about the failed validation. Example of a `SchemaValidatonError`:
 ```python from aws_lambda_powertools.utilities.validation import
 SchemaValidationError SchemaValidatonError( name="test-path.test-
 endpoint.requestBody[param_1]", path=["test-path", "test-endpoint",
 "requestBody", "param_1"], validation_message="'not an integer' is not of type
-'integer'" ) ``` ## Know Issues While all validation errors are caught, there
-is only limited information about the various errors. The decorator will try
-its best to throw a `SchemaValidatonError` (same as the Powertools validator
-would), with as much of the optional attributes as possible. In summary, it is
-possible that not all `SchemaValidationErrors`'s will have the correct name and
-path attributes. ## Contributions Please make a pull request and I will review
-it ASAP.
+'integer'.", message="'not an integer' is not of type 'integer'", rule="int",
+rule_definition="type", value="'not an integer'" ) ``` ## Know Issues While all
+validation errors are caught, there is only limited information about the
+various errors. The decorator will try its best to throw a
+`SchemaValidatonError` (same as the Powertools validator would), with as much
+of the optional attributes as possible. In summary, it is possible that not all
+`SchemaValidationErrors`'s will have the correct name and path attributes. ##
+Contributions Please make a pull request and I will review it ASAP.
```

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/middleware.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/overrides/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,13 +14,21 @@
     @CustomValidationErrorWrapper(OpenAPIError)
     def _get_body(self, body: Optional[str], mimetype: str, operation: Spec) -> Any:
         return super()._get_body.__wrapped__(  # type: ignore
             self, body=body, mimetype=mimetype, operation=operation
         )
 
     @CustomValidationErrorWrapper(OpenAPIError)
+    def _get_parameter(
+        self, parameters: RequestParameters, param: Spec
+    ) -> Optional[Dict[str, str]]:
+        return super()._get_parameter.__wrapped__(  # type: ignore
+            self, parameters=parameters, param=param
+        )
+
+    @CustomValidationErrorWrapper(OpenAPIError)
     def _get_security(
         self, parameters: RequestParameters, operation: Spec
     ) -> Optional[Dict[str, str]]:
         return super()._get_security.__wrapped__(  # type: ignore
             self, parameters=parameters, operation=operation
         )
```

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/services/error_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,114 @@
-import re
-from typing import List
+from typing import Union
 
 from aws_lambda_powertools.utilities.validation.exceptions import SchemaValidationError
+from openapi_core.casting.schemas.exceptions import CastError
 from openapi_core.templating.security.exceptions import SecurityNotFound
-from openapi_core.validation.request.exceptions import ParameterValidationError
+from openapi_core.validation.request.exceptions import (
+    MissingRequiredRequestBody,
+    ParameterValidationError,
+)
 from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
 
 from powertools_oas_validator.exceptions import UnhandledValidationError
-from powertools_oas_validator.types import ParamError, Request
+from powertools_oas_validator.types import Request
 
 
 class ErrorHandler:
     @staticmethod
     def raise_schema_validation_error(
         ex: Exception,
         request: Request,
     ) -> None:
         ex_type = type(ex)
 
-        if issubclass(ex_type, ParameterValidationError):
-            error = ErrorHandler._handle_parameter_error(ex, request)  # type: ignore
-        elif ex_type == InvalidSchemaValue:
+        if issubclass(ex_type, ParameterValidationError) or ex_type == CastError:
+            error = ErrorHandler._handle_parameter_error(ex)  # type: ignore
+        elif ex_type == InvalidSchemaValue or ex_type == MissingRequiredRequestBody:
             error = ErrorHandler._handle_body_error(ex, request)  # type: ignore
         elif ex_type == SecurityNotFound:
-            error = ErrorHandler._handle_security_error(ex, request)  # type: ignore
+            error = ErrorHandler._handle_security_error(ex)  # type: ignore
         else:
             raise UnhandledValidationError(
                 f"'{ex_type}' is unhandled. Please open an issue on:"
                 + "https://github.com/RasmusFangel/powertools-oas-validator/issues"
                 + " and it will be resolved ASAP!"
             )
         raise error
 
     @staticmethod
-    def _handle_security_error(
-        ex: SecurityNotFound, request: Request
-    ) -> SchemaValidationError:
+    def _handle_security_error(ex: SecurityNotFound) -> SchemaValidationError:
         violating_schemes = ex.schemes[0]
-        name = ErrorHandler._get_name(request, "security", violating_schemes[0])
-
-        validation_message = f"'{ex.schemes}' are required security scheme(s)."
+        name = f"security[{violating_schemes[0]}]"
+        path = name.replace("]", "").split("[")
+        validation_message = f"'{violating_schemes}' are required security scheme(s)"
 
         return SchemaValidationError(
-            message=None,
-            validation_message=validation_message,
+            message=validation_message,
+            validation_message=validation_message + ".",
             name=name,
-            path=ErrorHandler._get_path(name),
+            path=path,
             value=None,
             definition=None,
             rule=None,
             rule_definition=None,
         )
 
     @staticmethod
     def _handle_parameter_error(
-        ex: ParameterValidationError, request: Request
+        ex: Union[ParameterValidationError, CastError],
     ) -> SchemaValidationError:
-        name = ErrorHandler._get_name(request, "parameters", ex.name)
+        if type(ex) == CastError:
+            validation_message = f"Parameter '{ex.value}' is not of type: '{ex.type}'"
+            return SchemaValidationError(
+                message=validation_message, validation_message=validation_message + "."
+            )
+        name = f"parameters[{ex.name}]"  # type: ignore
 
-        validation_message = f"'{ex.name}' is a required {ex.location} parameter."
+        validation_message = (
+            f"'{ex.name}' is a required '{ex.location}' parameter"  # type: ignore
+        )
 
         return SchemaValidationError(
-            message=None,
-            validation_message=validation_message,
+            message=validation_message,
+            validation_message=validation_message + ".",
             name=name,
-            path=ErrorHandler._get_path(name),
+            path=name.replace("[", "").replace("]", "").split("."),
             value=None,
             definition=None,
-            rule=None,
+            rule=ex.location,  # type: ignore
             rule_definition=None,
         )
 
     @staticmethod
     def _handle_body_error(
-        ex: InvalidSchemaValue, request: Request
+        ex: Union[InvalidSchemaValue, MissingRequiredRequestBody], request: Request
     ) -> SchemaValidationError:
-        violating_req_params = []
-
-        for error in ex.schema_errors:
-            err_msg = str(error.message)  # type: ignore
-
-            violating_param = ErrorHandler._get_violating_param(err_msg)
-            if "required" in err_msg:
-                param = violating_param
-            else:
-                kv_swap = {v: k for k, v in ex.value.items()}  # type: ignore
-                param = kv_swap[violating_param]
-
-            violating_req_params.append(
-                (
-                    ParamError(
-                        param=param,
-                        validation_message=err_msg,
-                        value=violating_param,
-                    )
-                )
+        if type(ex) == MissingRequiredRequestBody:
+            return SchemaValidationError(
+                message="Missing required 'requestBody'",
+                validation_message="Missing required 'requestBody'.",
             )
+        error = None
         try:
-            name = ErrorHandler._get_name(
-                request, "requestBody", violating_req_params[0].param
-            )
-            path = ErrorHandler._get_path(name)
+            error = ex.schema_errors[0]  # type: ignore
+        except IndexError:
+            raise ValueError("Error has no Schema Error! Can't process errors")
 
-        except KeyError:
-            name = ErrorHandler._get_name(request, "request_body", "")
-            path = ErrorHandler._get_path("")
-
-        validation_message = ""
-
-        if violating_req_params:
-            try:
-                validation_message = violating_req_params[0].validation_message
-            except KeyError:
-                ...
+        try:
+            prop = error.absolute_path[0]
+        except IndexError:
+            prop = ""
+
+        name = f"requestBody.content.{request.mimetype}.schema.properties[{prop}]"
+        path = name.replace("[", ".").replace("]", "").split(".")
 
         return SchemaValidationError(
-            message=None,
-            validation_message=validation_message,
+            message=error.message,
+            validation_message=error.message + ".",
             name=name,
             path=path,
-            value=None,
+            value=error.instance,
             definition=None,
-            rule=None,
-            rule_definition=None,
+            rule=error.validator_value,
+            rule_definition=error.validator,
         )
-
-    @staticmethod
-    def _get_name(request: Request, path: str, violating_param: str) -> str:
-        return (
-            request.path.replace("/", ".").lstrip(".") + f".{path}[{violating_param}]"
-        )
-
-    @staticmethod
-    def _get_path(name: str) -> List[str]:
-        return name.replace("[", ".").replace("]", "").split(".")
-
-    @staticmethod
-    def _get_violating_param(p: str) -> str:
-        try:
-            return re.search("'(.+?)'", p).group(1)  # type: ignore
-        except IndexError:
-            return ""
-
-
-error_to_func = {
-    ParameterValidationError: ErrorHandler._handle_parameter_error,
-    InvalidSchemaValue: ErrorHandler._handle_body_error,
-}
```

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.8/powertools_oas_validator/types.py` & `powertools_oas_validator-6.0.0/powertools_oas_validator/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from dataclasses import dataclass
 
 from openapi_core.datatypes import RequestParameters
 from openapi_core.protocols import Request as CoreRequest
 
 
 @dataclass
-class OpenAPIVersion:
+class OpenAPIVersion:  # pragma: nocover
     major: int
     minor: int
     pico: int
 
     def __str__(self) -> str:
         return f"{self.major}.{self.minor}.{self.pico}"
 
 
-@dataclass
-class ParamError:
-    param: str = ""
-    validation_message: str = ""
-    value: str = ""
-
-
-class Request(CoreRequest):
+class Request(CoreRequest):  # pragma: nocover
     def __init__(
         self,
         host_url: str,
         path: str,
         full_url_pattern: str,
         method: str,
         parameters: RequestParameters,
```

### Comparing `powertools_oas_validator-0.5.8/pyproject.toml` & `powertools_oas_validator-6.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.8"
+version = "6.0.0"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.5.8/setup.py` & `powertools_oas_validator-6.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.5.8',
+    'version': '6.0.0',
     'description': '',
-    'long_description': '# powertools-oas-validator\n<br><a href="https://badge.fury.io/py/powertools-oas-validator"><img src="https://badge.fury.io/py/powertools-oas-validator.svg" alt="PyPI version"></a>  ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg) <img src="https://coveralls.io/repos/RasmusFangel/powertools-oas-validator/badge.svg?branch=main" alt="Coveralls"></a>\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\nExample of a `SchemaValidatonError`:\n```python\nfrom aws_lambda_powertools.utilities.validation import SchemaValidationError\n\nSchemaValidatonError(\n  name="test-path.test-endpoint.requestBody[param_1]",\n  path=["test-path", "test-endpoint", "requestBody", "param_1"],\n  validation_message="\'not an integer\' is not of type \'integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have the correct name and path attributes.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
+    'long_description': '# powertools-oas-validator\n<br><a href="https://badge.fury.io/py/powertools-oas-validator"><img src="https://badge.fury.io/py/powertools-oas-validator.svg" alt="PyPI version"></a>  ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg) <img src="https://coveralls.io/repos/RasmusFangel/powertools-oas-validator/badge.svg?branch=main" alt="Coveralls"></a>\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\nExample of a `SchemaValidatonError`:\n```python\nfrom aws_lambda_powertools.utilities.validation import SchemaValidationError\n\nSchemaValidatonError(\n  name="test-path.test-endpoint.requestBody[param_1]",\n  path=["test-path", "test-endpoint", "requestBody", "param_1"],\n  validation_message="\'not an integer\' is not of type \'integer\'.",\n  message="\'not an integer\' is not of type \'integer\'",\n  rule="int",\n  rule_definition="type",\n  value="\'not an integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have the correct name and path attributes.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RasmusFangel/powertools-oas-validator',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['powertools_oas_validator', 'powertools_oas_validator.overrides',
 'powertools_oas_validator.services'] package_data = \ {'': ['*']}
 install_requires = \ ['aws-lambda-powertools>=2.18.0,<3.0.0',
 'fastjsonschema>=2.17.1,<3.0.0', 'jmespath>=1.0.1,<2.0.0', 'openapi-
 core>=0.17.2,<0.18.0'] setup_kwargs = { 'name': 'powertools-oas-validator',
-'version': '0.5.8', 'description': '', 'long_description': '# powertools-oas-
+'version': '6.0.0', 'description': '', 'long_description': '# powertools-oas-
 validator\n
 [PyPI_version] ![CI](https://github.com/RasmusFangel/powertools-oas-validator/
 workflows/CI/badge.svg) [Coveralls]
 \n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/
 aws-powertools/powertools-lambda-python) is an awesome set of tools for
 supercharging your lambdas. Powertools supports validating incoming requests
 (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is
@@ -30,19 +30,21 @@
 response\n```\n\n## Error Handling\nIf the validation fails, the decorator
 throws a `SchemaValidatonError` with relevant information about the failed
 validation.\n\n\nExample of a `SchemaValidatonError`:\n```python\nfrom
 aws_lambda_powertools.utilities.validation import
 SchemaValidationError\n\nSchemaValidatonError(\n name="test-path.test-
 endpoint.requestBody[param_1]",\n path=["test-path", "test-endpoint",
 "requestBody", "param_1"],\n validation_message="\'not an integer\' is not of
-type \'integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are
-caught, there is only limited information about the various errors. The
-decorator will try its best to throw a `SchemaValidatonError`\n(same as the
-Powertools validator would), with as much of the optional attributes as
-possible.\n\nIn summary, it is possible that not all
-`SchemaValidationErrors`\'s will have the correct name and path
-attributes.\n\n\n## Contributions\nPlease make a pull request and I will review
-it ASAP.\n', 'author': 'Rasmus Hansen', 'author_email':
-'R.FangelHansen@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/RasmusFangel/powertools-oas-validator', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+type \'integer\'.",\n message="\'not an integer\' is not of type
+\'integer\'",\n rule="int",\n rule_definition="type",\n value="\'not an
+integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are caught,
+there is only limited information about the various errors. The decorator will
+try its best to throw a `SchemaValidatonError`\n(same as the Powertools
+validator would), with as much of the optional attributes as possible.\n\nIn
+summary, it is possible that not all `SchemaValidationErrors`\'s will have the
+correct name and path attributes.\n\n\n## Contributions\nPlease make a pull
+request and I will review it ASAP.\n', 'author': 'Rasmus Hansen',
+'author_email': 'R.FangelHansen@gmail.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/RasmusFangel/powertools-
+oas-validator', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `powertools_oas_validator-0.5.8/PKG-INFO` & `powertools_oas_validator-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.5.8
+Version: 6.0.0
 Summary: 
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,19 @@
 Example of a `SchemaValidatonError`:
 ```python
 from aws_lambda_powertools.utilities.validation import SchemaValidationError
 
 SchemaValidatonError(
   name="test-path.test-endpoint.requestBody[param_1]",
   path=["test-path", "test-endpoint", "requestBody", "param_1"],
-  validation_message="'not an integer' is not of type 'integer'"
+  validation_message="'not an integer' is not of type 'integer'.",
+  message="'not an integer' is not of type 'integer'",
+  rule="int",
+  rule_definition="type",
+  value="'not an integer'"
 )
 ```
 
 ## Know Issues
 While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
 (same as the Powertools validator would), with as much of the optional attributes as possible.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.5.8 Summary:
+Metadata-Version: 2.1 Name: powertools-oas-validator Version: 6.0.0 Summary:
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator License:
 MIT Author: Rasmus Hansen Author-email: R.FangelHansen@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0) Requires-Dist:
 fastjsonschema (>=2.17.1,<3.0.0) Requires-Dist: jmespath (>=1.0.1,<2.0.0)
@@ -32,14 +32,15 @@
 app.resolve(event, context) return response ``` ## Error Handling If the
 validation fails, the decorator throws a `SchemaValidatonError` with relevant
 information about the failed validation. Example of a `SchemaValidatonError`:
 ```python from aws_lambda_powertools.utilities.validation import
 SchemaValidationError SchemaValidatonError( name="test-path.test-
 endpoint.requestBody[param_1]", path=["test-path", "test-endpoint",
 "requestBody", "param_1"], validation_message="'not an integer' is not of type
-'integer'" ) ``` ## Know Issues While all validation errors are caught, there
-is only limited information about the various errors. The decorator will try
-its best to throw a `SchemaValidatonError` (same as the Powertools validator
-would), with as much of the optional attributes as possible. In summary, it is
-possible that not all `SchemaValidationErrors`'s will have the correct name and
-path attributes. ## Contributions Please make a pull request and I will review
-it ASAP.
+'integer'.", message="'not an integer' is not of type 'integer'", rule="int",
+rule_definition="type", value="'not an integer'" ) ``` ## Know Issues While all
+validation errors are caught, there is only limited information about the
+various errors. The decorator will try its best to throw a
+`SchemaValidatonError` (same as the Powertools validator would), with as much
+of the optional attributes as possible. In summary, it is possible that not all
+`SchemaValidationErrors`'s will have the correct name and path attributes. ##
+Contributions Please make a pull request and I will review it ASAP.
```

