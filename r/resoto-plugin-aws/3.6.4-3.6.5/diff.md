# Comparing `tmp/resoto-plugin-aws-3.6.4.tar.gz` & `tmp/resoto-plugin-aws-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.6.4.tar", last modified: Mon Jul 24 18:32:45 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.6.5.tar", last modified: Wed Aug  2 19:24:09 2023, max compression
```

## Comparing `resoto-plugin-aws-3.6.4.tar` & `resoto-plugin-aws-3.6.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.654960 resoto-plugin-aws-3.6.4/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.658961 resoto-plugin-aws-3.6.4/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.662961 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    19802 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   122318 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.658961 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:27:43.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.662961 resoto-plugin-aws-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.402792 resoto-plugin-aws-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-02 19:24:09.402792 resoto-plugin-aws-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.386791 resoto-plugin-aws-3.6.5/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.386791 resoto-plugin-aws-3.6.5/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.394791 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20809 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19802 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122318 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.386791 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:03.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 19:24:09.000000 resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 19:24:09.406792 resoto-plugin-aws-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.398791 resoto-plugin-aws-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:24:09.402792 resoto-plugin-aws-3.6.5/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 19:17:23.000000 resoto-plugin-aws-3.6.5/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.6.4/PKG-INFO` & `resoto-plugin-aws-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.4
+Version: 3.6.5
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.4/README.md` & `resoto-plugin-aws-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/pyproject.toml` & `resoto-plugin-aws-3.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.4",
+    "resotolib==3.6.5",
     "resotodata",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/configuration.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,18 @@
                     action=spec.api_action,
                     result_name=spec.result_property,
                     expected_errors=spec.expected_errors,
                     **kwargs,
                 )
                 cls.collect(items, builder)
                 if builder.config.collect_usage_metrics:
-                    cls.collect_usage_metrics(builder)
+                    try:
+                        cls.collect_usage_metrics(builder)
+                    except Exception as e:
+                        log.warning(f"Failed to collect usage metrics for {cls.__name__}: {e}")
             except Boto3Error as e:
                 msg = f"Error while collecting {cls.__name__} in region {builder.region.name}: {e}"
                 builder.core_feedback.error(msg, log)
                 raise
             except Exception as e:
                 msg = f"Error while collecting {cls.__name__} in region {builder.region.name}: {e}"
                 builder.core_feedback.info(msg, log)
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/route53.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,257 +1,250 @@
-from typing import ClassVar, Dict, Optional, Type, List
+from typing import ClassVar, Dict, Optional, List, Type
 
 from attrs import define, field
 
-from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec
-from resoto_plugin_aws.resource.ec2 import AwsEc2Subnet, AwsEc2SecurityGroup, AwsEc2Vpc, AwsEc2Instance
+from resoto_plugin_aws.aws_client import AwsClient
+from resoto_plugin_aws.resource.base import AwsResource, AwsApiSpec, GraphBuilder
 from resoto_plugin_aws.utils import ToDict
-from resotolib.baseresources import BaseLoadBalancer, ModelReference
+from resotolib.baseresources import (
+    BaseDNSZone,
+    BaseDNSRecord,
+    EdgeType,
+    BaseDNSRecordSet,
+    ModelReference,
+)
 from resotolib.graph import Graph
-from resotolib.json_bender import Bender, S, Bend, bend, ForallBend, K
+from resotolib.json_bender import F, Bender, S, Bend, ForallBend, bend
 from resotolib.types import Json
-from resoto_plugin_aws.aws_client import AwsClient
-
-service_name = "elb"
+from resotolib.utils import rrdata_as_dict
 
+service_name = "route53"
 
-# noinspection PyUnresolvedReferences
-class ElbTaggable:
-    def update_resource_tag(self, client: AwsClient, key: str, value: str) -> bool:
-        if isinstance(self, AwsResource):
-            if spec := self.api_spec:
-                client.call(
-                    aws_service=spec.service,
-                    action="add-tags",
-                    result_name=None,
-                    LoadBalancerNames=[self.name],
-                    Tags=[{"Key": key, "Value": value}],
-                )
-                return True
-            return False
-        return False
-
-    def delete_resource_tag(self, client: AwsClient, key: str) -> bool:
-        if isinstance(self, AwsResource):
-            if spec := self.api_spec:
-                client.call(
-                    aws_service=spec.service,
-                    action="remove-tags",
-                    result_name=None,
-                    LoadBalancerNames=[self.name],
-                    Tags=[{"Key": key}],
-                )
-                return True
-            return False
-        return False
 
-    @classmethod
-    def called_mutator_apis(cls) -> List[AwsApiSpec]:
-        return [
-            AwsApiSpec(service_name, "add-tags", override_iam_permission="elasticloadbalancing:AddTags"),
-            AwsApiSpec(service_name, "remove-tags", override_iam_permission="elasticloadbalancing:RemoveTags"),
-        ]
+@define(eq=False, slots=False)
+class AwsRoute53ZoneConfig:
+    kind: ClassVar[str] = "aws_route53_zone_config"
+    mapping: ClassVar[Dict[str, Bender]] = {"comment": S("Comment"), "private_zone": S("PrivateZone")}
+    comment: Optional[str] = field(default=None)
+    private_zone: Optional[bool] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsElbListener:
-    kind: ClassVar[str] = "aws_elb_listener"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "protocol": S("Protocol"),
-        "load_balancer_port": S("LoadBalancerPort"),
-        "instance_protocol": S("InstanceProtocol"),
-        "instance_port": S("InstancePort"),
-        "ssl_certificate_id": S("SSLCertificateId"),
-    }
-    protocol: Optional[str] = field(default=None)
-    load_balancer_port: Optional[int] = field(default=None)
-    instance_protocol: Optional[str] = field(default=None)
-    instance_port: Optional[int] = field(default=None)
-    ssl_certificate_id: Optional[str] = field(default=None)
+class AwsRoute53LinkedService:
+    kind: ClassVar[str] = "aws_route53_linked_service"
+    mapping: ClassVar[Dict[str, Bender]] = {"service_principal": S("ServicePrincipal"), "description": S("Description")}
+    service_principal: Optional[str] = field(default=None)
+    description: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsElbListenerDescription:
-    kind: ClassVar[str] = "aws_elb_listener_description"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "listener": S("Listener") >> Bend(AwsElbListener.mapping),
-        "policy_names": S("PolicyNames", default=[]),
-    }
-    listener: Optional[AwsElbListener] = field(default=None)
-    policy_names: List[str] = field(factory=list)
+class AwsRoute53Zone(AwsResource, BaseDNSZone):
+    kind: ClassVar[str] = "aws_route53_zone"
+    api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "list-hosted-zones", "HostedZones")
+    reference_kinds: ClassVar[ModelReference] = {
+        "successors": {
+            "default": ["aws_route53_resource_record_set"],
+            "delete": [],
+        }
+    }
+    mapping: ClassVar[Dict[str, Bender]] = {
+        "id": S("Id") >> F(lambda x: x.rsplit("/", 1)[-1]),  # remove leading "/hostedzones/"
+        "name": S("Name"),
+        "zone_caller_reference": S("CallerReference"),
+        "zone_config": S("Config") >> Bend(AwsRoute53ZoneConfig.mapping),
+        "zone_resource_record_set_count": S("ResourceRecordSetCount"),
+        "zone_linked_service": S("LinkedService") >> Bend(AwsRoute53LinkedService.mapping),
+    }
+    zone_caller_reference: Optional[str] = field(default=None)
+    zone_config: Optional[AwsRoute53ZoneConfig] = field(default=None)
+    zone_resource_record_set_count: Optional[int] = field(default=None)
+    zone_linked_service: Optional[AwsRoute53LinkedService] = field(default=None)
+
+    @classmethod
+    def called_collect_apis(cls) -> List[AwsApiSpec]:
+        return [
+            cls.api_spec,
+            AwsApiSpec(service_name, "list-resource-record-sets"),
+            AwsApiSpec(service_name, "list-tags-for-resource"),
+        ]
 
