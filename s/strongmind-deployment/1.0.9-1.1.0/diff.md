# Comparing `tmp/strongmind_deployment-1.0.9-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 8492 bytes, number of entries: 8
+Zip file size: 11121 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx    11433 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     9638 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+-rw-r--r--  2.0 unx    11707 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 strongmind_deployment/dynamo.py
+-rw-r--r--  2.0 unx    10429 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
 -rw-r--r--  2.0 unx     2918 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      711 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/RECORD
-8 files, 26515 bytes uncompressed, 7234 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx     2097 b- defN 20-Feb-02 00:00 strongmind_deployment/secrets.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      889 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.0.dist-info/RECORD
+10 files, 34612 bytes uncompressed, 9585 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: strongmind_deployment/__init__.py
 Comment: 
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
+Filename: strongmind_deployment/dynamo.py
+Comment: 
+
 Filename: strongmind_deployment/rails.py
 Comment: 
 
 Filename: strongmind_deployment/redis.py
 Comment: 
 
-Filename: strongmind_deployment-1.0.9.dist-info/METADATA
+Filename: strongmind_deployment/secrets.py
+Comment: 
+
+Filename: strongmind_deployment-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.0.9.dist-info/WHEEL
+Filename: strongmind_deployment-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.0.9.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.0.9.dist-info/RECORD
+Filename: strongmind_deployment-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -2,14 +2,15 @@
 import os
 import re
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 from pulumi import Config, export, Output
+from pulumi_awsx.awsx import DefaultRoleWithPolicyArgs
 from pulumi_cloudflare import get_zone, Record
 
 
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
@@ -26,14 +27,15 @@
         self.container_image = kwargs.get('container_image')
         self.app_path = kwargs.get('app_path', './')
         self.container_port = kwargs.get('container_port', 3000)
         self.cpu = kwargs.get('cpu', 256)
         self.memory = kwargs.get("memory", 512)
         self.entry_point = kwargs.get('entry_point')
         self.env_vars = kwargs.get('env_vars', {})
+        self.secrets = kwargs.get('secrets', [])
         self.kwargs = kwargs
         self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
 
         stack = pulumi.get_stack()
         project = pulumi.get_project()
         project_stack = f"{project}-{stack}"
         if name != 'container':
