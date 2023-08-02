# Comparing `tmp/clientele-0.4.0.tar.gz` & `tmp/clientele-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.4.0.tar", max compression
+gzip compressed data, was "clientele-0.4.1.tar", max compression
```

## Comparing `clientele-0.4.0.tar` & `clientele-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.4.0/LICENSE
--rw-r--r--   0        0        0     1718 2023-08-02 04:28:12.938554 clientele-0.4.0/README.md
--rw-r--r--   0        0        0      905 2023-08-01 23:12:34.358150 clientele-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.4.0/src/__init__.py
--rw-r--r--   0        0        0     2924 2023-08-01 23:27:45.401764 clientele-0.4.0/src/cli.py
--rw-r--r--   0        0        0       50 2023-07-31 02:40:13.111663 clientele-0.4.0/src/client_template/MANIFEST
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.4.0/src/client_template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.4.0/src/client_template/client.py
--rw-r--r--   0        0        0      993 2023-08-02 03:52:10.187256 clientele-0.4.0/src/client_template/http.py
--rw-r--r--   0        0        0       76 2023-08-02 03:43:33.184239 clientele-0.4.0/src/client_template/schemas.py
--rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.4.0/src/constants_template.py
--rw-r--r--   0        0        0     2069 2023-08-01 23:23:41.098914 clientele-0.4.0/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.4.0/src/generators/__init__.py
--rw-r--r--   0        0        0     8929 2023-08-02 04:19:58.737007 clientele-0.4.0/src/generators/clients.py
--rw-r--r--   0        0        0     2832 2023-08-02 02:28:17.182281 clientele-0.4.0/src/generators/http.py
--rw-r--r--   0        0        0     5850 2023-08-02 04:19:58.733008 clientele-0.4.0/src/generators/schemas.py
--rw-r--r--   0        0        0      391 2023-08-01 23:23:41.098914 clientele-0.4.0/src/settings.py
--rw-r--r--   0        0        0      464 2023-08-02 04:21:15.956387 clientele-0.4.0/src/templates/async_methods.jinja
--rw-r--r--   0        0        0       75 2023-08-01 23:33:19.745482 clientele-0.4.0/src/templates/basic_client.jinja2
--rw-r--r--   0        0        0      134 2023-08-01 23:34:59.694567 clientele-0.4.0/src/templates/bearer_client.jinja2
--rw-r--r--   0        0        0       34 2023-08-01 23:32:13.768760 clientele-0.4.0/src/templates/client.jinja2
--rw-r--r--   0        0        0      562 2023-08-02 04:26:47.439084 clientele-0.4.0/src/templates/get_method.jinja2
--rw-r--r--   0        0        0      607 2023-08-02 04:27:04.858109 clientele-0.4.0/src/templates/post_method.jinja2
--rw-r--r--   0        0        0      115 2023-08-02 04:06:42.400353 clientele-0.4.0/src/templates/schema_class.jinja2
--rw-r--r--   0        0        0      428 2023-08-02 04:21:04.265390 clientele-0.4.0/src/templates/sync_methods.jinja2
--rw-r--r--   0        0        0     2829 2023-08-02 04:19:58.733008 clientele-0.4.0/src/utils.py
--rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.4.0/src/writer.py
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 clientele-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1718 2023-08-02 04:28:12.938554 clientele-0.4.1/README.md
+-rw-r--r--   0        0        0      905 2023-08-02 21:28:27.197731 clientele-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.4.1/src/__init__.py
+-rw-r--r--   0        0        0     2924 2023-08-01 23:27:45.401764 clientele-0.4.1/src/cli.py
+-rw-r--r--   0        0        0       50 2023-07-31 02:40:13.111663 clientele-0.4.1/src/client_template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.4.1/src/client_template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.4.1/src/client_template/client.py
+-rw-r--r--   0        0        0      993 2023-08-02 03:52:10.187256 clientele-0.4.1/src/client_template/http.py
+-rw-r--r--   0        0        0       76 2023-08-02 03:43:33.184239 clientele-0.4.1/src/client_template/schemas.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.4.1/src/constants_template.py
+-rw-r--r--   0        0        0     2069 2023-08-01 23:23:41.098914 clientele-0.4.1/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.4.1/src/generators/__init__.py
+-rw-r--r--   0        0        0     9967 2023-08-02 21:23:33.310164 clientele-0.4.1/src/generators/clients.py
+-rw-r--r--   0        0        0     2830 2023-08-02 21:22:03.573057 clientele-0.4.1/src/generators/http.py
+-rw-r--r--   0        0        0     6297 2023-08-02 21:11:36.405951 clientele-0.4.1/src/generators/schemas.py
+-rw-r--r--   0        0        0      391 2023-08-02 21:28:31.333711 clientele-0.4.1/src/settings.py
+-rw-r--r--   0        0        0      464 2023-08-02 04:21:15.956387 clientele-0.4.1/src/templates/async_methods.jinja2
+-rw-r--r--   0        0        0       75 2023-08-01 23:33:19.745482 clientele-0.4.1/src/templates/basic_client.jinja2
+-rw-r--r--   0        0        0      134 2023-08-01 23:34:59.694567 clientele-0.4.1/src/templates/bearer_client.jinja2
+-rw-r--r--   0        0        0       34 2023-08-01 23:32:13.768760 clientele-0.4.1/src/templates/client.jinja2
+-rw-r--r--   0        0        0      571 2023-08-02 21:24:19.832994 clientele-0.4.1/src/templates/get_method.jinja2
+-rw-r--r--   0        0        0      607 2023-08-02 04:27:04.858109 clientele-0.4.1/src/templates/post_method.jinja2
+-rw-r--r--   0        0        0      115 2023-08-02 04:06:42.400353 clientele-0.4.1/src/templates/schema_class.jinja2
+-rw-r--r--   0        0        0      428 2023-08-02 04:21:04.265390 clientele-0.4.1/src/templates/sync_methods.jinja2
+-rw-r--r--   0        0        0     2884 2023-08-02 21:18:05.831839 clientele-0.4.1/src/utils.py
+-rw-r--r--   0        0        0      558 2023-08-02 21:21:10.707203 clientele-0.4.1/src/writer.py
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 clientele-0.4.1/PKG-INFO
```

### Comparing `clientele-0.4.0/LICENSE` & `clientele-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/README.md` & `clientele-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/pyproject.toml` & `clientele-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clientele"
-version = "0.4.0"
+version = "0.4.1"
 description = "Typed API Clients from OpenAPI schemas"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
 homepage = "https://phalt.github.io/clientele/"
