# Comparing `tmp/fastapi-csrf-protect-0.3.1.tar.gz` & `tmp/fastapi_csrf_protect-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-csrf-protect-0.3.1.tar", max compression
+gzip compressed data, was "fastapi_csrf_protect-0.3.2.tar", max compression
```

## Comparing `fastapi-csrf-protect-0.3.1.tar` & `fastapi_csrf_protect-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi-csrf-protect-0.3.1/LICENSE
--rw-r--r--   0        0        0     4524 2023-06-18 12:43:21.460103 fastapi-csrf-protect-0.3.1/README.md
--rw-r--r--   0        0        0      443 2023-06-18 12:37:02.455348 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/__init__.py
--rw-r--r--   0        0        0     7005 2023-06-18 12:37:02.446608 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/core.py
--rw-r--r--   0        0        0     1941 2023-06-18 12:37:02.451374 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/csrf_config.py
--rw-r--r--   0        0        0      825 2023-06-18 12:37:02.451249 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/exceptions.py
--rw-r--r--   0        0        0     1867 2023-06-18 12:37:02.451264 fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/load_config.py
--rw-r--r--   0        0        0     1768 2023-06-18 12:37:02.419399 fastapi-csrf-protect-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.1/setup.py
--rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi_csrf_protect-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5056 2023-08-02 06:18:49.057679 fastapi_csrf_protect-0.3.2/README.md
+-rw-r--r--   0        0        0      443 2023-08-02 06:08:34.791468 fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/__init__.py
+-rw-r--r--   0        0        0     7788 2023-08-02 06:08:34.790341 fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/core.py
+-rw-r--r--   0        0        0     2136 2023-08-02 06:08:34.791451 fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/csrf_config.py
+-rw-r--r--   0        0        0      825 2023-08-02 06:08:34.791440 fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/exceptions.py
+-rw-r--r--   0        0        0     2599 2023-08-02 06:08:34.791459 fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/load_config.py
+-rw-r--r--   0        0        0     1768 2023-08-02 06:08:34.790410 fastapi_csrf_protect-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6405 1970-01-01 00:00:00.000000 fastapi_csrf_protect-0.3.2/PKG-INFO
```

### Comparing `fastapi-csrf-protect-0.3.1/LICENSE` & `fastapi_csrf_protect-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-csrf-protect-0.3.1/README.md` & `fastapi_csrf_protect-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,14 @@
 FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
 Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
 If you were familiar with `flask-wtf` library this extension suitable for you.
 This extension inspired by `fastapi-jwt-auth` 😀
 
 - Storing `fastapi-csrf-token` in cookies or serve it in template's context
 
-## 🚧 Breaking Changes (0.3.0 -> 0.3.1)
-
-* The `generate_csrf` method has now been marked for deprecation
-* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned
-  and the latter signed
-* Recommended pattern is for the first token is aimed for returning as part of context
-* Recommended pattern is for the signed token to be set in client's cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)
-* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client's cookies as
-  per example code and recommended pattern.
-
 ## Installation
 
 The easiest way to start working with this extension with pip
 
 ```bash
 pip install fastapi-csrf-protect
 # or
@@ -69,19 +59,19 @@
   response = templates.TemplateResponse(
     "form.html", {"request": request, "csrf_token": csrf_token}
   )
   csrf_protect.set_csrf_cookie(signed_token, response)
   return response
 
 @app.post("/login", response_class=JSONResponse)
-def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
+async def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
   """
   Creates a new Post
   """
-  csrf_protect.validate_csrf(request)
+  await csrf_protect.validate_csrf(request)
   response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})
   csrf_protect.unset_csrf_cookie(response)  # prevent token reuse
   return response
 
 @app.exception_handler(CsrfProtectError)
 def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
   return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
@@ -101,25 +91,50 @@
 Testing can be done by the following command post-installation:
 
 ```bash
 poetry install --with test
 pytest
 ```
 
+## Changelog
+
+### 🚧 Breaking Changes (0.3.0 -> 0.3.1) The double submit update
+
+* The `generate_csrf` method has now been marked for deprecation
+* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned
+  and the latter signed
+* Recommended pattern is for the first token is aimed for returning as part of context
+* Recommended pattern is for the signed token to be set in client's cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)
+* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client's cookies as
+  per example code and recommended pattern.
+
+### 🚧 Breaking Changes (0.3.1 -> 0.3.2) The anti-JavaScript update
+
+* New keys are added at setup `token_location` (either `body` or `header`) and `token_key` is key
+  where form-encoded keeps the csrf token stored, cross-checked with csrf secret in cookies.
+* Asynchronous `validate_csrf` method now needs to be awaited therefore protected endpoints need to
+  be asynchronous as well.
+
 ### Run Examples
 
 To run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)
 Alternatively, run the following command on your terminal to do so
 
 ```bash
 poetry install --with examples
 ```
 
-Running the example utilizing Context and Headers
+Running the example utilizing form submission
+
+```bash
+uvicorn examples.body:app
+```
+
+Running the example utilizing headers via JavaScript
 
 ```bash
