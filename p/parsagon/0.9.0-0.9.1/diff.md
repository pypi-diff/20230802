# Comparing `tmp/parsagon-0.9.0.tar.gz` & `tmp/parsagon-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.9.0.tar", last modified: Sun Jul 30 03:09:47 2023, max compression
+gzip compressed data, was "parsagon-0.9.1.tar", last modified: Wed Aug  2 17:54:10 2023, max compression
```

## Comparing `parsagon-0.9.0.tar` & `parsagon-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.528297 parsagon-0.9.0/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-30 03:09:47.527944 parsagon-0.9.0/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.0/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-30 03:09:01.000000 parsagon-0.9.0/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-30 03:09:47.528396 parsagon-0.9.0/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.515199 parsagon-0.9.0/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.0/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.519436 parsagon-0.9.0/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4660 2023-07-30 02:20:05.000000 parsagon-0.9.0/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.0/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    12172 2023-07-30 02:56:40.000000 parsagon-0.9.0/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.9.0/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.0/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.527061 parsagon-0.9.0/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.0/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.0/src/parsagon/tests/test_executor.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.0/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-30 03:09:47.522699 parsagon-0.9.0/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      682 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-30 03:09:47.000000 parsagon-0.9.0/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.662508 parsagon-0.9.1/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 17:54:10.662121 parsagon-0.9.1/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.1/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1048 2023-08-02 09:54:56.000000 parsagon-0.9.1/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-02 17:54:10.662627 parsagon-0.9.1/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.642804 parsagon-0.9.1/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.1/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.650359 parsagon-0.9.1/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     5590 2023-08-02 06:48:17.000000 parsagon-0.9.1/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.1/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    15535 2023-08-02 10:33:44.000000 parsagon-0.9.1/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     9218 2023-08-02 10:12:43.000000 parsagon-0.9.1/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.1/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.661292 parsagon-0.9.1/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.1/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.1/src/parsagon/tests/test_executor.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.656357 parsagon-0.9.1/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      682 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.9.0/PKG-INFO` & `parsagon-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.0
+Version: 0.9.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.0/README.md` & `parsagon-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/pyproject.toml` & `parsagon-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.9.0"
+version = "0.9.1"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.9.0/src/parsagon/api.py` & `parsagon-0.9.1/src/parsagon/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,25 +76,54 @@
         httpx.post,
         "/transformers/get-nav-elem/",
         json={"html": marked_html, "elem_type": elem_type, "description": description},
     )["id"]
     return result
 
 
+def get_schema_fields(schema):
+    """
+    Gets fields and their types from a given schema
+    :param schema:
+    :return: A dict mapping fields to thir types
+    """
+    return _api_call(httpx.post, "/transformers/get-schema-fields/", json={"schema": schema})
+
+
+def get_cleaned_data(html, schema, nodes):
+    """
+    Gets cleaned data from the nodes to be scraped.
+    :param html: HTML of the page to scrape
+    :param schema: Schema of the data to scrape
+    :param nodes: Nodes to scrape
+    :return: Cleaned data
+    """
+    return _api_call(httpx.post, "/transformers/get-cleaned-data/", json={"html": html, "schema": schema, "nodes": nodes})
+
+
 def scrape_page(html, schema):
     """
     Scrapes data from the provided page HTML - data will be returned in the schema provided.
     :param url: url of the page to scrape.
     :param html: HTML of the page to scrape.
     :param schema: Schema of the data to scrape
-    :return: Scraped data, with lists truncated.
+    :return: Scraped data
     """
     return _api_call(httpx.post, "/transformers/get-custom-data/", json={"html": html, "schema": schema})
 
 
+def ask_about_data(data, question):
+    """
+    Asks GPT a question about the given data.
+    :param data: the data to give GPT
+    :param question: the question to ask about the data
+    """
+    return _api_call(httpx.post, "transformers/ask-about-data/", json={"data": data, "question": question})
+
+
 def create_pipeline(name, description, program_sketch):
     return _api_call(
         httpx.post, "/pipelines/", json={"name": name, "description": description, "program_sketch": program_sketch}
     )
 
 
 def delete_pipeline(pipeline_id):
```

### Comparing `parsagon-0.9.0/src/parsagon/custom_function.py` & `parsagon-0.9.1/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/exceptions.py` & `parsagon-0.9.1/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/executor.py` & `parsagon-0.9.1/src/parsagon/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import logging
+from pathlib import Path
 import time
 from urllib.parse import urljoin
 
 import lxml.html
 from pyvirtualdisplay import Display
 from selenium import webdriver
 import seleniumwire.undetected_chromedriver as uc
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.select import Select
 
