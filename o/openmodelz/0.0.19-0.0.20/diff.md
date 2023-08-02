# Comparing `tmp/openmodelz-0.0.19.tar.gz` & `tmp/openmodelz-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodelz-0.0.19.tar", last modified: Tue Aug  1 11:44:45 2023, max compression
+gzip compressed data, was "openmodelz-0.0.20.tar", last modified: Wed Aug  2 08:02:45 2023, max compression
```

## Comparing `openmodelz-0.0.19.tar` & `openmodelz-0.0.20.tar`

### file list

```diff
@@ -1,247 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.031546 openmodelz-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-08-01 11:42:55.000000 openmodelz-0.0.19/.all-contributorsrc
--rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-08-01 11:42:55.000000 openmodelz-0.0.19/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-08-01 11:42:55.000000 openmodelz-0.0.19/.goreleaser.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-01 11:42:55.000000 openmodelz-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-01 11:42:55.000000 openmodelz-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-08-01 11:44:45.031546 openmodelz-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11071 2023-08-01 11:42:55.000000 openmodelz-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.007546 openmodelz-0.0.19/agent/
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     7231 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/agent/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.007546 openmodelz-0.0.19/agent/api/types/
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/build.go
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/const.go
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/error.go
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/event.go
--rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/inference_deployment.go
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/inference_deployment_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/inference_status.go
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/info.go
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/log.go
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/namespace.go
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/queue.go
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/requests.go
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/secret.go
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/api/types/server.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/client/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/build.go
--rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/client.go
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/const.go
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/errors.go
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/hijack.go
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_remove.go
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_scale.go
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/info.go
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/instance_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/instance_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/log.go
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/namespace_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/options.go
--rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/request.go
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/client/transport.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/agent/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/cmd/agent/
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/cmd/agent/main.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/errdefs/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/errdefs/defs.go
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/errdefs/doc.go
--rw-r--r--   0 runner    (1001) docker     (122)     5850 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/errdefs/helpers.go
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/errdefs/http_helpers.go
--rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/errdefs/is.go
--rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/go.mod
--rw-r--r--   0 runner    (1001) docker     (122)   114827 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/agent/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/app/
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/app/config.go
--rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/app/root.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/config/
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/config/config.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/consts/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/consts/consts.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    37721 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/docs/docs.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/event/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/event/event.go
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/event/fake.go
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/event/username.go
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/event/util.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.011546 openmodelz-0.0.19/agent/pkg/k8s/
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/convert_deployment.go
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/convert_inference.go
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/convert_job.go
--rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/convert_pod.go
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/generate_job.go
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/k8s/resolver.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/log/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/log/factory.go
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/log/k8s.go
--rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/log/loki.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     4042 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/metrics/exporter.go
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/metrics/metrics.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/prom/
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/prom/prometheus_query.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/query/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/query/db.go
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/query/deployment_events.sql.go
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/query/models.go
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/query/querier.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/runtime/
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/build.go
--rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_replicas.go
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/namespace.go
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/runtime.go
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/util_domain.go
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/runtime/util_resource.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.015546 openmodelz-0.0.19/agent/pkg/scaling/
--rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/scaling/function_scaler.go
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/scaling/ranges.go
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/scaling/retry.go
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/scaling/service_query.go
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/scaling/util.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.019546 openmodelz-0.0.19/agent/pkg/server/
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/error.go
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_build_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_build_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_build_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_build_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_healthz.go
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_instance_exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_scale.go
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_inference_update.go
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_info.go
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_namespace_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_namespace_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_server_label_create.go
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/handler_server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/middleware_callid.go
--rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_factory.go
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_handlerfunc.go
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_init_kubernetes.go
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_init_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_init_metrics.go
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_init_route.go
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/server_run.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/agent/pkg/server/validator/
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/server/validator/validator.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/agent/pkg/version/
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/pkg/version/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/agent/sql/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/agent/sql/query/
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/sql/query/deployment_events.sql
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/sql/schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-08-01 11:42:55.000000 openmodelz-0.0.19/agent/sqlc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/mdz/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     7866 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/mdz/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/mdz/cmd/mdz/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/cmd/mdz/main.go
--rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/go.mod
--rw-r--r--   0 runner    (1001) docker     (122)    26290 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/mdz/hack/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/mdz/hack/cli-doc-gen/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/hack/cli-doc-gen/main.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/mdz/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.003545 openmodelz-0.0.19/mdz/pkg/agentd/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.023546 openmodelz-0.0.19/mdz/pkg/agentd/runtime/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/create.go
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/delete.go
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/label.go
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/list.go
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/runtime/runtime.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.027546 openmodelz-0.0.19/mdz/pkg/agentd/server/
--rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/error.go
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_healthz.go
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_create.go
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_get.go
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_list.go
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_proxy.go
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/handler_info.go
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/middleware_callid.go
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/server_factory.go
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/server_handlerfunc.go
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/server_init_route.go
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/agentd/server/server_run.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.027546 openmodelz-0.0.19/mdz/pkg/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/delete.go
--rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/deploy.go
--rw-r--r--   0 runner    (1001) docker     (122)     5225 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/exec.go
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/exec_stream.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.027546 openmodelz-0.0.19/mdz/pkg/cmd/ioutils/
--rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/ioutils/reader.go
--rw-r--r--   0 runner    (1001) docker     (122)     3634 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/list_instance.go
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/localagent.go
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/logs.go
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/portforward.go
--rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/root.go
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/scale.go
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server.go
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server_join.go
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server_label.go
--rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server_list.go
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server_start.go
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/server_stop.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.027546 openmodelz-0.0.19/mdz/pkg/cmd/streams/
--rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/streams/in.go
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/streams/out.go
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/streams/stream.go
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/cmd/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.031546 openmodelz-0.0.19/mdz/pkg/server/
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/agentd_run.go
--rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/engine.go
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/gpu-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/gpu_install.go
--rw-r--r--   0 runner    (1001) docker     (122)    32313 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/k3s-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/k3s_install.go
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/k3s_join.go
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/k3s_killall.go
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/nginx-dep.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/nginx_install.go
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/openmodelz.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/server/openmodelz_install.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.031546 openmodelz-0.0.19/mdz/pkg/term/
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/term/interrupt.go
--rw-r--r--   0 runner    (1001) docker     (122)     4045 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/term/term.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.031546 openmodelz-0.0.19/mdz/pkg/version/
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-01 11:42:55.000000 openmodelz-0.0.19/mdz/pkg/version/version.go
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 11:44:45.031546 openmodelz-0.0.19/openmodelz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-08-01 11:44:44.000000 openmodelz-0.0.19/openmodelz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-08-01 11:44:44.000000 openmodelz-0.0.19/openmodelz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 11:44:44.000000 openmodelz-0.0.19/openmodelz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 11:44:44.000000 openmodelz-0.0.19/openmodelz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-01 11:44:44.000000 openmodelz-0.0.19/openmodelz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-08-01 11:42:55.000000 openmodelz-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 11:44:45.031546 openmodelz-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-08-01 11:42:55.000000 openmodelz-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.all-contributorsrc
+-rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-08-02 08:00:54.000000 openmodelz-0.0.20/.goreleaser.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-02 08:00:54.000000 openmodelz-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-02 08:00:54.000000 openmodelz-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-02 08:02:45.494389 openmodelz-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-08-02 08:00:54.000000 openmodelz-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/agent/
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     7231 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/api/types/
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/const.go
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/event.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_deployment.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_deployment_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/inference_status.go
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/info.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/log.go
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/namespace.go
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/queue.go
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/requests.go
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/secret.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/api/types/server.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/client.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/const.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/errors.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/hijack.go
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_remove.go
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/info.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/instance_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/instance_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/log.go
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/namespace_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/options.go
+-rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/request.go
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/client/transport.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/cmd/agent/
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/cmd/agent/main.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/errdefs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/defs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/doc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5850 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/helpers.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/http_helpers.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/errdefs/is.go
+-rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/go.mod
+-rw-r--r--   0 runner    (1001) docker     (122)   114827 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.466389 openmodelz-0.0.20/agent/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/app/
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/app/config.go
+-rw-r--r--   0 runner    (1001) docker     (122)    10033 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/app/root.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/config/config.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.474389 openmodelz-0.0.20/agent/pkg/consts/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/consts/consts.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    37721 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/docs/docs.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/event/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/event.go
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/fake.go
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/username.go
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/event/util.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/k8s/
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_deployment.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_inference.go
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_job.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/convert_pod.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/generate_job.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/k8s/resolver.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/log/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/k8s.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/log/loki.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     4042 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/metrics/exporter.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/metrics/metrics.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/prom/
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/prom/prometheus_query.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.478389 openmodelz-0.0.20/agent/pkg/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/db.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/deployment_events.sql.go
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/models.go
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/query/querier.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.482389 openmodelz-0.0.20/agent/pkg/runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/build.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_replicas.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/namespace.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/runtime.go
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/util_domain.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/runtime/util_resource.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.482389 openmodelz-0.0.20/agent/pkg/scaling/
+-rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/function_scaler.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/ranges.go
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/retry.go
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/service_query.go
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/scaling/util.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_build_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_healthz.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_instance_exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_inference_update.go
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_info.go
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_namespace_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_namespace_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_server_label_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/handler_server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/middleware_callid.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_handlerfunc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_kubernetes.go
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_metrics.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_init_route.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/server_run.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/server/validator/
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/server/validator/validator.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/pkg/version/
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/pkg/version/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/sql/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/agent/sql/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sql/query/deployment_events.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sql/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-08-02 08:00:54.000000 openmodelz-0.0.20/agent/sqlc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     7866 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/cmd/mdz/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/cmd/mdz/main.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/go.mod
+-rw-r--r--   0 runner    (1001) docker     (122)    26290 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/hack/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/hack/cli-doc-gen/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/hack/cli-doc-gen/main.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.470389 openmodelz-0.0.20/mdz/pkg/agentd/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/pkg/agentd/runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/create.go
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/label.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/runtime/runtime.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.486389 openmodelz-0.0.20/mdz/pkg/agentd/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/error.go
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_healthz.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_create.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_get.go
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_proxy.go
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/handler_info.go
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/middleware_callid.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_factory.go
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_handlerfunc.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_init_route.go
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/agentd/server/server_run.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/delete.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/deploy.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5225 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/exec.go
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/exec_stream.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/ioutils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/ioutils/reader.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3634 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/list_instance.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/localagent.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/logs.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/portforward.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/root.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/scale.go
+-rw-r--r--   0 runner    (1001) docker     (122)      898 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_join.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_label.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3306 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_list.go
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_start.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/server_stop.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/cmd/streams/
+-rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/in.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/out.go
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/streams/stream.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/cmd/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/server/
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/agentd_run.go
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/engine.go
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/gpu-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/gpu_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)    32313 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s-install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_join.go
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_killall.go
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/k3s_prepare.go
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/nginx-dep.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/nginx_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/openmodelz.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/openmodelz_install.go
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/server/registries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.490389 openmodelz-0.0.20/mdz/pkg/term/
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/term/interrupt.go
+-rw-r--r--   0 runner    (1001) docker     (122)     4045 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/term/term.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/mdz/pkg/version/
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-02 08:00:54.000000 openmodelz-0.0.20/mdz/pkg/version/version.go
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:02:45.494389 openmodelz-0.0.20/openmodelz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6143 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-02 08:02:45.000000 openmodelz-0.0.20/openmodelz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-08-02 08:00:54.000000 openmodelz-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 08:02:45.494389 openmodelz-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-08-02 08:00:54.000000 openmodelz-0.0.20/setup.py
```

### Comparing `openmodelz-0.0.19/.all-contributorsrc` & `openmodelz-0.0.20/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/.gitignore` & `openmodelz-0.0.20/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/.goreleaser.yaml` & `openmodelz-0.0.20/.goreleaser.yaml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/LICENSE` & `openmodelz-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/README.md` & `openmodelz-0.0.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,29 @@
 
 ## Documentation 📝
 
 You can find the documentation at [docs.open.modelz.ai](https://docs.open.modelz.ai).
 
 ## Quick Start 🚀
 
-Once you've installed the `mdz` you can start deploying models and experimenting with them.
+### Install `mdz`
 
-There are only two concepts in `mdz`:
+You can install OpenModelZ using the following command:
+
+```text
+pip install openmodelz
+```
+
+You could verify the installation by running the following command:
+
+```text
+mdz
+```
+
+Once you've installed the `mdz` you can start deploying models and experimenting with them. There are only two concepts in `mdz`:
 
 - **Deployment**: A deployment is a running inference service. You could configure the number of replicas, the port, and the image, and some other parameters.
 - **Server**: A server is a machine that could run the deployments. It could be a cloud VM, a PC, or even a Raspberry Pi. You could start from a single server and scale it up to a cluster of machines without any hassle.
 
 ### Bootstrap `mdz`
 
 It's super easy to bootstrap the `mdz` server. You just need to find a server (could be a cloud VM, a home lab, or even a single machine) and run the `mdz server start` command. The `mdz` server will be bootstrapped on the server and you could start deploying your models.
```

#### html2text {}

```diff
@@ -21,68 +21,71 @@
 technical details for you, and provide a simple and easy-to-use CLI to deploy
 your models to **any cloud (GCP, AWS, or others), your home lab, or even a
 single machine**. You could **start from a single machine and scale it up to a
 cluster of machines** without any hassle. OpenModelZ lies at the heart of our
 [ModelZ](https://modelz.ai), which is a serverless inference platform. It's
 used in production to deploy models for our customers. ## Documentation ð
 You can find the documentation at [docs.open.modelz.ai](https://
-docs.open.modelz.ai). ## Quick Start ð Once you've installed the `mdz` you
-can start deploying models and experimenting with them. There are only two
-concepts in `mdz`: - **Deployment**: A deployment is a running inference
-service. You could configure the number of replicas, the port, and the image,
-and some other parameters. - **Server**: A server is a machine that could run
-the deployments. It could be a cloud VM, a PC, or even a Raspberry Pi. You
-could start from a single server and scale it up to a cluster of machines
-without any hassle. ### Bootstrap `mdz` It's super easy to bootstrap the `mdz`
-server. You just need to find a server (could be a cloud VM, a home lab, or
-even a single machine) and run the `mdz server start` command. The `mdz` server
-will be bootstrapped on the server and you could start deploying your models.
-``` $ mdz server start ð§ Initializing the server... ð§ Waiting for the
-server to be ready... ð Checking if the server is running... Agent: Version:
-v0.0.5 Build Date: 2023-07-19T09:12:55Z Git Commit:
-84d0171640453e9272f78a63e621392e93ef6bbb Git State: clean Go Version: go1.19.10
-Compiler: gc Platform: linux/amd64 ð³ The server is running at http://
-192.168.71.93.modelz.live ð You could set the environment variable to get
-started! export MDZ_URL=http://192.168.71.93.modelz.live ``` The internal IP
-address will be used as the default endpoint of your deployments. You could
-provide the public IP address of your server to the `mdz server start` command
-to make it accessible from the outside world. ```bash # Provide the public IP
-as an argument $ mdz server start 1.2.3.4 ... ð You could set the
-environment variable to get started! export MDZ_URL=http://1.2.3.4.modelz.live
-``` ### Create your first deployment Once you've bootstrapped the `mdz` server,
-you can start deploying your first applications. ``` $ mdz deploy --image
-aikain/simplehttpserver:0.1 --name simple-server --port 80 Inference simple-
-server is created $ mdz list NAME ENDPOINT STATUS INVOCATIONS REPLICAS simple-
-server http://simple-server-4k2epq5lynxbaayn.192.168.71.93.modelz.live Ready 2
-1/1 http://192.168.71.93.modelz.live/inference/simple-server.default ``` You
-could access the deployment by visiting the endpoint URL. It will be `http://
-simple-server-4k2epq5lynxbaayn.192.168.71.93.modelz.live` in this case. The
-endpoint could be accessed from the outside world as well if you've provided
-the public IP address of your server to the `mdz server start` command. ###
-Scale your deployment You could scale your deployment by using the `mdz scale`
-command. ```bash $ mdz scale simple-server --replicas 3 ``` The requests will
-be load balanced between the replicas of your deployment. ### Debug your
-deployment Sometimes you may want to debug your deployment. You could use the
-`mdz logs` command to get the logs of your deployment. ```bash $ mdz logs
-simple-server simple-server-6756dd67ff-4bf4g: 10.42.0.1 - - [27/Jul/2023 02:32:
-16] "GET / HTTP/1.1" 200 - simple-server-6756dd67ff-4bf4g: 10.42.0.1 - - [27/
-Jul/2023 02:32:16] "GET / HTTP/1.1" 200 - simple-server-6756dd67ff-4bf4g:
-10.42.0.1 - - [27/Jul/2023 02:32:17] "GET / HTTP/1.1" 200 - ``` You could also
-use the `mdz exec` command to execute a command in the container of your
-deployment. You do not need to ssh into the server to do that. ``` $ mdz exec
-simple-server ps PID USER TIME COMMAND 1 root 0:00 /usr/bin/dumb-init /bin/sh -
-c python3 -m http.server 80 7 root 0:00 /bin/sh -c python3 -m http.server 80 8
-root 0:00 python3 -m http.server 80 9 root 0:00 ps $ mdz exec simple-server -ti
-bash bash-4.4# uname -r 5.19.0-46-generic bash-4.4# ``` Or you could port-
-forward the deployment to your local machine and debug it locally. ``` $ mdz
-port-forward simple-server 7860 Forwarding inference simple-server to local
-port 7860 ``` ### Add more servers You could add more servers to your cluster
-by using the `mdz server join` command. The `mdz` server will be bootstrapped
-on the server and join the cluster automatically. ``` $ mdz server list NAME
-PHASE ALLOCATABLE CAPACITY node1 Ready cpu: 16 cpu: 16 mem: 32784748Ki mem:
+docs.open.modelz.ai). ## Quick Start ð ### Install `mdz` You can install
+OpenModelZ using the following command: ```text pip install openmodelz ``` You
+could verify the installation by running the following command: ```text mdz ```
+Once you've installed the `mdz` you can start deploying models and
+experimenting with them. There are only two concepts in `mdz`: -
+**Deployment**: A deployment is a running inference service. You could
+configure the number of replicas, the port, and the image, and some other
+parameters. - **Server**: A server is a machine that could run the deployments.
+It could be a cloud VM, a PC, or even a Raspberry Pi. You could start from a
+single server and scale it up to a cluster of machines without any hassle. ###
+Bootstrap `mdz` It's super easy to bootstrap the `mdz` server. You just need to
+find a server (could be a cloud VM, a home lab, or even a single machine) and
+run the `mdz server start` command. The `mdz` server will be bootstrapped on
+the server and you could start deploying your models. ``` $ mdz server start
+ð§ Initializing the server... ð§ Waiting for the server to be ready... ð
+Checking if the server is running... Agent: Version: v0.0.5 Build Date: 2023-
+07-19T09:12:55Z Git Commit: 84d0171640453e9272f78a63e621392e93ef6bbb Git State:
+clean Go Version: go1.19.10 Compiler: gc Platform: linux/amd64 ð³ The server
+is running at http://192.168.71.93.modelz.live ð You could set the
+environment variable to get started! export MDZ_URL=http://
+192.168.71.93.modelz.live ``` The internal IP address will be used as the
+default endpoint of your deployments. You could provide the public IP address
+of your server to the `mdz server start` command to make it accessible from the
+outside world. ```bash # Provide the public IP as an argument $ mdz server
+start 1.2.3.4 ... ð You could set the environment variable to get started!
+export MDZ_URL=http://1.2.3.4.modelz.live ``` ### Create your first deployment
+Once you've bootstrapped the `mdz` server, you can start deploying your first
+applications. ``` $ mdz deploy --image aikain/simplehttpserver:0.1 --name
+simple-server --port 80 Inference simple-server is created $ mdz list NAME
+ENDPOINT STATUS INVOCATIONS REPLICAS simple-server http://simple-server-
+4k2epq5lynxbaayn.192.168.71.93.modelz.live Ready 2 1/1 http://
+192.168.71.93.modelz.live/inference/simple-server.default ``` You could access
+the deployment by visiting the endpoint URL. It will be `http://simple-server-
+4k2epq5lynxbaayn.192.168.71.93.modelz.live` in this case. The endpoint could be
+accessed from the outside world as well if you've provided the public IP
+address of your server to the `mdz server start` command. ### Scale your
+deployment You could scale your deployment by using the `mdz scale` command.
+```bash $ mdz scale simple-server --replicas 3 ``` The requests will be load
+balanced between the replicas of your deployment. ### Debug your deployment
+Sometimes you may want to debug your deployment. You could use the `mdz logs`
+command to get the logs of your deployment. ```bash $ mdz logs simple-server
+simple-server-6756dd67ff-4bf4g: 10.42.0.1 - - [27/Jul/2023 02:32:16] "GET /
+HTTP/1.1" 200 - simple-server-6756dd67ff-4bf4g: 10.42.0.1 - - [27/Jul/2023 02:
+32:16] "GET / HTTP/1.1" 200 - simple-server-6756dd67ff-4bf4g: 10.42.0.1 - -
+[27/Jul/2023 02:32:17] "GET / HTTP/1.1" 200 - ``` You could also use the `mdz
+exec` command to execute a command in the container of your deployment. You do
+not need to ssh into the server to do that. ``` $ mdz exec simple-server ps PID
+USER TIME COMMAND 1 root 0:00 /usr/bin/dumb-init /bin/sh -c python3 -
+m http.server 80 7 root 0:00 /bin/sh -c python3 -m http.server 80 8 root 0:00
+python3 -m http.server 80 9 root 0:00 ps $ mdz exec simple-server -ti bash
+bash-4.4# uname -r 5.19.0-46-generic bash-4.4# ``` Or you could port-forward
+the deployment to your local machine and debug it locally. ``` $ mdz port-
+forward simple-server 7860 Forwarding inference simple-server to local port
+7860 ``` ### Add more servers You could add more servers to your cluster by
+using the `mdz server join` command. The `mdz` server will be bootstrapped on
+the server and join the cluster automatically. ``` $ mdz server list NAME PHASE
+ALLOCATABLE CAPACITY node1 Ready cpu: 16 cpu: 16 mem: 32784748Ki mem:
 32784748Ki node2 Ready cpu: 16 cpu: 16 mem: 32784748Ki mem: 32784748Ki ``` ###
 Label your servers You could label your servers to deploy your models to
 specific servers. For example, you could label your servers with `gpu=true` and
 deploy your models to servers with GPUs. ``` $ mdz server label node3 gpu=true
 type=nvidia-a100 $ mdz deploy --image aikain/simplehttpserver:0.1 --name
 simple-server --port 80 --node-labels gpu=true,type=nvidia-a100 ``` ## Roadmap
 ðï¸ Please checkout [ROADMAP](https://docs.open.modelz.ai/community). ##
```

### Comparing `openmodelz-0.0.19/agent/.gitignore` & `openmodelz-0.0.20/agent/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/Makefile` & `openmodelz-0.0.20/agent/Makefile`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/build.go` & `openmodelz-0.0.20/agent/api/types/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/inference_deployment.go` & `openmodelz-0.0.20/agent/api/types/inference_deployment.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/inference_deployment_instance.go` & `openmodelz-0.0.20/agent/api/types/inference_deployment_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/inference_status.go` & `openmodelz-0.0.20/agent/api/types/inference_status.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/info.go` & `openmodelz-0.0.20/agent/api/types/info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/log.go` & `openmodelz-0.0.20/agent/api/types/log.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/queue.go` & `openmodelz-0.0.20/agent/api/types/queue.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/requests.go` & `openmodelz-0.0.20/agent/api/types/requests.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/api/types/server.go` & `openmodelz-0.0.20/agent/api/types/server.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/build.go` & `openmodelz-0.0.20/agent/client/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/client.go` & `openmodelz-0.0.20/agent/client/client.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/const.go` & `openmodelz-0.0.20/agent/client/const.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/errors.go` & `openmodelz-0.0.20/agent/client/errors.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/hijack.go` & `openmodelz-0.0.20/agent/client/hijack.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_create.go` & `openmodelz-0.0.20/agent/client/inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_get.go` & `openmodelz-0.0.20/agent/client/inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_list.go` & `openmodelz-0.0.20/agent/client/inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_remove.go` & `openmodelz-0.0.20/agent/client/inference_remove.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_scale.go` & `openmodelz-0.0.20/agent/client/inference_scale.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/inference_update.go` & `openmodelz-0.0.20/agent/client/inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/info.go` & `openmodelz-0.0.20/agent/client/info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/instance_exec.go` & `openmodelz-0.0.20/agent/client/instance_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/instance_list.go` & `openmodelz-0.0.20/agent/client/instance_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/log.go` & `openmodelz-0.0.20/agent/client/log.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/namespace_create.go` & `openmodelz-0.0.20/agent/client/namespace_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/options.go` & `openmodelz-0.0.20/agent/client/options.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/request.go` & `openmodelz-0.0.20/agent/client/request.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/server_label_create.go` & `openmodelz-0.0.20/agent/client/server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/server_list.go` & `openmodelz-0.0.20/agent/client/server_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/client/transport.go` & `openmodelz-0.0.20/agent/client/transport.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/cmd/agent/main.go` & `openmodelz-0.0.20/agent/cmd/agent/main.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/errdefs/defs.go` & `openmodelz-0.0.20/agent/errdefs/defs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/errdefs/doc.go` & `openmodelz-0.0.20/agent/errdefs/doc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/errdefs/helpers.go` & `openmodelz-0.0.20/agent/errdefs/helpers.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/errdefs/http_helpers.go` & `openmodelz-0.0.20/agent/errdefs/http_helpers.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/errdefs/is.go` & `openmodelz-0.0.20/agent/errdefs/is.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/go.mod` & `openmodelz-0.0.20/agent/go.mod`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/go.sum` & `openmodelz-0.0.20/agent/go.sum`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/app/config.go` & `openmodelz-0.0.20/agent/pkg/app/config.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/app/root.go` & `openmodelz-0.0.20/agent/pkg/app/root.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/config/config.go` & `openmodelz-0.0.20/agent/pkg/config/config.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/docs/docs.go` & `openmodelz-0.0.20/agent/pkg/docs/docs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/event/event.go` & `openmodelz-0.0.20/agent/pkg/event/event.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/convert_deployment.go` & `openmodelz-0.0.20/agent/pkg/k8s/convert_deployment.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/convert_inference.go` & `openmodelz-0.0.20/agent/pkg/k8s/convert_inference.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/convert_job.go` & `openmodelz-0.0.20/agent/pkg/k8s/convert_job.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/convert_pod.go` & `openmodelz-0.0.20/agent/pkg/k8s/convert_pod.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/generate_job.go` & `openmodelz-0.0.20/agent/pkg/k8s/generate_job.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/k8s/resolver.go` & `openmodelz-0.0.20/agent/pkg/k8s/resolver.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/log/k8s.go` & `openmodelz-0.0.20/agent/pkg/log/k8s.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/log/loki.go` & `openmodelz-0.0.20/agent/pkg/log/loki.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/metrics/exporter.go` & `openmodelz-0.0.20/agent/pkg/metrics/exporter.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/metrics/metrics.go` & `openmodelz-0.0.20/agent/pkg/metrics/metrics.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/prom/prometheus_query.go` & `openmodelz-0.0.20/agent/pkg/prom/prometheus_query.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/query/db.go` & `openmodelz-0.0.20/agent/pkg/query/db.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/query/deployment_events.sql.go` & `openmodelz-0.0.20/agent/pkg/query/deployment_events.sql.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/build.go` & `openmodelz-0.0.20/agent/pkg/runtime/build.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_create.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_delete.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_exec.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_get.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_instance.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_list.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_replicas.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_replicas.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/inference_update.go` & `openmodelz-0.0.20/agent/pkg/runtime/inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/namespace.go` & `openmodelz-0.0.20/agent/pkg/runtime/namespace.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/runtime.go` & `openmodelz-0.0.20/agent/pkg/runtime/runtime.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/server_label_create.go` & `openmodelz-0.0.20/agent/pkg/runtime/server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/server_list.go` & `openmodelz-0.0.20/agent/pkg/runtime/server_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/util_domain.go` & `openmodelz-0.0.20/agent/pkg/runtime/util_domain.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/runtime/util_resource.go` & `openmodelz-0.0.20/agent/pkg/runtime/util_resource.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/scaling/function_scaler.go` & `openmodelz-0.0.20/agent/pkg/scaling/function_scaler.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/scaling/ranges.go` & `openmodelz-0.0.20/agent/pkg/scaling/ranges.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/scaling/service_query.go` & `openmodelz-0.0.20/agent/pkg/scaling/service_query.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/scaling/util.go` & `openmodelz-0.0.20/agent/pkg/scaling/util.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/error.go` & `openmodelz-0.0.20/agent/pkg/server/error.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_build_create.go` & `openmodelz-0.0.20/agent/pkg/server/handler_build_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_build_get.go` & `openmodelz-0.0.20/agent/pkg/server/handler_build_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_build_list.go` & `openmodelz-0.0.20/agent/pkg/server/handler_build_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_build_logs.go` & `openmodelz-0.0.20/agent/pkg/server/handler_build_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_create.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_delete.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_get.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_instance.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_instance_exec.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_instance_exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_list.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_logs.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_proxy.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_scale.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_scale.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_inference_update.go` & `openmodelz-0.0.20/agent/pkg/server/handler_inference_update.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_info.go` & `openmodelz-0.0.20/agent/pkg/server/handler_info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_namespace_create.go` & `openmodelz-0.0.20/agent/pkg/server/handler_namespace_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_namespace_list.go` & `openmodelz-0.0.20/agent/pkg/server/handler_namespace_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/handler_server_label_create.go` & `openmodelz-0.0.20/agent/pkg/server/handler_server_label_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/middleware_callid.go` & `openmodelz-0.0.20/agent/pkg/server/middleware_callid.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/server_factory.go` & `openmodelz-0.0.20/agent/pkg/server/server_factory.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/server_handlerfunc.go` & `openmodelz-0.0.20/agent/pkg/server/server_handlerfunc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/server_init_kubernetes.go` & `openmodelz-0.0.20/agent/pkg/server/server_init_kubernetes.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/server_init_route.go` & `openmodelz-0.0.20/agent/pkg/server/server_init_route.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/server_run.go` & `openmodelz-0.0.20/agent/pkg/server/server_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/server/validator/validator.go` & `openmodelz-0.0.20/agent/pkg/server/validator/validator.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/agent/pkg/version/version.go` & `openmodelz-0.0.20/agent/pkg/version/version.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/.gitignore` & `openmodelz-0.0.20/mdz/.gitignore`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/Makefile` & `openmodelz-0.0.20/mdz/Makefile`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/go.mod` & `openmodelz-0.0.20/mdz/go.mod`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/go.sum` & `openmodelz-0.0.20/mdz/go.sum`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/runtime/create.go` & `openmodelz-0.0.20/mdz/pkg/agentd/runtime/create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/runtime/delete.go` & `openmodelz-0.0.20/mdz/pkg/agentd/runtime/delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/runtime/list.go` & `openmodelz-0.0.20/mdz/pkg/agentd/runtime/list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/runtime/proxy.go` & `openmodelz-0.0.20/mdz/pkg/agentd/runtime/proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/runtime/runtime.go` & `openmodelz-0.0.20/mdz/pkg/agentd/runtime/runtime.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/error.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/error.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_create.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_create.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_delete.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_get.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_get.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_list.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_logs.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_inference_proxy.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_inference_proxy.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/handler_info.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/handler_info.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/middleware_callid.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/middleware_callid.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/server_factory.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/server_factory.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/server_handlerfunc.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/server_handlerfunc.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/server_init_route.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/server_init_route.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/agentd/server/server_run.go` & `openmodelz-0.0.20/mdz/pkg/agentd/server/server_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/delete.go` & `openmodelz-0.0.20/mdz/pkg/cmd/delete.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/deploy.go` & `openmodelz-0.0.20/mdz/pkg/cmd/deploy.go`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	deployImage       string
 	deployPort        int32
 	deployMinReplicas int32
 	deployMaxReplicas int32
 	deployName        string
 	deployGPU         int
 	deployNodeLabel   []string
+	deployCommand     string
 )
 
 // deployCmd represents the deploy command
 var deployCmd = &cobra.Command{
 	Use:   "deploy",
 	Short: "Deploy a new deployment",
 	Long:  `Deploys a new deployment directly via flags.`,
@@ -49,14 +50,15 @@
 	deployCmd.Flags().StringVar(&deployImage, "image", "", "Image to deploy")
 	deployCmd.Flags().Int32Var(&deployPort, "port", 8080, "Port to deploy on")
 	deployCmd.Flags().Int32Var(&deployMinReplicas, "min-replicas", 1, "Minimum number of replicas (can be 0)")
 	deployCmd.Flags().Int32Var(&deployMaxReplicas, "max-replicas", 1, "Maximum number of replicas")
 	deployCmd.Flags().IntVar(&deployGPU, "gpu", 0, "Number of GPUs")
 	deployCmd.Flags().StringVar(&deployName, "name", "", "Name of inference")
 	deployCmd.Flags().StringSliceVarP(&deployNodeLabel, "node-labels", "l", []string{}, "Node labels")
+	deployCmd.Flags().StringVar(&deployCommand, "command", "", "Command to run")
 }
 
 func commandDeploy(cmd *cobra.Command, args []string) error {
 	if deployImage == "" {
 		return cmd.Help()
 	}
 
@@ -83,14 +85,18 @@
 				StartupDuration: int32Ptr(600),
 				ZeroDuration:    int32Ptr(600),
 			},
 			Port: int32Ptr(deployPort),
 		},
 	}
 
