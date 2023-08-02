# Comparing `tmp/easyecs-0.2.3.tar.gz` & `tmp/easyecs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.2.3.tar", max compression
+gzip compressed data, was "easyecs-0.2.5.tar", max compression
```

## Comparing `easyecs-0.2.3.tar` & `easyecs-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     2230 2023-08-01 15:28:41.778321 easyecs-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/__init__.py
--rwxr-xr-x   0        0        0     7382 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0     3390 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1872 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     2770 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     7949 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12418 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1459 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2398 2023-08-01 15:28:41.798321 easyecs-0.2.3/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-01 15:28:41.798321 easyecs-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-02 13:17:02.752398 easyecs-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     7304 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     2825 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     7949 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0    12418 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     2398 2023-08-02 13:17:02.772399 easyecs-0.2.5/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-02 13:17:02.772399 easyecs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.2.5/PKG-INFO
```

### Comparing `easyecs-0.2.3/README.md` & `easyecs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/cli.py` & `easyecs-0.2.5/easyecs/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!python
 
 import time
-import boto3
 import click
 from easyecs.cloudformation.stack.create import create_stack
 from easyecs.cloudformation.stack.delete import delete_stack
 from easyecs.cloudformation.stack.update import update_stack
 from easyecs.cloudformation.template import create_template
 from easyecs.cloudformation.fetch import (
+    fetch_aws_account,
     fetch_containers,
     fetch_is_stack_created,
 )
 from easyecs.command import (
     run_nc_commands,
     create_port_forwards,
     execute_command,
@@ -111,15 +111,15 @@
         popen_proc.stdin.flush()
         popen_proc.wait()
 
 
 def action_run(ctx):
     no_docker_build = ctx.obj["no_docker_build"]
     force_redeployment = ctx.obj["force_redeployment"]
-    aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
+    aws_account = fetch_aws_account()
     cache_settings = load_settings(aws_account)
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
@@ -150,15 +150,15 @@
 
     exit(0)
 
 
 def action_dev(ctx):
     no_docker_build = ctx.obj["no_docker_build"]
     force_redeployment = ctx.obj["force_redeployment"]
-    aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
+    aws_account = fetch_aws_account()
     cache_settings = load_settings(aws_account)
     ecs_manifest = read_ecs_file()
     app_name = ecs_manifest.metadata.appname
     user = ecs_manifest.metadata.user
     aws_region = cache_settings["aws_region"]
     aws_account_id = cache_settings["aws_account_id"]
     vpc_id = cache_settings["vpc_id"]
```

### Comparing `easyecs-0.2.3/easyecs/cloudformation/fetch.py` & `easyecs-0.2.5/easyecs/cloudformation/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
     convert_containers_to_dict,
     convert_tags_to_dict,
 )
 
 from easyecs.helpers.selector import select_action
 
 
+def fetch_aws_account():
+    aws_account = boto3.client("iam").list_account_aliases()["AccountAliases"][0]
+    return aws_account
+
+
 def fetch_region():
     client = boto3.client("ec2")
     response = client.describe_regions()
     regions = response["Regions"]
     parsed_regions = [region["RegionName"] for region in regions]
     selected_region: str = select_action(parsed_regions, "Select your ECS region")
     return selected_region
```

### Comparing `easyecs-0.2.3/easyecs/cloudformation/stack/create.py` & `easyecs-0.2.5/easyecs/cloudformation/stack/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import json
 from typing import Dict
 
-import boto3
 from botocore.waiter import WaiterError
+from easyecs.cloudformation.client import get_client_cloudformation
 from easyecs.cloudformation.stack.delete import delete_stack
 
 from easyecs.helpers.color import Color
 from easyecs.helpers.common import load_template
 from easyecs.helpers.loader import Loader
 
 
 def create_cloudformation_stack(stack_name: str, template_body: Dict):
     """
     Sends a request to AWS to create a CloudFormation stack.
     """
-    client = boto3.client("cloudformation")
+    client = get_client_cloudformation()
     client.create_stack(
         StackName=stack_name,
         TemplateBody=json.dumps(template_body),
         Capabilities=["CAPABILITY_NAMED_IAM"],
     )
 
 
 def wait_for_stack_creation(stack_name: str):
     """
     Waits for the CloudFormation stack to be created.
     Throws an exception if the creation fails.
     """
-    client = boto3.client("cloudformation")
+    client = get_client_cloudformation()
     waiter = client.get_waiter("stack_create_complete")
     waiter.wait(StackName=stack_name)
 
 
 def handle_stack_creation_failure(e: WaiterError, stack_name: str):
     """
     Handles a CloudFormation stack creation failure.
```

### Comparing `easyecs-0.2.3/easyecs/cloudformation/stack/delete.py` & `easyecs-0.2.5/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/cloudformation/stack/update.py` & `easyecs-0.2.5/easyecs/cloudformation/stack/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import json
 from typing import Dict
 import boto3
 from botocore.utils import ClientError
+from easyecs.cloudformation.client import get_client_cloudformation
 from easyecs.command import run_force_new_deployment
 
 from easyecs.helpers.color import Color
 from easyecs.helpers.common import load_template
 from easyecs.helpers.loader import Loader
 
 
 def update_cloudformation_stack(stack_name: str, template_body: Dict):
     """
     Sends a request to AWS to update a CloudFormation stack.
     """
-    client = boto3.client("cloudformation")
+    client = get_client_cloudformation()
     client.update_stack(
         StackName=stack_name,
         TemplateBody=json.dumps(template_body),
         Capabilities=["CAPABILITY_NAMED_IAM"],
     )
 
 
 def wait_for_stack_update(stack_name: str):
     """
     Waits for the CloudFormation stack to be updated.
     Throws an exception if the update fails.
     """
-    client = boto3.client("cloudformation")
+    client = get_client_cloudformation()
     waiter = client.get_waiter("stack_update_complete")
     waiter.wait(StackName=stack_name)
 
 
 def wait_for_stack_rollback(stack_name: str):
     """
     Waits for the CloudFormation stack to be rolled back.
     """
-    client = boto3.client("cloudformation")
+    client = get_client_cloudformation()
     waiter = client.get_waiter("stack_rollback_complete")
     waiter.wait(StackName=stack_name)
 
 
 def handle_update_error(e: ClientError, stack_name: str, force_redeployment: bool):
     """
     Handles a CloudFormation stack update failure.
@@ -77,11 +78,11 @@
     cloudformation_template = load_template(stack_name)
 
     while True:
         try:
             update_cloudformation_stack(stack_name, cloudformation_template)
             wait_for_stack_update(stack_name)
             loader.stop()
-            break
         except ClientError as e:
             loader.stop_error()
             handle_update_error(e, stack_name, force_redeployment)
+        break
```

### Comparing `easyecs-0.2.3/easyecs/cloudformation/template/__init__.py` & `easyecs-0.2.5/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/command/__init__.py` & `easyecs-0.2.5/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/docker/__init__.py` & `easyecs-0.2.5/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/helpers/common.py` & `easyecs-0.2.5/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/helpers/loader.py` & `easyecs-0.2.5/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/helpers/selector.py` & `easyecs-0.2.5/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/helpers/settings.py` & `easyecs-0.2.5/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/easyecs/model/ecs.py` & `easyecs-0.2.5/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.2.3/pyproject.toml` & `easyecs-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.2.3"
+version = "0.2.5"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.2.3/PKG-INFO` & `easyecs-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.2.3
+Version: 0.2.5
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

