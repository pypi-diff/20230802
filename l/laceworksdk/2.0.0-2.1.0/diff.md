# Comparing `tmp/laceworksdk-2.0.0.tar.gz` & `tmp/laceworksdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laceworksdk-2.0.0.tar", max compression
+gzip compressed data, was "laceworksdk-2.1.0.tar", max compression
```

## Comparing `laceworksdk-2.0.0.tar` & `laceworksdk-2.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-06-29 09:44:02.591009 laceworksdk-2.0.0/LICENSE
--rw-r--r--   0        0        0     3956 2023-06-29 09:44:02.591009 laceworksdk-2.0.0/README.md
--rw-r--r--   0        0        0      412 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/__init__.py
--rw-r--r--   0        0        0     7572 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/__init__.py
--rw-r--r--   0        0        0     4288 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/base_endpoint.py
--rw-r--r--   0        0        0     3110 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/crud_endpoint.py
--rw-r--r--   0        0        0     1330 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/read_endpoint.py
--rw-r--r--   0        0        0     1612 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/search_endpoint.py
--rw-r--r--   0        0        0        0 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/__init__.py
--rw-r--r--   0        0        0     2000 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/activities.py
--rw-r--r--   0        0        0     2402 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/agent_access_tokens.py
--rw-r--r--   0        0        0      414 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/agent_info.py
--rw-r--r--   0        0        0     3834 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/alert_channels.py
--rw-r--r--   0        0        0     3551 2023-06-29 09:44:02.611009 laceworksdk-2.0.0/laceworksdk/api/v2/alert_profiles.py
--rw-r--r--   0        0        0     4325 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/alert_rules.py
--rw-r--r--   0        0        0     4538 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/alerts.py
--rw-r--r--   0        0        0     1558 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/audit_logs.py
--rw-r--r--   0        0        0     3484 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/cloud_accounts.py
--rw-r--r--   0        0        0     2566 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/cloud_activities.py
--rw-r--r--   0        0        0     1821 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/configs.py
--rw-r--r--   0        0        0     3549 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/container_registries.py
--rw-r--r--   0        0        0      900 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/contract_info.py
--rw-r--r--   0        0        0     2029 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/datasources.py
--rw-r--r--   0        0        0     5539 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/entities.py
--rw-r--r--   0        0        0     2861 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/events.py
--rw-r--r--   0        0        0     1516 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/inventory.py
--rw-r--r--   0        0        0      654 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/organization_info.py
--rw-r--r--   0        0        0     7228 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/policies.py
--rw-r--r--   0        0        0     4127 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/policy_exceptions.py
--rw-r--r--   0        0        0     5446 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/queries.py
--rw-r--r--   0        0        0     7183 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/report_definitions.py
--rw-r--r--   0        0        0     4383 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/report_rules.py
--rw-r--r--   0        0        0     2250 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/reports.py
--rw-r--r--   0        0        0     3286 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/resource_groups.py
--rw-r--r--   0        0        0     1092 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/schemas.py
--rw-r--r--   0        0        0     5376 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/team_members.py
--rw-r--r--   0        0        0     3185 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/team_users.py
--rw-r--r--   0        0        0     1378 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/user_groups.py
--rw-r--r--   0        0        0      624 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/user_profile.py
--rw-r--r--   0        0        0     4834 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerabilities.py
--rw-r--r--   0        0        0     7086 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_exceptions.py
--rw-r--r--   0        0        0     7094 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_policies.py
--rw-r--r--   0        0        0      696 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/config.py
--rw-r--r--   0        0        0     2498 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/exceptions.py
--rw-r--r--   0        0        0    14468 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/laceworksdk/http_session.py
--rw-r--r--   0        0        0     1576 2023-06-29 09:44:02.615008 laceworksdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5238 1970-01-01 00:00:00.000000 laceworksdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-02 10:53:32.429608 laceworksdk-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3956 2023-08-02 10:53:32.429608 laceworksdk-2.1.0/README.md
+-rw-r--r--   0        0        0      412 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/__init__.py
+-rw-r--r--   0        0        0     7572 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/__init__.py
+-rw-r--r--   0        0        0     4288 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/base_endpoint.py
+-rw-r--r--   0        0        0     3110 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/crud_endpoint.py
+-rw-r--r--   0        0        0     1330 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/read_endpoint.py
+-rw-r--r--   0        0        0     1612 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/search_endpoint.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/__init__.py
+-rw-r--r--   0        0        0     2000 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/activities.py
+-rw-r--r--   0        0        0     2402 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/agent_access_tokens.py
+-rw-r--r--   0        0        0      414 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/agent_info.py
+-rw-r--r--   0        0        0     3834 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/alert_channels.py
+-rw-r--r--   0        0        0     3551 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/alert_profiles.py
+-rw-r--r--   0        0        0     4325 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/alert_rules.py
+-rw-r--r--   0        0        0     4538 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/alerts.py
+-rw-r--r--   0        0        0     1558 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/audit_logs.py
+-rw-r--r--   0        0        0     3484 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/cloud_accounts.py
+-rw-r--r--   0        0        0     2566 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/cloud_activities.py
+-rw-r--r--   0        0        0     1821 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/configs.py
+-rw-r--r--   0        0        0     3549 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/container_registries.py
+-rw-r--r--   0        0        0      900 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/contract_info.py
+-rw-r--r--   0        0        0     2029 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/datasources.py
+-rw-r--r--   0        0        0     5539 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/entities.py
+-rw-r--r--   0        0        0     2861 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/events.py
+-rw-r--r--   0        0        0     1516 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/inventory.py
+-rw-r--r--   0        0        0      654 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/organization_info.py
+-rw-r--r--   0        0        0     7228 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/policies.py
+-rw-r--r--   0        0        0     4127 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/policy_exceptions.py
+-rw-r--r--   0        0        0     5446 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/queries.py
+-rw-r--r--   0        0        0     7183 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/report_definitions.py
+-rw-r--r--   0        0        0     4383 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/report_rules.py
+-rw-r--r--   0        0        0     2250 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/reports.py
+-rw-r--r--   0        0        0     3286 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/resource_groups.py
+-rw-r--r--   0        0        0     1092 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/schemas.py
+-rw-r--r--   0        0        0     5376 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/team_members.py
+-rw-r--r--   0        0        0     3185 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/team_users.py
+-rw-r--r--   0        0        0     1378 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/user_groups.py
+-rw-r--r--   0        0        0      624 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/user_profile.py
+-rw-r--r--   0        0        0     4834 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/vulnerabilities.py
+-rw-r--r--   0        0        0     7086 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/vulnerability_exceptions.py
+-rw-r--r--   0        0        0     7094 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/api/v2/vulnerability_policies.py
+-rw-r--r--   0        0        0      696 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/config.py
+-rw-r--r--   0        0        0     2498 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/exceptions.py
+-rw-r--r--   0        0        0    14468 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/laceworksdk/http_session.py
+-rw-r--r--   0        0        0     1498 2023-08-02 10:53:32.449609 laceworksdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 laceworksdk-2.1.0/PKG-INFO
```

### Comparing `laceworksdk-2.0.0/LICENSE` & `laceworksdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/README.md` & `laceworksdk-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         }
     ]
 })
 ```
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.8 or higher
 - Lacework API Credentials
   - Account Name
   - API Key
   - API Secret
 
 ## How-To
```

