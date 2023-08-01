# Comparing `tmp/carbonate_sdk-0.0.4.tar.gz` & `tmp/carbonate_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbonate_sdk-0.0.4.tar", max compression
+gzip compressed data, was "carbonate_sdk-0.0.5.tar", max compression
```

## Comparing `carbonate_sdk-0.0.4.tar` & `carbonate_sdk-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1062 2023-04-18 21:56:37.365649 carbonate_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0      645 2023-06-23 22:28:21.904477 carbonate_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      186 2023-04-29 15:56:35.860367 carbonate_sdk-0.0.4/carbonate_sdk/__init__.py
--rw-r--r--   0        0        0       96 2023-04-29 12:31:00.085631 carbonate_sdk-0.0.4/carbonate_sdk/action.py
--rw-r--r--   0        0        0     2908 2023-07-15 00:33:24.404953 carbonate_sdk-0.0.4/carbonate_sdk/api.py
--rw-r--r--   0        0        0      562 2023-06-17 20:33:05.653408 carbonate_sdk-0.0.4/carbonate_sdk/browser.py
--rw-r--r--   0        0        0      323 2023-04-30 18:29:14.697082 carbonate_sdk-0.0.4/carbonate_sdk/exceptions.py
--rw-r--r--   0        0        0      706 2023-04-29 12:31:00.087897 carbonate_sdk-0.0.4/carbonate_sdk/logger.py
--rw-r--r--   0        0        0        0 2023-04-29 12:31:00.103531 carbonate_sdk-0.0.4/carbonate_sdk/resources/__init__.py
--rw-r--r--   0        0        0     7169 2023-06-17 20:32:03.250275 carbonate_sdk-0.0.4/carbonate_sdk/resources/carbonate.js
--rw-r--r--   0        0        0    10460 2023-07-15 00:35:36.615141 carbonate_sdk-0.0.4/carbonate_sdk/sdk.py
--rw-r--r--   0        0        0      150 2023-05-11 17:42:17.036886 carbonate_sdk-0.0.4/carbonate_sdk/slugify.py
--rw-r--r--   0        0        0      924 2023-06-23 23:07:10.021123 carbonate_sdk-0.0.4/carbonate_sdk/test_decorator.py
--rw-r--r--   0        0        0     2262 2023-04-30 18:24:27.700523 carbonate_sdk-0.0.4/carbonate_sdk/test_logger.py
--rw-r--r--   0        0        0     3071 2023-06-23 23:47:31.787585 carbonate_sdk-0.0.4/carbonate_sdk/webdriver.py
--rw-r--r--   0        0        0      546 2023-07-15 22:31:28.529774 carbonate_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 carbonate_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-18 21:56:37.365649 carbonate_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0      645 2023-08-01 23:32:20.038242 carbonate_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      186 2023-04-29 15:56:35.860367 carbonate_sdk-0.0.5/carbonate_sdk/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-29 12:31:00.085631 carbonate_sdk-0.0.5/carbonate_sdk/action.py
+-rw-r--r--   0        0        0     2931 2023-08-01 23:32:20.039662 carbonate_sdk-0.0.5/carbonate_sdk/api.py
+-rw-r--r--   0        0        0      562 2023-06-17 20:33:05.653408 carbonate_sdk-0.0.5/carbonate_sdk/browser.py
+-rw-r--r--   0        0        0      375 2023-08-01 23:32:20.041945 carbonate_sdk-0.0.5/carbonate_sdk/exceptions.py
+-rw-r--r--   0        0        0      706 2023-04-29 12:31:00.087897 carbonate_sdk-0.0.5/carbonate_sdk/logger.py
+-rw-r--r--   0        0        0        0 2023-04-29 12:31:00.103531 carbonate_sdk-0.0.5/carbonate_sdk/resources/__init__.py
+-rw-r--r--   0        0        0     7169 2023-06-17 20:32:03.250275 carbonate_sdk-0.0.5/carbonate_sdk/resources/carbonate.js
+-rw-r--r--   0        0        0    11045 2023-08-01 23:32:20.042698 carbonate_sdk-0.0.5/carbonate_sdk/sdk.py
+-rw-r--r--   0        0        0      150 2023-05-11 17:42:17.036886 carbonate_sdk-0.0.5/carbonate_sdk/slugify.py
+-rw-r--r--   0        0        0      924 2023-06-23 23:07:10.021123 carbonate_sdk-0.0.5/carbonate_sdk/test_decorator.py
+-rw-r--r--   0        0        0     2264 2023-08-01 23:32:20.043302 carbonate_sdk-0.0.5/carbonate_sdk/test_logger.py
+-rw-r--r--   0        0        0     3265 2023-08-01 23:32:20.043890 carbonate_sdk-0.0.5/carbonate_sdk/webdriver.py
+-rw-r--r--   0        0        0      597 2023-08-01 23:32:20.124097 carbonate_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 carbonate_sdk-0.0.5/PKG-INFO
```

### Comparing `carbonate_sdk-0.0.4/LICENSE` & `carbonate_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carbonate_sdk-0.0.4/README.md` & `carbonate_sdk-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 Carbonate turns simple language driven instructions into end-to-end tests. This SDK lets you integrate it directly into your test suite.
 
 Learn more about Carbonate at [https://carbonate.dev](https://carbonate.dev).
 
 ## Getting Started
 
-Check out the [getting started guide](https://docs.carbonate.dev/sdk/getting-started/python) for instructions on how to integrate Carbonate into your test suite.
+Check out the [getting started guide](https://carbonate.dev/docs/sdk/getting-started/python) for instructions on how to integrate Carbonate into your test suite.
 
 ## License
 Distributed under the MIT License.
```

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/api.py` & `carbonate_sdk-0.0.5/carbonate_sdk/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
-from typing import Optional
+from typing import Optional, Union
 from requests import Session, RequestException
 
 from .exceptions import ApiException
 
 class Api:
     def __init__(
         self,
         api_user_id: Optional[str] = None,
         api_key: Optional[str] = None,
         api_url: Optional[str] = None,
-    ):
+    ) -> None:
         self.test_name = None
         self.api_user_id = api_user_id or os.environ.get("CARBONATE_USER_ID")
         self.api_key = api_key or os.environ.get("CARBONATE_API_KEY")
         self.api_url = api_url or "https://api.carbonate.dev/"
         self.client = Session()
 
         if not self.api_user_id:
@@ -23,15 +23,15 @@
             )
 
         if not self.api_key:
             raise ValueError(
                 "No API key provided, please either pass in api_key to the constructor or set the CARBONATE_API_KEY environment variable"
             )
 
-    def set_test(self, test):
+    def set_test(self, test) -> None:
         self.test_name = test
 
     def call_api(self, url: str, data: dict):
         if not data['test_name']:
             raise ValueError(
                 "No test name provided, please use the @carbonate.test() annotation or call start_test() with your test name"
             )
```

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/browser.py` & `carbonate_sdk-0.0.5/carbonate_sdk/browser.py`

 * *Files identical despite different names*

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/logger.py` & `carbonate_sdk-0.0.5/carbonate_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/resources/carbonate.js` & `carbonate_sdk-0.0.5/carbonate_sdk/resources/carbonate.js`

 * *Files identical despite different names*

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/sdk.py` & `carbonate_sdk-0.0.5/carbonate_sdk/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 import os
 import json
-from distutils.util import strtobool
 from time import sleep
-from typing import List, Callable, Optional, IO
+from typing import List, Callable, Optional, IO, Union, Any, Dict
 from .browser import Browser
 from .api import Api
-from .exceptions import FailedExtractionException, InvalidXpathException, BrowserException, TestException
+from .exceptions import FailedExtractionException, InvalidXpathException, BrowserException, TestException, \
+    LogicException
 from .logger import Logger
 from .slugify import slugify
 from .test_logger import TestLogger
-import logging as python_logging
 
 class SDK:
     def __init__(
             self,
             browser: Browser,
-            cache_dir: str = None,
-            api_user_id: str = None,
-            api_key: str = None,
+            cache_dir: Optional[str] = None,
+            api_user_id: Optional[str] = None,
+            api_key: Optional[str] = None,
             logging = None,
             client: Optional[Api] = None,
-    ):
+    ) -> None:
         self.browser = browser
         self.client = client or Api(api_user_id, api_key)
-        self.test_prefix = None
-        self.test_name = None
+        self.test_prefix: Optional[str] = None
+        self.test_name: Optional[str] = None
         self.cache_dir = cache_dir or os.environ.get('CARBONATE_CACHE_DIR')
-        self.network_whitelist = []
-        self.instruction_cache = {}
+        self.network_whitelist: List[str] = []
+        self.instruction_cache: Dict[str, Any] = {}
 
         # Log to exception - default
         if logging is None:
             self.logger = TestLogger()
         # Path to file or IO object
         elif isinstance(logging, str) or isinstance(logging, IO):
             self.logger = TestLogger(logging, False)
         # Custom logger
         else:
             self.logger = logging
 
-    def get_test_name(self):
+    def get_test_name(self) -> str:
+        if self.test_name is None:
+            raise LogicException("Test name not set, please call start_test first")
+
         if self.test_prefix:
             return self.test_prefix + ': ' + self.test_name
 
         return self.test_name
 
-    def wait_for_load(self, skip_func: Callable):
+    def wait_for_load(self, skip_func: Callable) -> None:
         i = 0
 
         while self.browser.evaluate_script('return window.carbonate_dom_updating') or self.browser.evaluate_script('return window.carbonate_active_xhr'):
             if skip_func():
                 self.logger.info("Found cached element, skipping DOM wait")
                 break
 
@@ -60,48 +62,51 @@
 
             if i > 20:
                 raise BrowserException("Waited too long for DOM/XHR update to finish")
 
             sleep(0.5)
             i += 1
 
-    def get_cache_path(self, instruction):
+    def get_cache_path(self, instruction) -> str:
+        if self.cache_dir is None:
+            raise LogicException("No cache dir set")
+
         return self.cache_dir + '/' + slugify(self.test_name) + '/' + slugify(instruction) + '.json'
 
-    def cached_actions(self, instruction):
+    def cached_actions(self, instruction) -> List[dict]:
         if self.cache_dir is not None and os.path.isfile(self.get_cache_path(instruction)):
             # Open the file as parse the json
             with open(self.get_cache_path(instruction), 'r') as f:
                 actions = json.load(f)
                 self.logger.debug("Using locally cached actions", {'actions': actions})
                 return actions
 
         return []
 
-    def extract_actions(self, instruction):
+    def extract_actions(self, instruction) -> List[dict]:
         actions = self.client.extract_actions(self.get_test_name(), instruction, self.browser.get_html())
 
         if len(actions) > 0:
             self.logger.info("Successfully extracted actions", {'actions': actions})
             self.cache_instruction(actions, instruction)
 
             return actions
 
         raise FailedExtractionException('Could not extract actions')
 
-    def cache_instruction(self, result, instruction):
+    def cache_instruction(self, result: Union[List[dict], dict], instruction: str) -> None:
         if self.cache_dir is not None:
             self.instruction_cache[instruction] = result
 
     def write_cache(self) -> None:
         if self.cache_dir is None:
-            raise Exception("Cannot call write_cache without setting cache_dir")
+            raise LogicException("Cannot call write_cache without setting cache_dir")
 
         if self.test_name is None:
-            raise Exception("Test name not set, please call start_Test first")
+            raise LogicException("Test name not set, please call start_test first")
 
         if len(self.instruction_cache) == 0:
             return
 
         # Create the cache directory if it doesn't exist
         if not os.path.exists(self.cache_dir):
             os.makedirs(self.cache_dir)
@@ -111,52 +116,52 @@
             os.makedirs(self.cache_dir + '/' + slugify(self.test_name))
 
         for instruction, result in self.instruction_cache.items():
             # Write the actions to a file
             with open(self.get_cache_path(instruction), 'w') as f:
                 json.dump(result, f)
 
-        self.instruction_cache = []
+        self.instruction_cache = {}
 
-    def cached_assertions(self, instruction):
+    def cached_assertions(self, instruction: str) -> List[dict]:
         if self.cache_dir is not None and os.path.isfile(self.get_cache_path(instruction)):
             # Open the file as parse the json
             with open(self.get_cache_path(instruction), 'r') as f:
                 actions = json.load(f)
                 self.logger.debug("Using locally cached assertions", {'actions': actions})
                 return actions
 
         return []
 
-    def extract_assertions(self, instruction):
+    def extract_assertions(self, instruction: str) -> List[dict]:
         assertions = self.client.extract_assertions(self.get_test_name(), instruction, self.browser.get_html())
 
         if len(assertions) > 0:
             self.logger.info("Successfully extracted assertions", {'assertions': assertions})
             self.cache_instruction(assertions, instruction)
 
             return assertions
 
         raise FailedExtractionException('Could not extract assertions')
 
-    def action(self, instruction):
+    def action(self, instruction: str):
         self.logger.info("Querying action", {'test_name': self.get_test_name(), 'instruction': instruction})
         actions = self.cached_actions(instruction)
 
         is_action_ready = lambda action: len(self.browser.find_by_xpath(action['xpath'])) > 0
         self.wait_for_load(lambda: len(actions) > 0 and all(map(is_action_ready, actions)))
 
         if len(actions) == 0:
             self.logger.notice("No actions found, extracting from page")
             actions = self.extract_actions(instruction)
 
         self.perform_actions(actions)
 
-    def perform_actions(self, actions):
-        previous_actions = []
+    def perform_actions(self, actions: List[dict]) -> List[dict]:
+        previous_actions: List[dict] = []
         for action in actions:
             self.logger.notice("Performing action", {'action': action})
             elements = self.browser.find_by_xpath(action['xpath'])
 
             if len(elements) == 0:
                 raise InvalidXpathException("Could not find element for xpath: " + action['xpath'])
 
@@ -168,70 +173,70 @@
                 return previous_actions
 
             self.browser.perform_action(action, elements)
             previous_actions.append(action)
 
         return previous_actions
 
-    def assertion(self, instruction):
+    def assertion(self, instruction: str):
         self.logger.info("Querying assertion", {'test_name': self.get_test_name(), 'instruction': instruction})
 
         assertions = self.cached_assertions(instruction)
 
         self.wait_for_load(lambda: len(assertions) > 0 and all(map(self.is_assertion_ready, assertions)))
 
         if len(assertions) == 0:
             self.logger.notice("No assertions found, extracting from page")
             assertions = self.extract_assertions(instruction)
 
         return self.perform_assertions(assertions)
 
-    def perform_assertions(self, assertions: List) -> bool:
+    def perform_assertions(self, assertions: List[dict]) -> bool:
         for assertion in assertions:
             result = self.perform_assertion(assertion)
 
             if not result:
                 return False
 
         return True
 
-    def is_assertion_ready(self, assertion):
+    def is_assertion_ready(self, assertion: dict) -> bool:
         try:
             self.perform_assertion(assertion)
             return True
         except BrowserException as e:
             return False
 
-    def perform_assertion(self, assertion):
+    def perform_assertion(self, assertion: dict) -> bool:
         self.logger.notice("Performing assertion", {'assertion': assertion['assertion']})
 
         return self.browser.evaluate_script('window.carbonate_reset_assertion_result(); (function() { ' + assertion['assertion'] + ' })(); return window.carbonate_assertion_result;')
 
-    def cached_lookup(self, instruction):
+    def cached_lookup(self, instruction: str) -> Optional[dict]:
         if self.cache_dir is not None and os.path.isfile(self.get_cache_path(instruction)):
             # Open the file as parse the json
             with open(self.get_cache_path(instruction), 'r') as f:
                 lookup = json.load(f)
                 self.logger.debug("Using locally cached lookup", {'lookup': lookup})
                 return lookup
 
         return None
 
-    def extract_lookup(self, instruction):
+    def extract_lookup(self, instruction: str) -> dict:
         lookup = self.client.extract_lookup(self.get_test_name(), instruction, self.browser.get_html())
 
         if lookup is not None:
             self.logger.info("Successfully extracted lookup", {'lookup': lookup})
             self.cache_instruction(lookup, instruction)
 
             return lookup
 
         raise FailedExtractionException('Could not extract lookup')
 
-    def lookup(self, instruction):
+    def lookup(self, instruction: str):
         self.logger.info("Querying lookup", {'test_name': self.get_test_name(), 'instruction': instruction})
         element = self.cached_lookup(instruction)
 
         self.wait_for_load(lambda: element is not None and len(self.browser.find_by_xpath(element['xpath'])) > 0)
 
         if element is None:
             self.logger.notice("No elements found, extracting from page")
@@ -240,41 +245,41 @@
         elements = self.browser.find_by_xpath(element['xpath'])
 
         if len(elements) == 0:
             raise InvalidXpathException("Could not find element for xpath: " + element['xpath'])
 
         return elements[0]
 
-    def start_test(self, test_prefix, test_name):
+    def start_test(self, test_prefix: str, test_name: str) -> None:
         if len(self.instruction_cache.keys()) > 0:
-            raise Exception("Instruction cache not empty, did you forget to call end_test()?")
+            raise LogicException("Instruction cache not empty, did you forget to call end_test()?")
 
         if hasattr(self.logger, 'clear_logs'):
             self.logger.clear_logs()
 
         self.test_prefix = test_prefix
         self.test_name = test_name
 
     def end_test(self):
         if self.cache_dir is not None:
             self.write_cache()
 
-    def load(self, url):
+    def load(self, url: str):
         self.logger.info("Loading page", {'url': url, 'whitelist': self.network_whitelist})
         self.browser.load(url, self.network_whitelist)
 
     def close(self):
         self.logger.info("Closing browser")
         self.browser.close()
 
-    def whitelist_network(self, url):
+    def whitelist_network(self, url: str):
         self.network_whitelist.append(url)
 
-    def handle_failed_test(self, e):
-        self.instruction_cache = []
+    def handle_failed_test(self, e: Exception) -> None:
+        self.instruction_cache = {}
 
         if hasattr(self.logger, 'get_logs'):
             raise TestException(self.logger.get_logs()) from e
 
         raise e
 
     def get_logger(self) -> Logger:
```

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/test_decorator.py` & `carbonate_sdk-0.0.5/carbonate_sdk/test_decorator.py`

 * *Files identical despite different names*

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/test_logger.py` & `carbonate_sdk-0.0.5/carbonate_sdk/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import Any, Dict, List, Optional
 from .logger import Logger
 
 class TestLogger(Logger):
-    def __init__(self, output_path = sys.stderr, buffer_logs = True):
+    def __init__(self, output_path=sys.stderr, buffer_logs: bool=True):
         if isinstance(output_path, str):
             output_path = open(output_path, 'w')
 
         self.output_file = output_path
         self.buffer_logs = buffer_logs
         self.logs: List[Dict[str, Any]] = []
```

### Comparing `carbonate_sdk-0.0.4/carbonate_sdk/webdriver.py` & `carbonate_sdk-0.0.5/carbonate_sdk/webdriver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import os
 import json
+from typing import Optional, List
+
 from selenium.common import ElementNotInteractableException
 from selenium.common.exceptions import JavascriptException
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By
 
 try:
     import importlib.resources as pkg_resources
     if not hasattr(pkg_resources, 'files'):
         raise ImportError
 except ImportError:
-    import importlib_resources as pkg_resources
+    import importlib_resources as pkg_resources # type: ignore
 
 from .browser import Browser
 from .action import Action
 from .exceptions import BrowserException
 
 class WebDriver(Browser):
-    def __init__(self, driver):
+    def __init__(self, driver) -> None:
         self.browser = driver
-        inject_js_resource = pkg_resources.files('carbonate_sdk.resources') / "carbonate.js"
+        inject_js_resource = pkg_resources.files('carbonate_sdk.resources') / "carbonate.js" # type: ignore[attr-defined]
         with inject_js_resource.open("r") as file:
             self.inject_js = file.read()
 
-    def get_html(self):
+    def get_html(self) -> str:
         return self.browser.execute_script("return document.documentElement.innerHTML")
 
-    def load(self, url, whitelist=None):
+    def load(self, url: str, whitelist: Optional[List[str]]=None) -> None:
         if self.evaluate_script('return typeof window.carbonate_dom_updating === "undefined"'):
             self.browser.execute_cdp_cmd('Page.addScriptToEvaluateOnNewDocument', {'source': self.inject_js})
 
         self.browser.get(url)
         self.evaluate_script('window.carbonate_set_xhr_whitelist(' + json.dumps(whitelist) + ')')
 
-    def close(self):
+    def close(self) -> None:
         self.browser.quit()
 
-    def find_by_xpath(self, xpath):
+    def find_by_xpath(self, xpath: str) -> list:
         return self.browser.find_elements(By.XPATH, xpath)
 
-    def find_by_id(self, id):
+    def find_by_id(self, id: str) -> list:
         return self.browser.find_elements(By.ID, id)
 
-    def evaluate_script(self, script):
+    def evaluate_script(self, script: str) -> str:
         try:
             return self.browser.execute_script(script)
         except JavascriptException as e:
             raise BrowserException("Could not evaluate script: " + script) from e
 
-    def perform_action(self, action, elements):
+    def perform_action(self, action: dict, elements: list) -> None:
         if action["action"] == Action.CLICK.value:
             try:
                 elements[0].click()
             except ElementNotInteractableException:
                 ActionChains(self.browser).move_to_element(elements[0]).click().perform()
 
         elif action["action"] == Action.TYPE.value:
```

### Comparing `carbonate_sdk-0.0.4/pyproject.toml` & `carbonate_sdk-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "carbonate-sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = "Run UI tests using AI"
 authors = ["Carbonate <team@cabonate.dev>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "carbonate_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.14"
 requests = "^2.28.2"
 importlib_resources = { version = "^5.12.0", python = "<3.9" }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 selenium = "^4.8.3"
-webdriver-manager = "^3.8.6"
+webdriver-manager = "^4.0.0"
 unittest-data-provider = "^1.0.1"
+mypy = "^1.4.1"
+types-requests = "^2.31.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `carbonate_sdk-0.0.4/PKG-INFO` & `carbonate_sdk-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbonate-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run UI tests using AI
 License: MIT
 Author: Carbonate
 Author-email: team@cabonate.dev
 Requires-Python: >=3.8.14,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,12 +25,12 @@
 
 Carbonate turns simple language driven instructions into end-to-end tests. This SDK lets you integrate it directly into your test suite.
 
 Learn more about Carbonate at [https://carbonate.dev](https://carbonate.dev).
 
 ## Getting Started
 
-Check out the [getting started guide](https://docs.carbonate.dev/sdk/getting-started/python) for instructions on how to integrate Carbonate into your test suite.
+Check out the [getting started guide](https://carbonate.dev/docs/sdk/getting-started/python) for instructions on how to integrate Carbonate into your test suite.
 
 ## License
 Distributed under the MIT License.
```

