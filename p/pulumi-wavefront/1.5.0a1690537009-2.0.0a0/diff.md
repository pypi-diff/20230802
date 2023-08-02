# Comparing `tmp/pulumi_wavefront-1.5.0a1690537009.tar.gz` & `tmp/pulumi_wavefront-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-1.5.0a1690537009.tar", last modified: Fri Jul 28 09:40:38 2023, max compression
+gzip compressed data, was "pulumi_wavefront-2.0.0a0.tar", last modified: Wed Aug  2 15:40:52 2023, max compression
```

## Comparing `pulumi_wavefront-1.5.0a1690537009.tar` & `pulumi_wavefront-2.0.0a0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76663 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   209561 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:40:38.885118 pulumi_wavefront-1.5.0a1690537009/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-28 09:40:38.000000 pulumi_wavefront-1.5.0a1690537009/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78096 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210614 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:40:52.963550 pulumi_wavefront-2.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-02 15:40:52.000000 pulumi_wavefront-2.0.0a0/setup.py
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/PKG-INFO` & `pulumi_wavefront-2.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 1.5.0a1690537009
+Version: 2.0.0a0
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -42,15 +42,15 @@
 
     $ pip install pulumi_wavefront
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-wavefront/sdk
+    $ go get github.com/pulumi/pulumi-wavefront/sdk/v2
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Wavefront
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/README.md` & `pulumi_wavefront-2.0.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     $ pip install pulumi_wavefront
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-wavefront/sdk
+    $ go get github.com/pulumi/pulumi-wavefront/sdk/v2
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Wavefront
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/__init__.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'CloudIntegrationNewRelicMetricFilterArgs',
     'DashboardParameterDetailArgs',
     'DashboardSectionArgs',
     'DashboardSectionRowArgs',
     'DashboardSectionRowChartArgs',
     'DashboardSectionRowChartChartSettingArgs',
     'DashboardSectionRowChartSourceArgs',
+    'IngestionPolicyTagArgs',
     'MetricsPolicyPolicyRuleArgs',
     'MetricsPolicyPolicyRuleTagArgs',
 ]
 
 @pulumi.input_type
 class AlertTargetRouteArgs:
     def __init__(__self__, *,
@@ -318,36 +319,40 @@
                  chart_setting: pulumi.Input['DashboardSectionRowChartChartSettingArgs'],
                  name: pulumi.Input[str],
                  sources: pulumi.Input[Sequence[pulumi.Input['DashboardSectionRowChartSourceArgs']]],
                  summarization: pulumi.Input[str],
                  units: pulumi.Input[str],
                  base: Optional[pulumi.Input[int]] = None,
                  chart_attribute: Optional[pulumi.Input[str]] = None,
-                 description: Optional[pulumi.Input[str]] = None):
+                 description: Optional[pulumi.Input[str]] = None,
+                 no_default_events: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input['DashboardSectionRowChartChartSettingArgs'] chart_setting: Chart settings. See chart settings.
         :param pulumi.Input[str] name: Name of the source.
         :param pulumi.Input[Sequence[pulumi.Input['DashboardSectionRowChartSourceArgs']]] sources: Query expression to plot on the chart. See chart source queries.
         :param pulumi.Input[str] summarization: Summarization strategy for the chart. MEAN is default. Valid options are, `MEAN`, 
                `MEDIAN`, `MIN`, `MAX`, `SUM`, `COUNT`, `LAST`, `FIRST`.
         :param pulumi.Input[str] units: String to label the units of the chart on the Y-Axis.
         :param pulumi.Input[int] base: The base of logarithmic scale charts. Omit or set to 0 for the default linear scale. Usually set to 10 for the traditional logarithmic scale.
         :param pulumi.Input[str] description: Description of the chart.