### Comparing `laceworksdk-2.0.0/laceworksdk/api/__init__.py` & `laceworksdk-2.1.0/laceworksdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/base_endpoint.py` & `laceworksdk-2.1.0/laceworksdk/api/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/crud_endpoint.py` & `laceworksdk-2.1.0/laceworksdk/api/crud_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/read_endpoint.py` & `laceworksdk-2.1.0/laceworksdk/api/read_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/search_endpoint.py` & `laceworksdk-2.1.0/laceworksdk/api/search_endpoint.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/activities.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/activities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/agent_access_tokens.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/agent_access_tokens.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/alert_channels.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/alert_channels.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/alert_profiles.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/alert_profiles.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/alert_rules.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/alert_rules.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/alerts.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/alerts.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/audit_logs.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/audit_logs.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/cloud_accounts.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/cloud_accounts.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/cloud_activities.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/cloud_activities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/configs.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/configs.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/container_registries.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/container_registries.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/contract_info.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/contract_info.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/datasources.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/datasources.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/entities.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/entities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/events.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/events.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/inventory.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/inventory.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/organization_info.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/organization_info.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/policies.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/policies.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/policy_exceptions.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/policy_exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/queries.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/queries.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/report_definitions.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/report_definitions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/report_rules.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/report_rules.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/reports.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/reports.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/resource_groups.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/resource_groups.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/schemas.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/team_members.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/team_members.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/team_users.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/team_users.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/user_groups.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/user_groups.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/user_profile.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerabilities.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_exceptions.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/vulnerability_exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/api/v2/vulnerability_policies.py` & `laceworksdk-2.1.0/laceworksdk/api/v2/vulnerability_policies.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/config.py` & `laceworksdk-2.1.0/laceworksdk/config.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/exceptions.py` & `laceworksdk-2.1.0/laceworksdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/laceworksdk/http_session.py` & `laceworksdk-2.1.0/laceworksdk/http_session.py`

 * *Files identical despite different names*

