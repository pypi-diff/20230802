# Comparing `tmp/ampapi-1.1.4.tar.gz` & `tmp/ampapi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.1.4.tar", last modified: Thu May 18 02:20:21 2023, max compression
+gzip compressed data, was "ampapi-1.1.5.tar", last modified: Wed Aug  2 21:07:52 2023, max compression
```

## Comparing `ampapi-1.1.4.tar` & `ampapi-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.950864 ampapi-1.1.4/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-05-18 02:15:32.000000 ampapi-1.1.4/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-18 02:20:21.950864 ampapi-1.1.4/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3610 2023-05-18 02:15:32.000000 ampapi-1.1.4/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.946864 ampapi-1.1.4/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:15:32.000000 ampapi-1.1.4/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)   160593 2023-05-18 02:20:09.000000 ampapi-1.1.4/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.950864 ampapi-1.1.4/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-05-18 02:15:32.000000 ampapi-1.1.4/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-05-18 02:20:21.950864 ampapi-1.1.4/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-08-02 21:07:52.898737 ampapi-1.1.5/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-07-15 02:08:27.000000 ampapi-1.1.5/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-08-02 21:07:52.898737 ampapi-1.1.5/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3610 2023-07-15 02:08:27.000000 ampapi-1.1.5/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-08-02 21:07:52.898737 ampapi-1.1.5/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-07-15 02:08:27.000000 ampapi-1.1.5/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)   161853 2023-08-02 21:07:38.000000 ampapi-1.1.5/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-08-02 21:07:52.898737 ampapi-1.1.5/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-08-02 21:07:52.000000 ampapi-1.1.5/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-08-02 21:07:52.000000 ampapi-1.1.5/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-08-02 21:07:52.000000 ampapi-1.1.5/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-08-02 21:07:52.000000 ampapi-1.1.5/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-07-15 02:08:27.000000 ampapi-1.1.5/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-08-02 21:07:52.898737 ampapi-1.1.5/setup.cfg
```

### Comparing `ampapi-1.1.4/LICENCE` & `ampapi-1.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.4/PKG-INFO` & `ampapi-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.4/README.md` & `ampapi-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.4/ampapi/ampapi.py` & `ampapi-1.1.5/ampapi/ampapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,26 +91,26 @@
         return await self.APICallAsync(endpoint="ADSModule/AddDatastore", data={
             "newDatastore": newDatastore, 
         })
 
     def ADSModule_DeleteDatastore(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/DeleteDatastore", data={
             "id": id, 
         })
 
     async def ADSModule_DeleteDatastoreAsync(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/DeleteDatastore", data={
             "id": id, 
         })
 
@@ -147,123 +147,123 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="ADSModule/GetDatastores")
 
     def ADSModule_RequestDatastoreSizeCalculation(self, datastoreId: int):
         """
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="ADSModule/RequestDatastoreSizeCalculation", data={
             "datastoreId": datastoreId, 
         })
 
     async def ADSModule_RequestDatastoreSizeCalculationAsync(self, datastoreId: int):
         """
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="ADSModule/RequestDatastoreSizeCalculation", data={
             "datastoreId": datastoreId, 
         })
 
     def ADSModule_GetDatastore(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: InstanceDatastore
         """
         return self.APICall(endpoint="ADSModule/GetDatastore", data={
             "id": id, 
         })
 
     async def ADSModule_GetDatastoreAsync(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: InstanceDatastore
         """
         return await self.APICallAsync(endpoint="ADSModule/GetDatastore", data={
             "id": id, 
         })
 
     def ADSModule_RepairDatastore(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="ADSModule/RepairDatastore", data={
             "id": id, 
         })
 
     async def ADSModule_RepairDatastoreAsync(self, id: int):
         """
         :param id: 
-        :type id: intFalse
+        :type id: int False
             AMP Type: Int32
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="ADSModule/RepairDatastore", data={
             "id": id, 
         })
 
     def ADSModule_GetDatastoreInstances(self, datastoreId: int):
         """
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return self.APICall(endpoint="ADSModule/GetDatastoreInstances", data={
             "datastoreId": datastoreId, 
         })
 
     async def ADSModule_GetDatastoreInstancesAsync(self, datastoreId: int):
         """
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="ADSModule/GetDatastoreInstances", data={
             "datastoreId": datastoreId, 
         })
 
     def ADSModule_MoveInstanceDatastore(self, instanceId: str, datastoreId: int):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: Task<RunningTask>
         """
         return self.APICall(endpoint="ADSModule/MoveInstanceDatastore", data={
             "instanceId": instanceId, 
             "datastoreId": datastoreId, 
         })
 
     async def ADSModule_MoveInstanceDatastoreAsync(self, instanceId: str, datastoreId: int):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :param datastoreId: 
-        :type datastoreId: intFalse
+        :type datastoreId: int False
             AMP Type: Int32
         :returns: AMP Type: Task<RunningTask>
         """
         return await self.APICallAsync(endpoint="ADSModule/MoveInstanceDatastore", data={
             "instanceId": instanceId, 
             "datastoreId": datastoreId, 
         })
@@ -281,26 +281,26 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="ADSModule/GetDeploymentTemplates")
 
     def ADSModule_CreateDeploymentTemplate(self, Name: str):
         """
         :param Name: 
-        :type Name: strFalse
+        :type Name: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/CreateDeploymentTemplate", data={
             "Name": Name, 
         })
 
     async def ADSModule_CreateDeploymentTemplateAsync(self, Name: str):
         """
         :param Name: 
-        :type Name: strFalse
+        :type Name: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/CreateDeploymentTemplate", data={
             "Name": Name, 
         })
 
@@ -323,80 +323,80 @@
         return await self.APICallAsync(endpoint="ADSModule/UpdateDeploymentTemplate", data={
             "templateToUpdate": templateToUpdate, 
         })
 
     def ADSModule_DeleteDeploymentTemplate(self, Id: int):
         """
         :param Id: 
-        :type Id: intFalse
+        :type Id: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/DeleteDeploymentTemplate", data={
             "Id": Id, 
         })
 
     async def ADSModule_DeleteDeploymentTemplateAsync(self, Id: int):
         """
         :param Id: 
-        :type Id: intFalse
+        :type Id: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/DeleteDeploymentTemplate", data={
             "Id": Id, 
         })
 
     def ADSModule_CloneTemplate(self, Id: int, NewName: str):
         """
         :param Id: 
-        :type Id: intFalse
+        :type Id: int False
             AMP Type: Int32
         :param NewName: 
-        :type NewName: strFalse
+        :type NewName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/CloneTemplate", data={
             "Id": Id, 
             "NewName": NewName, 
         })
 
     async def ADSModule_CloneTemplateAsync(self, Id: int, NewName: str):
         """
         :param Id: 
-        :type Id: intFalse
+        :type Id: int False
             AMP Type: Int32
         :param NewName: 
-        :type NewName: strFalse
+        :type NewName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/CloneTemplate", data={
             "Id": Id, 
             "NewName": NewName, 
         })
 
     def ADSModule_ApplyTemplate(self, InstanceID: str, TemplateID: int, NewFriendlyName: str, Secret: str, RestartIfPreviouslyRunning: bool):
         """Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.
             
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :param TemplateID: 
-        :type TemplateID: intFalse
+        :type TemplateID: int False
             AMP Type: Int32
         :param NewFriendlyName: 
-        :type NewFriendlyName: strTrue
+        :type NewFriendlyName: str True
             AMP Type: String
         :param Secret: 
-        :type Secret: strTrue
+        :type Secret: str True
             AMP Type: String
         :param RestartIfPreviouslyRunning: 
-        :type RestartIfPreviouslyRunning: boolTrue
+        :type RestartIfPreviouslyRunning: bool True
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/ApplyTemplate", data={
             "InstanceID": InstanceID, 
             "TemplateID": TemplateID, 
             "NewFriendlyName": NewFriendlyName, 
@@ -404,68 +404,68 @@
             "RestartIfPreviouslyRunning": RestartIfPreviouslyRunning, 
         })
 
     async def ADSModule_ApplyTemplateAsync(self, InstanceID: str, TemplateID: int, NewFriendlyName: str, Secret: str, RestartIfPreviouslyRunning: bool):
         """Overlays an existing template on an existing instance. Used to perform package reconfigurations. Do not use this to 'transform' an existing application into another. The instance should be deleted and re-created in that situation.
             
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :param TemplateID: 
-        :type TemplateID: intFalse
+        :type TemplateID: int False
             AMP Type: Int32
         :param NewFriendlyName: 
-        :type NewFriendlyName: strTrue
+        :type NewFriendlyName: str True
             AMP Type: String
         :param Secret: 
-        :type Secret: strTrue
+        :type Secret: str True
             AMP Type: String
         :param RestartIfPreviouslyRunning: 
-        :type RestartIfPreviouslyRunning: boolTrue
+        :type RestartIfPreviouslyRunning: bool True
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/ApplyTemplate", data={
             "InstanceID": InstanceID, 
             "TemplateID": TemplateID, 
             "NewFriendlyName": NewFriendlyName, 
             "Secret": Secret, 
             "RestartIfPreviouslyRunning": RestartIfPreviouslyRunning, 
         })
 
     def ADSModule_DeployTemplate(self, TemplateID: int, NewUsername: str, NewPassword: str, NewEmail: str, RequiredTags: list[str], Tag: str, FriendlyName: str, Secret: str, PostCreate, ExtraProvisionSettings: dict[str, str]):
         """
         :param TemplateID: The ID of the template to be deployed, as per the Template Management UI in AMP itself.
-        :type TemplateID: intFalse
+        :type TemplateID: int False
             AMP Type: Int32
         :param NewUsername: If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.
-        :type NewUsername: strTrue
+        :type NewUsername: str True
             AMP Type: String
         :param NewPassword: If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.
-        :type NewPassword: strTrue
+        :type NewPassword: str True
             AMP Type: String
         :param NewEmail: If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.
-        :type NewEmail: strTrue
+        :type NewEmail: str True
             AMP Type: String
         :param RequiredTags: If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.
-        :type RequiredTags: list[str]True
+        :type RequiredTags: list[str] True
             AMP Type: List<String>
         :param Tag: Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.
-        :type Tag: strTrue
+        :type Tag: str True
             AMP Type: String
         :param FriendlyName: A friendly name for this instance. If left blank, AMP will generate one for you.
-        :type FriendlyName: strTrue
+        :type FriendlyName: str True
             AMP Type: String
         :param Secret: Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.
-        :type Secret: strTrue
+        :type Secret: str True
             AMP Type: String
         :param PostCreate: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.
             AMP Type: PostCreateActions
         :param ExtraProvisionSettings: A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.