@@ -66,18 +68,18 @@
             retention_in_days=14,
             name=f'/aws/ecs/{project_stack}',
             tags=self.tags
         )
         port_mappings = None
         if self.target_group is not None:
             port_mappings = [awsx.ecs.TaskDefinitionPortMappingArgs(
-                    container_port=self.container_port,
-                    host_port=self.container_port,
-                    target_group=self.target_group,
-                )]
+                container_port=self.container_port,
+                host_port=self.container_port,
+                target_group=self.target_group,
+            )]
 
         execution_role = aws.iam.Role(
             f"{project_stack}-exec-role",
             name=f"{project_stack}-exec-role",
             assume_role_policy=json.dumps(
                 {
                     "Version": "2008-10-17",
@@ -115,25 +117,27 @@
                                 "ecr:DescribeImages",
                                 "ecr:InitiateLayerUpload",
                                 "ecr:UploadLayerPart",
                                 "ecr:CompleteLayerUpload",
                                 "ecr:PutImage",
                                 "logs:CreateLogStream",
                                 "logs:PutLogEvents",
+                                "secretsmanager:GetSecretValue",
                             ],
                             "Effect": "Allow",
                             "Resource": "*",
                         }
                     ],
                 }
             ),
             opts=pulumi.ResourceOptions(parent=self),
         )
 
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
+            execution_role=DefaultRoleWithPolicyArgs(role_arn=execution_role.arn),
             skip_destroy=True,
             family=project_stack,
             container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
                 name=project_stack,
                 log_configuration=awsx.ecs.TaskDefinitionLogConfigurationArgs(
                     log_driver="awslogs",
                     options={
@@ -144,14 +148,15 @@
                 ),
                 image=self.container_image,
                 cpu=self.cpu,
                 memory=self.memory,
                 entry_point=self.entry_point,
                 essential=True,
                 port_mappings=port_mappings,
+                secrets=self.secrets,
                 environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
             )
         )
         service_name = 'service'
         if name != 'container':
             service_name = f'{name}-service'
         self.fargate_service = awsx.ecs.FargateService(
```

## strongmind_deployment/rails.py

```diff
@@ -4,53 +4,58 @@
 import pulumi
 import pulumi_random as random
 import pulumi_aws as aws
 from pulumi import export, Output
 
 from strongmind_deployment.container import ContainerComponent
 from strongmind_deployment.redis import RedisComponent, QueueComponent, CacheComponent
+from strongmind_deployment.secrets import SecretsComponent
 
 
 def sidekiq_present():  # pragma: no cover
     return os.path.exists('../Gemfile') and 'sidekiq' in open('../Gemfile').read()
 
 
 class RailsComponent(pulumi.ComponentResource):
-    """
-    RailsComponent is a resource that produces a Rails application running on AWS Fargate.
 
-    :param name: The _unique_ name of the resource.
-    :param opts: A bag of optional settings that control this resource's behavior.
-    :param env_vars: A dictionary of environment variables to pass to the Rails application.
-    :param queue_redis: Either True to create a default queue Redis instance or a RedisComponent to use. Defaults to True if sidekiq is in the Gemfile.
-    :param cache_redis: Either True to create a default cache Redis instance or a RedisComponent to use.
-    :param web_entry_point: The entry point for the web container. Defaults to `["sh", "-c",
-                                                              "rails db:prepare db:migrate db:seed && "
-                                                              "rails assets:precompile && "
-                                                              "rails server --port 3000 -b 0.0.0.0"]`
-    :param need_worker: Whether or not to create a worker container. Defaults to True if sidekiq is in the Gemfile.
-    :param worker_entry_point: The entry point for the worker container. Defaults to `["sh", "-c", "bundle exec sidekiq"]`
-    :param cpu: The number of CPU units to reserve for the web container. Defaults to 256.
-    :param memory: The amount of memory (in MiB) to allow the web container to use. Defaults to 512.
-    :param app_path: The path to the Rails application for the web. Defaults to `./`.
-    :param worker_cpu: The number of CPU units to reserve for the worker container. Defaults to 256.
-    :param worker_memory: The amount of memory (in MiB) to allow the worker container to use. Defaults to 512.
-    :param worker_app_path: The path to the Rails application for the worker. Defaults to `./`.
-    """
     def __init__(self, name, opts=None, **kwargs):
+        """
+        Resource that produces a Rails application running on AWS Fargate.
+
+        :param name: The _unique_ name of the resource.
+        :param opts: A bag of optional settings that control this resource's behavior.
+        :key env_vars: A dictionary of environment variables to pass to the Rails application.
+        :key queue_redis: Either True to create a default queue Redis instance or a RedisComponent to use. Defaults to True if sidekiq is in the Gemfile.
+        :key cache_redis: Either True to create a default cache Redis instance or a RedisComponent to use.
+        :key web_entry_point: The entry point for the web container. Defaults to `["sh", "-c",
+                                                                                "rails db:prepare db:migrate db:seed && "
+                                                                                "rails assets:precompile && "
+                                                                                "rails server --port 3000 -b 0.0.0.0"]`
+        :key need_worker: Whether to create a worker container. Defaults to True if sidekiq is in the Gemfile.
+        :key worker_entry_point: The entry point for the worker container. Defaults to `["sh", "-c", "bundle exec sidekiq"]`
+        :key cpu: The number of CPU units to reserve for the web container. Defaults to 256.
+        :key memory: The amount of memory (in MiB) to allow the web container to use. Defaults to 512.
+        :key app_path: The path to the Rails application for the web. Defaults to `./`.
+        :key worker_cpu: The number of CPU units to reserve for the worker container. Defaults to 256.
+        :key worker_memory: The amount of memory (in MiB) to allow the worker container to use. Defaults to 512.
+        :key worker_app_path: The path to the Rails application for the worker. Defaults to `./`.
+        :key dynamo_tables: A list of DynamoDB tables to create. Defaults to `[]`. Each table is a DynamoComponent.
+        """
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
         self.need_worker = None
         self.cname_record = None
         self.firewall_rule = None
         self.db_password = None
         self.web_container = None
         self.worker_container = None
+        self.secret = None
         self.rds_serverless_cluster_instance = None
         self.rds_serverless_cluster = None
         self.kwargs = kwargs
+        self.dynamo_tables = self.kwargs.get('dynamo_tables', [])
         self.env_vars = self.kwargs.get('env_vars', {})
 
         self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
 
         project = pulumi.get_project()
         stack = pulumi.get_stack()
         project_stack = f"{project}-{stack}"
@@ -60,16 +65,20 @@
             "repository": project,
             "service": project,
             "environment": self.env_name,
         }
 
         self.rds(project_stack)
 