+    @classmethod
+    def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
+        def add_tags(zone: AwsRoute53Zone) -> None:
+            tags = builder.client.get(
+                service_name,
+                "list-tags-for-resource",
+                result_name="ResourceTagSet",
+                ResourceType="hostedzone",
+                ResourceId=zone.id,
+            )
+            if tags:
+                zone.tags = bend(S("Tags", default=[]) >> ToDict(), tags)
 
-@define(eq=False, slots=False)
-class AwsElbAppCookieStickinessPolicy:
-    kind: ClassVar[str] = "aws_elb_app_cookie_stickiness_policy"
-    mapping: ClassVar[Dict[str, Bender]] = {"policy_name": S("PolicyName"), "cookie_name": S("CookieName")}
-    policy_name: Optional[str] = field(default=None)
-    cookie_name: Optional[str] = field(default=None)
+        for js in json:
+            if zone := AwsRoute53Zone.from_api(js, builder):
+                builder.add_node(zone, js)
+                builder.submit_work(service_name, add_tags, zone)
+                for rs_js in builder.client.list(
+                    service_name, "list-resource-record-sets", "ResourceRecordSets", HostedZoneId=zone.id
+                ):
+                    if record_set := AwsRoute53ResourceRecordSet.from_api(rs_js, builder):
+                        builder.add_node(record_set, rs_js)
+                        builder.add_edge(zone, EdgeType.default, node=record_set)
+                        for data in record_set.record_values:
+                            record = AwsRoute53ResourceRecord(
+                                id=record_set.id,
+                                name=record_set.name,
+                                record_type=record_set.record_type,
+                                record_ttl=record_set.record_ttl or 0,
+                                record_data=data,
+                                **rrdata_as_dict(record_set.record_type, data),
+                            )
+                            builder.add_node(record, js)
+                            builder.add_edge(record_set, EdgeType.default, node=record)
+                            builder.add_edge(record_set, EdgeType.delete, node=record)
 
+    def update_resource_tag(self, client: AwsClient, key: str, value: str) -> bool:
+        client.call(
+            aws_service=service_name,
+            action="change-tags-for-resource",
+            result_name=None,
+            ResourceType="hostedzone",
+            ResourceId=self.id,
+            AddTags=[{"Key": key, "Value": value}],
+        )
+        return True
 
-@define(eq=False, slots=False)
-class AwsElbLBCookieStickinessPolicy:
-    kind: ClassVar[str] = "aws_elb_lb_cookie_stickiness_policy"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "policy_name": S("PolicyName"),
-        "cookie_expiration_period": S("CookieExpirationPeriod"),
-    }
-    policy_name: Optional[str] = field(default=None)
-    cookie_expiration_period: Optional[int] = field(default=None)
+    def delete_resource_tag(self, client: AwsClient, key: str) -> bool:
+        client.call(
+            aws_service=service_name,
+            action="change-tags-for-resource",
+            result_name=None,
+            ResourceType="hostedzone",
+            ResourceId=self.id,
+            RemoveTagKeys=[key],
+        )
+        return True
 
+    def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
+        client.call(
+            aws_service=service_name, action="delete-hosted-zone", result_name=None, Id=self.id.rsplit("/", 1)[-1]
+        )
+        return True
 
-@define(eq=False, slots=False)
-class AwsElbPolicies:
-    kind: ClassVar[str] = "aws_elb_policies"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "app_cookie_stickiness_policies": S("AppCookieStickinessPolicies", default=[])
-        >> ForallBend(AwsElbAppCookieStickinessPolicy.mapping),
-        "lb_cookie_stickiness_policies": S("LBCookieStickinessPolicies", default=[])
-        >> ForallBend(AwsElbLBCookieStickinessPolicy.mapping),
-        "other_policies": S("OtherPolicies", default=[]),
-    }
-    app_cookie_stickiness_policies: List[AwsElbAppCookieStickinessPolicy] = field(factory=list)
-    lb_cookie_stickiness_policies: List[AwsElbLBCookieStickinessPolicy] = field(factory=list)
-    other_policies: List[str] = field(factory=list)
+    @classmethod
+    def called_mutator_apis(cls) -> List[AwsApiSpec]:
+        return [
+            AwsApiSpec(service_name, "change-tags-for-resource"),
+            AwsApiSpec(service_name, "delete-hosted-zone"),
+        ]
 
 
 @define(eq=False, slots=False)
-class AwsElbBackendServerDescription:
-    kind: ClassVar[str] = "aws_elb_backend_server_description"
+class AwsRoute53GeoLocation:
+    kind: ClassVar[str] = "aws_route53_geo_location"
     mapping: ClassVar[Dict[str, Bender]] = {
-        "instance_port": S("InstancePort"),
-        "policy_names": S("PolicyNames", default=[]),
+        "continent_code": S("ContinentCode"),
+        "country_code": S("CountryCode"),
+        "subdivision_code": S("SubdivisionCode"),
     }
