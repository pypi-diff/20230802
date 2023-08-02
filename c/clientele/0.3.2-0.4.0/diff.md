# Comparing `tmp/clientele-0.3.2.tar.gz` & `tmp/clientele-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.3.2.tar", max compression
+gzip compressed data, was "clientele-0.4.0.tar", max compression
```

## Comparing `clientele-0.3.2.tar` & `clientele-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.3.2/LICENSE
--rw-r--r--   0        0        0     1742 2023-07-30 22:05:13.221961 clientele-0.3.2/README.md
--rw-r--r--   0        0        0      898 2023-07-30 21:43:47.060546 clientele-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.2/src/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-25 03:26:44.875798 clientele-0.3.2/src/cli.py
--rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.2/src/constants_template.py
--rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.2/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.2/src/generators/__init__.py
--rw-r--r--   0        0        0     7681 2023-07-30 22:01:28.730710 clientele-0.3.2/src/generators/clients.py
--rw-r--r--   0        0        0     2997 2023-07-25 21:56:31.511282 clientele-0.3.2/src/generators/http.py
--rw-r--r--   0        0        0     3815 2023-07-30 22:01:28.702712 clientele-0.3.2/src/generators/schemas.py
--rw-r--r--   0        0        0      190 2023-07-30 21:43:40.188450 clientele-0.3.2/src/settings.py
--rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.2/src/template/MANIFEST
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.2/src/template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.2/src/template/client.py
--rw-r--r--   0        0        0      974 2023-07-25 22:23:05.603189 clientele-0.3.2/src/template/http.py
--rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.2/src/template/schemas.py
--rw-r--r--   0        0        0     2202 2023-07-30 21:39:17.797808 clientele-0.3.2/src/utils.py
--rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.2/src/writer.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 clientele-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1718 2023-08-02 04:28:12.938554 clientele-0.4.0/README.md
+-rw-r--r--   0        0        0      905 2023-08-01 23:12:34.358150 clientele-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.4.0/src/__init__.py
+-rw-r--r--   0        0        0     2924 2023-08-01 23:27:45.401764 clientele-0.4.0/src/cli.py
+-rw-r--r--   0        0        0       50 2023-07-31 02:40:13.111663 clientele-0.4.0/src/client_template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.4.0/src/client_template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.4.0/src/client_template/client.py
+-rw-r--r--   0        0        0      993 2023-08-02 03:52:10.187256 clientele-0.4.0/src/client_template/http.py
+-rw-r--r--   0        0        0       76 2023-08-02 03:43:33.184239 clientele-0.4.0/src/client_template/schemas.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.4.0/src/constants_template.py
+-rw-r--r--   0        0        0     2069 2023-08-01 23:23:41.098914 clientele-0.4.0/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.4.0/src/generators/__init__.py
+-rw-r--r--   0        0        0     8929 2023-08-02 04:19:58.737007 clientele-0.4.0/src/generators/clients.py
+-rw-r--r--   0        0        0     2832 2023-08-02 02:28:17.182281 clientele-0.4.0/src/generators/http.py
+-rw-r--r--   0        0        0     5850 2023-08-02 04:19:58.733008 clientele-0.4.0/src/generators/schemas.py
+-rw-r--r--   0        0        0      391 2023-08-01 23:23:41.098914 clientele-0.4.0/src/settings.py
+-rw-r--r--   0        0        0      464 2023-08-02 04:21:15.956387 clientele-0.4.0/src/templates/async_methods.jinja
+-rw-r--r--   0        0        0       75 2023-08-01 23:33:19.745482 clientele-0.4.0/src/templates/basic_client.jinja2
+-rw-r--r--   0        0        0      134 2023-08-01 23:34:59.694567 clientele-0.4.0/src/templates/bearer_client.jinja2
+-rw-r--r--   0        0        0       34 2023-08-01 23:32:13.768760 clientele-0.4.0/src/templates/client.jinja2
+-rw-r--r--   0        0        0      562 2023-08-02 04:26:47.439084 clientele-0.4.0/src/templates/get_method.jinja2
+-rw-r--r--   0        0        0      607 2023-08-02 04:27:04.858109 clientele-0.4.0/src/templates/post_method.jinja2
+-rw-r--r--   0        0        0      115 2023-08-02 04:06:42.400353 clientele-0.4.0/src/templates/schema_class.jinja2
+-rw-r--r--   0        0        0      428 2023-08-02 04:21:04.265390 clientele-0.4.0/src/templates/sync_methods.jinja2
+-rw-r--r--   0        0        0     2829 2023-08-02 04:19:58.733008 clientele-0.4.0/src/utils.py
+-rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.4.0/src/writer.py
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 clientele-0.4.0/PKG-INFO
```

### Comparing `clientele-0.3.2/LICENSE` & `clientele-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clientele-0.3.2/README.md` & `clientele-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
     <h1>⚜️ Clientele</h1>
     <em>Typed API Clients from OpenAPI schemas</em>