+        self.setup_dynamo()
+
         self.setup_redis()
 
+        self.secrets()
+
         self.ecs()
 
         self.security()
 
         self.register_outputs({})
 
     def setup_redis(self):
@@ -124,20 +133,18 @@
             'RAILS_ENV': 'production'
         }
 
         self.env_vars.update(additional_env_vars)
         self.kwargs['env_vars'] = self.env_vars
         self.kwargs['container_image'] = container_image
 
-        web_entry_point = self.kwargs.get('web_entry_point', ["sh", "-c",
-                                                              "rails db:prepare db:migrate db:seed && "
-                                                              "rails assets:precompile && "
-                                                              "rails server --port 3000 -b 0.0.0.0"])
+        web_entry_point = self.kwargs.get('web_entry_point')
 
         self.kwargs['entry_point'] = web_entry_point
+        self.kwargs['secrets'] = self.secret.get_secrets()  # pragma: no cover
 
         self.web_container = ContainerComponent("container",
                                                 pulumi.ResourceOptions(parent=self),
                                                 **self.kwargs
                                                 )
 
         self.need_worker = self.kwargs.get('need_worker', None)
@@ -152,32 +159,41 @@
         worker_entry_point = self.kwargs.get('worker_entry_point', ["sh", "-c", "bundle exec sidekiq"])
         self.kwargs['entry_point'] = worker_entry_point
         self.kwargs['cpu'] = self.kwargs.get('worker_cpu')
         self.kwargs['memory'] = self.kwargs.get('worker_memory')
         self.kwargs['app_path'] = self.kwargs.get('worker_app_path')
         self.kwargs['need_load_balancer'] = False
         self.kwargs['ecs_cluster_arn'] = self.web_container.ecs_cluster_arn
+        self.kwargs['secrets'] = self.secret.get_secrets()  # pragma: no cover
         self.worker_container = ContainerComponent("worker",
                                                    pulumi.ResourceOptions(parent=self),
                                                    **self.kwargs
                                                    )
 
+    def secrets(self):
+        self.secret = SecretsComponent("secrets",
+                                       pulumi.ResourceOptions(parent=self),
+                                       **self.kwargs
+                                       )
+
     def rds(self, project_stack):
         self.db_password = random.RandomPassword("password",
                                                  length=30,
                                                  special=False)
         self.rds_serverless_cluster = aws.rds.Cluster(
             'rds_serverless_cluster',
             cluster_identifier=project_stack,
             engine='aurora-postgresql',
             engine_mode='provisioned',
             engine_version='15.2',
             database_name="app",
             master_username=project_stack.replace('-', '_'),
             master_password=self.db_password.result,
+            deletion_protection=True,
+            skip_final_snapshot=False,
             serverlessv2_scaling_configuration=aws.rds.ClusterServerlessv2ScalingConfigurationArgs(
                 min_capacity=0.5,
                 max_capacity=16,
             ),
             tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self,
                                         protect=True),
@@ -200,8 +216,13 @@
     def get_database_url(self):
         return Output.concat('postgres://',
                              self.rds_serverless_cluster.master_username,
                              ':',
                              self.rds_serverless_cluster.master_password,
                              '@',
                              self.rds_serverless_cluster.endpoint,
-                             ':5432/app')
+                             ':5432/app')
+
+    def setup_dynamo(self):
+        for table_component in self.dynamo_tables:
+            env_var_name = table_component._name.upper() + '_DYNAMO_TABLE_NAME'
+            self.env_vars[env_var_name] = table_component.table.name
```

## Comparing `strongmind_deployment-1.0.9.dist-info/METADATA` & `strongmind_deployment-1.1.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.0.9
+Version: 1.1.0
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.0.9.dist-info/licenses/LICENSE` & `strongmind_deployment-1.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