-    instance_port: Optional[int] = field(default=None)
-    policy_names: List[str] = field(factory=list)
+    continent_code: Optional[str] = field(default=None)
+    country_code: Optional[str] = field(default=None)
+    subdivision_code: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsElbHealthCheck:
-    kind: ClassVar[str] = "aws_elb_health_check"
+class AwsRoute53AliasTarget:
+    kind: ClassVar[str] = "aws_route53_alias_target"
     mapping: ClassVar[Dict[str, Bender]] = {
-        "target": S("Target"),
-        "interval": S("Interval"),
-        "timeout": S("Timeout"),
-        "unhealthy_threshold": S("UnhealthyThreshold"),
-        "healthy_threshold": S("HealthyThreshold"),
+        "hosted_zone_id": S("HostedZoneId"),
+        "dns_name": S("DNSName"),
+        "evaluate_target_health": S("EvaluateTargetHealth"),
     }
-    target: Optional[str] = field(default=None)
-    interval: Optional[int] = field(default=None)
-    timeout: Optional[int] = field(default=None)
-    unhealthy_threshold: Optional[int] = field(default=None)
-    healthy_threshold: Optional[int] = field(default=None)
+    hosted_zone_id: Optional[str] = field(default=None)
+    dns_name: Optional[str] = field(default=None)
+    evaluate_target_health: Optional[bool] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsElbSourceSecurityGroup:
-    kind: ClassVar[str] = "aws_elb_source_security_group"
-    mapping: ClassVar[Dict[str, Bender]] = {"owner_alias": S("OwnerAlias"), "group_name": S("GroupName")}
-    owner_alias: Optional[str] = field(default=None)
-    group_name: Optional[str] = field(default=None)
+class AwsRoute53CidrRoutingConfig:
+    kind: ClassVar[str] = "aws_route53_cidr_routing_config"
+    mapping: ClassVar[Dict[str, Bender]] = {"collection_id": S("CollectionId"), "location_name": S("LocationName")}
+    collection_id: Optional[str] = field(default=None)
+    location_name: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsElb(ElbTaggable, AwsResource, BaseLoadBalancer):
-    kind: ClassVar[str] = "aws_elb"
-    api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(
-        service_name,
-        "describe-load-balancers",
-        "LoadBalancerDescriptions",
-        override_iam_permission="elasticloadbalancing:DescribeLoadBalancers",
-    )
+class AwsRoute53ResourceRecord(AwsResource, BaseDNSRecord):
+    kind: ClassVar[str] = "aws_route53_resource_record"
     reference_kinds: ClassVar[ModelReference] = {
-        "predecessors": {
-            "default": ["aws_vpc", "aws_ec2_subnet", "aws_ec2_security_group"],
-            "delete": ["aws_vpc", "aws_ec2_subnet", "aws_ec2_security_group", "aws_ec2_instance"],
-        },
         "successors": {
-            "default": ["aws_ec2_instance"],
-        },
-    }
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("DNSName"),
-        "name": S("LoadBalancerName"),
-        "lb_type": K("elb"),
-        "ctime": S("CreatedTime"),
-        "backends": S("Instances", default=[]) >> ForallBend(S("InstanceId")),
-        "elb_canonical_hosted_zone_name": S("CanonicalHostedZoneName"),
-        "elb_canonical_hosted_zone_name_id": S("CanonicalHostedZoneNameID"),
-        "elb_listener_descriptions": S("ListenerDescriptions", default=[])
-        >> ForallBend(AwsElbListenerDescription.mapping),
-        "elb_policies": S("Policies") >> Bend(AwsElbPolicies.mapping),
-        "elb_backend_server_descriptions": S("BackendServerDescriptions", default=[])
-        >> ForallBend(AwsElbBackendServerDescription.mapping),
-        "elb_availability_zones": S("AvailabilityZones", default=[]),
-        "elb_health_check": S("HealthCheck") >> Bend(AwsElbHealthCheck.mapping),
-        "elb_source_security_group": S("SourceSecurityGroup") >> Bend(AwsElbSourceSecurityGroup.mapping),
-        "scheme": S("Scheme"),
+            "default": [],
+            "delete": [],
+        }
     }
-    scheme: Optional[str] = field(default=None)
-    elb_canonical_hosted_zone_name: Optional[str] = field(default=None)
-    elb_canonical_hosted_zone_name_id: Optional[str] = field(default=None)
-    elb_listener_descriptions: List[AwsElbListenerDescription] = field(factory=list)
-    elb_policies: Optional[AwsElbPolicies] = field(default=None)
-    elb_backend_server_descriptions: List[AwsElbBackendServerDescription] = field(factory=list)
-    elb_availability_zones: List[str] = field(factory=list)
-    elb_health_check: Optional[AwsElbHealthCheck] = field(default=None)
-    elb_source_security_group: Optional[AwsElbSourceSecurityGroup] = field(default=None)
-
-    @classmethod
-    def called_collect_apis(cls) -> List[AwsApiSpec]:
-        return [
-            cls.api_spec,
-            AwsApiSpec(
-                cls.api_spec.service,
-                "describe-tags",
-                override_iam_permission="elasticloadbalancing:DescribeTags",
-            ),
-        ]
 
     @classmethod
-    def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
-        def add_tags(elb: AwsElb) -> None:
-            tags = builder.client.list(
-                service_name,
-                "describe-tags",
-                "TagDescriptions",
-                LoadBalancerNames=[elb.name],
-                expected_errors=["LoadBalancerNotFound"],
-            )
-            if tags:
-                elb.tags = bend(S("Tags", default=[]) >> ToDict(), tags[0])
+    def service_name(cls) -> str:
+        return service_name
 
-        for js in json:
-            if instance := cls.from_api(js, builder):
-                builder.add_node(instance, js)
-                builder.submit_work(service_name, add_tags, instance)
-
-    def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        super().connect_in_graph(builder, source)
-        if vpc_id := source.get("VPCId"):
-            builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Vpc, id=vpc_id)
-        for subnet_id in source.get("Subnets", []):
-            builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Subnet, id=subnet_id)
-        for sg_id in source.get("SecurityGroups", []):
-            builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2SecurityGroup, id=sg_id)
-        for instance in self.backends:
-            builder.dependant_node(self, clazz=AwsEc2Instance, id=instance)
 