```

### Comparing `clientele-0.4.0/src/cli.py` & `clientele-0.4.1/src/cli.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/src/client_template/http.py` & `clientele-0.4.1/src/client_template/http.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/src/constants_template.py` & `clientele-0.4.1/src/constants_template.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/src/generator.py` & `clientele-0.4.1/src/generator.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/src/generators/clients.py` & `clientele-0.4.1/src/generators/clients.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,28 +110,42 @@
             param_keys.append(clean_key)
         return ParametersResponse(
             query_args=query_args,
             path_args=path_args,
             headers_args=headers_args,
         )
 
-    def get_response_class_names(self, responses: dict) -> list[str]:
+    def get_response_class_names(self, responses: dict, func_name: str) -> list[str]:
         """
         Generates a list of response class for this operation.
         """
         response_classes = []
-        for _, details in responses.items():
-            for encoding, content in details.get("content", {}).items():
+        for status_code, details in responses.items():
+            for _, content in details.get("content", {}).items():
                 class_name = ""
                 if ref := content["schema"].get("$ref", False):
+                    # An object reference, so should be generated
+                    # by the schema generator later.
                     class_name = class_name_titled(schema_ref(ref))
                 elif title := content["schema"].get("title", False):
+                    # This usually means we have an object that isn't
+                    # $ref so we need to create the schema class here
                     class_name = class_name_titled(title)
+                    self.schemas_generator.make_schema_class(
+                        class_name, schema=content["schema"]
+                    )
                 else:
-                    class_name = class_name_titled(encoding)
+                    # At this point we're just making things up!
+                    # It is likely it isn't an object it is just a simple resonse.
+                    class_name = class_name_titled(func_name + status_code + "Response")
+                    # We need to generate the class at this point because it does not exist
+                    self.schemas_generator.make_schema_class(
+                        func_name + status_code + "Response",
+                        schema={"properties": {"test": content["schema"]}},
+                    )
                 response_classes.append(class_name)
         return list(set(response_classes))
 
     def get_input_class_names(self, inputs: dict) -> list[str]:
         """
         Generates a list of input class for this operation.
         """
@@ -146,16 +160,18 @@
                 else:
                     # No idea, using the encoding?
                     class_name = encoding
                 class_name = class_name_titled(class_name)
                 input_classes.append(class_name)
         return list(set(input_classes))
 