-    <img src="https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true">
+    <img src="https://github.com/phalt/clientele/blob/main/docs/clientele.jpeg?raw=true">
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/clientele" target="_blank">
     <img src="https://img.shields.io/pypi/v/clientele?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/clientele" target="_blank">
@@ -27,24 +27,24 @@
 * Supports authentication (curently only HTTP Bearer and HTTP Basic auth).
 * Written entirely in Python - no need to install other languages to use OpenAPI.
 * The client footprint is minimal - it only requires `httpx` and `pydantic`.
 * Supports your own configuration - we provide an entry point that will never be overwritten.
 
 We're built on:
 
-* [Pydantic 2.0](https://docs.pydantic.dev/latest/)
+* [Pydantic 2.1](https://docs.pydantic.dev/latest/)
 * [httpx](https://www.python-httpx.org/)
 * [openapi-core](https://openapi-core.readthedocs.io/en/latest/)
 
 ## Install
 
 ```sh
-poetry add clientele
+pipx add clientele
 ```
 
 ## Usage
 
 ```sh
 clientele generate -f path/to/file.json -o my_client/ --asyncio t
 ```
 
-[Read the docs](https://beckett-software.github.io/clientele/)
+[Read the docs](https://phalt.github.io/clientele/)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 ****** âï¸ Clientele ******
-Typed API Clients from OpenAPI schemas [https://github.com/beckett-software/
-clientele/blob/main/docs/clientele.jpeg?raw=true]
+Typed API Clients from OpenAPI schemas [https://github.com/phalt/clientele/
+blob/main/docs/clientele.jpeg?raw=true]
                  [Package_version] [Supported_Python_versions]
 Clientele lets you generate fully-typed, functional, API Clients from OpenAPI
 schemas. It uses modern tools to be blazing fast and type safe. Plus - there is
 no complex boilerplate and the generated code is very small. ## Features *
 Fully typed API Client using Pydantic. * Minimalist and easy to use - the
 generated code is designed for readability. * Choose either sync or async - we
 support both, and you can switch between them easily. * Supports authentication
 (curently only HTTP Bearer and HTTP Basic auth). * Written entirely in Python -
 no need to install other languages to use OpenAPI. * The client footprint is
 minimal - it only requires `httpx` and `pydantic`. * Supports your own
 configuration - we provide an entry point that will never be overwritten. We're
-built on: * [Pydantic 2.0](https://docs.pydantic.dev/latest/) * [httpx](https:/
+built on: * [Pydantic 2.1](https://docs.pydantic.dev/latest/) * [httpx](https:/
 /www.python-httpx.org/) * [openapi-core](https://openapi-core.readthedocs.io/
-en/latest/) ## Install ```sh poetry add clientele ``` ## Usage ```sh clientele
+en/latest/) ## Install ```sh pipx add clientele ``` ## Usage ```sh clientele
 generate -f path/to/file.json -o my_client/ --asyncio t ``` [Read the docs]
-(https://beckett-software.github.io/clientele/)
+(https://phalt.github.io/clientele/)
```

### Comparing `clientele-0.3.2/pyproject.toml` & `clientele-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "clientele"
-version = "0.3.2"
+version = "0.4.0"
 description = "Typed API Clients from OpenAPI schemas"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
-homepage = "https://beckett-software.github.io/clientele/"
+homepage = "https://phalt.github.io/clientele/"
 
 [tool.poetry.scripts]
 clientele = "src.cli:cli_group"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.24.1"
 click = "^8.1.3"
-pydantic = "^2.0.3"
+pydantic = "^2.1.1"
 rich = "^13.4.2"
 openapi-core = "0.18.0"
 pyyaml = "^6.0.1"
 types-pyyaml = "^6.0.12.11"
+jinja2 = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "1.4.0"
 ruff = "^0.0.272"
 mkdocs = "^1.4.3"
 ipython = "^8.14.0"
```

### Comparing `clientele-0.3.2/src/constants_template.py` & `clientele-0.4.0/src/constants_template.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.2/src/generator.py` & `clientele-0.4.0/src/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from shutil import copyfile
 
 from openapi_core import Spec
 
 from src.generators.clients import ClientsGenerator
 from src.generators.http import HTTPGenerator
 from src.generators.schemas import SchemasGenerator
-from src.settings import CONSTANTS_ROOT, TEMPLATE_ROOT, VERSION
+from src.settings import CLIENT_TEMPLATE_ROOT, CONSTANTS_ROOT, VERSION
 from src.writer import write_to_manifest
 
 
 class Generator:
     """
     Top-level generator.
     """
@@ -45,15 +45,15 @@
         write_to_manifest(
             f"API VERSION: {self.spec['info']['version']}\n", self.output_dir
         )
         write_to_manifest(f"OPENAPI VERSION: {self.spec['openapi']}\n", self.output_dir)
         write_to_manifest(f"CLIENTELE VERSION: {VERSION}\n", self.output_dir)
 
     def generate(self) -> None:
-        copy_tree(src=TEMPLATE_ROOT, dst=self.output_dir)
+        copy_tree(src=CLIENT_TEMPLATE_ROOT, dst=self.output_dir)
         if not exists(f"{self.output_dir}constants.py"):
             copyfile(
                 f"{CONSTANTS_ROOT}/constants_template.py",
                 f"{self.output_dir}constants.py",
             )
         self.generate_manifest()
         self.schemas_generator.generate_schema_classes()
```

### Comparing `clientele-0.3.2/src/generators/clients.py` & `clientele-0.4.0/src/generators/clients.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 from collections import defaultdict
-from typing import Any, Dict, List
+from typing import Optional
 
 from openapi_core import Spec
+from pydantic import BaseModel
 from rich.console import Console
 
 from src.generators.schemas import SchemasGenerator
-from src.utils import class_name_titled, clean_prop, get_func_name, get_type
+from src.settings import templates
+from src.utils import (
+    class_name_titled,
+    clean_prop,
+    create_query_args,
+    get_func_name,
+    get_param_from_ref,
+    get_type,
+    schema_ref,
+)
 from src.writer import write_to_client
 
 console = Console()
 
 
+class ParametersResponse(BaseModel):
+    # Parameters that need to be passed in the URL query
+    query_args: dict[str, str]
+    # Parameters that need to be passed as variables in the function
+    path_args: dict[str, str]
+    # Parameters that are needed in the headers object
+    headers_args: dict[str, str]
+
+    def get_path_args_as_string(self):
+        # Get all the path arguments, and the query arguments and make a big string out of them.
+        args = list(self.path_args.items()) + list(self.query_args.items())
+        return ", ".join(f"{k}: {v}" for k, v in args)
+
+
 class ClientsGenerator:
     """
     Handles all the content generated in the clients.py file.
     """
 
-    results: Dict[str, int]
+    method_template_map: dict[str, str]
+    results: dict[str, int]
     spec: Spec
     output_dir: str
     schemas_generator: SchemasGenerator
 
     def __init__(
         self,
         spec: Spec,
@@ -29,164 +54,180 @@
         asyncio: bool,
     ) -> None:
         self.spec = spec
         self.output_dir = output_dir
         self.results = defaultdict(int)
         self.schemas_generator = schemas_generator
         self.asyncio = asyncio
+        self.method_template_map = dict(
+            get="get_method.jinja2",
+            delete="get_method.jinja2",
+            post="post_method.jinja2",
+        )
 
     def generate_paths(self) -> None:
         for path in self.spec["paths"].items():
             self.write_path_to_client(path=path)
-        console.log(f"Generated {self.results['get_methods']} GET methods...")
-        console.log(f"Generated {self.results['post_methods']} POST methods...")
-
-    def generate_function_args(self, parameters: List[Dict]) -> Dict[str, Any]:
-        return_string_bits = []
+        console.log(f"Generated {self.results['get']} GET methods...")
+        console.log(f"Generated {self.results['post']} POST methods...")
+        console.log(f"Generated {self.results['delete']} DELETE methods...")
+
+    def generate_parameters(
+        self, parameters: list[dict], additional_parameters: list[dict]
+    ) -> ParametersResponse:
         param_keys = []
-        query_args = []
-        path_args = []
-        for p in parameters:
-            if p.get("$ref"):
-                # Not currently supporter
-                continue
-            clean_key = clean_prop(p["name"])
+        query_args = {}
+        path_args = {}
+        headers_args = {}
+        all_parameters = parameters + additional_parameters
+        for param in all_parameters:
+            if param.get("$ref"):
+                # Get the actual parameter it is referencing
+                param = get_param_from_ref(spec=self.spec, param=param)
+            clean_key = clean_prop(param["name"])
             if clean_key in param_keys:
                 continue
-            in_ = p.get("in")
-            required = p.get("required", False) or in_ != "query"
+            in_ = param.get("in")
+            required = param.get("required", False) or in_ != "query"
             if in_ == "query":
-                query_args.append(p["name"])
+                # URL query string values
+                if required:
+                    query_args[clean_key] = get_type(param["schema"])
+                else:
+                    query_args[
+                        clean_key
+                    ] = f"typing.Optional[{get_type(param['schema'])}]"
             elif in_ == "path":
-                path_args.append(p["name"])
-            if required:
-                return_string_bits.append(f"{clean_key}: {get_type(p['schema'])}")
-            else:
-                return_string_bits.append(
-                    f"{clean_key}: typing.Optional[{get_type(p['schema'])}]"
-                )
+                # Function arguments
+                if required:
+                    path_args[clean_key] = get_type(param["schema"])
+                else:
+                    path_args[
+                        clean_key
+                    ] = f"typing.Optional[{get_type(param['schema'])}]"
+            elif in_ == "header":
+                # Header object arguments
+                headers_args[param["name"]] = get_type(param["schema"])
             param_keys.append(clean_key)
-        return_string = ", ".join(return_string_bits)
-        return {
-            "return_string": return_string,
-            "query_args": query_args,
-            "path_args": path_args,
-        }
+        return ParametersResponse(
+            query_args=query_args,
+            path_args=path_args,
+            headers_args=headers_args,
+        )
 
-    def get_response_class_names(self, responses: Dict) -> List[str]:
+    def get_response_class_names(self, responses: dict) -> list[str]:
         """
         Generates a list of response class for this operation.
         """
         response_classes = []
         for _, details in responses.items():
             for encoding, content in details.get("content", {}).items():
                 class_name = ""
                 if ref := content["schema"].get("$ref", False):
-                    class_name = class_name_titled(
-                        ref.replace("#/components/schemas/", "")
-                    )
+                    class_name = class_name_titled(schema_ref(ref))
                 elif title := content["schema"].get("title", False):
                     class_name = class_name_titled(title)
                 else:
                     class_name = class_name_titled(encoding)
                 response_classes.append(class_name)
         return list(set(response_classes))
 
-    def get_input_class_names(self, inputs: Dict) -> List[str]:
+    def get_input_class_names(self, inputs: dict) -> list[str]:
         """
         Generates a list of input class for this operation.
         """
         input_classes = []
         for _, details in inputs.items():
             for encoding, content in details.get("content", {}).items():
                 class_name = ""
                 if ref := content["schema"].get("$ref", False):
-                    class_name = class_name_titled(
-                        ref.replace("#/components/schemas/", "")
-                    )
+                    class_name = class_name_titled(schema_ref(ref))
                 elif title := content["schema"].get("title", False):
                     class_name = title
                 else:
                     # No idea, using the encoding?
                     class_name = encoding
                 class_name = class_name_titled(class_name)
                 input_classes.append(class_name)
         return list(set(input_classes))
 
-    def generate_response_types(self, responses: Dict) -> str:
+    def generate_response_types(self, responses: dict) -> str:
         response_class_names = self.get_response_class_names(responses=responses)
         if len(response_class_names) > 1:
             return f"""typing.Union[{', '.join([f'schemas.{r}' for r in response_class_names])}]"""
         elif len(response_class_names) == 0:
             return "None"
         else:
             return f"schemas.{response_class_names[0]}"
 
-    def generate_input_types(self, request_body: Dict) -> str:
+    def generate_input_types(self, request_body: dict) -> str:
         input_class_names = self.get_input_class_names(inputs={"": request_body})
         for input_class in input_class_names:
             if input_class not in self.schemas_generator.schemas.keys():
                 # It doesn't exist! Generate the schema for it
                 self.schemas_generator.generate_input_class(schema=request_body)
         if len(input_class_names) > 1:
             return f"""typing.Union[{', '.join([f'schemas.{r}' for r in input_class_names])}]"""
         elif len(input_class_names) == 0:
             return "None"
         else:
             return f"schemas.{input_class_names[0]}"
 
-    def generate_get_content(self, operation: Dict, path: str) -> None:
+    def generate_function(
+        self,
+        operation: dict,
+        method: str,
+        url: str,
+        additional_parameters: list[dict],
+        summary: Optional[str],
+    ):
         response_types = self.generate_response_types(operation["responses"])
-        func_name = get_func_name(operation, path)
-        function_arguments = self.generate_function_args(
-            operation.get("parameters", [])
+        func_name = get_func_name(operation, url)
+        function_arguments = self.generate_parameters(
+            parameters=operation.get("parameters", []),
+            additional_parameters=additional_parameters,
         )
-        if query_args := function_arguments["query_args"]:
-            # TODO do this far more elegantly
-            api_url = (
-                path + "?" + "&".join([f"{p}=" + "{" + p + "}" for p in query_args])
-            )
+        if query_args := function_arguments.query_args:
+            api_url = url + create_query_args(query_args)
         else:
-            api_url = path
-        CONTENT = f"""
-{self.asyncio and "async " or ""}def {func_name}({function_arguments['return_string']}) -> {response_types}:
-    response = {self.asyncio and "await " or ""}http.get(f"{api_url}")
-    return http.handle_response({func_name}, response)
-    """
-        self.results["get_methods"] += 1
-        write_to_client(content=CONTENT, output_dir=self.output_dir)
-
-    def generate_post_content(self, operation: Dict, path: str) -> None:
-        response_types = self.generate_response_types(operation["responses"])
-        func_name = get_func_name(operation, path)
-        if not operation.get("requestBody"):
-            input_class_name = "None"
-        else:
-            input_class_name = self.generate_input_types(
+            api_url = url
+        if method in ["post"] and not operation.get("requestBody"):
+            data_class_name = "None"
+        elif method in ["post"]:
+            data_class_name = self.generate_input_types(
                 operation.get("requestBody", {})
             )
-        function_arguments = self.generate_function_args(
-            operation.get("parameters", [])
+        else:
+            data_class_name = None
+        self.results[method] += 1
+        template = templates.get_template(self.method_template_map[method])
+        if headers := function_arguments.headers_args:
+            header_class_name = self.schemas_generator.generate_headers_class(
+                properties=headers,
+                func_name=func_name,
+            )
+        else:
+            header_class_name = None
+        content = template.render(
+            asyncio=self.asyncio,
+            func_name=func_name,
+            function_arguments=function_arguments.get_path_args_as_string(),
+            response_types=response_types,
+            data_class_name=data_class_name,
+            header_class_name=header_class_name,
+            api_url=api_url,
+            method=method,
+            summary=operation.get("summary", summary),
         )
-        FUNCTION_ARGS = f"""
-{function_arguments['return_string']}{function_arguments['return_string'] and ", "}data: {input_class_name}"""
-        CONTENT = f"""
-{self.asyncio and "async " or ""}def {func_name}({FUNCTION_ARGS}) -> {response_types}:
-    response = {self.asyncio and "await " or ""}http.post(f"{path}", data=data.model_dump())
-    return http.handle_response({func_name}, response)
-    """
-        self.results["post_methods"] += 1
-        write_to_client(content=CONTENT, output_dir=self.output_dir)
+        write_to_client(content=content, output_dir=self.output_dir)
 
-    def write_path_to_client(self, path: Dict) -> None:
+    def write_path_to_client(self, path: dict) -> None:
         url, operations = path
         for method, operation in operations.items():
-            if method == "get":
-                self.generate_get_content(
-                    operation=operation,
-                    path=url,
-                )
-            elif method == "post":
-                self.generate_post_content(
+            if method in self.method_template_map.keys():
+                self.generate_function(
                     operation=operation,
-                    path=url,
+                    method=method,
+                    url=url,
+                    additional_parameters=operations.get("parameters", []),
+                    summary=operations.get("summary", None),
                 )
```

### Comparing `clientele-0.3.2/src/template/http.py` & `clientele-0.4.0/src/client_template/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 from os import environ  # noqa
 from urllib.parse import urlparse
 
 import httpx  # noqa
-from pydantic import ValidationError
+from pydantic import BaseModel, ValidationError  # noqa
 
 from . import constants as c  # noqa
 
 
 def parse_url(url: str) -> str:
     """
     Returns the base API URL for this service
```

### Comparing `clientele-0.3.2/src/utils.py` & `clientele-0.4.0/src/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
-from typing import Dict
+
+from openapi_core import Spec
 
 
 class DataType:
     INTEGER = "integer"
     NUMBER = "number"
     STRING = "string"
     BOOLEAN = "boolean"
@@ -54,31 +55,54 @@
         s = s.replace(badchar, "_")
     s = _split_upper(s)
     if s[0] == "_":
         s = s[1:]
     return s.lower()
 
 
-def get_func_name(operation: Dict, path: str) -> str:
+def get_func_name(operation: dict, path: str) -> str:
     if operation.get("operationId"):
         return _snake_case(operation["operationId"].split("__")[0])
     return _snake_case(path)
 
 
 def get_type(t):
     t_type = t.get("type")
     if t_type == DataType.STRING:
         return "str"
     if t_type in [DataType.INTEGER, DataType.NUMBER]:
         return "int"
     if t_type == DataType.BOOLEAN:
         return "bool"
     if t_type == DataType.OBJECT:
-        return "typing.Dict[str, typing.Any]"
+        return "dict[str, typing.Any]"
     if t_type == DataType.ARRAY:
-        return "typing.List[typing.Any]"
+        return "list[typing.Any]"
     if ref := t.get("$ref"):
         return f'"{class_name_titled(ref.replace("#/components/schemas/", ""))}"'
     if t_type is None:
         # In this case, make it an "Any"
         return "typing.Any"
     return t_type
+
+
+def create_query_args(query_args: list[str]) -> str:
+    return "?" + "&".join([f"{p}=" + "{" + p + "}" for p in query_args])
+
+
+def schema_ref(ref: str) -> str:
+    return ref.replace("#/components/schemas/", "")
+
+
+def param_ref(ref: str) -> str:
+    return ref.replace("#/components/parameters/", "")
+
+
+def get_param_from_ref(spec: Spec, param: dict) -> dict:
+    ref = param.get("$ref")
+    stripped_name = param_ref(ref)
+    return spec["components"]["parameters"][stripped_name]
+
+
+def get_schema_from_ref(spec: Spec, ref: str) -> dict:
+    stripped_name = schema_ref(ref)
+    return spec["components"]["schemas"][stripped_name]
```

### Comparing `clientele-0.3.2/src/writer.py` & `clientele-0.4.0/src/writer.py`

 * *Files identical despite different names*

### Comparing `clientele-0.3.2/PKG-INFO` & `clientele-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: clientele
-Version: 0.3.2
+Version: 0.4.0
 Summary: Typed API Clients from OpenAPI schemas
-Home-page: https://beckett-software.github.io/clientele/
+Home-page: https://phalt.github.io/clientele/
 License: MIT
 Author: Paul Hallett
 Author-email: paulandrewhallett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: openapi-core (==0.18.0)
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.11,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <h1>⚜️ Clientele</h1>
     <em>Typed API Clients from OpenAPI schemas</em>
-    <img src="https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true">
+    <img src="https://github.com/phalt/clientele/blob/main/docs/clientele.jpeg?raw=true">
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/clientele" target="_blank">
     <img src="https://img.shields.io/pypi/v/clientele?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/clientele" target="_blank">
@@ -50,25 +51,25 @@
 * Supports authentication (curently only HTTP Bearer and HTTP Basic auth).
 * Written entirely in Python - no need to install other languages to use OpenAPI.
 * The client footprint is minimal - it only requires `httpx` and `pydantic`.
 * Supports your own configuration - we provide an entry point that will never be overwritten.
 
 We're built on:
 
-* [Pydantic 2.0](https://docs.pydantic.dev/latest/)
+* [Pydantic 2.1](https://docs.pydantic.dev/latest/)
 * [httpx](https://www.python-httpx.org/)
 * [openapi-core](https://openapi-core.readthedocs.io/en/latest/)
 
 ## Install
 
 ```sh
-poetry add clientele
+pipx add clientele
 ```
 
 ## Usage
 
 ```sh
 clientele generate -f path/to/file.json -o my_client/ --asyncio t
 ```
 
-[Read the docs](https://beckett-software.github.io/clientele/)
+[Read the docs](https://phalt.github.io/clientele/)
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: clientele Version: 0.3.2 Summary: Typed API Clients
-from OpenAPI schemas Home-page: https://beckett-software.github.io/clientele/
-License: MIT Author: Paul Hallett Author-email: paulandrewhallett@gmail.com
-Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist:
-openapi-core (==0.18.0) Requires-Dist: pydantic (>=2.0.3,<3.0.0) Requires-Dist:
-pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist:
-types-pyyaml (>=6.0.12.11,<7.0.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: clientele Version: 0.4.0 Summary: Typed API Clients
+from OpenAPI schemas Home-page: https://phalt.github.io/clientele/ License: MIT
+Author: Paul Hallett Author-email: paulandrewhallett@gmail.com Requires-Python:
+>=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: openapi-core (==0.18.0) Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: types-pyyaml (>=6.0.12.11,<7.0.0.0) Description-Content-Type:
+text/markdown
 ****** âï¸ Clientele ******
-Typed API Clients from OpenAPI schemas [https://github.com/beckett-software/
-clientele/blob/main/docs/clientele.jpeg?raw=true]
+Typed API Clients from OpenAPI schemas [https://github.com/phalt/clientele/
+blob/main/docs/clientele.jpeg?raw=true]
                  [Package_version] [Supported_Python_versions]
 Clientele lets you generate fully-typed, functional, API Clients from OpenAPI
 schemas. It uses modern tools to be blazing fast and type safe. Plus - there is
 no complex boilerplate and the generated code is very small. ## Features *
 Fully typed API Client using Pydantic. * Minimalist and easy to use - the
 generated code is designed for readability. * Choose either sync or async - we
 support both, and you can switch between them easily. * Supports authentication
 (curently only HTTP Bearer and HTTP Basic auth). * Written entirely in Python -
 no need to install other languages to use OpenAPI. * The client footprint is
 minimal - it only requires `httpx` and `pydantic`. * Supports your own
 configuration - we provide an entry point that will never be overwritten. We're
-built on: * [Pydantic 2.0](https://docs.pydantic.dev/latest/) * [httpx](https:/
+built on: * [Pydantic 2.1](https://docs.pydantic.dev/latest/) * [httpx](https:/
 /www.python-httpx.org/) * [openapi-core](https://openapi-core.readthedocs.io/
-en/latest/) ## Install ```sh poetry add clientele ``` ## Usage ```sh clientele
+en/latest/) ## Install ```sh pipx add clientele ``` ## Usage ```sh clientele
 generate -f path/to/file.json -o my_client/ --asyncio t ``` [Read the docs]
-(https://beckett-software.github.io/clientele/)
+(https://phalt.github.io/clientele/)
```