-    def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
-        client.call(
-            aws_service=self.api_spec.service,
-            action="delete-load-balancer",
-            result_name=None,
-            LoadBalancerName=self.name,
+@define(eq=False, slots=False)
+class AwsRoute53ResourceRecordSet(AwsResource, BaseDNSRecordSet):
+    kind: ClassVar[str] = "aws_route53_resource_record_set"
+    reference_kinds: ClassVar[ModelReference] = {
+        "successors": {
+            "default": ["aws_route53_resource_record"],
+            "delete": ["aws_route53_resource_record"],
+        }
+    }
+    mapping: ClassVar[Dict[str, Bender]] = {
+        "id": S("Name"),
+        "name": S("Name"),
+        "record_set_identifier": S("SetIdentifier"),
+        "record_type": S("Type"),
+        "record_weight": S("Weight"),
+        "record_region": S("Region"),
+        "record_geo_location": S("GeoLocation") >> Bend(AwsRoute53GeoLocation.mapping),
+        "record_fail_over": S("Failover"),
+        "record_multi_value_answer": S("MultiValueAnswer"),
+        "record_ttl": S("TTL"),
+        "record_values": S("ResourceRecords", default=[]) >> ForallBend(S("Value")),
+        "record_alias_target": S("AliasTarget") >> Bend(AwsRoute53AliasTarget.mapping),
+        "record_health_check_id": S("HealthCheckId"),
+        "record_traffic_policy_instance_id": S("TrafficPolicyInstanceId"),
+        "record_cidr_routing_config": S("CidrRoutingConfig") >> Bend(AwsRoute53CidrRoutingConfig.mapping),
+    }
+    record_name: Optional[str] = field(default=None)
+    record_set_identifier: Optional[str] = field(default=None)
+    record_weight: Optional[int] = field(default=None)
+    record_region: Optional[str] = field(default=None)
+    record_geo_location: Optional[AwsRoute53GeoLocation] = field(default=None)
+    record_fail_over: Optional[str] = field(default=None)
+    record_multi_value_answer: Optional[bool] = field(default=None)
+    record_alias_target: Optional[AwsRoute53AliasTarget] = field(default=None)
+    record_health_check_id: Optional[str] = field(default=None)
+    record_traffic_policy_instance_id: Optional[str] = field(default=None)
+    record_cidr_routing_config: Optional[AwsRoute53CidrRoutingConfig] = field(default=None)
+
+    def _keys(self) -> tuple[str, str, str, str, str, str, str, str, str, Optional[str]]:
+        if self._graph is None:
+            raise RuntimeError(f"_keys() called on {self.rtdname} before resource was added to graph")
+        return (
+            self.kind,
+            self.cloud().id,
+            self.account().id,
+            self.region().id,
+            self.zone().id,
+            self.dns_zone().id,
+            self.id,
+            self.safe_name,
+            self.record_type,
+            self.record_set_identifier,
         )
-        return True
 
     @classmethod
-    def called_mutator_apis(cls) -> List[AwsApiSpec]:
-        return super().called_mutator_apis() + [
-            AwsApiSpec(
-                service_name, "delete-load-balancer", override_iam_permission="elasticloadbalancing:DeleteLoadBalancer"
-            ),
-        ]
+    def service_name(cls) -> str:
+        return service_name
 
 
-resources: List[Type[AwsResource]] = [AwsElb]
+resources: List[Type[AwsResource]] = [AwsRoute53Zone, AwsRoute53ResourceRecord, AwsRoute53ResourceRecordSet]
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/elbv2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import ClassVar, Dict, Optional, Type, List
 
 from attrs import define, field
 
 from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, parse_json
 from resoto_plugin_aws.resource.ec2 import AwsEc2Vpc, AwsEc2Subnet, AwsEc2Instance, AwsEc2SecurityGroup
-from resoto_plugin_aws.utils import ToDict
+from resoto_plugin_aws.resource.cloudwatch import AwsCloudwatchQuery, AwsCloudwatchMetricData, update_resource_metrics
+from resoto_plugin_aws.utils import ToDict, MetricNormalization
 from resotolib.baseresources import BaseLoadBalancer, ModelReference
 from resotolib.graph import Graph
 from resotolib.json_bender import Bender, S, Bend, bend, ForallBend, K
 from resotolib.types import Json
 from resoto_plugin_aws.aws_client import AwsClient
 
 service_name = "elbv2"
@@ -330,14 +331,87 @@
                     service_name, "describe-listeners", "Listeners", LoadBalancerArn=lb.arn
                 ):
                     mapped = bend(AwsAlbListener.mapping, listener)
                     if listener := parse_json(mapped, AwsAlbListener, builder):
                         lb.alb_listener.append(listener)
                 builder.add_node(lb, js)
 
+    @classmethod
+    def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        albs = {alb.id: alb for alb in builder.nodes(clazz=AwsAlb) if alb.region().id == builder.region.id}
+        queries = []
+        delta = builder.metrics_delta
+        start = builder.metrics_start
+        now = builder.created_at
+        for alb_id, alb in albs.items():
+            lb_id = "/".join((alb.arn or "").split("/")[-3:])
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric,
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=alb_id,
+                        stat="Sum",
+                        unit="Count",
+                        LoadBalancer=lb_id,
+                    )
+                    for metric in [
+                        "RequestCount",
+                        "ActiveConnectionCount",
+                        "HTTPCode_Target_2XX_Count",
+                        "HTTPCode_Target_4XX_Count",
+                        "HTTPCode_Target_5XX_Count",
+                    ]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name="TargetResponseTime",
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=alb_id,
+                        stat=stat,
+                        unit="Seconds",
+                        LoadBalancer=lb_id,
+                    )
+                    for stat in ["Minimum", "Average", "Maximum"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name="ProcessedBytes",
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=alb_id,
+                        stat="Sum",
+                        unit="Bytes",
+                        LoadBalancer=lb_id,
+                    )
+                ]
+            )
+
+        metric_normalizers = {
+            "RequestCount": MetricNormalization(name="request_count"),
+            "ActiveConnectionCount": MetricNormalization(name="active_connection_count"),
+            "HTTPCode_Target_2XX_Count": MetricNormalization(name="status_code_2xx_count"),
+            "HTTPCode_Target_4XX_Count": MetricNormalization(name="status_code_4xx_count"),
+            "HTTPCode_Target_5XX_Count": MetricNormalization(name="status_code_5xx_count"),
+            "TargetResponseTime": MetricNormalization(
+                name="latency_seconds", normalize_value=lambda x: round(x, ndigits=3)
+            ),
+            "ProcessedBytes": MetricNormalization(name="processed_bytes"),
+        }
+
+        cloudwatch_result = AwsCloudwatchMetricData.query_for(builder.client, queries, start, now)
+
+        update_resource_metrics(albs, cloudwatch_result, metric_normalizers)
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if vpc_id := source.get("VpcId"):
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Vpc, id=vpc_id)
         for sg in self.alb_security_groups:
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2SecurityGroup, id=sg)
         for sn in self.alb_availability_zones:
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Subnet, id=sn.subnet_id)
@@ -434,14 +508,15 @@
         "alb_healthy_threshold_count": S("HealthyThresholdCount"),
         "alb_unhealthy_threshold_count": S("UnhealthyThresholdCount"),
         "alb_health_check_path": S("HealthCheckPath"),
         "alb_matcher": S("Matcher") >> Bend(AwsAlbMatcher.mapping),
         "target_type": S("TargetType"),
         "alb_protocol_version": S("ProtocolVersion"),
         "alb_ip_address_type": S("IpAddressType"),
