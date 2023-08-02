# Comparing `tmp/pulumi_signalfx-6.0.0.tar.gz` & `tmp/pulumi_signalfx-6.0.0a1690994377.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-6.0.0.tar", last modified: Wed Jul 26 20:20:00 2023, max compression
+gzip compressed data, was "pulumi_signalfx-6.0.0a1690994377.tar", last modified: Wed Aug  2 16:43:45 2023, max compression
```

## Comparing `pulumi_signalfx-6.0.0.tar` & `pulumi_signalfx-6.0.0a1690994377.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    81078 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61578 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34425 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62676 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (123)   127525 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    80156 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.405810 pulumi_signalfx-6.0.0a1690994377/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-02 16:43:45.405810 pulumi_signalfx-6.0.0a1690994377/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.397810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81078 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61578 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62676 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/logs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/logs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28664 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/logs/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127525 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.405810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80156 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.405810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:43:45.401810 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:43:45.405810 pulumi_signalfx-6.0.0a1690994377/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-02 16:43:45.000000 pulumi_signalfx-6.0.0a1690994377/setup.py
```

### Comparing `pulumi_signalfx-6.0.0/PKG-INFO` & `pulumi_signalfx-6.0.0a1690994377/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 6.0.0
+Version: 6.0.0a1690994377
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_signalfx-6.0.0/README.md` & `pulumi_signalfx-6.0.0a1690994377/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/__init__.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     azure = __azure
     import pulumi_signalfx.config as __config
     config = __config
     import pulumi_signalfx.gcp as __gcp
     gcp = __gcp
     import pulumi_signalfx.jira as __jira
     jira = __jira
+    import pulumi_signalfx.log as __log
+    log = __log
     import pulumi_signalfx.logs as __logs
     logs = __logs
     import pulumi_signalfx.opsgenie as __opsgenie
     opsgenie = __opsgenie
     import pulumi_signalfx.pagerduty as __pagerduty
     pagerduty = __pagerduty
     import pulumi_signalfx.servicenow as __servicenow
@@ -52,14 +54,15 @@
     victorops = __victorops
 else:
     aws = _utilities.lazy_import('pulumi_signalfx.aws')
     azure = _utilities.lazy_import('pulumi_signalfx.azure')
     config = _utilities.lazy_import('pulumi_signalfx.config')
     gcp = _utilities.lazy_import('pulumi_signalfx.gcp')
     jira = _utilities.lazy_import('pulumi_signalfx.jira')
+    log = _utilities.lazy_import('pulumi_signalfx.log')
     logs = _utilities.lazy_import('pulumi_signalfx.logs')
     opsgenie = _utilities.lazy_import('pulumi_signalfx.opsgenie')
     pagerduty = _utilities.lazy_import('pulumi_signalfx.pagerduty')
     servicenow = _utilities.lazy_import('pulumi_signalfx.servicenow')
     slack = _utilities.lazy_import('pulumi_signalfx.slack')
     victorops = _utilities.lazy_import('pulumi_signalfx.victorops')
 
