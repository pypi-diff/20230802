# Comparing `tmp/fiddler-client-2.0.0.dev8.tar.gz` & `tmp/fiddler-client-2.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev8.tar", last modified: Mon Jul 31 16:37:49 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev9.tar", last modified: Wed Aug  2 08:58:30 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev8.tar` & `fiddler-client-2.0.0.dev9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    16868 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.860216 fiddler-client-2.0.0.dev8/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)     1476 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/api/
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16916 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4187 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9813 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1313 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/compatibility_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16963 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    22076 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15332 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9792 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/generate_schema_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4722 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4496 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4118 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21054 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3198 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/api/project_mixin.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1822 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   112950 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2490 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/exceptions.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6439 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/libs/http_client.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/packtools/template_model.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.864215 fiddler-client-2.0.0.dev8/fiddler/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4493 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      343 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      487 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3045 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      879 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      501 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1104 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      121 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      388 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/schemas/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1535 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1124 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1000) docker    (1001)      642 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1000) docker    (1001)      679 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1000) docker    (1001)      313 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/schemas/xai_params.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4399 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4284 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/compatibility_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3613 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2561 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)      189 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5493 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/pandas_helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1818 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15839 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/semver_version.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/utils/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1933 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/fiddler/validators/dataset_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2927 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      144 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-07-31 16:37:49.000000 fiddler-client-2.0.0.dev8/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1250 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.868216 fiddler-client-2.0.0.dev8/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/tests/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1418 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1785 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3787 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_add_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)    36786 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)    10277 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)      906 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_check_version_decorator.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3028 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_custom_features.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6307 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_dataset_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7718 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_events_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2801 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15111 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_explainability_apis.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7611 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_file_upload.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3256 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_generate_schema.py
--rw-r--r--   0 runner    (1000) docker    (1001)      820 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4608 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_job.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7397 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6548 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_project.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2958 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13719 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_upload_dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      581 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/test_validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:49.872216 fiddler-client-2.0.0.dev8/tests/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1473 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8084 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1800 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/fiddler/utils/tests_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5346 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/test_object_inference.py
--rw-r--r--   0 runner    (1000) docker    (1001)      280 2023-07-31 16:37:44.000000 fiddler-client-2.0.0.dev8/tests/utils.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.159603 fiddler-client-2.0.0.dev9/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-08-02 08:58:30.159603 fiddler-client-2.0.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    16868 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.147603 fiddler-client-2.0.0.dev9/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)     1826 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16916 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4187 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9813 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1313 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/compatibility_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16963 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    22076 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15332 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9792 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/generate_schema_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4722 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4496 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4118 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21055 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3198 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/api/project_mixin.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1822 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   112950 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2490 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/exceptions.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6439 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/libs/http_client.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/packtools/template_model.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4493 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      343 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      487 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3045 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      879 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      501 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1104 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      121 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      388 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.151603 fiddler-client-2.0.0.dev9/fiddler/schemas/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1750 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1124 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      642 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      679 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      313 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/schemas/xai_params.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.155603 fiddler-client-2.0.0.dev9/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4399 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4284 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/compatibility_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3613 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2561 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      189 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5493 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/pandas_helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1818 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15839 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/semver_version.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/utils/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.155603 fiddler-client-2.0.0.dev9/fiddler/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1933 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/fiddler/validators/dataset_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.155603 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    20648 2023-08-02 08:58:30.000000 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2927 2023-08-02 08:58:30.000000 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-08-02 08:58:30.000000 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      144 2023-08-02 08:58:30.000000 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-08-02 08:58:30.000000 fiddler-client-2.0.0.dev9/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-08-02 08:58:30.159603 fiddler-client-2.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1250 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.155603 fiddler-client-2.0.0.dev9/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.159603 fiddler-client-2.0.0.dev9/tests/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1418 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1785 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3787 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_add_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    36786 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    10277 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      906 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_check_version_decorator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3028 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_custom_features.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6307 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_dataset_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7718 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_events_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2801 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15111 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_explainability_apis.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7611 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_file_upload.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3256 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_generate_schema.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      820 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4608 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7397 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6548 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2958 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13719 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_upload_dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      581 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/test_validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:30.159603 fiddler-client-2.0.0.dev9/tests/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1473 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/utils/test_general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8084 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/utils/test_pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1800 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/fiddler/utils/tests_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5346 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/test_object_inference.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      280 2023-08-02 08:58:25.000000 fiddler-client-2.0.0.dev9/tests/utils.py
```

### Comparing `fiddler-client-2.0.0.dev8/PKG-INFO` & `fiddler-client-2.0.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev8
+Version: 2.0.0.dev9
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-2.0.0.dev8/PUBLIC.md` & `fiddler-client-2.0.0.dev9/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/README.md` & `fiddler-client-2.0.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/__init__.py` & `fiddler-client-2.0.0.dev9/fiddler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 TODO: Add Licence.
 """
 
 from fiddler import utils
 from fiddler._version import __version__
 from fiddler.api import FiddlerApi, FiddlerClient
+from fiddler.api.explainability_mixin import (
+    DatasetDataSource,
+    RowDataSource,
+    SqlSliceQueryDataSource,
+)
 from fiddler.constants import CSV_EXTENSION
 from fiddler.core_objects import (
     ArtifactStatus,
     BaselineType,
     BatchPublishType,
     Column,
     DatasetInfo,
@@ -25,14 +30,24 @@
     ModelInfo,
     ModelInputType,
     ModelTask,
     WeightingParams,
     WindowSize,
 )
 from fiddler.packtools import gem
+from fiddler.schema.alert import (
+    AlertCondition,
+    AlertType,
+    BinSize,
+    ComparePeriod,
+    CompareTo,
+    Metric,
+    Priority,
+)
+from fiddler.schema.model_deployment import DeploymentParams
 from fiddler.schemas.custom_features import Multivariate, TextEmbedding, ImageEmbedding
 from fiddler.utils import logger, ColorLogger
 from fiddler.utils.validator import (
     PackageValidator,
     ValidationChainSettings,
     ValidationModule,
 )
@@ -48,14 +63,15 @@
     'Column',
     'Multivariate',
     'TextEmbedding',
     'ImageEmbedding',
     'ColorLogger',
     'DatasetInfo',
     'DataType',
+    'DeploymentParams',
     'FiddlerClient',
     'FiddlerApi',
     'FiddlerTimestamp',
     'FiddlerPublishSchema',
     'gem',
     'ModelInfo',
     'ModelInputType',
```

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/alert_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/alert_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/api.py` & `fiddler-client-2.0.0.dev9/fiddler/api/api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/baseline_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/compatibility_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/compatibility_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/dataset_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/events_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/events_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/explainability_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/generate_schema_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/generate_schema_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/helpers.py` & `fiddler-client-2.0.0.dev9/fiddler/api/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/job_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/job_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev9/fiddler/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/model_deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/model_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
                 model_name,
                 artifact_dir,
             )
             file_path = shutil.make_archive(
                 base_name=str(Path(tmp) / 'files'),
                 format='tar',
                 root_dir=str(artifact_dir),
-                base_dir='',
+                base_dir='.',
             )
 
             logger.info(
                 'Model[%s/%s] - Model artifact tar file created at %s',
                 project_name,
                 model_name,
                 file_path,
```

### Comparing `fiddler-client-2.0.0.dev8/fiddler/api/project_mixin.py` & `fiddler-client-2.0.0.dev9/fiddler/api/project_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev9/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/constants.py` & `fiddler-client-2.0.0.dev9/fiddler/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev9/fiddler/core_objects.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/exceptions.py` & `fiddler-client-2.0.0.dev9/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev9/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev9/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev9/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev9/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev9/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schema/alert.py` & `fiddler-client-2.0.0.dev9/fiddler/schema/alert.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schema/dataset.py` & `fiddler-client-2.0.0.dev9/fiddler/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schema/events.py` & `fiddler-client-2.0.0.dev9/fiddler/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schema/model_deployment.py` & `fiddler-client-2.0.0.dev9/fiddler/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schemas/custom_features.py` & `fiddler-client-2.0.0.dev9/fiddler/schemas/custom_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pydantic import BaseModel
 
 T = TypeVar('T', bound='CustomFeature')
 
 
 class CustomFeatureType(str, Enum):
     FROM_COLUMNS = 'FROM_COLUMNS'
+    FROM_VECTOR = 'FROM_VECTOR'
     FROM_TEXT_EMBEDDING = 'FROM_TEXT_EMBEDDING'
     FROM_IMAGE_EMBEDDING = 'FROM_IMAGE_EMBEDDING'
 
 
 class CustomFeature(BaseModel):
     name: str
     type: CustomFeatureType
@@ -22,28 +23,31 @@
         allow_mutation = False
 
     @classmethod
     def from_dict(cls: Type[T], deserialized_json: dict) -> T:
         feature_type = CustomFeatureType(deserialized_json['type'])
         if feature_type == CustomFeatureType.FROM_COLUMNS:
             return Multivariate.parse_obj(deserialized_json)
+        elif feature_type == CustomFeatureType.FROM_VECTOR:
+            return VectorFeature.parse_obj(deserialized_json)
         elif feature_type == CustomFeatureType.FROM_TEXT_EMBEDDING:
             return TextEmbedding.parse_obj(deserialized_json)
         elif feature_type == CustomFeatureType.FROM_IMAGE_EMBEDDING:
             return ImageEmbedding.parse_obj(deserialized_json)
         else:
             raise ValueError(f'Unsupported feature type: {feature_type}')
 
 
 class Multivariate(CustomFeature):
     columns: List[str]
     monitor_components: bool = False
 
 
 class VectorFeature(CustomFeature):
+    type: CustomFeatureType  = CustomFeatureType.FROM_VECTOR
     source_column: Optional[str] = None
     column: str
 
 
 class TextEmbedding(VectorFeature):
     type: CustomFeatureType = CustomFeatureType.FROM_TEXT_EMBEDDING
```

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schemas/model_schema.py` & `fiddler-client-2.0.0.dev9/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schemas/model_spec.py` & `fiddler-client-2.0.0.dev9/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/schemas/model_task_params.py` & `fiddler-client-2.0.0.dev9/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/compatibility_helpers.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/compatibility_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/decorators.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/helpers.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/pandas_helper.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/response_handler.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/semver_version.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/semver_version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/utils/validator.py` & `fiddler-client-2.0.0.dev9/fiddler/utils/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev9/fiddler/validators/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev9/fiddler_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev8
+Version: 2.0.0.dev9
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-2.0.0.dev8/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev9/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/setup.py` & `fiddler-client-2.0.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/base.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/helper.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_add_model.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_add_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_alert.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_alert.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_baseline.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_check_version_decorator.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_check_version_decorator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_custom_features.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_dataset_api.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_events_api.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_events_api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_exceptions.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_explainability_apis.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_explainability_apis.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_file_upload.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_generate_schema.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_generate_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_helpers.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_job.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_model.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_project.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_response_handler.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_upload_dataset.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/test_validations.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/test_validations.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_general_checks.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/utils/test_general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/utils/test_pandas.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/fiddler/utils/tests_utils.py` & `fiddler-client-2.0.0.dev9/tests/fiddler/utils/tests_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev8/tests/test_object_inference.py` & `fiddler-client-2.0.0.dev9/tests/test_object_inference.py`

 * *Files identical despite different names*

