# Comparing `tmp/alibabacloud_gpdb20160503-2.0.1.tar.gz` & `tmp/alibabacloud_gpdb20160503-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.1.tar", last modified: Wed Jul 26 06:51:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.2.tar", last modified: Wed Aug  2 02:10:31 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503-2.0.1.tar` & `alibabacloud_gpdb20160503-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   506126 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   738237 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2637 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   509950 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   743266 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/setup.py
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/ChangeLog.md` & `alibabacloud_gpdb20160503-2.0.2/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-26 Version: 2.0.1
+- Add Cloud Disk Encryption.
+
 2023-07-10 Version: 2.0.0
 - Add Cloud Disk Encryption.
 
 2023-01-09 Version: 1.1.21
 - Support Pause and Resume Instance.
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/LICENSE` & `alibabacloud_gpdb20160503-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.1/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/README-CN.md` & `alibabacloud_gpdb20160503-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.1/README.md` & `alibabacloud_gpdb20160503-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/client.py` & `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3359,14 +3359,16 @@
     def describe_dbinstance_net_info_with_options(
         self,
         request: gpdb_20160503_models.DescribeDBInstanceNetInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> gpdb_20160503_models.DescribeDBInstanceNetInfoResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.connection_string):
+            query['ConnectionString'] = request.connection_string
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBInstanceNetInfo',
@@ -3387,14 +3389,16 @@
     async def describe_dbinstance_net_info_with_options_async(
         self,
         request: gpdb_20160503_models.DescribeDBInstanceNetInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> gpdb_20160503_models.DescribeDBInstanceNetInfoResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.connection_string):
+            query['ConnectionString'] = request.connection_string
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBInstanceNetInfo',
@@ -7050,14 +7054,100 @@
     async def grant_collection_async(
         self,
         request: gpdb_20160503_models.GrantCollectionRequest,
     ) -> gpdb_20160503_models.GrantCollectionResponse:
         runtime = util_models.RuntimeOptions()
         return await self.grant_collection_with_options_async(request, runtime)
 
