# Comparing `tmp/jsm_user_services-1.3.4.tar.gz` & `tmp/jsm_user_services-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.3.4.tar", max compression
+gzip compressed data, was "jsm_user_services-1.3.5.tar", max compression
```

## Comparing `jsm_user_services-1.3.4.tar` & `jsm_user_services-1.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/LICENSE
--rw-r--r--   0        0        0    10306 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/README.md
--rw-r--r--   0        0        0       54 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     2475 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    14221 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/flask/__init__.py
--rw-r--r--   0        0        0     3462 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/flask/middleware.py
--rw-r--r--   0        0        0     3167 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4258 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     4657 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     1840 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1007 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      419 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     2185 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1572 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 jsm_user_services-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/LICENSE
+-rw-r--r--   0        0        0    10306 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/README.md
+-rw-r--r--   0        0        0       54 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2475 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14221 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/flask/__init__.py
+-rw-r--r--   0        0        0     3462 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/flask/middleware.py
+-rw-r--r--   0        0        0     3167 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4247 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     4657 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     1840 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1007 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      419 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1572 2023-08-02 14:31:56.626486 jsm_user_services-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0    11385 1970-01-01 00:00:00.000000 jsm_user_services-1.3.5/PKG-INFO
```

### Comparing `jsm_user_services-1.3.4/LICENSE` & `jsm_user_services-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/README.md` & `jsm_user_services-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.3.5/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.3.5/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.3.5/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.3.5/jsm_user_services/drf_tools/permissions.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/exception.py` & `jsm_user_services-1.3.5/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.3.5/jsm_user_services/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/middleware.py` & `jsm_user_services-1.3.5/jsm_user_services/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/services/everest.py` & `jsm_user_services-1.3.5/jsm_user_services/services/everest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import TypedDict
 
 from requests import Response
-from typing_extensions import TypedDict
 
 from jsm_user_services.exception import EmailValidationError
 from jsm_user_services.support.email_utils import perform_callback_function_validators
 from jsm_user_services.support.email_utils import validate_format_email
 from jsm_user_services.support.http_utils import get_response_body
 from jsm_user_services.support.http_utils import request
 from jsm_user_services.support.settings_utils import get_from_settings_or_raise_missing_config
```

### Comparing `jsm_user_services-1.3.4/jsm_user_services/services/google.py` & `jsm_user_services-1.3.5/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/services/user.py` & `jsm_user_services-1.3.5/jsm_user_services/services/user.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/settings.py` & `jsm_user_services-1.3.5/jsm_user_services/settings.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.3.5/jsm_user_services/support/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.3.5/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.3.5/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/support/request_id.py` & `jsm_user_services-1.3.5/jsm_user_services/support/request_id.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.3.5/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.4/pyproject.toml` & `jsm_user_services-1.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.3.4"
+version = "1.3.5"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
@@ -16,15 +16,15 @@
     "Framework :: Django",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 PyJWT = "2.1.0"
 requests = "*"
 
 [tool.poetry.extras]
 flask = ["flask", "flask-log-request-id"]
 drf = ["djangorestframework", "request-id-django-log"]
```

### Comparing `jsm_user_services-1.3.4/PKG-INFO` & `jsm_user_services-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.3.4
+Version: 1.3.5
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: drf
 Provides-Extra: flask
```