+	if deployCommand != "" {
+		inf.Spec.Command = &deployCommand
+	}
+
 	if len(deployNodeLabel) > 0 {
 		inf.Spec.Constraints = []string{}
 		for _, label := range deployNodeLabel {
 			inf.Spec.Constraints = append(inf.Spec.Constraints, "tensorchord.ai/"+label)
 		}
 	}
```

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/exec.go` & `openmodelz-0.0.20/mdz/pkg/cmd/exec.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/exec_stream.go` & `openmodelz-0.0.20/mdz/pkg/cmd/exec_stream.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/ioutils/reader.go` & `openmodelz-0.0.20/mdz/pkg/cmd/ioutils/reader.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/list.go` & `openmodelz-0.0.20/mdz/pkg/cmd/list.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/list_instance.go` & `openmodelz-0.0.20/mdz/pkg/cmd/list_instance.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/localagent.go` & `openmodelz-0.0.20/mdz/pkg/cmd/localagent.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/logs.go` & `openmodelz-0.0.20/mdz/pkg/cmd/logs.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/portforward.go` & `openmodelz-0.0.20/mdz/pkg/cmd/portforward.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/root.go` & `openmodelz-0.0.20/mdz/pkg/cmd/root.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/scale.go` & `openmodelz-0.0.20/mdz/pkg/cmd/scale.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/server.go` & `openmodelz-0.0.20/mdz/pkg/cmd/server.go`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import (
 	"time"
 
 	"github.com/spf13/cobra"
 )
 
 var (
-	serverVerbose         bool
-	serverPollingInterval time.Duration = 3 * time.Second
+	serverVerbose                 bool
+	serverPollingInterval         time.Duration = 3 * time.Second
+	serverRegistryMirrorName      string
+	serverRegistryMirrorEndpoints []string
 )
 
 // serverCmd represents the server command
 var serverCmd = &cobra.Command{
 	Use:     "server",
 	Short:   "Manage the servers",
 	Long:    `Manage the servers`,
```

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/server_join.go` & `openmodelz-0.0.20/mdz/pkg/cmd/server_stop.go`

 * *Files 16% similar despite different names*

```diff
@@ -3,50 +3,48 @@
 import (
 	"github.com/cockroachdb/errors"
 	"github.com/spf13/cobra"
 
 	"github.com/tensorchord/openmodelz/mdz/pkg/server"
 )
 
-// serverJoinCmd represents the server join command
-var serverJoinCmd = &cobra.Command{
-	Use:     "join",
-	Short:   "Join to the cluster",
-	Long:    `Join to the cluster`,
-	Example: `  mdz server join 192.168.31.192`,
+// serverStopCmd represents the server stop command
+var serverStopCmd = &cobra.Command{
+	Use:     "stop",
+	Short:   "Stop the server",
+	Long:    `Stop the server`,
+	Example: `  mdz server stop`,
 	PreRunE: commandInitLog,
-	Args:    cobra.ExactArgs(1),
-	RunE:    commandServerJoin,
+	RunE:    commandServerStop,
 }
 
 func init() {
-	serverCmd.AddCommand(serverJoinCmd)
+	serverCmd.AddCommand(serverStopCmd)
 
 	// Here you will define your flags and configuration settings.
 
 	// Cobra supports Persistent Flags which will work for this command
 	// and all subcommands, e.g.:
 
 	// Cobra supports local flags which will only run when this command
 	// is called directly, e.g.:
 }
 
-func commandServerJoin(cmd *cobra.Command, args []string) error {
-	engine, err := server.NewJoin(server.Options{
+func commandServerStop(cmd *cobra.Command, args []string) error {
+	engine, err := server.NewStop(server.Options{
 		Verbose:       serverVerbose,
 		OutputStream:  cmd.ErrOrStderr(),
 		RetryInternal: serverPollingInterval,
-		ServerIP:      args[0],
 	})
 	if err != nil {
-		cmd.PrintErrf("Failed to join the cluster: %s\n", errors.Cause(err))
+		cmd.PrintErrf("Failed to stop the server: %s\n", errors.Cause(err))
 		return err
 	}
 
 	_, err = engine.Run()
 	if err != nil {
-		cmd.PrintErrf("Failed to join the cluster: %s\n", errors.Cause(err))
+		cmd.PrintErrf("Failed to stop the server: %s\n", errors.Cause(err))
 		return err
 	}
-	cmd.Printf("✅ Server joined\n")
+	cmd.Printf("✅ Server stopped\n")
 	return nil
 }
```

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/server_label.go` & `openmodelz-0.0.20/mdz/pkg/cmd/server_label.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/server_list.go` & `openmodelz-0.0.20/mdz/pkg/cmd/server_list.go`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,17 @@
 }
 
 func labelsString(labels map[string]string) string {
 	res := ""
 	for k, v := range labels {
 		res += fmt.Sprintf("%s=%s\n", k, v)
 	}
+	if len(res) == 0 {
+		return res
+	}
 	return res[:len(res)-1]
 }
 
 func resourceListString(l types.ResourceList) string {
 	res := fmt.Sprintf("cpu: %s\nmem: %s", l["cpu"], l["memory"])
 	if l[types.ResourceGPU] != "" {
 		res += fmt.Sprintf("\ngpu: %s", l[types.ResourceGPU])
```

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/server_start.go` & `openmodelz-0.0.20/mdz/pkg/cmd/server_start.go`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 	// is called directly, e.g.:
 	// serverStartCmd.Flags().StringVarP(&serverStartRuntime, "runtime", "r", "k3s", "Runtime to use (k3s, docker) in the started server")
 	serverStartCmd.Flags().StringVarP(&serverStartVersion, "version", "",
 		version.HelmChartVersion, "Version of the server to start")
 	serverStartCmd.Flags().MarkHidden("version")
 	serverStartCmd.Flags().BoolVarP(&serverStartWithGPU, "force-gpu", "g",
 		false, "Start the server with GPU support (ignore the GPU detection)")
+	serverStartCmd.Flags().StringVarP(&serverRegistryMirrorName, "mirror-name", "",
+		"", "Mirror name of the registry")
+	serverStartCmd.Flags().StringArrayVarP(&serverRegistryMirrorEndpoints, "mirror-endpoints", "",
+		[]string{}, "Mirror endpoints of the registry")
 }
 
 func commandServerStart(cmd *cobra.Command, args []string) error {
 	var domain *string
 	if len(args) > 0 {
 		domainWithSuffix := fmt.Sprintf("%s.%s", args[0], serverStartDomain)
 		domain = &domainWithSuffix
@@ -60,14 +64,18 @@
 		Verbose:       serverVerbose,
 		Runtime:       server.Runtime(serverStartRuntime),
 		OutputStream:  cmd.ErrOrStderr(),
 		RetryInternal: serverPollingInterval,
 		Domain:        domain,
 		Version:       serverStartVersion,
 		ForceGPU:      serverStartWithGPU,
+		Mirror: server.Mirror{
+			Name:      serverRegistryMirrorName,
+			Endpoints: serverRegistryMirrorEndpoints,
+		},
 	})
 	if err != nil {
 		cmd.PrintErrf("Failed to start the server: %s\n", errors.Cause(err))
 		return err
 	}
 
 	result, err := engine.Run()
```

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/streams/in.go` & `openmodelz-0.0.20/mdz/pkg/cmd/streams/in.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/streams/out.go` & `openmodelz-0.0.20/mdz/pkg/cmd/streams/out.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/streams/stream.go` & `openmodelz-0.0.20/mdz/pkg/cmd/streams/stream.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/cmd/version.go` & `openmodelz-0.0.20/mdz/pkg/cmd/version.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/agentd_run.go` & `openmodelz-0.0.20/mdz/pkg/server/agentd_run.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/engine.go` & `openmodelz-0.0.20/mdz/pkg/server/engine.go`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,31 @@
 	AgentPort = 31112
 )
 
 type Options struct {
 	Verbose       bool
 	OutputStream  io.Writer
 	Runtime       Runtime
+	Mirror        Mirror
 	RetryInternal time.Duration
 	ServerIP      string
 	Domain        *string
 	Version       string
 	ForceGPU      bool
 }
 
+type Mirror struct {
+	Name      string
+	Endpoints []string
+}
+
+func (m *Mirror) Configured() bool {
+	return m.Name != "" && len(m.Endpoints) > 0
+}
+
 type Runtime string
 
 var (
 	RuntimeK3s    Runtime = "k3s"
 	RuntimeDocker Runtime = "docker"
 )
 
@@ -34,14 +44,17 @@
 }
 
 type Result struct {
 	MDZURL string
 }
 
 func NewStart(o Options) (*Engine, error) {
+	if o.Verbose {
+		fmt.Fprintf(o.OutputStream, "Starting the server with config: %+v\n", o)
+	}
 	var engine *Engine
 	switch o.Runtime {
 	case RuntimeDocker:
 		engine = &Engine{
 			options: o,
 			Steps: []Step{
 				&agentDRunStep{
@@ -50,14 +63,17 @@
 			},
 		}
 	default:
 		engine = &Engine{
 			options: o,
 			Steps: []Step{
 				// Install k3s and related tools.
+				&k3sPrepare{
+					options: o,
+				},
 				&k3sInstallStep{
 					options: o,
 				},
 				&nginxInstallStep{
 					options: o,
 				},
 				&gpuInstallStep{
```

### Comparing `openmodelz-0.0.19/mdz/pkg/server/gpu_install.go` & `openmodelz-0.0.20/mdz/pkg/server/gpu_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/k3s-install.sh` & `openmodelz-0.0.20/mdz/pkg/server/k3s-install.sh`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/k3s_install.go` & `openmodelz-0.0.20/mdz/pkg/server/k3s_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/k3s_join.go` & `openmodelz-0.0.20/mdz/pkg/server/k3s_join.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/k3s_killall.go` & `openmodelz-0.0.20/mdz/pkg/server/k3s_killall.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/nginx-dep.yaml` & `openmodelz-0.0.20/mdz/pkg/server/nginx-dep.yaml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/nginx_install.go` & `openmodelz-0.0.20/mdz/pkg/server/nginx_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/server/openmodelz_install.go` & `openmodelz-0.0.20/mdz/pkg/server/openmodelz_install.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/term/interrupt.go` & `openmodelz-0.0.20/mdz/pkg/term/interrupt.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/term/term.go` & `openmodelz-0.0.20/mdz/pkg/term/term.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/mdz/pkg/version/version.go` & `openmodelz-0.0.20/mdz/pkg/version/version.go`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/openmodelz.egg-info/SOURCES.txt` & `openmodelz-0.0.20/openmodelz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -185,18 +185,20 @@
 mdz/pkg/server/engine.go
 mdz/pkg/server/gpu-resource.yaml
 mdz/pkg/server/gpu_install.go
 mdz/pkg/server/k3s-install.sh
 mdz/pkg/server/k3s_install.go
 mdz/pkg/server/k3s_join.go
 mdz/pkg/server/k3s_killall.go
+mdz/pkg/server/k3s_prepare.go
 mdz/pkg/server/nginx-dep.yaml
 mdz/pkg/server/nginx_install.go
 mdz/pkg/server/openmodelz.yaml
 mdz/pkg/server/openmodelz_install.go
+mdz/pkg/server/registries.yaml
 mdz/pkg/term/interrupt.go
 mdz/pkg/term/term.go
 mdz/pkg/version/version.go
 openmodelz.egg-info/PKG-INFO
 openmodelz.egg-info/SOURCES.txt
 openmodelz.egg-info/dependency_links.txt
 openmodelz.egg-info/not-zip-safe
```

### Comparing `openmodelz-0.0.19/pyproject.toml` & `openmodelz-0.0.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmodelz-0.0.19/setup.py` & `openmodelz-0.0.20/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import shlex
 from wheel.bdist_wheel import bdist_wheel
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 from setuptools_scm import get_version
 
 
+with open("README.md", "r", encoding="utf-8") as f:
+    readme = f.read()
+
 class bdist_wheel_universal(bdist_wheel):
     def get_tag(self):
         *_, plat = super().get_tag()
         return "py2.py3", "none", plat
 
 
 def build_if_not_exist():
@@ -36,14 +39,21 @@
 
         build_if_not_exist()
 
 
 setup(
     name="openmodelz",
     use_scm_version=True,
+    description="Simplify machine learning deployment for any environments.",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url="https://github.com/tensorchord/openmodelz",
+    license="Apache License 2.0",
+    author="TensorChord",
+    author_email="modelz@tensorchord.ai",
     packages=find_packages("mdz"),
     include_package_data=True,
     data_files=[("bin", ["mdz/bin/mdz"])],
     zip_safe=False,
     ext_modules=[
         ModelzExtension(name="mdz", sources=["mdz/*"]),
     ],
```