### Comparing `laceworksdk-2.0.0/pyproject.toml` & `laceworksdk-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laceworksdk"
-version = "2.0.0"
+version = "2.1.0"
 description = "Community-developed Python SDK for the Lacework APIs"
 authors = ["Jon Stewart <jon.stewart@lacework.net>"]
 maintainers = ["Jon Stewart <jon.stewart@lacework.net>", "Matthew Cadorette <matthew.cadorette@lacework.net>"]
 readme = "README.md"
 packages = [{include = "laceworksdk"}]
 license = "MIT"
 homepage = "https://github.com/lacework/python-sdk"
@@ -12,30 +12,28 @@
 keywords = ["lacework", "api", "sdk", "python"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.16"
-python-dotenv = "^0.20.0"
-requests = "^2.27.1"
-configparser = "^5.2.0"
-bleach = "^4.1.0"
-urllib3 = "^1.26.15"
-importlib-metadata = "4.2"
+python = ">=3.8,<4"
+python-dotenv = ">=0.20.0"
+requests = ">=2.27.1"
+configparser = ">=5.2.0"
+bleach = ">=4.1.0"
+urllib3 = ">=1.26.15"
+importlib-metadata = ">=4.2"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^1.7"
 flake8 = "^5.0.4"
 flake8-quotes = "^3.3"
 pytest = "^7.2.2"
 pytest-lazy-fixture = "^0.6.3"
```

### Comparing `laceworksdk-2.0.0/PKG-INFO` & `laceworksdk-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: laceworksdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: Community-developed Python SDK for the Lacework APIs
 Home-page: https://github.com/lacework/python-sdk
 License: MIT
 Keywords: lacework,api,sdk,python
 Author: Jon Stewart
 Author-email: jon.stewart@lacework.net
 Maintainer: Jon Stewart
 Maintainer-email: jon.stewart@lacework.net
-Requires-Python: >=3.7.16,<4.0.0
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Dist: bleach (>=4.1.0,<5.0.0)
-Requires-Dist: configparser (>=5.2.0,<6.0.0)
-Requires-Dist: importlib-metadata (==4.2)
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Requires-Dist: bleach (>=4.1.0)
+Requires-Dist: configparser (>=5.2.0)
+Requires-Dist: importlib-metadata (>=4.2)
+Requires-Dist: python-dotenv (>=0.20.0)
+Requires-Dist: requests (>=2.27.1)
+Requires-Dist: urllib3 (>=1.26.15)
 Project-URL: Repository, https://github.com/lacework/python-sdk
 Description-Content-Type: text/markdown
 
 <img src="https://techally-content.s3-us-west-1.amazonaws.com/public-content/lacework_logo_full.png" width="600">
 
 # Lacework Python SDK
 
@@ -81,15 +79,15 @@
         }
     ]
 })
 ```
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.8 or higher
 - Lacework API Credentials
   - Account Name
   - API Key
   - API Secret
 
 ## How-To
```

