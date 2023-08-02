# Comparing `tmp/neulabs-cdk-constructs-0.5.2.tar.gz` & `tmp/neulabs-cdk-constructs-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.5.2.tar", last modified: Mon Jul 31 15:09:36 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.5.3.tar", last modified: Wed Aug  2 13:09:39 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.5.2.tar` & `neulabs-cdk-constructs-0.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   117850 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    49582 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.808113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-31 15:09:24.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:09:36.804113 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 15:09:36.000000 neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.247220 neulabs-cdk-constructs-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117579 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   306174 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    49782 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    47689 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-02 13:09:22.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:09:39.251220 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 13:09:39.000000 neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.5.2/LICENSE` & `neulabs-cdk-constructs-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/PKG-INFO` & `neulabs-cdk-constructs-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.2
+Version: 0.5.3
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.2/README.md` & `neulabs-cdk-constructs-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/setup.py` & `neulabs-cdk-constructs-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.5.2",
+    "version": "0.5.3",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,27 +27,27 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.5.2.jsii.tgz"
+            "neulabs-cdk-constructs@0.5.3.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib==2.89.0",
         "aws-cdk.aws-apigatewayv2-alpha==2.89.0.a0",
         "aws-cdk.aws-apigatewayv2-integrations-alpha==2.89.0.a0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.85.0, <2.0.0",
+        "jsii>=1.86.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.5.2",
+    "0.5.3",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.5.2.jsii.tgz",
+    "neulabs-cdk-constructs@0.5.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,19 +104,19 @@
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         new_relic_account_id: builtins.str,
-        new_relic_api_url_logs: EndpointUrlLogs,
-        new_relic_api_url_metrics: EndpointUrlMetrics,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
         cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
+        new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
@@ -125,19 +125,19 @@
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param new_relic_account_id: 
-        :param new_relic_api_url_logs: 
-        :param new_relic_api_url_metrics: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
         :param cloudwatch_metric_stream_props: 
+        :param new_relic_api_url_logs: 
+        :param new_relic_api_url_metrics: 
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
@@ -148,19 +148,19 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = NewRelicStackProps(
             new_relic_account_id=new_relic_account_id,
-            new_relic_api_url_logs=new_relic_api_url_logs,
-            new_relic_api_url_metrics=new_relic_api_url_metrics,
             new_relic_bucket_name=new_relic_bucket_name,
             new_relic_license_key=new_relic_license_key,
             cloudwatch_metric_stream_props=cloudwatch_metric_stream_props,
+            new_relic_api_url_logs=new_relic_api_url_logs,
+            new_relic_api_url_metrics=new_relic_api_url_metrics,
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
@@ -396,19 +396,19 @@
         "stack_name": "stackName",
         "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "new_relic_account_id": "newRelicAccountId",
-        "new_relic_api_url_logs": "newRelicApiUrlLogs",
-        "new_relic_api_url_metrics": "newRelicApiUrlMetrics",
         "new_relic_bucket_name": "newRelicBucketName",
         "new_relic_license_key": "newRelicLicenseKey",
         "cloudwatch_metric_stream_props": "cloudwatchMetricStreamProps",
+        "new_relic_api_url_logs": "newRelicApiUrlLogs",
+        "new_relic_api_url_metrics": "newRelicApiUrlMetrics",
     },
 )
 class NewRelicStackProps(_BaseStackProps_bfec638c):
     def __init__(
         self,
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
@@ -419,38 +419,38 @@
         stack_name: typing.Optional[builtins.str] = None,
         suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         new_relic_account_id: builtins.str,
-        new_relic_api_url_logs: EndpointUrlLogs,
-        new_relic_api_url_metrics: EndpointUrlMetrics,
         new_relic_bucket_name: builtins.str,
         new_relic_license_key: builtins.str,
         cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
+        new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param new_relic_account_id: 
-        :param new_relic_api_url_logs: 
-        :param new_relic_api_url_metrics: 
         :param new_relic_bucket_name: 
         :param new_relic_license_key: 
         :param cloudwatch_metric_stream_props: 
+        :param new_relic_api_url_logs: 
+        :param new_relic_api_url_metrics: 
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
         if isinstance(cloudwatch_metric_stream_props, dict):
             cloudwatch_metric_stream_props = CfnMetricStreamProps(**cloudwatch_metric_stream_props)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1b73444472d0b16a38d845ab8c4feabeadd9937eadb9c68ca1f7a002e868c7df)
@@ -462,24 +462,22 @@
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
             check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument new_relic_account_id", value=new_relic_account_id, expected_type=type_hints["new_relic_account_id"])