-        :type ExtraProvisionSettings: dict[str, str]True
+        :type ExtraProvisionSettings: dict[str, str] True
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="ADSModule/DeployTemplate", data={
             "TemplateID": TemplateID, 
             "NewUsername": NewUsername, 
             "NewPassword": NewPassword, 
@@ -477,41 +477,41 @@
             "PostCreate": PostCreate, 
             "ExtraProvisionSettings": ExtraProvisionSettings, 
         })
 
     async def ADSModule_DeployTemplateAsync(self, TemplateID: int, NewUsername: str, NewPassword: str, NewEmail: str, RequiredTags: list[str], Tag: str, FriendlyName: str, Secret: str, PostCreate, ExtraProvisionSettings: dict[str, str]):
         """
         :param TemplateID: The ID of the template to be deployed, as per the Template Management UI in AMP itself.
-        :type TemplateID: intFalse
+        :type TemplateID: int False
             AMP Type: Int32
         :param NewUsername: If specified, AMP will create a new user with this name for this instance. Must be unique. If this user already exists, this will be ignored but the new instance will be assigned to this user.
-        :type NewUsername: strTrue
+        :type NewUsername: str True
             AMP Type: String
         :param NewPassword: If 'NewUsername' is specified and the user doesn't already exist, the password that will be assigned to this user.
-        :type NewPassword: strTrue
+        :type NewPassword: str True
             AMP Type: String
         :param NewEmail: If 'NewUsername' is specified and the user doesn't already exist, the email address that will be assigned to this user.
-        :type NewEmail: strTrue
+        :type NewEmail: str True
             AMP Type: String
         :param RequiredTags: If specified, AMP will only deploy this template to targets that have every single 'tag' specified in their target configuration. You can adjust this via the controller by clicking 'Edit' on the target settings.
-        :type RequiredTags: list[str]True
+        :type RequiredTags: list[str] True
             AMP Type: List<String>
         :param Tag: Unrelated to RequiredTags. This is to uniquely identify this instance to your own systems. It may be something like an order ID or service ID so you can find the associated instance again at a later time. If 'UseTagAsInstanceName' is enabled, then this will also be used as the instance name for the created instance - but it must be unique.
-        :type Tag: strTrue
+        :type Tag: str True
             AMP Type: String
         :param FriendlyName: A friendly name for this instance. If left blank, AMP will generate one for you.
-        :type FriendlyName: strTrue
+        :type FriendlyName: str True
             AMP Type: String
         :param Secret: Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.
-        :type Secret: strTrue
+        :type Secret: str True
             AMP Type: String
         :param PostCreate: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.
             AMP Type: PostCreateActions
         :param ExtraProvisionSettings: A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.
-        :type ExtraProvisionSettings: dict[str, str]True
+        :type ExtraProvisionSettings: dict[str, str] True
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="ADSModule/DeployTemplate", data={
             "TemplateID": TemplateID, 
             "NewUsername": NewUsername, 
             "NewPassword": NewPassword, 
@@ -577,27 +577,27 @@
         :rtype: None
         """
         return await self.APICallAsync(endpoint="ADSModule/RefreshRemoteConfigStores")
 
     def ADSModule_GetApplicationEndpoints(self, instanceId: str):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :returns: AMP Type: IEnumerable<EndpointInfo>
         :rtype: list
         """
         return self.APICall(endpoint="ADSModule/GetApplicationEndpoints", data={
             "instanceId": instanceId, 
         })
 
     async def ADSModule_GetApplicationEndpointsAsync(self, instanceId: str):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :returns: AMP Type: IEnumerable<EndpointInfo>
         :rtype: list
         """
         return await self.APICallAsync(endpoint="ADSModule/GetApplicationEndpoints", data={
             "instanceId": instanceId, 
         })
@@ -627,54 +627,54 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="ADSModule/GetInstances")
 
     def ADSModule_GetInstance(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return self.APICall(endpoint="ADSModule/GetInstance", data={
             "InstanceId": InstanceId, 
         })
 
     async def ADSModule_GetInstanceAsync(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="ADSModule/GetInstance", data={
             "InstanceId": InstanceId, 
         })
 
     def ADSModule_ModifyCustomFirewallRule(self, instanceId: str, PortNumber: int, Range: int, Protocol: str, Description: str, Open: bool):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :param PortNumber: 
-        :type PortNumber: intFalse
+        :type PortNumber: int False
             AMP Type: Int32
         :param Range: 
-        :type Range: intFalse
+        :type Range: int False
             AMP Type: Int32
         :param Protocol: 
-        :type Protocol: strFalse
+        :type Protocol: str False
             AMP Type: PortProtocol
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Open: 
-        :type Open: boolFalse
+        :type Open: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/ModifyCustomFirewallRule", data={
             "instanceId": instanceId, 
             "PortNumber": PortNumber, 
             "Range": Range, 
@@ -682,30 +682,30 @@
             "Description": Description, 
             "Open": Open, 
         })
 
     async def ADSModule_ModifyCustomFirewallRuleAsync(self, instanceId: str, PortNumber: int, Range: int, Protocol: str, Description: str, Open: bool):
         """
         :param instanceId: 
-        :type instanceId: strFalse
+        :type instanceId: str False
             AMP Type: Guid
         :param PortNumber: 
-        :type PortNumber: intFalse
+        :type PortNumber: int False
             AMP Type: Int32
         :param Range: 
-        :type Range: intFalse
+        :type Range: int False
             AMP Type: Int32
         :param Protocol: 
-        :type Protocol: strFalse
+        :type Protocol: str False
             AMP Type: PortProtocol
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Open: 
-        :type Open: boolFalse
+        :type Open: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/ModifyCustomFirewallRule", data={
             "instanceId": instanceId, 
             "PortNumber": PortNumber, 
             "Range": Range, 
@@ -713,72 +713,72 @@
             "Description": Description, 
             "Open": Open, 
         })
 
     def ADSModule_ManageInstance(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult<String>
         """
         return self.APICall(endpoint="ADSModule/ManageInstance", data={
             "InstanceId": InstanceId, 
         })
 
     async def ADSModule_ManageInstanceAsync(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult<String>
         """
         return await self.APICallAsync(endpoint="ADSModule/ManageInstance", data={
             "InstanceId": InstanceId, 
         })
 
     def ADSModule_GetGroup(self, GroupId: str):
         """
         :param GroupId: 
-        :type GroupId: strFalse
+        :type GroupId: str False
             AMP Type: Guid
         :returns: AMP Type: IADSInstance
         :rtype: bool
         """
         return self.APICall(endpoint="ADSModule/GetGroup", data={
             "GroupId": GroupId, 
         })
 
     async def ADSModule_GetGroupAsync(self, GroupId: str):
         """
         :param GroupId: 
-        :type GroupId: strFalse
+        :type GroupId: str False
             AMP Type: Guid
         :returns: AMP Type: IADSInstance
         :rtype: bool
         """
         return await self.APICallAsync(endpoint="ADSModule/GetGroup", data={
             "GroupId": GroupId, 
         })
 
     def ADSModule_RefreshGroup(self, GroupId: str):
         """
         :param GroupId: 
-        :type GroupId: strFalse
+        :type GroupId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/RefreshGroup", data={
             "GroupId": GroupId, 
         })
 
     async def ADSModule_RefreshGroupAsync(self, GroupId: str):
         """
         :param GroupId: 
-        :type GroupId: strFalse
+        :type GroupId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/RefreshGroup", data={
             "GroupId": GroupId, 
         })
 
@@ -823,246 +823,246 @@
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="ADSModule/GetProvisionFitness")
 
     def ADSModule_AttachADS(self, Friendly: str, IsHTTPS: bool, Host: str, Port: int, InstanceID: str):
         """
         :param Friendly: 
-        :type Friendly: strFalse
+        :type Friendly: str False
             AMP Type: String
         :param IsHTTPS: 
-        :type IsHTTPS: boolFalse
+        :type IsHTTPS: bool False
             AMP Type: Boolean
         :param Host: 
-        :type Host: strFalse
+        :type Host: str False
             AMP Type: String
         :param Port: 
-        :type Port: intFalse
+        :type Port: int False
             AMP Type: Int32
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/AttachADS", data={
             "Friendly": Friendly, 
             "IsHTTPS": IsHTTPS, 
             "Host": Host, 
             "Port": Port, 
             "InstanceID": InstanceID, 
         })
 
     async def ADSModule_AttachADSAsync(self, Friendly: str, IsHTTPS: bool, Host: str, Port: int, InstanceID: str):
         """
         :param Friendly: 
-        :type Friendly: strFalse
+        :type Friendly: str False
             AMP Type: String
         :param IsHTTPS: 
-        :type IsHTTPS: boolFalse
+        :type IsHTTPS: bool False
             AMP Type: Boolean
         :param Host: 
-        :type Host: strFalse
+        :type Host: str False
             AMP Type: String
         :param Port: 
-        :type Port: intFalse
+        :type Port: int False
             AMP Type: Int32
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/AttachADS", data={
             "Friendly": Friendly, 
             "IsHTTPS": IsHTTPS, 
             "Host": Host, 
             "Port": Port, 
             "InstanceID": InstanceID, 
         })
 
     def ADSModule_DetatchTarget(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/DetatchTarget", data={
             "Id": Id, 
         })
 
     async def ADSModule_DetatchTargetAsync(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/DetatchTarget", data={
             "Id": Id, 
         })
 
     def ADSModule_UpdateTargetInfo(self, Id: str, FriendlyName: str, Url: str, Description: str, Tags: list[str]):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param Url: 
-        :type Url: strFalse
+        :type Url: str False
             AMP Type: Uri
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Tags: 
-        :type Tags: list[str]False
+        :type Tags: list[str] False
             AMP Type: List<String>
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/UpdateTargetInfo", data={
             "Id": Id, 
             "FriendlyName": FriendlyName, 
             "Url": Url, 
             "Description": Description, 
             "Tags": Tags, 
         })
 
     async def ADSModule_UpdateTargetInfoAsync(self, Id: str, FriendlyName: str, Url: str, Description: str, Tags: list[str]):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param Url: 
-        :type Url: strFalse
+        :type Url: str False
             AMP Type: Uri
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Tags: 
-        :type Tags: list[str]False
+        :type Tags: list[str] False
             AMP Type: List<String>
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/UpdateTargetInfo", data={
             "Id": Id, 
             "FriendlyName": FriendlyName, 
             "Url": Url, 
             "Description": Description, 
             "Tags": Tags, 
         })
 
     def ADSModule_ConvertToManaged(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/ConvertToManaged", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_ConvertToManagedAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/ConvertToManaged", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_GetInstanceNetworkInfo(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<PortUsage>
         :rtype: list
         """
         return self.APICall(endpoint="ADSModule/GetInstanceNetworkInfo", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_GetInstanceNetworkInfoAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<PortUsage>
         :rtype: list
         """
         return await self.APICallAsync(endpoint="ADSModule/GetInstanceNetworkInfo", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_SetInstanceNetworkInfo(self, InstanceId: str, PortMappings: dict[str, int]):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :param PortMappings: 
-        :type PortMappings: dict[str, int]False
+        :type PortMappings: dict[str, int] False
             AMP Type: Dictionary<String, Int32>
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/SetInstanceNetworkInfo", data={
             "InstanceId": InstanceId, 
             "PortMappings": PortMappings, 
         })
 
     async def ADSModule_SetInstanceNetworkInfoAsync(self, InstanceId: str, PortMappings: dict[str, int]):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :param PortMappings: 
-        :type PortMappings: dict[str, int]False
+        :type PortMappings: dict[str, int] False
             AMP Type: Dictionary<String, Int32>
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/SetInstanceNetworkInfo", data={
             "InstanceId": InstanceId, 
             "PortMappings": PortMappings, 
         })
 
     def ADSModule_ApplyInstanceConfiguration(self, InstanceID: str, Args: dict[str, str], RebuildConfiguration: bool):
         """
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :param Args: 
-        :type Args: dict[str, str]False
+        :type Args: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :param RebuildConfiguration: 
-        :type RebuildConfiguration: boolTrue
+        :type RebuildConfiguration: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/ApplyInstanceConfiguration", data={
             "InstanceID": InstanceID, 
             "Args": Args, 
             "RebuildConfiguration": RebuildConfiguration, 
         })
 
     async def ADSModule_ApplyInstanceConfigurationAsync(self, InstanceID: str, Args: dict[str, str], RebuildConfiguration: bool):
         """
         :param InstanceID: 
-        :type InstanceID: strFalse
+        :type InstanceID: str False
             AMP Type: Guid
         :param Args: 
-        :type Args: dict[str, str]False
+        :type Args: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :param RebuildConfiguration: 
-        :type RebuildConfiguration: boolTrue
+        :type RebuildConfiguration: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/ApplyInstanceConfiguration", data={
             "InstanceID": InstanceID, 
             "Args": Args, 
             "RebuildConfiguration": RebuildConfiguration, 
@@ -1093,56 +1093,56 @@
             "Instance": Instance, 
             "PostCreate": PostCreate, 
         })
 
     def ADSModule_CreateInstance(self, TargetADSInstance: str, NewInstanceId: str, Module: str, InstanceName: str, FriendlyName: str, IPBinding: str, PortNumber: int, AdminUsername: str, AdminPassword: str, ProvisionSettings: dict[str, str], AutoConfigure: bool, PostCreate, StartOnBoot: bool, DisplayImageSource: str, TargetDatastore: int):
         """
         :param TargetADSInstance: 
-        :type TargetADSInstance: strFalse
+        :type TargetADSInstance: str False
             AMP Type: Guid
         :param NewInstanceId: 
-        :type NewInstanceId: strFalse
+        :type NewInstanceId: str False
             AMP Type: Guid
         :param Module: 
-        :type Module: strFalse
+        :type Module: str False
             AMP Type: String
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param IPBinding: 
-        :type IPBinding: strFalse
+        :type IPBinding: str False
             AMP Type: String
         :param PortNumber: 
-        :type PortNumber: intFalse
+        :type PortNumber: int False
             AMP Type: Int32
         :param AdminUsername: 
