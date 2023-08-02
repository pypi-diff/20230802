# Comparing `tmp/mosaicml-cli-0.5.2.tar.gz` & `tmp/mosaicml-cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.5.2.tar", last modified: Thu Jul 27 22:06:59 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.5.3.tar", last modified: Wed Aug  2 21:37:36 2023, max compression
```

## Comparing `mosaicml-cli-0.5.2.tar` & `mosaicml-cli-0.5.3.tar`

### file list

```diff
@@ -1,210 +1,213 @@
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.762686 mosaicml-cli-0.5.2/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-27 22:06:59.762567 mosaicml-cli-0.5.2/PKG-INFO
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7089 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/README.md
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.731190 mosaicml-cli-0.5.2/mcli/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2122 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.731972 mosaicml-cli-0.5.2/mcli/api/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.732274 mosaicml-cli-0.5.2/mcli/api/cluster/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      134 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/cluster/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5459 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.732480 mosaicml-cli-0.5.2/mcli/api/engine/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/engine/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    26027 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/engine/engine.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13444 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/exceptions.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.739746 mosaicml-cli-0.5.2/mcli/api/inference_deployments/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1521 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3297 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5045 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3992 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8413 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2294 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2746 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.740175 mosaicml-cli-0.5.2/mcli/api/mint/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/shell.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2676 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/mint/tty.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.740779 mosaicml-cli-0.5.2/mcli/api/model/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1114 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/model/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10405 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/model/cluster_details.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4583 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/api/model/inference_deployment.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    14890 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/api/model/run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743071 mosaicml-cli-0.5.2/mcli/api/runs/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1269 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3785 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_create_interactive_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3034 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_create_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4365 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8796 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    12239 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5367 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_start_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5559 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5916 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_update_run.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4091 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10414 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743361 mosaicml-cli-0.5.2/mcli/api/schema/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/schema/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      636 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.743900 mosaicml-cli-0.5.2/mcli/api/secrets/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      309 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2386 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2943 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3665 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2354 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/typing_future.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.744186 mosaicml-cli-0.5.2/mcli/api/users/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      139 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/users/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2715 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/users/api_get_users.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      920 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/api/utils.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.744435 mosaicml-cli-0.5.2/mcli/cli/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/__init__.py
--rwxr-xr-x   0 margaret.qian   (502) staff       (20)     6069 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/cli.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.745179 mosaicml-cli-0.5.2/mcli/cli/common/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/common/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2560 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.745509 mosaicml-cli-0.5.2/mcli/cli/m_connect/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6426 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.746083 mosaicml-cli-0.5.2/mcli/cli/m_create/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2385 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/m_create.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    16900 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.746744 mosaicml-cli-0.5.2/mcli/cli/m_delete/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6448 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/delete.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5838 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.747137 mosaicml-cli-0.5.2/mcli/cli/m_deploy/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4253 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.748046 mosaicml-cli-0.5.2/mcli/cli/m_describe/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8364 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_clusters.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3929 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13495 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2719 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.749449 mosaicml-cli-0.5.2/mcli/cli/m_get/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      467 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7069 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/clusters.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6459 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/display.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5807 2023-07-27 19:50:50.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4804 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/m_get.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     8967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/runs.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2189 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/secrets.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1580 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_get/users.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.749743 mosaicml-cli-0.5.2/mcli/cli/m_init/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_init/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3908 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.750076 mosaicml-cli-0.5.2/mcli/cli/m_interactive/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     9036 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.750948 mosaicml-cli-0.5.2/mcli/cli/m_kube/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5523 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1398 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2050 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6946 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751210 mosaicml-cli-0.5.2/mcli/cli/m_log/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_log/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    11756 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751553 mosaicml-cli-0.5.2/mcli/cli/m_ping/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1411 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.751860 mosaicml-cli-0.5.2/mcli/cli/m_predict/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1905 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.752181 mosaicml-cli-0.5.2/mcli/cli/m_root/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_root/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      536 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.752415 mosaicml-cli-0.5.2/mcli/cli/m_run/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_run/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    11501 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.753593 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2964 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1793 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1656 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/organization.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      745 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.753787 mosaicml-cli-0.5.2/mcli/cli/m_stop/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4062 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754018 mosaicml-cli-0.5.2/mcli/cli/m_update/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_update/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6568 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/cli/m_update/m_update.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754444 mosaicml-cli-0.5.2/mcli/cli/m_util/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      797 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/m_util.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     9035 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/cli/m_util/util.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.754629 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3544 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/cli/m_watchdog/m_watchdog.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    13108 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.755578 mosaicml-cli-0.5.2/mcli/models/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/gpu_type.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    12287 2023-07-26 00:26:41.000000 mosaicml-cli-0.5.2/mcli/models/inference_deployment_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      427 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_cluster.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      456 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_envvar.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6728 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/models/mcli_secret.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    17258 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.2/mcli/models/run_config.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.755850 mosaicml-cli-0.5.2/mcli/objects/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.756774 mosaicml-cli-0.5.2/mcli/objects/secrets/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1090 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.757927 mosaicml-cli-0.5.2/mcli/objects/secrets/create/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1646 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/base.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2244 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2408 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6377 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3858 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5342 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      783 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1017 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/env_var.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      556 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/gcp.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/mounted.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/oci.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      961 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/s3.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1718 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.758155 mosaicml-cli-0.5.2/mcli/proto/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/proto/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1477 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.758305 mosaicml-cli-0.5.2/mcli/sdk/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2006 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/sdk/__init__.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.761089 mosaicml-cli-0.5.2/mcli/utils/
--rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/__init__.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6318 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/utils/utils_cli.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4409 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.2/mcli/utils/utils_completers.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     7047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)      740 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_date.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10749 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_docker.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2225 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_epilog.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10774 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_interactive.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4527 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_logging.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     2160 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1087 2023-07-27 22:06:17.000000 mosaicml-cli-0.5.2/mcli/utils/utils_model.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6605 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_pypi.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3115 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_rich.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5358 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.2/mcli/utils/utils_run_status.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     4350 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_spinner.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)    10751 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_string_functions.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1677 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_types.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/mcli/utils/utils_yaml.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3876 2023-07-27 22:06:24.000000 mosaicml-cli-0.5.2/mcli/version.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.761745 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/
--rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 margaret.qian   (502) staff       (20)     5147 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)        1 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)       75 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)     1654 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)        5 2023-07-27 22:06:59.000000 mosaicml-cli-0.5.2/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 margaret.qian   (502) staff       (20)    31087 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/pyproject.toml
--rw-r--r--   0 margaret.qian   (502) staff       (20)       38 2023-07-27 22:06:59.762722 mosaicml-cli-0.5.2/setup.cfg
--rw-r--r--   0 margaret.qian   (502) staff       (20)     3056 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/setup.py
-drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-27 22:06:59.762310 mosaicml-cli-0.5.2/tests/
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6449 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_config.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)       62 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_simple.py
--rw-r--r--   0 margaret.qian   (502) staff       (20)     6116 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.2/tests/test_upgrade.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.884269 mosaicml-cli-0.5.3/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-02 21:37:36.884139 mosaicml-cli-0.5.3/PKG-INFO
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7089 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/README.md
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857267 mosaicml-cli-0.5.3/mcli/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2239 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857731 mosaicml-cli-0.5.3/mcli/api/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857956 mosaicml-cli-0.5.3/mcli/api/cluster/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      210 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5805 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.858155 mosaicml-cli-0.5.3/mcli/api/engine/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/engine/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    26027 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/engine/engine.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13444 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/exceptions.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.858428 mosaicml-cli-0.5.3/mcli/api/finetune/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      141 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/finetune/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6802 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/finetune/api_instruction_finetune.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.859364 mosaicml-cli-0.5.3/mcli/api/inference_deployments/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1521 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3297 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5045 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3992 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8516 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2294 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2746 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6499 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.859728 mosaicml-cli-0.5.3/mcli/api/mint/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/shell.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2676 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/tty.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.860151 mosaicml-cli-0.5.3/mcli/api/model/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1114 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/model/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10386 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5770 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    14890 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/model/run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.861323 mosaicml-cli-0.5.3/mcli/api/runs/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1269 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3785 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3034 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4365 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8796 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    11001 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5367 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5559 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5916 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4091 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10049 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.861534 mosaicml-cli-0.5.3/mcli/api/schema/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/schema/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      636 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862018 mosaicml-cli-0.5.3/mcli/api/secrets/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      309 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2386 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2943 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3665 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2354 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/typing_future.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862231 mosaicml-cli-0.5.3/mcli/api/users/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      139 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/users/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2715 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/users/api_get_users.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      920 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/utils.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862450 mosaicml-cli-0.5.3/mcli/cli/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/__init__.py
+-rwxr-xr-x   0 tyler.lee   (502) staff       (20)     6069 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/cli.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871104 mosaicml-cli-0.5.3/mcli/cli/common/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/common/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2560 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7464 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871362 mosaicml-cli-0.5.3/mcli/cli/m_connect/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6462 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871695 mosaicml-cli-0.5.3/mcli/cli/m_create/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2385 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    16900 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872036 mosaicml-cli-0.5.3/mcli/cli/m_delete/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6448 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5838 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872230 mosaicml-cli-0.5.3/mcli/cli/m_deploy/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4253 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872794 mosaicml-cli-0.5.3/mcli/cli/m_describe/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7869 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_clusters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3929 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13495 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2719 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.873735 mosaicml-cli-0.5.3/mcli/cli/m_get/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      467 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7069 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6459 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/display.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8135 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4804 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8967 2023-08-01 21:45:05.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2189 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1580 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.873968 mosaicml-cli-0.5.3/mcli/cli/m_init/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3908 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874177 mosaicml-cli-0.5.3/mcli/cli/m_interactive/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     9036 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874711 mosaicml-cli-0.5.3/mcli/cli/m_kube/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5523 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1398 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2050 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6946 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874939 mosaicml-cli-0.5.3/mcli/cli/m_log/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    11756 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875420 mosaicml-cli-0.5.3/mcli/cli/m_ping/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1411 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875626 mosaicml-cli-0.5.3/mcli/cli/m_predict/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1905 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875832 mosaicml-cli-0.5.3/mcli/cli/m_root/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      536 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.876041 mosaicml-cli-0.5.3/mcli/cli/m_run/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    11501 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.876790 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2964 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1793 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1656 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      745 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877027 mosaicml-cli-0.5.3/mcli/cli/m_stop/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4062 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877240 mosaicml-cli-0.5.3/mcli/cli/m_update/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6560 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877571 mosaicml-cli-0.5.3/mcli/cli/m_util/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1161 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     9495 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/util.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877792 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3544 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13108 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.878642 mosaicml-cli-0.5.3/mcli/models/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/gpu_type.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    12287 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      479 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      456 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6728 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/mcli_secret.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    17258 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/models/run_config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.878784 mosaicml-cli-0.5.3/mcli/objects/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.879657 mosaicml-cli-0.5.3/mcli/objects/secrets/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1090 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880644 mosaicml-cli-0.5.3/mcli/objects/secrets/create/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1646 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2244 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2408 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6377 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3858 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5342 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      783 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1017 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      556 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      967 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      961 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1718 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880871 mosaicml-cli-0.5.3/mcli/proto/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/proto/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1477 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880994 mosaicml-cli-0.5.3/mcli/sdk/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2006 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/sdk/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883053 mosaicml-cli-0.5.3/mcli/utils/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6318 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/utils/utils_cli.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4409 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/utils/utils_completers.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      740 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_date.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2225 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7140 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/utils/utils_finetune.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10774 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4527 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_logging.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2160 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1087 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/utils/utils_model.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6605 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3115 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_rich.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5358 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4350 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10751 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1677 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_types.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3876 2023-08-02 21:36:35.000000 mosaicml-cli-0.5.3/mcli/version.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883688 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5225 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        1 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       75 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1660 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        5 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    31087 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/pyproject.toml
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       38 2023-08-02 21:37:36.884306 mosaicml-cli-0.5.3/setup.cfg
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3062 2023-08-02 21:36:35.000000 mosaicml-cli-0.5.3/setup.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883977 mosaicml-cli-0.5.3/tests/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6449 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       62 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_simple.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6116 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.5.2/PKG-INFO` & `mosaicml-cli-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.2/README.md` & `mosaicml-cli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/__init__.py` & `mosaicml-cli-0.5.3/mcli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ MCLI Package """
 
-from mcli.api.cluster import get_clusters
+from mcli.api.cluster import ClusterDetails, get_clusters
 from mcli.api.exceptions import MAPIException
+from mcli.api.finetune import instruction_finetune
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
                                             delete_inference_deployment, delete_inference_deployments,
                                             get_inference_deployment, get_inference_deployment_logs,
                                             get_inference_deployments, ping, predict, update_inference_deployment,
                                             update_inference_deployments)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
@@ -22,14 +23,15 @@
     'create_run',
     'create_secret',
     'delete_inference_deployment',
     'delete_inference_deployments',
     'delete_run',
     'delete_runs',
     'delete_secrets',
+    'ClusterDetails',
     'FeatureFlag',
     'FinalRunConfig',
     'follow_run_logs',
     'get_clusters',
     'get_inference_deployment_logs',
     'get_inference_deployment',
     'get_inference_deployments',
@@ -48,14 +50,15 @@
     'RunConfig',
     'RunStatus',
     'set_api_key',
     'start_run',
     'start_runs',
     'stop_run',
     'stop_runs',
+    'instruction_finetune',
     'update_inference_deployment',
     'update_inference_deployments',
     'update_run_metadata',
     'update_run',
     'wait_for_run_status',
     'watch_run_status',
 ]
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.5.3/mcli/api/cluster/api_get_clusters.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from typing_extensions import Literal
 
 from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
 from mcli.api.model.cluster_details import ClusterDetails
 from mcli.config import MCLIConfig
 from mcli.models.mcli_cluster import Cluster
+from mcli.utils.utils_model import SubmissionType
 
 __all__ = ['get_clusters']
 
 QUERY_FUNCTION = 'getClusters'
 VARIABLE_DATA_NAME = 'getClustersData'
 QUERY = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
@@ -133,35 +134,38 @@
 @overload
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     *,
     include_utilization: bool = False,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
+    submission_type_filter: Optional[SubmissionType] = None,
 ) -> List[ClusterDetails]:
     ...
 
 
 @overload
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     *,
     include_utilization: bool = False,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
+    submission_type_filter: Optional[SubmissionType] = None,
 ) -> Future[List[ClusterDetails]]:
     ...
 
 
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     *,
     include_utilization: bool = False,
     timeout: Optional[float] = 10,
     future: bool = False,
+    submission_type_filter: Optional[SubmissionType] = None,
 ):
     """Get clusters available in the MosaicML platform
 
     Arguments:
         clusters (:class:`~mcli.models.mcli_cluster.Cluster`): List of
             :class:`~mcli.models.mcli_cluster.Cluster` objects or cluster name
             strings to get.
