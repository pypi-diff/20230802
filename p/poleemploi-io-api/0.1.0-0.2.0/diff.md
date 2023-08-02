# Comparing `tmp/poleemploi_io_api-0.1.0.tar.gz` & `tmp/poleemploi_io_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poleemploi_io_api-0.1.0.tar", max compression
+gzip compressed data, was "poleemploi_io_api-0.2.0.tar", max compression
```

## Comparing `poleemploi_io_api-0.1.0.tar` & `poleemploi_io_api-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      416 2023-02-03 13:01:08.644072 poleemploi_io_api-0.1.0/README.md
--rw-r--r--   0        0        0       84 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/__init__.py
--rw-r--r--   0        0        0       29 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/base/__init__.py
--rw-r--r--   0        0        0     1434 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/base/api.py
--rw-r--r--   0        0        0      134 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/base/schemas.py
--rw-r--r--   0        0        0       29 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/rome/v1/__init__.py
--rw-r--r--   0        0        0     1891 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/rome/v1/api.py
--rw-r--r--   0        0        0       20 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/tests/__init__.py
--rw-r--r--   0        0        0     1096 2023-02-03 13:01:08.648072 poleemploi_io_api-0.1.0/poleemploi_io_api/tests/test_base.py
--rw-r--r--   0        0        0     1184 2023-02-03 13:31:02.676313 poleemploi_io_api-0.1.0/poleemploi_io_api/tests/test_rome_v1.py
--rw-r--r--   0        0        0     1614 2023-02-03 13:31:36.048094 poleemploi_io_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 poleemploi_io_api-0.1.0/setup.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 poleemploi_io_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      416 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/README.md
+-rw-r--r--   0        0        0      127 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/__init__.py
+-rw-r--r--   0        0        0       29 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/base/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/base/api.py
+-rw-r--r--   0        0        0      134 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/base/schemas.py
+-rw-r--r--   0        0        0       29 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/rome/v1/__init__.py
+-rw-r--r--   0        0        0     1891 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/rome/v1/api.py
+-rw-r--r--   0        0        0       42 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/rome/v4/__init__.py
+-rw-r--r--   0        0        0     1936 2023-08-02 09:55:07.722279 poleemploi_io_api-0.2.0/poleemploi_io_api/rome/v4/api.py
+-rw-r--r--   0        0        0       20 2023-08-02 09:55:07.734279 poleemploi_io_api-0.2.0/poleemploi_io_api/tests/__init__.py
+-rw-r--r--   0        0        0     1096 2023-08-02 09:55:07.734279 poleemploi_io_api-0.2.0/poleemploi_io_api/tests/test_base.py
+-rw-r--r--   0        0        0     1184 2023-08-02 09:55:07.734279 poleemploi_io_api-0.2.0/poleemploi_io_api/tests/test_rome_v1.py
+-rw-r--r--   0        0        0     1631 2023-08-02 09:55:07.734279 poleemploi_io_api-0.2.0/poleemploi_io_api/tests/test_rome_v4.py
+-rw-r--r--   0        0        0     1614 2023-08-02 09:55:40.538717 poleemploi_io_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 poleemploi_io_api-0.2.0/PKG-INFO
```

### Comparing `poleemploi_io_api-0.1.0/poleemploi_io_api/base/api.py` & `poleemploi_io_api-0.2.0/poleemploi_io_api/base/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import requests
 from .schemas import Token
 
 
-class Api():
-
+class Api:
     def __init__(self, **kwargs):
-
         # params
-        self._token_url = kwargs.get(
-            "url", "https://entreprise.pole-emploi.fr")
+        self._token_url = kwargs.get("url", "https://entreprise.pole-emploi.fr")
         self._client_secret = kwargs.get("client_secret", None)
         self._client_id = kwargs.get("client_id", None)
 
         self._access_token = None
 
     def scope(self) -> str:
         raise NotImplementedError(
-            "You must define this function to define the scope of the token")
+            "You must define this function to define the scope of the token"
+        )
 
     def _get_access_token(self):
-
         scope = self.scope()
 
         params = {
             "grant_type": "client_credentials",
             "scope": scope,
         }