-        :type AdminUsername: strFalse
+        :type AdminUsername: str False
             AMP Type: String
         :param AdminPassword: 
-        :type AdminPassword: strFalse
+        :type AdminPassword: str False
             AMP Type: String
         :param ProvisionSettings: 
-        :type ProvisionSettings: dict[str, str]False
+        :type ProvisionSettings: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :param AutoConfigure: When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.
-        :type AutoConfigure: boolTrue
+        :type AutoConfigure: bool True
             AMP Type: Boolean
         :param PostCreate: 
             AMP Type: PostCreateActions
         :param StartOnBoot: 
-        :type StartOnBoot: boolTrue
+        :type StartOnBoot: bool True
             AMP Type: Boolean
         :param DisplayImageSource: 
-        :type DisplayImageSource: strTrue
+        :type DisplayImageSource: str True
             AMP Type: String
         :param TargetDatastore: 
-        :type TargetDatastore: intTrue
+        :type TargetDatastore: int True
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/CreateInstance", data={
             "TargetADSInstance": TargetADSInstance, 
             "NewInstanceId": NewInstanceId, 
             "Module": Module, 
@@ -1159,56 +1159,56 @@
             "DisplayImageSource": DisplayImageSource, 
             "TargetDatastore": TargetDatastore, 
         })
 
     async def ADSModule_CreateInstanceAsync(self, TargetADSInstance: str, NewInstanceId: str, Module: str, InstanceName: str, FriendlyName: str, IPBinding: str, PortNumber: int, AdminUsername: str, AdminPassword: str, ProvisionSettings: dict[str, str], AutoConfigure: bool, PostCreate, StartOnBoot: bool, DisplayImageSource: str, TargetDatastore: int):
         """
         :param TargetADSInstance: 
-        :type TargetADSInstance: strFalse
+        :type TargetADSInstance: str False
             AMP Type: Guid
         :param NewInstanceId: 
-        :type NewInstanceId: strFalse
+        :type NewInstanceId: str False
             AMP Type: Guid
         :param Module: 
-        :type Module: strFalse
+        :type Module: str False
             AMP Type: String
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param IPBinding: 
-        :type IPBinding: strFalse
+        :type IPBinding: str False
             AMP Type: String
         :param PortNumber: 
-        :type PortNumber: intFalse
+        :type PortNumber: int False
             AMP Type: Int32
         :param AdminUsername: 
-        :type AdminUsername: strFalse
+        :type AdminUsername: str False
             AMP Type: String
         :param AdminPassword: 
-        :type AdminPassword: strFalse
+        :type AdminPassword: str False
             AMP Type: String
         :param ProvisionSettings: 
-        :type ProvisionSettings: dict[str, str]False
+        :type ProvisionSettings: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :param AutoConfigure: When enabled, all settings other than the Module, Target and FriendlyName are ignored and replaced with automatically generated values.
-        :type AutoConfigure: boolTrue
+        :type AutoConfigure: bool True
             AMP Type: Boolean
         :param PostCreate: 
             AMP Type: PostCreateActions
         :param StartOnBoot: 
-        :type StartOnBoot: boolTrue
+        :type StartOnBoot: bool True
             AMP Type: Boolean
         :param DisplayImageSource: 
-        :type DisplayImageSource: strTrue
+        :type DisplayImageSource: str True
             AMP Type: String
         :param TargetDatastore: 
-        :type TargetDatastore: intTrue
+        :type TargetDatastore: int True
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/CreateInstance", data={
             "TargetADSInstance": TargetADSInstance, 
             "NewInstanceId": NewInstanceId, 
             "Module": Module, 
@@ -1225,190 +1225,190 @@
             "DisplayImageSource": DisplayImageSource, 
             "TargetDatastore": TargetDatastore, 
         })
 
     def ADSModule_SetInstanceConfig(self, InstanceName: str, SettingNode: str, Value: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param Value: 
-        :type Value: strFalse
+        :type Value: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/SetInstanceConfig", data={
             "InstanceName": InstanceName, 
             "SettingNode": SettingNode, 
             "Value": Value, 
         })
 
     async def ADSModule_SetInstanceConfigAsync(self, InstanceName: str, SettingNode: str, Value: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param Value: 
-        :type Value: strFalse
+        :type Value: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/SetInstanceConfig", data={
             "InstanceName": InstanceName, 
             "SettingNode": SettingNode, 
             "Value": Value, 
         })
 
     def ADSModule_RefreshInstanceConfig(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/RefreshInstanceConfig", data={
             "InstanceId": InstanceId, 
         })
 
     async def ADSModule_RefreshInstanceConfigAsync(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/RefreshInstanceConfig", data={
             "InstanceId": InstanceId, 
         })
 
     def ADSModule_HandoutInstanceConfigs(self, ForModule: str, SettingNode: str, Values: list[str]):
         """
         :param ForModule: 
-        :type ForModule: strFalse
+        :type ForModule: str False
             AMP Type: String
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param Values: 
-        :type Values: list[str]False
+        :type Values: list[str] False
             AMP Type: List<String>
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/HandoutInstanceConfigs", data={
             "ForModule": ForModule, 
             "SettingNode": SettingNode, 
             "Values": Values, 
         })
 
     async def ADSModule_HandoutInstanceConfigsAsync(self, ForModule: str, SettingNode: str, Values: list[str]):
         """
         :param ForModule: 
-        :type ForModule: strFalse
+        :type ForModule: str False
             AMP Type: String
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param Values: 
-        :type Values: list[str]False
+        :type Values: list[str] False
             AMP Type: List<String>
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/HandoutInstanceConfigs", data={
             "ForModule": ForModule, 
             "SettingNode": SettingNode, 
             "Values": Values, 
         })
 
     def ADSModule_GetProvisionArguments(self, ModuleName: str):
         """
         :param ModuleName: 
-        :type ModuleName: strFalse
+        :type ModuleName: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return self.APICall(endpoint="ADSModule/GetProvisionArguments", data={
             "ModuleName": ModuleName, 
         })
 
     async def ADSModule_GetProvisionArgumentsAsync(self, ModuleName: str):
         """
         :param ModuleName: 
-        :type ModuleName: strFalse
+        :type ModuleName: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="ADSModule/GetProvisionArguments", data={
             "ModuleName": ModuleName, 
         })
 
     def ADSModule_TestADSLoginDetails(self, url: str, username: str, password: str):
         """
         :param url: 
-        :type url: strFalse
+        :type url: str False
             AMP Type: String
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/TestADSLoginDetails", data={
             "url": url, 
             "username": username, 
             "password": password, 
         })
 
     async def ADSModule_TestADSLoginDetailsAsync(self, url: str, username: str, password: str):
         """
         :param url: 
-        :type url: strFalse
+        :type url: str False
             AMP Type: String
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/TestADSLoginDetails", data={
             "url": url, 
             "username": username, 
             "password": password, 
         })
 
     def ADSModule_RegisterTarget(self, controllerUrl: str, myUrl: str, username: str, password: str, twoFactorToken: str, friendlyName: str):
         """
         :param controllerUrl: 
-        :type controllerUrl: strFalse
+        :type controllerUrl: str False
             AMP Type: String
         :param myUrl: 
-        :type myUrl: strFalse
+        :type myUrl: str False
             AMP Type: String
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :param twoFactorToken: 
-        :type twoFactorToken: strFalse
+        :type twoFactorToken: str False
             AMP Type: String
         :param friendlyName: 
-        :type friendlyName: strFalse
+        :type friendlyName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/RegisterTarget", data={
             "controllerUrl": controllerUrl, 
             "myUrl": myUrl, 
             "username": username, 
@@ -1416,30 +1416,30 @@
             "twoFactorToken": twoFactorToken, 
             "friendlyName": friendlyName, 
         })
 
     async def ADSModule_RegisterTargetAsync(self, controllerUrl: str, myUrl: str, username: str, password: str, twoFactorToken: str, friendlyName: str):
         """
         :param controllerUrl: 
-        :type controllerUrl: strFalse
+        :type controllerUrl: str False
             AMP Type: String
         :param myUrl: 
-        :type myUrl: strFalse
+        :type myUrl: str False
             AMP Type: String
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :param twoFactorToken: 
-        :type twoFactorToken: strFalse
+        :type twoFactorToken: str False
             AMP Type: String
         :param friendlyName: 
-        :type friendlyName: strFalse
+        :type friendlyName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/RegisterTarget", data={
             "controllerUrl": controllerUrl, 
             "myUrl": myUrl, 
             "username": username, 
@@ -1447,170 +1447,178 @@
             "twoFactorToken": twoFactorToken, 
             "friendlyName": friendlyName, 
         })
 
     def ADSModule_UpdateTarget(self, TargetID: str):
         """
         :param TargetID: 
-        :type TargetID: strFalse
+        :type TargetID: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="ADSModule/UpdateTarget", data={
             "TargetID": TargetID, 
         })
 
     async def ADSModule_UpdateTargetAsync(self, TargetID: str):
         """
         :param TargetID: 
-        :type TargetID: strFalse
+        :type TargetID: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="ADSModule/UpdateTarget", data={
             "TargetID": TargetID, 
         })
 
-    def ADSModule_UpdateInstanceInfo(self, InstanceId: str, FriendlyName: str, Description: str, StartOnBoot: bool, Suspended: bool, ExcludeFromFirewall: bool, RunInContainer: bool, ContainerMemory: int, MemoryPolicy, ContainerMaxCPU):
+    def ADSModule_UpdateInstanceInfo(self, InstanceId: str, FriendlyName: str, Description: str, StartOnBoot: bool, Suspended: bool, ExcludeFromFirewall: bool, RunInContainer: bool, ContainerMemory: int, MemoryPolicy, ContainerMaxCPU, ContainerImage: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: String
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param StartOnBoot: 
-        :type StartOnBoot: boolFalse
+        :type StartOnBoot: bool False
             AMP Type: Boolean
         :param Suspended: 
-        :type Suspended: boolFalse
+        :type Suspended: bool False
             AMP Type: Boolean
         :param ExcludeFromFirewall: 
-        :type ExcludeFromFirewall: boolFalse
+        :type ExcludeFromFirewall: bool False
             AMP Type: Boolean
         :param RunInContainer: 
-        :type RunInContainer: boolFalse
+        :type RunInContainer: bool False
             AMP Type: Boolean
         :param ContainerMemory: 
-        :type ContainerMemory: intFalse
+        :type ContainerMemory: int False
             AMP Type: Int32
         :param MemoryPolicy: 
             AMP Type: ContainerMemoryPolicy
         :param ContainerMaxCPU: 
             AMP Type: Single
+        :param ContainerImage: 
+        :type ContainerImage: str False
+            AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/UpdateInstanceInfo", data={
             "InstanceId": InstanceId, 
             "FriendlyName": FriendlyName, 
             "Description": Description, 
             "StartOnBoot": StartOnBoot, 
             "Suspended": Suspended, 
             "ExcludeFromFirewall": ExcludeFromFirewall, 
             "RunInContainer": RunInContainer, 
             "ContainerMemory": ContainerMemory, 
             "MemoryPolicy": MemoryPolicy, 
             "ContainerMaxCPU": ContainerMaxCPU, 
+            "ContainerImage": ContainerImage, 
         })
 
-    async def ADSModule_UpdateInstanceInfoAsync(self, InstanceId: str, FriendlyName: str, Description: str, StartOnBoot: bool, Suspended: bool, ExcludeFromFirewall: bool, RunInContainer: bool, ContainerMemory: int, MemoryPolicy, ContainerMaxCPU):
+    async def ADSModule_UpdateInstanceInfoAsync(self, InstanceId: str, FriendlyName: str, Description: str, StartOnBoot: bool, Suspended: bool, ExcludeFromFirewall: bool, RunInContainer: bool, ContainerMemory: int, MemoryPolicy, ContainerMaxCPU, ContainerImage: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: String
         :param FriendlyName: 
-        :type FriendlyName: strFalse
+        :type FriendlyName: str False
             AMP Type: String
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param StartOnBoot: 
-        :type StartOnBoot: boolFalse
+        :type StartOnBoot: bool False
             AMP Type: Boolean
         :param Suspended: 
-        :type Suspended: boolFalse
+        :type Suspended: bool False
             AMP Type: Boolean
         :param ExcludeFromFirewall: 
-        :type ExcludeFromFirewall: boolFalse
+        :type ExcludeFromFirewall: bool False
             AMP Type: Boolean
         :param RunInContainer: 
-        :type RunInContainer: boolFalse
+        :type RunInContainer: bool False
             AMP Type: Boolean
         :param ContainerMemory: 
-        :type ContainerMemory: intFalse
+        :type ContainerMemory: int False
             AMP Type: Int32
         :param MemoryPolicy: 
             AMP Type: ContainerMemoryPolicy
         :param ContainerMaxCPU: 
             AMP Type: Single
+        :param ContainerImage: 
+        :type ContainerImage: str False
+            AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/UpdateInstanceInfo", data={
             "InstanceId": InstanceId, 
             "FriendlyName": FriendlyName, 
             "Description": Description, 
             "StartOnBoot": StartOnBoot, 
             "Suspended": Suspended, 
             "ExcludeFromFirewall": ExcludeFromFirewall, 
             "RunInContainer": RunInContainer, 
             "ContainerMemory": ContainerMemory, 
             "MemoryPolicy": MemoryPolicy, 
             "ContainerMaxCPU": ContainerMaxCPU, 
+            "ContainerImage": ContainerImage, 
         })
 
     def ADSModule_SetInstanceSuspended(self, InstanceName: str, Suspended: bool):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param Suspended: 
-        :type Suspended: boolFalse
+        :type Suspended: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/SetInstanceSuspended", data={
             "InstanceName": InstanceName, 
             "Suspended": Suspended, 
         })
 
     async def ADSModule_SetInstanceSuspendedAsync(self, InstanceName: str, Suspended: bool):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :param Suspended: 
-        :type Suspended: boolFalse
+        :type Suspended: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/SetInstanceSuspended", data={
             "InstanceName": InstanceName, 
             "Suspended": Suspended, 
         })
 
     def ADSModule_UpgradeInstance(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/UpgradeInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_UpgradeInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/UpgradeInstance", data={
             "InstanceName": InstanceName, 
         })
 
@@ -1637,187 +1645,187 @@
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/StopAllInstances")
 
     def ADSModule_UpgradeAllInstances(self, RestartRunning: bool):
         """
         :param RestartRunning: 
