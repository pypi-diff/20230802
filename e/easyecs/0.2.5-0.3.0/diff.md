# Comparing `tmp/easyecs-0.2.5.tar.gz` & `tmp/easyecs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.2.5.tar", max compression
+gzip compressed data, was "easyecs-0.3.0.tar", max compression
```

## Comparing `easyecs-0.2.5.tar` & `easyecs-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-02 13:17:02.752398 easyecs-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/__init__.py
--rwxr-xr-x   0        0        0     7304 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     2825 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     7949 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1459 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2398 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-02 13:17:02.772399 easyecs-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-02 20:41:14.802827 easyecs-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     7304 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     2825 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     8573 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:41:14.818827 easyecs-0.3.0/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2804 2023-08-02 20:41:14.822827 easyecs-0.3.0/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-02 20:41:14.822827 easyecs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.3.0/PKG-INFO
```

### Comparing `easyecs-0.2.5/README.md` & `easyecs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cli.py` & `easyecs-0.3.0/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cloudformation/fetch.py` & `easyecs-0.3.0/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cloudformation/stack/create.py` & `easyecs-0.3.0/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cloudformation/stack/delete.py` & `easyecs-0.3.0/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cloudformation/stack/update.py` & `easyecs-0.3.0/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/cloudformation/template/__init__.py` & `easyecs-0.3.0/easyecs/cloudformation/template/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,27 +167,33 @@
     from aws_cdk.aws_secretsmanager import Secret
     from aws_cdk.aws_ecs import (
         ContainerImage,
         LogDriver,
         FargateTaskDefinition,
         Secret as ECSSecret,
     )
+    from aws_cdk.aws_ecs import EfsVolumeConfiguration, MountPoint
 
     task_definition_name = f"{service_name}-task-definition"
     resource_limits = ecs_data.task_definition.resources.limits
     cpu_limit = resource_limits.cpu * 1024
     memory_limit = resource_limits.memory
     task_definition: FargateTaskDefinition = FargateTaskDefinition(
         stack,
         task_definition_name,
         task_role=task_role,
         execution_role=execution_role,
         cpu=cpu_limit,
         memory_limit_mib=memory_limit,
     )
+    for volume in ecs_data.task_definition.volumes:
+        efs_volume_configuration = EfsVolumeConfiguration(file_system_id=volume.id)
+        task_definition.add_volume(
+            name=volume.name, efs_volume_configuration=efs_volume_configuration
+        )
     container_definitions = ecs_data.task_definition.containers
     log_configuration = LogDriver.aws_logs(stream_prefix="ecs", log_group=log_group)
     for container_definition in container_definitions:
         name = container_definition.name
         image = container_definition.image
         user = container_definition.user
         resource_limits = container_definition.resources.limits
@@ -209,26 +215,33 @@
             secret_field = secret_definition.field
             secret_arn = secret_definition.arn
             secret = Secret.from_secret_complete_arn(
                 stack, f"{secret_name}_{name}", secret_arn
             )
             ecs_secret = ECSSecret.from_secrets_manager(secret, secret_field)
             secrets[secret_name] = ecs_secret
-        task_definition.add_container(
+        container = task_definition.add_container(
             id=name,
             container_name=name,
             image=ContainerImage.from_registry(image),
             command=command,
             logging=log_configuration,
             environment=environment,
             secrets=secrets,
             cpu=cpu,
             memory_limit_mib=memory,
             user=user,
         )
+        for volume in container_definition.volumes:
+            mount_point = MountPoint(
+                container_path=volume.mount_point,
+                read_only=False,
+                source_volume=volume.name,
+            )
+            container.add_mount_points(mount_point)
     return task_definition
 
 
 def create_ecs_service(
     stack, service_name, cluster, task_definition, subnets, security_group
 ):
     from aws_cdk.aws_ecs import FargateService
```

### Comparing `easyecs-0.2.5/easyecs/command/__init__.py` & `easyecs-0.3.0/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/docker/__init__.py` & `easyecs-0.3.0/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/helpers/common.py` & `easyecs-0.3.0/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/helpers/loader.py` & `easyecs-0.3.0/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/helpers/selector.py` & `easyecs-0.3.0/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/helpers/settings.py` & `easyecs-0.3.0/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.5/easyecs/model/ecs.py` & `easyecs-0.3.0/easyecs/model/ecs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from typing import Dict, List, Optional
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel, computed_field, field_validator
 
 
 class EcsFileMetadataModel(BaseModel):
     appname: str
     user: str = os.environ["USER"]
 
 
@@ -58,26 +58,33 @@
 class EcsFileSecretModel(BaseModel):
     name: str
     arn: str
     field: str
     active: bool = True
 
 
+class EcsFileVolumeModel(BaseModel):
+    name: str
+    id: str
+    mount_point: str
+
+
 class EcsFileContainerModel(BaseModel):
     name: str
     image: str
     user: str = "root"
     tty: bool = False
     command: Optional[str] = None
     resources: EcsFileResourcesModel
     build: Optional[EcsFileBuildModel] = None
     synchronize: Optional[EcsFileSynchronizeModel] = None
     port_forward: List[str] = []
     env: List[EcsFileEnvModel] = []
     secrets: List[EcsFileSecretModel] = []
+    volumes: List[EcsFileVolumeModel] = []
 
 
 class EcsTaskDefinitionModel(BaseModel):
     resources: EcsFileResourcesModel
     containers: List[EcsFileContainerModel]
 
     @field_validator("containers")
@@ -86,13 +93,21 @@
         if len(tty_containers) > 1:
             raise ValueError(
                 "More than one container has tty set to true:"
                 f" {', '.join(tty_containers)}."
             )
         return containers
 
+    @computed_field(return_type=List[EcsFileVolumeModel])
+    @property
+    def volumes(self) -> List[EcsFileVolumeModel]:
+        volumes = [
+            volume for container in self.containers for volume in container.volumes
+        ]
+        return volumes
+
 
 class EcsFileModel(BaseModel):
     metadata: EcsFileMetadataModel
     role: EcsFileRoleModel
     execution_role: EcsFileRoleModel
     task_definition: EcsTaskDefinitionModel
```

### Comparing `easyecs-0.2.5/pyproject.toml` & `easyecs-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.2.5"
+version = "0.3.0"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.2.5/PKG-INFO` & `easyecs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