@@ -180,14 +184,17 @@
         ``MAPIException``: If connecting to MAPI, raised when a MAPI communication error occurs
     """
     filters = {}
     if clusters:
         cluster_names = [c.name if isinstance(c, Cluster) else c for c in clusters]
         filters['name'] = {'in': cluster_names}
 
+    if submission_type_filter:
+        filters['allowedSubmissionTypes'] = {'has': submission_type_filter.name}
+
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters
         },
     }
 
     cfg = MCLIConfig.load_config()
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/engine/engine.py` & `mosaicml-cli-0.5.3/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/exceptions.py` & `mosaicml-cli-0.5.3/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
     publicDNS
     createdByEmail
+    replicas{{
+        name
+        status
+        latestRestartCount
+        latestRestartTime
+    }}
   }}
 }}"""
 
 
 @overload
 def get_inference_deployment(
     deployment: Optional[Union[str, InferenceDeployment]] = None,
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/mint/shell.py` & `mosaicml-cli-0.5.3/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/mint/tty.py` & `mosaicml-cli-0.5.3/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/model/__init__.py` & `mosaicml-cli-0.5.3/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.5.3/mcli/api/model/cluster_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,18 +216,17 @@
 def get_provider_name(raw_provider: str):
     raw_provider = raw_provider.upper()
 
     overrides = {
         'COREWEAVE': 'CoreWeave',
         'MICROK8S': 'MicroK8s',
         'MOSAICML_COLO': 'MosaicML',
-        'MINIKUBE': 'Minikube',
     }
 
-    return overrides.get(raw_provider, raw_provider)
+    return overrides.get(raw_provider, raw_provider.capitalize())
 
 
 @dataclass
 @functools.total_ordering
 class ClusterDetails(SerializableDataclass, DeserializableModel):
     """Details of a cluster, including instances and utilization
     """
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.5.3/mcli/api/model/inference_deployment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 """GraphQL representaion of Deployment"""
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
 from mcli.models.inference_deployment_config import FinalInferenceDeploymentConfig, InferenceDeploymentConfig
 
 
 @dataclass
+class InferenceDeploymentReplica(DeserializableModel):
+    """A specific replica of an inference deployment
+    """
+
+    name: str
+    status: str
+    latest_restart_count: int
+    latest_restart_time: Optional[datetime] = None
+
+    @classmethod
+    def from_mapi_response(cls, response: Dict[str, Any]):
+        latest_restart_time = None if response['latestRestartTime'] is None else convert_datetime(
+            response['latestRestartTime'])
+        return cls(name=response["name"],
+                   status=response["status"],
+                   latest_restart_count=response["latestRestartCount"],
+                   latest_restart_time=latest_restart_time)
+
+
+@dataclass
 class InferenceDeployment(DeserializableModel):
     """A deployment that has been launched on the MosaicML Cloud
 
     Args:
         deployment_uid (`str`): Unique identifier for the deployment
         name (`str`): User-defined name of the deployment
         status (:class:`~mcli.utils.utils_deployment_status.DeploymentStatus`): Status of the deployment
@@ -32,14 +52,15 @@
     updated_at: datetime
     config: FinalInferenceDeploymentConfig
     created_by: str
     public_dns: str = ""
 
     deleted_at: Optional[datetime] = None
     submitted_config: Optional[InferenceDeploymentConfig] = None
+    replicas: List[InferenceDeploymentReplica] = field(default_factory=List)
 
     _required_properties: Tuple[str] = tuple(
         ['id', 'name', 'status', 'createdAt', 'updatedAt', 'inferenceDeploymentInput', 'publicDNS'])
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]):
         missing = set(cls._required_properties) - set(response)
@@ -53,24 +74,35 @@
         if response['deletedAt'] is not None:
             deleted_at = convert_datetime(response['deletedAt'])
 
         submit_config = None
         if response.get('originalInferenceDeploymentInput', {}):
             submit_config = InferenceDeploymentConfig.from_mapi_response(response['originalInferenceDeploymentInput'])
 
+        replicas = [] if 'replicas' not in response else [
+            InferenceDeploymentReplica.from_mapi_response(replica) for replica in response['replicas']
+        ]
+
         return cls(deployment_uid=response['id'],
                    name=response['name'],
                    created_at=convert_datetime(response['createdAt']),
                    updated_at=convert_datetime(response['updatedAt']),
                    deleted_at=deleted_at,
                    status=response['status'],
                    public_dns=response['publicDNS'],
                    created_by=response['createdByEmail'],
                    config=FinalInferenceDeploymentConfig.from_mapi_response(response['inferenceDeploymentInput']),
-                   submitted_config=submit_config)
+                   submitted_config=submit_config,
+                   replicas=replicas)
+
+    def get_ready_replicas(self):
+        if self.replicas is None:
+            return self.config.replicas
+        else:
+            return len([r.status for r in self.replicas if r.status == "RUNNING"])
 
     def refresh(self) -> "InferenceDeployment":
         """
         Refreshed the data on the deployment object
 
         Returns:
             Refreshed :class:`~mcli.api.model.inference_deployment.InferenceDeployment` object
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/model/run.py` & `mosaicml-cli-0.5.3/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/__init__.py` & `mosaicml-cli-0.5.3/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_create_interactive_run.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_create_interactive_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_get_runs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from concurrent.futures import Future
 from datetime import datetime
 from http import HTTPStatus
 from typing import List, Optional, Union, cast, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import (convert_plural_future_to_singleton, get_return_response, run_paginated_mapi_request,
-                                    run_plural_mapi_request)
+from mcli.api.engine.engine import convert_plural_future_to_singleton, get_return_response, run_paginated_mapi_request
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 from mcli.models.gpu_type import GPUType
 from mcli.models.mcli_cluster import Cluster
 from mcli.utils.utils_run_status import RunStatus
 
 __all__ = ['get_runs', 'get_run']
 
-QUERY_FUNCTION = 'getRuns'
-VARIABLE_DATA_NAME = 'getRunsData'
+QUERY_FUNCTION_PAGINATED = 'getRunsPaginated'
+VARIABLE_DATA_NAME_PAGINATED = 'getRunsPaginatedData'
 QUERY = f"""
-query GetRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
-  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
+  {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
+  runs {{
     id
     name
     status
     createdAt
     startedAt
     completedAt
     updatedAt
@@ -45,19 +45,21 @@
         nodes
         executionIndex
         startTime
         endTime
         status
     }}
   }}
+  }}
 }}"""
 
 QUERY_WITH_DETAILS = f"""
-query GetRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
-  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
+query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
+  {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
+  runs {{
     id
     name
     status
     createdAt
     startedAt
     completedAt
     updatedAt
@@ -92,47 +94,14 @@
         }}
         nodes {{
             rank
             name
         }}
     }}
   }}
-}}
-"""
-QUERY_FUNCTION_PAGINATED = 'getRunsPaginated'
-VARIABLE_DATA_NAME_PAGINATED = 'getRunsPaginatedData'
-QUERY_PAGINATED = f"""
-query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
-  {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
-  runs {{
-    id
-    name
-    status
-    createdAt
-    startedAt
-    completedAt
-    updatedAt
-    reason
-    createdByEmail
-    priority
-    maxRetries
-    preemptible
-    retryOnSystemFailure
-    resumptions {{
-        clusterName
-        cpus
-        gpuType
-        gpus
-        nodes
-        executionIndex
-        startTime
-        endTime
-        status
-    }}
-  }}
   }}
 }}"""
 
 
 @overload
 def get_run(
     run: Union[str, Run],
@@ -281,18 +250,14 @@
         include_details: If true, will fetch detailed information like run input for each run.
         limit: Maximum number of runs to return. If None, all runs will be returned.
         include_interactive: Whether the run is interactive or not. If None, all runs will be returned.
 
     Raises:
         MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
     """
-    # We could support run details in pagination, but it goes against the point of the paginated view:
-    # This is a view that is meant to be used for listing runs, not for fetching detailed information
-    if limit and include_details:
-        raise MAPIException(HTTPStatus.BAD_REQUEST, "Cannot use limit and include_details together")
 
     filters = {}
     if runs:
         filters['name'] = {'in': [r.name if isinstance(r, Run) else r for r in runs]}
     if before or after:
         date_filters = {}
         if before:
@@ -311,41 +276,31 @@
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
     if gpu_nums:
         filters['gpuNum'] = {'in': gpu_nums}
 
     if include_interactive is not None:
         filters['isInteractive'] = {'equals': include_interactive}
 
-    variable_name = VARIABLE_DATA_NAME if limit is None else VARIABLE_DATA_NAME_PAGINATED
     variables = {
-        variable_name: {
+        VARIABLE_DATA_NAME_PAGINATED: {
             'filters': filters,
             'includeDeleted': False,
+            'limit': limit,
         },
     }
 
     cfg = MCLIConfig.load_config()
-    cfg.update_entity(variables[variable_name])
+    cfg.update_entity(variables[VARIABLE_DATA_NAME_PAGINATED])
     if user_emails:
-        if variables[variable_name].get('entity'):
-            variables[variable_name]['entity']['emails'] = user_emails
+        if variables[VARIABLE_DATA_NAME_PAGINATED].get('entity'):
+            variables[VARIABLE_DATA_NAME_PAGINATED]['entity']['emails'] = user_emails
         else:
-            variables[variable_name]['entity'] = {'emails': user_emails}
+            variables[VARIABLE_DATA_NAME_PAGINATED]['entity'] = {'emails': user_emails}
 
-    if limit is None:
-        response = run_plural_mapi_request(
-            query=QUERY if not include_details else QUERY_WITH_DETAILS,
-            query_function=QUERY_FUNCTION,
-            return_model_type=Run,
-            variables=variables,
-        )
-    else:
-        # use paginated getRuns query
-        variables[variable_name]['limit'] = limit
-        response = run_paginated_mapi_request(
-            query=QUERY_PAGINATED,
-            query_function=QUERY_FUNCTION_PAGINATED,
-            return_model_type=Run,
-            variables=variables,
-        )
+    response = run_paginated_mapi_request(
+        query=QUERY if not include_details else QUERY_WITH_DETAILS,
+        query_function=QUERY_FUNCTION_PAGINATED,
+        return_model_type=Run,
+        variables=variables,
+    )
 
     return get_return_response(response, future=future, timeout=timeout)
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_update_run.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_update_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.5.3/mcli/api/runs/api_watch_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Adds run status watching for the MCloud API"""
 from __future__ import annotations
 
 import functools
 import logging
 from concurrent.futures import Future
-from http import HTTPStatus
 from typing import Any, Dict, Generator, Optional, Union, overload
 
 import gql
 from typing_extensions import Literal
 
 from mcli.api.engine.engine import MAPIConnection, get_return_response, run_in_threadpool
-from mcli.api.exceptions import MAPIException
 from mcli.api.model.run import Run
-from mcli.api.runs.api_get_runs import get_runs
+from mcli.api.runs.api_get_runs import get_run
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import progress
 
 logger = logging.getLogger(__name__)
 
 QUERY_FUNCTION = 'watchRunStatus'
 VARIABLE_DATA_NAME = 'watchRunStatusInput'
@@ -106,18 +104,15 @@
     response = run_in_threadpool(_threaded_wait_for_run_status, run=run, status=status)
     return get_return_response(response, future=future, timeout=timeout)
 
 
 def _threaded_wait_for_run_status(run: Union[Run, str], status: RunStatus):
     # Convert to Run
     if not isinstance(run, Run):
-        try:
-            run = get_runs([run])[0]
-        except IndexError as e:
-            raise MAPIException(status=HTTPStatus.NOT_FOUND, message=f"Could not find a run named {run}") from e
+        run = get_run(run, include_details=False)
 
     updated_run: Optional[Run] = None
     for updated_run in watch_run_status(run):
         if updated_run.status.after(status, inclusive=True):
             return updated_run
 
     if not updated_run:
@@ -179,18 +174,15 @@
         Otherwise:
             A :class:`~concurrent.futures.Future` for the run. This will not resolve until
             the run reaches a new status
     """
 
     # Convert to Run
     if not isinstance(run, Run):
-        try:
-            run = get_runs([run])[0]
-        except IndexError as e:
-            raise MAPIException(status=HTTPStatus.NOT_FOUND, message=f"Could not find a run named {run}") from e
+        run = get_run(run, include_details=False)
 
     variables: Dict[str, Any] = {'name': run.name}
 
     variables = {VARIABLE_DATA_NAME: variables}
     query = gql.gql(QUERY)
 
     connection = MAPIConnection.get_current_connection()
```

### Comparing `mosaicml-cli-0.5.2/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.5.3/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.5.3/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.5.3/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.5.3/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/typing_future.py` & `mosaicml-cli-0.5.3/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.5.3/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/api/utils.py` & `mosaicml-cli-0.5.3/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/cli.py` & `mosaicml-cli-0.5.3/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.5.3/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.5.3/mcli/cli/common/run_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
     if not name_filter:
         # Accept all that pass other filters
         name_filter = []
 
     # Use get_runs only for the non-glob names provided
     glob_filters, run_names = _split_glob_filters(name_filter)
 
+    # If we're getting the latest run, we only need to get one
+    if latest:
+        limit = 1
+
     with console_status('Retrieving requested runs...'):
         runs = get_runs(
             runs=(run_names or None) if not glob_filters else None,
             cluster_names=cluster_filter,
             user_emails=user_filter,
             before=before_filter,
             after=after_filter,
@@ -203,12 +207,8 @@
         expected_names = set(run_names)
         for run_name in found_runs:
             if run_name in expected_names:
                 filtered.add(run_name)
 
         runs = list(found_runs[r] for r in filtered)
 
-    if latest and runs:
-        latest_run = sorted(runs, key=lambda x: x.created_at, reverse=True)[0]
-        runs = [latest_run]
-
     return runs
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.5.3/mcli/cli/m_connect/m_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,45 +58,46 @@
     runs: Optional[List[Run]] = None,
     **kwargs,
 ):
     del kwargs
 
     if name:
         run = get_run(name)
+    elif latest:
+        runs = get_runs_to_connect_to(limit=1)
+        if not runs:
+            logger.error(f'{FAIL} No running runs available to connect to')
+            return 1
+        run = runs[0]
     else:
         # If a user doesn't specify a run name, get all starting and running runs
         # When runs are passed in, don't perform another query
         available_runs = runs or get_runs_to_connect_to()
         if not available_runs:
             logger.error(f'{FAIL} No running runs available to connect to')
             return 1
         elif len(available_runs) == 1:
             # Only one run, connect to this one automatically
             run = available_runs[0]
         else:
             # Multiple options for runs to connect to...
             sorted_runs = sorted(available_runs, key=lambda x: x.created_at, reverse=True)
 
-            if latest:
-                # User specified --latest
-                run = sorted_runs[0]
-            else:
-
-                def name_formatter(r: Run):
-                    if r.started_at:
-                        details = f'Started at {format_timestamp(r.started_at)}'
-                    else:
-                        details = 'Not yet started'
-                    return f'{r.name} ({details})'
-
-                run = choose_one(
-                    'Which run would you like to connect to?',
-                    options=available_runs,
-                    formatter=name_formatter,
-                )
+            def name_formatter(r: Run):
+                if r.started_at:
+                    details = f'Started at {format_timestamp(r.started_at)}'
+                else:
+                    details = 'Not yet started'
+                return f'{r.name} ({details})'
+
+            run = choose_one(
+                'Which run would you like to connect to?',
+                options=sorted_runs,
+                formatter=name_formatter,
+            )
 
     # Wait for the run to be ready
     ready = wait_for_run(run)
     if not ready:
         return 1
 
     # Get the command and connect to the shell
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.5.3/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.5.3/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.5.3/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.5.3/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.5.3/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_clusters.py` & `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_clusters.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,51 +108,40 @@
         total_nodes = sum(instance.nodes for instance in self.model)
         total_cpus = sum(instance.cpus for instance in self.model if instance.cpus is not None)
         print(f'Total Nodes: {total_nodes}')
         print(f'Total GPUs: {total_gpus}')
         print(f'Total CPUs: {total_cpus}')
 
         for instance in self.model:
-            if count % 4 == 0 and count != 0:
+            if count % 3 == 0 and count != 0:
                 all_columns.append(Columns(curr_columns))
                 curr_columns = [create_instance_panel(instance)]
             else:
                 curr_columns.append(create_instance_panel(instance))
             count += 1
         all_columns.append(Columns(curr_columns))
 
         for col in all_columns:
             rprint(col)
             print()
 
 
-def calculate_quantity_per_node(quantity: str, nodes: int) -> str:
-    unit = quantity.lstrip('0123456789')
-    value = int(quantity.rstrip(unit))
-    return f'{value/nodes}{unit}'
-
-
 def create_instance_panel(instance: Instance) -> Panel:
     """ Creates a panel for instance details """
     if len(instance.name) > 20:
         instance.name = instance.name[:17] + "..."
-    instance_details = f"[bold]Name: [/bold]{instance.name}\n[bold]GPU Type: [/bold]{instance.gpu_type}"
+    instance_details = f"[bold]Instance Name: [/bold]{instance.name}\n[bold]GPU Type: [/bold]{instance.gpu_type}"
     gpu_string = f"GPUs: {instance.gpus*instance.nodes}"
     nodes = instance.nodes
     node_string = f"Nodes: {nodes}"
-    storage_string = f"RAM: {instance.storage}"
-    memory_string = f"Memory: {instance.memory}"
     per_node = "\n\n\n"
-    if nodes > 0:
-        storage_per_node = calculate_quantity_per_node(instance.storage, nodes)
-        memory_per_node = calculate_quantity_per_node(instance.memory, nodes)
-        per_node = f"[bold]Per Node: [/bold]\nGPUs: {instance.gpus}\nRAM: {storage_per_node}\nMemory: {memory_per_node}"
-    return Panel(f"{instance_details}\n\n{node_string}\n{gpu_string}\n{storage_string}\n{memory_string}\n\n{per_node}",
-                 expand=True,
-                 width=30)
+    storage_per_node = f"Storage: {instance.storage}"
+    memory_per_node = f"RAM: {instance.memory}"
+    per_node = f"[bold]Per Node: [/bold]\nGPUs: {instance.gpus}\n{storage_per_node}\n{memory_per_node}"
+    return Panel(f"{instance_details}\n\n{node_string}\n{gpu_string}\n\n{per_node}", expand=True, width=40)
 
 
 @dataclass
 class NodeDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for display purposes.
     """
     name: str
@@ -216,15 +205,14 @@
     print(format_string('Cluster Details', FormatString.BOLD))
     cluster_details_display = MCLIDescribeClusterDetailsDisplay(cluster)
     cluster_details_display.print(output)
     print()
 
     # Instance details section
     instances = cluster[0].cluster_instances
-    print(format_string('Instance Details', FormatString.BOLD))
     instance_display = MCLIInstanceDisplay(instances)
     instance_display.print()
     print()
 
     # Node details section
     print(format_string('Node Details', FormatString.BOLD))
     display = MCLIInstanceNodeDisplay(instances)
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.5.3/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/display.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/inference_deployments.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,39 @@
 import argparse
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Generator, List, Optional
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
-from mcli.api.model.inference_deployment import InferenceDeployment
+from mcli.api.model.inference_deployment import InferenceDeployment, InferenceDeploymentReplica
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import configure_submission_filter_argparser
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
 from mcli.utils.utils_model import SubmissionType
 
 
 class InferenceDeploymentColumns(Enum):
     ID = 'id'
     NAME = 'name'
+    REPLICAS = 'replicas'
+    STATUS = 'status'
     USER = 'user'
     CLUSTER = 'cluster'
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
-    REPLICAS = 'replicas'
     CREATED_TIME = 'created_time'
-    STATUS = 'status'
+
+
+@dataclass
+class InferenceDeploymentReplicaItem(MCLIDisplayItem):
+    deployment_name: Optional[str]
+    replica: str
+    status: str
+    restart: str
 
 
 @dataclass
 class InferenceDeploymentDisplayItem(MCLIDisplayItem):
     """Tuple that extracts deployment data for display purposes.
     """
     name: str
@@ -42,23 +50,32 @@
     id: Optional[str] = None
 
     @classmethod
     def from_deployment(cls,
                         deployment: InferenceDeployment,
                         include_ids: bool = False) -> InferenceDeploymentDisplayItem:
         extracted: Dict[str, str] = {
-            InferenceDeploymentColumns.NAME.value: deployment.name,
-            InferenceDeploymentColumns.USER.value: deployment.created_by,
-            InferenceDeploymentColumns.GPU_NUM.value: str(deployment.config.gpu_num),
-            InferenceDeploymentColumns.CREATED_TIME.value: format_timestamp(deployment.created_at),
-            InferenceDeploymentColumns.STATUS.value: deployment.status,
-            InferenceDeploymentColumns.CLUSTER.value: deployment.config.cluster,
-            InferenceDeploymentColumns.GPU_TYPE.value: str(deployment.config.gpu_type),
-            InferenceDeploymentColumns.REPLICAS.value: str(deployment.config.replicas)
+            InferenceDeploymentColumns.NAME.value:
+                deployment.name,
+            InferenceDeploymentColumns.USER.value:
+                deployment.created_by,
+            InferenceDeploymentColumns.GPU_NUM.value:
+                str(deployment.config.gpu_num),
+            InferenceDeploymentColumns.CREATED_TIME.value:
+                format_timestamp(deployment.created_at),
+            InferenceDeploymentColumns.CLUSTER.value:
+                deployment.config.cluster,
+            InferenceDeploymentColumns.GPU_TYPE.value:
+                str(deployment.config.gpu_type),
+            InferenceDeploymentColumns.REPLICAS.value:
+                str(deployment.config.replicas),
+            InferenceDeploymentColumns.STATUS.value:
+                f'{deployment.get_ready_replicas()}/{deployment.config.replicas} Ready'
         }
+
         if include_ids:
             extracted[InferenceDeploymentColumns.ID.value] = deployment.deployment_uid
 
         return InferenceDeploymentDisplayItem(**extracted)
 
 
 class InferenceDeploymentDisplay(MCLIGetDisplay):
@@ -81,37 +98,74 @@
         return cols
 
     def __iter__(self) -> Generator[InferenceDeploymentDisplayItem, None, None]:
         for deployment in self.deployments:
             yield InferenceDeploymentDisplayItem.from_deployment(deployment, self.include_ids)
 
 
+class InferenceDeploymentReplicaDisplay(MCLIGetDisplay):
+    """Display information about a deployment replica
+    """
+
+    @property
+    def index_label(self) -> str:
+        return "deployment_name"
+
+    def __init__(self, deployments: List[InferenceDeployment]) -> None:
+        self.deployments = sorted(deployments, key=lambda x: x.created_at, reverse=True)
+
+    def format_restarts(self, replica: InferenceDeploymentReplica) -> str:
+        if replica.latest_restart_count > 0:
+            return (f'{replica.latest_restart_count} restarts, '
+                    f'Last restart at {format_timestamp(replica.latest_restart_time)}')
+        else:
+            return f'0 restarts, Started at {format_timestamp(replica.latest_restart_time)}'
+
+    def __iter__(self) -> Generator[MCLIDisplayItem, None, None]:
+        for deploy in self.deployments:
+            for i, replica in enumerate(deploy.replicas):
+                deploy_name = deploy.name
+                if i > 0:
+                    deploy_name = ''
+                yield InferenceDeploymentReplicaItem(deploy_name, replica.name[-5:], replica.status,
+                                                     self.format_restarts(replica))
+
+
 @cli_error_handler('mcli get deployments')
 def cli_get_deployments(
     name_filter: Optional[List[str]] = None,
     cluster_filter: Optional[List[str]] = None,
     before_filter: Optional[str] = None,
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[str]] = None,
     output: OutputDisplay = OutputDisplay.TABLE,
     include_ids: bool = False,
+    compact: bool = False,
     **kwargs,
 ) -> int:
     """Get a table of ongoing and completed inference deployments
     """
     del kwargs
 
     deployments = get_deployments_with_filters(name_filter, cluster_filter, before_filter, after_filter,
                                                gpu_type_filter, gpu_num_filter, status_filter)
 
+    if not compact and len(deployments) > 0:
+        print('Inference Deployments Overview')
     display = InferenceDeploymentDisplay(deployments, include_ids=include_ids)
     display.print(output)
 
+    deployments_with_replicas = [deploy for deploy in deployments if deploy.replicas]
+    if not compact and len(deployments_with_replicas) > 0:
+        print('\nReplica Details')
+        replicas_display = InferenceDeploymentReplicaDisplay(deployments_with_replicas)
+        replicas_display.print(OutputDisplay.TABLE)
+
     return 0
 
 
 def get_deployments_argparser(subparsers: argparse._SubParsersAction):
     """Configures the ``mcli get deployments`` argparser
     """
 
@@ -124,14 +178,20 @@
     deployments_parser = subparsers.add_parser(
         'deployments',
         aliases=['deployment'],
         help='Get information on all of your existing deployments across all clusters.',
         epilog=deployment_examples,
         formatter_class=argparse.RawDescriptionHelpFormatter)
 
+    deployments_parser.add_argument('--compact',
+                                    action='store_true',
+                                    dest='compact',
+                                    default=False,
+                                    help='Hide detailed replica statuses and only show individual deployments')
+
     deployments_parser.add_argument(
         '--name',
         dest='name_filter',
         nargs='*',
         metavar='DEPLOYMENT',
         default=None,
         help='String or glob of the name(s) of the deployments to get',
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_get/users.py` & `mosaicml-cli-0.5.3/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.5.3/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.5.3/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.5.3/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.5.3/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.5.3/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.5.3/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.5.3/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.5.3/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/organization.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/organization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.5.3/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_update/m_update.py` & `mosaicml-cli-0.5.3/mcli/cli/m_update/m_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 > mcli update run example-run --priority high --max-retries 4 --no-preemptible
 """
 
 UPDATE_DEPLOYMENT_EXAMPLE = """
 Example:
 
 # Update a deployment
-> mcli update deployment mpt30b-deployment --image ../path/to/mpt30b.yaml --replicas 4
+> mcli update deployment mpt30b-deployment --image new_image_name --replicas 4
 """
 
 
 def update_entrypoint(parser, **kwargs) -> int:
     del kwargs
     parser.print_help()
     return 0
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_util/util.py` & `mosaicml-cli-0.5.3/mcli/cli/m_util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,27 +202,43 @@
                 row_args["style"] = Style(color=color)
             data_table.add_row(item['name'], *data_row, **row_args)
 
         return data_table
 
 
 @cli_error_handler('mcli util')
-def get_util(clusters: Optional[List[str]] = None, hide_users: bool = False, **kwargs) -> int:
+def get_util(clusters: Optional[List[str]] = None,
+             hide_users: bool = False,
+             training: bool = False,
+             inference: bool = False,
+             **kwargs) -> int:
+
+    submission_type_filter = None
+    if training:
+        submission_type_filter = SubmissionType.TRAINING
+    elif inference:
+        submission_type_filter = SubmissionType.INFERENCE
+
     del kwargs
     try:
-        c = get_clusters(clusters=clusters, include_utilization=True)
+        c = get_clusters(clusters=clusters, include_utilization=True, submission_type_filter=submission_type_filter)
     except MAPIException as e:
         if e.status == HTTPStatus.NOT_FOUND:
             e.message = MAPIErrorMessages.NOT_FOUND_CLUSTER.value
         raise e
 
     if len(c) == 0:
         raise MAPIException(HTTPStatus.NOT_FOUND, f'No clusters found with name(s): {clusters}')
-    # for submission_type in SubmissionType:
-    for i, submission_type in enumerate(SubmissionType):
+
+    if submission_type_filter is None:
+        submission_types_list = SubmissionType
+    else:
+        submission_types_list = [submission_type_filter]
+
+    for i, submission_type in enumerate(submission_types_list):
         submission_cluster = [cluster for cluster in c if submission_type in cluster.submission_types]
         if len(submission_cluster) == 0:
             continue
         agg = ''
         if len({cluster.name for cluster in submission_cluster}) > 1:
             agg = ' by Cluster'
 
@@ -239,10 +255,10 @@
 
             print(f'\nQueued {submission_type.value}s{agg}:')
             queued_display = SubmissionUtilizationDisplay(submission_cluster,
                                                           submission_type=submission_type,
                                                           is_active=False)
             queued_display.print(OutputDisplay.TABLE)
 
-        if i < len(SubmissionType) - 1:
+        if i < len(submission_types_list) - 1:
             print("\n")
     return 0
```

### Comparing `mosaicml-cli-0.5.2/mcli/cli/m_watchdog/m_watchdog.py` & `mosaicml-cli-0.5.3/mcli/cli/m_watchdog/m_watchdog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/config.py` & `mosaicml-cli-0.5.3/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/models/__init__.py` & `mosaicml-cli-0.5.3/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/models/gpu_type.py` & `mosaicml-cli-0.5.3/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.5.3/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/models/mcli_secret.py` & `mosaicml-cli-0.5.3/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/models/run_config.py` & `mosaicml-cli-0.5.3/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.5.3/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.5.3/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/sdk/__init__.py` & `mosaicml-cli-0.5.3/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_cli.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_completers.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_completers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_config.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_date.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_logging.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_model.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_rich.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_types.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.5.3/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/mcli/version.py` & `mosaicml-cli-0.5.3/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 mcli/api/exceptions.py
 mcli/api/typing_future.py
 mcli/api/utils.py
 mcli/api/cluster/__init__.py
 mcli/api/cluster/api_get_clusters.py
 mcli/api/engine/__init__.py
 mcli/api/engine/engine.py
+mcli/api/finetune/__init__.py
+mcli/api/finetune/api_instruction_finetune.py
 mcli/api/inference_deployments/__init__.py
 mcli/api/inference_deployments/api_create_inference_deployment.py
 mcli/api/inference_deployments/api_delete_inference_deployments.py
 mcli/api/inference_deployments/api_get_inference_deployment_logs.py
 mcli/api/inference_deployments/api_get_inference_deployments.py
 mcli/api/inference_deployments/api_ping.py
 mcli/api/inference_deployments/api_predict_inference_deployment.py
@@ -137,16 +139,16 @@
 mcli/proto/mint_pb2.py
 mcli/sdk/__init__.py
 mcli/utils/__init__.py
 mcli/utils/utils_cli.py
 mcli/utils/utils_completers.py
 mcli/utils/utils_config.py
 mcli/utils/utils_date.py
-mcli/utils/utils_docker.py
 mcli/utils/utils_epilog.py
+mcli/utils/utils_finetune.py
 mcli/utils/utils_interactive.py
 mcli/utils/utils_logging.py
 mcli/utils/utils_message_decoding.py
 mcli/utils/utils_model.py
 mcli/utils/utils_pypi.py
 mcli/utils/utils_rich.py
 mcli/utils/utils_run_status.py
```

### Comparing `mosaicml-cli-0.5.2/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 argcomplete>=2.0.0
 arrow>=1.2.2
 backoff>=2.2.1
-docker>=5.0.3
 gql[websockets]>=3.4.0
 prompt_toolkit>=3.0.29
 protobuf>=3.20.0
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=12.6.0
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
+requests<3,>=2.26.0
 
 [all]
-sphinxext-opengraph==0.8.2
-sphinxcontrib-jsmath>=1.0.1
-pytest-mock>=3.7.0
-sphinxcontrib-serializinghtml==1.1.5
-sphinx-design
-docutils>=0.17.0
 sphinx-copybutton==0.5.2
+pytest-cov>=4.0.0
+pytest>=6.2.5
+radon>=5.1.0
+yapf>=0.33.0
+furo==2022.9.29
+sphinx-rtd-theme==1.0.0
+sphinx-argparse==0.4.0
+sphinxcontrib-qthelp>=1.0.3
 sphinx-markdown-tables==0.0.17
-isort>=5.9.3
-sphinx_external_toc==0.3.0
-sphinxcontrib-applehelp>=1.0.2
+sphinxext-opengraph==0.8.2
+build>=0.10.0
+sphinxcontrib-devhelp>=1.0.2
 sphinxcontrib-htmlhelp>=2.0.0
-pre-commit>=2.17.0
-sphinxcontrib-katex==0.9.4
-toml>=0.10.2
-pyright==1.1.256
 sphinxemoji==0.2.0
-twine>=4.0.2
-sphinx-rtd-theme==1.0.0
-radon>=5.1.0
-pytest>=6.2.5
+docutils>=0.17.0
+sphinx_external_toc==0.3.0
+sphinxcontrib-katex==0.9.4
+myst-parser>=0.16.1
 sphinxcontrib-images>=0.9.4
+pyright==1.1.256
+isort>=5.9.3
+pytest-mock>=3.7.0
 sphinx==4.4.0
-pytest-cov>=4.0.0
-myst-parser>=0.16.1
-sphinx-panels==0.6.0
-build>=0.10.0
+sphinx-design
+twine>=4.0.2
+sphinxcontrib-jsmath>=1.0.1
+sphinxcontrib-applehelp>=1.0.2
+toml>=0.10.2
+sphinxcontrib-serializinghtml==1.1.5
+pre-commit>=2.17.0
 pylint>=2.12.2
-sphinxcontrib-qthelp>=1.0.3
-yapf>=0.33.0
-sphinxcontrib-devhelp>=1.0.2
-furo==2022.9.29
-sphinx-argparse==0.4.0
+sphinx-panels==0.6.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.5.2/pyproject.toml` & `mosaicml-cli-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/setup.py` & `mosaicml-cli-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # pylint: disable-next=exec-used,consider-using-with
 exec(open('mcli/version.py', 'r', encoding='utf-8').read())
 
 install_requires = [
     'argcomplete>=2.0.0',
     'arrow>=1.2.2',
     'backoff>=2.2.1',
-    'docker>=5.0.3',
     'gql[websockets]>=3.4.0',
     'prompt_toolkit>=3.0.29',
     'protobuf>=3.20.0',
     'pyyaml>=5.4.1',
     'questionary>=1.10.0',
     'rich>=12.6.0',
     'ruamel.yaml>=0.17.21',
     'typing_extensions>=4.0.1',
     'validators>=0.20.0',
+    'requests>=2.26.0,<3',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'build>=0.10.0',
     'isort>=5.9.3',
```

### Comparing `mosaicml-cli-0.5.2/tests/test_config.py` & `mosaicml-cli-0.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.2/tests/test_upgrade.py` & `mosaicml-cli-0.5.3/tests/test_upgrade.py`

 * *Files identical despite different names*