-        :type RestartRunning: boolFalse
+        :type RestartRunning: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/UpgradeAllInstances", data={
             "RestartRunning": RestartRunning, 
         })
 
     async def ADSModule_UpgradeAllInstancesAsync(self, RestartRunning: bool):
         """
         :param RestartRunning: 
-        :type RestartRunning: boolFalse
+        :type RestartRunning: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/UpgradeAllInstances", data={
             "RestartRunning": RestartRunning, 
         })
 
     def ADSModule_StartInstance(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/StartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_StartInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/StartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_RestartInstance(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/RestartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_RestartInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/RestartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_StopInstance(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/StopInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_StopInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/StopInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_DeleteInstanceUsers(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/DeleteInstanceUsers", data={
             "InstanceId": InstanceId, 
         })
 
     async def ADSModule_DeleteInstanceUsersAsync(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/DeleteInstanceUsers", data={
             "InstanceId": InstanceId, 
         })
 
     def ADSModule_DeleteInstance(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="ADSModule/DeleteInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_DeleteInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
-        :type InstanceName: strFalse
+        :type InstanceName: str False
             AMP Type: String
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="ADSModule/DeleteInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_ExtractEverywhere(self, SourceArchive: str):
         """
         :param SourceArchive: 
-        :type SourceArchive: strFalse
+        :type SourceArchive: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="ADSModule/ExtractEverywhere", data={
             "SourceArchive": SourceArchive, 
         })
 
     async def ADSModule_ExtractEverywhereAsync(self, SourceArchive: str):
         """
         :param SourceArchive: 
-        :type SourceArchive: strFalse
+        :type SourceArchive: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="ADSModule/ExtractEverywhere", data={
             "SourceArchive": SourceArchive, 
         })
 
     def ADSModule_Servers(self, id: str, REQ_RAWJSON: str):
         """
         :param id: 
-        :type id: strFalse
+        :type id: str False
             AMP Type: String
         :param REQ_RAWJSON: 
-        :type REQ_RAWJSON: strFalse
+        :type REQ_RAWJSON: str False
             AMP Type: String
         :returns: AMP Type: Task<JObject>
         """
         return self.APICall(endpoint="ADSModule/Servers", data={
             "id": id, 
             "REQ_RAWJSON": REQ_RAWJSON, 
         })
 
     async def ADSModule_ServersAsync(self, id: str, REQ_RAWJSON: str):
         """
         :param id: 
-        :type id: strFalse
+        :type id: str False
             AMP Type: String
         :param REQ_RAWJSON: 
-        :type REQ_RAWJSON: strFalse
+        :type REQ_RAWJSON: str False
             AMP Type: String
         :returns: AMP Type: Task<JObject>
         """
         return await self.APICallAsync(endpoint="ADSModule/Servers", data={
             "id": id, 
             "REQ_RAWJSON": REQ_RAWJSON, 
         })
@@ -1835,519 +1843,519 @@
         :rtype: None
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/Dummy")
 
     def FileManagerPlugin_CalculateFileMD5Sum(self, FilePath: str):
         """
         :param FilePath: 
-        :type FilePath: strFalse
+        :type FilePath: str False
             AMP Type: String
         :returns: AMP Type: ActionResult<String>
         """
         return self.APICall(endpoint="FileManagerPlugin/CalculateFileMD5Sum", data={
             "FilePath": FilePath, 
         })
 
     async def FileManagerPlugin_CalculateFileMD5SumAsync(self, FilePath: str):
         """
         :param FilePath: 
-        :type FilePath: strFalse
+        :type FilePath: str False
             AMP Type: String
         :returns: AMP Type: ActionResult<String>
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/CalculateFileMD5Sum", data={
             "FilePath": FilePath, 
         })
 
     def FileManagerPlugin_ChangeExclusion(self, ModifyPath: str, AsDirectory: bool, Exclude: bool):
         """
         :param ModifyPath: 
-        :type ModifyPath: strFalse
+        :type ModifyPath: str False
             AMP Type: String
         :param AsDirectory: 
-        :type AsDirectory: boolFalse
+        :type AsDirectory: bool False
             AMP Type: Boolean
         :param Exclude: 
-        :type Exclude: boolFalse
+        :type Exclude: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/ChangeExclusion", data={
             "ModifyPath": ModifyPath, 
             "AsDirectory": AsDirectory, 
             "Exclude": Exclude, 
         })
 
     async def FileManagerPlugin_ChangeExclusionAsync(self, ModifyPath: str, AsDirectory: bool, Exclude: bool):
         """
         :param ModifyPath: 
-        :type ModifyPath: strFalse
+        :type ModifyPath: str False
             AMP Type: String
         :param AsDirectory: 
-        :type AsDirectory: boolFalse
+        :type AsDirectory: bool False
             AMP Type: Boolean
         :param Exclude: 
-        :type Exclude: boolFalse
+        :type Exclude: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/ChangeExclusion", data={
             "ModifyPath": ModifyPath, 
             "AsDirectory": AsDirectory, 
             "Exclude": Exclude, 
         })
 
     def FileManagerPlugin_CreateArchive(self, PathToArchive: str):
         """
         :param PathToArchive: 
-        :type PathToArchive: strFalse
+        :type PathToArchive: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/CreateArchive", data={
             "PathToArchive": PathToArchive, 
         })
 
     async def FileManagerPlugin_CreateArchiveAsync(self, PathToArchive: str):
         """
         :param PathToArchive: 
-        :type PathToArchive: strFalse
+        :type PathToArchive: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/CreateArchive", data={
             "PathToArchive": PathToArchive, 
         })
 
     def FileManagerPlugin_ExtractArchive(self, ArchivePath: str, DestinationPath: str):
         """
         :param ArchivePath: 
-        :type ArchivePath: strFalse
+        :type ArchivePath: str False
             AMP Type: String
         :param DestinationPath: 
-        :type DestinationPath: strTrue
+        :type DestinationPath: str True
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/ExtractArchive", data={
             "ArchivePath": ArchivePath, 
             "DestinationPath": DestinationPath, 
         })
 
     async def FileManagerPlugin_ExtractArchiveAsync(self, ArchivePath: str, DestinationPath: str):
         """
         :param ArchivePath: 
-        :type ArchivePath: strFalse
+        :type ArchivePath: str False
             AMP Type: String
         :param DestinationPath: 
-        :type DestinationPath: strTrue
+        :type DestinationPath: str True
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/ExtractArchive", data={
             "ArchivePath": ArchivePath, 
             "DestinationPath": DestinationPath, 
         })
 
     def FileManagerPlugin_GetDirectoryListing(self, Dir: str):
         """
         :param Dir: 
-        :type Dir: strFalse
+        :type Dir: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return self.APICall(endpoint="FileManagerPlugin/GetDirectoryListing", data={
             "Dir": Dir, 
         })
 
     async def FileManagerPlugin_GetDirectoryListingAsync(self, Dir: str):
         """
         :param Dir: 
-        :type Dir: strFalse
+        :type Dir: str False
             AMP Type: String
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/GetDirectoryListing", data={
             "Dir": Dir, 
         })
 
     def FileManagerPlugin_GetFileChunk(self, Filename: str, Position: int, Length: int):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Position: 
-        :type Position: intFalse
+        :type Position: int False
             AMP Type: Int64
         :param Length: 
-        :type Length: intFalse
+        :type Length: int False
             AMP Type: Int32
         :returns: AMP Type: FileChunkData
         """
         return self.APICall(endpoint="FileManagerPlugin/GetFileChunk", data={
             "Filename": Filename, 
             "Position": Position, 
             "Length": Length, 
         })
 
     async def FileManagerPlugin_GetFileChunkAsync(self, Filename: str, Position: int, Length: int):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Position: 
-        :type Position: intFalse
+        :type Position: int False
             AMP Type: Int64
         :param Length: 
-        :type Length: intFalse
+        :type Length: int False
             AMP Type: Int32
         :returns: AMP Type: FileChunkData
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/GetFileChunk", data={
             "Filename": Filename, 
             "Position": Position, 
             "Length": Length, 
         })
 
     def FileManagerPlugin_AppendFileChunk(self, Filename: str, Data: str, Delete: bool):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Data: 
-        :type Data: strFalse
+        :type Data: str False
             AMP Type: String
         :param Delete: 
-        :type Delete: boolFalse
+        :type Delete: bool False
             AMP Type: Boolean
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="FileManagerPlugin/AppendFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Delete": Delete, 
         })
 
     async def FileManagerPlugin_AppendFileChunkAsync(self, Filename: str, Data: str, Delete: bool):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Data: 
-        :type Data: strFalse
+        :type Data: str False
             AMP Type: String
         :param Delete: 
-        :type Delete: boolFalse
+        :type Delete: bool False
             AMP Type: Boolean
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/AppendFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Delete": Delete, 
         })
 
     def FileManagerPlugin_ReadFileChunk(self, Filename: str, Offset: int, ChunkSize: int):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Offset: 
-        :type Offset: intFalse
+        :type Offset: int False
             AMP Type: Int64
         :param ChunkSize: 
-        :type ChunkSize: intTrue
+        :type ChunkSize: int True
             AMP Type: Int64
         :returns: AMP Type: ActionResult<String>
         """
         return self.APICall(endpoint="FileManagerPlugin/ReadFileChunk", data={
             "Filename": Filename, 
             "Offset": Offset, 
             "ChunkSize": ChunkSize, 
         })
 
     async def FileManagerPlugin_ReadFileChunkAsync(self, Filename: str, Offset: int, ChunkSize: int):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Offset: 
-        :type Offset: intFalse
+        :type Offset: int False
             AMP Type: Int64
         :param ChunkSize: 
-        :type ChunkSize: intTrue
+        :type ChunkSize: int True
             AMP Type: Int64
         :returns: AMP Type: ActionResult<String>
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/ReadFileChunk", data={
             "Filename": Filename, 
             "Offset": Offset, 
             "ChunkSize": ChunkSize, 
         })
 
     def FileManagerPlugin_WriteFileChunk(self, Filename: str, Data: str, Offset: int, FinalChunk: bool):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Data: 
-        :type Data: strFalse
+        :type Data: str False
             AMP Type: String
         :param Offset: 
-        :type Offset: intFalse
+        :type Offset: int False
             AMP Type: Int64
         :param FinalChunk: 