-from parsagon.api import get_interaction_element_id, scrape_page
+from parsagon.api import get_interaction_element_id, get_schema_fields, get_cleaned_data, scrape_page
 from parsagon.custom_function import CustomFunction
 from parsagon.exceptions import ParsagonException
 
 logger = logging.getLogger(__name__)
 
 
 # A dictionary of custom function names to their descriptions for the user
@@ -25,20 +26,30 @@
     "goto": "go to a page",
     "click_elem": "click an element",
     "fill_input": "fill an input",
     "select_option": "select an option",
 }
 
 
+# A dict of schema types to element types
+ELEMENT_TYPES = {
+    "str": "TEXT",
+    "num": "TEXT",
+    "link": "URL",
+    "image": "IMAGE",
+    "element": "ACTION",
+}
+
+
 class Executor:
     """
     Executes code produced by GPT with the proper context.  Records custom_function usage along the way.
     """
 
-    def __init__(self, headless=False):
+    def __init__(self, headless=False, infer=False):
         self.headless = headless
         if self.headless:
             self.display = Display(visible=False, size=(1280, 1050)).start()
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument("--start-maximized")
         seleniumwire_options = {"disable_capture": True}
         self.driver = uc.Chrome(options=chrome_options, seleniumwire_options=seleniumwire_options)
@@ -51,21 +62,38 @@
             "select_option": self.select_option,
             "scroll": self.scroll,
             "wait": self.wait,
             "scrape_data": self.scrape_data,
         }
         logger.debug("Available functions: %s", ", ".join(self.execution_context.keys()))
         self.custom_functions = {}
+        self.infer = infer
+
+        highlights_path = Path(__file__).parent / "highlights.js"
+        with highlights_path.open() as f:
+            self.highlights_script = f.read()
 
     def add_custom_function(self, call_id, custom_function):
         if call_id in self.custom_functions:
             self.custom_functions[call_id].examples.extend(custom_function.examples)
         else:
             self.custom_functions[call_id] = custom_function
 