+        "alb_lb_arns": S("LoadBalancerArns"),
     }
     target_type: Optional[str] = field(default=None)
     protocol: Optional[str] = field(default=None)
     port: Optional[int] = field(default=None)
     alb_health_check_protocol: Optional[str] = field(default=None)
     alb_health_check_port: Optional[str] = field(default=None)
     alb_health_check_enabled: Optional[bool] = field(default=None)
@@ -450,14 +525,15 @@
     alb_healthy_threshold_count: Optional[int] = field(default=None)
     alb_unhealthy_threshold_count: Optional[int] = field(default=None)
     alb_health_check_path: Optional[str] = field(default=None)
     alb_matcher: Optional[AwsAlbMatcher] = field(default=None)
     alb_protocol_version: Optional[str] = field(default=None)
     alb_ip_address_type: Optional[str] = field(default=None)
     alb_target_health: List[AwsAlbTargetHealthDescription] = field(factory=list)
+    alb_lb_arns: List[str] = field(factory=list)
 
     @classmethod
     def called_collect_apis(cls) -> List[AwsApiSpec]:
         return [
             cls.api_spec,
             AwsApiSpec(
                 service_name,
@@ -478,14 +554,106 @@
                     service_name, "describe-target-health", "TargetHealthDescriptions", TargetGroupArn=tg.arn
                 ):
                     mapped = bend(AwsAlbTargetHealthDescription.mapping, health)
                     if tgh := parse_json(mapped, AwsAlbTargetHealthDescription, builder):
                         tg.alb_target_health.append(tgh)
                 builder.add_node(tg, js)
 
+    @classmethod
+    def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        target_groups = {
+            tg.id: tg
+            for tg in builder.nodes(clazz=AwsAlbTargetGroup)
+            if tg.region().id == builder.region.id and tg.alb_lb_arns
+        }
+        queries = []
+        delta = builder.metrics_delta
+        start = builder.metrics_start
+        now = builder.created_at
+        for tg_id, tg in target_groups.items():
+            tg_arn_id = (tg.arn or "").split(":")[-1]
+            lb_arn_id = "/".join(tg.alb_lb_arns[0].split("/")[-3:])
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric,
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=tg_id,
+                        stat="Sum",
+                        unit="Count",
+                        LoadBalancer=lb_arn_id,
+                        TargetGroup=tg_arn_id,
+                    )
+                    for metric in [
+                        "RequestCount",
+                        "HealthyHostCount",
+                        "UnHealthyHostCount",
+                        "HTTPCode_Target_2XX_Count",
+                        "HTTPCode_Target_4XX_Count",
+                        "HTTPCode_Target_5XX_Count",
+                    ]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name="TargetResponseTime",
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=tg_id,
+                        stat=stat,
+                        unit="Seconds",
+                        LoadBalancer=lb_arn_id,
+                        TargetGroup=tg_arn_id,
+                    )
+                    for stat in ["Minimum", "Average", "Maximum"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric,
+                        namespace="AWS/ApplicationELB",
+                        period=delta,
+                        ref_id=tg_id,
+                        stat="Sum",
+                        unit="Bytes",
+                        LoadBalancer=lb_arn_id,
+                        TargetGroup=tg_arn_id,
+                    )
+                    for metric in [
+                        "HealthyStateRouting",
+                        "UnhealthyStateRouting",
+                        "HealthyStateDNS",
+                        "UnhealthyStateDNS",
+                    ]
+                ]
+            )
+
+        metric_normalizers = {
+            "RequestCount": MetricNormalization(name="request_count"),
+            "HealthyHostCount": MetricNormalization(name="healthy_host_count"),
+            "UnHealthyHostCount": MetricNormalization(name="unhealthy_host_count"),
+            "HTTPCode_Target_2XX_Count": MetricNormalization(name="status_code_2xx_count"),
+            "HTTPCode_Target_4XX_Count": MetricNormalization(name="status_code_4xx_count"),
+            "HTTPCode_Target_5XX_Count": MetricNormalization(name="status_code_5xx_count"),
+            "TargetResponseTime": MetricNormalization(
+                name="latency_seconds", normalize_value=lambda x: round(x, ndigits=3)
+            ),
+            "HealthyStateRouting": MetricNormalization(name="healthy_state_routing"),
+            "UnhealthyStateRouting": MetricNormalization(name="unhealthy_state_routing"),
+            "HealthyStateDNS": MetricNormalization(name="healthy_state_dns"),
+            "UnhealthyStateDNS": MetricNormalization(name="unhealthy_state_dns"),
+        }
+
+        cloudwatch_result = AwsCloudwatchMetricData.query_for(builder.client, queries, start, now)
+
+        update_resource_metrics(target_groups, cloudwatch_result, metric_normalizers)
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if vpc_id := source.get("VpcId"):
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Vpc, id=vpc_id)
         for lb_arn in bend(S("LoadBalancerArns", default=[]), source):
             if lb := builder.node(AwsAlb, arn=lb_arn):
                 builder.dependant_node(lb, node=self)
                 for th in self.alb_target_health:
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/service_quotas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,250 +1,224 @@
-from typing import ClassVar, Dict, Optional, List, Type
+import logging
+import re
+from typing import ClassVar, Dict, Optional, Type, Any, List, Pattern, Union
+
+from attr import field, evolve
+from attrs import define
+
+from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, AwsRegion
+from resotolib.baseresources import BaseQuota, EdgeType, ModelReference
+from resotolib.json_bender import Bender, S, Bend
+from resotolib.types import Json
+from resoto_plugin_aws.aws_client import AwsClient
 