+    def init_vector_database_with_options(
+        self,
+        request: gpdb_20160503_models.InitVectorDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> gpdb_20160503_models.InitVectorDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dbinstance_id):
+            query['DBInstanceId'] = request.dbinstance_id
+        if not UtilClient.is_unset(request.manager_account):
+            query['ManagerAccount'] = request.manager_account
+        if not UtilClient.is_unset(request.manager_account_password):
+            query['ManagerAccountPassword'] = request.manager_account_password
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='InitVectorDatabase',
+            version='2016-05-03',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            gpdb_20160503_models.InitVectorDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def init_vector_database_with_options_async(
+        self,
+        request: gpdb_20160503_models.InitVectorDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> gpdb_20160503_models.InitVectorDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dbinstance_id):
+            query['DBInstanceId'] = request.dbinstance_id
+        if not UtilClient.is_unset(request.manager_account):
+            query['ManagerAccount'] = request.manager_account
+        if not UtilClient.is_unset(request.manager_account_password):
+            query['ManagerAccountPassword'] = request.manager_account_password
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='InitVectorDatabase',
+            version='2016-05-03',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            gpdb_20160503_models.InitVectorDatabaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def init_vector_database(
+        self,
+        request: gpdb_20160503_models.InitVectorDatabaseRequest,
+    ) -> gpdb_20160503_models.InitVectorDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.init_vector_database_with_options(request, runtime)
+
+    async def init_vector_database_async(
+        self,
+        request: gpdb_20160503_models.InitVectorDatabaseRequest,
+    ) -> gpdb_20160503_models.InitVectorDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.init_vector_database_with_options_async(request, runtime)
+
     def list_collections_with_options(
         self,
         request: gpdb_20160503_models.ListCollectionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> gpdb_20160503_models.ListCollectionsResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/models.py` & `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6597,36 +6597,42 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDBInstanceNetInfoRequest(TeaModel):
     def __init__(
         self,
+        connection_string: str = None,
         dbinstance_id: str = None,
     ):
+        self.connection_string = connection_string
         # The ID of the instance.
         # 
         # >  You can call the [DescribeDBInstances](~~86911~~) operation to query details about all AnalyticDB for PostgreSQL instances in a specific region, including instance IDs.
         self.dbinstance_id = dbinstance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.connection_string is not None:
+            result['ConnectionString'] = self.connection_string
         if self.dbinstance_id is not None:
             result['DBInstanceId'] = self.dbinstance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('ConnectionString') is not None:
+            self.connection_string = m.get('ConnectionString')
         if m.get('DBInstanceId') is not None:
             self.dbinstance_id = m.get('DBInstanceId')
         return self
 
 
 class DescribeDBInstanceNetInfoResponseBodyDBInstanceNetInfosDBInstanceNetInfo(TeaModel):
     def __init__(
@@ -15561,14 +15567,148 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GrantCollectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class InitVectorDatabaseRequest(TeaModel):
+    def __init__(
+        self,
+        dbinstance_id: str = None,
+        manager_account: str = None,
+        manager_account_password: str = None,
+        owner_id: int = None,
+        region_id: str = None,
+    ):
+        self.dbinstance_id = dbinstance_id
+        self.manager_account = manager_account
+        self.manager_account_password = manager_account_password
+        self.owner_id = owner_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dbinstance_id is not None:
+            result['DBInstanceId'] = self.dbinstance_id
+        if self.manager_account is not None:
+            result['ManagerAccount'] = self.manager_account
+        if self.manager_account_password is not None:
+            result['ManagerAccountPassword'] = self.manager_account_password
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DBInstanceId') is not None:
+            self.dbinstance_id = m.get('DBInstanceId')
+        if m.get('ManagerAccount') is not None:
+            self.manager_account = m.get('ManagerAccount')
+        if m.get('ManagerAccountPassword') is not None:
+            self.manager_account_password = m.get('ManagerAccountPassword')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class InitVectorDatabaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        message: str = None,
+        request_id: str = None,
+        status: str = None,
+    ):
+        self.message = message
+        self.request_id = request_id
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class InitVectorDatabaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: InitVectorDatabaseResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = InitVectorDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListCollectionsRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         namespace: str = None,
         namespace_password: str = None,
         owner_id: int = None,
@@ -18148,18 +18288,20 @@
 
 
 class QueryCollectionDataResponseBodyMatchesMatch(TeaModel):
     def __init__(
         self,
         id: str = None,
         metadata: Dict[str, str] = None,
+        similarity: float = None,
         values: QueryCollectionDataResponseBodyMatchesMatchValues = None,
     ):
         self.id = id
         self.metadata = metadata
+        self.similarity = similarity
         self.values = values
 
     def validate(self):
         if self.values:
             self.values.validate()
 
     def to_map(self):
@@ -18168,24 +18310,28 @@
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.metadata is not None:
             result['Metadata'] = self.metadata
+        if self.similarity is not None:
+            result['Similarity'] = self.similarity
         if self.values is not None:
             result['Values'] = self.values.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Metadata') is not None:
             self.metadata = m.get('Metadata')
+        if m.get('Similarity') is not None:
+            self.similarity = m.get('Similarity')
         if m.get('Values') is not None:
             temp_model = QueryCollectionDataResponseBodyMatchesMatchValues()
             self.values = temp_model.from_map(m['Values'])
         return self
 
 
 class QueryCollectionDataResponseBodyMatches(TeaModel):
@@ -18223,18 +18369,20 @@
         return self
 
 
 class QueryCollectionDataResponseBody(TeaModel):
     def __init__(
         self,
         matches: QueryCollectionDataResponseBodyMatches = None,
+        message: str = None,
         request_id: str = None,
         status: str = None,
     ):
         self.matches = matches
+        self.message = message
         self.request_id = request_id
         self.status = status
 
     def validate(self):
         if self.matches:
             self.matches.validate()
 
@@ -18242,25 +18390,29 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.matches is not None:
             result['Matches'] = self.matches.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Matches') is not None:
             temp_model = QueryCollectionDataResponseBodyMatches()
             self.matches = temp_model.from_map(m['Matches'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.1/setup.py` & `alibabacloud_gpdb20160503-2.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503.
 
-Created on 26/07/2023
+Created on 02/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python"
```

