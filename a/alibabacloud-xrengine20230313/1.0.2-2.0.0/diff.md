# Comparing `tmp/alibabacloud_xrengine20230313-1.0.2.tar.gz` & `tmp/alibabacloud_xrengine20230313-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-1.0.2.tar", last modified: Thu Jul 27 08:06:14 2023, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.0.0.tar", last modified: Wed Aug  2 08:46:43 2023, max compression
```

## Comparing `alibabacloud_xrengine20230313-1.0.2.tar` & `alibabacloud_xrengine20230313-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62573 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   216135 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72515 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   245018 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-08-02 08:46:43.000000 alibabacloud_xrengine20230313-2.0.0/setup.py
```

### Comparing `alibabacloud_xrengine20230313-1.0.2/LICENSE` & `alibabacloud_xrengine20230313-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.2/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 1.0.2
+Version: 2.0.0
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.2/README-CN.md` & `alibabacloud_xrengine20230313-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.2/README.md` & `alibabacloud_xrengine20230313-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -855,14 +855,84 @@
     async def pop_build_object_project_async(
         self,
         request: xr_engine_20230313_models.PopBuildObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopBuildObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_build_object_project_with_options_async(request, runtime)
 
+    def pop_build_text_to_avatar_project_with_options(
+        self,
+        request: xr_engine_20230313_models.PopBuildTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.project_id):
+            body['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopBuildTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_build_text_to_avatar_project_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopBuildTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.project_id):
+            body['ProjectId'] = request.project_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopBuildTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_build_text_to_avatar_project(
+        self,
+        request: xr_engine_20230313_models.PopBuildTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_build_text_to_avatar_project_with_options(request, runtime)
+
+    async def pop_build_text_to_avatar_project_async(
+        self,
+        request: xr_engine_20230313_models.PopBuildTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopBuildTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_build_text_to_avatar_project_with_options_async(request, runtime)
+
     def pop_create_feature_to_avatar_project_with_options(
         self,
         request: xr_engine_20230313_models.PopCreateFeatureToAvatarProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopCreateFeatureToAvatarProjectResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1035,14 +1105,92 @@
     async def pop_create_object_project_async(
         self,
         request: xr_engine_20230313_models.PopCreateObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopCreateObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_create_object_project_with_options_async(request, runtime)
 
+    def pop_create_text_to_avatar_project_with_options(
+        self,
+        request: xr_engine_20230313_models.PopCreateTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.ext_info):
+            body['ExtInfo'] = request.ext_info
+        if not UtilClient.is_unset(request.intro):
+            body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopCreateTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_create_text_to_avatar_project_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopCreateTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.ext_info):
+            body['ExtInfo'] = request.ext_info
+        if not UtilClient.is_unset(request.intro):
+            body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopCreateTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_create_text_to_avatar_project(
+        self,
+        request: xr_engine_20230313_models.PopCreateTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_create_text_to_avatar_project_with_options(request, runtime)
+
+    async def pop_create_text_to_avatar_project_async(
+        self,
+        request: xr_engine_20230313_models.PopCreateTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopCreateTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_create_text_to_avatar_project_with_options_async(request, runtime)
+
     def pop_list_feature_to_avatar_materials_with_options(
         self,
         request: xr_engine_20230313_models.PopListFeatureToAvatarMaterialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopListFeatureToAvatarMaterialsResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1383,14 +1531,108 @@
     async def pop_list_object_project_async(
         self,
         request: xr_engine_20230313_models.PopListObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopListObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_list_object_project_with_options_async(request, runtime)
 
+    def pop_list_text_to_avatar_project_with_options(
+        self,
+        request: xr_engine_20230313_models.PopListTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            query['JwtToken'] = request.jwt_token
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        if not UtilClient.is_unset(request.sort_field):
+            body['SortField'] = request.sort_field
+        if not UtilClient.is_unset(request.status):
+            body['Status'] = request.status
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListTextToAvatarProjectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_list_text_to_avatar_project_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopListTextToAvatarProjectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListTextToAvatarProjectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            query['JwtToken'] = request.jwt_token
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        if not UtilClient.is_unset(request.sort_field):
+            body['SortField'] = request.sort_field
+        if not UtilClient.is_unset(request.status):
+            body['Status'] = request.status
+        if not UtilClient.is_unset(request.title):
+            body['Title'] = request.title
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListTextToAvatarProject',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListTextToAvatarProjectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_list_text_to_avatar_project(
+        self,
+        request: xr_engine_20230313_models.PopListTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopListTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_list_text_to_avatar_project_with_options(request, runtime)
+
+    async def pop_list_text_to_avatar_project_async(
+        self,
+        request: xr_engine_20230313_models.PopListTextToAvatarProjectRequest,
+    ) -> xr_engine_20230313_models.PopListTextToAvatarProjectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_list_text_to_avatar_project_with_options_async(request, runtime)
+
     def pop_object_project_detail_with_options(
         self,
         request: xr_engine_20230313_models.PopObjectProjectDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopObjectProjectDetailResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1642,14 +1642,130 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopBuildObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopBuildTextToAvatarProjectRequest(TeaModel):
+    def __init__(
+        self,
+        project_id: str = None,
+    ):
+        self.project_id = project_id
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
+        if self.project_id is not None:
+            result['ProjectId'] = self.project_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ProjectId') is not None:
+            self.project_id = m.get('ProjectId')
+        return self
+
+
+class PopBuildTextToAvatarProjectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopBuildTextToAvatarProjectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopBuildTextToAvatarProjectResponseBody = None,
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
+            temp_model = PopBuildTextToAvatarProjectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopCreateFeatureToAvatarProjectRequest(TeaModel):
     def __init__(
         self,
         ext_info: str = None,
         intro: str = None,
         title: str = None,
     ):
@@ -3049,14 +3165,261 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopCreateObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopCreateTextToAvatarProjectRequest(TeaModel):
+    def __init__(
+        self,
+        ext_info: str = None,
+        intro: str = None,
+        title: str = None,
+    ):
+        self.ext_info = ext_info
+        self.intro = intro
+        self.title = title
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
+        if self.ext_info is not None:
+            result['ExtInfo'] = self.ext_info
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExtInfo') is not None:
+            self.ext_info = m.get('ExtInfo')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class PopCreateTextToAvatarProjectResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        auto_build: bool = None,
+        biz_usage: str = None,
+        check_status: str = None,
+        create_mode: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        dependencies: str = None,
+        ext: str = None,
+        id: str = None,
+        intro: str = None,
+        material_cover_url: str = None,
+        modified_time: str = None,
+        status: str = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.auto_build = auto_build
+        self.biz_usage = biz_usage
+        self.check_status = check_status
+        self.create_mode = create_mode
+        self.create_time = create_time
+        self.deleted = deleted
+        self.dependencies = dependencies
+        self.ext = ext
+        self.id = id
+        self.intro = intro
+        self.material_cover_url = material_cover_url
+        self.modified_time = modified_time
+        self.status = status
+        self.title = title
+        self.type = type
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
+        if self.auto_build is not None:
+            result['AutoBuild'] = self.auto_build
+        if self.biz_usage is not None:
+            result['BizUsage'] = self.biz_usage
+        if self.check_status is not None:
+            result['CheckStatus'] = self.check_status
+        if self.create_mode is not None:
+            result['CreateMode'] = self.create_mode
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.dependencies is not None:
+            result['Dependencies'] = self.dependencies
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.material_cover_url is not None:
+            result['MaterialCoverUrl'] = self.material_cover_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoBuild') is not None:
+            self.auto_build = m.get('AutoBuild')
+        if m.get('BizUsage') is not None:
+            self.biz_usage = m.get('BizUsage')
+        if m.get('CheckStatus') is not None:
+            self.check_status = m.get('CheckStatus')
+        if m.get('CreateMode') is not None:
+            self.create_mode = m.get('CreateMode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('Dependencies') is not None:
+            self.dependencies = m.get('Dependencies')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('MaterialCoverUrl') is not None:
+            self.material_cover_url = m.get('MaterialCoverUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopCreateTextToAvatarProjectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: PopCreateTextToAvatarProjectResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = PopCreateTextToAvatarProjectResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopCreateTextToAvatarProjectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopCreateTextToAvatarProjectResponseBody = None,
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
+            temp_model = PopCreateTextToAvatarProjectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopListFeatureToAvatarMaterialsRequest(TeaModel):
     def __init__(
         self,
         current: int = None,
         list_status: str = None,
         size: int = None,
         tags: str = None,
@@ -3367,26 +3730,24 @@
     def __init__(
         self,
         completed_time: str = None,
         create_time: str = None,
         deleted: bool = None,
         error_message: str = None,
         estimated_duration: int = None,
-        id: int = None,
         modified_time: str = None,
         running_time: str = None,
         status: str = None,
         submit_time: str = None,
     ):
         self.completed_time = completed_time
         self.create_time = create_time
         self.deleted = deleted
         self.error_message = error_message
         self.estimated_duration = estimated_duration
-        self.id = id
         self.modified_time = modified_time
         self.running_time = running_time
         self.status = status
         self.submit_time = submit_time
 
     def validate(self):
         pass
@@ -3403,16 +3764,14 @@
             result['CreateTime'] = self.create_time
         if self.deleted is not None:
             result['Deleted'] = self.deleted
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.estimated_duration is not None:
             result['EstimatedDuration'] = self.estimated_duration
-        if self.id is not None:
-            result['Id'] = self.id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.running_time is not None:
             result['RunningTime'] = self.running_time
         if self.status is not None:
             result['Status'] = self.status
         if self.submit_time is not None:
@@ -3427,16 +3786,14 @@
             self.create_time = m.get('CreateTime')
         if m.get('Deleted') is not None:
             self.deleted = m.get('Deleted')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('EstimatedDuration') is not None:
             self.estimated_duration = m.get('EstimatedDuration')
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('RunningTime') is not None:
             self.running_time = m.get('RunningTime')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SubmitTime') is not None:
@@ -3507,15 +3864,14 @@
         build_result_url: Dict[str, Any] = None,
         cover_url: str = None,
         create_time: str = None,
         deleted: bool = None,
         error_code: str = None,
         error_message: str = None,
         glb_model_url: str = None,
-        id: int = None,
         model_url: str = None,
         modified_time: str = None,
         origin_result_url: str = None,
         oss_key: str = None,
         policy: PopListFeatureToAvatarProjectResponseBodyDataDatasetPolicy = None,
         pose_url: str = None,
         preview_url: str = None,
@@ -3523,15 +3879,14 @@
         self.build_result_url = build_result_url
         self.cover_url = cover_url
         self.create_time = create_time
         self.deleted = deleted
         self.error_code = error_code
         self.error_message = error_message
         self.glb_model_url = glb_model_url
-        self.id = id
         self.model_url = model_url
         self.modified_time = modified_time
         self.origin_result_url = origin_result_url
         self.oss_key = oss_key
         self.policy = policy
         self.pose_url = pose_url
         self.preview_url = preview_url
@@ -3556,16 +3911,14 @@
             result['Deleted'] = self.deleted
         if self.error_code is not None:
             result['ErrorCode'] = self.error_code
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.glb_model_url is not None:
             result['GlbModelUrl'] = self.glb_model_url
-        if self.id is not None:
-            result['Id'] = self.id
         if self.model_url is not None:
             result['ModelUrl'] = self.model_url
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.origin_result_url is not None:
             result['OriginResultUrl'] = self.origin_result_url
         if self.oss_key is not None:
@@ -3590,16 +3943,14 @@
             self.deleted = m.get('Deleted')
         if m.get('ErrorCode') is not None:
             self.error_code = m.get('ErrorCode')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('GlbModelUrl') is not None:
             self.glb_model_url = m.get('GlbModelUrl')
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
         if m.get('ModelUrl') is not None:
             self.model_url = m.get('ModelUrl')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('OriginResultUrl') is not None:
             self.origin_result_url = m.get('OriginResultUrl')
         if m.get('OssKey') is not None:
@@ -5541,14 +5892,529 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopListObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopListTextToAvatarProjectRequest(TeaModel):
+    def __init__(
+        self,
+        current: int = None,
+        jwt_token: str = None,
+        size: int = None,
+        sort_field: str = None,
+        status: str = None,
+        title: str = None,
+    ):
+        self.current = current
+        self.jwt_token = jwt_token
+        self.size = size
+        self.sort_field = sort_field
+        self.status = status
+        self.title = title
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
+        if self.current is not None:
+            result['Current'] = self.current
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        if self.size is not None:
+            result['Size'] = self.size
+        if self.sort_field is not None:
+            result['SortField'] = self.sort_field
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        if m.get('SortField') is not None:
+            self.sort_field = m.get('SortField')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        return self
+
+
+class PopListTextToAvatarProjectResponseBodyDataBuildDetail(TeaModel):
+    def __init__(
+        self,
+        completed_time: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_message: str = None,
+        estimated_duration: int = None,
+        modified_time: str = None,
+        running_time: str = None,
+        status: str = None,
+        submit_time: str = None,
+    ):
+        self.completed_time = completed_time
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_message = error_message
+        self.estimated_duration = estimated_duration
+        self.modified_time = modified_time
+        self.running_time = running_time
+        self.status = status
+        self.submit_time = submit_time
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
+        if self.completed_time is not None:
+            result['CompletedTime'] = self.completed_time
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.estimated_duration is not None:
+            result['EstimatedDuration'] = self.estimated_duration
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.running_time is not None:
+            result['RunningTime'] = self.running_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.submit_time is not None:
+            result['SubmitTime'] = self.submit_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CompletedTime') is not None:
+            self.completed_time = m.get('CompletedTime')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('EstimatedDuration') is not None:
+            self.estimated_duration = m.get('EstimatedDuration')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('RunningTime') is not None:
+            self.running_time = m.get('RunningTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SubmitTime') is not None:
+            self.submit_time = m.get('SubmitTime')
+        return self
+
+
+class PopListTextToAvatarProjectResponseBodyDataDatasetPolicy(TeaModel):
+    def __init__(
+        self,
+        access_id: str = None,
+        dir: str = None,
+        expire: str = None,
+        host: str = None,
+        policy: str = None,
+        signature: str = None,
+    ):
+        self.access_id = access_id
+        self.dir = dir
+        self.expire = expire
+        self.host = host
+        self.policy = policy
+        self.signature = signature
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
+        if self.access_id is not None:
+            result['AccessId'] = self.access_id
+        if self.dir is not None:
+            result['Dir'] = self.dir
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        if self.host is not None:
+            result['Host'] = self.host
+        if self.policy is not None:
+            result['Policy'] = self.policy
+        if self.signature is not None:
+            result['Signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessId') is not None:
+            self.access_id = m.get('AccessId')
+        if m.get('Dir') is not None:
+            self.dir = m.get('Dir')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
+        if m.get('Policy') is not None:
+            self.policy = m.get('Policy')
+        if m.get('Signature') is not None:
+            self.signature = m.get('Signature')
+        return self
+
+
+class PopListTextToAvatarProjectResponseBodyDataDataset(TeaModel):
+    def __init__(
+        self,
+        build_result_url: Dict[str, Any] = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_code: str = None,
+        error_message: str = None,
+        modified_time: str = None,
+        oss_key: str = None,
+        policy: PopListTextToAvatarProjectResponseBodyDataDatasetPolicy = None,
+    ):
+        self.build_result_url = build_result_url
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_code = error_code
+        self.error_message = error_message
+        self.modified_time = modified_time
+        self.oss_key = oss_key
+        self.policy = policy
+
+    def validate(self):
+        if self.policy:
+            self.policy.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.build_result_url is not None:
+            result['BuildResultUrl'] = self.build_result_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BuildResultUrl') is not None:
+            self.build_result_url = m.get('BuildResultUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('Policy') is not None:
+            temp_model = PopListTextToAvatarProjectResponseBodyDataDatasetPolicy()
+            self.policy = temp_model.from_map(m['Policy'])
+        return self
+
+
+class PopListTextToAvatarProjectResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        auto_build: bool = None,
+        biz_usage: str = None,
+        build_detail: PopListTextToAvatarProjectResponseBodyDataBuildDetail = None,
+        check_status: str = None,
+        create_mode: str = None,
+        create_time: str = None,
+        dataset: PopListTextToAvatarProjectResponseBodyDataDataset = None,
+        deleted: bool = None,
+        dependencies: str = None,
+        ext: str = None,
+        id: str = None,
+        intro: str = None,
+        material_cover_url: str = None,
+        modified_time: str = None,
+        status: str = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.auto_build = auto_build
+        self.biz_usage = biz_usage
+        self.build_detail = build_detail
+        self.check_status = check_status
+        self.create_mode = create_mode
+        self.create_time = create_time
+        self.dataset = dataset
+        self.deleted = deleted
+        self.dependencies = dependencies
+        self.ext = ext
+        self.id = id
+        self.intro = intro
+        self.material_cover_url = material_cover_url
+        self.modified_time = modified_time
+        self.status = status
+        self.title = title
+        self.type = type
+
+    def validate(self):
+        if self.build_detail:
+            self.build_detail.validate()
+        if self.dataset:
+            self.dataset.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_build is not None:
+            result['AutoBuild'] = self.auto_build
+        if self.biz_usage is not None:
+            result['BizUsage'] = self.biz_usage
+        if self.build_detail is not None:
+            result['BuildDetail'] = self.build_detail.to_map()
+        if self.check_status is not None:
+            result['CheckStatus'] = self.check_status
+        if self.create_mode is not None:
+            result['CreateMode'] = self.create_mode
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.dataset is not None:
+            result['Dataset'] = self.dataset.to_map()
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.dependencies is not None:
+            result['Dependencies'] = self.dependencies
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.material_cover_url is not None:
+            result['MaterialCoverUrl'] = self.material_cover_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoBuild') is not None:
+            self.auto_build = m.get('AutoBuild')
+        if m.get('BizUsage') is not None:
+            self.biz_usage = m.get('BizUsage')
+        if m.get('BuildDetail') is not None:
+            temp_model = PopListTextToAvatarProjectResponseBodyDataBuildDetail()
+            self.build_detail = temp_model.from_map(m['BuildDetail'])
+        if m.get('CheckStatus') is not None:
+            self.check_status = m.get('CheckStatus')
+        if m.get('CreateMode') is not None:
+            self.create_mode = m.get('CreateMode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Dataset') is not None:
+            temp_model = PopListTextToAvatarProjectResponseBodyDataDataset()
+            self.dataset = temp_model.from_map(m['Dataset'])
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('Dependencies') is not None:
+            self.dependencies = m.get('Dependencies')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('MaterialCoverUrl') is not None:
+            self.material_cover_url = m.get('MaterialCoverUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopListTextToAvatarProjectResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        current: int = None,
+        data: List[PopListTextToAvatarProjectResponseBodyData] = None,
+        message: str = None,
+        pages: int = None,
+        request_id: str = None,
+        size: int = None,
+        success: bool = None,
+        total: int = None,
+    ):
+        self.code = code
+        self.current = current
+        self.data = data
+        self.message = message
+        self.pages = pages
+        self.request_id = request_id
+        self.size = size
+        self.success = success
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.current is not None:
+            result['Current'] = self.current
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.pages is not None:
+            result['Pages'] = self.pages
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.size is not None:
+            result['Size'] = self.size
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = PopListTextToAvatarProjectResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Pages') is not None:
+            self.pages = m.get('Pages')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class PopListTextToAvatarProjectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopListTextToAvatarProjectResponseBody = None,
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
+            temp_model = PopListTextToAvatarProjectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopObjectProjectDetailRequest(TeaModel):
     def __init__(
         self,
         jwt_token: str = None,
         project_id: str = None,
     ):
         self.jwt_token = jwt_token
```

### Comparing `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 1.0.2
+Version: 2.0.0
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.2/setup.py` & `alibabacloud_xrengine20230313-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 27/07/2023
+Created on 02/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
```