-from attrs import define, field
+log = logging.getLogger("resoto.plugins.aws")
+service_name = "service-quotas"
 
-from resoto_plugin_aws.aws_client import AwsClient
-from resoto_plugin_aws.resource.base import AwsResource, AwsApiSpec, GraphBuilder
-from resoto_plugin_aws.utils import ToDict
-from resotolib.baseresources import (
-    BaseDNSZone,
-    BaseDNSRecord,
-    EdgeType,
-    BaseDNSRecordSet,
-    ModelReference,
-)
-from resotolib.graph import Graph
-from resotolib.json_bender import F, Bender, S, Bend, ForallBend, bend
-from resotolib.types import Json
-from resotolib.utils import rrdata_as_dict
 
-service_name = "route53"
+@define(eq=False, slots=False)
+class AwsQuotaMetricInfo:
+    kind: ClassVar[str] = "aws_quota_metric_info"
+    mapping: ClassVar[Dict[str, Bender]] = {
+        "metric_namespace": S("MetricNamespace"),
+        "metric_name": S("MetricName"),
+        "metric_dimensions": S("MetricDimensions"),
+        "metric_statistic_recommendation": S("MetricStatisticRecommendation"),
+    }
+    metric_namespace: Optional[str] = field(default=None)
+    metric_name: Optional[str] = field(default=None)
+    metric_dimensions: Optional[Dict[str, str]] = field(default=None)
+    metric_statistic_recommendation: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsRoute53ZoneConfig:
-    kind: ClassVar[str] = "aws_route53_zone_config"
-    mapping: ClassVar[Dict[str, Bender]] = {"comment": S("Comment"), "private_zone": S("PrivateZone")}
-    comment: Optional[str] = field(default=None)
-    private_zone: Optional[bool] = field(default=None)
+class AwsQuotaPeriod:
+    kind: ClassVar[str] = "aws_quota_period"
+    mapping: ClassVar[Dict[str, Bender]] = {"period_value": S("PeriodValue"), "period_unit": S("PeriodUnit")}
+    period_value: Optional[int] = field(default=None)
+    period_unit: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsRoute53LinkedService:
-    kind: ClassVar[str] = "aws_route53_linked_service"
-    mapping: ClassVar[Dict[str, Bender]] = {"service_principal": S("ServicePrincipal"), "description": S("Description")}
-    service_principal: Optional[str] = field(default=None)
-    description: Optional[str] = field(default=None)
+class AwsQuotaErrorReason:
+    kind: ClassVar[str] = "aws_quota_error_reason"
+    mapping: ClassVar[Dict[str, Bender]] = {"error_code": S("ErrorCode"), "error_message": S("ErrorMessage")}
+    error_code: Optional[str] = field(default=None)
+    error_message: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class AwsRoute53Zone(AwsResource, BaseDNSZone):
-    kind: ClassVar[str] = "aws_route53_zone"
-    api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "list-hosted-zones", "HostedZones")
+class AwsServiceQuota(AwsResource, BaseQuota):
+    kind: ClassVar[str] = "aws_service_quota"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
-            "default": ["aws_route53_resource_record_set"],
-            "delete": [],
+            "default": [
+                "aws_ec2_instance_type",
+                "aws_ec2_volume_type",
+                "aws_vpc",
+                "aws_elb",
+                "aws_alb",
+                "aws_iam_server_certificate",
+            ]
         }
     }
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("Id") >> F(lambda x: x.rsplit("/", 1)[-1]),  # remove leading "/hostedzones/"
-        "name": S("Name"),
-        "zone_caller_reference": S("CallerReference"),
-        "zone_config": S("Config") >> Bend(AwsRoute53ZoneConfig.mapping),
-        "zone_resource_record_set_count": S("ResourceRecordSetCount"),
-        "zone_linked_service": S("LinkedService") >> Bend(AwsRoute53LinkedService.mapping),
-    }
-    zone_caller_reference: Optional[str] = field(default=None)
-    zone_config: Optional[AwsRoute53ZoneConfig] = field(default=None)
-    zone_resource_record_set_count: Optional[int] = field(default=None)
-    zone_linked_service: Optional[AwsRoute53LinkedService] = field(default=None)
+        "id": S("QuotaCode"),
+        "name": S("QuotaName"),
+        "service_code": S("ServiceCode"),
+        "service_name": S("ServiceName"),
+        "arn": S("QuotaArn"),
+        "quota": S("Value"),
+        "quota_unit": S("Unit"),
+        "quota_adjustable": S("Adjustable"),
+        "quota_global": S("GlobalQuota"),
+        "quota_usage_metric": S("UsageMetric") >> Bend(AwsQuotaMetricInfo.mapping),
+        "quota_period": S("Period") >> Bend(AwsQuotaPeriod.mapping),
+        "quota_error_reason": S("ErrorReason") >> Bend(AwsQuotaErrorReason.mapping),
+    }
+    quota_unit: Optional[str] = field(default=None)
+    quota_adjustable: Optional[bool] = field(default=None)
+    quota_global: Optional[bool] = field(default=None)
+    quota_usage_metric: Optional[AwsQuotaMetricInfo] = field(default=None)
+    quota_period: Optional[AwsQuotaPeriod] = field(default=None)
+    quota_error_reason: Optional[AwsQuotaErrorReason] = field(default=None)
 
     @classmethod
     def called_collect_apis(cls) -> List[AwsApiSpec]:
         return [
-            cls.api_spec,
-            AwsApiSpec(service_name, "list-resource-record-sets"),
-            AwsApiSpec(service_name, "list-tags-for-resource"),
+            AwsApiSpec(service_name, "list-service-quotas", override_iam_permission="servicequotas:ListServiceQuotas")
         ]
 
     @classmethod