-        :type FinalChunk: boolFalse
+        :type FinalChunk: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/WriteFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Offset": Offset, 
             "FinalChunk": FinalChunk, 
         })
 
     async def FileManagerPlugin_WriteFileChunkAsync(self, Filename: str, Data: str, Offset: int, FinalChunk: bool):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param Data: 
-        :type Data: strFalse
+        :type Data: str False
             AMP Type: String
         :param Offset: 
-        :type Offset: intFalse
+        :type Offset: int False
             AMP Type: Int64
         :param FinalChunk: 
-        :type FinalChunk: boolFalse
+        :type FinalChunk: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/WriteFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Offset": Offset, 
             "FinalChunk": FinalChunk, 
         })
 
     def FileManagerPlugin_DownloadFileFromURL(self, Source: str, TargetDirectory: str):
         """
         :param Source: 
-        :type Source: strFalse
+        :type Source: str False
             AMP Type: Uri
         :param TargetDirectory: 
-        :type TargetDirectory: strFalse
+        :type TargetDirectory: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/DownloadFileFromURL", data={
             "Source": Source, 
             "TargetDirectory": TargetDirectory, 
         })
 
     async def FileManagerPlugin_DownloadFileFromURLAsync(self, Source: str, TargetDirectory: str):
         """
         :param Source: 
-        :type Source: strFalse
+        :type Source: str False
             AMP Type: Uri
         :param TargetDirectory: 
-        :type TargetDirectory: strFalse
+        :type TargetDirectory: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/DownloadFileFromURL", data={
             "Source": Source, 
             "TargetDirectory": TargetDirectory, 
         })
 
     def FileManagerPlugin_RenameFile(self, Filename: str, NewFilename: str):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param NewFilename: 
-        :type NewFilename: strFalse
+        :type NewFilename: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/RenameFile", data={
             "Filename": Filename, 
             "NewFilename": NewFilename, 
         })
 
     async def FileManagerPlugin_RenameFileAsync(self, Filename: str, NewFilename: str):
         """
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :param NewFilename: 
-        :type NewFilename: strFalse
+        :type NewFilename: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/RenameFile", data={
             "Filename": Filename, 
             "NewFilename": NewFilename, 
         })
 
     def FileManagerPlugin_CopyFile(self, Origin: str, TargetDirectory: str):
         """
         :param Origin: 
-        :type Origin: strFalse
+        :type Origin: str False
             AMP Type: String
         :param TargetDirectory: 
-        :type TargetDirectory: strFalse
+        :type TargetDirectory: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/CopyFile", data={
             "Origin": Origin, 
             "TargetDirectory": TargetDirectory, 
         })
 
     async def FileManagerPlugin_CopyFileAsync(self, Origin: str, TargetDirectory: str):
         """
         :param Origin: 
-        :type Origin: strFalse
+        :type Origin: str False
             AMP Type: String
         :param TargetDirectory: 
-        :type TargetDirectory: strFalse
+        :type TargetDirectory: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/CopyFile", data={
             "Origin": Origin, 
             "TargetDirectory": TargetDirectory, 
         })
 
     def FileManagerPlugin_TrashFile(self, Filename: str):
         """Moves a file to trash, files must be trashed before they can be deleted.
             
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/TrashFile", data={
             "Filename": Filename, 
         })
 
     async def FileManagerPlugin_TrashFileAsync(self, Filename: str):
         """Moves a file to trash, files must be trashed before they can be deleted.
             
         :param Filename: 
-        :type Filename: strFalse
+        :type Filename: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/TrashFile", data={
             "Filename": Filename, 
         })
 
     def FileManagerPlugin_TrashDirectory(self, DirectoryName: str):
         """Moves a directory to trash, files must be trashed before they can be deleted.
             
         :param DirectoryName: 
-        :type DirectoryName: strFalse
+        :type DirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/TrashDirectory", data={
             "DirectoryName": DirectoryName, 
         })
 
     async def FileManagerPlugin_TrashDirectoryAsync(self, DirectoryName: str):
         """Moves a directory to trash, files must be trashed before they can be deleted.
             
         :param DirectoryName: 
-        :type DirectoryName: strFalse
+        :type DirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/TrashDirectory", data={
             "DirectoryName": DirectoryName, 
         })
 
     def FileManagerPlugin_EmptyTrash(self, TrashDirectoryName: str):
         """Empties a trash bin
             
         :param TrashDirectoryName: 
-        :type TrashDirectoryName: strFalse
+        :type TrashDirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/EmptyTrash", data={
             "TrashDirectoryName": TrashDirectoryName, 
         })
 
     async def FileManagerPlugin_EmptyTrashAsync(self, TrashDirectoryName: str):
         """Empties a trash bin
             
         :param TrashDirectoryName: 
-        :type TrashDirectoryName: strFalse
+        :type TrashDirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/EmptyTrash", data={
             "TrashDirectoryName": TrashDirectoryName, 
         })
 
     def FileManagerPlugin_CreateDirectory(self, NewPath: str):
         """Creates a new directory. The parent directory must already exist.
             
         :param NewPath: 
-        :type NewPath: strFalse
+        :type NewPath: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/CreateDirectory", data={
             "NewPath": NewPath, 
         })
 
     async def FileManagerPlugin_CreateDirectoryAsync(self, NewPath: str):
         """Creates a new directory. The parent directory must already exist.
             
         :param NewPath: 
-        :type NewPath: strFalse
+        :type NewPath: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/CreateDirectory", data={
             "NewPath": NewPath, 
         })
 
     def FileManagerPlugin_RenameDirectory(self, oldDirectory: str, NewDirectoryName: str):
         """Renames a directory
             
         :param oldDirectory: The full path to the old directory
-        :type oldDirectory: strFalse
+        :type oldDirectory: str False
             AMP Type: String
         :param NewDirectoryName: The name component of the new directory (not the full path)
-        :type NewDirectoryName: strFalse
+        :type NewDirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/RenameDirectory", data={
             "oldDirectory": oldDirectory, 
             "NewDirectoryName": NewDirectoryName, 
         })
 
     async def FileManagerPlugin_RenameDirectoryAsync(self, oldDirectory: str, NewDirectoryName: str):
         """Renames a directory
             
         :param oldDirectory: The full path to the old directory
-        :type oldDirectory: strFalse
+        :type oldDirectory: str False
             AMP Type: String
         :param NewDirectoryName: The name component of the new directory (not the full path)
-        :type NewDirectoryName: strFalse
+        :type NewDirectoryName: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/RenameDirectory", data={
             "oldDirectory": oldDirectory, 
             "NewDirectoryName": NewDirectoryName, 
         })
@@ -2363,70 +2371,70 @@
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="EmailSenderPlugin/TestSMTPSettings")
 
     def LocalFileBackupPlugin_UploadToS3(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/UploadToS3", data={
             "BackupId": BackupId, 
         })
 
     async def LocalFileBackupPlugin_UploadToS3Async(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/UploadToS3", data={
             "BackupId": BackupId, 
         })
 
     def LocalFileBackupPlugin_DownloadFromS3(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/DownloadFromS3", data={
             "BackupId": BackupId, 
         })
 
     async def LocalFileBackupPlugin_DownloadFromS3Async(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/DownloadFromS3", data={
             "BackupId": BackupId, 
         })
 
     def LocalFileBackupPlugin_DeleteFromS3(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/DeleteFromS3", data={
             "BackupId": BackupId, 
         })
 
     async def LocalFileBackupPlugin_DeleteFromS3Async(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/DeleteFromS3", data={
             "BackupId": BackupId, 
         })
 
@@ -2443,156 +2451,156 @@
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/GetBackups")
 
     def LocalFileBackupPlugin_RestoreBackup(self, BackupId: str, DeleteExistingData: bool):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :param DeleteExistingData: 
-        :type DeleteExistingData: boolTrue
+        :type DeleteExistingData: bool True
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/RestoreBackup", data={
             "BackupId": BackupId, 
             "DeleteExistingData": DeleteExistingData, 
         })
 
     async def LocalFileBackupPlugin_RestoreBackupAsync(self, BackupId: str, DeleteExistingData: bool):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :param DeleteExistingData: 
-        :type DeleteExistingData: boolTrue
+        :type DeleteExistingData: bool True
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/RestoreBackup", data={
             "BackupId": BackupId, 
             "DeleteExistingData": DeleteExistingData, 
         })
 
     def LocalFileBackupPlugin_DeleteLocalBackup(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/DeleteLocalBackup", data={
             "BackupId": BackupId, 
         })
 
     async def LocalFileBackupPlugin_DeleteLocalBackupAsync(self, BackupId: str):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/DeleteLocalBackup", data={
             "BackupId": BackupId, 
         })
 
     def LocalFileBackupPlugin_SetBackupSticky(self, BackupId: str, Sticky: bool):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :param Sticky: 
-        :type Sticky: boolFalse
+        :type Sticky: bool False
             AMP Type: Boolean
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/SetBackupSticky", data={
             "BackupId": BackupId, 
             "Sticky": Sticky, 
         })
 
     async def LocalFileBackupPlugin_SetBackupStickyAsync(self, BackupId: str, Sticky: bool):
         """
         :param BackupId: 
-        :type BackupId: strFalse
+        :type BackupId: str False
             AMP Type: Guid
         :param Sticky: 
-        :type Sticky: boolFalse
+        :type Sticky: bool False
             AMP Type: Boolean
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/SetBackupSticky", data={
             "BackupId": BackupId, 
             "Sticky": Sticky, 
         })
 
     def LocalFileBackupPlugin_TakeBackup(self, Title: str, Description: str, Sticky: bool):
         """
         :param Title: 
-        :type Title: strFalse
+        :type Title: str False
             AMP Type: String
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Sticky: 
-        :type Sticky: boolFalse
+        :type Sticky: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="LocalFileBackupPlugin/TakeBackup", data={
             "Title": Title, 
             "Description": Description, 
             "Sticky": Sticky, 
         })
 
     async def LocalFileBackupPlugin_TakeBackupAsync(self, Title: str, Description: str, Sticky: bool):
         """
         :param Title: 
-        :type Title: strFalse
+        :type Title: str False
             AMP Type: String
         :param Description: 
-        :type Description: strFalse
+        :type Description: str False
             AMP Type: String
         :param Sticky: 
-        :type Sticky: boolFalse
+        :type Sticky: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="LocalFileBackupPlugin/TakeBackup", data={
             "Title": Title, 
             "Description": Description, 
             "Sticky": Sticky, 
         })
 
     def Core_GetAuditLogEntries(self, Before, Count: int):
         """
         :param Before: 
             AMP Type: Nullable<DateTime>
         :param Count: 
-        :type Count: intFalse
+        :type Count: int False
             AMP Type: Int32
         :returns: AMP Type: IEnumerable<IAuditLogEntry>
         :rtype: dict
         """
         return self.APICall(endpoint="Core/GetAuditLogEntries", data={
             "Before": Before, 
             "Count": Count, 
         })
 
     async def Core_GetAuditLogEntriesAsync(self, Before, Count: int):
         """
         :param Before: 
             AMP Type: Nullable<DateTime>
         :param Count: 
-        :type Count: intFalse
+        :type Count: int False
             AMP Type: Int32
         :returns: AMP Type: IEnumerable<IAuditLogEntry>
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="Core/GetAuditLogEntries", data={
             "Before": Before, 
             "Count": Count, 
@@ -2611,26 +2619,26 @@
         :rtype: dict[str, list[dict]]
         """
         return await self.APICallAsync(endpoint="Core/GetSettingsSpec")
 
     def Core_RefreshSettingValueList(self, Node: str):
         """
         :param Node: 
-        :type Node: strFalse
+        :type Node: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/RefreshSettingValueList", data={
             "Node": Node, 
         })
 
     async def Core_RefreshSettingValueListAsync(self, Node: str):
         """
         :param Node: 
-        :type Node: strFalse
+        :type Node: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/RefreshSettingValueList", data={
             "Node": Node, 
         })
 