-uvicorn examples.login:app
+uvicorn examples.header:app
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/core.py` & `fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  core.py
-# VERSION: 	 0.3.1
+# VERSION: 	 0.3.2
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 import re
-from os import urandom
-from hashlib import sha1
-from typing import Optional, Tuple
 from fastapi.requests import Request
 from fastapi.responses import Response
-from starlette.datastructures import Headers
-from itsdangerous import BadData, SignatureExpired, URLSafeTimedSerializer
 from fastapi_csrf_protect.csrf_config import CsrfConfig
 from fastapi_csrf_protect.exceptions import (
     InvalidHeaderError,
     MissingTokenError,
     TokenValidationError,
 )
+from itsdangerous import BadData, SignatureExpired, URLSafeTimedSerializer
+from hashlib import sha1
+from os import urandom
+from pydantic import create_model
+from starlette.datastructures import Headers
+from typing import Any, Dict, Optional, Tuple
 from warnings import warn
 
 
 class CsrfProtect(CsrfConfig):
     def generate_csrf(self, secret_key: Optional[str] = None) -> Tuple[str, str]:
         """
         Deprecated. Please use `generate_csrf_tokens` method instead.
 
         ---
         :param secret_key: (Optional) the secret key used when generating tokens for users
         :type secret_key: (str | None) Defaults to None.
         """
-        warn("This is deprecated; version=0.3.1", DeprecationWarning, stacklevel=2)
+        warn("This is deprecated; version=0.3.2", DeprecationWarning, stacklevel=2)
         return self.generate_csrf_tokens(secret_key)
 
     def generate_csrf_tokens(self, secret_key: Optional[str] = None) -> Tuple[str, str]:
         """
         Generate a CSRF token and a signed CSRF token using server's secret key to be stored in
         cookie. R
 
@@ -50,17 +51,33 @@
         if secret_key is None:
             raise RuntimeError("A secret key is required to use CsrfProtect extension.")
         serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
         token = sha1(urandom(64)).hexdigest()
         signed = serializer.dumps(token)
         return token, signed
 
+    def get_csrf_from_body(self, data: bytes) -> str:
+        """
+        Get token from the request body
+
+        ---
+        :param data: attached request body containing cookie data with configured `token_key`
+        :type data: bytes
+        """
+        fields: Dict[str, Any] = {self._token_key: (str, "csrf-token")}
+        Body = create_model("Body", **fields)
+        content: str = (
+            '{"' + data.decode("utf-8").replace("&", '","').replace("=", '":"') + '"}'
+        )
+        body: Body = Body.parse_raw(content)
+        return body.dict()[self._token_key]
+
     def get_csrf_from_headers(self, headers: Headers) -> str:
         """