+        :param pulumi.Input[bool] no_default_events: Show events related to the sources included in queries
         """
         pulumi.set(__self__, "chart_setting", chart_setting)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sources", sources)
         pulumi.set(__self__, "summarization", summarization)
         pulumi.set(__self__, "units", units)
         if base is not None:
             pulumi.set(__self__, "base", base)
         if chart_attribute is not None:
             pulumi.set(__self__, "chart_attribute", chart_attribute)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if no_default_events is not None:
+            pulumi.set(__self__, "no_default_events", no_default_events)
 
     @property
     @pulumi.getter(name="chartSetting")
     def chart_setting(self) -> pulumi.Input['DashboardSectionRowChartChartSettingArgs']:
         """
         Chart settings. See chart settings.
         """
@@ -435,14 +440,26 @@
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
+    @property
+    @pulumi.getter(name="noDefaultEvents")
+    def no_default_events(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Show events related to the sources included in queries
+        """
+        return pulumi.get(self, "no_default_events")
+
+    @no_default_events.setter
+    def no_default_events(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_default_events", value)
+
 
 @pulumi.input_type
 class DashboardSectionRowChartChartSettingArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  auto_column_tags: Optional[pulumi.Input[bool]] = None,
                  column_tags: Optional[pulumi.Input[str]] = None,
@@ -1508,14 +1525,41 @@
 
     @source_description.setter
     def source_description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_description", value)
 
 
 @pulumi.input_type
+class IngestionPolicyTagArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class MetricsPolicyPolicyRuleArgs:
     def __init__(__self__, *,
                  access_type: pulumi.Input[str],
                  description: pulumi.Input[str],
                  name: pulumi.Input[str],
                  prefixes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  tags_anded: pulumi.Input[bool],
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/alert.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/alert_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/event.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/external_link.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alert.py`

 * *Files 10% similar despite different names*

```diff
@@ -328,37 +328,37 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['targets'] = targets
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getAlert:getAlert', __args__, opts=opts, typ=GetAlertResult).value
 
     return AwaitableGetAlertResult(
-        additional_information=__ret__.additional_information,
-        alert_type=__ret__.alert_type,
-        can_modifies=__ret__.can_modifies,
-        can_views=__ret__.can_views,
-        condition=__ret__.condition,
-        conditions=__ret__.conditions,
-        display_expression=__ret__.display_expression,
-        evaluate_realtime_data=__ret__.evaluate_realtime_data,
-        failing_host_label_pairs=__ret__.failing_host_label_pairs,
-        id=__ret__.id,
-        in_maintenance_host_label_pairs=__ret__.in_maintenance_host_label_pairs,
-        include_obsolete_metrics=__ret__.include_obsolete_metrics,
-        minutes=__ret__.minutes,
-        name=__ret__.name,
-        notification_resend_frequency_minutes=__ret__.notification_resend_frequency_minutes,
-        process_rate_minutes=__ret__.process_rate_minutes,
-        resolve_after_minutes=__ret__.resolve_after_minutes,
-        severity=__ret__.severity,
-        severity_lists=__ret__.severity_lists,
-        statuses=__ret__.statuses,
-        tags=__ret__.tags,
-        target=__ret__.target,
-        targets=__ret__.targets)
+        additional_information=pulumi.get(__ret__, 'additional_information'),
+        alert_type=pulumi.get(__ret__, 'alert_type'),
+        can_modifies=pulumi.get(__ret__, 'can_modifies'),
+        can_views=pulumi.get(__ret__, 'can_views'),
+        condition=pulumi.get(__ret__, 'condition'),
+        conditions=pulumi.get(__ret__, 'conditions'),
+        display_expression=pulumi.get(__ret__, 'display_expression'),
+        evaluate_realtime_data=pulumi.get(__ret__, 'evaluate_realtime_data'),
+        failing_host_label_pairs=pulumi.get(__ret__, 'failing_host_label_pairs'),
+        id=pulumi.get(__ret__, 'id'),
+        in_maintenance_host_label_pairs=pulumi.get(__ret__, 'in_maintenance_host_label_pairs'),
+        include_obsolete_metrics=pulumi.get(__ret__, 'include_obsolete_metrics'),
+        minutes=pulumi.get(__ret__, 'minutes'),
+        name=pulumi.get(__ret__, 'name'),
+        notification_resend_frequency_minutes=pulumi.get(__ret__, 'notification_resend_frequency_minutes'),
+        process_rate_minutes=pulumi.get(__ret__, 'process_rate_minutes'),
+        resolve_after_minutes=pulumi.get(__ret__, 'resolve_after_minutes'),
+        severity=pulumi.get(__ret__, 'severity'),
+        severity_lists=pulumi.get(__ret__, 'severity_lists'),
+        statuses=pulumi.get(__ret__, 'statuses'),
+        tags=pulumi.get(__ret__, 'tags'),
+        target=pulumi.get(__ret__, 'target'),
+        targets=pulumi.get(__ret__, 'targets'))
 
 
 @_utilities.lift_output_func(get_alert)
 def get_alert_output(id: Optional[pulumi.Input[str]] = None,
                      targets: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAlertResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_alerts.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getAlerts:getAlerts', __args__, opts=opts, typ=GetAlertsResult).value
 
     return AwaitableGetAlertsResult(
-        alerts=__ret__.alerts,
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset)
+        alerts=pulumi.get(__ret__, 'alerts'),
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_alerts)
 def get_alerts_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                       offset: Optional[pulumi.Input[Optional[int]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAlertsResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -400,49 +400,49 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDashboard:getDashboard', __args__, opts=opts, typ=GetDashboardResult).value
 
     return AwaitableGetDashboardResult(
-        can_modifies=__ret__.can_modifies,
-        can_views=__ret__.can_views,
-        chart_title_bg_color=__ret__.chart_title_bg_color,
-        chart_title_color=__ret__.chart_title_color,
-        chart_title_scalar=__ret__.chart_title_scalar,
-        created_epoch_millis=__ret__.created_epoch_millis,
-        creator_id=__ret__.creator_id,
-        customer=__ret__.customer,
-        default_end_time=__ret__.default_end_time,
-        default_start_time=__ret__.default_start_time,
-        default_time_window=__ret__.default_time_window,
-        deleted=__ret__.deleted,
-        description=__ret__.description,
-        display_description=__ret__.display_description,
-        display_query_parameters=__ret__.display_query_parameters,
-        display_section_table_of_contents=__ret__.display_section_table_of_contents,
-        event_filter_type=__ret__.event_filter_type,
-        event_query=__ret__.event_query,
-        favorite=__ret__.favorite,
-        hidden=__ret__.hidden,
-        id=__ret__.id,
-        name=__ret__.name,
-        num_charts=__ret__.num_charts,
-        num_favorites=__ret__.num_favorites,
-        parameter_details=__ret__.parameter_details,
-        parameters=__ret__.parameters,
-        sections=__ret__.sections,
-        system_owned=__ret__.system_owned,
-        tags=__ret__.tags,
-        updated_epoch_millis=__ret__.updated_epoch_millis,
-        updater_id=__ret__.updater_id,
-        url=__ret__.url,
-        views_last_day=__ret__.views_last_day,
-        views_last_month=__ret__.views_last_month,
-        views_last_week=__ret__.views_last_week)
+        can_modifies=pulumi.get(__ret__, 'can_modifies'),
+        can_views=pulumi.get(__ret__, 'can_views'),
+        chart_title_bg_color=pulumi.get(__ret__, 'chart_title_bg_color'),
+        chart_title_color=pulumi.get(__ret__, 'chart_title_color'),
+        chart_title_scalar=pulumi.get(__ret__, 'chart_title_scalar'),
+        created_epoch_millis=pulumi.get(__ret__, 'created_epoch_millis'),
+        creator_id=pulumi.get(__ret__, 'creator_id'),
+        customer=pulumi.get(__ret__, 'customer'),
+        default_end_time=pulumi.get(__ret__, 'default_end_time'),
+        default_start_time=pulumi.get(__ret__, 'default_start_time'),
+        default_time_window=pulumi.get(__ret__, 'default_time_window'),
+        deleted=pulumi.get(__ret__, 'deleted'),
+        description=pulumi.get(__ret__, 'description'),
+        display_description=pulumi.get(__ret__, 'display_description'),
+        display_query_parameters=pulumi.get(__ret__, 'display_query_parameters'),
+        display_section_table_of_contents=pulumi.get(__ret__, 'display_section_table_of_contents'),
+        event_filter_type=pulumi.get(__ret__, 'event_filter_type'),
+        event_query=pulumi.get(__ret__, 'event_query'),
+        favorite=pulumi.get(__ret__, 'favorite'),
+        hidden=pulumi.get(__ret__, 'hidden'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        num_charts=pulumi.get(__ret__, 'num_charts'),
+        num_favorites=pulumi.get(__ret__, 'num_favorites'),
+        parameter_details=pulumi.get(__ret__, 'parameter_details'),
+        parameters=pulumi.get(__ret__, 'parameters'),
+        sections=pulumi.get(__ret__, 'sections'),
+        system_owned=pulumi.get(__ret__, 'system_owned'),
+        tags=pulumi.get(__ret__, 'tags'),
+        updated_epoch_millis=pulumi.get(__ret__, 'updated_epoch_millis'),
+        updater_id=pulumi.get(__ret__, 'updater_id'),
+        url=pulumi.get(__ret__, 'url'),
+        views_last_day=pulumi.get(__ret__, 'views_last_day'),
+        views_last_month=pulumi.get(__ret__, 'views_last_month'),
+        views_last_week=pulumi.get(__ret__, 'views_last_week'))
 
 
 @_utilities.lift_output_func(get_dashboard)
 def get_dashboard_output(id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDashboardResult]:
     """
     Use this data source to get information about a certain Wavefront dashboard by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_dashboards.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDashboards:getDashboards', __args__, opts=opts, typ=GetDashboardsResult).value
 
     return AwaitableGetDashboardsResult(
-        dashboards=__ret__.dashboards,
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset)
+        dashboards=pulumi.get(__ret__, 'dashboards'),
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_dashboards)
 def get_dashboards_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                           offset: Optional[pulumi.Input[Optional[int]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDashboardsResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_default_user_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDefaultUserGroup:getDefaultUserGroup', __args__, opts=opts, typ=GetDefaultUserGroupResult).value
 
     return AwaitableGetDefaultUserGroupResult(
-        group_id=__ret__.group_id,
-        id=__ret__.id)
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -339,38 +339,38 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDerivedMetric:getDerivedMetric', __args__, opts=opts, typ=GetDerivedMetricResult).value
 
     return AwaitableGetDerivedMetricResult(
-        additional_information=__ret__.additional_information,
-        create_user_id=__ret__.create_user_id,
-        created_epoch_millis=__ret__.created_epoch_millis,
-        deleted=__ret__.deleted,
-        hosts_useds=__ret__.hosts_useds,
-        id=__ret__.id,
-        in_trash=__ret__.in_trash,
-        include_obsolete_metrics=__ret__.include_obsolete_metrics,
-        last_error_message=__ret__.last_error_message,
-        last_failed_time=__ret__.last_failed_time,
-        last_processed_millis=__ret__.last_processed_millis,
-        last_query_time=__ret__.last_query_time,
-        metrics_useds=__ret__.metrics_useds,
-        minutes=__ret__.minutes,
-        name=__ret__.name,
-        points_scanned_at_last_query=__ret__.points_scanned_at_last_query,
-        process_rate_minutes=__ret__.process_rate_minutes,
-        query=__ret__.query,
-        query_failing=__ret__.query_failing,
-        query_qb_enabled=__ret__.query_qb_enabled,
-        statuses=__ret__.statuses,
-        tags=__ret__.tags,
-        update_user_id=__ret__.update_user_id,
-        updated_epoch_millis=__ret__.updated_epoch_millis)
+        additional_information=pulumi.get(__ret__, 'additional_information'),
+        create_user_id=pulumi.get(__ret__, 'create_user_id'),
+        created_epoch_millis=pulumi.get(__ret__, 'created_epoch_millis'),
+        deleted=pulumi.get(__ret__, 'deleted'),
+        hosts_useds=pulumi.get(__ret__, 'hosts_useds'),
+        id=pulumi.get(__ret__, 'id'),
+        in_trash=pulumi.get(__ret__, 'in_trash'),
+        include_obsolete_metrics=pulumi.get(__ret__, 'include_obsolete_metrics'),
+        last_error_message=pulumi.get(__ret__, 'last_error_message'),
+        last_failed_time=pulumi.get(__ret__, 'last_failed_time'),
+        last_processed_millis=pulumi.get(__ret__, 'last_processed_millis'),
+        last_query_time=pulumi.get(__ret__, 'last_query_time'),
+        metrics_useds=pulumi.get(__ret__, 'metrics_useds'),
+        minutes=pulumi.get(__ret__, 'minutes'),
+        name=pulumi.get(__ret__, 'name'),
+        points_scanned_at_last_query=pulumi.get(__ret__, 'points_scanned_at_last_query'),
+        process_rate_minutes=pulumi.get(__ret__, 'process_rate_minutes'),
+        query=pulumi.get(__ret__, 'query'),
+        query_failing=pulumi.get(__ret__, 'query_failing'),
+        query_qb_enabled=pulumi.get(__ret__, 'query_qb_enabled'),
+        statuses=pulumi.get(__ret__, 'statuses'),
+        tags=pulumi.get(__ret__, 'tags'),
+        update_user_id=pulumi.get(__ret__, 'update_user_id'),
+        updated_epoch_millis=pulumi.get(__ret__, 'updated_epoch_millis'))
 
 
 @_utilities.lift_output_func(get_derived_metric)
 def get_derived_metric_output(id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDerivedMetricResult]:
     """
     Use this data source to get information about a certain Wavefront derived metric by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_derived_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDerivedMetrics:getDerivedMetrics', __args__, opts=opts, typ=GetDerivedMetricsResult).value
 
     return AwaitableGetDerivedMetricsResult(
-        derived_metrics=__ret__.derived_metrics,
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset)
+        derived_metrics=pulumi.get(__ret__, 'derived_metrics'),
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_derived_metrics)
 def get_derived_metrics_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                                offset: Optional[pulumi.Input[Optional[int]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDerivedMetricsResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_event.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,24 +168,24 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getEvent:getEvent', __args__, opts=opts, typ=GetEventResult).value
 
     return AwaitableGetEventResult(
-        annotations=__ret__.annotations,
-        details=__ret__.details,
-        endtime_key=__ret__.endtime_key,
-        id=__ret__.id,
-        is_ephemeral=__ret__.is_ephemeral,
-        name=__ret__.name,
-        severity=__ret__.severity,
-        start_time=__ret__.start_time,
-        tags=__ret__.tags,
-        type=__ret__.type)
+        annotations=pulumi.get(__ret__, 'annotations'),
+        details=pulumi.get(__ret__, 'details'),
+        endtime_key=pulumi.get(__ret__, 'endtime_key'),
+        id=pulumi.get(__ret__, 'id'),
+        is_ephemeral=pulumi.get(__ret__, 'is_ephemeral'),
+        name=pulumi.get(__ret__, 'name'),
+        severity=pulumi.get(__ret__, 'severity'),
+        start_time=pulumi.get(__ret__, 'start_time'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_event)
 def get_event_output(id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEventResult]:
     """
     Use this data source to get information about a certain Wavefront event.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_events.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,20 +130,20 @@
     __args__['latestStartTimeEpochMillis'] = latest_start_time_epoch_millis
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getEvents:getEvents', __args__, opts=opts, typ=GetEventsResult).value
 
     return AwaitableGetEventsResult(
-        earliest_start_time_epoch_millis=__ret__.earliest_start_time_epoch_millis,
-        events=__ret__.events,
-        id=__ret__.id,
-        latest_start_time_epoch_millis=__ret__.latest_start_time_epoch_millis,
-        limit=__ret__.limit,
-        offset=__ret__.offset)
+        earliest_start_time_epoch_millis=pulumi.get(__ret__, 'earliest_start_time_epoch_millis'),
+        events=pulumi.get(__ret__, 'events'),
+        id=pulumi.get(__ret__, 'id'),
+        latest_start_time_epoch_millis=pulumi.get(__ret__, 'latest_start_time_epoch_millis'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_events)
 def get_events_output(earliest_start_time_epoch_millis: Optional[pulumi.Input[int]] = None,
                       latest_start_time_epoch_millis: Optional[pulumi.Input[int]] = None,
                       limit: Optional[pulumi.Input[Optional[int]]] = None,
                       offset: Optional[pulumi.Input[Optional[int]]] = None,
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_link.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,26 +198,26 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getExternalLink:getExternalLink', __args__, opts=opts, typ=GetExternalLinkResult).value
 
     return AwaitableGetExternalLinkResult(
-        created_epoch_millis=__ret__.created_epoch_millis,
-        creator_id=__ret__.creator_id,
-        description=__ret__.description,
-        id=__ret__.id,
-        is_log_integration=__ret__.is_log_integration,
-        metric_filter_regex=__ret__.metric_filter_regex,
-        name=__ret__.name,
-        point_tag_filter_regexes=__ret__.point_tag_filter_regexes,
-        source_filter_regex=__ret__.source_filter_regex,
-        template=__ret__.template,
-        updated_epoch_millis=__ret__.updated_epoch_millis,
-        updater_id=__ret__.updater_id)
+        created_epoch_millis=pulumi.get(__ret__, 'created_epoch_millis'),
+        creator_id=pulumi.get(__ret__, 'creator_id'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        is_log_integration=pulumi.get(__ret__, 'is_log_integration'),
+        metric_filter_regex=pulumi.get(__ret__, 'metric_filter_regex'),
+        name=pulumi.get(__ret__, 'name'),
+        point_tag_filter_regexes=pulumi.get(__ret__, 'point_tag_filter_regexes'),
+        source_filter_regex=pulumi.get(__ret__, 'source_filter_regex'),
+        template=pulumi.get(__ret__, 'template'),
+        updated_epoch_millis=pulumi.get(__ret__, 'updated_epoch_millis'),
+        updater_id=pulumi.get(__ret__, 'updater_id'))
 
 
 @_utilities.lift_output_func(get_external_link)
 def get_external_link_output(id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetExternalLinkResult]:
     """
     Use this data source to get information about a Wavefront external link by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_external_links.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getExternalLinks:getExternalLinks', __args__, opts=opts, typ=GetExternalLinksResult).value
 
     return AwaitableGetExternalLinksResult(
-        external_links=__ret__.external_links,
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset)
+        external_links=pulumi.get(__ret__, 'external_links'),
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_external_links)
 def get_external_links_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                               offset: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetExternalLinksResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -273,32 +273,32 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getMaintenanceWindow:getMaintenanceWindow', __args__, opts=opts, typ=GetMaintenanceWindowResult).value
 
     return AwaitableGetMaintenanceWindowResult(
-        created_epoch_millis=__ret__.created_epoch_millis,
-        creator_id=__ret__.creator_id,
-        customer_id=__ret__.customer_id,
-        end_time_in_seconds=__ret__.end_time_in_seconds,
-        event_name=__ret__.event_name,
-        host_tag_group_host_names_group_anded=__ret__.host_tag_group_host_names_group_anded,
-        id=__ret__.id,
-        reason=__ret__.reason,
-        relevant_customer_tags=__ret__.relevant_customer_tags,
-        relevant_host_names=__ret__.relevant_host_names,
-        relevant_host_tags=__ret__.relevant_host_tags,
-        relevant_host_tags_anded=__ret__.relevant_host_tags_anded,
-        running_state=__ret__.running_state,
-        sort_attr=__ret__.sort_attr,
-        start_time_in_seconds=__ret__.start_time_in_seconds,
-        title=__ret__.title,
-        updated_epoch_millis=__ret__.updated_epoch_millis,
-        updater_id=__ret__.updater_id)
+        created_epoch_millis=pulumi.get(__ret__, 'created_epoch_millis'),
+        creator_id=pulumi.get(__ret__, 'creator_id'),
+        customer_id=pulumi.get(__ret__, 'customer_id'),
+        end_time_in_seconds=pulumi.get(__ret__, 'end_time_in_seconds'),
+        event_name=pulumi.get(__ret__, 'event_name'),
+        host_tag_group_host_names_group_anded=pulumi.get(__ret__, 'host_tag_group_host_names_group_anded'),
+        id=pulumi.get(__ret__, 'id'),
+        reason=pulumi.get(__ret__, 'reason'),
+        relevant_customer_tags=pulumi.get(__ret__, 'relevant_customer_tags'),
+        relevant_host_names=pulumi.get(__ret__, 'relevant_host_names'),
+        relevant_host_tags=pulumi.get(__ret__, 'relevant_host_tags'),
+        relevant_host_tags_anded=pulumi.get(__ret__, 'relevant_host_tags_anded'),
+        running_state=pulumi.get(__ret__, 'running_state'),
+        sort_attr=pulumi.get(__ret__, 'sort_attr'),
+        start_time_in_seconds=pulumi.get(__ret__, 'start_time_in_seconds'),
+        title=pulumi.get(__ret__, 'title'),
+        updated_epoch_millis=pulumi.get(__ret__, 'updated_epoch_millis'),
+        updater_id=pulumi.get(__ret__, 'updater_id'))
 
 
 @_utilities.lift_output_func(get_maintenance_window)
 def get_maintenance_window_output(id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMaintenanceWindowResult]:
     """
     Use this data source to get information about a Wavefront maintenance window by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getMaintenanceWindowAll:getMaintenanceWindowAll', __args__, opts=opts, typ=GetMaintenanceWindowAllResult).value
 
     return AwaitableGetMaintenanceWindowAllResult(
-        id=__ret__.id,
-        limit=__ret__.limit,
-        maintenance_windows=__ret__.maintenance_windows,
-        offset=__ret__.offset)
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        maintenance_windows=pulumi.get(__ret__, 'maintenance_windows'),
+        offset=pulumi.get(__ret__, 'offset'))
 
 
 @_utilities.lift_output_func(get_maintenance_window_all)
 def get_maintenance_window_all_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                                       offset: Optional[pulumi.Input[Optional[int]]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMaintenanceWindowAllResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_metrics_policy.py`

 * *Files 17% similar despite different names*

```diff
@@ -85,12 +85,12 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getMetricsPolicy:getMetricsPolicy', __args__, opts=opts, typ=GetMetricsPolicyResult).value
 
     return AwaitableGetMetricsPolicyResult(
-        customer=__ret__.customer,
-        id=__ret__.id,
-        policy_rules=__ret__.policy_rules,
-        updated_epoch_millis=__ret__.updated_epoch_millis,
-        updater_id=__ret__.updater_id)
+        customer=pulumi.get(__ret__, 'customer'),
+        id=pulumi.get(__ret__, 'id'),
+        policy_rules=pulumi.get(__ret__, 'policy_rules'),
+        updated_epoch_millis=pulumi.get(__ret__, 'updated_epoch_millis'),
+        updater_id=pulumi.get(__ret__, 'updater_id'))
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_role.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,18 +99,18 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
     return AwaitableGetRoleResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        permissions=__ret__.permissions)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        permissions=pulumi.get(__ret__, 'permissions'))
 
 
 @_utilities.lift_output_func(get_role)
 def get_role_output(id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
     """
     Use this data source to get information about a Wavefront role by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
 
     return AwaitableGetRolesResult(
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset,
-        roles=__ret__.roles)
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'),
+        roles=pulumi.get(__ret__, 'roles'))
 
 
 @_utilities.lift_output_func(get_roles)
 def get_roles_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                      offset: Optional[pulumi.Input[Optional[int]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRolesResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,20 +120,20 @@
     """
     __args__ = dict()
     __args__['email'] = email
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        customer=__ret__.customer,
-        email=__ret__.email,
-        id=__ret__.id,
-        last_successful_login=__ret__.last_successful_login,
-        permissions=__ret__.permissions,
-        user_group_ids=__ret__.user_group_ids)
+        customer=pulumi.get(__ret__, 'customer'),
+        email=pulumi.get(__ret__, 'email'),
+        id=pulumi.get(__ret__, 'id'),
+        last_successful_login=pulumi.get(__ret__, 'last_successful_login'),
+        permissions=pulumi.get(__ret__, 'permissions'),
+        user_group_ids=pulumi.get(__ret__, 'user_group_ids'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(email: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to get information for a given user by email from Wavefront.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,19 +111,19 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getUserGroup:getUserGroup', __args__, opts=opts, typ=GetUserGroupResult).value
 
     return AwaitableGetUserGroupResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        roles=__ret__.roles,
-        users=__ret__.users)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        roles=pulumi.get(__ret__, 'roles'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_user_group)
 def get_user_group_output(id: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserGroupResult]:
     """
     Use this data source to get information about a Wavefront user group by its ID.
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_user_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     __args__ = dict()
     __args__['limit'] = limit
     __args__['offset'] = offset
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getUserGroups:getUserGroups', __args__, opts=opts, typ=GetUserGroupsResult).value
 
     return AwaitableGetUserGroupsResult(
-        id=__ret__.id,
-        limit=__ret__.limit,
-        offset=__ret__.offset,
-        user_groups=__ret__.user_groups)
+        id=pulumi.get(__ret__, 'id'),
+        limit=pulumi.get(__ret__, 'limit'),
+        offset=pulumi.get(__ret__, 'offset'),
+        user_groups=pulumi.get(__ret__, 'user_groups'))
 
 
 @_utilities.lift_output_func(get_user_groups)
 def get_user_groups_output(limit: Optional[pulumi.Input[Optional[int]]] = None,
                            offset: Optional[pulumi.Input[Optional[int]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserGroupsResult]:
     """
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/get_users.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/get_users.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
     return AwaitableGetUsersResult(
-        id=__ret__.id,
-        users=__ret__.users)
+        id=pulumi.get(__ret__, 'id'),
+        users=pulumi.get(__ret__, 'users'))
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/outputs.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     'CloudIntegrationNewRelicMetricFilter',
     'DashboardParameterDetail',
     'DashboardSection',
     'DashboardSectionRow',
     'DashboardSectionRowChart',
     'DashboardSectionRowChartChartSetting',
     'DashboardSectionRowChartSource',
+    'IngestionPolicyTag',
     'MetricsPolicyPolicyRule',
     'MetricsPolicyPolicyRuleTag',
     'GetAlertFailingHostLabelPairResult',
     'GetAlertInMaintenanceHostLabelPairResult',
     'GetAlertsAlertResult',
     'GetAlertsAlertFailingHostLabelPairResult',
     'GetAlertsAlertInMaintenanceHostLabelPairResult',
@@ -325,14 +326,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "chartSetting":
             suggest = "chart_setting"
         elif key == "chartAttribute":
             suggest = "chart_attribute"
+        elif key == "noDefaultEvents":
+            suggest = "no_default_events"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in DashboardSectionRowChart. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         DashboardSectionRowChart.__key_warning(key)
         return super().__getitem__(key)
@@ -345,36 +348,40 @@
                  chart_setting: 'outputs.DashboardSectionRowChartChartSetting',
                  name: str,
                  sources: Sequence['outputs.DashboardSectionRowChartSource'],
                  summarization: str,
                  units: str,
                  base: Optional[int] = None,
                  chart_attribute: Optional[str] = None,
-                 description: Optional[str] = None):
+                 description: Optional[str] = None,
+                 no_default_events: Optional[bool] = None):
         """
         :param 'DashboardSectionRowChartChartSettingArgs' chart_setting: Chart settings. See chart settings.
         :param str name: Name of the source.
         :param Sequence['DashboardSectionRowChartSourceArgs'] sources: Query expression to plot on the chart. See chart source queries.
         :param str summarization: Summarization strategy for the chart. MEAN is default. Valid options are, `MEAN`, 
                `MEDIAN`, `MIN`, `MAX`, `SUM`, `COUNT`, `LAST`, `FIRST`.
         :param str units: String to label the units of the chart on the Y-Axis.
         :param int base: The base of logarithmic scale charts. Omit or set to 0 for the default linear scale. Usually set to 10 for the traditional logarithmic scale.
         :param str description: Description of the chart.
+        :param bool no_default_events: Show events related to the sources included in queries
         """
         pulumi.set(__self__, "chart_setting", chart_setting)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sources", sources)
         pulumi.set(__self__, "summarization", summarization)
         pulumi.set(__self__, "units", units)
         if base is not None:
             pulumi.set(__self__, "base", base)
         if chart_attribute is not None:
             pulumi.set(__self__, "chart_attribute", chart_attribute)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if no_default_events is not None:
+            pulumi.set(__self__, "no_default_events", no_default_events)
 
     @property
     @pulumi.getter(name="chartSetting")
     def chart_setting(self) -> 'outputs.DashboardSectionRowChartChartSetting':
         """
         Chart settings. See chart settings.
         """
@@ -430,14 +437,22 @@
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
         Description of the chart.
         """
         return pulumi.get(self, "description")
 
+    @property
+    @pulumi.getter(name="noDefaultEvents")
+    def no_default_events(self) -> Optional[bool]:
+        """
+        Show events related to the sources included in queries
+        """
+        return pulumi.get(self, "no_default_events")
+
 
 @pulumi.output_type
 class DashboardSectionRowChartChartSetting(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "autoColumnTags":
@@ -1381,14 +1396,33 @@
         """
         A description for the purpose of this source.
         """
         return pulumi.get(self, "source_description")
 
 
 @pulumi.output_type
+class IngestionPolicyTag(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 value: str):
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class MetricsPolicyPolicyRule(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "accessType":
             suggest = "access_type"
         elif key == "tagsAnded":
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/provider.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/role.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/service_account.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/user.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront/user_group.py` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-wavefront
-Version: 1.5.0a1690537009
+Version: 2.0.0a0
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -42,15 +42,15 @@
 
     $ pip install pulumi_wavefront
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-wavefront/sdk
+    $ go get github.com/pulumi/pulumi-wavefront/sdk/v2
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Wavefront
```

### Comparing `pulumi_wavefront-1.5.0a1690537009/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-2.0.0a0/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1690537009/setup.py` & `pulumi_wavefront-2.0.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.5.0a1690537009"
-PLUGIN_VERSION = "1.5.0-alpha.1690537009+0bb8d1d9"
+VERSION = "2.0.0a0"
+PLUGIN_VERSION = "2.0.0-alpha.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'wavefront', PLUGIN_VERSION])
         except OSError as error:
```