@@ -240,14 +243,30 @@
   "fqn": "pulumi_signalfx.jira",
   "classes": {
    "signalfx:jira/integration:Integration": "Integration"
   }
  },
  {
   "pkg": "signalfx",
+  "mod": "log/timeline",
+  "fqn": "pulumi_signalfx.log",
+  "classes": {
+   "signalfx:log/timeline:Timeline": "Timeline"
+  }
+ },
+ {
+  "pkg": "signalfx",
+  "mod": "log/view",
+  "fqn": "pulumi_signalfx.log",
+  "classes": {
+   "signalfx:log/view:View": "View"
+  }
+ },
+ {
+  "pkg": "signalfx",
   "mod": "logs/view",
   "fqn": "pulumi_signalfx.logs",
   "classes": {
    "signalfx:logs/view:View": "View"
   }
  },
  {
```

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/data_link.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/detector.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,16 @@
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  project_service_keys: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_metric_source_project_for_quota: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that you want to monitor
-        :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-               to true.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
+        :param pulumi.Input[bool] import_gcp_metrics: If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]] project_service_keys: GCP projects to add.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
@@ -72,28 +71,27 @@
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="customMetricTypeDomains")
     def custom_metric_type_domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of additional GCP service domain names that you want to monitor
+        List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         """
         return pulumi.get(self, "custom_metric_type_domains")
 
     @custom_metric_type_domains.setter
     def custom_metric_type_domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_metric_type_domains", value)
 
     @property
     @pulumi.getter(name="importGcpMetrics")
     def import_gcp_metrics(self) -> Optional[pulumi.Input[bool]]:
         """
-        If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-        to true.
+        If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         """
         return pulumi.get(self, "import_gcp_metrics")
 
     @import_gcp_metrics.setter
     def import_gcp_metrics(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "import_gcp_metrics", value)
 
@@ -193,18 +191,17 @@
                  named_token: Optional[pulumi.Input[str]] = None,
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  project_service_keys: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_metric_source_project_for_quota: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that you want to monitor
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
-        :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-               to true.
+        :param pulumi.Input[bool] import_gcp_metrics: If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]] project_service_keys: GCP projects to add.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
@@ -230,15 +227,15 @@
         if use_metric_source_project_for_quota is not None:
             pulumi.set(__self__, "use_metric_source_project_for_quota", use_metric_source_project_for_quota)
 
     @property
     @pulumi.getter(name="customMetricTypeDomains")
     def custom_metric_type_domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of additional GCP service domain names that you want to monitor
+        List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         """
         return pulumi.get(self, "custom_metric_type_domains")
 
     @custom_metric_type_domains.setter
     def custom_metric_type_domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_metric_type_domains", value)
 
@@ -254,16 +251,15 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="importGcpMetrics")
     def import_gcp_metrics(self) -> Optional[pulumi.Input[bool]]:
         """
-        If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-        to true.
+        If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         """
         return pulumi.get(self, "import_gcp_metrics")
 
     @import_gcp_metrics.setter
     def import_gcp_metrics(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "import_gcp_metrics", value)
 
@@ -376,15 +372,17 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         gcp_myteam = signalfx.gcp.Integration("gcpMyteam",
+            custom_metric_type_domains=["istio.io"],
             enabled=True,
+            import_gcp_metrics=True,
             poll_rate=300,
             project_service_keys=[
                 signalfx.gcp.IntegrationProjectServiceKeyArgs(
                     project_id="gcp_project_id_1",
                     project_key=(lambda path: open(path).read())("/path/to/gcp_credentials_1.json"),
                 ),
                 signalfx.gcp.IntegrationProjectServiceKeyArgs(
@@ -393,18 +391,17 @@
                 ),
             ],
             services=["compute"])
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that you want to monitor
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
-        :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-               to true.
+        :param pulumi.Input[bool] import_gcp_metrics: If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationProjectServiceKeyArgs']]]] project_service_keys: GCP projects to add.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
@@ -423,15 +420,17 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         gcp_myteam = signalfx.gcp.Integration("gcpMyteam",
+            custom_metric_type_domains=["istio.io"],
             enabled=True,
+            import_gcp_metrics=True,
             poll_rate=300,
             project_service_keys=[
                 signalfx.gcp.IntegrationProjectServiceKeyArgs(
                     project_id="gcp_project_id_1",
                     project_key=(lambda path: open(path).read())("/path/to/gcp_credentials_1.json"),
                 ),
                 signalfx.gcp.IntegrationProjectServiceKeyArgs(
@@ -513,18 +512,17 @@
         """
         Get an existing Integration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that you want to monitor
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_metric_type_domains: List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
-        :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-               to true.
+        :param pulumi.Input[bool] import_gcp_metrics: If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationProjectServiceKeyArgs']]]] project_service_keys: GCP projects to add.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
@@ -545,15 +543,15 @@
         __props__.__dict__["use_metric_source_project_for_quota"] = use_metric_source_project_for_quota
         return Integration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="customMetricTypeDomains")
     def custom_metric_type_domains(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of additional GCP service domain names that you want to monitor
+        List of additional GCP service domain names that Splunk Observability Cloud will monitor. See [Custom Metric Type Domains documentation](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/#Custom-metric-type-domains)
         """
         return pulumi.get(self, "custom_metric_type_domains")
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Output[bool]:
         """
@@ -561,16 +559,15 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="importGcpMetrics")
     def import_gcp_metrics(self) -> pulumi.Output[Optional[bool]]:
         """
-        If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
-        to true.
+        If enabled, Splunk Observability Cloud will sync also Google Cloud Monitoring data. If disabled, Splunk Observability Cloud will import only metadata. Defaults to true.
         """
         return pulumi.get(self, "import_gcp_metrics")
 
     @property
     @pulumi.getter(name="includeLists")
     def include_lists(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/_inputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/outputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/view.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/log/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,40 +352,40 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
-        my_log_view = signalfx.logs.View("myLogView",
+        my_log_view = signalfx.log.View("myLogView",
             columns=[
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="severity",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="time",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.currency_code",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.nanos",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.units",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="message",
                 ),
             ],
             description="Lorem ipsum dolor sit amet, laudem tibique iracundia at mea. Nam posse dolores ex, nec cu adhuc putent honestatis",
             program_text=\"\"\"logs(filter=field('message') == 'Transaction processed' and field('service.name') == 'paymentservice').publish()
 
         \"\"\",
-            sort_options=[signalfx.logs.ViewSortOptionArgs(
+            sort_options=[signalfx.log.ViewSortOptionArgs(
                 descending=False,
                 field="severity",
             )],
             time_range=900)
         ```
 
         :param str resource_name: The name of the resource.
@@ -411,40 +411,40 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
-        my_log_view = signalfx.logs.View("myLogView",
+        my_log_view = signalfx.log.View("myLogView",
             columns=[
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="severity",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="time",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.currency_code",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.nanos",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="amount.units",
                 ),
-                signalfx.logs.ViewColumnArgs(
+                signalfx.log.ViewColumnArgs(
                     name="message",
                 ),
             ],
             description="Lorem ipsum dolor sit amet, laudem tibique iracundia at mea. Nam posse dolores ex, nec cu adhuc putent honestatis",
             program_text=\"\"\"logs(filter=field('message') == 'Transaction processed' and field('service.name') == 'paymentservice').publish()
 
         \"\"\",
-            sort_options=[signalfx.logs.ViewSortOptionArgs(
+            sort_options=[signalfx.log.ViewSortOptionArgs(
                 descending=False,
                 field="severity",
             )],
             time_range=900)
         ```
 
         :param str resource_name: The name of the resource.
@@ -488,16 +488,18 @@
             if program_text is None and not opts.urn:
                 raise TypeError("Missing required property 'program_text'")
             __props__.__dict__["program_text"] = program_text
             __props__.__dict__["sort_options"] = sort_options
             __props__.__dict__["start_time"] = start_time
             __props__.__dict__["time_range"] = time_range
             __props__.__dict__["url"] = None
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="signalfx:logs/view:View")])
+        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
         super(View, __self__).__init__(
-            'signalfx:logs/view:View',
+            'signalfx:log/view:View',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
```

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/org_token.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/outputs.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/provider.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/team.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-signalfx
-Version: 6.0.0
+Version: 6.0.0a1690994377
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-6.0.0a1690994377/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 pulumi_signalfx/config/vars.py
 pulumi_signalfx/gcp/__init__.py
 pulumi_signalfx/gcp/_inputs.py
 pulumi_signalfx/gcp/integration.py
 pulumi_signalfx/gcp/outputs.py
 pulumi_signalfx/jira/__init__.py
 pulumi_signalfx/jira/integration.py
+pulumi_signalfx/log/__init__.py
+pulumi_signalfx/log/_inputs.py
+pulumi_signalfx/log/outputs.py
+pulumi_signalfx/log/timeline.py
+pulumi_signalfx/log/view.py
 pulumi_signalfx/logs/__init__.py
 pulumi_signalfx/logs/_inputs.py
 pulumi_signalfx/logs/outputs.py
 pulumi_signalfx/logs/view.py
 pulumi_signalfx/opsgenie/__init__.py
 pulumi_signalfx/opsgenie/integration.py
 pulumi_signalfx/pagerduty/__init__.py
```

### Comparing `pulumi_signalfx-6.0.0/setup.py` & `pulumi_signalfx-6.0.0a1690994377/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.0.0"
-PLUGIN_VERSION = "6.0.0"
+VERSION = "6.0.0a1690994377"
+PLUGIN_VERSION = "6.0.0-alpha.1690994377+490f1bb0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'signalfx', PLUGIN_VERSION])
         except OSError as error:
```