@@ -2647,34 +2655,34 @@
         :rtype: None
         """
         return await self.APICallAsync(endpoint="Core/RefreshSettingsSourceCache")
 
     def Core_GetSettingValues(self, SettingNode: str, WithRefresh: bool):
         """
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param WithRefresh: 
-        :type WithRefresh: boolTrue
+        :type WithRefresh: bool True
             AMP Type: Boolean
         :returns: AMP Type: IDictionary<String, String>
         :rtype: dict[str, str]
         """
         return self.APICall(endpoint="Core/GetSettingValues", data={
             "SettingNode": SettingNode, 
             "WithRefresh": WithRefresh, 
         })
 
     async def Core_GetSettingValuesAsync(self, SettingNode: str, WithRefresh: bool):
         """
         :param SettingNode: 
-        :type SettingNode: strFalse
+        :type SettingNode: str False
             AMP Type: String
         :param WithRefresh: 
-        :type WithRefresh: boolTrue
+        :type WithRefresh: bool True
             AMP Type: Boolean
         :returns: AMP Type: IDictionary<String, String>
         :rtype: dict[str, str]
         """
         return await self.APICallAsync(endpoint="Core/GetSettingValues", data={
             "SettingNode": SettingNode, 
             "WithRefresh": WithRefresh, 
@@ -2693,105 +2701,105 @@
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="Core/GetProvisionSpec")
 
     def Core_GetConfig(self, node: str):
         """
         :param node: 
-        :type node: strFalse
+        :type node: str False
             AMP Type: String
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return self.APICall(endpoint="Core/GetConfig", data={
             "node": node, 
         })
 
     async def Core_GetConfigAsync(self, node: str):
         """
         :param node: 
-        :type node: strFalse
+        :type node: str False
             AMP Type: String
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="Core/GetConfig", data={
             "node": node, 
         })
 
     def Core_GetConfigs(self, nodes: list[str]):
         """
         :param nodes: 
-        :type nodes: list[str]False
+        :type nodes: list[str] False
             AMP Type: String[]
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return self.APICall(endpoint="Core/GetConfigs", data={
             "nodes": nodes, 
         })
 
     async def Core_GetConfigsAsync(self, nodes: list[str]):
         """
         :param nodes: 
-        :type nodes: list[str]False
+        :type nodes: list[str] False
             AMP Type: String[]
         :returns: AMP Type: IEnumerable<JObject>
         :rtype: list[dict]
         """
         return await self.APICallAsync(endpoint="Core/GetConfigs", data={
             "nodes": nodes, 
         })
 
     def Core_SetConfigs(self, data: dict[str, str]):
         """
         :param data: 
-        :type data: dict[str, str]False
+        :type data: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: Boolean
         :rtype: bool
         """
         return self.APICall(endpoint="Core/SetConfigs", data={
             "data": data, 
         })
 
     async def Core_SetConfigsAsync(self, data: dict[str, str]):
         """
         :param data: 
-        :type data: dict[str, str]False
+        :type data: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: Boolean
         :rtype: bool
         """
         return await self.APICallAsync(endpoint="Core/SetConfigs", data={
             "data": data, 
         })
 
     def Core_SetConfig(self, node: str, value: str):
         """
         :param node: 
-        :type node: strFalse
+        :type node: str False
             AMP Type: String
         :param value: 
-        :type value: strFalse
+        :type value: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/SetConfig", data={
             "node": node, 
             "value": value, 
         })
 
     async def Core_SetConfigAsync(self, node: str, value: str):
         """
         :param node: 
-        :type node: strFalse
+        :type node: str False
             AMP Type: String
         :param value: 
-        :type value: strFalse
+        :type value: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/SetConfig", data={
             "node": node, 
             "value": value, 
         })
@@ -2819,168 +2827,168 @@
         :returns: AMP Type: Task<IDictionary<Guid, String>>
         """
         return await self.APICallAsync(endpoint="Core/GetRoleIds")
 
     def Core_GetRole(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<AuthRoleSummary>
         """
         return self.APICall(endpoint="Core/GetRole", data={
             "RoleId": RoleId, 
         })
 
     async def Core_GetRoleAsync(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<AuthRoleSummary>
         """
         return await self.APICallAsync(endpoint="Core/GetRole", data={
             "RoleId": RoleId, 
         })
 
     def Core_CreateRole(self, Name: str, AsCommonRole: bool):
         """
         :param Name: 
-        :type Name: strFalse
+        :type Name: str False
             AMP Type: String
         :param AsCommonRole: 
-        :type AsCommonRole: boolTrue
+        :type AsCommonRole: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult<Guid>>
         """
         return self.APICall(endpoint="Core/CreateRole", data={
             "Name": Name, 
             "AsCommonRole": AsCommonRole, 
         })
 
     async def Core_CreateRoleAsync(self, Name: str, AsCommonRole: bool):
         """
         :param Name: 
-        :type Name: strFalse
+        :type Name: str False
             AMP Type: String
         :param AsCommonRole: 
-        :type AsCommonRole: boolTrue
+        :type AsCommonRole: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult<Guid>>
         """
         return await self.APICallAsync(endpoint="Core/CreateRole", data={
             "Name": Name, 
             "AsCommonRole": AsCommonRole, 
         })
 
     def Core_DeleteRole(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/DeleteRole", data={
             "RoleId": RoleId, 
         })
 
     async def Core_DeleteRoleAsync(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/DeleteRole", data={
             "RoleId": RoleId, 
         })
 
     def Core_RenameRole(self, RoleId: str, NewName: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param NewName: 
-        :type NewName: strFalse
+        :type NewName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/RenameRole", data={
             "RoleId": RoleId, 
             "NewName": NewName, 
         })
 
     async def Core_RenameRoleAsync(self, RoleId: str, NewName: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param NewName: 
-        :type NewName: strFalse
+        :type NewName: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/RenameRole", data={
             "RoleId": RoleId, 
             "NewName": NewName, 
         })
 
     def Core_SetAMPRolePermission(self, RoleId: str, PermissionNode: str, Enabled: bool | None):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param PermissionNode: 
-        :type PermissionNode: strFalse
+        :type PermissionNode: str False
             AMP Type: String
         :param Enabled: 
-        :type Enabled: bool | NoneFalse
+        :type Enabled: bool | None False
             AMP Type: Nullable<Boolean>
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/SetAMPRolePermission", data={
             "RoleId": RoleId, 
             "PermissionNode": PermissionNode, 
             "Enabled": Enabled, 
         })
 
     async def Core_SetAMPRolePermissionAsync(self, RoleId: str, PermissionNode: str, Enabled: bool | None):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param PermissionNode: 
-        :type PermissionNode: strFalse
+        :type PermissionNode: str False
             AMP Type: String
         :param Enabled: 
-        :type Enabled: bool | NoneFalse
+        :type Enabled: bool | None False
             AMP Type: Nullable<Boolean>
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/SetAMPRolePermission", data={
             "RoleId": RoleId, 
             "PermissionNode": PermissionNode, 
             "Enabled": Enabled, 
         })
 
     def Core_GetAMPRolePermissions(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<IEnumerable<String>>
         """
         return self.APICall(endpoint="Core/GetAMPRolePermissions", data={
             "RoleId": RoleId, 
         })
 
     async def Core_GetAMPRolePermissionsAsync(self, RoleId: str):
         """
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<IEnumerable<String>>
         """
         return await self.APICallAsync(endpoint="Core/GetAMPRolePermissions", data={
             "RoleId": RoleId, 
         })
 
@@ -2995,74 +3003,74 @@
         :returns: AMP Type: ScheduleInfo
         """
         return await self.APICallAsync(endpoint="Core/GetScheduleData")
 
     def Core_AddEventTrigger(self, triggerId: str):
         """
         :param triggerId: 
-        :type triggerId: strFalse
+        :type triggerId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/AddEventTrigger", data={
             "triggerId": triggerId, 
         })
 
     async def Core_AddEventTriggerAsync(self, triggerId: str):
         """
         :param triggerId: 
-        :type triggerId: strFalse
+        :type triggerId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/AddEventTrigger", data={
             "triggerId": triggerId, 
         })
 
     def Core_RunEventTriggerImmediately(self, triggerId: str):
         """
         :param triggerId: 
-        :type triggerId: strFalse
+        :type triggerId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/RunEventTriggerImmediately", data={
             "triggerId": triggerId, 
         })
 
     async def Core_RunEventTriggerImmediatelyAsync(self, triggerId: str):
         """
         :param triggerId: 
-        :type triggerId: strFalse
+        :type triggerId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/RunEventTriggerImmediately", data={
             "triggerId": triggerId, 
         })
 
     def Core_AddIntervalTrigger(self, months: list[int], days: list[int], hours: list[int], minutes: list[int], daysOfMonth: list[int], description: str):
         """
         :param months: 
-        :type months: list[int]False
+        :type months: list[int] False
             AMP Type: Int32[]
         :param days: 
-        :type days: list[int]False
+        :type days: list[int] False
             AMP Type: Int32[]
         :param hours: 
-        :type hours: list[int]False
+        :type hours: list[int] False
             AMP Type: Int32[]
         :param minutes: 
-        :type minutes: list[int]False
+        :type minutes: list[int] False
             AMP Type: Int32[]
         :param daysOfMonth: 
-        :type daysOfMonth: list[int]False
+        :type daysOfMonth: list[int] False
             AMP Type: Int32[]
         :param description: 
-        :type description: strFalse
+        :type description: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/AddIntervalTrigger", data={
             "months": months, 
             "days": days, 
             "hours": hours, 
