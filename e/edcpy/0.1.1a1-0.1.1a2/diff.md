# Comparing `tmp/edcpy-0.1.1a1.tar.gz` & `tmp/edcpy-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edcpy-0.1.1a1.tar", max compression
+gzip compressed data, was "edcpy-0.1.1a2.tar", max compression
```

## Comparing `edcpy-0.1.1a1.tar` & `edcpy-0.1.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      113 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/README.md
--rw-r--r--   0        0        0        0 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/__init__.py
--rw-r--r--   0        0        0     5959 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/backend.py
--rw-r--r--   0        0        0     5233 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/config.py
--rw-r--r--   0        0        0    10682 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/keycloak.py
--rw-r--r--   0        0        0     4076 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/messaging.py
--rw-r--r--   0        0        0        0 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/__init__.py
--rw-r--r--   0        0        0     1511 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/asset.py
--rw-r--r--   0        0        0      713 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/contract_definition.py
--rw-r--r--   0        0        0     1454 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/contract_negotiation.py
--rw-r--r--   0        0        0      803 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/data_plane_instance.py
--rw-r--r--   0        0        0      627 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/policy_definition.py
--rw-r--r--   0        0        0     2008 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/models/transfer_process.py
--rw-r--r--   0        0        0    11828 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/orchestrator.py
--rw-r--r--   0        0        0      245 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/edcpy/utils.py
--rw-r--r--   0        0        0      978 2023-07-17 09:18:49.886621 edcpy-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 edcpy-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-08-02 12:23:36.112810 edcpy-0.1.1a2/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 12:23:36.112810 edcpy-0.1.1a2/edcpy/__init__.py
+-rw-r--r--   0        0        0     5959 2023-08-02 12:23:36.112810 edcpy-0.1.1a2/edcpy/backend.py
+-rw-r--r--   0        0        0     5233 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/config.py
+-rw-r--r--   0        0        0    10682 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/keycloak.py
+-rw-r--r--   0        0        0     4076 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/messaging.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/__init__.py
+-rw-r--r--   0        0        0     1511 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/asset.py
+-rw-r--r--   0        0        0      713 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/contract_definition.py
+-rw-r--r--   0        0        0     1454 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/contract_negotiation.py
+-rw-r--r--   0        0        0      803 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/data_plane_instance.py
+-rw-r--r--   0        0        0      627 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/policy_definition.py
+-rw-r--r--   0        0        0     2008 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/models/transfer_process.py
+-rw-r--r--   0        0        0    12166 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/orchestrator.py
+-rw-r--r--   0        0        0      245 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/edcpy/utils.py
+-rw-r--r--   0        0        0      978 2023-08-02 12:23:36.116810 edcpy-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 edcpy-0.1.1a2/PKG-INFO
```

### Comparing `edcpy-0.1.1a1/edcpy/backend.py` & `edcpy-0.1.1a2/edcpy/backend.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/config.py` & `edcpy-0.1.1a2/edcpy/config.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/keycloak.py` & `edcpy-0.1.1a2/edcpy/keycloak.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/messaging.py` & `edcpy-0.1.1a2/edcpy/messaging.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/asset.py` & `edcpy-0.1.1a2/edcpy/models/asset.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/contract_definition.py` & `edcpy-0.1.1a2/edcpy/models/contract_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/contract_negotiation.py` & `edcpy-0.1.1a2/edcpy/models/contract_negotiation.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/data_plane_instance.py` & `edcpy-0.1.1a2/edcpy/models/data_plane_instance.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/policy_definition.py` & `edcpy-0.1.1a2/edcpy/models/policy_definition.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/models/transfer_process.py` & `edcpy-0.1.1a2/edcpy/models/transfer_process.py`

 * *Files identical despite different names*

### Comparing `edcpy-0.1.1a1/edcpy/orchestrator.py` & `edcpy-0.1.1a2/edcpy/orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
 import logging
 import pprint
-import time
 from dataclasses import dataclass
 from typing import Iterator, Union
 
 import httpx
 
 from edcpy.config import ConsumerProviderPairConfig
 from edcpy.models.asset import Asset
 from edcpy.models.contract_definition import ContractDefinition
 from edcpy.models.contract_negotiation import ContractNegotiation
 from edcpy.models.data_plane_instance import DataPlaneInstance
 from edcpy.models.policy_definition import PolicyDefinition
 from edcpy.models.transfer_process import TransferProcess
 from edcpy.utils import join_url
 
+_DEFAULT_TIMEOUT_SECS = 60
+
 _logger = logging.getLogger(__name__)
 
 
 def _log_req(method, url, data=None):
     _logger.debug("-> %s %s\n%s", method, url, pprint.pformat(data) if data else "")
 
 
@@ -89,15 +90,15 @@
     async def fetch_provider_catalog_from_consumer(self) -> dict:
         data = {
             "@context": {"edc": "https://w3id.org/edc/v0.0.1/ns/"},
             "providerUrl": self.config.provider_protocol_url,
             "protocol": "dataspace-protocol-http",
         }
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(self.config.consumer_management_url, "v2/catalog/request")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
             _log_res("POST", url, resp_json)
 
         return resp_json