+    def inject_highlights_script(self):
+        self.driver.execute_script(self.highlights_script);
+
+    def highlights_setup(self, field_type, max_examples="null"):
+        self.driver.execute_script(f"window.currentFieldType = '{field_type}'; window.maxExamples = {max_examples};");
+
+    def highlights_cleanup(self):
+        self.driver.execute_script(f"window.currentFieldType = null; window.maxExamples = null; window.clearCSS();");
+
+    def get_selected_node_ids(self):
+        return self.driver.execute_script("return Array.from(document.getElementsByClassName('parsagon-io-example-stored')).map((elem) => elem.getAttribute('data-psgn-id'))");
+
     def mark_html(self):
         """
         Adds node IDs to elements on the current page that don't already have IDs.
         """
         logger.debug("  Marking HTML...")
         self.max_elem_id = self.driver.execute_script(
             "let elemIdx = 0; for (const node of document.all) { node.setAttribute('data-psgn-id', elemIdx); elemIdx++; } return elemIdx;"
@@ -131,33 +159,50 @@
             if not selenium_elem.is_displayed():
                 parent = lxml_elem.getparent()
                 if parent is not None:
                     parent.remove(lxml_elem)
 
         return lxml.html.tostring(root).decode()
 
-    def get_elem_by_description(self, elem_type, description):
+    def get_elem(self, description, elem_type):
+        if self.infer:
+            return self.get_elem_by_description(description, elem_type)
+        self.highlights_setup("ACTION", max_examples=1)
+        user_input = input(f'Click the element referred to by "{description}". Hit ENTER to confirm your selection, or type "INFER" to let Parsagon infer the element: ')
+        selected_node_ids = self.get_selected_node_ids()
+        while user_input != "INFER" and not selected_node_ids:
+            user_input = input('Please click an element or type "INFER": ')
+            selected_node_ids = self.get_selected_node_ids()
+        self.highlights_cleanup()
+        if user_input == "INFER":
+            return self.get_elem_by_description(description, elem_type)
+        else:
+            elem_id = selected_node_ids[0]
+            elem = self._id_to_elem(elem_id)
+        return elem, elem_id
+
+    def get_elem_by_description(self, description, elem_type):
         logger.info(f'Looking for {elem_type.lower()}: "{description}"')
         visible_html = self.get_visible_html()
         elem_id = get_interaction_element_id(visible_html, elem_type, description)
         if elem_id is None:
             raise ParsagonException(
                 f'Could not find an element matching "{description}". Perhaps try rephrasing your prompt.'
             )
-        return elem_id
+        elem = self._id_to_elem(elem_id)
+        log_suffix = f' with text "{elem.text}"' if elem.text else ""
+        logger.info(f"Found element" + log_suffix)
+        return elem, elem_id
 
-    def _get_elem(self, elem_id):
+    def _id_to_elem(self, elem_id):
         """
         Gets a selenium element by Parsagon ID (psgn-id).
         """
         assert elem_id is not None
         result = self.driver.find_element(By.XPATH, f'//*[@data-psgn-id="{elem_id}"]')
-        elem_text = result.text
-        log_suffix = f' with text "{elem_text}"' if elem_text else ""
-        logger.info(f"Found element" + log_suffix)
         return result
 
     def custom_assert(self, v):
         assert v, "Web page interaction failed."
 
     def goto(self, url, window_id=None):
         if window_id in self.driver.window_handles:
@@ -166,38 +211,40 @@
             self.driver.switch_to.new_window("tab")
 
         # Go to website
         logger.info(f"Going to {url}")
         self.driver.get(url)
 
         # Wait for website to load
-        time.sleep(5)
+        time.sleep(2)
         self.mark_html()
+        self.inject_highlights_script()
 
         return self.driver.current_window_handle
 
     def click_elem(self, description, window_id, call_id):
         """
         Clicks a button.
         """
-        html = self.get_scrape_html()
-        elem_id = self.get_elem_by_description("BUTTON", description)
         self.driver.switch_to.window(window_id)
-        elem = self._get_elem(elem_id)
+        elem, elem_id = self.get_elem(description, "BUTTON")
+        html = self.get_scrape_html()
+
         for i in range(3):
             try:
                 elem.click()
                 logger.info("Clicked element")
-                time.sleep(5)
+                time.sleep(2)
                 break
             except Exception as e:
-                time.sleep(5)
+                time.sleep(2)
         else:
             return False
         self.mark_html()
+        self.inject_highlights_script()
         custom_function = CustomFunction(
             "click_elem",
             arguments={},
             examples=[
                 {
                     "html": html,
                     "url": self.driver.current_url,
@@ -208,29 +255,31 @@
         self.add_custom_function(call_id, custom_function)
         return True
 
     def select_option(self, description, option, window_id, call_id):
         """
         Selects an option by name from a dropdown.
         """
+        self.driver.switch_to.window(window_id)
+        elem, elem_id = self.get_elem(description, "SELECT")
         html = self.get_scrape_html()
-        elem_id = self.get_elem_by_description("SELECT", description)
-        elem = self._get_elem(elem_id)
+
         for i in range(3):
             try:
                 select_obj = Select(elem)
                 select_obj.select_by_visible_text(option)
                 logger.info(f'Selected option "{option}"')
-                time.sleep(5)
+                time.sleep(2)
                 break
             except:
-                time.sleep(5)
+                time.sleep(2)
         else:
             return False
         self.mark_html()
+        self.inject_highlights_script()
         custom_function = CustomFunction(
             "select_option",
             arguments={
                 "option": option,
             },
             examples=[
                 {
@@ -243,32 +292,34 @@
         self.add_custom_function(call_id, custom_function)
         return True
 
     def fill_input(self, description, text, enter, window_id, call_id):
         """
         Fills an input text field, then presses an optional end key.
         """
+        self.driver.switch_to.window(window_id)
+        elem, elem_id = self.get_elem(description, "INPUT")
         html = self.get_scrape_html()
-        elem_id = self.get_elem_by_description("INPUT", description)
-        elem = self._get_elem(elem_id)
+
         for i in range(3):
             try:
                 elem.clear()
                 elem.send_keys(text)
                 logger.info(f'Typed "{text}" into element')
                 if enter:
                     elem.send_keys(Keys.RETURN)
                     logger.debug("Pressed enter")
-                time.sleep(5)
+                time.sleep(2)
                 break
             except:
-                time.sleep(5)
+                time.sleep(2)
         else:
             return False
         self.mark_html()
+        self.inject_highlights_script()
         custom_function = CustomFunction(
             "fill_input",
             arguments={
                 "text": text,
                 "enter": enter,
             },
             examples=[
@@ -290,50 +341,72 @@
         )
         time.sleep(1)
 
     def wait(self, seconds):
         logger.info(f"Waiting {seconds} seconds...")
         time.sleep(seconds)
         self.mark_html()
+        self.inject_highlights_script()
 
     def scrape_data(self, schema, window_id, call_id):
         """
         Scrapes data from the current page.
         """
         self.driver.switch_to.window(window_id)
-        logger.info("Scraping data...")
         html = self.get_scrape_html()
-        result = scrape_page(html, schema)
-        scraped_data = result["data"]
-        nodes = result["nodes"]
-        if not scraped_data and not nodes:
-            raise ParsagonException(
-                f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt."
-            )
-        elif not nodes:
-            raise ParsagonException(
-                f"Parsagon found the following data on the page for the format {schema}:\n\n{scraped_data}\n\nHowever, it could not find a plausible program to scrape this data. If the data above is incorrect, perhaps try rephrasing your prompt."
-            )
+
+        if self.infer:
+            user_input = "INFER"
+        else:
+            user_input = input(f'Now determining what elements to scrape to collect data in the format {schema}. Hit ENTER to continue by clicking on the elements to scrape, or type "INFER" to let Parsagon infer the elements: ')
+            while user_input not in ("", "INFER"):
+                user_input = input('Hit ENTER or type "INFER": ')
+        if user_input == "":
+            nodes = {}
+            field_types = get_schema_fields(schema)
+            for field, field_type in field_types.items():
+                self.highlights_setup(ELEMENT_TYPES[field_type])
+                field_repr = field.replace("dataset0|", "").replace("|", " / ")
+                input(f"Click elements containing data for the field `{field_repr}`. Hit TAB to autocomplete or DELETE/BACKSPACE to clear selections. Hit ENTER when done: ")
+                nodes[field] = [[node_id] for node_id in self.get_selected_node_ids()]
+                self.highlights_cleanup()
+            logger.info("Scraping data...")
+            result = get_cleaned_data(html, schema, nodes)
+            scraped_data = result["data"]
+        else:
+            logger.info("Scraping data...")
+            result = scrape_page(html, schema)
+            scraped_data = result["data"]
+            nodes = result["nodes"]
+            if not scraped_data and not nodes:
+                raise ParsagonException(
+                    f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt."
+                )
+            elif not nodes:
+                raise ParsagonException(
+                    f"Parsagon found the following data on the page for the format {schema}:\n\n{scraped_data}\n\nHowever, it could not find a plausible program to scrape this data. If the data above is incorrect, perhaps try rephrasing your prompt."
+                )
         logger.info(f"Scraped data:\n{scraped_data}")
+
         custom_function = CustomFunction(
             "scrape_data",
             arguments={
                 "schema": schema,
             },
             examples=[
                 {
-                    "html": self.get_scrape_html(),
+                    "html": html,
                     "url": self.driver.current_url,
                     "nodes": nodes,
                     "scraped_data": scraped_data,
                 }
             ],
         )
         self.add_custom_function(call_id, custom_function)
-        return result["data"]
+        return scraped_data
 
     def execute(self, code):
         try:
             exec(code, self.execution_context)
         finally:
             self.driver.quit()
             if self.headless:
```

### Comparing `parsagon-0.9.0/src/parsagon/main.py` & `parsagon-0.9.1/src/parsagon/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         help="the name of the program to create",
     )
     parser_create.add_argument(
         "--headless",
         action="store_true",
         help="run the browser in headless mode",
     )
+    parser_create.add_argument(
+        "--infer",
+        action="store_true",
+        help="let Parsagon infer all elements to be scraped",
+    )
     parser_create.set_defaults(func=create)
 
     # Detail
     parser_detail = subparsers.add_parser(
         "detail",
         description="Outputs details of a created program.",
     )
@@ -138,15 +143,15 @@
         except ParsagonException as e:
             error_message = "Error:\n" + e.to_string(verbose)
             logger.error(error_message)
     else:
         parser.print_help()
 
 
-def create(task=None, program_name=None, headless=False, verbose=False):
+def create(task=None, program_name=None, headless=False, infer=False, verbose=False):
     if task:
         logger.info("Launched with task description:\n%s", task)
     else:
         task = input("Type what you want to do: ")
 
     logger.info("Analyzing task description...")
     program_sketches = get_program_sketches(task)
@@ -154,15 +159,15 @@
 
     full_program = program_sketches["full"]
     abridged_program = program_sketches["abridged"]
     logger.debug("Program:\n%s", abridged_program)
     abridged_program += "\n\noutput = func()\nprint(f'Program finished and returned a value of:\\n{output}\\n')\n"  # Make the program runnable
 
     # Execute the abridged program to gather examples
-    executor = Executor(headless=headless)
+    executor = Executor(headless=headless, infer=infer)
     executor.execute(abridged_program)
 
     # The user must select a name
     while True:
         if not program_name:
             program_name = input("Name this program to save, or press enter without typing a name to DISCARD: ")
         if program_name:
```

### Comparing `parsagon-0.9.0/src/parsagon/settings.py` & `parsagon-0.9.1/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/tests/api_mocks.py` & `parsagon-0.9.1/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/tests/test_executor.py` & `parsagon-0.9.1/src/parsagon/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.9.1/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.9.1/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.0/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.9.1/src/parsagon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.0
+Version: 0.9.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.0/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.9.1/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