-            check_type(argname="argument new_relic_api_url_logs", value=new_relic_api_url_logs, expected_type=type_hints["new_relic_api_url_logs"])
-            check_type(argname="argument new_relic_api_url_metrics", value=new_relic_api_url_metrics, expected_type=type_hints["new_relic_api_url_metrics"])
             check_type(argname="argument new_relic_bucket_name", value=new_relic_bucket_name, expected_type=type_hints["new_relic_bucket_name"])
             check_type(argname="argument new_relic_license_key", value=new_relic_license_key, expected_type=type_hints["new_relic_license_key"])
             check_type(argname="argument cloudwatch_metric_stream_props", value=cloudwatch_metric_stream_props, expected_type=type_hints["cloudwatch_metric_stream_props"])
+            check_type(argname="argument new_relic_api_url_logs", value=new_relic_api_url_logs, expected_type=type_hints["new_relic_api_url_logs"])
+            check_type(argname="argument new_relic_api_url_metrics", value=new_relic_api_url_metrics, expected_type=type_hints["new_relic_api_url_metrics"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage": stage,
             "new_relic_account_id": new_relic_account_id,
-            "new_relic_api_url_logs": new_relic_api_url_logs,
-            "new_relic_api_url_metrics": new_relic_api_url_metrics,
             "new_relic_bucket_name": new_relic_bucket_name,
             "new_relic_license_key": new_relic_license_key,
         }
         if analytics_reporting is not None:
             self._values["analytics_reporting"] = analytics_reporting
         if cross_region_references is not None:
             self._values["cross_region_references"] = cross_region_references
@@ -497,14 +495,18 @@
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
         if cloudwatch_metric_stream_props is not None:
             self._values["cloudwatch_metric_stream_props"] = cloudwatch_metric_stream_props
+        if new_relic_api_url_logs is not None:
+            self._values["new_relic_api_url_logs"] = new_relic_api_url_logs
+        if new_relic_api_url_metrics is not None:
+            self._values["new_relic_api_url_metrics"] = new_relic_api_url_metrics
 
     @builtins.property
     def analytics_reporting(self) -> typing.Optional[builtins.bool]:
         '''Include runtime versioning information in this Stack.
 
         :default:
 
@@ -686,26 +688,14 @@
     @builtins.property
     def new_relic_account_id(self) -> builtins.str:
         result = self._values.get("new_relic_account_id")
         assert result is not None, "Required property 'new_relic_account_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def new_relic_api_url_logs(self) -> EndpointUrlLogs:
-        result = self._values.get("new_relic_api_url_logs")
-        assert result is not None, "Required property 'new_relic_api_url_logs' is missing"
-        return typing.cast(EndpointUrlLogs, result)
-
-    @builtins.property
-    def new_relic_api_url_metrics(self) -> EndpointUrlMetrics:
-        result = self._values.get("new_relic_api_url_metrics")
-        assert result is not None, "Required property 'new_relic_api_url_metrics' is missing"
-        return typing.cast(EndpointUrlMetrics, result)
-
-    @builtins.property
     def new_relic_bucket_name(self) -> builtins.str:
         result = self._values.get("new_relic_bucket_name")
         assert result is not None, "Required property 'new_relic_bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def new_relic_license_key(self) -> builtins.str:
@@ -714,14 +704,24 @@
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cloudwatch_metric_stream_props(self) -> typing.Optional[CfnMetricStreamProps]:
         result = self._values.get("cloudwatch_metric_stream_props")
         return typing.cast(typing.Optional[CfnMetricStreamProps], result)
 
+    @builtins.property
+    def new_relic_api_url_logs(self) -> typing.Optional[EndpointUrlLogs]:
+        result = self._values.get("new_relic_api_url_logs")
+        return typing.cast(typing.Optional[EndpointUrlLogs], result)
+
+    @builtins.property
+    def new_relic_api_url_metrics(self) -> typing.Optional[EndpointUrlMetrics]:
+        result = self._values.get("new_relic_api_url_metrics")
+        return typing.cast(typing.Optional[EndpointUrlMetrics], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -750,19 +750,19 @@
     pass
 
 def _typecheckingstub__3d16994fa6098e1a11bee3003bb87e23e040f04cdc0edc42f729eccb764b26ca(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     new_relic_account_id: builtins.str,
-    new_relic_api_url_logs: EndpointUrlLogs,
-    new_relic_api_url_metrics: EndpointUrlMetrics,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
     cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
+    new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
@@ -870,15 +870,15 @@
     stack_name: typing.Optional[builtins.str] = None,
     suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     new_relic_account_id: builtins.str,
-    new_relic_api_url_logs: EndpointUrlLogs,
-    new_relic_api_url_metrics: EndpointUrlMetrics,
     new_relic_bucket_name: builtins.str,
     new_relic_license_key: builtins.str,
     cloudwatch_metric_stream_props: typing.Optional[typing.Union[CfnMetricStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    new_relic_api_url_logs: typing.Optional[EndpointUrlLogs] = None,
+    new_relic_api_url_metrics: typing.Optional[EndpointUrlMetrics] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.5.2
+Version: 0.5.3
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.5.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.5.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.2.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.5.3.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