-    def generate_response_types(self, responses: dict) -> str:
-        response_class_names = self.get_response_class_names(responses=responses)
+    def generate_response_types(self, responses: dict, func_name: str) -> str:
+        response_class_names = self.get_response_class_names(
+            responses=responses, func_name=func_name
+        )
         if len(response_class_names) > 1:
             return f"""typing.Union[{', '.join([f'schemas.{r}' for r in response_class_names])}]"""
         elif len(response_class_names) == 0:
             return "None"
         else:
             return f"schemas.{response_class_names[0]}"
 
@@ -176,22 +192,24 @@
         self,
         operation: dict,
         method: str,
         url: str,
         additional_parameters: list[dict],
         summary: Optional[str],
     ):
-        response_types = self.generate_response_types(operation["responses"])
         func_name = get_func_name(operation, url)
+        response_types = self.generate_response_types(
+            responses=operation["responses"], func_name=func_name
+        )
         function_arguments = self.generate_parameters(
             parameters=operation.get("parameters", []),
             additional_parameters=additional_parameters,
         )
         if query_args := function_arguments.query_args:
-            api_url = url + create_query_args(query_args)
+            api_url = url + create_query_args(list(query_args.keys()))
         else:
             api_url = url
         if method in ["post"] and not operation.get("requestBody"):
             data_class_name = "None"
         elif method in ["post"]:
             data_class_name = self.generate_input_types(
                 operation.get("requestBody", {})
```

### Comparing `clientele-0.4.0/src/generators/http.py` & `clientele-0.4.1/src/generators/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,11 +59,11 @@
         if client_generated is False:
             console.log(f"Generating {'async' if self.asyncio else 'sync'} client...")
             template = templates.get_template("client.jinja2")
             content = template.render(client_type=client_type)
             client_generated = True
         write_to_http(content, output_dir=self.output_dir)
         if self.asyncio:
-            template = templates.get_template("async_methods.jinja").render()
+            content = templates.get_template("async_methods.jinja2").render()
         else:
-            template = templates.get_template("sync_methods.jinja2").render()
-        write_to_http(template, output_dir=self.output_dir)
+            content = templates.get_template("sync_methods.jinja2").render()
+        write_to_http(content, output_dir=self.output_dir)
```

### Comparing `clientele-0.4.0/src/generators/schemas.py` & `clientele-0.4.1/src/generators/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,51 +103,61 @@
                     class_name=class_name, properties=properties, enum=False
                 )
             write_to_schemas(
                 out_content,
                 output_dir=self.output_dir,
             )
 
-    def generate_schema_classes(self) -> None:
-        """
-        Generates the Pydantic response classes.
-        """
-        for schema_key, schema in self.spec["components"]["schemas"].items():
-            schema_key = class_name_titled(schema_key)
-            enum = False
-            properties: str = ""
-            if all_of := schema.get("allOf"):
-                # This schema uses "all of" the properties from another model
-                for other_ref in all_of:
-                    other_schema_key = class_name_titled(schema_ref(other_ref["$ref"]))
+    def make_schema_class(self, schema_key: str, schema: dict) -> None:
+        schema_key = class_name_titled(schema_key)
+        enum = False
+        properties: str = ""
+        if all_of := schema.get("allOf"):
+            # This schema uses "all of" the properties inside it
+            for other_ref in all_of:
+                is_ref = other_ref.get("$ref", False)
+                if is_ref:
+                    other_schema_key = class_name_titled(schema_ref(is_ref))
                     if other_schema_key in self.schemas:
                         properties += self.schemas[other_schema_key]
                     else:
-                        # We need to generate it now
-                        schema_model = get_schema_from_ref(
-                            spec=self.spec, ref=other_ref["$ref"]
-                        )
+                        # It's a ref but we've just not made it yet
+                        schema_model = get_schema_from_ref(spec=self.spec, ref=is_ref)
                         properties += self.generate_class_properties(
                             properties=schema_model.get("properties", {}),
                             required=schema_model.get("required", None),
                         )
