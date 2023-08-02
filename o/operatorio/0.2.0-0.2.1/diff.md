# Comparing `tmp/operatorio-0.2.0.tar.gz` & `tmp/operatorio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.2.0.tar", last modified: Wed Aug  2 15:20:32 2023, max compression
+gzip compressed data, was "operatorio-0.2.1.tar", last modified: Wed Aug  2 15:30:41 2023, max compression
```

## Comparing `operatorio-0.2.0.tar` & `operatorio-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.049281 operatorio-0.2.0/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:20:32.049023 operatorio-0.2.0/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.047032 operatorio-0.2.0/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.2.0/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2498 2023-08-02 15:19:17.000000 operatorio-0.2.0/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:20:32.048209 operatorio-0.2.0/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-08-02 15:20:32.000000 operatorio-0.2.0/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-08-02 15:20:31.000000 operatorio-0.2.0/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-08-02 15:20:32.049347 operatorio-0.2.0/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-08-02 15:20:16.000000 operatorio-0.2.0/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.774871 operatorio-0.2.1/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:30:41.774638 operatorio-0.2.1/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.772803 operatorio-0.2.1/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.2.1/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2635 2023-08-02 15:30:28.000000 operatorio-0.2.1/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.774385 operatorio-0.2.1/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-08-02 15:30:41.774936 operatorio-0.2.1/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-08-02 15:30:33.000000 operatorio-0.2.1/setup.py
```

### Comparing `operatorio-0.2.0/operatorio/main.py` & `operatorio-0.2.1/operatorio/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 from dataclasses import dataclass, asdict
 from enum import Enum
-from typing import List, Dict, Union
+from typing import List, Dict, Any, Union
 
 # Models
 class EntityType(Enum):
     identity = "identity"
     nft = "nft"
     token = "token"
 
@@ -16,15 +16,20 @@
     semantic_similarity: float
     network_value: float = 0.0
     rank: float = 0.0
 
 @dataclass
 class AddressMatch:
     address: str
-    metadata: Dict[str, any]
+    metadata: Dict[str, Any]
+
+@dataclass
+class Addresses:
+    query: str
+    matches: List[Address]
 
 @dataclass
 class DescribeInput:
     address: str
     blockchain: str
 
 @dataclass
@@ -63,24 +68,25 @@
 
 class OperatorSearchAPI:
     BASE_URL = 'https://api.operator.io/'
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
-    def search(self, query: Query) -> Dict[str, any]:
+    def search(self, query: Query) -> Addresses:
         headers = {"X-API-Key": self.api_key}
         response = requests.post(
             self.BASE_URL + 'search/',
             headers=headers,
             json=query.to_dict()
         )
         
         if response.status_code == 200:
-            return response.json()
+            data = response.json()
+            return Addresses(query=data['query'], matches=[Address(**address) for address in data['matches']])
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
 
     def describe(self, describe_input: DescribeInput) -> DescribeOutput:
         headers = {"X-API-Key": self.api_key}
@@ -88,12 +94,12 @@
             self.BASE_URL + 'describe/',
             headers=headers,
             json=asdict(describe_input)
         )
 
         if response.status_code == 200:
             data = response.json()
-            return DescribeOutput(matches=[AddressMatch(address=match['address'], metadata=match['metadata']) for match in data['matches']])
+            return DescribeOutput(matches=[AddressMatch(**match) for match in data['matches']])
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
```

### Comparing `operatorio-0.2.0/setup.py` & `operatorio-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.2.0",
+    version="0.2.1",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

