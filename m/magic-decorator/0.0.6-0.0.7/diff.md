# Comparing `tmp/magic_decorator-0.0.6.tar.gz` & `tmp/magic_decorator-0.0.7.tar.gz`

## Comparing `magic_decorator-0.0.6.tar` & `magic_decorator-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/LICENSE
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 magic_decorator-0.0.7/PKG-INFO
```

### Comparing `magic_decorator-0.0.6/magic_decorator.py` & `magic_decorator-0.0.7/magic_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import inspect
 import json
 import logging
 import textwrap
 from functools import wraps
 
-import sick_json
 import openai
+import sick_json
 from pydantic import BaseModel, Field
 
 
 def _function_stringfy(func):
     docstring = f'"""\n{inspect.cleandoc(inspect.getdoc(func))}\n"""'
     docstring = textwrap.indent(docstring, "    ")
     return f"def {func.__name__}{str(inspect.signature(func))}:\n" f"{docstring}"
 
 
 JSON_PROMPT = "You should always answer according to the JSON schema below: "
 
 
 def get_json_format_prompt(pydantic_model, default_prompt=JSON_PROMPT):
-    return (
-        f"{default_prompt}\n"
-        f"{pydantic_model.schema_json()}"
-    )
+    return f"{default_prompt}\n" f"{pydantic_model.schema_json()}"
 
 
 def get_return_model(return_annotation):
     class Answer(BaseModel):
         thought: str = Field(
             description="Write down your thoughts or reasoning step by step."
         )
@@ -42,16 +39,18 @@
 
 
 SYSTEM_PROMPT = (
     "You are now the following python function:\n"
     "```\n"
     "{function_code}\n"
     "```\n\n"
-    "{json_prompt}"
+    "{format_instruction}"
 )
+
+
 def magic(return_all=False, **openai_kwargs):
     def wrapper(func):
         @wraps(func)
         def do_magic(*args, **kwargs):
             function_code = _function_stringfy(func)
             arguments = []
             for arg in args:
@@ -65,93 +64,108 @@
             json_prompt = get_json_format_prompt(return_model)
 
             messages = [
                 {
                     "role": "system",
                     "content": SYSTEM_PROMPT.format(
                         function_code=function_code,
-                        json_prompt=json_prompt,
+                        format_instruction=json_prompt,
                     ),
                 },
                 {
                     "role": "user",
                     "content": arguments_string,
                 },
             ]
-            
-            
+
             logging.debug("System Message: ")
             logging.debug(messages[0]["content"])
             logging.debug("User Message: ")
             logging.debug(messages[1]["content"])
 
             response = openai.ChatCompletion.create(
                 messages=messages,
                 **openai_kwargs,
             )
-            
+
             logging.debug("Bot Message: ")
             logging.debug(response.choices[0].message.content)
 
             bot_says = sick_json.parse(
                 response.choices[0].message.content,
                 pydantic_model=return_model,
             )
-                
+
             if return_all:
                 return bot_says
             else:
                 return bot_says["return"]
 
         return do_magic
 
     return wrapper
 
+
 try:
-    from langchain.chains import LLMChain
-    from langchain.chat_models import AzureChatOpenAI
     from langchain.base_language import BaseLanguageModel
+    from langchain.chains import LLMChain
+    from langchain.output_parsers.pydantic import PydanticOutputParser
+    from langchain.prompts import (
+        ChatPromptTemplate,
+        HumanMessagePromptTemplate,
+        SystemMessagePromptTemplate,
+    )
     from langchain.schema import BaseOutputParser
-    from langchain.prompts import SystemMessagePromptTemplate, HumanMessagePromptTemplate, ChatPromptTemplate
+
+    class SickJsonOutputParser(PydanticOutputParser):
+        return_all: bool = False
+
+        def parse(self, text: str) -> dict:
+            parsed = sick_json.parse(
+                text,
+                pydantic_model=self.pydantic_object,
+            )
+            return parsed if self.return_all else parsed["return"]
 
     def magic_langchain(llm: BaseLanguageModel, return_all=False):
         def wrapper(func):
             function_code = _function_stringfy(func)
             return_annotation = inspect.signature(func).return_annotation
             return_model = get_return_model(return_annotation)
-            json_prompt = get_json_format_prompt(return_model)
+            output_parser = SickJsonOutputParser(
+                pydantic_object=return_model, return_all=return_all
+            )
 
-            system_prompt = SYSTEM_PROMPT.format(
-                function_code=function_code,
-                json_prompt=json_prompt,
-            ).replace("{", "{{").replace("}", "}}")
+            system_prompt = (
+                SYSTEM_PROMPT.format(
+                    function_code=function_code,
+                    format_instruction=output_parser.get_format_instructions(),
+                )
+                .replace("{", "{{")
+                .replace("}", "}}")
+            )
 
             argument_list = list(inspect.signature(func).parameters.keys())
             arguments = ", ".join(["{" + key + "}" for key in argument_list])
             user_prompt = f"{func.__name__}({arguments})"
 
-            class SickJSONParser(BaseOutputParser):
-                def parse(self, text: str):
-                    parsed = sick_json.parse(
-                        text,
-                        pydantic_model=return_model,
-                    )
-                    return parsed if return_all else parsed["return"]
-
             template = ChatPromptTemplate(
                 input_variables=argument_list,
                 messages=[
                     SystemMessagePromptTemplate.from_template(system_prompt),
                     HumanMessagePromptTemplate.from_template(user_prompt),
                 ],
-                output_parser=SickJSONParser(),
             )
 
             chain = LLMChain(
                 llm=llm,
                 prompt=template,
+                output_parser=output_parser,
+                return_final_only=True,
             )
 
             return chain
+
         return wrapper
+
 except Exception as e:
-    pass
+    pass
```

### Comparing `magic_decorator-0.0.6/.gitignore` & `magic_decorator-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.6/LICENSE` & `magic_decorator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.6/README.md` & `magic_decorator-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,14 @@
     ...
 ```
 
 Added a decorator for langchain. In this case, it becomes LLMChain.
 ```python
 llm = SomeLLMModels()
 @magic_langchain(llm=llm)
-def mychain():
+def mychain(arg1: int, arg2: str):
     ...
 
-mychain.predict_and_parse()
+mychain.predict(arg1=2, arg2="hi")
 ```
 
 There is no preprocessing, no postprocessing, and no error handling in this module. It's just code to do a simple thing, so there are no prompts to encourage better answers.
```

### Comparing `magic_decorator-0.0.6/pyproject.toml` & `magic_decorator-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magic-decorator"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     {name="Kim Minjong", email="make.dirty.code@gmail.com"},
 ]
 description = "A magic function decorator using OpenAI ChatCompletion"
 readme = "README.md"
 requires-python = ">=3.7.1"
 dependencies = ["openai>0.27", "sick-json"]
```

### Comparing `magic_decorator-0.0.6/PKG-INFO` & `magic_decorator-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
@@ -78,14 +78,14 @@
     ...
 ```
 
 Added a decorator for langchain. In this case, it becomes LLMChain.
 ```python
 llm = SomeLLMModels()
 @magic_langchain(llm=llm)
-def mychain():
+def mychain(arg1: int, arg2: str):
     ...
 
-mychain.predict_and_parse()
+mychain.predict(arg1=2, arg2="hi")
 ```
 
 There is no preprocessing, no postprocessing, and no error handling in this module. It's just code to do a simple thing, so there are no prompts to encourage better answers.
```