-            elif schema.get("enum"):
-                enum = True
-                properties = self.generate_enum_properties(
-                    {v: {"type": f'"{v}"'} for v in schema["enum"]}
-                )
-            else:
-                properties = self.generate_class_properties(
-                    properties=schema.get("properties", {}),
-                    required=schema.get("required", None),
-                )
-            self.schemas[schema_key] = properties
-            template = templates.get_template("schema_class.jinja2")
-            content = template.render(
-                class_name=schema_key, properties=properties, enum=enum
+                else:
+                    # It's not a ref and we need to figure out what it is
+                    if other_ref.get("type") == "object":
+                        properties += self.generate_class_properties(
+                            properties=other_ref.get("properties", {}),
+                            required=other_ref.get("required", None),
+                        )
+        elif schema.get("enum"):
+            enum = True
+            properties = self.generate_enum_properties(
+                {v: {"type": f'"{v}"'} for v in schema["enum"]}
             )
-            write_to_schemas(
-                content,
-                output_dir=self.output_dir,
+        else:
+            properties = self.generate_class_properties(
+                properties=schema.get("properties", {}),
+                required=schema.get("required", None),
             )
+        self.schemas[schema_key] = properties
+        template = templates.get_template("schema_class.jinja2")
+        content = template.render(
+            class_name=schema_key, properties=properties, enum=enum
+        )
+        write_to_schemas(
+            content,
+            output_dir=self.output_dir,
+        )
+
+    def generate_schema_classes(self) -> None:
+        """
+        Generates all Pydantic schema classes.
+        """
+        for schema_key, schema in self.spec["components"]["schemas"].items():
+            self.make_schema_class(schema_key=schema_key, schema=schema)
 
         console.log(f"Generated {len(self.schemas.items())} schemas...")
```

### Comparing `clientele-0.4.0/src/templates/get_method.jinja2` & `clientele-0.4.1/src/templates/get_method.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 
 
 {{asyncio and "async " or ""}}def {{func_name}}({{function_arguments}}{% if header_class_name %}{% if function_arguments%}, {% endif %}headers: {{header_class_name}}{% endif %}) -> {{response_types}}:
     {% if summary %}""" {{summary}} """{% endif %}
-    {% if header_class_name %}headers_dict = headers and headers.model_dump(by_alias=True) or None {% endif %}
+    {% if header_class_name %}headers_dict = headers and headers.model_dump(by_alias=True) or None {% else%}{% endif %}
     response = {{asyncio and "await " or ""}}http.{{method}}(url=f"{{api_url}}"{% if header_class_name %}, headers=headers_dict{% endif %})
     return http.handle_response({{func_name}}, response)
```

### Comparing `clientele-0.4.0/src/templates/post_method.jinja2` & `clientele-0.4.1/src/templates/post_method.jinja2`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/src/utils.py` & `clientele-0.4.1/src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,16 @@
     if t_type in [DataType.INTEGER, DataType.NUMBER]:
         return "int"
     if t_type == DataType.BOOLEAN:
         return "bool"
     if t_type == DataType.OBJECT:
         return "dict[str, typing.Any]"
     if t_type == DataType.ARRAY:
-        return "list[typing.Any]"
+        inner_class = get_type(t.get("items"))
+        return f"list[{inner_class}]"
     if ref := t.get("$ref"):
         return f'"{class_name_titled(ref.replace("#/components/schemas/", ""))}"'
     if t_type is None:
         # In this case, make it an "Any"
         return "typing.Any"
     return t_type
 
@@ -94,15 +95,15 @@
 
 
 def param_ref(ref: str) -> str:
     return ref.replace("#/components/parameters/", "")
 
 
 def get_param_from_ref(spec: Spec, param: dict) -> dict:
-    ref = param.get("$ref")
+    ref = param.get("$ref", "")
     stripped_name = param_ref(ref)
     return spec["components"]["parameters"][stripped_name]
 
 
 def get_schema_from_ref(spec: Spec, ref: str) -> dict:
     stripped_name = schema_ref(ref)
     return spec["components"]["schemas"][stripped_name]
```

### Comparing `clientele-0.4.0/src/writer.py` & `clientele-0.4.1/src/writer.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.0/PKG-INFO` & `clientele-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clientele
-Version: 0.4.0
+Version: 0.4.1
 Summary: Typed API Clients from OpenAPI schemas
 Home-page: https://phalt.github.io/clientele/
 License: MIT
 Author: Paul Hallett
 Author-email: paulandrewhallett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clientele Version: 0.4.0 Summary: Typed API Clients
+Metadata-Version: 2.1 Name: clientele Version: 0.4.1 Summary: Typed API Clients
 from OpenAPI schemas Home-page: https://phalt.github.io/clientele/ License: MIT
 Author: Paul Hallett Author-email: paulandrewhallett@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
```

