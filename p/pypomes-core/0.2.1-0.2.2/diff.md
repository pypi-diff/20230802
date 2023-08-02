# Comparing `tmp/pypomes_core-0.2.1.tar.gz` & `tmp/pypomes_core-0.2.2.tar.gz`

## Comparing `pypomes_core-0.2.1.tar` & `pypomes_core-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27260 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/README.md
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27324 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/README.md
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/PKG-INFO
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/__init__.py` & `pypomes_core-0.2.2/src/pypomes_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,8 @@
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
 ]
 
 __version__ = "0.2.1"
-__version_info__ = (0, 2, 1)
+__version_info__ = (0, 2, 2)
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/dict_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         else:
             # no, retrieve the element corresponding to 'key' in the dictionary
             result = result.get(key)
 
     return result
 
 
-def dict_set_value(target: dict, key_chain: list[str], value: any):
+def dict_set_value(target: dict, key_chain: list[str], value: any) -> None:
     """
     Assign to an element of *source* the value *value*.
 
     The element in question is appointed to by the key chain *[keys[0]: ... :keys[n]*.
     If the element does not exist, it is created with the specified value.
     Any non-existing intermediate elements are created with the value of an empty *dict*.
     A key might indicate the position of the element within a list, using the format *<key>[<pos>]*.
@@ -215,23 +215,23 @@
         elif key in parent:
             # sim, remova o elemento indicado e retorne seu valor
             result = parent.pop(key)
 
     return result
 
 
-def dict_replace_value(target: dict, old_value: any, new_value: any):
+def dict_replace_value(target: dict, old_value: any, new_value: any) -> None:
     """
     Replace in *target* all occurrences of *old_value* with *new_value*.
 
     :param target: the reference dict
     :param old_value: the value to be replaced
     :param new_value: the new value
     """
-    def list_replace_value(items: list[any], old_val: any, new_val: any):
+    def list_replace_value(items: list[any], old_val: any, new_val: any) -> None:
         # traverse the list
         for item in items:
 
             # is 'item' a dict ?
             if isinstance(item, dict):
                 # yes, process it recursively
                 dict_replace_value(item, old_val, new_val)
@@ -289,15 +289,15 @@
     :param source: dicionário a ser pesquisado
     :param value: valor de referência
     :return: lista de chaves associadas ao valor de referência
     """
     return [key for key, val in source.items() if val == value]
 
 
-def dict_merge(target: dict, source: dict):
+def dict_merge(target: dict, source: dict) -> None:
     """
     Percorre os elementos de *source* para atualizar *target*, obedecendo um conjunto de critérios.
 
     Os critérios a sere mseguidos são:
       - acrescentar o elemento a *target*, se não existir
       - se o elemento existir em *target*:
 
@@ -331,15 +331,15 @@
                 # os elementos não são ambos listas ou dicionários, substitua o valor em target
                 target[skey] = svalue
         else:
             # não, acrescente-o
             target[skey] = svalue
 
 
-def dict_coalesce(target: dict, key_chain: list[str]):
+def dict_coalesce(target: dict, key_chain: list[str]) -> None:
     """
     Coalesce o elemento do tipo *list* em *target* no nível *n*, com a lista no nível imediatamente anterior.
 
     Esse elemento é apontado pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*, e é processado
     como uma sequência de multiplos elementos. Para tanto, as duas últimas chaves da cadeia
     *key_chain* devem estar associadas a valores do tipo *list*.
 
@@ -428,15 +428,15 @@
                     # não, salve-o
                     penultimate_list.append(last_elem)
 
             # substitue a lista original associada à penúltima chave com a nova lista coalescida
             curr_dict[key_chain[-2]] = penultimate_list
 
 
-def dict_reduce(target: dict, key_chain: list[str]):
+def dict_reduce(target: dict, key_chain: list[str]) -> None:
     """
     Realoca os elementos de *target* no nível *n*, para o nível imediatamente acima.
 
     Esses elementos são apontados pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*.
     O elemento no nivel *n* é removido, ao final.
 
     :param target: o dicionário a ser reduzido
@@ -607,26 +607,26 @@
 
             # atribui o valor transformado ao resultado
             dict_set_value(result, to_keys_deep, to_value)
 
     return result
 
 
-def dict_listify(target: dict, key_chain: list[str]):
+def dict_listify(target: dict, key_chain: list[str]) -> None:
     """
     Insere o valor do item de *target* apontado pela cadeia de chaves *[keys[0]: ... :keys[n]* em uma lista.
 
     Essa inserção ocorrerá apenas se esse valor já não for uma lista.
     Todas as listas eventualmente encontradas no percurso até a penúltima chava
     da cadeia serão recursivamente processadas.
 
     :param target: dicionário a ser modificado
     :param key_chain: cadeia de chaves aninhadas apontando para o item em questão
     """
-    def items_listify(in_targets: list, in_keys: list[str]):
+    def items_listify(in_targets: list, in_keys: list[str]) -> None:
 
         # percorra os itens da lista
         for in_target in in_targets:
             # o elemento é um dicionário ?
             if isinstance(in_target, dict):
                 # sim, processe-o
                 dict_listify(in_target, in_keys)
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/email_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/email_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 EMAIL_ACCOUNT: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_ACCOUNT")
 EMAIL_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_PWD")
 EMAIL_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_EMAIL_PORT")
 EMAIL_SERVER: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_SERVER")
 
 
-def email_send(errors: list[str], user_email: str, subject: str, content: str):
+def email_send(errors: list[str], user_email: str, subject: str, content: str) -> None:
     """
     Send email, to *user_email", with *subject* as the email subject, and *content* as the email message.
 
     :param errors: incidental error messages
     :param user_email: the address to send the email to
     :param subject: the email subject
     :param content: the email message
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/env_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/file_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/http_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/http_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/json_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/json_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 from collections.abc import Iterable
 
 
-def json_normalize_dict(source: dict):
+def json_normalize_dict(source: dict) -> None:
     """
     Turn the values in *source* into values that can be serialized to JSON, avoiding *TypeError*.
 
     Possible transformations:
         - *bytes* e *bytearray* are changed to *str* in *Base64* format
         - *Iterable* is changed into a *list*
         - all other types kept as they are
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/list_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/logging_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,17 +124,16 @@
                         result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
 def logging_log_msgs(msgs: list[str], output_dev: TextIO = None,
-                     log_level: Literal["debug", "info", "warning",
-                                        "error", "critical"] = "error",
-                     logger: logging.Logger = PYPOMES_LOGGER):
+                     log_level: Literal["debug", "info", "warning", "error", "critical"] = "error",
+                     logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write all messages in *msgs* to *PYPOMES_LOGGER*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* ou *sys.stderr*.
 
     :param msgs: the messages list
     :param output_dev: output device where the message is to be printed (None for no device printing)
```

### Comparing `pypomes_core-0.2.1/src/pypomes_core/str_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.2.2/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/LICENSE` & `pypomes_core-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.1/pyproject.toml` & `pypomes_core-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.2.1/PKG-INFO` & `pypomes_core-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

