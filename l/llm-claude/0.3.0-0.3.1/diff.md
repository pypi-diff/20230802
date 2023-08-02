# Comparing `tmp/llm-claude-0.3.0.tar.gz` & `tmp/llm-claude-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-claude-0.3.0.tar", last modified: Thu Jul 27 22:09:17 2023, max compression
+gzip compressed data, was "llm-claude-0.3.1.tar", last modified: Wed Aug  2 17:46:04 2023, max compression
```

## Comparing `llm-claude-0.3.0.tar` & `llm-claude-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 22:09:03.000000 llm-claude-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 22:09:17.751294 llm-claude-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 22:09:03.000000 llm-claude-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46863 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/completions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion_create_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 22:09:03.000000 llm-claude-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:09:17.751294 llm-claude-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-27 22:09:03.000000 llm-claude-0.3.0/tests/test_llm_claude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 17:45:49.000000 llm-claude-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-02 17:46:04.070572 llm-claude-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 17:45:49.000000 llm-claude-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.066571 llm-claude-0.3.1/llm_claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/llm_claude/vendored_anthropic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_base_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/llm_claude/vendored_anthropic/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/resources/completions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/llm_claude/vendored_anthropic/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/types/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-08-02 17:45:49.000000 llm-claude-0.3.1/llm_claude/vendored_anthropic/types/completion_create_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.066571 llm-claude-0.3.1/llm_claude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 17:46:04.000000 llm-claude-0.3.1/llm_claude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-02 17:45:49.000000 llm-claude-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:46:04.070572 llm-claude-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:46:04.070572 llm-claude-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-02 17:45:49.000000 llm-claude-0.3.1/tests/test_llm_claude.py
```

### Comparing `llm-claude-0.3.0/LICENSE` & `llm-claude-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/PKG-INFO` & `llm-claude-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-claude
-Version: 0.3.0
+Version: 0.3.1
 Summary: LLM plugin for Anthropic's Claude
 Author: Tom Viner
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tomviner/llm-claude
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 # llm-claude
 
 [![PyPI](https://img.shields.io/pypi/v/llm-claude.svg)](https://pypi.org/project/llm-claude/)
 [![Changelog](https://img.shields.io/github/v/release/tomviner/llm-claude?include_prereleases&label=changelog)](https://github.com/tomviner/llm-claude/releases)
 [![Tests](https://github.com/tomviner/llm-claude/workflows/Test/badge.svg)](https://github.com/tomviner/llm-claude/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tomviner/llm-claude/blob/main/LICENSE)
 
-Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude model.
+Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude models.
 
 ## Installation
 
 Install this plugin in the same environment as LLM.
 ```bash
 llm install llm-claude
 ```
@@ -45,15 +45,15 @@
 
 Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
 > - **Claude Instant**: low-latency, high throughput
 > - **Claude**: superior performance on tasks that require complex reasoning
 
-You can execute them like this:
+You can query them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
 ```
 
 ```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
```

### Comparing `llm-claude-0.3.0/README.md` & `llm-claude-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # llm-claude
 
 [![PyPI](https://img.shields.io/pypi/v/llm-claude.svg)](https://pypi.org/project/llm-claude/)
 [![Changelog](https://img.shields.io/github/v/release/tomviner/llm-claude?include_prereleases&label=changelog)](https://github.com/tomviner/llm-claude/releases)
 [![Tests](https://github.com/tomviner/llm-claude/workflows/Test/badge.svg)](https://github.com/tomviner/llm-claude/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tomviner/llm-claude/blob/main/LICENSE)
 
-Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude model.
+Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude models.
 
 ## Installation
 
 Install this plugin in the same environment as LLM.
 ```bash
 llm install llm-claude
 ```
@@ -32,15 +32,15 @@
 
 Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
 > - **Claude Instant**: low-latency, high throughput
 > - **Claude**: superior performance on tasks that require complex reasoning
 
-You can execute them like this:
+You can query them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
 ```
 
 ```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
```

### Comparing `llm-claude-0.3.0/llm_claude/__init__.py` & `llm-claude-0.3.1/llm_claude/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/__init__.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_client.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import time
 import uuid
 import inspect
 import platform
+from types import TracebackType
 from random import random
 from typing import (
     Any,
     Dict,
     Type,
     Union,
     Generic,
@@ -675,14 +676,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        self._client.close()
+
+    def __enter__(self: _T) -> _T:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        self.close()
+
     @overload
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
@@ -810,15 +832,15 @@
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
     ) -> SyncPageT:
-        resp = cast(SyncPageT, self.request(page, options, stream=False))
+        resp = self.request(page, options, stream=False)
         resp._set_private_attributes(  # pyright: ignore[reportPrivateUsage]
             client=self,
             model=model,
             options=options,
         )
         return resp
 
@@ -931,38 +953,38 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="patch", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def put(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="put", url=path, json_data=body, files=files, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def delete(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
         model: Type[ModelT],
         page: Type[SyncPageT],
@@ -1007,14 +1029,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    async def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        await self._client.aclose()
+
+    async def __aenter__(self: _T) -> _T:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.close()
+
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: Literal[False] = False,
```

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_exceptions.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_client.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import os
+import asyncio
 from typing import Union, Mapping, Optional
 
 import httpx
 from tokenizers import Tokenizer  # type: ignore[import]
 
-from . import resources
+from . import resources, _constants
 from ._qs import Querystring
 from ._types import (
     NOT_GIVEN,
     Omit,
     Headers,
     Timeout,
     NotGiven,
@@ -48,14 +49,18 @@
 class Anthropic(SyncAPIClient):
     completions: resources.Completions
 
     # client options
     api_key: str | None
     auth_token: str | None
 
+    # constants
+    HUMAN_PROMPT = _constants.HUMAN_PROMPT
+    AI_PROMPT = _constants.AI_PROMPT
+
     def __init__(
         self,
         *,
         auth_token: str | None = None,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: Union[float, Timeout, None] = DEFAULT_TIMEOUT,
@@ -77,40 +82,39 @@
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous anthropic client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
-        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         - `api_key` from `ANTHROPIC_API_KEY`
+        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         """
-        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", "")
+        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", None)
+        self.api_key = api_key
+
+        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
+        self.auth_token = auth_token or auth_token_envvar or None
 
         if base_url is None:
-            base_url = "https://api.anthropic.com"
+            base_url = f"https://api.anthropic.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.api_key = api_key
-
-        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
-        self.auth_token = auth_token or auth_token_envvar or None
-
         self._default_stream_cls = Stream
 
         self.completions = resources.Completions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -212,14 +216,17 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        self.close()
+
     def count_tokens(
         self,
         text: str,
     ) -> int:
         """Count the number of tokens in a given string"""
         # Note: tokenizer is untyped
         tokenizer = self.get_tokenizer()
@@ -233,14 +240,18 @@
 class AsyncAnthropic(AsyncAPIClient):
     completions: resources.AsyncCompletions
 
     # client options
     api_key: str | None
     auth_token: str | None
 
+    # constants
+    HUMAN_PROMPT = _constants.HUMAN_PROMPT
+    AI_PROMPT = _constants.AI_PROMPT
+
     def __init__(
         self,
         *,
         auth_token: str | None = None,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: Union[float, Timeout, None] = DEFAULT_TIMEOUT,
@@ -262,40 +273,39 @@
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async anthropic client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
-        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         - `api_key` from `ANTHROPIC_API_KEY`
+        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         """
-        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", "")
+        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", None)
+        self.api_key = api_key
+
+        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
+        self.auth_token = auth_token or auth_token_envvar or None
 
         if base_url is None:
-            base_url = "https://api.anthropic.com"
+            base_url = f"https://api.anthropic.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.api_key = api_key
-
-        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
-        self.auth_token = auth_token or auth_token_envvar or None
-
         self._default_stream_cls = AsyncStream
 
         self.completions = resources.AsyncCompletions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -397,14 +407,20 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        try:
+            asyncio.get_running_loop().create_task(self.close())
+        except Exception:
+            pass
+
     async def count_tokens(
         self,
         text: str,
     ) -> int:
         """Count the number of tokens in a given string"""
         # Note: tokenizer is untyped
         tokenizer = await self.get_tokenizer()
```

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_exceptions.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_models.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_qs.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_resource.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_streaming.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_tokenizers.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_types.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/__init__.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_transform.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_utils.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/completions.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/resources/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import List, overload
+from typing import List, Union, overload
 from typing_extensions import Literal
 
 from ..types import Completion, completion_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import required_args, maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._streaming import Stream, AsyncStream
@@ -17,15 +17,15 @@
 
 class Completions(SyncAPIResource):
     @overload
     def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         metadata: completion_create_params.CompletionRequestNonStreamingMetadata | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         stream: Literal[False] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
@@ -109,15 +109,15 @@
         ...
 
     @overload
     def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         stream: Literal[True],
         metadata: completion_create_params.CompletionRequestStreamingMetadata | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
@@ -201,15 +201,15 @@
         ...
 
     @required_args(["max_tokens_to_sample", "model", "prompt"], ["max_tokens_to_sample", "model", "prompt", "stream"])
     def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         metadata: completion_create_params.CompletionRequestNonStreamingMetadata
         | completion_create_params.CompletionRequestStreamingMetadata
         | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         stream: Literal[False] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
@@ -249,15 +249,15 @@
 
 class AsyncCompletions(AsyncAPIResource):
     @overload
     async def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         metadata: completion_create_params.CompletionRequestNonStreamingMetadata | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         stream: Literal[False] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
@@ -341,15 +341,15 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         stream: Literal[True],
         metadata: completion_create_params.CompletionRequestStreamingMetadata | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
         top_k: int | NotGiven = NOT_GIVEN,
         top_p: float | NotGiven = NOT_GIVEN,
@@ -433,15 +433,15 @@
         ...
 
     @required_args(["max_tokens_to_sample", "model", "prompt"], ["max_tokens_to_sample", "model", "prompt", "stream"])
     async def create(
         self,
         *,
         max_tokens_to_sample: int,
-        model: str,
+        model: Union[str, Literal["claude-2", "claude-instant-1"]],
         prompt: str,
         metadata: completion_create_params.CompletionRequestNonStreamingMetadata
         | completion_create_params.CompletionRequestStreamingMetadata
         | NotGiven = NOT_GIVEN,
         stop_sequences: List[str] | NotGiven = NOT_GIVEN,
         stream: Literal[False] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: float | NotGiven = NOT_GIVEN,
```

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion_create_params.py` & `llm-claude-0.3.1/llm_claude/vendored_anthropic/types/completion_create_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     max_tokens_to_sample: Required[int]
     """The maximum number of tokens to generate before stopping.
 
     Note that our models may stop _before_ reaching this maximum. This parameter
     only specifies the absolute maximum number of tokens to generate.
     """
 
-    model: Required[str]
+    model: Required[Union[str, Literal["claude-2", "claude-instant-1"]]]
     """The model that will complete your prompt.
 
     As we improve Claude, we develop new versions of it that you can query. This
     parameter controls which version of Claude answers your request. Right now we
     are offering two model families: Claude, and Claude Instant. You can use them by
     setting `model` to `"claude-2"` or `"claude-instant-1"`, respectively. See
     [models](https://docs.anthropic.com/claude/reference/selecting-a-model) for
@@ -105,15 +105,15 @@
     max_tokens_to_sample: Required[int]
     """The maximum number of tokens to generate before stopping.
 
     Note that our models may stop _before_ reaching this maximum. This parameter
     only specifies the absolute maximum number of tokens to generate.
     """
 
-    model: Required[str]
+    model: Required[Union[str, Literal["claude-2", "claude-instant-1"]]]
     """The model that will complete your prompt.
 
     As we improve Claude, we develop new versions of it that you can query. This
     parameter controls which version of Claude answers your request. Right now we
     are offering two model families: Claude, and Claude Instant. You can use them by
     setting `model` to `"claude-2"` or `"claude-instant-1"`, respectively. See
     [models](https://docs.anthropic.com/claude/reference/selecting-a-model) for
```

### Comparing `llm-claude-0.3.0/llm_claude.egg-info/PKG-INFO` & `llm-claude-0.3.1/llm_claude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-claude
-Version: 0.3.0
+Version: 0.3.1
 Summary: LLM plugin for Anthropic's Claude
 Author: Tom Viner
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tomviner/llm-claude
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 # llm-claude
 
 [![PyPI](https://img.shields.io/pypi/v/llm-claude.svg)](https://pypi.org/project/llm-claude/)
 [![Changelog](https://img.shields.io/github/v/release/tomviner/llm-claude?include_prereleases&label=changelog)](https://github.com/tomviner/llm-claude/releases)
 [![Tests](https://github.com/tomviner/llm-claude/workflows/Test/badge.svg)](https://github.com/tomviner/llm-claude/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tomviner/llm-claude/blob/main/LICENSE)
 
-Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude model.
+Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude models.
 
 ## Installation
 
 Install this plugin in the same environment as LLM.
 ```bash
 llm install llm-claude
 ```
@@ -45,15 +45,15 @@
 
 Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
 > - **Claude Instant**: low-latency, high throughput
 > - **Claude**: superior performance on tasks that require complex reasoning
 
-You can execute them like this:
+You can query them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
 ```
 
 ```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
```

### Comparing `llm-claude-0.3.0/llm_claude.egg-info/SOURCES.txt` & `llm-claude-0.3.1/llm_claude.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-claude-0.3.0/pyproject.toml` & `llm-claude-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-claude"
-version = "0.3.0"
+version = "0.3.1"
 
 description = "LLM plugin for Anthropic's Claude"
 readme = "README.md"
 authors = [{name = "Tom Viner"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `llm-claude-0.3.0/tests/test_llm_claude.py` & `llm-claude-0.3.1/tests/test_llm_claude.py`

 * *Files identical despite different names*

