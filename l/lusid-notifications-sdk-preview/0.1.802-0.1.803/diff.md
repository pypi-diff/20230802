# Comparing `tmp/lusid-notifications-sdk-preview-0.1.802.tar.gz` & `tmp/lusid-notifications-sdk-preview-0.1.803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.802.tar", last modified: Mon Jul 31 09:30:43 2023, max compression
+gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.803.tar", last modified: Wed Aug  2 10:31:13 2023, max compression
```

## Comparing `lusid-notifications-sdk-preview-0.1.802.tar` & `lusid-notifications-sdk-preview-0.1.803.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9646 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/
--rw-r--r--   0 root         (0) root         (0)     4432 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10524 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   122660 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47811 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9027 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    13280 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_details.py
--rw-r--r--   0 root         (0) root         (0)     4727 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)    10747 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9540 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10705 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7437 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18059 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6099 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7775 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16992 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/utilities/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2745 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 09:30:43.000000 lusid-notifications-sdk-preview-0.1.802/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2322 2023-07-31 09:28:16.000000 lusid-notifications-sdk-preview-0.1.802/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      373 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9646 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10524 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   122660 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47811 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13280 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16932 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_details.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9540 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10705 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    18059 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7775 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7327 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16992 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    17004 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/utilities/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-02 10:31:12.000000 lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 10:31:13.000000 lusid-notifications-sdk-preview-0.1.803/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-08-02 10:28:02.000000 lusid-notifications-sdk-preview-0.1.803/setup.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/README.md` & `lusid-notifications-sdk-preview-0.1.803/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.802
-- Package version: 0.1.802
+- API version: 0.1.803
+- Package version: 0.1.803
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/__init__.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.802"
+__version__ = "0.1.803"
 
 # import apis into sdk package
 from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notifications.api.deliveries_api import DeliveriesApi
 from lusid_notifications.api.event_types_api import EventTypesApi
 from lusid_notifications.api.events_api import EventsApi
 from lusid_notifications.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/application_metadata_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/application_metadata_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/deliveries_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/deliveries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/event_types_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/events_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -150,15 +150,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "EventDetails",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/notifications_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/notifications_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -201,15 +201,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -384,15 +384,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -567,15 +567,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -750,15 +750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -930,15 +930,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1107,15 +1107,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1277,15 +1277,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -1480,15 +1480,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1683,15 +1683,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1886,15 +1886,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -2089,15 +2089,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api/subscriptions_api.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.802'
+        header_params['X-LUSID-SDK-Version'] = '0.1.803'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/api_client.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.802/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.803/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/configuration.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.802\n"\
-               "SDK Package Version: 0.1.802".\
+               "Version of the API: 0.1.803\n"\
+               "SDK Package Version: 0.1.803".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/exceptions.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/__init__.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/access_controlled_action.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/action_id.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/attempt.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/attempt_status.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/attempt_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_email_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_subscription.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/create_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/create_webhook_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -73,15 +73,15 @@
         
         :param description:  The summary of the services provided by the notification (required)
         :type description: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
-        :param authentication_type:  The type of authentication to use on the request (required)
+        :param authentication_type:  The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict(str, str)
         :param content_type:  The type of the content e.g. Json
         :type content_type: str
         :param content:  The content of the request
         :type content: object
@@ -204,26 +204,26 @@
 
         self._url = url
 
     @property
     def authentication_type(self):
         """Gets the authentication_type of this CreateWebhookNotification.  # noqa: E501
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :return: The authentication_type of this CreateWebhookNotification.  # noqa: E501
         :rtype: str
         """
         return self._authentication_type
 
     @authentication_type.setter
     def authentication_type(self, authentication_type):
         """Sets the authentication_type of this CreateWebhookNotification.
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :param authentication_type: The authentication_type of this CreateWebhookNotification.  # noqa: E501
         :type authentication_type: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_type is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/delivery.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_details.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_field_definition.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_field_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/id_selector_definition.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/identifier_part_schema.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/link.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/lusid_problem_details.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/matching_pattern.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/notification_status.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/notification_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_id.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_delivery.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/resource_list_of_subscription.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/subscription.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_email_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_subscription.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/models/update_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/models/update_webhook_notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -73,17 +73,17 @@
         
         :param description:  The summary of the services provided by the notification (required)
         :type description: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
-        :param authentication_type:  The type of authentication to use on the request (required)
+        :param authentication_type:  The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call (required)
         :type authentication_type: str
-        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
+        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None Required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict(str, str)
         :param content_type:  The type of the content e.g. Json
         :type content_type: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
@@ -204,26 +204,26 @@
 
         self._url = url
 
     @property
     def authentication_type(self):
         """Gets the authentication_type of this UpdateWebhookNotification.  # noqa: E501
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :return: The authentication_type of this UpdateWebhookNotification.  # noqa: E501
         :rtype: str
         """
         return self._authentication_type
 
     @authentication_type.setter
     def authentication_type(self, authentication_type):
         """Sets the authentication_type of this UpdateWebhookNotification.
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :param authentication_type: The authentication_type of this UpdateWebhookNotification.  # noqa: E501
         :type authentication_type: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_type is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
@@ -232,26 +232,26 @@
 
         self._authentication_type = authentication_type
 
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this UpdateWebhookNotification.  # noqa: E501
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None Required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this UpdateWebhookNotification.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this UpdateWebhookNotification.
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None Required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this UpdateWebhookNotification.  # noqa: E501
         :type authentication_configuration_item_paths: dict(str, str)
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/rest.py` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.802
+    The version of the OpenAPI document: 0.1.803
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications/utilities/config_keys.json` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.802/lusid_notifications_sdk_preview.egg-info/SOURCES.txt` & `lusid-notifications-sdk-preview-0.1.803/lusid_notifications_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.802/setup.py` & `lusid-notifications-sdk-preview-0.1.803/setup.py`

 * *Files identical despite different names*

