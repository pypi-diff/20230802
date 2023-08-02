# Comparing `tmp/formal-sdk-1.0.3.tar.gz` & `tmp/formal-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-1.0.3.tar", last modified: Wed Aug  2 14:34:59 2023, max compression
+gzip compressed data, was "formal-sdk-1.0.4.tar", last modified: Wed Aug  2 16:40:31 2023, max compression
```

## Comparing `formal-sdk-1.0.3.tar` & `formal-sdk-1.0.4.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.226861 formal-sdk-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 14:34:59.222861 formal-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:34:59.226861 formal-sdk-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.170858 formal-sdk-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.182859 formal-sdk-1.0.3/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/cord.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.170858 formal-sdk-1.0.3/src/formal_sdk/gen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.166858 formal-sdk-1.0.3/src/formal_sdk/gen/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.210860 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.170858 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.222861 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/column_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/key_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.170858 formal-sdk-1.0.3/src/formal_sdk/gen/validate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.222861 formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/validate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/validate_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/identities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_code_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_datahub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_external_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/integration_sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/native_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-02 14:34:42.000000 formal-sdk-1.0.3/src/formal_sdk/work_os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:59.182859 formal-sdk-1.0.3/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 14:34:59.000000 formal-sdk-1.0.3/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-08-02 14:34:59.000000 formal-sdk-1.0.3/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:34:59.000000 formal-sdk-1.0.3/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 14:34:59.000000 formal-sdk-1.0.3/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 14:34:59.000000 formal-sdk-1.0.3/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.871971 formal-sdk-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 16:40:31.871971 formal-sdk-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:40:31.871971 formal-sdk-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.835970 formal-sdk-1.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.847970 formal-sdk-1.0.4/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/cord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.835970 formal-sdk-1.0.4/src/formal_sdk/gen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.835970 formal-sdk-1.0.4/src/formal_sdk/gen/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.863971 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.835970 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.871971 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/column_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/key_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.835970 formal-sdk-1.0.4/src/formal_sdk/gen/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.871971 formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/validate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/validate_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/identities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_code_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_datahub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_external_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/integration_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/native_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-02 16:40:17.000000 formal-sdk-1.0.4/src/formal_sdk/work_os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:40:31.847970 formal-sdk-1.0.4/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 16:40:31.000000 formal-sdk-1.0.4/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-08-02 16:40:31.000000 formal-sdk-1.0.4/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:40:31.000000 formal-sdk-1.0.4/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 16:40:31.000000 formal-sdk-1.0.4/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 16:40:31.000000 formal-sdk-1.0.4/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-1.0.3/LICENSE` & `formal-sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/PKG-INFO` & `formal-sdk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-1.0.3/README.md` & `formal-sdk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/pyproject.toml` & `formal-sdk-1.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-sdk-1.0.3/src/example.py` & `formal-sdk-1.0.4/src/example.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/__init__.py` & `formal-sdk-1.0.4/src/formal_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/admin.py` & `formal-sdk-1.0.4/src/formal_sdk/admin.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/audit.py` & `formal-sdk-1.0.4/src/formal_sdk/audit.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/cord.py` & `formal-sdk-1.0.4/src/formal_sdk/cord.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/datastore.py` & `formal-sdk-1.0.4/src/formal_sdk/datastore.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/encryption.py` & `formal-sdk-1.0.4/src/formal_sdk/encryption.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from .types.v1 import search_pb2 as admin_dot_v1_dot_types_dot_v1_dot_search__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61\x64min/v1/search.proto\x12\x08\x61\x64min.v1\x1a\x1e\x61\x64min/v1/types/v1/search.proto\"|\n\rSearchRequest\x12\x1f\n\x0bobject_type\x18\x01 \x01(\tR\nobjectType\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\x12\x1b\n\tfilter_by\x18\x03 \x01(\tR\x08\x66ilterBy\x12\x17\n\x07sort_by\x18\x04 \x01(\tR\x06sortBy\"\x8c\x03\n\x0eSearchResponse\x12\x33\n\x05users\x18\x01 \x01(\x0b\x32\x1b.admin.v1.WrappedSearchUserH\x00R\x05users\x12\x36\n\x06groups\x18\x02 \x01(\x0b\x32\x1c.admin.v1.WrappedSearchGroupH\x00R\x06groups\x12;\n\x08policies\x18\x03 \x01(\x0b\x32\x1d.admin.v1.WrappedSearchPolicyH\x00R\x08policies\x12\x42\n\ndatastores\x18\x04 \x01(\x0b\x32 .admin.v1.WrappedSearchDatastoreH\x00R\ndatastores\x12<\n\x08sidecars\x18\x05 \x01(\x0b\x32\x1e.admin.v1.WrappedSearchSidecarH\x00R\x08sidecars\x12\x44\n\x0binventories\x18\x06 \x01(\x0b\x32 .admin.v1.WrappedSearchInventoryH\x00R\x0binventoriesB\x08\n\x06result\"F\n\x11WrappedSearchUser\x12\x31\n\x04user\x18\x01 \x03(\x0b\x32\x1d.admin.v1.types.v1.SearchUserR\x04user\"J\n\x12WrappedSearchGroup\x12\x34\n\x05group\x18\x01 \x03(\x0b\x32\x1e.admin.v1.types.v1.SearchGroupR\x05group\"N\n\x13WrappedSearchPolicy\x12\x37\n\x06policy\x18\x01 \x03(\x0b\x32\x1f.admin.v1.types.v1.SearchPolicyR\x06policy\"Z\n\x16WrappedSearchDatastore\x12@\n\tdatastore\x18\x01 \x03(\x0b\x32\".admin.v1.types.v1.SearchDatastoreR\tdatastore\"R\n\x14WrappedSearchSidecar\x12:\n\x07sidecar\x18\x01 \x03(\x0b\x32 .admin.v1.types.v1.SearchSidecarR\x07sidecar\"Z\n\x16WrappedSearchInventory\x12@\n\tinventory\x18\x01 \x03(\x0b\x32\".admin.v1.types.v1.SearchInventoryR\tinventory2N\n\rSearchService\x12=\n\x06Search\x12\x17.admin.v1.SearchRequest\x1a\x18.admin.v1.SearchResponse\"\x00\x42\xa6\x01\n\x0c\x63om.admin.v1B\x0bSearchProtoP\x01ZHgithub.com/formalco/control-plane/backend/admin-api/gen/admin/v1;adminv1\xa2\x02\x03\x41XX\xaa\x02\x08\x41\x64min.V1\xca\x02\x08\x41\x64min\\V1\xe2\x02\x14\x41\x64min\\V1\\GPBMetadata\xea\x02\tAdmin::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61\x64min/v1/search.proto\x12\x08\x61\x64min.v1\x1a\x1e\x61\x64min/v1/types/v1/search.proto\"\xa6\x01\n\rSearchRequest\x12\x1f\n\x0bobject_type\x18\x01 \x01(\tR\nobjectType\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\x12\x1b\n\tfilter_by\x18\x03 \x01(\tR\x08\x66ilterBy\x12\x17\n\x07sort_by\x18\x04 \x01(\tR\x06sortBy\x12\x12\n\x04page\x18\x05 \x01(\x05R\x04page\x12\x14\n\x05limit\x18\x06 \x01(\x05R\x05limit\"\x98\x04\n\x0eSearchResponse\x12\x33\n\x05users\x18\x01 \x01(\x0b\x32\x1b.admin.v1.WrappedSearchUserH\x00R\x05users\x12\x36\n\x06groups\x18\x02 \x01(\x0b\x32\x1c.admin.v1.WrappedSearchGroupH\x00R\x06groups\x12;\n\x08policies\x18\x03 \x01(\x0b\x32\x1d.admin.v1.WrappedSearchPolicyH\x00R\x08policies\x12\x42\n\ndatastores\x18\x04 \x01(\x0b\x32 .admin.v1.WrappedSearchDatastoreH\x00R\ndatastores\x12<\n\x08sidecars\x18\x05 \x01(\x0b\x32\x1e.admin.v1.WrappedSearchSidecarH\x00R\x08sidecars\x12\x44\n\x0binventories\x18\x06 \x01(\x0b\x32 .admin.v1.WrappedSearchInventoryH\x00R\x0binventories\x12\x14\n\x05\x66ound\x18\x07 \x01(\x05R\x05\x66ound\x12\x12\n\x04page\x18\x08 \x01(\x05R\x04page\x12\x15\n\x06out_of\x18\t \x01(\x05R\x05outOf\x12$\n\x0esearch_time_ms\x18\n \x01(\x05R\x0csearchTimeMs\x12#\n\rsearch_cutoff\x18\x0b \x01(\x08R\x0csearchCutoffB\x08\n\x06result\"F\n\x11WrappedSearchUser\x12\x31\n\x04user\x18\x01 \x03(\x0b\x32\x1d.admin.v1.types.v1.SearchUserR\x04user\"J\n\x12WrappedSearchGroup\x12\x34\n\x05group\x18\x01 \x03(\x0b\x32\x1e.admin.v1.types.v1.SearchGroupR\x05group\"N\n\x13WrappedSearchPolicy\x12\x37\n\x06policy\x18\x01 \x03(\x0b\x32\x1f.admin.v1.types.v1.SearchPolicyR\x06policy\"Z\n\x16WrappedSearchDatastore\x12@\n\tdatastore\x18\x01 \x03(\x0b\x32\".admin.v1.types.v1.SearchDatastoreR\tdatastore\"R\n\x14WrappedSearchSidecar\x12:\n\x07sidecar\x18\x01 \x03(\x0b\x32 .admin.v1.types.v1.SearchSidecarR\x07sidecar\"Z\n\x16WrappedSearchInventory\x12@\n\tinventory\x18\x01 \x03(\x0b\x32\".admin.v1.types.v1.SearchInventoryR\tinventory2N\n\rSearchService\x12=\n\x06Search\x12\x17.admin.v1.SearchRequest\x1a\x18.admin.v1.SearchResponse\"\x00\x42\xa6\x01\n\x0c\x63om.admin.v1B\x0bSearchProtoP\x01ZHgithub.com/formalco/control-plane/backend/admin-api/gen/admin/v1;adminv1\xa2\x02\x03\x41XX\xaa\x02\x08\x41\x64min.V1\xca\x02\x08\x41\x64min\\V1\xe2\x02\x14\x41\x64min\\V1\\GPBMetadata\xea\x02\tAdmin::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'admin.v1.search_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\014com.admin.v1B\013SearchProtoP\001ZHgithub.com/formalco/control-plane/backend/admin-api/gen/admin/v1;adminv1\242\002\003AXX\252\002\010Admin.V1\312\002\010Admin\\V1\342\002\024Admin\\V1\\GPBMetadata\352\002\tAdmin::V1'
-  _globals['_SEARCHREQUEST']._serialized_start=67
-  _globals['_SEARCHREQUEST']._serialized_end=191
-  _globals['_SEARCHRESPONSE']._serialized_start=194
-  _globals['_SEARCHRESPONSE']._serialized_end=590
-  _globals['_WRAPPEDSEARCHUSER']._serialized_start=592
-  _globals['_WRAPPEDSEARCHUSER']._serialized_end=662
-  _globals['_WRAPPEDSEARCHGROUP']._serialized_start=664
-  _globals['_WRAPPEDSEARCHGROUP']._serialized_end=738
-  _globals['_WRAPPEDSEARCHPOLICY']._serialized_start=740
-  _globals['_WRAPPEDSEARCHPOLICY']._serialized_end=818
-  _globals['_WRAPPEDSEARCHDATASTORE']._serialized_start=820
-  _globals['_WRAPPEDSEARCHDATASTORE']._serialized_end=910
-  _globals['_WRAPPEDSEARCHSIDECAR']._serialized_start=912
-  _globals['_WRAPPEDSEARCHSIDECAR']._serialized_end=994
-  _globals['_WRAPPEDSEARCHINVENTORY']._serialized_start=996
-  _globals['_WRAPPEDSEARCHINVENTORY']._serialized_end=1086
-  _globals['_SEARCHSERVICE']._serialized_start=1088
-  _globals['_SEARCHSERVICE']._serialized_end=1166
+  _globals['_SEARCHREQUEST']._serialized_start=68
+  _globals['_SEARCHREQUEST']._serialized_end=234
+  _globals['_SEARCHRESPONSE']._serialized_start=237
+  _globals['_SEARCHRESPONSE']._serialized_end=773
+  _globals['_WRAPPEDSEARCHUSER']._serialized_start=775
+  _globals['_WRAPPEDSEARCHUSER']._serialized_end=845
+  _globals['_WRAPPEDSEARCHGROUP']._serialized_start=847
+  _globals['_WRAPPEDSEARCHGROUP']._serialized_end=921
+  _globals['_WRAPPEDSEARCHPOLICY']._serialized_start=923
+  _globals['_WRAPPEDSEARCHPOLICY']._serialized_end=1001
+  _globals['_WRAPPEDSEARCHDATASTORE']._serialized_start=1003
+  _globals['_WRAPPEDSEARCHDATASTORE']._serialized_end=1093
+  _globals['_WRAPPEDSEARCHSIDECAR']._serialized_start=1095
+  _globals['_WRAPPEDSEARCHSIDECAR']._serialized_end=1177
+  _globals['_WRAPPEDSEARCHINVENTORY']._serialized_start=1179
+  _globals['_WRAPPEDSEARCHINVENTORY']._serialized_end=1269
+  _globals['_SEARCHSERVICE']._serialized_start=1271
+  _globals['_SEARCHSERVICE']._serialized_end=1349
 # @@protoc_insertion_point(module_scope)