@@ -3070,30 +3078,30 @@
             "daysOfMonth": daysOfMonth, 
             "description": description, 
         })
 
     async def Core_AddIntervalTriggerAsync(self, months: list[int], days: list[int], hours: list[int], minutes: list[int], daysOfMonth: list[int], description: str):
         """
         :param months: 
-        :type months: list[int]False
+        :type months: list[int] False
             AMP Type: Int32[]
         :param days: 
-        :type days: list[int]False
+        :type days: list[int] False
             AMP Type: Int32[]
         :param hours: 
-        :type hours: list[int]False
+        :type hours: list[int] False
             AMP Type: Int32[]
         :param minutes: 
-        :type minutes: list[int]False
+        :type minutes: list[int] False
             AMP Type: Int32[]
         :param daysOfMonth: 
-        :type daysOfMonth: list[int]False
+        :type daysOfMonth: list[int] False
             AMP Type: Int32[]
         :param description: 
-        :type description: strFalse
+        :type description: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/AddIntervalTrigger", data={
             "months": months, 
             "days": days, 
             "hours": hours, 
@@ -3101,55 +3109,55 @@
             "daysOfMonth": daysOfMonth, 
             "description": description, 
         })
 
     def Core_GetTimeIntervalTrigger(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: TimeIntervalTrigger
         """
         return self.APICall(endpoint="Core/GetTimeIntervalTrigger", data={
             "Id": Id, 
         })
 
     async def Core_GetTimeIntervalTriggerAsync(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: TimeIntervalTrigger
         """
         return await self.APICallAsync(endpoint="Core/GetTimeIntervalTrigger", data={
             "Id": Id, 
         })
 
     def Core_EditIntervalTrigger(self, Id: str, months: list[int], days: list[int], hours: list[int], minutes: list[int], daysOfMonth: list[int], description: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param months: 
-        :type months: list[int]False
+        :type months: list[int] False
             AMP Type: Int32[]
         :param days: 
-        :type days: list[int]False
+        :type days: list[int] False
             AMP Type: Int32[]
         :param hours: 
-        :type hours: list[int]False
+        :type hours: list[int] False
             AMP Type: Int32[]
         :param minutes: 
-        :type minutes: list[int]False
+        :type minutes: list[int] False
             AMP Type: Int32[]
         :param daysOfMonth: 
-        :type daysOfMonth: list[int]False
+        :type daysOfMonth: list[int] False
             AMP Type: Int32[]
         :param description: 
-        :type description: strFalse
+        :type description: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/EditIntervalTrigger", data={
             "Id": Id, 
             "months": months, 
             "days": days, 
@@ -3158,33 +3166,33 @@
             "daysOfMonth": daysOfMonth, 
             "description": description, 
         })
 
     async def Core_EditIntervalTriggerAsync(self, Id: str, months: list[int], days: list[int], hours: list[int], minutes: list[int], daysOfMonth: list[int], description: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param months: 
-        :type months: list[int]False
+        :type months: list[int] False
             AMP Type: Int32[]
         :param days: 
-        :type days: list[int]False
+        :type days: list[int] False
             AMP Type: Int32[]
         :param hours: 
-        :type hours: list[int]False
+        :type hours: list[int] False
             AMP Type: Int32[]
         :param minutes: 
-        :type minutes: list[int]False
+        :type minutes: list[int] False
             AMP Type: Int32[]
         :param daysOfMonth: 
-        :type daysOfMonth: list[int]False
+        :type daysOfMonth: list[int] False
             AMP Type: Int32[]
         :param description: 
-        :type description: strFalse
+        :type description: str False
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/EditIntervalTrigger", data={
             "Id": Id, 
             "months": months, 
             "days": days, 
@@ -3193,200 +3201,200 @@
             "daysOfMonth": daysOfMonth, 
             "description": description, 
         })
 
     def Core_SetTriggerEnabled(self, Id: str, Enabled: bool):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param Enabled: 
-        :type Enabled: boolFalse
+        :type Enabled: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/SetTriggerEnabled", data={
             "Id": Id, 
             "Enabled": Enabled, 
         })
 
     async def Core_SetTriggerEnabledAsync(self, Id: str, Enabled: bool):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :param Enabled: 
-        :type Enabled: boolFalse
+        :type Enabled: bool False
             AMP Type: Boolean
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/SetTriggerEnabled", data={
             "Id": Id, 
             "Enabled": Enabled, 
         })
 
     def Core_AddTask(self, TriggerID: str, MethodID: str, ParameterMapping: dict[str, str]):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param MethodID: 
-        :type MethodID: strFalse
+        :type MethodID: str False
             AMP Type: String
         :param ParameterMapping: 
-        :type ParameterMapping: dict[str, str]False
+        :type ParameterMapping: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/AddTask", data={
             "TriggerID": TriggerID, 
             "MethodID": MethodID, 
             "ParameterMapping": ParameterMapping, 
         })
 
     async def Core_AddTaskAsync(self, TriggerID: str, MethodID: str, ParameterMapping: dict[str, str]):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param MethodID: 
-        :type MethodID: strFalse
+        :type MethodID: str False
             AMP Type: String
         :param ParameterMapping: 
-        :type ParameterMapping: dict[str, str]False
+        :type ParameterMapping: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/AddTask", data={
             "TriggerID": TriggerID, 
             "MethodID": MethodID, 
             "ParameterMapping": ParameterMapping, 
         })
 
     def Core_EditTask(self, TriggerID: str, TaskID: str, ParameterMapping: dict[str, str]):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :param ParameterMapping: 
-        :type ParameterMapping: dict[str, str]False
+        :type ParameterMapping: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/EditTask", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
             "ParameterMapping": ParameterMapping, 
         })
 
     async def Core_EditTaskAsync(self, TriggerID: str, TaskID: str, ParameterMapping: dict[str, str]):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :param ParameterMapping: 
-        :type ParameterMapping: dict[str, str]False
+        :type ParameterMapping: dict[str, str] False
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/EditTask", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
             "ParameterMapping": ParameterMapping, 
         })
 
     def Core_ChangeTaskOrder(self, TriggerID: str, TaskID: str, NewOrder: int):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :param NewOrder: 
-        :type NewOrder: intFalse
+        :type NewOrder: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/ChangeTaskOrder", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
             "NewOrder": NewOrder, 
         })
 
     async def Core_ChangeTaskOrderAsync(self, TriggerID: str, TaskID: str, NewOrder: int):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :param NewOrder: 
-        :type NewOrder: intFalse
+        :type NewOrder: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/ChangeTaskOrder", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
             "NewOrder": NewOrder, 
         })
 
     def Core_DeleteTask(self, TriggerID: str, TaskID: str):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/DeleteTask", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
         })
 
     async def Core_DeleteTaskAsync(self, TriggerID: str, TaskID: str):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :param TaskID: 
-        :type TaskID: strFalse
+        :type TaskID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/DeleteTask", data={
             "TriggerID": TriggerID, 
             "TaskID": TaskID, 
         })
 
     def Core_DeleteTrigger(self, TriggerID: str):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/DeleteTrigger", data={
             "TriggerID": TriggerID, 
         })
 
     async def Core_DeleteTriggerAsync(self, TriggerID: str):
         """
         :param TriggerID: 
-        :type TriggerID: strFalse
+        :type TriggerID: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/DeleteTrigger", data={
             "TriggerID": TriggerID, 
         })
 
@@ -3403,27 +3411,27 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="Core/GetActiveAMPSessions")
 
     def Core_EndUserSession(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="Core/EndUserSession", data={
             "Id": Id, 
         })
 
     async def Core_EndUserSessionAsync(self, Id: str):
         """
         :param Id: 
-        :type Id: strFalse
+        :type Id: str False
             AMP Type: Guid
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="Core/EndUserSession", data={
             "Id": Id, 
         })
@@ -3439,26 +3447,26 @@
         :returns: AMP Type: Task<IEnumerable<UserInfoSummary>>
         """
         return await self.APICallAsync(endpoint="Core/GetAMPUsersSummary")
 
     def Core_GetAMPUserInfo(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<UserInfo>
         """
         return self.APICall(endpoint="Core/GetAMPUserInfo", data={
             "Username": Username, 
         })
 
     async def Core_GetAMPUserInfoAsync(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<UserInfo>
         """
         return await self.APICallAsync(endpoint="Core/GetAMPUserInfo", data={
             "Username": Username, 
         })
 
@@ -3473,40 +3481,40 @@
         :returns: AMP Type: Task<IEnumerable<UserInfo>>
         """
         return await self.APICallAsync(endpoint="Core/GetAllAMPUserInfo")
 
     def Core_SetAMPUserRoleMembership(self, UserId: str, RoleId: str, IsMember: bool):
         """
         :param UserId: 
-        :type UserId: strFalse
+        :type UserId: str False
             AMP Type: Guid
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param IsMember: 
-        :type IsMember: boolFalse
+        :type IsMember: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/SetAMPUserRoleMembership", data={
             "UserId": UserId, 
             "RoleId": RoleId, 
             "IsMember": IsMember, 
         })
 
     async def Core_SetAMPUserRoleMembershipAsync(self, UserId: str, RoleId: str, IsMember: bool):
         """
         :param UserId: 
-        :type UserId: strFalse
+        :type UserId: str False
             AMP Type: Guid
         :param RoleId: 
-        :type RoleId: strFalse
+        :type RoleId: str False
             AMP Type: Guid
         :param IsMember: 
-        :type IsMember: boolFalse
+        :type IsMember: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/SetAMPUserRoleMembership", data={
             "UserId": UserId, 
             "RoleId": RoleId, 
             "IsMember": IsMember, 
@@ -3525,74 +3533,74 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="Core/GetPermissionsSpec")
 
     def Core_CreateUser(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult<Guid>>
         """
         return self.APICall(endpoint="Core/CreateUser", data={
             "Username": Username, 
         })
 
     async def Core_CreateUserAsync(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult<Guid>>
         """
         return await self.APICallAsync(endpoint="Core/CreateUser", data={
             "Username": Username, 
         })
 
     def Core_DeleteUser(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/DeleteUser", data={
             "Username": Username, 
         })
 
     async def Core_DeleteUserAsync(self, Username: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/DeleteUser", data={
             "Username": Username, 
         })
 
     def Core_UpdateUserInfo(self, Username: str, Disabled: bool, PasswordExpires: bool, CannotChangePassword: bool, MustChangePassword: bool, EmailAddress: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param Disabled: 
-        :type Disabled: boolFalse
+        :type Disabled: bool False
             AMP Type: Boolean
         :param PasswordExpires: 
-        :type PasswordExpires: boolFalse
+        :type PasswordExpires: bool False
             AMP Type: Boolean
         :param CannotChangePassword: 
-        :type CannotChangePassword: boolFalse
+        :type CannotChangePassword: bool False
             AMP Type: Boolean
         :param MustChangePassword: 
-        :type MustChangePassword: boolFalse
+        :type MustChangePassword: bool False
             AMP Type: Boolean
         :param EmailAddress: 
-        :type EmailAddress: strTrue
+        :type EmailAddress: str True
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/UpdateUserInfo", data={
             "Username": Username, 
             "Disabled": Disabled, 
             "PasswordExpires": PasswordExpires, 
@@ -3600,30 +3608,30 @@
             "MustChangePassword": MustChangePassword, 
             "EmailAddress": EmailAddress, 
         })
 
     async def Core_UpdateUserInfoAsync(self, Username: str, Disabled: bool, PasswordExpires: bool, CannotChangePassword: bool, MustChangePassword: bool, EmailAddress: str):
         """
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param Disabled: 
-        :type Disabled: boolFalse
+        :type Disabled: bool False
             AMP Type: Boolean
         :param PasswordExpires: 
-        :type PasswordExpires: boolFalse
+        :type PasswordExpires: bool False
             AMP Type: Boolean
         :param CannotChangePassword: 
-        :type CannotChangePassword: boolFalse
+        :type CannotChangePassword: bool False
             AMP Type: Boolean
         :param MustChangePassword: 
-        :type MustChangePassword: boolFalse
+        :type MustChangePassword: bool False
             AMP Type: Boolean
         :param EmailAddress: 
-        :type EmailAddress: strTrue
+        :type EmailAddress: str True
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/UpdateUserInfo", data={
             "Username": Username, 
             "Disabled": Disabled, 
             "PasswordExpires": PasswordExpires, 
@@ -3643,62 +3651,62 @@
         :returns: AMP Type: ActionResult<String>
         """
         return await self.APICallAsync(endpoint="Core/GetWebauthnChallenge")
 
     def Core_GetWebauthnCredentialIDs(self, username: str):
         """
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :returns: AMP Type: WebauthnLoginInfo
         """
         return self.APICall(endpoint="Core/GetWebauthnCredentialIDs", data={
             "username": username, 
         })
 
     async def Core_GetWebauthnCredentialIDsAsync(self, username: str):
         """
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :returns: AMP Type: WebauthnLoginInfo
         """
         return await self.APICallAsync(endpoint="Core/GetWebauthnCredentialIDs", data={
             "username": username, 
         })
 
     def Core_WebauthnRegister(self, attestationObject: str, clientDataJSON: str, description: str):
         """
         :param attestationObject: 
-        :type attestationObject: strFalse
+        :type attestationObject: str False
             AMP Type: String
         :param clientDataJSON: 
-        :type clientDataJSON: strFalse
+        :type clientDataJSON: str False
             AMP Type: String
         :param description: 
-        :type description: strTrue
+        :type description: str True
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/WebauthnRegister", data={
             "attestationObject": attestationObject, 
             "clientDataJSON": clientDataJSON, 
             "description": description, 
         })
 
     async def Core_WebauthnRegisterAsync(self, attestationObject: str, clientDataJSON: str, description: str):
         """
         :param attestationObject: 
-        :type attestationObject: strFalse
+        :type attestationObject: str False
             AMP Type: String
         :param clientDataJSON: 
-        :type clientDataJSON: strFalse
+        :type clientDataJSON: str False
             AMP Type: String
         :param description: 
-        :type description: strTrue
+        :type description: str True
             AMP Type: String
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/WebauthnRegister", data={
             "attestationObject": attestationObject, 
             "clientDataJSON": clientDataJSON, 
             "description": description, 
@@ -3717,249 +3725,249 @@
         :rtype: list
         """
         return await self.APICallAsync(endpoint="Core/GetWebauthnCredentialSummaries")
 
     def Core_RevokeWebauthnCredential(self, ID: int):
         """
         :param ID: 
-        :type ID: intFalse
+        :type ID: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/RevokeWebauthnCredential", data={
             "ID": ID, 
         })
 
     async def Core_RevokeWebauthnCredentialAsync(self, ID: int):
         """
         :param ID: 
-        :type ID: intFalse
+        :type ID: int False
             AMP Type: Int32
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/RevokeWebauthnCredential", data={
             "ID": ID, 
         })
 
     def Core_UpdateAccountInfo(self, EmailAddress: str, TwoFactorPIN: str):
         """
         :param EmailAddress: 
-        :type EmailAddress: strFalse
+        :type EmailAddress: str False
             AMP Type: String
         :param TwoFactorPIN: 
-        :type TwoFactorPIN: strFalse
+        :type TwoFactorPIN: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/UpdateAccountInfo", data={
             "EmailAddress": EmailAddress, 
             "TwoFactorPIN": TwoFactorPIN, 
         })
 
     async def Core_UpdateAccountInfoAsync(self, EmailAddress: str, TwoFactorPIN: str):
         """
         :param EmailAddress: 