-    def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
-        def add_tags(zone: AwsRoute53Zone) -> None:
-            tags = builder.client.get(
-                service_name,
-                "list-tags-for-resource",
-                result_name="ResourceTagSet",
-                ResourceType="hostedzone",
-                ResourceId=zone.id,
-            )
-            if tags:
-                zone.tags = bend(S("Tags", default=[]) >> ToDict(), tags)
-
-        for js in json:
-            if zone := AwsRoute53Zone.from_api(js, builder):
-                builder.add_node(zone, js)
-                builder.submit_work(service_name, add_tags, zone)
-                for rs_js in builder.client.list(
-                    service_name, "list-resource-record-sets", "ResourceRecordSets", HostedZoneId=zone.id
+    def collect_service(cls, service_code: str, matchers: List["QuotaMatcher"], builder: GraphBuilder) -> None:
+        log.debug(f"Collecting Service quotas for {service_code} in region {builder.region.name}")
+        for js in builder.client.list(service_name, "list-service-quotas", "Quotas", ServiceCode=service_code):
+            if quota := AwsServiceQuota.from_api(js, builder):
+                for matcher in matchers:
+                    if matcher.match(quota):
+                        builder.add_node(quota, dict(source=js, matcher=evolve(matcher, region=builder.region)))
+
+    @classmethod
+    def collect_resources(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        # This collect run will be called for the global region as well as any configured region.
+        # We select the quotas to select based on the given region.
+        quotas = GlobalQuotas if builder.region.name == "global" else RegionalQuotas
+        for service, ms in quotas.items():
+            AwsServiceQuota.collect_service(service, ms, builder)
+
+    def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
+        super().connect_in_graph(builder, source)
+        matcher: Optional[QuotaMatcher] = source.get("matcher", None)
+
+        def prop_matches(attr: Any, expect: Any) -> bool:
+            if isinstance(expect, Pattern):
+                return expect.match(attr) is not None
+            else:
+                return bool(attr == expect)
+
+        if matcher:
+            for node in builder.graph.nodes:
+                if (
+                    node.kind == matcher.node_kind
+                    and (matcher.region is None or node.region().id == matcher.region.id)
+                    and all(prop_matches(getattr(node, k, None), v) for k, v in matcher.node_selector.items())
                 ):
-                    if record_set := AwsRoute53ResourceRecordSet.from_api(rs_js, builder):
-                        builder.add_node(record_set, rs_js)
-                        builder.add_edge(zone, EdgeType.default, node=record_set)
-                        for data in record_set.record_values:
-                            record = AwsRoute53ResourceRecord(
-                                id=record_set.id,
-                                name=record_set.name,
-                                record_type=record_set.record_type,
-                                record_ttl=record_set.record_ttl or 0,
-                                record_data=data,
-                                **rrdata_as_dict(record_set.record_type, data),
-                            )
-                            builder.add_node(record, js)
-                            builder.add_edge(record_set, EdgeType.default, node=record)
-                            builder.add_edge(record_set, EdgeType.delete, node=record)
+                    builder.add_edge(self, EdgeType.default, node=node)
 
     def update_resource_tag(self, client: AwsClient, key: str, value: str) -> bool:
         client.call(
             aws_service=service_name,
-            action="change-tags-for-resource",
+            action="tag-resource",
             result_name=None,
-            ResourceType="hostedzone",
-            ResourceId=self.id,
-            AddTags=[{"Key": key, "Value": value}],
+            ResourceARN=self.arn,
+            Tags=[{"Key": key, "Value": value}],
         )
         return True
 
     def delete_resource_tag(self, client: AwsClient, key: str) -> bool:
         client.call(
             aws_service=service_name,
-            action="change-tags-for-resource",
+            action="untag-resource",
             result_name=None,
-            ResourceType="hostedzone",
-            ResourceId=self.id,
-            RemoveTagKeys=[key],
-        )
-        return True
-
-    def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
-        client.call(
-            aws_service=service_name, action="delete-hosted-zone", result_name=None, Id=self.id.rsplit("/", 1)[-1]
+            ResourceARN=self.arn,
+            TagKeys=[key],
         )
         return True
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [
-            AwsApiSpec(service_name, "change-tags-for-resource"),
-            AwsApiSpec(service_name, "delete-hosted-zone"),
+            AwsApiSpec(service_name, "tag-resource", override_iam_permission="servicequotas:TagResource"),
+            AwsApiSpec(service_name, "untag-resource", override_iam_permission="servicequotas:UntagResource"),
         ]
 
-
-@define(eq=False, slots=False)
-class AwsRoute53GeoLocation:
-    kind: ClassVar[str] = "aws_route53_geo_location"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "continent_code": S("ContinentCode"),
-        "country_code": S("CountryCode"),
-        "subdivision_code": S("SubdivisionCode"),
-    }
-    continent_code: Optional[str] = field(default=None)
-    country_code: Optional[str] = field(default=None)
-    subdivision_code: Optional[str] = field(default=None)
-
-
-@define(eq=False, slots=False)
-class AwsRoute53AliasTarget:
-    kind: ClassVar[str] = "aws_route53_alias_target"
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "hosted_zone_id": S("HostedZoneId"),
-        "dns_name": S("DNSName"),
-        "evaluate_target_health": S("EvaluateTargetHealth"),
-    }
-    hosted_zone_id: Optional[str] = field(default=None)
-    dns_name: Optional[str] = field(default=None)
-    evaluate_target_health: Optional[bool] = field(default=None)
-
-
-@define(eq=False, slots=False)
-class AwsRoute53CidrRoutingConfig:
-    kind: ClassVar[str] = "aws_route53_cidr_routing_config"
-    mapping: ClassVar[Dict[str, Bender]] = {"collection_id": S("CollectionId"), "location_name": S("LocationName")}
-    collection_id: Optional[str] = field(default=None)
-    location_name: Optional[str] = field(default=None)
-
-
-@define(eq=False, slots=False)
-class AwsRoute53ResourceRecord(AwsResource, BaseDNSRecord):
-    kind: ClassVar[str] = "aws_route53_resource_record"
-    reference_kinds: ClassVar[ModelReference] = {
-        "successors": {
-            "default": [],
-            "delete": [],
-        }
-    }
-
     @classmethod
     def service_name(cls) -> str:
         return service_name
 
 