@@ -105,15 +106,15 @@
     async def _register_data_plane(
         self, management_url, control_url, public_api_url
     ) -> dict:
         data = DataPlaneInstance.build(
             control_url=control_url, public_api_url=public_api_url
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(management_url, "instances")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             response.raise_for_status()
 
         return data
 
@@ -141,41 +142,41 @@
         data = Asset.build_http_data(
             source_base_url=base_url,
             source_path=path,
             source_method=method,
             source_content_type=content_type,
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(self.config.provider_management_url, "v2/assets")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
             _log_res("POST", url, resp_json)
 
         return resp_json
 
     async def create_provider_policy_definition(self) -> dict:
         data = PolicyDefinition.build()
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(self.config.provider_management_url, "v2/policydefinitions")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
             _log_res("POST", url, resp_json)
 
         return resp_json
 
     async def create_provider_contract_definition(
         self, policy_definition_id: str
     ) -> dict:
         data = ContractDefinition.build(policy_definition_id=policy_definition_id)
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(
                 self.config.provider_management_url, "v2/contractdefinitions"
             )
 
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
@@ -191,15 +192,15 @@
             connector_ids_url=self.config.provider_protocol_url,
             consumer_id=self.config.consumer_participant_id,
             provider_id=self.config.provider_participant_id,
             offer_id=offer_id,
             asset_id=asset_id,
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(
                 self.config.consumer_management_url, "v2/contractnegotiations"
             )
 
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
@@ -211,15 +212,15 @@
         self, contract_negotiation_id: str, iter_sleep: float = 1.0
     ) -> str:
         url = join_url(
             self.config.consumer_management_url,
             f"v2/contractnegotiations/{contract_negotiation_id}",
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             while True:
                 _log_req("GET", url)
                 response = await client.get(url, headers=self.DEFAULT_HEADERS)
                 resp_json = response.json()
                 _log_res("GET", url, resp_json)
 
                 agreement_id = resp_json.get("edc:contractAgreementId")
@@ -247,15 +248,15 @@
             asset_id=asset_id,
             sink_base_url=sink_base_url,
             sink_path=sink_path,
             sink_method=sink_method,
             sink_content_type=sink_content_type,
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(self.config.consumer_management_url, "v2/transferprocesses")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
             _log_res("POST", url, resp_json)
 
         return resp_json
@@ -266,15 +267,15 @@
         data = TransferProcess.build_for_consumer_http_pull(
             connector_id=self.config.provider_connector_id,
             connector_ids_url=self.config.provider_protocol_url,
             contract_agreement_id=contract_agreement_id,
             asset_id=asset_id,
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             url = join_url(self.config.consumer_management_url, "v2/transferprocesses")
             _log_req("POST", url, data)
             response = await client.post(url, headers=self.DEFAULT_HEADERS, json=data)
             resp_json = response.json()
             _log_res("POST", url, resp_json)
 
         return resp_json
@@ -283,15 +284,15 @@
         self, transfer_process_id: str, iter_sleep: float = 1.0
     ) -> None:
         url = join_url(
             self.config.consumer_management_url,
             f"v2/transferprocesses/{transfer_process_id}",
         )
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(timeout=_DEFAULT_TIMEOUT_SECS) as client:
             while True:
                 _log_req("GET", url)
                 response = await client.get(url, headers=self.DEFAULT_HEADERS)
                 resp_json = response.json()
                 _log_res("GET", url, resp_json)
 
                 if resp_json.get("edc:state") == "COMPLETED":
@@ -304,15 +305,18 @@
         self, asset_query: Union[str, None]
     ) -> TransferProcessDetails:
         _logger.info("Preparing to transfer asset (query: %s)", asset_query)
 
         catalog = await self.fetch_provider_catalog_from_consumer()
         catalog_content = CatalogContent(data=catalog)
         dataset_dict = catalog_content.find_one_dataset(asset_query)
-        assert dataset_dict, f"Dataset not found for query: {asset_query}"
+
+        if not dataset_dict:
+            raise ValueError(f"Dataset not found for query: {asset_query}")
+
         _logger.debug("Selected dataset:\n%s", pprint.pformat(dataset_dict))
         dataset = CatalogDataset(data=dataset_dict)
         contract_offer_id = dataset.default_contract_offer_id
         _logger.debug(f"Contract Offer ID: {contract_offer_id}")
         asset_id = dataset.default_asset_id
         _logger.debug(f"Asset ID: {asset_id}")
```

### Comparing `edcpy-0.1.1a1/pyproject.toml` & `edcpy-0.1.1a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edcpy"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector"
 authors = ["Andres Garcia Mangas <andres.garcia@fundacionctic.org>"]
 license = "EUPL-1.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `edcpy-0.1.1a1/PKG-INFO` & `edcpy-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edcpy
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Package that provides a series of utilities to facilitate interaction with the Management and Control APIs of an EDC connector
 License: EUPL-1.2
 Author: Andres Garcia Mangas
 Author-email: andres.garcia@fundacionctic.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

