# Comparing `tmp/lusid-notification-sdk-preview-0.1.802.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.802.tar", last modified: Mon Jul 31 09:34:03 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.803.tar", last modified: Wed Aug  2 10:35:01 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.802.tar` & `lusid-notification-sdk-preview-0.1.803.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8236 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27783 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3399 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11055 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     8318 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    10618 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    13061 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15029 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/email_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6879 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    16037 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    33958 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)    24077 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8104 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6008 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/sms_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8447 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15899 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13098 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/models/webhook_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2868 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 09:34:03.000000 lusid-notification-sdk-preview-0.1.802/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-31 09:32:49.000000 lusid-notification-sdk-preview-0.1.802/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27783 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11055 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8318 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10618 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    13061 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15029 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6879 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    34801 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    24077 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8447 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16742 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13098 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 10:35:01.000000 lusid-notification-sdk-preview-0.1.803/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-08-02 10:34:27.000000 lusid-notification-sdk-preview-0.1.803/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.802/README.md` & `lusid-notification-sdk-preview-0.1.803/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/__init__.py`

 * *Files 1% similar despite different names*

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
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api/application_metadata_api.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api/event_types_api.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api/manual_event_api.py`

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
 
@@ -155,15 +155,15 @@
 
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
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api/notifications_api.py`

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
 
@@ -195,15 +195,15 @@
 
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
@@ -375,15 +375,15 @@
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
@@ -552,15 +552,15 @@
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
@@ -722,15 +722,15 @@
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
@@ -925,15 +925,15 @@
 
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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api/subscriptions_api.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/api_client.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/configuration.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/exceptions.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/__init__.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/access_controlled_action.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/access_controlled_resource.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/action_id.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/amazon_sqs_notification_type.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/amazon_sqs_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/amazon_sqs_notification_type_response.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/create_notification_request.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/create_subscription.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/email_notification_type.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/email_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/email_notification_type_response.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/event_field_definition.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/event_type_schema.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/id_selector_definition.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/identifier_part_schema.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/link.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/lusid_problem_details.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/lusid_validation_problem_details.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_body.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_header.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/manual_event_request.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/matching_pattern.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_status.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_type.py`

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
@@ -128,17 +128,17 @@
         :type email_address_bcc: list[str]
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
-        :param authentication_type:  The type of authentication to use on the request (required)
+        :param authentication_type:  The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call (required)
         :type authentication_type: str
-        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
+        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
@@ -610,26 +610,26 @@
 
         self._url = url
 
     @property
     def authentication_type(self):
         """Gets the authentication_type of this NotificationType.  # noqa: E501
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :return: The authentication_type of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._authentication_type
 
     @authentication_type.setter
     def authentication_type(self, authentication_type):
         """Sets the authentication_type of this NotificationType.
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :param authentication_type: The authentication_type of this NotificationType.  # noqa: E501
         :type authentication_type: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_type is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
@@ -638,26 +638,26 @@
 
         self._authentication_type = authentication_type
 
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this NotificationType.  # noqa: E501
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
         :rtype: dict[str, str]
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this NotificationType.
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
         :type authentication_configuration_item_paths: dict[str, str]
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
```

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/notification_type_response.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/notification_type_response.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_id.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_access_controlled_resource.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_event_type_schema.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_notification.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/resource_list_of_subscription.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/sms_notification_type.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/sms_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/sms_notification_type_response.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/subscription.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/update_notification_request.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/update_subscription.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/webhook_notification_type.py`

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
@@ -73,17 +73,17 @@
         
         :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
-        :param authentication_type:  The type of authentication to use on the request (required)
+        :param authentication_type:  The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call (required)
         :type authentication_type: str
-        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
+        :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
@@ -201,26 +201,26 @@
 
         self._url = url
 
     @property
     def authentication_type(self):
         """Gets the authentication_type of this WebhookNotificationType.  # noqa: E501
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :return: The authentication_type of this WebhookNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._authentication_type
 
     @authentication_type.setter
     def authentication_type(self, authentication_type):
         """Sets the authentication_type of this WebhookNotificationType.
 
-        The type of authentication to use on the request  # noqa: E501
+        The type of authentication to use on the request, can be one of the following values:  - Lusid -  Internal LUSID call  - BasicAuth - User specified Username and password  - BearerToken - Authorization header with Bearer scheme and user specified key  - None - No Authorization required on the webhook call  # noqa: E501
 
         :param authentication_type: The authentication_type of this WebhookNotificationType.  # noqa: E501
         :type authentication_type: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_type is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
@@ -229,26 +229,26 @@
 
         self._authentication_type = authentication_type
 
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
         :rtype: dict[str, str]
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this WebhookNotificationType.
 
-        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
+        The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'  - None - None required                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
         :type authentication_configuration_item_paths: dict[str, str]
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
```

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/models/webhook_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/models/webhook_notification_type_response.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/rest.py`

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

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.803/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.802/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.803/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.802/setup.py` & `lusid-notification-sdk-preview-0.1.803/setup.py`

 * *Files identical despite different names*