-        data = {
-            'client_secret': self._client_secret,
-            'client_id': self._client_id
-        }
+        data = {"client_secret": self._client_secret, "client_id": self._client_id}
 
         r = requests.post(
-            self._token_url + "/connexion/oauth2/access_token?realm=%2Fpartenaire", params=params, data=data)
+            self._token_url + "/connexion/oauth2/access_token?realm=%2Fpartenaire",
+            params=params,
+            data=data,
+        )
 
         if r.status_code != 200:
             raise ValueError(
-                f"Could not read token from api. status_code={r.status_code} response={r.content}")
+                f"Could not read token from api. status_code={r.status_code} response={r.content}"
+            )
 
         self._access_token = Token(**r.json())
 
     def _get_auth_header(self, header=None):
-
         if not self._access_token:
             self._get_access_token()
 
         if not header:
             header = {}
 
-        header["Authorization"] = f"{self._access_token.token_type} {self._access_token.access_token}"
+        header[
+            "Authorization"
+        ] = f"{self._access_token.token_type} {self._access_token.access_token}"
 
         return header
```

### Comparing `poleemploi_io_api-0.1.0/poleemploi_io_api/rome/v1/api.py` & `poleemploi_io_api-0.2.0/poleemploi_io_api/rome/v1/api.py`

 * *Files identical despite different names*

### Comparing `poleemploi_io_api-0.1.0/poleemploi_io_api/tests/test_base.py` & `poleemploi_io_api-0.2.0/poleemploi_io_api/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `poleemploi_io_api-0.1.0/poleemploi_io_api/tests/test_rome_v1.py` & `poleemploi_io_api-0.2.0/poleemploi_io_api/tests/test_rome_v1.py`

 * *Files identical despite different names*

### Comparing `poleemploi_io_api-0.1.0/pyproject.toml` & `poleemploi_io_api-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poleemploi-io-api"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python package to use poleemploi io api (requires account)"
 authors = ["La Bonne Boite <labonneboite@pole-emploi.fr>"]
 license  = "GPL-3.0-only"
 keywords = ["poleemploi", "poleemploi_io", "poleemploi_io_api"]
 readme = "README.md"
 packages = [
     { include = "poleemploi_io_api" }
```

### Comparing `poleemploi_io_api-0.1.0/setup.py` & `poleemploi_io_api-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,51 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: poleemploi-io-api
+Version: 0.2.0
+Summary: Python package to use poleemploi io api (requires account)
+Home-page: https://github.com/StartupsPoleEmploi/poleemploi-io-api
+License: GPL-3.0-only
+Keywords: poleemploi,poleemploi_io,poleemploi_io_api
+Author: La Bonne Boite
+Author-email: labonneboite@pole-emploi.fr
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic[email] (>=1.10.4,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Repository, https://github.com/StartupsPoleEmploi/poleemploi-io-api
+Description-Content-Type: text/markdown
 
-packages = \
-['poleemploi_io_api',
- 'poleemploi_io_api.base',
- 'poleemploi_io_api.rome.v1',
- 'poleemploi_io_api.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic[email]>=1.10.4,<2.0.0', 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'poleemploi-io-api',
-    'version': '0.1.0',
-    'description': 'Python package to use poleemploi io api (requires account)',
-    'long_description': '# PoleEmploi IO - Python Package\n\n## About\n\nThis package was intended to use the [poleemploi.io](https://pole-emploi.io/) api.\n\nTo be able to use you need valid poleemloi.io credentials.\n\n\n## How tos\n\n### Tests\n\n``` bash\nmake test\n```\n\n### Documentation\n\nThe documentation is based on [mkdocs](https://www.mkdocs.org/)\n\nTo open the docs:\n\n``` bash\nmake help\n```\n\nIt will be accessible [here](http://127.0.0.1:9999/)\n',
-    'author': 'La Bonne Boite',
-    'author_email': 'labonneboite@pole-emploi.fr',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/StartupsPoleEmploi/poleemploi-io-api',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+# PoleEmploi IO - Python Package
 
+## About
+
+This package was intended to use the [poleemploi.io](https://pole-emploi.io/) api.
+
+To be able to use you need valid poleemloi.io credentials.
+
+
+## How tos
+
+### Tests
+
+``` bash
+make test
+```
+
+### Documentation
+
+The documentation is based on [mkdocs](https://www.mkdocs.org/)
+
+To open the docs:
+
+``` bash
+make help
+```
+
+It will be accessible [here](http://127.0.0.1:9999/)
 
-setup(**setup_kwargs)
```

