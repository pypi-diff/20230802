# Comparing `tmp/operatorio-0.1.9.tar.gz` & `tmp/operatorio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.9.tar", last modified: Tue Aug  1 07:29:05 2023, max compression
+gzip compressed data, was "operatorio-0.2.0.tar", last modified: Wed Aug  2 15:20:32 2023, max compression
```

## Comparing `operatorio-0.1.9.tar` & `operatorio-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.599061 operatorio-0.1.9/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-01 07:29:05.598834 operatorio-0.1.9/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.597161 operatorio-0.1.9/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.9/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2536 2023-08-01 07:28:32.000000 operatorio-0.1.9/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.598561 operatorio-0.1.9/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-08-01 07:29:05.599146 operatorio-0.1.9/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-08-01 07:29:04.000000 operatorio-0.1.9/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.049281 operatorio-0.2.0/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:20:32.049023 operatorio-0.2.0/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.047032 operatorio-0.2.0/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.2.0/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2498 2023-08-02 15:19:17.000000 operatorio-0.2.0/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.048209 operatorio-0.2.0/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-08-02 15:20:32.000000 operatorio-0.2.0/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-08-02 15:20:32.049347 operatorio-0.2.0/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-08-02 15:20:16.000000 operatorio-0.2.0/setup.py
```

### Comparing `operatorio-0.1.9/operatorio/main.py` & `operatorio-0.2.0/operatorio/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 from dataclasses import dataclass, asdict
 from enum import Enum
-from typing import List, Dict, Optional
-from requests.models import PreparedRequest
+from typing import List, Dict, Union
 
 # Models
 class EntityType(Enum):
     identity = "identity"
     nft = "nft"
     token = "token"
 
@@ -36,15 +35,15 @@
 class Query:
     query: str
     blockchain: str
     entity_type: EntityType
     query_by: List[str]
 
     def to_dict(self):
-        return {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self).items()}
+        return {k: (v.value if isinstance(v, Enum) else v) for k, v in asdict(self).items()}
 
 @dataclass
 class ValidationError:
     loc: List[Union[str, int]]
     msg: str
     type: str
 
@@ -89,13 +88,12 @@
             self.BASE_URL + 'describe/',
             headers=headers,
             json=asdict(describe_input)
         )
 
         if response.status_code == 200:
             data = response.json()
-            matches = [AddressMatch(**match) for match in data.get('matches', [])]
-            return DescribeOutput(matches=matches)
+            return DescribeOutput(matches=[AddressMatch(address=match['address'], metadata=match['metadata']) for match in data['matches']])
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
```

### Comparing `operatorio-0.1.9/setup.py` & `operatorio-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.9",
+    version="0.2.0",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