-        Get token from the headers
+        Get token from the request headers
 
         ---
         :param headers: Headers containing header with configured `header_name`
         :type headers: starlette.datastructures.Headers
         """
         header_name, header_type = self._header_name, self._header_type
         header_parts = None
@@ -124,15 +141,15 @@
         """
         if not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
         response.delete_cookie(
             self._cookie_key, path=self._cookie_path, domain=self._cookie_domain
         )
 
-    def validate_csrf(
+    async def validate_csrf(
         self,
         request: Request,
         cookie_key: Optional[str] = None,
         secret_key: Optional[str] = None,
         time_limit: Optional[int] = None,
     ):
         """
@@ -157,15 +174,19 @@
         if secret_key is None:
             raise RuntimeError("A secret key is required to use CsrfProtect extension.")
         cookie_key = cookie_key or self._cookie_key
         signed_token = request.cookies.get(cookie_key)
         if signed_token is None:
             raise MissingTokenError(f"Missing Cookie: `{cookie_key}`.")
         time_limit = time_limit or self._max_age
-        token: str = self.get_csrf_from_headers(request.headers)
+        token: str
+        if self._token_location == "header":
+            token = self.get_csrf_from_headers(request.headers)
+        else:
+            token = self.get_csrf_from_body(await request.body())
         serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
         try:
             signature: str = serializer.loads(signed_token, max_age=time_limit)
             if token != signature:
                 raise TokenValidationError(
                     "The CSRF signatures submitted do not match."
                 )
```

### Comparing `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/csrf_config.py` & `fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/csrf_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  fastapi_csrf_config.py
-# VERSION: 	 0.3.1
+# VERSION: 	 0.3.2
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 ### Standard Packages ###
@@ -17,23 +17,25 @@
 ### Local Modules ###
 from fastapi_csrf_protect.load_config import LoadConfig
 
 
 class CsrfConfig(object):
     _cookie_key: str = "fastapi-csrf-token"
     _cookie_path: str = "/"
-    _cookie_domain: str = None
+    _cookie_domain: Optional[str] = None
     _cookie_samesite: Optional[Literal["lax", "strict", "none"]] = None
     _cookie_secure: bool = False
     _header_name: str = "X-CSRF-Token"
-    _header_type: str = None
+    _header_type: Optional[str] = None
     _httponly: bool = True
     _max_age: int = 3600
     _methods: Sequence[str] = {"POST", "PUT", "PATCH", "DELETE"}
     _secret_key: str = None
+    _token_location: str = "header"
+    _token_key: Optional[str] = None
 
     @classmethod
     def load_config(cls, settings: Callable[..., List[tuple]]) -> None:
         try:
             config = LoadConfig(**{key.lower(): value for key, value in settings()})
             cls._cookie_key = config.cookie_key
             cls._cookie_path = config.cookie_path
@@ -42,14 +44,16 @@
             cls._cookie_secure = config.cookie_secure
             cls._header_name = config.header_name
             cls._header_type = config.header_type
             cls._httponly = config.httponly
             cls._max_age = config.max_age
             cls._methods = config.methods
             cls._secret_key = config.secret_key
+            cls._token_location = config.token_location
+            cls._token_key = config.token_key
         except ValidationError:
             raise
         except Exception as err:
             print(err)
             raise TypeError(
                 'CsrfConfig must be pydantic "BaseSettings" or list of tuple'
             )
```

### Comparing `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/exceptions.py` & `fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  exceptions.py
-# VERSION: 	 0.3.1
+# VERSION: 	 0.3.2
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 class CsrfProtectError(Exception):
```

### Comparing `fastapi-csrf-protect-0.3.1/fastapi_csrf_protect/load_config.py` & `fastapi_csrf_protect-0.3.2/fastapi_csrf_protect/load_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 #!/usr/bin/env python3
 # Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  load_config.py
-# VERSION: 	 0.3.1
+# VERSION: 	 0.3.2
 # CREATED: 	 2020-11-25 14:35
 # AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
-from typing import Optional, Sequence
+from typing import Any, Dict, Optional, Set
 from pydantic import BaseModel, validator, StrictBool, StrictInt, StrictStr
 
 
 class LoadConfig(BaseModel):
     cookie_key: Optional[StrictStr] = "fastapi-csrf-token"
     cookie_path: Optional[StrictStr] = "/"
     cookie_domain: Optional[StrictStr] = None
     # NOTE: `cookie_secure` must be placed before `cookie_samesite`
     cookie_secure: Optional[StrictBool] = False
     cookie_samesite: Optional[StrictStr] = "lax"
     header_name: Optional[StrictStr] = "X-CSRF-Token"
     header_type: Optional[StrictStr] = None
     httponly: Optional[StrictBool] = True
     max_age: Optional[StrictInt] = 3600
-    methods: Optional[Sequence[StrictStr]] = {"POST", "PUT", "PATCH", "DELETE"}
+    methods: Optional[Set[StrictStr]] = {"POST", "PUT", "PATCH", "DELETE"}
     secret_key: Optional[StrictStr] = None
+    token_location: Optional[StrictStr] = "header"
+    token_key: Optional[StrictStr] = None
 
     @validator("methods", each_item=True)
     def validate_csrf_methods(cls, value):
         if value.upper() not in {"GET", "HEAD", "POST", "PUT", "DELETE", "PATCH"}:
             raise ValueError('The "csrf_methods" must be between http request methods')
         return value.upper()
 
     @validator("cookie_samesite", always=True)
-    def validate_cookie_samesite(cls, value: str, values: dict):
+    def validate_cookie_samesite(cls, value: str, values: Dict[str, Any]):
         if value not in {"strict", "lax", "none"}:
             raise ValueError(
                 'The "cookie_samesite" must be between "strict", "lax", or "none".'
             )
         elif value == "none" and values.get("cookie_secure", False) is not True:
             raise ValueError(
                 'The "cookie_secure" must be True if "cookie_samesite" set to "none".'
             )
         return value
+
+    @validator("token_location")
+    def validate_token_location(cls, value: str):
+        if value not in {"body", "header"}:
+            raise ValueError('The "token_location" must be either "body" or "header".')
+        return value
+
+    @validator("token_key", always=True)
+    def validate_token_key(cls, value: Optional[str], values: Dict[str, Any]):
+        token_location: str = values.get("token_location", "header")
+        if token_location == "body" and value is None:
+            raise ValueError(
+                'The "body_key" must be present when "token_location" is "body"'
+            )
+        return value
```

### Comparing `fastapi-csrf-protect-0.3.1/pyproject.toml` & `fastapi_csrf_protect-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-csrf-protect"
-version = "0.3.1"
+version = "0.3.2"
 description = "Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern"
 authors = ["Sitt Guruvanich <aekazitt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aekasitt/fastapi-csrf-protect"
 repository = "https://github.com/aekasitt/fastapi-csrf-protect"
 keywords = ["starlette", "fastapi", "csrf", "xsrf", "cross-site request forgery", "samesite", "asynchronous"]
@@ -24,15 +24,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 fastapi = "^0"
 itsdangerous = ">=2.0.1,<3.0.0"
-pydantic = ">=1.7.2,<2.0.0"
+pydantic = ">=1.7.2,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.3.0"
 
 [tool.poetry.group.examples]
 optional = true
```

### Comparing `fastapi-csrf-protect-0.3.1/setup.py` & `fastapi_csrf_protect-0.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-csrf-protect
+Version: 0.3.2
+Summary: Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern
+Home-page: https://github.com/aekasitt/fastapi-csrf-protect
+License: MIT
+Keywords: starlette,fastapi,csrf,xsrf,cross-site request forgery,samesite,asynchronous
+Author: Sitt Guruvanich
+Author-email: aekazitt@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: fastapi (>=0,<1)
+Requires-Dist: itsdangerous (>=2.0.1,<3.0.0)
+Requires-Dist: pydantic (>=1.7.2,<3.0.0)
+Project-URL: Repository, https://github.com/aekasitt/fastapi-csrf-protect
+Description-Content-Type: text/markdown
+
+# FastAPI CSRF Protect
+
+[![Build Status](https://travis-ci.com/aekasitt/fastapi-csrf-protect.svg?branch=master)](https://app.travis-ci.com/github/aekasitt/fastapi-csrf-protect)
+[![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
+[![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
+[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
+[![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
+
+## Features
+
+FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
+Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
+If you were familiar with `flask-wtf` library this extension suitable for you.
+This extension inspired by `fastapi-jwt-auth` 😀
+
+- Storing `fastapi-csrf-token` in cookies or serve it in template's context
+
+## Installation
+
+The easiest way to start working with this extension with pip
+
+```bash
+pip install fastapi-csrf-protect
+# or
+poetry add fastapi-csrf-protect
+```
+
+## Getting Started
+
+The following examples show you how to integrate this extension to a FastAPI App
+
+### Example Login Form
+
+```python
+from fastapi import FastAPI, Request, Depends
+from fastapi.responses import JSONResponse
+from fastapi.templating import Jinja2Templates
+from fastapi_csrf_protect import CsrfProtect
+from fastapi_csrf_protect.exceptions import CsrfProtectError
+from pydantic import BaseModel
+
+app = FastAPI()
+templates = Jinja2Templates(directory="templates")
+
+class CsrfSettings(BaseModel):
+  secret_key: str = "asecrettoeverybody"
+  cookie_samesite: str = "none"
+
+@CsrfProtect.load_config
+def get_csrf_config():
+  return CsrfSettings()
+
+@app.get("/login")
+def form(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
+  Returns form template.
+  """
+  csrf_token, signed_token = csrf_protect.generate_csrf_tokens()
+  response = templates.TemplateResponse(
+    "form.html", {"request": request, "csrf_token": csrf_token}
+  )
+  csrf_protect.set_csrf_cookie(signed_token, response)
+  return response
+
+@app.post("/login", response_class=JSONResponse)
+async def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
+  Creates a new Post
+  """
+  await csrf_protect.validate_csrf(request)
+  response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})
+  csrf_protect.unset_csrf_cookie(response)  # prevent token reuse
+  return response
+
+@app.exception_handler(CsrfProtectError)
+def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
+  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
+
+```
+
+## Contributions
+
+To contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)
+Alternatively, run the following command on your terminal to do so:
+
+```bash
+pip install -U poetry
+poetry install
+```
+
+Testing can be done by the following command post-installation:
+
+```bash
+poetry install --with test
+pytest
+```
+
+## Changelog
+
+### 🚧 Breaking Changes (0.3.0 -> 0.3.1) The double submit update
+
+* The `generate_csrf` method has now been marked for deprecation
+* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned
+  and the latter signed
+* Recommended pattern is for the first token is aimed for returning as part of context
+* Recommended pattern is for the signed token to be set in client's cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)
+* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client's cookies as
+  per example code and recommended pattern.
+
+### 🚧 Breaking Changes (0.3.1 -> 0.3.2) The anti-JavaScript update
+
+* New keys are added at setup `token_location` (either `body` or `header`) and `token_key` is key
+  where form-encoded keeps the csrf token stored, cross-checked with csrf secret in cookies.
+* Asynchronous `validate_csrf` method now needs to be awaited therefore protected endpoints need to
+  be asynchronous as well.
+
+### Run Examples
+
+To run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)
+Alternatively, run the following command on your terminal to do so
+
+```bash
+poetry install --with examples
+```
+
+Running the example utilizing form submission
+
+```bash
+uvicorn examples.body:app
+```
+
+Running the example utilizing headers via JavaScript
+
+```bash
+uvicorn examples.header:app
+```
 
-packages = \
-['fastapi_csrf_protect']
+## License
 
-package_data = \
-{'': ['*']}
+This project is licensed under the terms of the MIT license.
 
-install_requires = \
-['fastapi>=0,<1', 'itsdangerous>=2.0.1,<3.0.0', 'pydantic>=1.7.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'fastapi-csrf-protect',
-    'version': '0.3.1',
-    'description': 'Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern',
-    'long_description': '# FastAPI CSRF Protect\n\n[![Build Status](https://travis-ci.com/aekasitt/fastapi-csrf-protect.svg?branch=master)](https://app.travis-ci.com/github/aekasitt/fastapi-csrf-protect)\n[![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n[![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)\n\n## Features\n\nFastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.\nAimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.\nIf you were familiar with `flask-wtf` library this extension suitable for you.\nThis extension inspired by `fastapi-jwt-auth` 😀\n\n- Storing `fastapi-csrf-token` in cookies or serve it in template\'s context\n\n## 🚧 Breaking Changes (0.3.0 -> 0.3.1)\n\n* The `generate_csrf` method has now been marked for deprecation\n* The recommended method is now `generate_csrf_tokens` which returns a tuple of tokens, first unsigned\n  and the latter signed\n* Recommended pattern is for the first token is aimed for returning as part of context\n* Recommended pattern is for the signed token to be set in client\'s cookie completing [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie)\n* To prevent token reuse, protected endpoint can unset the signed CSRF Token in client\'s cookies as\n  per example code and recommended pattern.\n\n## Installation\n\nThe easiest way to start working with this extension with pip\n\n```bash\npip install fastapi-csrf-protect\n# or\npoetry add fastapi-csrf-protect\n```\n\n## Getting Started\n\nThe following examples show you how to integrate this extension to a FastAPI App\n\n### Example Login Form\n\n```python\nfrom fastapi import FastAPI, Request, Depends\nfrom fastapi.responses import JSONResponse\nfrom fastapi.templating import Jinja2Templates\nfrom fastapi_csrf_protect import CsrfProtect\nfrom fastapi_csrf_protect.exceptions import CsrfProtectError\nfrom pydantic import BaseModel\n\napp = FastAPI()\ntemplates = Jinja2Templates(directory="templates")\n\nclass CsrfSettings(BaseModel):\n  secret_key: str = "asecrettoeverybody"\n  cookie_samesite: str = "none"\n\n@CsrfProtect.load_config\ndef get_csrf_config():\n  return CsrfSettings()\n\n@app.get("/login")\ndef form(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Returns form template.\n  """\n  csrf_token, signed_token = csrf_protect.generate_csrf_tokens()\n  response = templates.TemplateResponse(\n    "form.html", {"request": request, "csrf_token": csrf_token}\n  )\n  csrf_protect.set_csrf_cookie(signed_token, response)\n  return response\n\n@app.post("/login", response_class=JSONResponse)\ndef create_post(request: Request, csrf_protect: CsrfProtect = Depends()):\n  """\n  Creates a new Post\n  """\n  csrf_protect.validate_csrf(request)\n  response: JSONResponse = JSONResponse(status_code=200, content={"detail": "OK"})\n  csrf_protect.unset_csrf_cookie(response)  # prevent token reuse\n  return response\n\n@app.exception_handler(CsrfProtectError)\ndef csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):\n  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})\n\n```\n\n## Contributions\n\nTo contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)\nAlternatively, run the following command on your terminal to do so:\n\n```bash\npip install -U poetry\npoetry install\n```\n\nTesting can be done by the following command post-installation:\n\n```bash\npoetry install --with test\npytest\n```\n\n### Run Examples\n\nTo run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)\nAlternatively, run the following command on your terminal to do so\n\n```bash\npoetry install --with examples\n```\n\nRunning the example utilizing Context and Headers\n\n```bash\nuvicorn examples.login:app\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
-    'author': 'Sitt Guruvanich',
-    'author_email': 'aekazitt@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/aekasitt/fastapi-csrf-protect',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