```

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -3,40 +3,54 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SearchRequest(_message.Message):
-    __slots__ = ["object_type", "query", "filter_by", "sort_by"]
+    __slots__ = ["object_type", "query", "filter_by", "sort_by", "page", "limit"]
     OBJECT_TYPE_FIELD_NUMBER: _ClassVar[int]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     FILTER_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    PAGE_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
     object_type: str
     query: str
     filter_by: str
     sort_by: str
-    def __init__(self, object_type: _Optional[str] = ..., query: _Optional[str] = ..., filter_by: _Optional[str] = ..., sort_by: _Optional[str] = ...) -> None: ...
+    page: int
+    limit: int
+    def __init__(self, object_type: _Optional[str] = ..., query: _Optional[str] = ..., filter_by: _Optional[str] = ..., sort_by: _Optional[str] = ..., page: _Optional[int] = ..., limit: _Optional[int] = ...) -> None: ...
 
 class SearchResponse(_message.Message):
-    __slots__ = ["users", "groups", "policies", "datastores", "sidecars", "inventories"]
+    __slots__ = ["users", "groups", "policies", "datastores", "sidecars", "inventories", "found", "page", "out_of", "search_time_ms", "search_cutoff"]
     USERS_FIELD_NUMBER: _ClassVar[int]
     GROUPS_FIELD_NUMBER: _ClassVar[int]
     POLICIES_FIELD_NUMBER: _ClassVar[int]
     DATASTORES_FIELD_NUMBER: _ClassVar[int]
     SIDECARS_FIELD_NUMBER: _ClassVar[int]
     INVENTORIES_FIELD_NUMBER: _ClassVar[int]
+    FOUND_FIELD_NUMBER: _ClassVar[int]
+    PAGE_FIELD_NUMBER: _ClassVar[int]
+    OUT_OF_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_TIME_MS_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_CUTOFF_FIELD_NUMBER: _ClassVar[int]
     users: WrappedSearchUser
     groups: WrappedSearchGroup
     policies: WrappedSearchPolicy
     datastores: WrappedSearchDatastore
     sidecars: WrappedSearchSidecar
     inventories: WrappedSearchInventory
-    def __init__(self, users: _Optional[_Union[WrappedSearchUser, _Mapping]] = ..., groups: _Optional[_Union[WrappedSearchGroup, _Mapping]] = ..., policies: _Optional[_Union[WrappedSearchPolicy, _Mapping]] = ..., datastores: _Optional[_Union[WrappedSearchDatastore, _Mapping]] = ..., sidecars: _Optional[_Union[WrappedSearchSidecar, _Mapping]] = ..., inventories: _Optional[_Union[WrappedSearchInventory, _Mapping]] = ...) -> None: ...
+    found: int
+    page: int
+    out_of: int
+    search_time_ms: int
+    search_cutoff: bool
+    def __init__(self, users: _Optional[_Union[WrappedSearchUser, _Mapping]] = ..., groups: _Optional[_Union[WrappedSearchGroup, _Mapping]] = ..., policies: _Optional[_Union[WrappedSearchPolicy, _Mapping]] = ..., datastores: _Optional[_Union[WrappedSearchDatastore, _Mapping]] = ..., sidecars: _Optional[_Union[WrappedSearchSidecar, _Mapping]] = ..., inventories: _Optional[_Union[WrappedSearchInventory, _Mapping]] = ..., found: _Optional[int] = ..., page: _Optional[int] = ..., out_of: _Optional[int] = ..., search_time_ms: _Optional[int] = ..., search_cutoff: bool = ...) -> None: ...
 
 class WrappedSearchUser(_message.Message):
     __slots__ = ["user"]
     USER_FIELD_NUMBER: _ClassVar[int]
     user: _containers.RepeatedCompositeFieldContainer[_search_pb2.SearchUser]
     def __init__(self, user: _Optional[_Iterable[_Union[_search_pb2.SearchUser, _Mapping]]] = ...) -> None: ...
```

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/validate_pb2.py` & `formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/gen/validate/v1/validate_pb2.pyi` & `formal-sdk-1.0.4/src/formal_sdk/gen/validate/v1/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/identities.py` & `formal-sdk-1.0.4/src/formal_sdk/identities.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_app.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_app.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_cloud.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_cloud.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_code_repository.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_code_repository.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_datahub.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_datahub.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_external_api.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_external_api.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_github.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_github.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_incident.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_incident.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_kms.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_kms.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_log.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_log.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_slack.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_slack.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/integration_sso.py` & `formal-sdk-1.0.4/src/formal_sdk/integration_sso.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/inventory.py` & `formal-sdk-1.0.4/src/formal_sdk/inventory.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/metrics.py` & `formal-sdk-1.0.4/src/formal_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/native_user.py` & `formal-sdk-1.0.4/src/formal_sdk/native_user.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/outputs.py` & `formal-sdk-1.0.4/src/formal_sdk/outputs.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/policies.py` & `formal-sdk-1.0.4/src/formal_sdk/policies.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/registry.py` & `formal-sdk-1.0.4/src/formal_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/satellite.py` & `formal-sdk-1.0.4/src/formal_sdk/satellite.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/search.py` & `formal-sdk-1.0.4/src/formal_sdk/search.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/sidecar.py` & `formal-sdk-1.0.4/src/formal_sdk/sidecar.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk/work_os.py` & `formal-sdk-1.0.4/src/formal_sdk/work_os.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.3/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-1.0.4/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-1.0.3/src/formal_sdk.egg-info/SOURCES.txt` & `formal-sdk-1.0.4/src/formal_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