-@define(eq=False, slots=False)
-class AwsRoute53ResourceRecordSet(AwsResource, BaseDNSRecordSet):
-    kind: ClassVar[str] = "aws_route53_resource_record_set"
-    reference_kinds: ClassVar[ModelReference] = {
-        "successors": {
-            "default": ["aws_route53_resource_record"],
-            "delete": ["aws_route53_resource_record"],
-        }
-    }
-    mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("Name"),
-        "name": S("Name"),
-        "record_set_identifier": S("SetIdentifier"),
-        "record_type": S("Type"),
-        "record_weight": S("Weight"),
-        "record_region": S("Region"),
-        "record_geo_location": S("GeoLocation") >> Bend(AwsRoute53GeoLocation.mapping),
-        "record_fail_over": S("Failover"),
-        "record_multi_value_answer": S("MultiValueAnswer"),
-        "record_ttl": S("TTL"),
-        "record_values": S("ResourceRecords", default=[]) >> ForallBend(S("Value")),
-        "record_alias_target": S("AliasTarget") >> Bend(AwsRoute53AliasTarget.mapping),
-        "record_health_check_id": S("HealthCheckId"),
-        "record_traffic_policy_instance_id": S("TrafficPolicyInstanceId"),
-        "record_cidr_routing_config": S("CidrRoutingConfig") >> Bend(AwsRoute53CidrRoutingConfig.mapping),
-    }
-    record_name: Optional[str] = field(default=None)
-    record_set_identifier: Optional[str] = field(default=None)
-    record_weight: Optional[int] = field(default=None)
-    record_region: Optional[str] = field(default=None)
-    record_geo_location: Optional[AwsRoute53GeoLocation] = field(default=None)
-    record_fail_over: Optional[str] = field(default=None)
-    record_multi_value_answer: Optional[bool] = field(default=None)
-    record_alias_target: Optional[AwsRoute53AliasTarget] = field(default=None)
-    record_health_check_id: Optional[str] = field(default=None)
-    record_traffic_policy_instance_id: Optional[str] = field(default=None)
-    record_cidr_routing_config: Optional[AwsRoute53CidrRoutingConfig] = field(default=None)
-
-    def _keys(self) -> tuple[str, str, str, str, str, str, str, str, str, Optional[str]]:
-        if self._graph is None:
-            raise RuntimeError(f"_keys() called on {self.rtdname} before resource was added to graph")
-        return (
-            self.kind,
-            self.cloud().id,
-            self.account().id,
-            self.region().id,
-            self.zone().id,
-            self.dns_zone().id,
-            self.id,
-            self.safe_name,
-            self.record_type,
-            self.record_set_identifier,
+@define
+class QuotaMatcher:
+    quota_name: Union[str, Pattern[str], None]
+    node_kind: str
+    node_selector: Dict[str, Any] = field(factory=dict)
+    region: Optional[AwsRegion] = None
+
+    def match(self, quota: AwsServiceQuota) -> bool:
+        if self.quota_name is None:
+            return False
+        elif isinstance(self.quota_name, Pattern):
+            return self.quota_name.match(quota.safe_name) is not None
+        else:
+            return self.quota_name == quota.safe_name
+
+
+RegionalQuotas = {
+    "ec2": [
+        # Example: "Running On-Demand F instances" --> match InstanceTypes that start with F
+        QuotaMatcher(
+            quota_name=f"Running On-Demand {name} instances",
+            node_kind="aws_ec2_instance_type",
+            node_selector=dict(instance_type=re.compile("^" + start + "\\d")),
         )
-
-    @classmethod
-    def service_name(cls) -> str:
-        return service_name
+        for name, start in {
+            "Standard (A, C, D, H, I, M, R, T, Z)": "[acdhimrtz]",  # matches e.g. m4.large, i3en.3xlarge
+            "F": "f",
+            "G and VT": "g",
+            "P": "p",
+            "Inf": "inf",
+            "X": "x",
+            "High Memory instances": "u",
+            "DL": "dl",
+        }.items()
+    ],
+    "ebs": [
+        QuotaMatcher(
+            quota_name=re.compile(name_pattern),
+            node_kind="aws_ec2_volume_type",
+            node_selector=dict(volume_type=volume_type),
+        )
+        for name_pattern, volume_type in {
+            "^Storage for.*gp2": "gp2",
+            "^Storage for.*gp3": "gp3",
+            "^Storage for.*standard": "standard",
+            "^Storage for.*io1": "io1",
+            "^Storage for.*io2": "io2",
+            "^Storage for.*sc1": "sc1",
+            "^Storage for.*st1": "st1",
+        }.items()
+    ],
+    "vpc": [QuotaMatcher(quota_name="Internet gateways per Region", node_kind="aws_vpc")],
+    "elasticloadbalancing": [
+        QuotaMatcher(quota_name="Application Load Balancers per Region", node_kind="aws_alb"),
+        QuotaMatcher(quota_name="Classic Load Balancers per Region", node_kind="aws_elb"),
+    ],
+}
+
+GlobalQuotas = {
+    "iam": [
+        QuotaMatcher(quota_name="Server certificates per account", node_kind="aws_iam_server_certificate"),
+    ],
+}
 
 
-resources: List[Type[AwsResource]] = [AwsRoute53Zone, AwsRoute53ResourceRecord, AwsRoute53ResourceRecordSet]
+resources: List[Type[AwsResource]] = [AwsServiceQuota]
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.4
+Version: 3.6.5
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.6.5/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/__init__.py` & `resoto-plugin-aws-3.6.5/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/aws_client_test.py` & `resoto-plugin-aws-3.6.5/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/collector_test.py` & `resoto-plugin-aws-3.6.5/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/configuration_test.py` & `resoto-plugin-aws-3.6.5/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/graphbuilder_test.py` & `resoto-plugin-aws-3.6.5/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/__init__.py` & `resoto-plugin-aws-3.6.5/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.6.5/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/athena_test.py` & `resoto-plugin-aws-3.6.5/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.6.5/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/base_test.py` & `resoto-plugin-aws-3.6.5/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.6.5/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.6.5/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.6.5/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.6.5/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/cognito_test.py` & `resoto-plugin-aws-3.6.5/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.6.5/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/ec2_test.py` & `resoto-plugin-aws-3.6.5/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/ecs_test.py` & `resoto-plugin-aws-3.6.5/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/eks_test.py` & `resoto-plugin-aws-3.6.5/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.6.5/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.6.5/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/elb_test.py` & `resoto-plugin-aws-3.6.5/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.6.5/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/glacier_test.py` & `resoto-plugin-aws-3.6.5/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/iam_test.py` & `resoto-plugin-aws-3.6.5/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.6.5/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/kms_test.py` & `resoto-plugin-aws-3.6.5/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/lambda_test.py` & `resoto-plugin-aws-3.6.5/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/pricing_test.py` & `resoto-plugin-aws-3.6.5/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/rds_test.py` & `resoto-plugin-aws-3.6.5/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/redshift_test.py` & `resoto-plugin-aws-3.6.5/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/route53_test.py` & `resoto-plugin-aws-3.6.5/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/s3_test.py` & `resoto-plugin-aws-3.6.5/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.6.5/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.6.5/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/sns_test.py` & `resoto-plugin-aws-3.6.5/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/resources/sqs_test.py` & `resoto-plugin-aws-3.6.5/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.4/test/test_utils.py` & `resoto-plugin-aws-3.6.5/test/test_utils.py`

 * *Files identical despite different names*