-        :type EmailAddress: strFalse
+        :type EmailAddress: str False
             AMP Type: String
         :param TwoFactorPIN: 
-        :type TwoFactorPIN: strFalse
+        :type TwoFactorPIN: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/UpdateAccountInfo", data={
             "EmailAddress": EmailAddress, 
             "TwoFactorPIN": TwoFactorPIN, 
         })
 
     def Core_EnableTwoFactor(self, Username: str, Password: str):
         """Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param Password: 
-        :type Password: strFalse
+        :type Password: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult<TwoFactorSetupInfo>>
         """
         return self.APICall(endpoint="Core/EnableTwoFactor", data={
             "Username": Username, 
             "Password": Password, 
         })
 
     async def Core_EnableTwoFactorAsync(self, Username: str, Password: str):
         """Sets up two-factor authentication for the given user. ConfirmTwoFactorSetup must be invoked to complete setup.
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param Password: 
-        :type Password: strFalse
+        :type Password: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult<TwoFactorSetupInfo>>
         """
         return await self.APICallAsync(endpoint="Core/EnableTwoFactor", data={
             "Username": Username, 
             "Password": Password, 
         })
 
     def Core_ConfirmTwoFactorSetup(self, Username: str, TwoFactorCode: str):
         """Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param TwoFactorCode: 
-        :type TwoFactorCode: strFalse
+        :type TwoFactorCode: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/ConfirmTwoFactorSetup", data={
             "Username": Username, 
             "TwoFactorCode": TwoFactorCode, 
         })
 
     async def Core_ConfirmTwoFactorSetupAsync(self, Username: str, TwoFactorCode: str):
         """Completes two-factor setup by supplying a valid two factor code based on the secret provided by EnableTwoFactor
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param TwoFactorCode: 
-        :type TwoFactorCode: strFalse
+        :type TwoFactorCode: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/ConfirmTwoFactorSetup", data={
             "Username": Username, 
             "TwoFactorCode": TwoFactorCode, 
         })
 
     def Core_DisableTwoFactor(self, Password: str, TwoFactorCode: str):
         """
         :param Password: 
-        :type Password: strFalse
+        :type Password: str False
             AMP Type: String
         :param TwoFactorCode: 
-        :type TwoFactorCode: strFalse
+        :type TwoFactorCode: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/DisableTwoFactor", data={
             "Password": Password, 
             "TwoFactorCode": TwoFactorCode, 
         })
 
     async def Core_DisableTwoFactorAsync(self, Password: str, TwoFactorCode: str):
         """
         :param Password: 
-        :type Password: strFalse
+        :type Password: str False
             AMP Type: String
         :param TwoFactorCode: 
-        :type TwoFactorCode: strFalse
+        :type TwoFactorCode: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/DisableTwoFactor", data={
             "Password": Password, 
             "TwoFactorCode": TwoFactorCode, 
         })
 
     def Core_ResetUserPassword(self, Username: str, NewPassword: str):
         """For administrative users to alter the password of another user
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param NewPassword: 
-        :type NewPassword: strFalse
+        :type NewPassword: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/ResetUserPassword", data={
             "Username": Username, 
             "NewPassword": NewPassword, 
         })
 
     async def Core_ResetUserPasswordAsync(self, Username: str, NewPassword: str):
         """For administrative users to alter the password of another user
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param NewPassword: 
-        :type NewPassword: strFalse
+        :type NewPassword: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/ResetUserPassword", data={
             "Username": Username, 
             "NewPassword": NewPassword, 
         })
 
     def Core_DeleteInstanceUsers(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/DeleteInstanceUsers", data={
             "InstanceId": InstanceId, 
         })
 
     async def Core_DeleteInstanceUsersAsync(self, InstanceId: str):
         """
         :param InstanceId: 
-        :type InstanceId: strFalse
+        :type InstanceId: str False
             AMP Type: Guid
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/DeleteInstanceUsers", data={
             "InstanceId": InstanceId, 
         })
 
     def Core_ChangeUserPassword(self, Username: str, OldPassword: str, NewPassword: str, TwoFactorPIN: str):
         """For a user to change their own password, requires knowing the old password
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param OldPassword: 
-        :type OldPassword: strFalse
+        :type OldPassword: str False
             AMP Type: String
         :param NewPassword: 
-        :type NewPassword: strFalse
+        :type NewPassword: str False
             AMP Type: String
         :param TwoFactorPIN: 
-        :type TwoFactorPIN: strFalse
+        :type TwoFactorPIN: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return self.APICall(endpoint="Core/ChangeUserPassword", data={
             "Username": Username, 
             "OldPassword": OldPassword, 
             "NewPassword": NewPassword, 
             "TwoFactorPIN": TwoFactorPIN, 
         })
 
     async def Core_ChangeUserPasswordAsync(self, Username: str, OldPassword: str, NewPassword: str, TwoFactorPIN: str):
         """For a user to change their own password, requires knowing the old password
             
         :param Username: 
-        :type Username: strFalse
+        :type Username: str False
             AMP Type: String
         :param OldPassword: 
-        :type OldPassword: strFalse
+        :type OldPassword: str False
             AMP Type: String
         :param NewPassword: 
-        :type NewPassword: strFalse
+        :type NewPassword: str False
             AMP Type: String
         :param TwoFactorPIN: 
-        :type TwoFactorPIN: strFalse
+        :type TwoFactorPIN: str False
             AMP Type: String
         :returns: AMP Type: Task<ActionResult>
         """
         return await self.APICallAsync(endpoint="Core/ChangeUserPassword", data={
             "Username": Username, 
             "OldPassword": OldPassword, 
             "NewPassword": NewPassword, 
@@ -4011,27 +4019,27 @@
         :rtype: dict[str, str]
         """
         return await self.APICallAsync(endpoint="Core/GetUserList")
 
     def Core_CurrentSessionHasPermission(self, PermissionNode: str):
         """
         :param PermissionNode: 
-        :type PermissionNode: strFalse
+        :type PermissionNode: str False
             AMP Type: String
         :returns: AMP Type: Boolean
         :rtype: bool
         """
         return self.APICall(endpoint="Core/CurrentSessionHasPermission", data={
             "PermissionNode": PermissionNode, 
         })
 
     async def Core_CurrentSessionHasPermissionAsync(self, PermissionNode: str):
         """
         :param PermissionNode: 
-        :type PermissionNode: strFalse
+        :type PermissionNode: str False
             AMP Type: String
         :returns: AMP Type: Boolean
         :rtype: bool
         """
         return await self.APICallAsync(endpoint="Core/CurrentSessionHasPermission", data={
             "PermissionNode": PermissionNode, 
         })
@@ -4044,14 +4052,28 @@
 
     async def Core_GetTasksAsync(self):
         """
         :returns: AMP Type: IEnumerable<RunningTask>
         """
         return await self.APICallAsync(endpoint="Core/GetTasks")
 
+    def Core_GetPortSummaries(self):
+        """
+        :returns: AMP Type: IEnumerable<ListeningPortSummary>
+        :rtype: list
+        """
+        return self.APICall(endpoint="Core/GetPortSummaries")
+
+    async def Core_GetPortSummariesAsync(self):
+        """
+        :returns: AMP Type: IEnumerable<ListeningPortSummary>
+        :rtype: list
+        """
+        return await self.APICallAsync(endpoint="Core/GetPortSummaries")
+
     def Core_GetStatus(self):
         """
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return self.APICall(endpoint="Core/GetStatus")
 
@@ -4061,48 +4083,48 @@
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="Core/GetStatus")
 
     def Core_CancelTask(self, TaskId: str):
         """
         :param TaskId: 
-        :type TaskId: strFalse
+        :type TaskId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/CancelTask", data={
             "TaskId": TaskId, 
         })
 
     async def Core_CancelTaskAsync(self, TaskId: str):
         """
         :param TaskId: 
-        :type TaskId: strFalse
+        :type TaskId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/CancelTask", data={
             "TaskId": TaskId, 
         })
 
     def Core_DismissTask(self, TaskId: str):
         """
         :param TaskId: 
-        :type TaskId: strFalse
+        :type TaskId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="Core/DismissTask", data={
             "TaskId": TaskId, 
         })
 
     async def Core_DismissTaskAsync(self, TaskId: str):
         """
         :param TaskId: 
-        :type TaskId: strFalse
+        :type TaskId: str False
             AMP Type: Guid
         :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="Core/DismissTask", data={
             "TaskId": TaskId, 
         })
 
@@ -4118,28 +4140,28 @@
         """
         return await self.APICallAsync(endpoint="Core/DismissAllTasks")
 
     def Core_GetUserInfo(self, UID: str):
         """Provides information about a given in-application user (as opposed to AMP system users)
             
         :param UID: 
-        :type UID: strFalse
+        :type UID: str False
             AMP Type: String
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return self.APICall(endpoint="Core/GetUserInfo", data={
             "UID": UID, 
         })
 
     async def Core_GetUserInfoAsync(self, UID: str):
         """Provides information about a given in-application user (as opposed to AMP system users)
             
         :param UID: 
-        :type UID: strFalse
+        :type UID: str False
             AMP Type: String
         :returns: AMP Type: JObject
         :rtype: dict
         """
         return await self.APICallAsync(endpoint="Core/GetUserInfo", data={
             "UID": UID, 
         })
@@ -4303,103 +4325,103 @@
         :returns: AMP Type: Object
         """
         return await self.APICallAsync(endpoint="Core/GetUserActionsSpec")
 
     def Core_Login(self, username: str, password: str, token: str, rememberMe: bool):
         """
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :param token: 
-        :type token: strFalse
+        :type token: str False
             AMP Type: String
         :param rememberMe: 
-        :type rememberMe: boolFalse
+        :type rememberMe: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<JObject>
         """
         return self.APICall(endpoint="Core/Login", data={
             "username": username, 
             "password": password, 
             "token": token, 
             "rememberMe": rememberMe, 
         })
 
     async def Core_LoginAsync(self, username: str, password: str, token: str, rememberMe: bool):
         """
         :param username: 
-        :type username: strFalse
+        :type username: str False
             AMP Type: String
         :param password: 
-        :type password: strFalse
+        :type password: str False
             AMP Type: String
         :param token: 
-        :type token: strFalse
+        :type token: str False
             AMP Type: String
         :param rememberMe: 
-        :type rememberMe: boolFalse
+        :type rememberMe: bool False
             AMP Type: Boolean
         :returns: AMP Type: Task<JObject>
         """
         return await self.APICallAsync(endpoint="Core/Login", data={
             "username": username, 
             "password": password, 
             "token": token, 
             "rememberMe": rememberMe, 
         })
 
     def Core_GetRemoteLoginToken(self, Description: str, IsTemporary: bool):
         """
         :param Description: 
-        :type Description: strTrue
+        :type Description: str True
             AMP Type: String
         :param IsTemporary: 
-        :type IsTemporary: boolTrue
+        :type IsTemporary: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<String>
         """
         return self.APICall(endpoint="Core/GetRemoteLoginToken", data={
             "Description": Description, 
             "IsTemporary": IsTemporary, 
         })
 
     async def Core_GetRemoteLoginTokenAsync(self, Description: str, IsTemporary: bool):
         """
         :param Description: 
-        :type Description: strTrue
+        :type Description: str True
             AMP Type: String
         :param IsTemporary: 
-        :type IsTemporary: boolTrue
+        :type IsTemporary: bool True
             AMP Type: Boolean
         :returns: AMP Type: Task<String>
         """
         return await self.APICallAsync(endpoint="Core/GetRemoteLoginToken", data={
             "Description": Description, 
             "IsTemporary": IsTemporary, 
         })
 
     def Core_SendConsoleMessage(self, message: str):
         """
         :param message: 
-        :type message: strFalse
+        :type message: str False
             AMP Type: String
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="Core/SendConsoleMessage", data={
             "message": message, 
         })
 
     async def Core_SendConsoleMessageAsync(self, message: str):
         """
         :param message: 
-        :type message: strFalse
+        :type message: str False
             AMP Type: String
         :returns: AMP Type: Void
         :rtype: None
         """
         return await self.APICallAsync(endpoint="Core/SendConsoleMessage", data={
             "message": message, 
         })
```

### Comparing `ampapi-1.1.4/ampapi.egg-info/PKG-INFO` & `ampapi-1.1.5/ampapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.4/setup.cfg` & `ampapi-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.1.4
+version = 1.1.5
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```

