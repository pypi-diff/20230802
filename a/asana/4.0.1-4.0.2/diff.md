# Comparing `tmp/asana-4.0.1.tar.gz` & `tmp/asana-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-epf3bxnu/asana-4.0.1.tar", last modified: Mon Jul 31 23:50:44 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-zjkduhpk/asana-4.0.2.tar", last modified: Wed Aug  2 20:51:35 2023, max compression
```

## Comparing `asana-4.0.1.tar` & `asana-4.0.2.tar`

### file list

```diff
@@ -1,917 +1,941 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-31 23:50:33.000000 asana-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-31 23:50:44.000000 asana-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    61965 2023-07-31 23:50:33.000000 asana-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/asana/
--rw-r--r--   0 runner    (1001) docker     (123)    32590 2023-07-31 23:50:33.000000 asana-4.0.1/asana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/asana/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28584 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52939 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    63742 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   106576 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   163533 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api/workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-07-31 23:50:33.000000 asana-4.0.1/asana/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-07-31 23:50:33.000000 asana-4.0.1/asana/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/asana/models/
--rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/inline_response412.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/inline_response412_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/like.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    31095 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    44565 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/teams_team_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-31 23:50:33.000000 asana-4.0.1/asana/models/workspaces_workspace_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-31 23:50:33.000000 asana-4.0.1/asana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 23:50:44.000000 asana-4.0.1/asana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:50:44.000000 asana-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-31 23:50:33.000000 asana-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:50:44.000000 asana-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 23:50:33.000000 asana-4.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_inline_response412.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_inline_response412_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_teams_team_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:50:33.000000 asana-4.0.1/test/test_workspaces_workspace_gid_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 20:51:25.000000 asana-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    62600 2023-08-02 20:51:35.000000 asana-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    62371 2023-08-02 20:51:25.000000 asana-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/asana/
+-rw-r--r--   0 runner    (1001) docker     (123)    33076 2023-08-02 20:51:25.000000 asana-4.0.2/asana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/asana/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45545 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28584 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52939 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63742 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106576 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163533 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-08-02 20:51:25.000000 asana-4.0.2/asana/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-08-02 20:51:25.000000 asana-4.0.2/asana/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/asana/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_membership_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_compact_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_compact_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_compact_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19771 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_compact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_normal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_normal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25790 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32570 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24102 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44565 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-02 20:51:25.000000 asana-4.0.2/asana/models/workspaces_workspace_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-08-02 20:51:25.000000 asana-4.0.2/asana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    62600 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36288 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 20:51:35.000000 asana-4.0.2/asana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:51:35.000000 asana-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-02 20:51:25.000000 asana-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:35.000000 asana-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 20:51:25.000000 asana-4.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_membership_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_compact_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_compact_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_compact_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_compact_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_normal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_normal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:51:25.000000 asana-4.0.2/test/test_workspaces_workspace_gid_body.py
```

### Comparing `asana-4.0.1/LICENSE` & `asana-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/PKG-INFO` & `asana-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: asana
-Version: 4.0.1
+Version: 4.0.2
 Summary: Asana
 Home-page: http://github.com/asana/python-asana
 Author: Asana, Inc
 License: MIT
 Keywords: asana,Asana
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.1
+- Package version: 4.0.2
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -493,17 +493,18 @@
  - [GoalGidAddFollowersBody](docs/GoalGidAddFollowersBody.md)
  - [GoalGidAddSupportingRelationshipBody](docs/GoalGidAddSupportingRelationshipBody.md)
  - [GoalGidRemoveFollowersBody](docs/GoalGidRemoveFollowersBody.md)
  - [GoalGidRemoveSupportingRelationshipBody](docs/GoalGidRemoveSupportingRelationshipBody.md)
  - [GoalGidSetMetricBody](docs/GoalGidSetMetricBody.md)
  - [GoalGidSetMetricCurrentValueBody](docs/GoalGidSetMetricCurrentValueBody.md)
  - [GoalMembershipBase](docs/GoalMembershipBase.md)
- - [GoalMembershipBaseGoal](docs/GoalMembershipBaseGoal.md)
  - [GoalMembershipCompact](docs/GoalMembershipCompact.md)
  - [GoalMembershipResponse](docs/GoalMembershipResponse.md)
+ - [GoalMembershipResponseUser](docs/GoalMembershipResponseUser.md)
+ - [GoalMembershipResponseWorkspace](docs/GoalMembershipResponseWorkspace.md)
  - [GoalMetricBase](docs/GoalMetricBase.md)
  - [GoalMetricCurrentValueRequest](docs/GoalMetricCurrentValueRequest.md)
  - [GoalMetricRequest](docs/GoalMetricRequest.md)
  - [GoalRelationshipBase](docs/GoalRelationshipBase.md)
  - [GoalRelationshipBaseSupportedGoal](docs/GoalRelationshipBaseSupportedGoal.md)
  - [GoalRelationshipBaseSupportingResource](docs/GoalRelationshipBaseSupportingResource.md)
  - [GoalRelationshipCompact](docs/GoalRelationshipCompact.md)
@@ -535,14 +536,18 @@
  - [JobBaseNewProjectTemplate](docs/JobBaseNewProjectTemplate.md)
  - [JobBaseNewTask](docs/JobBaseNewTask.md)
  - [JobCompact](docs/JobCompact.md)
  - [JobResponse](docs/JobResponse.md)
  - [JobResponseData](docs/JobResponseData.md)
  - [Like](docs/Like.md)
  - [MemberCompact](docs/MemberCompact.md)
+ - [MembershipCompact](docs/MembershipCompact.md)
+ - [MembershipCompactGoal](docs/MembershipCompactGoal.md)
+ - [MembershipCompactMember](docs/MembershipCompactMember.md)
+ - [MembershipCompactParent](docs/MembershipCompactParent.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [MembershipResponse](docs/MembershipResponse.md)
  - [MembershipResponseArray](docs/MembershipResponseArray.md)
  - [MembershipResponseData](docs/MembershipResponseData.md)
  - [MembershipsBody](docs/MembershipsBody.md)
  - [ModifyDependenciesRequest](docs/ModifyDependenciesRequest.md)
  - [ModifyDependentsRequest](docs/ModifyDependentsRequest.md)
@@ -579,15 +584,14 @@
  - [PortfolioResponseWorkspace](docs/PortfolioResponseWorkspace.md)
  - [PortfoliosBody](docs/PortfoliosBody.md)
  - [PortfoliosPortfolioGidBody](docs/PortfoliosPortfolioGidBody.md)
  - [Preview](docs/Preview.md)
  - [ProjectBase](docs/ProjectBase.md)
  - [ProjectBaseCurrentStatus](docs/ProjectBaseCurrentStatus.md)
  - [ProjectBaseCurrentStatusUpdate](docs/ProjectBaseCurrentStatusUpdate.md)
- - [ProjectBaseWorkspace](docs/ProjectBaseWorkspace.md)
  - [ProjectBriefBase](docs/ProjectBriefBase.md)
  - [ProjectBriefCompact](docs/ProjectBriefCompact.md)
  - [ProjectBriefRequest](docs/ProjectBriefRequest.md)
  - [ProjectBriefResponse](docs/ProjectBriefResponse.md)
  - [ProjectBriefResponseData](docs/ProjectBriefResponseData.md)
  - [ProjectBriefResponseProject](docs/ProjectBriefResponseProject.md)
  - [ProjectBriefsProjectBriefGidBody](docs/ProjectBriefsProjectBriefGidBody.md)
@@ -603,26 +607,27 @@
  - [ProjectGidRemoveCustomFieldSettingBody](docs/ProjectGidRemoveCustomFieldSettingBody.md)
  - [ProjectGidRemoveFollowersBody](docs/ProjectGidRemoveFollowersBody.md)
  - [ProjectGidRemoveMembersBody](docs/ProjectGidRemoveMembersBody.md)
  - [ProjectGidSaveAsTemplateBody](docs/ProjectGidSaveAsTemplateBody.md)
  - [ProjectGidSectionsBody](docs/ProjectGidSectionsBody.md)
  - [ProjectMembershipBase](docs/ProjectMembershipBase.md)
  - [ProjectMembershipCompact](docs/ProjectMembershipCompact.md)
- - [ProjectMembershipResponse](docs/ProjectMembershipResponse.md)
- - [ProjectMembershipResponseArray](docs/ProjectMembershipResponseArray.md)
- - [ProjectMembershipResponseData](docs/ProjectMembershipResponseData.md)
- - [ProjectMembershipResponseMember](docs/ProjectMembershipResponseMember.md)
+ - [ProjectMembershipCompactArray](docs/ProjectMembershipCompactArray.md)
+ - [ProjectMembershipCompactResponse](docs/ProjectMembershipCompactResponse.md)
+ - [ProjectMembershipNormalResponse](docs/ProjectMembershipNormalResponse.md)
+ - [ProjectMembershipNormalResponseData](docs/ProjectMembershipNormalResponseData.md)
  - [ProjectRequest](docs/ProjectRequest.md)
  - [ProjectResponse](docs/ProjectResponse.md)
  - [ProjectResponseArray](docs/ProjectResponseArray.md)
  - [ProjectResponseCompletedBy](docs/ProjectResponseCompletedBy.md)
  - [ProjectResponseCreatedFromTemplate](docs/ProjectResponseCreatedFromTemplate.md)
  - [ProjectResponseData](docs/ProjectResponseData.md)
  - [ProjectResponseProjectBrief](docs/ProjectResponseProjectBrief.md)
  - [ProjectResponseTeam](docs/ProjectResponseTeam.md)
+ - [ProjectResponseWorkspace](docs/ProjectResponseWorkspace.md)
  - [ProjectSaveAsTemplateRequest](docs/ProjectSaveAsTemplateRequest.md)
  - [ProjectSectionInsertRequest](docs/ProjectSectionInsertRequest.md)
  - [ProjectStatusBase](docs/ProjectStatusBase.md)
  - [ProjectStatusCompact](docs/ProjectStatusCompact.md)
  - [ProjectStatusRequest](docs/ProjectStatusRequest.md)
  - [ProjectStatusResponse](docs/ProjectStatusResponse.md)
  - [ProjectStatusResponseArray](docs/ProjectStatusResponseArray.md)
@@ -635,14 +640,15 @@
  - [ProjectTemplateGidInstantiateProjectBody](docs/ProjectTemplateGidInstantiateProjectBody.md)
  - [ProjectTemplateInstantiateProjectRequest](docs/ProjectTemplateInstantiateProjectRequest.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedDates](docs/ProjectTemplateInstantiateProjectRequestRequestedDates.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedRoles](docs/ProjectTemplateInstantiateProjectRequestRequestedRoles.md)
  - [ProjectTemplateResponse](docs/ProjectTemplateResponse.md)
  - [ProjectTemplateResponseArray](docs/ProjectTemplateResponseArray.md)
  - [ProjectTemplateResponseData](docs/ProjectTemplateResponseData.md)
+ - [ProjectUpdateRequest](docs/ProjectUpdateRequest.md)
  - [ProjectsBody](docs/ProjectsBody.md)
  - [ProjectsProjectGidBody](docs/ProjectsProjectGidBody.md)
  - [RemoveCustomFieldSettingRequest](docs/RemoveCustomFieldSettingRequest.md)
  - [RemoveFollowersRequest](docs/RemoveFollowersRequest.md)
  - [RemoveMembersRequest](docs/RemoveMembersRequest.md)
  - [RequestedRoleRequest](docs/RequestedRoleRequest.md)
  - [RuleTriggerGidRunBody](docs/RuleTriggerGidRunBody.md)
```

### Comparing `asana-4.0.1/README.md` & `asana-4.0.2/asana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+Metadata-Version: 2.1
+Name: asana
+Version: 4.0.2
+Summary: Asana
+Home-page: http://github.com/asana/python-asana
+Author: Asana, Inc
+License: MIT
+Keywords: asana,Asana
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.1
+- Package version: 4.0.2
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -482,17 +493,18 @@
  - [GoalGidAddFollowersBody](docs/GoalGidAddFollowersBody.md)
  - [GoalGidAddSupportingRelationshipBody](docs/GoalGidAddSupportingRelationshipBody.md)
  - [GoalGidRemoveFollowersBody](docs/GoalGidRemoveFollowersBody.md)
  - [GoalGidRemoveSupportingRelationshipBody](docs/GoalGidRemoveSupportingRelationshipBody.md)
  - [GoalGidSetMetricBody](docs/GoalGidSetMetricBody.md)
  - [GoalGidSetMetricCurrentValueBody](docs/GoalGidSetMetricCurrentValueBody.md)
  - [GoalMembershipBase](docs/GoalMembershipBase.md)
- - [GoalMembershipBaseGoal](docs/GoalMembershipBaseGoal.md)
  - [GoalMembershipCompact](docs/GoalMembershipCompact.md)
  - [GoalMembershipResponse](docs/GoalMembershipResponse.md)
+ - [GoalMembershipResponseUser](docs/GoalMembershipResponseUser.md)
+ - [GoalMembershipResponseWorkspace](docs/GoalMembershipResponseWorkspace.md)
  - [GoalMetricBase](docs/GoalMetricBase.md)
  - [GoalMetricCurrentValueRequest](docs/GoalMetricCurrentValueRequest.md)
  - [GoalMetricRequest](docs/GoalMetricRequest.md)
  - [GoalRelationshipBase](docs/GoalRelationshipBase.md)
  - [GoalRelationshipBaseSupportedGoal](docs/GoalRelationshipBaseSupportedGoal.md)
  - [GoalRelationshipBaseSupportingResource](docs/GoalRelationshipBaseSupportingResource.md)
  - [GoalRelationshipCompact](docs/GoalRelationshipCompact.md)
@@ -524,14 +536,18 @@
  - [JobBaseNewProjectTemplate](docs/JobBaseNewProjectTemplate.md)
  - [JobBaseNewTask](docs/JobBaseNewTask.md)
  - [JobCompact](docs/JobCompact.md)
  - [JobResponse](docs/JobResponse.md)
  - [JobResponseData](docs/JobResponseData.md)
  - [Like](docs/Like.md)
  - [MemberCompact](docs/MemberCompact.md)
+ - [MembershipCompact](docs/MembershipCompact.md)
+ - [MembershipCompactGoal](docs/MembershipCompactGoal.md)
+ - [MembershipCompactMember](docs/MembershipCompactMember.md)
+ - [MembershipCompactParent](docs/MembershipCompactParent.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [MembershipResponse](docs/MembershipResponse.md)
  - [MembershipResponseArray](docs/MembershipResponseArray.md)
  - [MembershipResponseData](docs/MembershipResponseData.md)
  - [MembershipsBody](docs/MembershipsBody.md)
  - [ModifyDependenciesRequest](docs/ModifyDependenciesRequest.md)
  - [ModifyDependentsRequest](docs/ModifyDependentsRequest.md)
@@ -568,15 +584,14 @@
  - [PortfolioResponseWorkspace](docs/PortfolioResponseWorkspace.md)
  - [PortfoliosBody](docs/PortfoliosBody.md)
  - [PortfoliosPortfolioGidBody](docs/PortfoliosPortfolioGidBody.md)
  - [Preview](docs/Preview.md)
  - [ProjectBase](docs/ProjectBase.md)
  - [ProjectBaseCurrentStatus](docs/ProjectBaseCurrentStatus.md)
  - [ProjectBaseCurrentStatusUpdate](docs/ProjectBaseCurrentStatusUpdate.md)
- - [ProjectBaseWorkspace](docs/ProjectBaseWorkspace.md)
  - [ProjectBriefBase](docs/ProjectBriefBase.md)
  - [ProjectBriefCompact](docs/ProjectBriefCompact.md)
  - [ProjectBriefRequest](docs/ProjectBriefRequest.md)
  - [ProjectBriefResponse](docs/ProjectBriefResponse.md)
  - [ProjectBriefResponseData](docs/ProjectBriefResponseData.md)
  - [ProjectBriefResponseProject](docs/ProjectBriefResponseProject.md)
  - [ProjectBriefsProjectBriefGidBody](docs/ProjectBriefsProjectBriefGidBody.md)
@@ -592,26 +607,27 @@
  - [ProjectGidRemoveCustomFieldSettingBody](docs/ProjectGidRemoveCustomFieldSettingBody.md)
  - [ProjectGidRemoveFollowersBody](docs/ProjectGidRemoveFollowersBody.md)
  - [ProjectGidRemoveMembersBody](docs/ProjectGidRemoveMembersBody.md)
  - [ProjectGidSaveAsTemplateBody](docs/ProjectGidSaveAsTemplateBody.md)
  - [ProjectGidSectionsBody](docs/ProjectGidSectionsBody.md)
  - [ProjectMembershipBase](docs/ProjectMembershipBase.md)
  - [ProjectMembershipCompact](docs/ProjectMembershipCompact.md)
- - [ProjectMembershipResponse](docs/ProjectMembershipResponse.md)
- - [ProjectMembershipResponseArray](docs/ProjectMembershipResponseArray.md)
- - [ProjectMembershipResponseData](docs/ProjectMembershipResponseData.md)
- - [ProjectMembershipResponseMember](docs/ProjectMembershipResponseMember.md)
+ - [ProjectMembershipCompactArray](docs/ProjectMembershipCompactArray.md)
+ - [ProjectMembershipCompactResponse](docs/ProjectMembershipCompactResponse.md)
+ - [ProjectMembershipNormalResponse](docs/ProjectMembershipNormalResponse.md)
+ - [ProjectMembershipNormalResponseData](docs/ProjectMembershipNormalResponseData.md)
  - [ProjectRequest](docs/ProjectRequest.md)
  - [ProjectResponse](docs/ProjectResponse.md)
  - [ProjectResponseArray](docs/ProjectResponseArray.md)
  - [ProjectResponseCompletedBy](docs/ProjectResponseCompletedBy.md)
  - [ProjectResponseCreatedFromTemplate](docs/ProjectResponseCreatedFromTemplate.md)
  - [ProjectResponseData](docs/ProjectResponseData.md)
  - [ProjectResponseProjectBrief](docs/ProjectResponseProjectBrief.md)
  - [ProjectResponseTeam](docs/ProjectResponseTeam.md)
+ - [ProjectResponseWorkspace](docs/ProjectResponseWorkspace.md)
  - [ProjectSaveAsTemplateRequest](docs/ProjectSaveAsTemplateRequest.md)
  - [ProjectSectionInsertRequest](docs/ProjectSectionInsertRequest.md)
  - [ProjectStatusBase](docs/ProjectStatusBase.md)
  - [ProjectStatusCompact](docs/ProjectStatusCompact.md)
  - [ProjectStatusRequest](docs/ProjectStatusRequest.md)
  - [ProjectStatusResponse](docs/ProjectStatusResponse.md)
  - [ProjectStatusResponseArray](docs/ProjectStatusResponseArray.md)
@@ -624,14 +640,15 @@
  - [ProjectTemplateGidInstantiateProjectBody](docs/ProjectTemplateGidInstantiateProjectBody.md)
  - [ProjectTemplateInstantiateProjectRequest](docs/ProjectTemplateInstantiateProjectRequest.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedDates](docs/ProjectTemplateInstantiateProjectRequestRequestedDates.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedRoles](docs/ProjectTemplateInstantiateProjectRequestRequestedRoles.md)
  - [ProjectTemplateResponse](docs/ProjectTemplateResponse.md)
  - [ProjectTemplateResponseArray](docs/ProjectTemplateResponseArray.md)
  - [ProjectTemplateResponseData](docs/ProjectTemplateResponseData.md)
+ - [ProjectUpdateRequest](docs/ProjectUpdateRequest.md)
  - [ProjectsBody](docs/ProjectsBody.md)
  - [ProjectsProjectGidBody](docs/ProjectsProjectGidBody.md)
  - [RemoveCustomFieldSettingRequest](docs/RemoveCustomFieldSettingRequest.md)
  - [RemoveFollowersRequest](docs/RemoveFollowersRequest.md)
  - [RemoveMembersRequest](docs/RemoveMembersRequest.md)
  - [RequestedRoleRequest](docs/RequestedRoleRequest.md)
  - [RuleTriggerGidRunBody](docs/RuleTriggerGidRunBody.md)
```

### Comparing `asana-4.0.1/asana/__init__.py` & `asana-4.0.2/asana/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,18 @@
 from asana.models.goal_gid_add_followers_body import GoalGidAddFollowersBody
 from asana.models.goal_gid_add_supporting_relationship_body import GoalGidAddSupportingRelationshipBody
 from asana.models.goal_gid_remove_followers_body import GoalGidRemoveFollowersBody
 from asana.models.goal_gid_remove_supporting_relationship_body import GoalGidRemoveSupportingRelationshipBody
 from asana.models.goal_gid_set_metric_body import GoalGidSetMetricBody
 from asana.models.goal_gid_set_metric_current_value_body import GoalGidSetMetricCurrentValueBody
 from asana.models.goal_membership_base import GoalMembershipBase
-from asana.models.goal_membership_base_goal import GoalMembershipBaseGoal
 from asana.models.goal_membership_compact import GoalMembershipCompact
 from asana.models.goal_membership_response import GoalMembershipResponse
+from asana.models.goal_membership_response_user import GoalMembershipResponseUser
+from asana.models.goal_membership_response_workspace import GoalMembershipResponseWorkspace
 from asana.models.goal_metric_base import GoalMetricBase
 from asana.models.goal_metric_current_value_request import GoalMetricCurrentValueRequest
 from asana.models.goal_metric_request import GoalMetricRequest
 from asana.models.goal_relationship_base import GoalRelationshipBase
 from asana.models.goal_relationship_base_supported_goal import GoalRelationshipBaseSupportedGoal
 from asana.models.goal_relationship_base_supporting_resource import GoalRelationshipBaseSupportingResource
 from asana.models.goal_relationship_compact import GoalRelationshipCompact
@@ -188,14 +189,18 @@
 from asana.models.job_base_new_project_template import JobBaseNewProjectTemplate
 from asana.models.job_base_new_task import JobBaseNewTask
 from asana.models.job_compact import JobCompact
 from asana.models.job_response import JobResponse
 from asana.models.job_response_data import JobResponseData
 from asana.models.like import Like
 from asana.models.member_compact import MemberCompact
+from asana.models.membership_compact import MembershipCompact
+from asana.models.membership_compact_goal import MembershipCompactGoal
+from asana.models.membership_compact_member import MembershipCompactMember
+from asana.models.membership_compact_parent import MembershipCompactParent
 from asana.models.membership_request import MembershipRequest
 from asana.models.membership_response import MembershipResponse
 from asana.models.membership_response_array import MembershipResponseArray
 from asana.models.membership_response_data import MembershipResponseData
 from asana.models.memberships_body import MembershipsBody
 from asana.models.modify_dependencies_request import ModifyDependenciesRequest
 from asana.models.modify_dependents_request import ModifyDependentsRequest
@@ -232,15 +237,14 @@
 from asana.models.portfolio_response_workspace import PortfolioResponseWorkspace
 from asana.models.portfolios_body import PortfoliosBody
 from asana.models.portfolios_portfolio_gid_body import PortfoliosPortfolioGidBody
 from asana.models.preview import Preview
 from asana.models.project_base import ProjectBase
 from asana.models.project_base_current_status import ProjectBaseCurrentStatus
 from asana.models.project_base_current_status_update import ProjectBaseCurrentStatusUpdate
-from asana.models.project_base_workspace import ProjectBaseWorkspace
 from asana.models.project_brief_base import ProjectBriefBase
 from asana.models.project_brief_compact import ProjectBriefCompact
 from asana.models.project_brief_request import ProjectBriefRequest
 from asana.models.project_brief_response import ProjectBriefResponse
 from asana.models.project_brief_response_data import ProjectBriefResponseData
 from asana.models.project_brief_response_project import ProjectBriefResponseProject
 from asana.models.project_briefs_project_brief_gid_body import ProjectBriefsProjectBriefGidBody
@@ -256,26 +260,27 @@
 from asana.models.project_gid_remove_custom_field_setting_body import ProjectGidRemoveCustomFieldSettingBody
 from asana.models.project_gid_remove_followers_body import ProjectGidRemoveFollowersBody
 from asana.models.project_gid_remove_members_body import ProjectGidRemoveMembersBody
 from asana.models.project_gid_save_as_template_body import ProjectGidSaveAsTemplateBody
 from asana.models.project_gid_sections_body import ProjectGidSectionsBody
 from asana.models.project_membership_base import ProjectMembershipBase
 from asana.models.project_membership_compact import ProjectMembershipCompact
-from asana.models.project_membership_response import ProjectMembershipResponse
-from asana.models.project_membership_response_array import ProjectMembershipResponseArray
-from asana.models.project_membership_response_data import ProjectMembershipResponseData
-from asana.models.project_membership_response_member import ProjectMembershipResponseMember
+from asana.models.project_membership_compact_array import ProjectMembershipCompactArray
+from asana.models.project_membership_compact_response import ProjectMembershipCompactResponse
+from asana.models.project_membership_normal_response import ProjectMembershipNormalResponse
+from asana.models.project_membership_normal_response_data import ProjectMembershipNormalResponseData
 from asana.models.project_request import ProjectRequest
 from asana.models.project_response import ProjectResponse
 from asana.models.project_response_array import ProjectResponseArray
 from asana.models.project_response_completed_by import ProjectResponseCompletedBy
 from asana.models.project_response_created_from_template import ProjectResponseCreatedFromTemplate
 from asana.models.project_response_data import ProjectResponseData
 from asana.models.project_response_project_brief import ProjectResponseProjectBrief
 from asana.models.project_response_team import ProjectResponseTeam
+from asana.models.project_response_workspace import ProjectResponseWorkspace
 from asana.models.project_save_as_template_request import ProjectSaveAsTemplateRequest
 from asana.models.project_section_insert_request import ProjectSectionInsertRequest
 from asana.models.project_status_base import ProjectStatusBase
 from asana.models.project_status_compact import ProjectStatusCompact
 from asana.models.project_status_request import ProjectStatusRequest
 from asana.models.project_status_response import ProjectStatusResponse
 from asana.models.project_status_response_array import ProjectStatusResponseArray
@@ -288,14 +293,15 @@
 from asana.models.project_template_gid_instantiate_project_body import ProjectTemplateGidInstantiateProjectBody
 from asana.models.project_template_instantiate_project_request import ProjectTemplateInstantiateProjectRequest
 from asana.models.project_template_instantiate_project_request_requested_dates import ProjectTemplateInstantiateProjectRequestRequestedDates
 from asana.models.project_template_instantiate_project_request_requested_roles import ProjectTemplateInstantiateProjectRequestRequestedRoles
 from asana.models.project_template_response import ProjectTemplateResponse
 from asana.models.project_template_response_array import ProjectTemplateResponseArray
 from asana.models.project_template_response_data import ProjectTemplateResponseData
+from asana.models.project_update_request import ProjectUpdateRequest
 from asana.models.projects_body import ProjectsBody
 from asana.models.projects_project_gid_body import ProjectsProjectGidBody
 from asana.models.remove_custom_field_setting_request import RemoveCustomFieldSettingRequest
 from asana.models.remove_followers_request import RemoveFollowersRequest
 from asana.models.remove_members_request import RemoveMembersRequest
 from asana.models.requested_role_request import RequestedRoleRequest
 from asana.models.rule_trigger_gid_run_body import RuleTriggerGidRunBody
```

### Comparing `asana-4.0.1/asana/api/__init__.py` & `asana-4.0.2/asana/api/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/attachments_api.py` & `asana-4.0.2/asana/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/audit_log_api_api.py` & `asana-4.0.2/asana/api/audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/batch_api_api.py` & `asana-4.0.2/asana/api/batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/custom_field_settings_api.py` & `asana-4.0.2/asana/api/custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/custom_fields_api.py` & `asana-4.0.2/asana/api/custom_fields_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,48 +28,48 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_custom_field(self, **kwargs):  # noqa: E501
+    def create_custom_field(self, body, **kwargs):  # noqa: E501
         """Create a custom field  # noqa: E501
 
         Creates a new custom field in a workspace. Every custom field is required to be created in a specific workspace, and this workspace cannot be changed once set.  A custom field’s name must be unique within a workspace and not conflict with names of existing task properties such as `Due Date` or `Assignee`. A custom field’s type must be one of `text`, `enum`, `multi_enum`, `number`, `date`, or `people`.  Returns the full record of the newly created custom field.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_custom_field(async_req=True)
+        >>> thread = api.create_custom_field(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CustomFieldsBody body: The custom field object to create.
+        :param CustomFieldsBody body: The custom field object to create. (required)
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
         :return: CustomFieldResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.create_custom_field_with_http_info(**kwargs)  # noqa: E501
+            return self.create_custom_field_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.create_custom_field_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.create_custom_field_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def create_custom_field_with_http_info(self, **kwargs):  # noqa: E501
+    def create_custom_field_with_http_info(self, body, **kwargs):  # noqa: E501
         """Create a custom field  # noqa: E501
 
         Creates a new custom field in a workspace. Every custom field is required to be created in a specific workspace, and this workspace cannot be changed once set.  A custom field’s name must be unique within a workspace and not conflict with names of existing task properties such as `Due Date` or `Assignee`. A custom field’s type must be one of `text`, `enum`, `multi_enum`, `number`, `date`, or `people`.  Returns the full record of the newly created custom field.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_custom_field_with_http_info(async_req=True)
+        >>> thread = api.create_custom_field_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CustomFieldsBody body: The custom field object to create.
+        :param CustomFieldsBody body: The custom field object to create. (required)
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
         :return: CustomFieldResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'opt_fields']  # noqa: E501
@@ -83,14 +83,18 @@
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create_custom_field" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `create_custom_field`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'opt_fields' in params:
```

### Comparing `asana-4.0.1/asana/api/events_api.py` & `asana-4.0.2/asana/api/events_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/goal_relationships_api.py` & `asana-4.0.2/asana/api/goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/goals_api.py` & `asana-4.0.2/asana/api/goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/jobs_api.py` & `asana-4.0.2/asana/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/memberships_api.py` & `asana-4.0.2/asana/api/memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/organization_exports_api.py` & `asana-4.0.2/asana/api/organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/portfolio_memberships_api.py` & `asana-4.0.2/asana/api/portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/portfolios_api.py` & `asana-4.0.2/asana/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/project_briefs_api.py` & `asana-4.0.2/asana/api/project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/project_memberships_api.py` & `asana-4.0.2/asana/api/project_memberships_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_project_membership(project_membership_gid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_membership_gid: (required)
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
-        :return: ProjectMembershipResponseData
+        :return: ProjectMembershipNormalResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_project_membership_with_http_info(project_membership_gid, **kwargs)  # noqa: E501
         else:
@@ -63,15 +63,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_project_membership_with_http_info(project_membership_gid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_membership_gid: (required)
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
-        :return: ProjectMembershipResponseData
+        :return: ProjectMembershipNormalResponseData
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['project_membership_gid', 'opt_fields']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -120,15 +120,15 @@
             '/project_memberships/{project_membership_gid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ProjectMembershipResponseData',  # noqa: E501
+            response_type='ProjectMembershipNormalResponseData',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -143,15 +143,15 @@
 
         :param async_req bool
         :param str project_gid: Globally unique identifier for the project. (required)
         :param str user: A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.
         :param int limit: Results per page. The number of objects to return per page. The value must be between 1 and 100.
         :param str offset: Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
-        :return: ProjectMembershipResponseArray
+        :return: ProjectMembershipCompactArray
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_project_memberships_for_project_with_http_info(project_gid, **kwargs)  # noqa: E501
         else:
@@ -169,15 +169,15 @@
 
         :param async_req bool
         :param str project_gid: Globally unique identifier for the project. (required)
         :param str user: A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.
         :param int limit: Results per page. The number of objects to return per page. The value must be between 1 and 100.
         :param str offset: Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'
         :param list[str] opt_fields: This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.
-        :return: ProjectMembershipResponseArray
+        :return: ProjectMembershipCompactArray
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['project_gid', 'user', 'limit', 'offset', 'opt_fields']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -232,14 +232,14 @@
             '/projects/{project_gid}/project_memberships', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ProjectMembershipResponseArray',  # noqa: E501
+            response_type='ProjectMembershipCompactArray',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `asana-4.0.1/asana/api/project_statuses_api.py` & `asana-4.0.2/asana/api/project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/project_templates_api.py` & `asana-4.0.2/asana/api/project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/projects_api.py` & `asana-4.0.2/asana/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/rules_api.py` & `asana-4.0.2/asana/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/sections_api.py` & `asana-4.0.2/asana/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/status_updates_api.py` & `asana-4.0.2/asana/api/status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/stories_api.py` & `asana-4.0.2/asana/api/stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/tags_api.py` & `asana-4.0.2/asana/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/tasks_api.py` & `asana-4.0.2/asana/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/team_memberships_api.py` & `asana-4.0.2/asana/api/team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/teams_api.py` & `asana-4.0.2/asana/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/time_periods_api.py` & `asana-4.0.2/asana/api/time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/time_tracking_entries_api.py` & `asana-4.0.2/asana/api/time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/typeahead_api.py` & `asana-4.0.2/asana/api/typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/user_task_lists_api.py` & `asana-4.0.2/asana/api/user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/users_api.py` & `asana-4.0.2/asana/api/users_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/webhooks_api.py` & `asana-4.0.2/asana/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/workspace_memberships_api.py` & `asana-4.0.2/asana/api/workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api/workspaces_api.py` & `asana-4.0.2/asana/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/api_client.py` & `asana-4.0.2/asana/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/4.0.1/python'
+        self.user_agent = 'Swagger-Codegen/4.0.2/python'
         # Add custom header
         self.default_headers['X-Asana-Client-Lib'] = urlencode(
             {
                 'language': 'Python',
-                'version': '4.0.1',
+                'version': '4.0.2',
                 'language_version': platform.python_version(),
                 'os': platform.system(),
                 'os_version': platform.release()
             }
         )
 
     def __del__(self):
```

### Comparing `asana-4.0.1/asana/configuration.py` & `asana-4.0.2/asana/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,9 +245,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 4.0.1".\
+               "SDK Package Version: 4.0.2".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asana-4.0.1/asana/models/__init__.py` & `asana-4.0.2/asana/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,18 @@
 from asana.models.goal_gid_add_followers_body import GoalGidAddFollowersBody
 from asana.models.goal_gid_add_supporting_relationship_body import GoalGidAddSupportingRelationshipBody
 from asana.models.goal_gid_remove_followers_body import GoalGidRemoveFollowersBody
 from asana.models.goal_gid_remove_supporting_relationship_body import GoalGidRemoveSupportingRelationshipBody
 from asana.models.goal_gid_set_metric_body import GoalGidSetMetricBody
 from asana.models.goal_gid_set_metric_current_value_body import GoalGidSetMetricCurrentValueBody
 from asana.models.goal_membership_base import GoalMembershipBase
-from asana.models.goal_membership_base_goal import GoalMembershipBaseGoal
 from asana.models.goal_membership_compact import GoalMembershipCompact
 from asana.models.goal_membership_response import GoalMembershipResponse
+from asana.models.goal_membership_response_user import GoalMembershipResponseUser
+from asana.models.goal_membership_response_workspace import GoalMembershipResponseWorkspace
 from asana.models.goal_metric_base import GoalMetricBase
 from asana.models.goal_metric_current_value_request import GoalMetricCurrentValueRequest
 from asana.models.goal_metric_request import GoalMetricRequest
 from asana.models.goal_relationship_base import GoalRelationshipBase
 from asana.models.goal_relationship_base_supported_goal import GoalRelationshipBaseSupportedGoal
 from asana.models.goal_relationship_base_supporting_resource import GoalRelationshipBaseSupportingResource
 from asana.models.goal_relationship_compact import GoalRelationshipCompact
@@ -149,14 +150,18 @@
 from asana.models.job_base_new_project_template import JobBaseNewProjectTemplate
 from asana.models.job_base_new_task import JobBaseNewTask
 from asana.models.job_compact import JobCompact
 from asana.models.job_response import JobResponse
 from asana.models.job_response_data import JobResponseData
 from asana.models.like import Like
 from asana.models.member_compact import MemberCompact
+from asana.models.membership_compact import MembershipCompact
+from asana.models.membership_compact_goal import MembershipCompactGoal
+from asana.models.membership_compact_member import MembershipCompactMember
+from asana.models.membership_compact_parent import MembershipCompactParent
 from asana.models.membership_request import MembershipRequest
 from asana.models.membership_response import MembershipResponse
 from asana.models.membership_response_array import MembershipResponseArray
 from asana.models.membership_response_data import MembershipResponseData
 from asana.models.memberships_body import MembershipsBody
 from asana.models.modify_dependencies_request import ModifyDependenciesRequest
 from asana.models.modify_dependents_request import ModifyDependentsRequest
@@ -193,15 +198,14 @@
 from asana.models.portfolio_response_workspace import PortfolioResponseWorkspace
 from asana.models.portfolios_body import PortfoliosBody
 from asana.models.portfolios_portfolio_gid_body import PortfoliosPortfolioGidBody
 from asana.models.preview import Preview
 from asana.models.project_base import ProjectBase
 from asana.models.project_base_current_status import ProjectBaseCurrentStatus
 from asana.models.project_base_current_status_update import ProjectBaseCurrentStatusUpdate
-from asana.models.project_base_workspace import ProjectBaseWorkspace
 from asana.models.project_brief_base import ProjectBriefBase
 from asana.models.project_brief_compact import ProjectBriefCompact
 from asana.models.project_brief_request import ProjectBriefRequest
 from asana.models.project_brief_response import ProjectBriefResponse
 from asana.models.project_brief_response_data import ProjectBriefResponseData
 from asana.models.project_brief_response_project import ProjectBriefResponseProject
 from asana.models.project_briefs_project_brief_gid_body import ProjectBriefsProjectBriefGidBody
@@ -217,26 +221,27 @@
 from asana.models.project_gid_remove_custom_field_setting_body import ProjectGidRemoveCustomFieldSettingBody
 from asana.models.project_gid_remove_followers_body import ProjectGidRemoveFollowersBody
 from asana.models.project_gid_remove_members_body import ProjectGidRemoveMembersBody
 from asana.models.project_gid_save_as_template_body import ProjectGidSaveAsTemplateBody
 from asana.models.project_gid_sections_body import ProjectGidSectionsBody
 from asana.models.project_membership_base import ProjectMembershipBase
 from asana.models.project_membership_compact import ProjectMembershipCompact
-from asana.models.project_membership_response import ProjectMembershipResponse
-from asana.models.project_membership_response_array import ProjectMembershipResponseArray
-from asana.models.project_membership_response_data import ProjectMembershipResponseData
-from asana.models.project_membership_response_member import ProjectMembershipResponseMember
+from asana.models.project_membership_compact_array import ProjectMembershipCompactArray
+from asana.models.project_membership_compact_response import ProjectMembershipCompactResponse
+from asana.models.project_membership_normal_response import ProjectMembershipNormalResponse
+from asana.models.project_membership_normal_response_data import ProjectMembershipNormalResponseData
 from asana.models.project_request import ProjectRequest
 from asana.models.project_response import ProjectResponse
 from asana.models.project_response_array import ProjectResponseArray
 from asana.models.project_response_completed_by import ProjectResponseCompletedBy
 from asana.models.project_response_created_from_template import ProjectResponseCreatedFromTemplate
 from asana.models.project_response_data import ProjectResponseData
 from asana.models.project_response_project_brief import ProjectResponseProjectBrief
 from asana.models.project_response_team import ProjectResponseTeam
+from asana.models.project_response_workspace import ProjectResponseWorkspace
 from asana.models.project_save_as_template_request import ProjectSaveAsTemplateRequest
 from asana.models.project_section_insert_request import ProjectSectionInsertRequest
 from asana.models.project_status_base import ProjectStatusBase
 from asana.models.project_status_compact import ProjectStatusCompact
 from asana.models.project_status_request import ProjectStatusRequest
 from asana.models.project_status_response import ProjectStatusResponse
 from asana.models.project_status_response_array import ProjectStatusResponseArray
@@ -249,14 +254,15 @@
 from asana.models.project_template_gid_instantiate_project_body import ProjectTemplateGidInstantiateProjectBody
 from asana.models.project_template_instantiate_project_request import ProjectTemplateInstantiateProjectRequest
 from asana.models.project_template_instantiate_project_request_requested_dates import ProjectTemplateInstantiateProjectRequestRequestedDates
 from asana.models.project_template_instantiate_project_request_requested_roles import ProjectTemplateInstantiateProjectRequestRequestedRoles
 from asana.models.project_template_response import ProjectTemplateResponse
 from asana.models.project_template_response_array import ProjectTemplateResponseArray
 from asana.models.project_template_response_data import ProjectTemplateResponseData
+from asana.models.project_update_request import ProjectUpdateRequest
 from asana.models.projects_body import ProjectsBody
 from asana.models.projects_project_gid_body import ProjectsProjectGidBody
 from asana.models.remove_custom_field_setting_request import RemoveCustomFieldSettingRequest
 from asana.models.remove_followers_request import RemoveFollowersRequest
 from asana.models.remove_members_request import RemoveMembersRequest
 from asana.models.requested_role_request import RequestedRoleRequest
 from asana.models.rule_trigger_gid_run_body import RuleTriggerGidRunBody
```

### Comparing `asana-4.0.1/asana/models/add_custom_field_setting_request.py` & `asana-4.0.2/asana/models/add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/add_followers_request.py` & `asana-4.0.2/asana/models/add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/add_members_request.py` & `asana-4.0.2/asana/models/add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_project_response_owner.py` & `asana-4.0.2/asana/models/all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_project_template_base_owner.py` & `asana-4.0.2/asana/models/all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_project_template_response_owner.py` & `asana-4.0.2/asana/models/all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_story_response_new_date_value.py` & `asana-4.0.2/asana/models/all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_story_response_old_date_value.py` & `asana-4.0.2/asana/models/all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_base_owner.py` & `asana-4.0.2/asana/models/all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_base_workspace.py` & `asana-4.0.2/asana/models/all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_compact_owner.py` & `asana-4.0.2/asana/models/all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_compact_workspace.py` & `asana-4.0.2/asana/models/all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_request_owner.py` & `asana-4.0.2/asana/models/all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_request_workspace.py` & `asana-4.0.2/asana/models/all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_response_owner.py` & `asana-4.0.2/asana/models/all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_user_task_list_response_workspace.py` & `asana-4.0.2/asana/models/all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_workspace_membership_response_user_task_list_owner.py` & `asana-4.0.2/asana/models/all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py` & `asana-4.0.2/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/asana_named_resource.py` & `asana-4.0.2/asana/models/asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/asana_named_resource_array.py` & `asana-4.0.2/asana/models/asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/asana_resource.py` & `asana-4.0.2/asana/models/asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_base.py` & `asana-4.0.2/asana/models/attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_compact.py` & `asana-4.0.2/asana/models/attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_request.py` & `asana-4.0.2/asana/models/attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_response.py` & `asana-4.0.2/asana/models/attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_response_array.py` & `asana-4.0.2/asana/models/attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_response_data.py` & `asana-4.0.2/asana/models/attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/attachment_response_parent.py` & `asana-4.0.2/asana/models/attachment_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event.py` & `asana-4.0.2/asana/models/audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event_actor.py` & `asana-4.0.2/asana/models/audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event_array.py` & `asana-4.0.2/asana/models/audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event_context.py` & `asana-4.0.2/asana/models/audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event_details.py` & `asana-4.0.2/asana/models/audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/audit_log_event_resource.py` & `asana-4.0.2/asana/models/audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_body.py` & `asana-4.0.2/asana/models/batch_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_request.py` & `asana-4.0.2/asana/models/batch_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_request_action.py` & `asana-4.0.2/asana/models/batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_request_actions.py` & `asana-4.0.2/asana/models/batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_request_options.py` & `asana-4.0.2/asana/models/batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_response.py` & `asana-4.0.2/asana/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/batch_response_array.py` & `asana-4.0.2/asana/models/batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/create_membership_request.py` & `asana-4.0.2/asana/models/create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/create_time_tracking_entry_request.py` & `asana-4.0.2/asana/models/create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_base.py` & `asana-4.0.2/asana/models/custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_base_date_value.py` & `asana-4.0.2/asana/models/custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_base_enum_options.py` & `asana-4.0.2/asana/models/custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_base_enum_value.py` & `asana-4.0.2/asana/models/custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_compact.py` & `asana-4.0.2/asana/models/custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_gid_enum_options_body.py` & `asana-4.0.2/asana/models/custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_request.py` & `asana-4.0.2/asana/models/custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_response.py` & `asana-4.0.2/asana/models/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_response_array.py` & `asana-4.0.2/asana/models/custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_response_created_by.py` & `asana-4.0.2/asana/models/custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_response_data.py` & `asana-4.0.2/asana/models/custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_response_people_value.py` & `asana-4.0.2/asana/models/custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_base.py` & `asana-4.0.2/asana/models/custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_compact.py` & `asana-4.0.2/asana/models/custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response.py` & `asana-4.0.2/asana/models/custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response_array.py` & `asana-4.0.2/asana/models/custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response_custom_field.py` & `asana-4.0.2/asana/models/custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response_data.py` & `asana-4.0.2/asana/models/custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response_parent.py` & `asana-4.0.2/asana/models/custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_field_setting_response_project.py` & `asana-4.0.2/asana/models/custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_fields_body.py` & `asana-4.0.2/asana/models/custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/custom_fields_custom_field_gid_body.py` & `asana-4.0.2/asana/models/custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/date_variable_compact.py` & `asana-4.0.2/asana/models/date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/date_variable_request.py` & `asana-4.0.2/asana/models/date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/empty_response.py` & `asana-4.0.2/asana/models/empty_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/empty_response_data.py` & `asana-4.0.2/asana/models/empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_option.py` & `asana-4.0.2/asana/models/enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_option_base.py` & `asana-4.0.2/asana/models/enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_option_data.py` & `asana-4.0.2/asana/models/enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_option_insert_request.py` & `asana-4.0.2/asana/models/enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_option_request.py` & `asana-4.0.2/asana/models/enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_options_enum_option_gid_body.py` & `asana-4.0.2/asana/models/enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/enum_options_insert_body.py` & `asana-4.0.2/asana/models/enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/error.py` & `asana-4.0.2/asana/models/error.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/error_response.py` & `asana-4.0.2/asana/models/error_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/error_response_errors.py` & `asana-4.0.2/asana/models/error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response.py` & `asana-4.0.2/asana/models/event_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response_array.py` & `asana-4.0.2/asana/models/event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response_change.py` & `asana-4.0.2/asana/models/event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response_parent.py` & `asana-4.0.2/asana/models/event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response_resource.py` & `asana-4.0.2/asana/models/event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/event_response_user.py` & `asana-4.0.2/asana/models/event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_add_subgoal_request.py` & `asana-4.0.2/asana/models/goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_add_supporting_relationship_request.py` & `asana-4.0.2/asana/models/goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_add_supporting_work_request.py` & `asana-4.0.2/asana/models/goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_base.py` & `asana-4.0.2/asana/models/goal_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_compact.py` & `asana-4.0.2/asana/models/goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_add_followers_body.py` & `asana-4.0.2/asana/models/goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_add_supporting_relationship_body.py` & `asana-4.0.2/asana/models/goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_remove_followers_body.py` & `asana-4.0.2/asana/models/goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_remove_supporting_relationship_body.py` & `asana-4.0.2/asana/models/goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_set_metric_body.py` & `asana-4.0.2/asana/models/goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_gid_set_metric_current_value_body.py` & `asana-4.0.2/asana/models/goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_membership_base.py` & `asana-4.0.2/asana/models/goal_membership_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,50 +26,55 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
-        'member': 'ProjectMembershipResponseMember',
-        'goal': 'GoalMembershipBaseGoal',
-        'is_commenter': 'bool',
-        'is_editor': 'bool'
+        'resource_subtype': 'str',
+        'member': 'MembershipCompactMember',
+        'parent': 'MembershipCompactParent',
+        'role': 'str',
+        'goal': 'MembershipCompactGoal'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
+        'resource_subtype': 'resource_subtype',
         'member': 'member',
-        'goal': 'goal',
-        'is_commenter': 'is_commenter',
-        'is_editor': 'is_editor'
+        'parent': 'parent',
+        'role': 'role',
+        'goal': 'goal'
     }
 
-    def __init__(self, gid=None, resource_type=None, member=None, goal=None, is_commenter=None, is_editor=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, resource_subtype=None, member=None, parent=None, role=None, goal=None):  # noqa: E501
         """GoalMembershipBase - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
+        self._resource_subtype = None
         self._member = None
+        self._parent = None
+        self._role = None
         self._goal = None
-        self._is_commenter = None
-        self._is_editor = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
+        if resource_subtype is not None:
+            self.resource_subtype = resource_subtype
         if member is not None:
             self.member = member
+        if parent is not None:
+            self.parent = parent
+        if role is not None:
+            self.role = role
         if goal is not None:
             self.goal = goal
-        if is_commenter is not None:
-            self.is_commenter = is_commenter
-        if is_editor is not None:
-            self.is_editor = is_editor
 
     @property
     def gid(self):
         """Gets the gid of this GoalMembershipBase.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -110,100 +115,127 @@
         :param resource_type: The resource_type of this GoalMembershipBase.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
+    def resource_subtype(self):
+        """Gets the resource_subtype of this GoalMembershipBase.  # noqa: E501
+
+        The type of membership.  # noqa: E501
+
+        :return: The resource_subtype of this GoalMembershipBase.  # noqa: E501
+        :rtype: str
+        """
+        return self._resource_subtype
+
+    @resource_subtype.setter
+    def resource_subtype(self, resource_subtype):
+        """Sets the resource_subtype of this GoalMembershipBase.
+
+        The type of membership.  # noqa: E501
+
+        :param resource_subtype: The resource_subtype of this GoalMembershipBase.  # noqa: E501
+        :type: str
+        """
+
+        self._resource_subtype = resource_subtype
+
+    @property
     def member(self):
         """Gets the member of this GoalMembershipBase.  # noqa: E501
 
 
         :return: The member of this GoalMembershipBase.  # noqa: E501
-        :rtype: ProjectMembershipResponseMember
+        :rtype: MembershipCompactMember
         """
         return self._member
 
     @member.setter
     def member(self, member):
         """Sets the member of this GoalMembershipBase.
 
 
         :param member: The member of this GoalMembershipBase.  # noqa: E501
-        :type: ProjectMembershipResponseMember
+        :type: MembershipCompactMember
         """
 
         self._member = member
 
     @property
-    def goal(self):
-        """Gets the goal of this GoalMembershipBase.  # noqa: E501
+    def parent(self):
+        """Gets the parent of this GoalMembershipBase.  # noqa: E501
 
 
-        :return: The goal of this GoalMembershipBase.  # noqa: E501
-        :rtype: GoalMembershipBaseGoal
+        :return: The parent of this GoalMembershipBase.  # noqa: E501
+        :rtype: MembershipCompactParent
         """
-        return self._goal
+        return self._parent
 
-    @goal.setter
-    def goal(self, goal):
-        """Sets the goal of this GoalMembershipBase.
+    @parent.setter
+    def parent(self, parent):
+        """Sets the parent of this GoalMembershipBase.
 
 
-        :param goal: The goal of this GoalMembershipBase.  # noqa: E501
-        :type: GoalMembershipBaseGoal
+        :param parent: The parent of this GoalMembershipBase.  # noqa: E501
+        :type: MembershipCompactParent
         """
 
-        self._goal = goal
+        self._parent = parent
 
     @property
-    def is_commenter(self):
-        """Gets the is_commenter of this GoalMembershipBase.  # noqa: E501
+    def role(self):
+        """Gets the role of this GoalMembershipBase.  # noqa: E501
 
-        Describes if the member is comment only in goal.  # noqa: E501
+        Describes if the member is a commenter or editor in goal.  # noqa: E501
 
-        :return: The is_commenter of this GoalMembershipBase.  # noqa: E501
-        :rtype: bool
+        :return: The role of this GoalMembershipBase.  # noqa: E501
+        :rtype: str
         """
-        return self._is_commenter
+        return self._role
 
-    @is_commenter.setter
-    def is_commenter(self, is_commenter):
-        """Sets the is_commenter of this GoalMembershipBase.
+    @role.setter
+    def role(self, role):
+        """Sets the role of this GoalMembershipBase.
 
-        Describes if the member is comment only in goal.  # noqa: E501
+        Describes if the member is a commenter or editor in goal.  # noqa: E501
 
-        :param is_commenter: The is_commenter of this GoalMembershipBase.  # noqa: E501
-        :type: bool
+        :param role: The role of this GoalMembershipBase.  # noqa: E501
+        :type: str
         """
+        allowed_values = ["commenter", "editor"]  # noqa: E501
+        if role not in allowed_values:
+            raise ValueError(
+                "Invalid value for `role` ({0}), must be one of {1}"  # noqa: E501
+                .format(role, allowed_values)
+            )
 
-        self._is_commenter = is_commenter
+        self._role = role
 
     @property
-    def is_editor(self):
-        """Gets the is_editor of this GoalMembershipBase.  # noqa: E501
+    def goal(self):
+        """Gets the goal of this GoalMembershipBase.  # noqa: E501
 
-        Describes if the member is editor in goal.  # noqa: E501
 
-        :return: The is_editor of this GoalMembershipBase.  # noqa: E501
-        :rtype: bool
+        :return: The goal of this GoalMembershipBase.  # noqa: E501
+        :rtype: MembershipCompactGoal
         """
-        return self._is_editor
+        return self._goal
 
-    @is_editor.setter
-    def is_editor(self, is_editor):
-        """Sets the is_editor of this GoalMembershipBase.
+    @goal.setter
+    def goal(self, goal):
+        """Sets the goal of this GoalMembershipBase.
 
-        Describes if the member is editor in goal.  # noqa: E501
 
-        :param is_editor: The is_editor of this GoalMembershipBase.  # noqa: E501
-        :type: bool
+        :param goal: The goal of this GoalMembershipBase.  # noqa: E501
+        :type: MembershipCompactGoal
         """
 
-        self._is_editor = is_editor
+        self._goal = goal
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
```

### Comparing `asana-4.0.1/asana/models/goal_membership_base_goal.py` & `asana-4.0.2/asana/models/goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_membership_compact.py` & `asana-4.0.2/asana/models/goal_membership_compact.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,44 +26,59 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
-        'member': 'ProjectMembershipResponseMember',
-        'goal': 'GoalMembershipBaseGoal',
+        'resource_subtype': 'str',
+        'member': 'MembershipCompactMember',
+        'parent': 'MembershipCompactParent',
+        'role': 'str',
+        'goal': 'MembershipCompactGoal',
         'is_commenter': 'bool',
         'is_editor': 'bool'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
+        'resource_subtype': 'resource_subtype',
         'member': 'member',
+        'parent': 'parent',
+        'role': 'role',
         'goal': 'goal',
         'is_commenter': 'is_commenter',
         'is_editor': 'is_editor'
     }
 
-    def __init__(self, gid=None, resource_type=None, member=None, goal=None, is_commenter=None, is_editor=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, resource_subtype=None, member=None, parent=None, role=None, goal=None, is_commenter=None, is_editor=None):  # noqa: E501
         """GoalMembershipCompact - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
+        self._resource_subtype = None
         self._member = None
+        self._parent = None
+        self._role = None
         self._goal = None
         self._is_commenter = None
         self._is_editor = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
+        if resource_subtype is not None:
+            self.resource_subtype = resource_subtype
         if member is not None:
             self.member = member
+        if parent is not None:
+            self.parent = parent
+        if role is not None:
+            self.role = role
         if goal is not None:
             self.goal = goal
         if is_commenter is not None:
             self.is_commenter = is_commenter
         if is_editor is not None:
             self.is_editor = is_editor
 
@@ -110,94 +125,167 @@
         :param resource_type: The resource_type of this GoalMembershipCompact.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
+    def resource_subtype(self):
+        """Gets the resource_subtype of this GoalMembershipCompact.  # noqa: E501
+
+        The type of membership.  # noqa: E501
+
+        :return: The resource_subtype of this GoalMembershipCompact.  # noqa: E501
+        :rtype: str
+        """
+        return self._resource_subtype
+
+    @resource_subtype.setter
+    def resource_subtype(self, resource_subtype):
+        """Sets the resource_subtype of this GoalMembershipCompact.
+
+        The type of membership.  # noqa: E501
+
+        :param resource_subtype: The resource_subtype of this GoalMembershipCompact.  # noqa: E501
+        :type: str
+        """
+
+        self._resource_subtype = resource_subtype
+
+    @property
     def member(self):
         """Gets the member of this GoalMembershipCompact.  # noqa: E501
 
 
         :return: The member of this GoalMembershipCompact.  # noqa: E501
-        :rtype: ProjectMembershipResponseMember
+        :rtype: MembershipCompactMember
         """
         return self._member
 
     @member.setter
     def member(self, member):
         """Sets the member of this GoalMembershipCompact.
 
 
         :param member: The member of this GoalMembershipCompact.  # noqa: E501
-        :type: ProjectMembershipResponseMember
+        :type: MembershipCompactMember
         """
 
         self._member = member
 
     @property
+    def parent(self):
+        """Gets the parent of this GoalMembershipCompact.  # noqa: E501
+
+
+        :return: The parent of this GoalMembershipCompact.  # noqa: E501
+        :rtype: MembershipCompactParent
+        """
+        return self._parent
+
+    @parent.setter
+    def parent(self, parent):
+        """Sets the parent of this GoalMembershipCompact.
+
+
+        :param parent: The parent of this GoalMembershipCompact.  # noqa: E501
+        :type: MembershipCompactParent
+        """
+
+        self._parent = parent
+
+    @property
+    def role(self):
+        """Gets the role of this GoalMembershipCompact.  # noqa: E501
+
+        Describes if the member is a commenter or editor in goal.  # noqa: E501
+
+        :return: The role of this GoalMembershipCompact.  # noqa: E501
+        :rtype: str
+        """
+        return self._role
+
+    @role.setter
+    def role(self, role):
+        """Sets the role of this GoalMembershipCompact.
+
+        Describes if the member is a commenter or editor in goal.  # noqa: E501
+
+        :param role: The role of this GoalMembershipCompact.  # noqa: E501
+        :type: str
+        """
+        allowed_values = ["commenter", "editor"]  # noqa: E501
+        if role not in allowed_values:
+            raise ValueError(
+                "Invalid value for `role` ({0}), must be one of {1}"  # noqa: E501
+                .format(role, allowed_values)
+            )
+
+        self._role = role
+
+    @property
     def goal(self):
         """Gets the goal of this GoalMembershipCompact.  # noqa: E501
 
 
         :return: The goal of this GoalMembershipCompact.  # noqa: E501
-        :rtype: GoalMembershipBaseGoal
+        :rtype: MembershipCompactGoal
         """
         return self._goal
 
     @goal.setter
     def goal(self, goal):
         """Sets the goal of this GoalMembershipCompact.
 
 
         :param goal: The goal of this GoalMembershipCompact.  # noqa: E501
-        :type: GoalMembershipBaseGoal
+        :type: MembershipCompactGoal
         """
 
         self._goal = goal
 
     @property
     def is_commenter(self):
         """Gets the is_commenter of this GoalMembershipCompact.  # noqa: E501
 
-        Describes if the member is comment only in goal.  # noqa: E501
+        *Deprecated: new integrations should prefer the `role` field.* Describes if the member is comment only in goal.  # noqa: E501
 
         :return: The is_commenter of this GoalMembershipCompact.  # noqa: E501
         :rtype: bool
         """
         return self._is_commenter
 
     @is_commenter.setter
     def is_commenter(self, is_commenter):
         """Sets the is_commenter of this GoalMembershipCompact.
 
-        Describes if the member is comment only in goal.  # noqa: E501
+        *Deprecated: new integrations should prefer the `role` field.* Describes if the member is comment only in goal.  # noqa: E501
 
         :param is_commenter: The is_commenter of this GoalMembershipCompact.  # noqa: E501
         :type: bool
         """
 
         self._is_commenter = is_commenter
 
     @property
     def is_editor(self):
         """Gets the is_editor of this GoalMembershipCompact.  # noqa: E501
 
-        Describes if the member is editor in goal.  # noqa: E501
+        *Deprecated: new integrations should prefer the `role` field.* Describes if the member is editor in goal.  # noqa: E501
 
         :return: The is_editor of this GoalMembershipCompact.  # noqa: E501
         :rtype: bool
         """
         return self._is_editor
 
     @is_editor.setter
     def is_editor(self, is_editor):
         """Sets the is_editor of this GoalMembershipCompact.
 
-        Describes if the member is editor in goal.  # noqa: E501
+        *Deprecated: new integrations should prefer the `role` field.* Describes if the member is editor in goal.  # noqa: E501
 
         :param is_editor: The is_editor of this GoalMembershipCompact.  # noqa: E501
         :type: bool
         """
 
         self._is_editor = is_editor
```

### Comparing `asana-4.0.1/asana/models/goal_membership_response.py` & `asana-4.0.2/asana/models/user_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,199 +11,201 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GoalMembershipResponse(object):
+class UserResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
-        'member': 'ProjectMembershipResponseMember',
-        'goal': 'GoalMembershipBaseGoal',
-        'is_commenter': 'bool',
-        'is_editor': 'bool'
+        'name': 'str',
+        'email': 'str',
+        'photo': 'UserBaseResponsePhoto',
+        'workspaces': 'list[GoalResponseWorkspace]'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
-        'member': 'member',
-        'goal': 'goal',
-        'is_commenter': 'is_commenter',
-        'is_editor': 'is_editor'
+        'name': 'name',
+        'email': 'email',
+        'photo': 'photo',
+        'workspaces': 'workspaces'
     }
 
-    def __init__(self, gid=None, resource_type=None, member=None, goal=None, is_commenter=None, is_editor=None):  # noqa: E501
-        """GoalMembershipResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, email=None, photo=None, workspaces=None):  # noqa: E501
+        """UserResponse - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
-        self._member = None
-        self._goal = None
-        self._is_commenter = None
-        self._is_editor = None
+        self._name = None
+        self._email = None
+        self._photo = None
+        self._workspaces = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
-        if member is not None:
-            self.member = member
-        if goal is not None:
-            self.goal = goal
-        if is_commenter is not None:
-            self.is_commenter = is_commenter
-        if is_editor is not None:
-            self.is_editor = is_editor
+        if name is not None:
+            self.name = name
+        if email is not None:
+            self.email = email
+        if photo is not None:
+            self.photo = photo
+        if workspaces is not None:
+            self.workspaces = workspaces
 
     @property
     def gid(self):
-        """Gets the gid of this GoalMembershipResponse.  # noqa: E501
+        """Gets the gid of this UserResponse.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this GoalMembershipResponse.  # noqa: E501
+        :return: The gid of this UserResponse.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this GoalMembershipResponse.
+        """Sets the gid of this UserResponse.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this GoalMembershipResponse.  # noqa: E501
+        :param gid: The gid of this UserResponse.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this GoalMembershipResponse.  # noqa: E501
+        """Gets the resource_type of this UserResponse.  # noqa: E501
 
         The base type of this resource.  # noqa: E501
 
-        :return: The resource_type of this GoalMembershipResponse.  # noqa: E501
+        :return: The resource_type of this UserResponse.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this GoalMembershipResponse.
+        """Sets the resource_type of this UserResponse.
 
         The base type of this resource.  # noqa: E501
 
-        :param resource_type: The resource_type of this GoalMembershipResponse.  # noqa: E501
+        :param resource_type: The resource_type of this UserResponse.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
-    def member(self):
-        """Gets the member of this GoalMembershipResponse.  # noqa: E501
+    def name(self):
+        """Gets the name of this UserResponse.  # noqa: E501
 
+        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
 
-        :return: The member of this GoalMembershipResponse.  # noqa: E501
-        :rtype: ProjectMembershipResponseMember
+        :return: The name of this UserResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._member
+        return self._name
 
-    @member.setter
-    def member(self, member):
-        """Sets the member of this GoalMembershipResponse.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this UserResponse.
 
+        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
 
-        :param member: The member of this GoalMembershipResponse.  # noqa: E501
-        :type: ProjectMembershipResponseMember
+        :param name: The name of this UserResponse.  # noqa: E501
+        :type: str
         """
 
-        self._member = member
+        self._name = name
 
     @property
-    def goal(self):
-        """Gets the goal of this GoalMembershipResponse.  # noqa: E501
+    def email(self):
+        """Gets the email of this UserResponse.  # noqa: E501
 
+        The user's email address.  # noqa: E501
 
-        :return: The goal of this GoalMembershipResponse.  # noqa: E501
-        :rtype: GoalMembershipBaseGoal
+        :return: The email of this UserResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._goal
+        return self._email
 
-    @goal.setter
-    def goal(self, goal):
-        """Sets the goal of this GoalMembershipResponse.
+    @email.setter
+    def email(self, email):
+        """Sets the email of this UserResponse.
 
+        The user's email address.  # noqa: E501
 
-        :param goal: The goal of this GoalMembershipResponse.  # noqa: E501
-        :type: GoalMembershipBaseGoal
+        :param email: The email of this UserResponse.  # noqa: E501
+        :type: str
         """
 
-        self._goal = goal
+        self._email = email
 
     @property
-    def is_commenter(self):
-        """Gets the is_commenter of this GoalMembershipResponse.  # noqa: E501
+    def photo(self):
+        """Gets the photo of this UserResponse.  # noqa: E501
 
-        Describes if the member is comment only in goal.  # noqa: E501
 
-        :return: The is_commenter of this GoalMembershipResponse.  # noqa: E501
-        :rtype: bool
+        :return: The photo of this UserResponse.  # noqa: E501
+        :rtype: UserBaseResponsePhoto
         """
-        return self._is_commenter
+        return self._photo
 
-    @is_commenter.setter
-    def is_commenter(self, is_commenter):
-        """Sets the is_commenter of this GoalMembershipResponse.
+    @photo.setter
+    def photo(self, photo):
+        """Sets the photo of this UserResponse.
 
-        Describes if the member is comment only in goal.  # noqa: E501
 
-        :param is_commenter: The is_commenter of this GoalMembershipResponse.  # noqa: E501
-        :type: bool
+        :param photo: The photo of this UserResponse.  # noqa: E501
+        :type: UserBaseResponsePhoto
         """
 
-        self._is_commenter = is_commenter
+        self._photo = photo
 
     @property
-    def is_editor(self):
-        """Gets the is_editor of this GoalMembershipResponse.  # noqa: E501
+    def workspaces(self):
+        """Gets the workspaces of this UserResponse.  # noqa: E501
 
-        Describes if the member is editor in goal.  # noqa: E501
+        Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.  # noqa: E501
 
-        :return: The is_editor of this GoalMembershipResponse.  # noqa: E501
-        :rtype: bool
+        :return: The workspaces of this UserResponse.  # noqa: E501
+        :rtype: list[GoalResponseWorkspace]
         """
-        return self._is_editor
+        return self._workspaces
 
-    @is_editor.setter
-    def is_editor(self, is_editor):
-        """Sets the is_editor of this GoalMembershipResponse.
+    @workspaces.setter
+    def workspaces(self, workspaces):
+        """Sets the workspaces of this UserResponse.
 
-        Describes if the member is editor in goal.  # noqa: E501
+        Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.  # noqa: E501
 
-        :param is_editor: The is_editor of this GoalMembershipResponse.  # noqa: E501
-        :type: bool
+        :param workspaces: The workspaces of this UserResponse.  # noqa: E501
+        :type: list[GoalResponseWorkspace]
         """
 
-        self._is_editor = is_editor
+        self._workspaces = workspaces
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -218,15 +220,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GoalMembershipResponse, dict):
+        if issubclass(UserResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -234,15 +236,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GoalMembershipResponse):
+        if not isinstance(other, UserResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-4.0.1/asana/models/goal_metric_base.py` & `asana-4.0.2/asana/models/goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_metric_current_value_request.py` & `asana-4.0.2/asana/models/goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_metric_request.py` & `asana-4.0.2/asana/models/goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_base.py` & `asana-4.0.2/asana/models/goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_base_supported_goal.py` & `asana-4.0.2/asana/models/goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_base_supporting_resource.py` & `asana-4.0.2/asana/models/goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_compact.py` & `asana-4.0.2/asana/models/goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_request.py` & `asana-4.0.2/asana/models/goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_response.py` & `asana-4.0.2/asana/models/goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_response_array.py` & `asana-4.0.2/asana/models/goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationship_response_data.py` & `asana-4.0.2/asana/models/goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_relationships_goal_relationship_gid_body.py` & `asana-4.0.2/asana/models/goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_remove_subgoal_request.py` & `asana-4.0.2/asana/models/goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_remove_supporting_relationship_request.py` & `asana-4.0.2/asana/models/goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_request.py` & `asana-4.0.2/asana/models/goal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_request_base.py` & `asana-4.0.2/asana/models/goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response.py` & `asana-4.0.2/asana/models/goal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_array.py` & `asana-4.0.2/asana/models/goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_current_status_update.py` & `asana-4.0.2/asana/models/goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_data.py` & `asana-4.0.2/asana/models/goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_likes.py` & `asana-4.0.2/asana/models/goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_metric.py` & `asana-4.0.2/asana/models/goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_team.py` & `asana-4.0.2/asana/models/goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_time_period.py` & `asana-4.0.2/asana/models/goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_response_workspace.py` & `asana-4.0.2/asana/models/goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goal_update_request.py` & `asana-4.0.2/asana/models/goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goals_body.py` & `asana-4.0.2/asana/models/goals_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/goals_goal_gid_body.py` & `asana-4.0.2/asana/models/goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/inline_response412.py` & `asana-4.0.2/asana/models/inline_response412.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/inline_response412_errors.py` & `asana-4.0.2/asana/models/inline_response412_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_base.py` & `asana-4.0.2/asana/models/job_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_base_new_project.py` & `asana-4.0.2/asana/models/job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_base_new_project_template.py` & `asana-4.0.2/asana/models/job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_base_new_task.py` & `asana-4.0.2/asana/models/job_base_new_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_compact.py` & `asana-4.0.2/asana/models/job_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_response.py` & `asana-4.0.2/asana/models/job_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/job_response_data.py` & `asana-4.0.2/asana/models/job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/like.py` & `asana-4.0.2/asana/models/like.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/member_compact.py` & `asana-4.0.2/asana/models/member_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/membership_request.py` & `asana-4.0.2/asana/models/membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/membership_response.py` & `asana-4.0.2/asana/models/membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/membership_response_array.py` & `asana-4.0.2/asana/models/membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/membership_response_data.py` & `asana-4.0.2/asana/models/membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/memberships_body.py` & `asana-4.0.2/asana/models/memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/modify_dependencies_request.py` & `asana-4.0.2/asana/models/modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/modify_dependents_request.py` & `asana-4.0.2/asana/models/modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/next_page.py` & `asana-4.0.2/asana/models/next_page.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_export_base.py` & `asana-4.0.2/asana/models/organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_export_compact.py` & `asana-4.0.2/asana/models/organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_export_request.py` & `asana-4.0.2/asana/models/organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_export_response.py` & `asana-4.0.2/asana/models/organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_export_response_data.py` & `asana-4.0.2/asana/models/organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/organization_exports_body.py` & `asana-4.0.2/asana/models/organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_add_item_request.py` & `asana-4.0.2/asana/models/portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_base.py` & `asana-4.0.2/asana/models/portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_compact.py` & `asana-4.0.2/asana/models/portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_add_custom_field_setting_body.py` & `asana-4.0.2/asana/models/portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_add_item_body.py` & `asana-4.0.2/asana/models/portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_add_members_body.py` & `asana-4.0.2/asana/models/portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_remove_custom_field_setting_body.py` & `asana-4.0.2/asana/models/portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_remove_item_body.py` & `asana-4.0.2/asana/models/portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_gid_remove_members_body.py` & `asana-4.0.2/asana/models/portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_base.py` & `asana-4.0.2/asana/models/portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_base_portfolio.py` & `asana-4.0.2/asana/models/portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_compact.py` & `asana-4.0.2/asana/models/portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_response.py` & `asana-4.0.2/asana/models/portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_response_array.py` & `asana-4.0.2/asana/models/portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_membership_response_data.py` & `asana-4.0.2/asana/models/portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_remove_item_request.py` & `asana-4.0.2/asana/models/portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_request.py` & `asana-4.0.2/asana/models/portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response.py` & `asana-4.0.2/asana/models/portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_array.py` & `asana-4.0.2/asana/models/portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_current_status_update.py` & `asana-4.0.2/asana/models/portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_custom_field_settings.py` & `asana-4.0.2/asana/models/portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_custom_fields.py` & `asana-4.0.2/asana/models/portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_data.py` & `asana-4.0.2/asana/models/portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolio_response_workspace.py` & `asana-4.0.2/asana/models/portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolios_body.py` & `asana-4.0.2/asana/models/portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/portfolios_portfolio_gid_body.py` & `asana-4.0.2/asana/models/portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/preview.py` & `asana-4.0.2/asana/models/preview.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_base.py` & `asana-4.0.2/asana/models/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         'due_date': 'date',
         'due_on': 'date',
         'html_notes': 'str',
         'members': 'list[CustomFieldResponsePeopleValue]',
         'modified_at': 'datetime',
         'notes': 'str',
         'public': 'bool',
-        'start_on': 'date',
-        'workspace': 'ProjectBaseWorkspace'
+        'start_on': 'date'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
         'archived': 'archived',
@@ -63,19 +62,18 @@
         'due_date': 'due_date',
         'due_on': 'due_on',
         'html_notes': 'html_notes',
         'members': 'members',
         'modified_at': 'modified_at',
         'notes': 'notes',
         'public': 'public',
-        'start_on': 'start_on',
-        'workspace': 'workspace'
+        'start_on': 'start_on'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None, workspace=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None):  # noqa: E501
         """ProjectBase - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._archived = None
         self._color = None
         self._created_at = None
@@ -87,15 +85,14 @@
         self._due_on = None
         self._html_notes = None
         self._members = None
         self._modified_at = None
         self._notes = None
         self._public = None
         self._start_on = None
-        self._workspace = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
@@ -125,16 +122,14 @@
             self.modified_at = modified_at
         if notes is not None:
             self.notes = notes
         if public is not None:
             self.public = public
         if start_on is not None:
             self.start_on = start_on
-        if workspace is not None:
-            self.workspace = workspace
 
     @property
     def gid(self):
         """Gets the gid of this ProjectBase.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -550,35 +545,14 @@
 
         :param start_on: The start_on of this ProjectBase.  # noqa: E501
         :type: date
         """
 
         self._start_on = start_on
 
-    @property
-    def workspace(self):
-        """Gets the workspace of this ProjectBase.  # noqa: E501
-
-
-        :return: The workspace of this ProjectBase.  # noqa: E501
-        :rtype: ProjectBaseWorkspace
-        """
-        return self._workspace
-
-    @workspace.setter
-    def workspace(self, workspace):
-        """Sets the workspace of this ProjectBase.
-
-
-        :param workspace: The workspace of this ProjectBase.  # noqa: E501
-        :type: ProjectBaseWorkspace
-        """
-
-        self._workspace = workspace
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.1/asana/models/project_base_current_status.py` & `asana-4.0.2/asana/models/project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_base_current_status_update.py` & `asana-4.0.2/asana/models/project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_base_workspace.py` & `asana-4.0.2/asana/models/project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_base.py` & `asana-4.0.2/asana/models/project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_compact.py` & `asana-4.0.2/asana/models/project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_request.py` & `asana-4.0.2/asana/models/project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_response.py` & `asana-4.0.2/asana/models/project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_response_data.py` & `asana-4.0.2/asana/models/project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_brief_response_project.py` & `asana-4.0.2/asana/models/project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_briefs_project_brief_gid_body.py` & `asana-4.0.2/asana/models/project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_compact.py` & `asana-4.0.2/asana/models/project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_duplicate_request.py` & `asana-4.0.2/asana/models/project_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_duplicate_request_schedule_dates.py` & `asana-4.0.2/asana/models/project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_add_custom_field_setting_body.py` & `asana-4.0.2/asana/models/project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_add_followers_body.py` & `asana-4.0.2/asana/models/project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_add_members_body.py` & `asana-4.0.2/asana/models/project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_duplicate_body.py` & `asana-4.0.2/asana/models/project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_project_briefs_body.py` & `asana-4.0.2/asana/models/project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_project_statuses_body.py` & `asana-4.0.2/asana/models/project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_remove_custom_field_setting_body.py` & `asana-4.0.2/asana/models/project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_remove_followers_body.py` & `asana-4.0.2/asana/models/project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_remove_members_body.py` & `asana-4.0.2/asana/models/project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_save_as_template_body.py` & `asana-4.0.2/asana/models/project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_gid_sections_body.py` & `asana-4.0.2/asana/models/project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_membership_base.py` & `asana-4.0.2/asana/models/project_membership_response_member.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,117 +11,119 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectMembershipBase(object):
+class ProjectMembershipResponseMember(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
-        'user': 'CustomFieldResponsePeopleValue'
+        'name': 'str'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
-        'user': 'user'
+        'name': 'name'
     }
 
-    def __init__(self, gid=None, resource_type=None, user=None):  # noqa: E501
-        """ProjectMembershipBase - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None):  # noqa: E501
+        """ProjectMembershipResponseMember - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
-        self._user = None
+        self._name = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
-        if user is not None:
-            self.user = user
+        if name is not None:
+            self.name = name
 
     @property
     def gid(self):
-        """Gets the gid of this ProjectMembershipBase.  # noqa: E501
+        """Gets the gid of this ProjectMembershipResponseMember.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this ProjectMembershipBase.  # noqa: E501
+        :return: The gid of this ProjectMembershipResponseMember.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this ProjectMembershipBase.
+        """Sets the gid of this ProjectMembershipResponseMember.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this ProjectMembershipBase.  # noqa: E501
+        :param gid: The gid of this ProjectMembershipResponseMember.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this ProjectMembershipBase.  # noqa: E501
+        """Gets the resource_type of this ProjectMembershipResponseMember.  # noqa: E501
 
-        The base type of this resource.  # noqa: E501
+        The type of the member (team or user)  # noqa: E501
 
-        :return: The resource_type of this ProjectMembershipBase.  # noqa: E501
+        :return: The resource_type of this ProjectMembershipResponseMember.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this ProjectMembershipBase.
+        """Sets the resource_type of this ProjectMembershipResponseMember.
 
-        The base type of this resource.  # noqa: E501
+        The type of the member (team or user)  # noqa: E501
 
-        :param resource_type: The resource_type of this ProjectMembershipBase.  # noqa: E501
+        :param resource_type: The resource_type of this ProjectMembershipResponseMember.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
-    def user(self):
-        """Gets the user of this ProjectMembershipBase.  # noqa: E501
+    def name(self):
+        """Gets the name of this ProjectMembershipResponseMember.  # noqa: E501
 
+        The name of the member  # noqa: E501
 
-        :return: The user of this ProjectMembershipBase.  # noqa: E501
-        :rtype: CustomFieldResponsePeopleValue
+        :return: The name of this ProjectMembershipResponseMember.  # noqa: E501
+        :rtype: str
         """
-        return self._user
+        return self._name
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this ProjectMembershipBase.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ProjectMembershipResponseMember.
 
+        The name of the member  # noqa: E501
 
-        :param user: The user of this ProjectMembershipBase.  # noqa: E501
-        :type: CustomFieldResponsePeopleValue
+        :param name: The name of this ProjectMembershipResponseMember.  # noqa: E501
+        :type: str
         """
 
-        self._user = user
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -136,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectMembershipBase, dict):
+        if issubclass(ProjectMembershipResponseMember, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectMembershipBase):
+        if not isinstance(other, ProjectMembershipResponseMember):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.1/asana/models/project_membership_compact.py` & `asana-4.0.2/asana/models/membership_compact_member.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,117 +11,119 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectMembershipCompact(object):
+class MembershipCompactMember(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
-        'user': 'CustomFieldResponsePeopleValue'
+        'name': 'str'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
-        'user': 'user'
+        'name': 'name'
     }
 
-    def __init__(self, gid=None, resource_type=None, user=None):  # noqa: E501
-        """ProjectMembershipCompact - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None):  # noqa: E501
+        """MembershipCompactMember - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
-        self._user = None
+        self._name = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
-        if user is not None:
-            self.user = user
+        if name is not None:
+            self.name = name
 
     @property
     def gid(self):
-        """Gets the gid of this ProjectMembershipCompact.  # noqa: E501
+        """Gets the gid of this MembershipCompactMember.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this ProjectMembershipCompact.  # noqa: E501
+        :return: The gid of this MembershipCompactMember.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this ProjectMembershipCompact.
+        """Sets the gid of this MembershipCompactMember.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this ProjectMembershipCompact.  # noqa: E501
+        :param gid: The gid of this MembershipCompactMember.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this ProjectMembershipCompact.  # noqa: E501
+        """Gets the resource_type of this MembershipCompactMember.  # noqa: E501
 
-        The base type of this resource.  # noqa: E501
+        The type of the member (team or user)  # noqa: E501
 
-        :return: The resource_type of this ProjectMembershipCompact.  # noqa: E501
+        :return: The resource_type of this MembershipCompactMember.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this ProjectMembershipCompact.
+        """Sets the resource_type of this MembershipCompactMember.
 
-        The base type of this resource.  # noqa: E501
+        The type of the member (team or user)  # noqa: E501
 
-        :param resource_type: The resource_type of this ProjectMembershipCompact.  # noqa: E501
+        :param resource_type: The resource_type of this MembershipCompactMember.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
-    def user(self):
-        """Gets the user of this ProjectMembershipCompact.  # noqa: E501
+    def name(self):
+        """Gets the name of this MembershipCompactMember.  # noqa: E501
 
+        The name of the member  # noqa: E501
 
-        :return: The user of this ProjectMembershipCompact.  # noqa: E501
-        :rtype: CustomFieldResponsePeopleValue
+        :return: The name of this MembershipCompactMember.  # noqa: E501
+        :rtype: str
         """
-        return self._user
+        return self._name
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this ProjectMembershipCompact.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this MembershipCompactMember.
 
+        The name of the member  # noqa: E501
 
-        :param user: The user of this ProjectMembershipCompact.  # noqa: E501
-        :type: CustomFieldResponsePeopleValue
+        :param name: The name of this MembershipCompactMember.  # noqa: E501
+        :type: str
         """
 
-        self._user = user
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -136,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectMembershipCompact, dict):
+        if issubclass(MembershipCompactMember, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectMembershipCompact):
+        if not isinstance(other, MembershipCompactMember):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.1/asana/models/project_membership_response.py` & `asana-4.0.2/asana/models/project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_membership_response_array.py` & `asana-4.0.2/asana/models/project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_membership_response_data.py` & `asana-4.0.2/asana/models/project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_membership_response_member.py` & `asana-4.0.2/asana/models/goal_membership_response_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectMembershipResponseMember(object):
+class GoalMembershipResponseUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,90 +36,90 @@
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name'
     }
 
     def __init__(self, gid=None, resource_type=None, name=None):  # noqa: E501
-        """ProjectMembershipResponseMember - a model defined in Swagger"""  # noqa: E501
+        """GoalMembershipResponseUser - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
 
     @property
     def gid(self):
-        """Gets the gid of this ProjectMembershipResponseMember.  # noqa: E501
+        """Gets the gid of this GoalMembershipResponseUser.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this ProjectMembershipResponseMember.  # noqa: E501
+        :return: The gid of this GoalMembershipResponseUser.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this ProjectMembershipResponseMember.
+        """Sets the gid of this GoalMembershipResponseUser.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this ProjectMembershipResponseMember.  # noqa: E501
+        :param gid: The gid of this GoalMembershipResponseUser.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this ProjectMembershipResponseMember.  # noqa: E501
+        """Gets the resource_type of this GoalMembershipResponseUser.  # noqa: E501
 
-        The type of the member (team or user)  # noqa: E501
+        The base type of this resource.  # noqa: E501
 
-        :return: The resource_type of this ProjectMembershipResponseMember.  # noqa: E501
+        :return: The resource_type of this GoalMembershipResponseUser.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this ProjectMembershipResponseMember.
+        """Sets the resource_type of this GoalMembershipResponseUser.
 
-        The type of the member (team or user)  # noqa: E501
+        The base type of this resource.  # noqa: E501
 
-        :param resource_type: The resource_type of this ProjectMembershipResponseMember.  # noqa: E501
+        :param resource_type: The resource_type of this GoalMembershipResponseUser.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
     def name(self):
-        """Gets the name of this ProjectMembershipResponseMember.  # noqa: E501
+        """Gets the name of this GoalMembershipResponseUser.  # noqa: E501
 
-        The name of the member  # noqa: E501
+        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
 
-        :return: The name of this ProjectMembershipResponseMember.  # noqa: E501
+        :return: The name of this GoalMembershipResponseUser.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this ProjectMembershipResponseMember.
+        """Sets the name of this GoalMembershipResponseUser.
 
-        The name of the member  # noqa: E501
+        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
 
-        :param name: The name of this ProjectMembershipResponseMember.  # noqa: E501
+        :param name: The name of this GoalMembershipResponseUser.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectMembershipResponseMember, dict):
+        if issubclass(GoalMembershipResponseUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectMembershipResponseMember):
+        if not isinstance(other, GoalMembershipResponseUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-4.0.1/asana/models/project_request.py` & `asana-4.0.2/asana/models/project_update_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectRequest(object):
+class ProjectUpdateRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -42,15 +42,14 @@
         'due_on': 'date',
         'html_notes': 'str',
         'members': 'list[CustomFieldResponsePeopleValue]',
         'modified_at': 'datetime',
         'notes': 'str',
         'public': 'bool',
         'start_on': 'date',
-        'workspace': 'ProjectBaseWorkspace',
         'custom_fields': 'dict(str, str)',
         'followers': 'str',
         'owner': 'str',
         'team': 'str'
     }
 
     attribute_map = {
@@ -68,23 +67,22 @@
         'due_on': 'due_on',
         'html_notes': 'html_notes',
         'members': 'members',
         'modified_at': 'modified_at',
         'notes': 'notes',
         'public': 'public',
         'start_on': 'start_on',
-        'workspace': 'workspace',
         'custom_fields': 'custom_fields',
         'followers': 'followers',
         'owner': 'owner',
         'team': 'team'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None, workspace=None, custom_fields=None, followers=None, owner=None, team=None):  # noqa: E501
-        """ProjectRequest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None, custom_fields=None, followers=None, owner=None, team=None):  # noqa: E501
+        """ProjectUpdateRequest - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._archived = None
         self._color = None
         self._created_at = None
         self._current_status = None
@@ -95,15 +93,14 @@
         self._due_on = None
         self._html_notes = None
         self._members = None
         self._modified_at = None
         self._notes = None
         self._public = None
         self._start_on = None
-        self._workspace = None
         self._custom_fields = None
         self._followers = None
         self._owner = None
         self._team = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
@@ -137,555 +134,532 @@
             self.modified_at = modified_at
         if notes is not None:
             self.notes = notes
         if public is not None:
             self.public = public
         if start_on is not None:
             self.start_on = start_on
-        if workspace is not None:
-            self.workspace = workspace
         if custom_fields is not None:
             self.custom_fields = custom_fields
         if followers is not None:
             self.followers = followers
         if owner is not None:
             self.owner = owner
         if team is not None:
             self.team = team
 
     @property
     def gid(self):
-        """Gets the gid of this ProjectRequest.  # noqa: E501
+        """Gets the gid of this ProjectUpdateRequest.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this ProjectRequest.  # noqa: E501
+        :return: The gid of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this ProjectRequest.
+        """Sets the gid of this ProjectUpdateRequest.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this ProjectRequest.  # noqa: E501
+        :param gid: The gid of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this ProjectRequest.  # noqa: E501
+        """Gets the resource_type of this ProjectUpdateRequest.  # noqa: E501
 
         The base type of this resource.  # noqa: E501
 
-        :return: The resource_type of this ProjectRequest.  # noqa: E501
+        :return: The resource_type of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this ProjectRequest.
+        """Sets the resource_type of this ProjectUpdateRequest.
 
         The base type of this resource.  # noqa: E501
 
-        :param resource_type: The resource_type of this ProjectRequest.  # noqa: E501
+        :param resource_type: The resource_type of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
     def name(self):
-        """Gets the name of this ProjectRequest.  # noqa: E501
+        """Gets the name of this ProjectUpdateRequest.  # noqa: E501
 
         Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.  # noqa: E501
 
-        :return: The name of this ProjectRequest.  # noqa: E501
+        :return: The name of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this ProjectRequest.
+        """Sets the name of this ProjectUpdateRequest.
 
         Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.  # noqa: E501
 
-        :param name: The name of this ProjectRequest.  # noqa: E501
+        :param name: The name of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def archived(self):
-        """Gets the archived of this ProjectRequest.  # noqa: E501
+        """Gets the archived of this ProjectUpdateRequest.  # noqa: E501
 
         True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.  # noqa: E501
 
-        :return: The archived of this ProjectRequest.  # noqa: E501
+        :return: The archived of this ProjectUpdateRequest.  # noqa: E501
         :rtype: bool
         """
         return self._archived
 
     @archived.setter
     def archived(self, archived):
-        """Sets the archived of this ProjectRequest.
+        """Sets the archived of this ProjectUpdateRequest.
 
         True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.  # noqa: E501
 
-        :param archived: The archived of this ProjectRequest.  # noqa: E501
+        :param archived: The archived of this ProjectUpdateRequest.  # noqa: E501
         :type: bool
         """
 
         self._archived = archived
 
     @property
     def color(self):
-        """Gets the color of this ProjectRequest.  # noqa: E501
+        """Gets the color of this ProjectUpdateRequest.  # noqa: E501
 
         Color of the project.  # noqa: E501
 
-        :return: The color of this ProjectRequest.  # noqa: E501
+        :return: The color of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._color
 
     @color.setter
     def color(self, color):
-        """Sets the color of this ProjectRequest.
+        """Sets the color of this ProjectUpdateRequest.
 
         Color of the project.  # noqa: E501
 
-        :param color: The color of this ProjectRequest.  # noqa: E501
+        :param color: The color of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
         allowed_values = ["dark-pink", "dark-green", "dark-blue", "dark-red", "dark-teal", "dark-brown", "dark-orange", "dark-purple", "dark-warm-gray", "light-pink", "light-green", "light-blue", "light-red", "light-teal", "light-brown", "light-orange", "light-purple", "light-warm-gray", "none", ""]  # noqa: E501
         if color not in allowed_values:
             raise ValueError(
                 "Invalid value for `color` ({0}), must be one of {1}"  # noqa: E501
                 .format(color, allowed_values)
             )
 
         self._color = color
 
     @property
     def created_at(self):
-        """Gets the created_at of this ProjectRequest.  # noqa: E501
+        """Gets the created_at of this ProjectUpdateRequest.  # noqa: E501
 
         The time at which this resource was created.  # noqa: E501
 
-        :return: The created_at of this ProjectRequest.  # noqa: E501
+        :return: The created_at of this ProjectUpdateRequest.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
-        """Sets the created_at of this ProjectRequest.
+        """Sets the created_at of this ProjectUpdateRequest.
 
         The time at which this resource was created.  # noqa: E501
 
-        :param created_at: The created_at of this ProjectRequest.  # noqa: E501
+        :param created_at: The created_at of this ProjectUpdateRequest.  # noqa: E501
         :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def current_status(self):
-        """Gets the current_status of this ProjectRequest.  # noqa: E501
+        """Gets the current_status of this ProjectUpdateRequest.  # noqa: E501
 
 
-        :return: The current_status of this ProjectRequest.  # noqa: E501
+        :return: The current_status of this ProjectUpdateRequest.  # noqa: E501
         :rtype: ProjectBaseCurrentStatus
         """
         return self._current_status
 
     @current_status.setter
     def current_status(self, current_status):
-        """Sets the current_status of this ProjectRequest.
+        """Sets the current_status of this ProjectUpdateRequest.
 
 
-        :param current_status: The current_status of this ProjectRequest.  # noqa: E501
+        :param current_status: The current_status of this ProjectUpdateRequest.  # noqa: E501
         :type: ProjectBaseCurrentStatus
         """
 
         self._current_status = current_status
 
     @property
     def current_status_update(self):
-        """Gets the current_status_update of this ProjectRequest.  # noqa: E501
+        """Gets the current_status_update of this ProjectUpdateRequest.  # noqa: E501
 
 
-        :return: The current_status_update of this ProjectRequest.  # noqa: E501
+        :return: The current_status_update of this ProjectUpdateRequest.  # noqa: E501
         :rtype: ProjectBaseCurrentStatusUpdate
         """
         return self._current_status_update
 
     @current_status_update.setter
     def current_status_update(self, current_status_update):
-        """Sets the current_status_update of this ProjectRequest.
+        """Sets the current_status_update of this ProjectUpdateRequest.
 
 
-        :param current_status_update: The current_status_update of this ProjectRequest.  # noqa: E501
+        :param current_status_update: The current_status_update of this ProjectUpdateRequest.  # noqa: E501
         :type: ProjectBaseCurrentStatusUpdate
         """
 
         self._current_status_update = current_status_update
 
     @property
     def custom_field_settings(self):
-        """Gets the custom_field_settings of this ProjectRequest.  # noqa: E501
+        """Gets the custom_field_settings of this ProjectUpdateRequest.  # noqa: E501
 
         Array of Custom Field Settings (in compact form).  # noqa: E501
 
-        :return: The custom_field_settings of this ProjectRequest.  # noqa: E501
+        :return: The custom_field_settings of this ProjectUpdateRequest.  # noqa: E501
         :rtype: list[PortfolioResponseCustomFieldSettings]
         """
         return self._custom_field_settings
 
     @custom_field_settings.setter
     def custom_field_settings(self, custom_field_settings):
-        """Sets the custom_field_settings of this ProjectRequest.
+        """Sets the custom_field_settings of this ProjectUpdateRequest.
 
         Array of Custom Field Settings (in compact form).  # noqa: E501
 
-        :param custom_field_settings: The custom_field_settings of this ProjectRequest.  # noqa: E501
+        :param custom_field_settings: The custom_field_settings of this ProjectUpdateRequest.  # noqa: E501
         :type: list[PortfolioResponseCustomFieldSettings]
         """
 
         self._custom_field_settings = custom_field_settings
 
     @property
     def default_view(self):
-        """Gets the default_view of this ProjectRequest.  # noqa: E501
+        """Gets the default_view of this ProjectUpdateRequest.  # noqa: E501
 
         The default view (list, board, calendar, or timeline) of a project.  # noqa: E501
 
-        :return: The default_view of this ProjectRequest.  # noqa: E501
+        :return: The default_view of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._default_view
 
     @default_view.setter
     def default_view(self, default_view):
-        """Sets the default_view of this ProjectRequest.
+        """Sets the default_view of this ProjectUpdateRequest.
 
         The default view (list, board, calendar, or timeline) of a project.  # noqa: E501
 
-        :param default_view: The default_view of this ProjectRequest.  # noqa: E501
+        :param default_view: The default_view of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
         allowed_values = ["list", "board", "calendar", "timeline"]  # noqa: E501
         if default_view not in allowed_values:
             raise ValueError(
                 "Invalid value for `default_view` ({0}), must be one of {1}"  # noqa: E501
                 .format(default_view, allowed_values)
             )
 
         self._default_view = default_view
 
     @property
     def due_date(self):
-        """Gets the due_date of this ProjectRequest.  # noqa: E501
+        """Gets the due_date of this ProjectUpdateRequest.  # noqa: E501
 
         *Deprecated: new integrations should prefer the `due_on` field.*  # noqa: E501
 
-        :return: The due_date of this ProjectRequest.  # noqa: E501
+        :return: The due_date of this ProjectUpdateRequest.  # noqa: E501
         :rtype: date
         """
         return self._due_date
 
     @due_date.setter
     def due_date(self, due_date):
-        """Sets the due_date of this ProjectRequest.
+        """Sets the due_date of this ProjectUpdateRequest.
 
         *Deprecated: new integrations should prefer the `due_on` field.*  # noqa: E501
 
-        :param due_date: The due_date of this ProjectRequest.  # noqa: E501
+        :param due_date: The due_date of this ProjectUpdateRequest.  # noqa: E501
         :type: date
         """
 
         self._due_date = due_date
 
     @property
     def due_on(self):
-        """Gets the due_on of this ProjectRequest.  # noqa: E501
+        """Gets the due_on of this ProjectUpdateRequest.  # noqa: E501
 
         The day on which this project is due. This takes a date with format YYYY-MM-DD.  # noqa: E501
 
-        :return: The due_on of this ProjectRequest.  # noqa: E501
+        :return: The due_on of this ProjectUpdateRequest.  # noqa: E501
         :rtype: date
         """
         return self._due_on
 
     @due_on.setter
     def due_on(self, due_on):
-        """Sets the due_on of this ProjectRequest.
+        """Sets the due_on of this ProjectUpdateRequest.
 
         The day on which this project is due. This takes a date with format YYYY-MM-DD.  # noqa: E501
 
-        :param due_on: The due_on of this ProjectRequest.  # noqa: E501
+        :param due_on: The due_on of this ProjectUpdateRequest.  # noqa: E501
         :type: date
         """
 
         self._due_on = due_on
 
     @property
     def html_notes(self):
-        """Gets the html_notes of this ProjectRequest.  # noqa: E501
+        """Gets the html_notes of this ProjectUpdateRequest.  # noqa: E501
 
         [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.  # noqa: E501
 
-        :return: The html_notes of this ProjectRequest.  # noqa: E501
+        :return: The html_notes of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._html_notes
 
     @html_notes.setter
     def html_notes(self, html_notes):
-        """Sets the html_notes of this ProjectRequest.
+        """Sets the html_notes of this ProjectUpdateRequest.
 
         [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.  # noqa: E501
 
-        :param html_notes: The html_notes of this ProjectRequest.  # noqa: E501
+        :param html_notes: The html_notes of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._html_notes = html_notes
 
     @property
     def members(self):
-        """Gets the members of this ProjectRequest.  # noqa: E501
+        """Gets the members of this ProjectUpdateRequest.  # noqa: E501
 
         Array of users who are members of this project.  # noqa: E501
 
-        :return: The members of this ProjectRequest.  # noqa: E501
+        :return: The members of this ProjectUpdateRequest.  # noqa: E501
         :rtype: list[CustomFieldResponsePeopleValue]
         """
         return self._members
 
     @members.setter
     def members(self, members):
-        """Sets the members of this ProjectRequest.
+        """Sets the members of this ProjectUpdateRequest.
 
         Array of users who are members of this project.  # noqa: E501
 
-        :param members: The members of this ProjectRequest.  # noqa: E501
+        :param members: The members of this ProjectUpdateRequest.  # noqa: E501
         :type: list[CustomFieldResponsePeopleValue]
         """
 
         self._members = members
 
     @property
     def modified_at(self):
-        """Gets the modified_at of this ProjectRequest.  # noqa: E501
+        """Gets the modified_at of this ProjectUpdateRequest.  # noqa: E501
 
         The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*  # noqa: E501
 
-        :return: The modified_at of this ProjectRequest.  # noqa: E501
+        :return: The modified_at of this ProjectUpdateRequest.  # noqa: E501
         :rtype: datetime
         """
         return self._modified_at
 
     @modified_at.setter
     def modified_at(self, modified_at):
-        """Sets the modified_at of this ProjectRequest.
+        """Sets the modified_at of this ProjectUpdateRequest.
 
         The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*  # noqa: E501
 
-        :param modified_at: The modified_at of this ProjectRequest.  # noqa: E501
+        :param modified_at: The modified_at of this ProjectUpdateRequest.  # noqa: E501
         :type: datetime
         """
 
         self._modified_at = modified_at
 
     @property
     def notes(self):
-        """Gets the notes of this ProjectRequest.  # noqa: E501
+        """Gets the notes of this ProjectUpdateRequest.  # noqa: E501
 
         Free-form textual information associated with the project (ie., its description).  # noqa: E501
 
-        :return: The notes of this ProjectRequest.  # noqa: E501
+        :return: The notes of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._notes
 
     @notes.setter
     def notes(self, notes):
-        """Sets the notes of this ProjectRequest.
+        """Sets the notes of this ProjectUpdateRequest.
 
         Free-form textual information associated with the project (ie., its description).  # noqa: E501
 
-        :param notes: The notes of this ProjectRequest.  # noqa: E501
+        :param notes: The notes of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._notes = notes
 
     @property
     def public(self):
-        """Gets the public of this ProjectRequest.  # noqa: E501
+        """Gets the public of this ProjectUpdateRequest.  # noqa: E501
 
         True if the project is public to its team.  # noqa: E501
 
-        :return: The public of this ProjectRequest.  # noqa: E501
+        :return: The public of this ProjectUpdateRequest.  # noqa: E501
         :rtype: bool
         """
         return self._public
 
     @public.setter
     def public(self, public):
-        """Sets the public of this ProjectRequest.
+        """Sets the public of this ProjectUpdateRequest.
 
         True if the project is public to its team.  # noqa: E501
 
-        :param public: The public of this ProjectRequest.  # noqa: E501
+        :param public: The public of this ProjectUpdateRequest.  # noqa: E501
         :type: bool
         """
 
         self._public = public
 
     @property
     def start_on(self):
-        """Gets the start_on of this ProjectRequest.  # noqa: E501
+        """Gets the start_on of this ProjectUpdateRequest.  # noqa: E501
 
         The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*  # noqa: E501
 
-        :return: The start_on of this ProjectRequest.  # noqa: E501
+        :return: The start_on of this ProjectUpdateRequest.  # noqa: E501
         :rtype: date
         """
         return self._start_on
 
     @start_on.setter
     def start_on(self, start_on):
-        """Sets the start_on of this ProjectRequest.
+        """Sets the start_on of this ProjectUpdateRequest.
 
         The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*  # noqa: E501
 
-        :param start_on: The start_on of this ProjectRequest.  # noqa: E501
+        :param start_on: The start_on of this ProjectUpdateRequest.  # noqa: E501
         :type: date
         """
 
         self._start_on = start_on
 
     @property
-    def workspace(self):
-        """Gets the workspace of this ProjectRequest.  # noqa: E501
-
-
-        :return: The workspace of this ProjectRequest.  # noqa: E501
-        :rtype: ProjectBaseWorkspace
-        """
-        return self._workspace
-
-    @workspace.setter
-    def workspace(self, workspace):
-        """Sets the workspace of this ProjectRequest.
-
-
-        :param workspace: The workspace of this ProjectRequest.  # noqa: E501
-        :type: ProjectBaseWorkspace
-        """
-
-        self._workspace = workspace
-
-    @property
     def custom_fields(self):
-        """Gets the custom_fields of this ProjectRequest.  # noqa: E501
+        """Gets the custom_fields of this ProjectUpdateRequest.  # noqa: E501
 
         An object where each key is a Custom Field GID and each value is an enum GID, string, number, or object.  # noqa: E501
 
-        :return: The custom_fields of this ProjectRequest.  # noqa: E501
+        :return: The custom_fields of this ProjectUpdateRequest.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._custom_fields
 
     @custom_fields.setter
     def custom_fields(self, custom_fields):
-        """Sets the custom_fields of this ProjectRequest.
+        """Sets the custom_fields of this ProjectUpdateRequest.
 
         An object where each key is a Custom Field GID and each value is an enum GID, string, number, or object.  # noqa: E501
 
-        :param custom_fields: The custom_fields of this ProjectRequest.  # noqa: E501
+        :param custom_fields: The custom_fields of this ProjectUpdateRequest.  # noqa: E501
         :type: dict(str, str)
         """
 
         self._custom_fields = custom_fields
 
     @property
     def followers(self):
-        """Gets the followers of this ProjectRequest.  # noqa: E501
+        """Gets the followers of this ProjectUpdateRequest.  # noqa: E501
 
         *Create-only*. Comma separated string of users. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.  # noqa: E501
 
-        :return: The followers of this ProjectRequest.  # noqa: E501
+        :return: The followers of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._followers
 
     @followers.setter
     def followers(self, followers):
-        """Sets the followers of this ProjectRequest.
+        """Sets the followers of this ProjectUpdateRequest.
 
         *Create-only*. Comma separated string of users. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.  # noqa: E501
 
-        :param followers: The followers of this ProjectRequest.  # noqa: E501
+        :param followers: The followers of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._followers = followers
 
     @property
     def owner(self):
-        """Gets the owner of this ProjectRequest.  # noqa: E501
+        """Gets the owner of this ProjectUpdateRequest.  # noqa: E501
 
         The current owner of the project, may be null.  # noqa: E501
 
-        :return: The owner of this ProjectRequest.  # noqa: E501
+        :return: The owner of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._owner
 
     @owner.setter
     def owner(self, owner):
-        """Sets the owner of this ProjectRequest.
+        """Sets the owner of this ProjectUpdateRequest.
 
         The current owner of the project, may be null.  # noqa: E501
 
-        :param owner: The owner of this ProjectRequest.  # noqa: E501
+        :param owner: The owner of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._owner = owner
 
     @property
     def team(self):
-        """Gets the team of this ProjectRequest.  # noqa: E501
+        """Gets the team of this ProjectUpdateRequest.  # noqa: E501
 
         The team that this project is shared with.  # noqa: E501
 
-        :return: The team of this ProjectRequest.  # noqa: E501
+        :return: The team of this ProjectUpdateRequest.  # noqa: E501
         :rtype: str
         """
         return self._team
 
     @team.setter
     def team(self, team):
-        """Sets the team of this ProjectRequest.
+        """Sets the team of this ProjectUpdateRequest.
 
         The team that this project is shared with.  # noqa: E501
 
-        :param team: The team of this ProjectRequest.  # noqa: E501
+        :param team: The team of this ProjectUpdateRequest.  # noqa: E501
         :type: str
         """
 
         self._team = team
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -704,15 +678,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectRequest, dict):
+        if issubclass(ProjectUpdateRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -720,15 +694,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectRequest):
+        if not isinstance(other, ProjectUpdateRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.1/asana/models/project_response.py` & `asana-4.0.2/asana/models/project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,27 @@
         'due_on': 'date',
         'html_notes': 'str',
         'members': 'list[CustomFieldResponsePeopleValue]',
         'modified_at': 'datetime',
         'notes': 'str',
         'public': 'bool',
         'start_on': 'date',
-        'workspace': 'ProjectBaseWorkspace',
         'custom_fields': 'list[PortfolioResponseCustomFields]',
         'completed': 'bool',
         'completed_at': 'datetime',
         'completed_by': 'ProjectResponseCompletedBy',
         'followers': 'list[CustomFieldResponsePeopleValue]',
         'owner': 'AllOfProjectResponseOwner',
         'team': 'ProjectResponseTeam',
         'icon': 'str',
         'permalink_url': 'str',
         'project_brief': 'ProjectResponseProjectBrief',
-        'created_from_template': 'ProjectResponseCreatedFromTemplate'
+        'created_from_template': 'ProjectResponseCreatedFromTemplate',
+        'default_access_level': 'str',
+        'workspace': 'ProjectResponseWorkspace'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
         'archived': 'archived',
@@ -75,29 +76,30 @@
         'due_on': 'due_on',
         'html_notes': 'html_notes',
         'members': 'members',
         'modified_at': 'modified_at',
         'notes': 'notes',
         'public': 'public',
         'start_on': 'start_on',
-        'workspace': 'workspace',
         'custom_fields': 'custom_fields',
         'completed': 'completed',
         'completed_at': 'completed_at',
         'completed_by': 'completed_by',
         'followers': 'followers',
         'owner': 'owner',
         'team': 'team',
         'icon': 'icon',
         'permalink_url': 'permalink_url',
         'project_brief': 'project_brief',
-        'created_from_template': 'created_from_template'
+        'created_from_template': 'created_from_template',
+        'default_access_level': 'default_access_level',
+        'workspace': 'workspace'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None, workspace=None, custom_fields=None, completed=None, completed_at=None, completed_by=None, followers=None, owner=None, team=None, icon=None, permalink_url=None, project_brief=None, created_from_template=None):  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, archived=None, color=None, created_at=None, current_status=None, current_status_update=None, custom_field_settings=None, default_view=None, due_date=None, due_on=None, html_notes=None, members=None, modified_at=None, notes=None, public=None, start_on=None, custom_fields=None, completed=None, completed_at=None, completed_by=None, followers=None, owner=None, team=None, icon=None, permalink_url=None, project_brief=None, created_from_template=None, default_access_level=None, workspace=None):  # noqa: E501
         """ProjectResponse - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
         self._archived = None
         self._color = None
         self._created_at = None
@@ -109,26 +111,27 @@
         self._due_on = None
         self._html_notes = None
         self._members = None
         self._modified_at = None
         self._notes = None
         self._public = None
         self._start_on = None
-        self._workspace = None
         self._custom_fields = None
         self._completed = None
         self._completed_at = None
         self._completed_by = None
         self._followers = None
         self._owner = None
         self._team = None
         self._icon = None
         self._permalink_url = None
         self._project_brief = None
         self._created_from_template = None
+        self._default_access_level = None
+        self._workspace = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
@@ -158,16 +161,14 @@
             self.modified_at = modified_at
         if notes is not None:
             self.notes = notes
         if public is not None:
             self.public = public
         if start_on is not None:
             self.start_on = start_on
-        if workspace is not None:
-            self.workspace = workspace
         if custom_fields is not None:
             self.custom_fields = custom_fields
         if completed is not None:
             self.completed = completed
         if completed_at is not None:
             self.completed_at = completed_at
         if completed_by is not None:
@@ -182,14 +183,18 @@
             self.icon = icon
         if permalink_url is not None:
             self.permalink_url = permalink_url
         if project_brief is not None:
             self.project_brief = project_brief
         if created_from_template is not None:
             self.created_from_template = created_from_template
+        if default_access_level is not None:
+            self.default_access_level = default_access_level
+        if workspace is not None:
+            self.workspace = workspace
 
     @property
     def gid(self):
         """Gets the gid of this ProjectResponse.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
@@ -606,35 +611,14 @@
         :param start_on: The start_on of this ProjectResponse.  # noqa: E501
         :type: date
         """
 
         self._start_on = start_on
 
     @property
-    def workspace(self):
-        """Gets the workspace of this ProjectResponse.  # noqa: E501
-
-
-        :return: The workspace of this ProjectResponse.  # noqa: E501
-        :rtype: ProjectBaseWorkspace
-        """
-        return self._workspace
-
-    @workspace.setter
-    def workspace(self, workspace):
-        """Sets the workspace of this ProjectResponse.
-
-
-        :param workspace: The workspace of this ProjectResponse.  # noqa: E501
-        :type: ProjectBaseWorkspace
-        """
-
-        self._workspace = workspace
-
-    @property
     def custom_fields(self):
         """Gets the custom_fields of this ProjectResponse.  # noqa: E501
 
         Array of Custom Fields.  # noqa: E501
 
         :return: The custom_fields of this ProjectResponse.  # noqa: E501
         :rtype: list[PortfolioResponseCustomFields]
@@ -877,14 +861,64 @@
 
         :param created_from_template: The created_from_template of this ProjectResponse.  # noqa: E501
         :type: ProjectResponseCreatedFromTemplate
         """
 
         self._created_from_template = created_from_template
 
+    @property
+    def default_access_level(self):
+        """Gets the default_access_level of this ProjectResponse.  # noqa: E501
+
+        The default access users for users who join or are added as members to the project.  # noqa: E501
+
+        :return: The default_access_level of this ProjectResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._default_access_level
+
+    @default_access_level.setter
+    def default_access_level(self, default_access_level):
+        """Sets the default_access_level of this ProjectResponse.
+
+        The default access users for users who join or are added as members to the project.  # noqa: E501
+
+        :param default_access_level: The default_access_level of this ProjectResponse.  # noqa: E501
+        :type: str
+        """
+        allowed_values = ["admin", "editor", "commenter", "viewer"]  # noqa: E501
+        if default_access_level not in allowed_values:
+            raise ValueError(
+                "Invalid value for `default_access_level` ({0}), must be one of {1}"  # noqa: E501
+                .format(default_access_level, allowed_values)
+            )
+
+        self._default_access_level = default_access_level
+
+    @property
+    def workspace(self):
+        """Gets the workspace of this ProjectResponse.  # noqa: E501
+
+
+        :return: The workspace of this ProjectResponse.  # noqa: E501
+        :rtype: ProjectResponseWorkspace
+        """
+        return self._workspace
+
+    @workspace.setter
+    def workspace(self, workspace):
+        """Sets the workspace of this ProjectResponse.
+
+
+        :param workspace: The workspace of this ProjectResponse.  # noqa: E501
+        :type: ProjectResponseWorkspace
+        """
+
+        self._workspace = workspace
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asana-4.0.1/asana/models/project_response_array.py` & `asana-4.0.2/asana/models/project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_response_completed_by.py` & `asana-4.0.2/asana/models/project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_response_created_from_template.py` & `asana-4.0.2/asana/models/project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_response_data.py` & `asana-4.0.2/asana/models/project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_response_project_brief.py` & `asana-4.0.2/asana/models/project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_response_team.py` & `asana-4.0.2/asana/models/project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_save_as_template_request.py` & `asana-4.0.2/asana/models/project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_section_insert_request.py` & `asana-4.0.2/asana/models/project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_base.py` & `asana-4.0.2/asana/models/project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_compact.py` & `asana-4.0.2/asana/models/project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_request.py` & `asana-4.0.2/asana/models/project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_response.py` & `asana-4.0.2/asana/models/project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_response_array.py` & `asana-4.0.2/asana/models/project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_status_response_data.py` & `asana-4.0.2/asana/models/project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_base.py` & `asana-4.0.2/asana/models/project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_base_requested_dates.py` & `asana-4.0.2/asana/models/project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_base_requested_roles.py` & `asana-4.0.2/asana/models/project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_base_team.py` & `asana-4.0.2/asana/models/project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_compact.py` & `asana-4.0.2/asana/models/project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_gid_instantiate_project_body.py` & `asana-4.0.2/asana/models/project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_instantiate_project_request.py` & `asana-4.0.2/asana/models/project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_instantiate_project_request_requested_dates.py` & `asana-4.0.2/asana/models/project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_instantiate_project_request_requested_roles.py` & `asana-4.0.2/asana/models/project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_response.py` & `asana-4.0.2/asana/models/project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_response_array.py` & `asana-4.0.2/asana/models/project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/project_template_response_data.py` & `asana-4.0.2/asana/models/project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/projects_body.py` & `asana-4.0.2/asana/models/projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/projects_project_gid_body.py` & `asana-4.0.2/asana/models/projects_project_gid_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'ProjectRequest'
+        'data': 'ProjectUpdateRequest'
     }
 
     attribute_map = {
         'data': 'data'
     }
 
     def __init__(self, data=None):  # noqa: E501
@@ -44,25 +44,25 @@
 
     @property
     def data(self):
         """Gets the data of this ProjectsProjectGidBody.  # noqa: E501
 
 
         :return: The data of this ProjectsProjectGidBody.  # noqa: E501
-        :rtype: ProjectRequest
+        :rtype: ProjectUpdateRequest
         """
         return self._data
 
     @data.setter
     def data(self, data):
         """Sets the data of this ProjectsProjectGidBody.
 
 
         :param data: The data of this ProjectsProjectGidBody.  # noqa: E501
-        :type: ProjectRequest
+        :type: ProjectUpdateRequest
         """
 
         self._data = data
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `asana-4.0.1/asana/models/remove_custom_field_setting_request.py` & `asana-4.0.2/asana/models/remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/remove_followers_request.py` & `asana-4.0.2/asana/models/remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/remove_members_request.py` & `asana-4.0.2/asana/models/remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/requested_role_request.py` & `asana-4.0.2/asana/models/requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/rule_trigger_gid_run_body.py` & `asana-4.0.2/asana/models/rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/rule_trigger_request.py` & `asana-4.0.2/asana/models/rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/rule_trigger_response.py` & `asana-4.0.2/asana/models/rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/rule_trigger_response_data.py` & `asana-4.0.2/asana/models/rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_base.py` & `asana-4.0.2/asana/models/section_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_compact.py` & `asana-4.0.2/asana/models/section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_gid_add_task_body.py` & `asana-4.0.2/asana/models/section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_request.py` & `asana-4.0.2/asana/models/section_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_response.py` & `asana-4.0.2/asana/models/section_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_response_array.py` & `asana-4.0.2/asana/models/section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_response_data.py` & `asana-4.0.2/asana/models/section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/section_task_insert_request.py` & `asana-4.0.2/asana/models/section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/sections_insert_body.py` & `asana-4.0.2/asana/models/sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/sections_section_gid_body.py` & `asana-4.0.2/asana/models/sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_base.py` & `asana-4.0.2/asana/models/status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_compact.py` & `asana-4.0.2/asana/models/status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_request.py` & `asana-4.0.2/asana/models/status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_response.py` & `asana-4.0.2/asana/models/status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_response_array.py` & `asana-4.0.2/asana/models/status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_response_data.py` & `asana-4.0.2/asana/models/status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_update_response_parent.py` & `asana-4.0.2/asana/models/status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/status_updates_body.py` & `asana-4.0.2/asana/models/status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/stories_story_gid_body.py` & `asana-4.0.2/asana/models/stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_base.py` & `asana-4.0.2/asana/models/story_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_compact.py` & `asana-4.0.2/asana/models/story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_request.py` & `asana-4.0.2/asana/models/story_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response.py` & `asana-4.0.2/asana/models/story_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_array.py` & `asana-4.0.2/asana/models/story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_assignee.py` & `asana-4.0.2/asana/models/story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_custom_field.py` & `asana-4.0.2/asana/models/story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_data.py` & `asana-4.0.2/asana/models/story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_dates.py` & `asana-4.0.2/asana/models/story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_old_dates.py` & `asana-4.0.2/asana/models/story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_old_enum_value.py` & `asana-4.0.2/asana/models/story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_old_section.py` & `asana-4.0.2/asana/models/story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_previews.py` & `asana-4.0.2/asana/models/story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_project.py` & `asana-4.0.2/asana/models/story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_story.py` & `asana-4.0.2/asana/models/story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_tag.py` & `asana-4.0.2/asana/models/story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_target.py` & `asana-4.0.2/asana/models/story_response_target.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/story_response_task.py` & `asana-4.0.2/asana/models/story_response_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_base.py` & `asana-4.0.2/asana/models/tag_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_compact.py` & `asana-4.0.2/asana/models/tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_request.py` & `asana-4.0.2/asana/models/tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_response.py` & `asana-4.0.2/asana/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_response_array.py` & `asana-4.0.2/asana/models/tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tag_response_data.py` & `asana-4.0.2/asana/models/tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tags_body.py` & `asana-4.0.2/asana/models/tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_add_followers_request.py` & `asana-4.0.2/asana/models/task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_add_project_request.py` & `asana-4.0.2/asana/models/task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_add_tag_request.py` & `asana-4.0.2/asana/models/task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base.py` & `asana-4.0.2/asana/models/task_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base_completed_by.py` & `asana-4.0.2/asana/models/task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base_dependencies.py` & `asana-4.0.2/asana/models/task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base_external.py` & `asana-4.0.2/asana/models/task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base_memberships.py` & `asana-4.0.2/asana/models/task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_base_section.py` & `asana-4.0.2/asana/models/task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_compact.py` & `asana-4.0.2/asana/models/task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_count_response.py` & `asana-4.0.2/asana/models/task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_count_response_data.py` & `asana-4.0.2/asana/models/task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_duplicate_request.py` & `asana-4.0.2/asana/models/task_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_add_dependencies_body.py` & `asana-4.0.2/asana/models/task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_add_dependents_body.py` & `asana-4.0.2/asana/models/task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_add_followers_body.py` & `asana-4.0.2/asana/models/task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_add_project_body.py` & `asana-4.0.2/asana/models/task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_add_tag_body.py` & `asana-4.0.2/asana/models/task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_duplicate_body.py` & `asana-4.0.2/asana/models/task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_remove_dependencies_body.py` & `asana-4.0.2/asana/models/task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_remove_dependents_body.py` & `asana-4.0.2/asana/models/task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_remove_followers_body.py` & `asana-4.0.2/asana/models/task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_remove_project_body.py` & `asana-4.0.2/asana/models/task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_remove_tag_body.py` & `asana-4.0.2/asana/models/task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_set_parent_body.py` & `asana-4.0.2/asana/models/task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_stories_body.py` & `asana-4.0.2/asana/models/task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_subtasks_body.py` & `asana-4.0.2/asana/models/task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_gid_time_tracking_entries_body.py` & `asana-4.0.2/asana/models/task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_remove_followers_request.py` & `asana-4.0.2/asana/models/task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_remove_project_request.py` & `asana-4.0.2/asana/models/task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_remove_tag_request.py` & `asana-4.0.2/asana/models/task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_request.py` & `asana-4.0.2/asana/models/task_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response.py` & `asana-4.0.2/asana/models/task_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_array.py` & `asana-4.0.2/asana/models/task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_assignee_section.py` & `asana-4.0.2/asana/models/task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_custom_fields.py` & `asana-4.0.2/asana/models/task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_data.py` & `asana-4.0.2/asana/models/task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_parent.py` & `asana-4.0.2/asana/models/task_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_tags.py` & `asana-4.0.2/asana/models/task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_response_workspace.py` & `asana-4.0.2/asana/models/task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/task_set_parent_request.py` & `asana-4.0.2/asana/models/task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tasks_body.py` & `asana-4.0.2/asana/models/tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/tasks_task_gid_body.py` & `asana-4.0.2/asana/models/tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_add_user_request.py` & `asana-4.0.2/asana/models/team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_base.py` & `asana-4.0.2/asana/models/team_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_compact.py` & `asana-4.0.2/asana/models/team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_gid_add_user_body.py` & `asana-4.0.2/asana/models/team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_gid_projects_body.py` & `asana-4.0.2/asana/models/team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_gid_remove_user_body.py` & `asana-4.0.2/asana/models/team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_membership_base.py` & `asana-4.0.2/asana/models/team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_membership_compact.py` & `asana-4.0.2/asana/models/team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_membership_response.py` & `asana-4.0.2/asana/models/team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_membership_response_array.py` & `asana-4.0.2/asana/models/team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_membership_response_data.py` & `asana-4.0.2/asana/models/team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_remove_user_request.py` & `asana-4.0.2/asana/models/team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_request.py` & `asana-4.0.2/asana/models/team_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_response.py` & `asana-4.0.2/asana/models/team_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_response_array.py` & `asana-4.0.2/asana/models/team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_response_data.py` & `asana-4.0.2/asana/models/team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/team_response_organization.py` & `asana-4.0.2/asana/models/team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/teams_body.py` & `asana-4.0.2/asana/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/teams_team_gid_body.py` & `asana-4.0.2/asana/models/teams_team_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/template_role.py` & `asana-4.0.2/asana/models/template_role.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_period_base.py` & `asana-4.0.2/asana/models/time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_period_compact.py` & `asana-4.0.2/asana/models/time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_period_response.py` & `asana-4.0.2/asana/models/time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_period_response_array.py` & `asana-4.0.2/asana/models/time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_period_response_data.py` & `asana-4.0.2/asana/models/time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py` & `asana-4.0.2/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_tracking_entry_base.py` & `asana-4.0.2/asana/models/time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_tracking_entry_base_data.py` & `asana-4.0.2/asana/models/time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_tracking_entry_compact.py` & `asana-4.0.2/asana/models/time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/time_tracking_entry_compact_array.py` & `asana-4.0.2/asana/models/time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/update_time_tracking_entry_request.py` & `asana-4.0.2/asana/models/update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_base.py` & `asana-4.0.2/asana/models/user_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_base_response.py` & `asana-4.0.2/asana/models/user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_base_response_data.py` & `asana-4.0.2/asana/models/user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_base_response_photo.py` & `asana-4.0.2/asana/models/user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_compact.py` & `asana-4.0.2/asana/models/user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_request.py` & `asana-4.0.2/asana/models/user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_response.py` & `asana-4.0.2/asana/models/user_task_list_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserResponse(object):
+class UserTaskListResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -27,185 +27,159 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'gid': 'str',
         'resource_type': 'str',
         'name': 'str',
-        'email': 'str',
-        'photo': 'UserBaseResponsePhoto',
-        'workspaces': 'list[GoalResponseWorkspace]'
+        'owner': 'AllOfUserTaskListResponseOwner',
+        'workspace': 'AllOfUserTaskListResponseWorkspace'
     }
 
     attribute_map = {
         'gid': 'gid',
         'resource_type': 'resource_type',
         'name': 'name',
-        'email': 'email',
-        'photo': 'photo',
-        'workspaces': 'workspaces'
+        'owner': 'owner',
+        'workspace': 'workspace'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, email=None, photo=None, workspaces=None):  # noqa: E501
-        """UserResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, gid=None, resource_type=None, name=None, owner=None, workspace=None):  # noqa: E501
+        """UserTaskListResponse - a model defined in Swagger"""  # noqa: E501
         self._gid = None
         self._resource_type = None
         self._name = None
-        self._email = None
-        self._photo = None
-        self._workspaces = None
+        self._owner = None
+        self._workspace = None
         self.discriminator = None
         if gid is not None:
             self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
         if name is not None:
             self.name = name
-        if email is not None:
-            self.email = email
-        if photo is not None:
-            self.photo = photo
-        if workspaces is not None:
-            self.workspaces = workspaces
+        if owner is not None:
+            self.owner = owner
+        if workspace is not None:
+            self.workspace = workspace
 
     @property
     def gid(self):
-        """Gets the gid of this UserResponse.  # noqa: E501
+        """Gets the gid of this UserTaskListResponse.  # noqa: E501
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :return: The gid of this UserResponse.  # noqa: E501
+        :return: The gid of this UserTaskListResponse.  # noqa: E501
         :rtype: str
         """
         return self._gid
 
     @gid.setter
     def gid(self, gid):
-        """Sets the gid of this UserResponse.
+        """Sets the gid of this UserTaskListResponse.
 
         Globally unique identifier of the resource, as a string.  # noqa: E501
 
-        :param gid: The gid of this UserResponse.  # noqa: E501
+        :param gid: The gid of this UserTaskListResponse.  # noqa: E501
         :type: str
         """
 
         self._gid = gid
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this UserResponse.  # noqa: E501
+        """Gets the resource_type of this UserTaskListResponse.  # noqa: E501
 
         The base type of this resource.  # noqa: E501
 
-        :return: The resource_type of this UserResponse.  # noqa: E501
+        :return: The resource_type of this UserTaskListResponse.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this UserResponse.
+        """Sets the resource_type of this UserTaskListResponse.
 
         The base type of this resource.  # noqa: E501
 
-        :param resource_type: The resource_type of this UserResponse.  # noqa: E501
+        :param resource_type: The resource_type of this UserTaskListResponse.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
     def name(self):
-        """Gets the name of this UserResponse.  # noqa: E501
+        """Gets the name of this UserTaskListResponse.  # noqa: E501
 
-        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
+        The name of the user task list.  # noqa: E501
 
-        :return: The name of this UserResponse.  # noqa: E501
+        :return: The name of this UserTaskListResponse.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this UserResponse.
+        """Sets the name of this UserTaskListResponse.
 
-        *Read-only except when same user as requester*. The user’s name.  # noqa: E501
+        The name of the user task list.  # noqa: E501
 
-        :param name: The name of this UserResponse.  # noqa: E501
+        :param name: The name of this UserTaskListResponse.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
-    def email(self):
-        """Gets the email of this UserResponse.  # noqa: E501
+    def owner(self):
+        """Gets the owner of this UserTaskListResponse.  # noqa: E501
 
-        The user's email address.  # noqa: E501
+        The owner of the user task list, i.e. the person whose My Tasks is represented by this resource.  # noqa: E501
 
-        :return: The email of this UserResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._email
-
-    @email.setter
-    def email(self, email):
-        """Sets the email of this UserResponse.
-
-        The user's email address.  # noqa: E501
-
-        :param email: The email of this UserResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._email = email
-
-    @property
-    def photo(self):
-        """Gets the photo of this UserResponse.  # noqa: E501
-
-
-        :return: The photo of this UserResponse.  # noqa: E501
-        :rtype: UserBaseResponsePhoto
+        :return: The owner of this UserTaskListResponse.  # noqa: E501
+        :rtype: AllOfUserTaskListResponseOwner
         """
-        return self._photo
+        return self._owner
 
-    @photo.setter
-    def photo(self, photo):
-        """Sets the photo of this UserResponse.
+    @owner.setter
+    def owner(self, owner):
+        """Sets the owner of this UserTaskListResponse.
 
+        The owner of the user task list, i.e. the person whose My Tasks is represented by this resource.  # noqa: E501
 
-        :param photo: The photo of this UserResponse.  # noqa: E501
-        :type: UserBaseResponsePhoto
+        :param owner: The owner of this UserTaskListResponse.  # noqa: E501
+        :type: AllOfUserTaskListResponseOwner
         """
 
-        self._photo = photo
+        self._owner = owner
 
     @property
-    def workspaces(self):
-        """Gets the workspaces of this UserResponse.  # noqa: E501
+    def workspace(self):
+        """Gets the workspace of this UserTaskListResponse.  # noqa: E501
 
-        Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.  # noqa: E501
+        The workspace in which the user task list is located.  # noqa: E501
 
-        :return: The workspaces of this UserResponse.  # noqa: E501
-        :rtype: list[GoalResponseWorkspace]
+        :return: The workspace of this UserTaskListResponse.  # noqa: E501
+        :rtype: AllOfUserTaskListResponseWorkspace
         """
-        return self._workspaces
+        return self._workspace
 
-    @workspaces.setter
-    def workspaces(self, workspaces):
-        """Sets the workspaces of this UserResponse.
+    @workspace.setter
+    def workspace(self, workspace):
+        """Sets the workspace of this UserTaskListResponse.
 
-        Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.  # noqa: E501
+        The workspace in which the user task list is located.  # noqa: E501
 
-        :param workspaces: The workspaces of this UserResponse.  # noqa: E501
-        :type: list[GoalResponseWorkspace]
+        :param workspace: The workspace of this UserTaskListResponse.  # noqa: E501
+        :type: AllOfUserTaskListResponseWorkspace
         """
 
-        self._workspaces = workspaces
+        self._workspace = workspace
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -220,15 +194,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserResponse, dict):
+        if issubclass(UserTaskListResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -236,15 +210,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserResponse):
+        if not isinstance(other, UserTaskListResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-4.0.1/asana/models/user_response_array.py` & `asana-4.0.2/asana/models/user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_response_data.py` & `asana-4.0.2/asana/models/user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_task_list_base.py` & `asana-4.0.2/asana/models/user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_task_list_compact.py` & `asana-4.0.2/asana/models/user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_task_list_request.py` & `asana-4.0.2/asana/models/user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/user_task_list_response.py` & `asana-4.0.2/asana/models/webhook_filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,175 +11,147 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserTaskListResponse(object):
+class WebhookFilter(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'gid': 'str',
         'resource_type': 'str',
-        'name': 'str',
-        'owner': 'AllOfUserTaskListResponseOwner',
-        'workspace': 'AllOfUserTaskListResponseWorkspace'
+        'resource_subtype': 'str',
+        'action': 'str',
+        'fields': 'list[str]'
     }
 
     attribute_map = {
-        'gid': 'gid',
         'resource_type': 'resource_type',
-        'name': 'name',
-        'owner': 'owner',
-        'workspace': 'workspace'
+        'resource_subtype': 'resource_subtype',
+        'action': 'action',
+        'fields': 'fields'
     }
 
-    def __init__(self, gid=None, resource_type=None, name=None, owner=None, workspace=None):  # noqa: E501
-        """UserTaskListResponse - a model defined in Swagger"""  # noqa: E501
-        self._gid = None
+    def __init__(self, resource_type=None, resource_subtype=None, action=None, fields=None):  # noqa: E501
+        """WebhookFilter - a model defined in Swagger"""  # noqa: E501
         self._resource_type = None
-        self._name = None
-        self._owner = None
-        self._workspace = None
+        self._resource_subtype = None
+        self._action = None
+        self._fields = None
         self.discriminator = None
-        if gid is not None:
-            self.gid = gid
         if resource_type is not None:
             self.resource_type = resource_type
-        if name is not None:
-            self.name = name
-        if owner is not None:
-            self.owner = owner
-        if workspace is not None:
-            self.workspace = workspace
-
-    @property
-    def gid(self):
-        """Gets the gid of this UserTaskListResponse.  # noqa: E501
-
-        Globally unique identifier of the resource, as a string.  # noqa: E501
-
-        :return: The gid of this UserTaskListResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._gid
-
-    @gid.setter
-    def gid(self, gid):
-        """Sets the gid of this UserTaskListResponse.
-
-        Globally unique identifier of the resource, as a string.  # noqa: E501
-
-        :param gid: The gid of this UserTaskListResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._gid = gid
+        if resource_subtype is not None:
+            self.resource_subtype = resource_subtype
+        if action is not None:
+            self.action = action
+        if fields is not None:
+            self.fields = fields
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this UserTaskListResponse.  # noqa: E501
+        """Gets the resource_type of this WebhookFilter.  # noqa: E501
 
-        The base type of this resource.  # noqa: E501
+        The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :return: The resource_type of this UserTaskListResponse.  # noqa: E501
+        :return: The resource_type of this WebhookFilter.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this UserTaskListResponse.
+        """Sets the resource_type of this WebhookFilter.
 
-        The base type of this resource.  # noqa: E501
+        The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :param resource_type: The resource_type of this UserTaskListResponse.  # noqa: E501
+        :param resource_type: The resource_type of this WebhookFilter.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
-    def name(self):
-        """Gets the name of this UserTaskListResponse.  # noqa: E501
+    def resource_subtype(self):
+        """Gets the resource_subtype of this WebhookFilter.  # noqa: E501
 
-        The name of the user task list.  # noqa: E501
+        The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :return: The name of this UserTaskListResponse.  # noqa: E501
+        :return: The resource_subtype of this WebhookFilter.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._resource_subtype
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this UserTaskListResponse.
+    @resource_subtype.setter
+    def resource_subtype(self, resource_subtype):
+        """Sets the resource_subtype of this WebhookFilter.
 
-        The name of the user task list.  # noqa: E501
+        The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :param name: The name of this UserTaskListResponse.  # noqa: E501
+        :param resource_subtype: The resource_subtype of this WebhookFilter.  # noqa: E501
         :type: str
         """
 
-        self._name = name
+        self._resource_subtype = resource_subtype
 
     @property
-    def owner(self):
-        """Gets the owner of this UserTaskListResponse.  # noqa: E501
+    def action(self):
+        """Gets the action of this WebhookFilter.  # noqa: E501
 
-        The owner of the user task list, i.e. the person whose My Tasks is represented by this resource.  # noqa: E501
+        The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :return: The owner of this UserTaskListResponse.  # noqa: E501
-        :rtype: AllOfUserTaskListResponseOwner
+        :return: The action of this WebhookFilter.  # noqa: E501
+        :rtype: str
         """
-        return self._owner
+        return self._action
 
-    @owner.setter
-    def owner(self, owner):
-        """Sets the owner of this UserTaskListResponse.
+    @action.setter
+    def action(self, action):
+        """Sets the action of this WebhookFilter.
 
-        The owner of the user task list, i.e. the person whose My Tasks is represented by this resource.  # noqa: E501
+        The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :param owner: The owner of this UserTaskListResponse.  # noqa: E501
-        :type: AllOfUserTaskListResponseOwner
+        :param action: The action of this WebhookFilter.  # noqa: E501
+        :type: str
         """
 
-        self._owner = owner
+        self._action = action
 
     @property
-    def workspace(self):
-        """Gets the workspace of this UserTaskListResponse.  # noqa: E501
+    def fields(self):
+        """Gets the fields of this WebhookFilter.  # noqa: E501
 
-        The workspace in which the user task list is located.  # noqa: E501
+        *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :return: The workspace of this UserTaskListResponse.  # noqa: E501
-        :rtype: AllOfUserTaskListResponseWorkspace
+        :return: The fields of this WebhookFilter.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._workspace
+        return self._fields
 
-    @workspace.setter
-    def workspace(self, workspace):
-        """Sets the workspace of this UserTaskListResponse.
+    @fields.setter
+    def fields(self, fields):
+        """Sets the fields of this WebhookFilter.
 
-        The workspace in which the user task list is located.  # noqa: E501
+        *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :param workspace: The workspace of this UserTaskListResponse.  # noqa: E501
-        :type: AllOfUserTaskListResponseWorkspace
+        :param fields: The fields of this WebhookFilter.  # noqa: E501
+        :type: list[str]
         """
 
-        self._workspace = workspace
+        self._fields = fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -194,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserTaskListResponse, dict):
+        if issubclass(WebhookFilter, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -210,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserTaskListResponse):
+        if not isinstance(other, WebhookFilter):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.1/asana/models/user_task_list_response_data.py` & `asana-4.0.2/asana/models/user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_compact.py` & `asana-4.0.2/asana/models/webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_compact_resource.py` & `asana-4.0.2/asana/models/webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_filter.py` & `asana-4.0.2/asana/models/webhook_request_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WebhookFilter(object):
+class WebhookRequestFilters(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,15 +38,15 @@
         'resource_type': 'resource_type',
         'resource_subtype': 'resource_subtype',
         'action': 'action',
         'fields': 'fields'
     }
 
     def __init__(self, resource_type=None, resource_subtype=None, action=None, fields=None):  # noqa: E501
-        """WebhookFilter - a model defined in Swagger"""  # noqa: E501
+        """WebhookRequestFilters - a model defined in Swagger"""  # noqa: E501
         self._resource_type = None
         self._resource_subtype = None
         self._action = None
         self._fields = None
         self.discriminator = None
         if resource_type is not None:
             self.resource_type = resource_type
@@ -55,99 +55,99 @@
         if action is not None:
             self.action = action
         if fields is not None:
             self.fields = fields
 
     @property
     def resource_type(self):
-        """Gets the resource_type of this WebhookFilter.  # noqa: E501
+        """Gets the resource_type of this WebhookRequestFilters.  # noqa: E501
 
         The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :return: The resource_type of this WebhookFilter.  # noqa: E501
+        :return: The resource_type of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._resource_type
 
     @resource_type.setter
     def resource_type(self, resource_type):
-        """Sets the resource_type of this WebhookFilter.
+        """Sets the resource_type of this WebhookRequestFilters.
 
         The type of the resource which created the event when modified; for example, to filter to changes on regular tasks this field should be set to `task`.  # noqa: E501
 
-        :param resource_type: The resource_type of this WebhookFilter.  # noqa: E501
+        :param resource_type: The resource_type of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._resource_type = resource_type
 
     @property
     def resource_subtype(self):
-        """Gets the resource_subtype of this WebhookFilter.  # noqa: E501
+        """Gets the resource_subtype of this WebhookRequestFilters.  # noqa: E501
 
         The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :return: The resource_subtype of this WebhookFilter.  # noqa: E501
+        :return: The resource_subtype of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._resource_subtype
 
     @resource_subtype.setter
     def resource_subtype(self, resource_subtype):
-        """Sets the resource_subtype of this WebhookFilter.
+        """Sets the resource_subtype of this WebhookRequestFilters.
 
         The resource subtype of the resource that the filter applies to. This should be set to the same value as is returned on the `resource_subtype` field on the resources themselves.  # noqa: E501
 
-        :param resource_subtype: The resource_subtype of this WebhookFilter.  # noqa: E501
+        :param resource_subtype: The resource_subtype of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._resource_subtype = resource_subtype
 
     @property
     def action(self):
-        """Gets the action of this WebhookFilter.  # noqa: E501
+        """Gets the action of this WebhookRequestFilters.  # noqa: E501
 
         The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :return: The action of this WebhookFilter.  # noqa: E501
+        :return: The action of this WebhookRequestFilters.  # noqa: E501
         :rtype: str
         """
         return self._action
 
     @action.setter
     def action(self, action):
-        """Sets the action of this WebhookFilter.
+        """Sets the action of this WebhookRequestFilters.
 
         The type of change on the **resource** to pass through the filter. For more information refer to `Event.action` in the [event](/reference/events) schema. This can be one of `changed`, `added`, `removed`, `deleted`, and `undeleted` depending on the nature of what has occurred on the resource.  # noqa: E501
 
-        :param action: The action of this WebhookFilter.  # noqa: E501
+        :param action: The action of this WebhookRequestFilters.  # noqa: E501
         :type: str
         """
 
         self._action = action
 
     @property
     def fields(self):
-        """Gets the fields of this WebhookFilter.  # noqa: E501
+        """Gets the fields of this WebhookRequestFilters.  # noqa: E501
 
         *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :return: The fields of this WebhookFilter.  # noqa: E501
+        :return: The fields of this WebhookRequestFilters.  # noqa: E501
         :rtype: list[str]
         """
         return self._fields
 
     @fields.setter
     def fields(self, fields):
-        """Sets the fields of this WebhookFilter.
+        """Sets the fields of this WebhookRequestFilters.
 
         *Conditional.* A whitelist of fields for events which will pass the filter when the resource is changed. These can be any combination of the fields on the resources themselves. This field is only valid for `action` of type `changed`  # noqa: E501
 
-        :param fields: The fields of this WebhookFilter.  # noqa: E501
+        :param fields: The fields of this WebhookRequestFilters.  # noqa: E501
         :type: list[str]
         """
 
         self._fields = fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -166,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WebhookFilter, dict):
+        if issubclass(WebhookRequestFilters, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -182,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WebhookFilter):
+        if not isinstance(other, WebhookRequestFilters):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asana-4.0.1/asana/models/webhook_request.py` & `asana-4.0.2/asana/models/webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_response.py` & `asana-4.0.2/asana/models/webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_response_array.py` & `asana-4.0.2/asana/models/webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_response_data.py` & `asana-4.0.2/asana/models/webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhook_update_request.py` & `asana-4.0.2/asana/models/webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhooks_body.py` & `asana-4.0.2/asana/models/webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/webhooks_webhook_gid_body.py` & `asana-4.0.2/asana/models/webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_add_user_request.py` & `asana-4.0.2/asana/models/workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_base.py` & `asana-4.0.2/asana/models/workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_compact.py` & `asana-4.0.2/asana/models/workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_gid_add_user_body.py` & `asana-4.0.2/asana/models/workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_gid_projects_body.py` & `asana-4.0.2/asana/models/workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_gid_remove_user_body.py` & `asana-4.0.2/asana/models/workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_gid_tags_body.py` & `asana-4.0.2/asana/models/workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_base.py` & `asana-4.0.2/asana/models/workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_compact.py` & `asana-4.0.2/asana/models/workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_request.py` & `asana-4.0.2/asana/models/workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_response.py` & `asana-4.0.2/asana/models/workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_response_array.py` & `asana-4.0.2/asana/models/workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_response_data.py` & `asana-4.0.2/asana/models/workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_response_user_task_list.py` & `asana-4.0.2/asana/models/workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_membership_response_vacation_dates.py` & `asana-4.0.2/asana/models/workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_remove_user_request.py` & `asana-4.0.2/asana/models/workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_request.py` & `asana-4.0.2/asana/models/workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_response.py` & `asana-4.0.2/asana/models/workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_response_array.py` & `asana-4.0.2/asana/models/workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspace_response_data.py` & `asana-4.0.2/asana/models/workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/models/workspaces_workspace_gid_body.py` & `asana-4.0.2/asana/models/workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana/rest.py` & `asana-4.0.2/asana/rest.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/asana.egg-info/PKG-INFO` & `asana-4.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: asana
-Version: 4.0.1
-Summary: Asana
-Home-page: http://github.com/asana/python-asana
-Author: Asana, Inc
-License: MIT
-Keywords: asana,Asana
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # asana [![GitHub release][release-image]]() [![Build][github-actions-image]][github-actions-url] [![PyPi Version][pypi-image]][pypi-url]
 
 Python client library for Asana
 
 - API version: 1.0
-- Package version: 4.0.1
+- Package version: 4.0.2
 
 ## Requirements.
 
 Python 3.4+
 
 ## Installation & Usage
 ### pip install from [PyPI](https://pypi.org/project/asana/)
@@ -493,17 +482,18 @@
  - [GoalGidAddFollowersBody](docs/GoalGidAddFollowersBody.md)
  - [GoalGidAddSupportingRelationshipBody](docs/GoalGidAddSupportingRelationshipBody.md)
  - [GoalGidRemoveFollowersBody](docs/GoalGidRemoveFollowersBody.md)
  - [GoalGidRemoveSupportingRelationshipBody](docs/GoalGidRemoveSupportingRelationshipBody.md)
  - [GoalGidSetMetricBody](docs/GoalGidSetMetricBody.md)
  - [GoalGidSetMetricCurrentValueBody](docs/GoalGidSetMetricCurrentValueBody.md)
  - [GoalMembershipBase](docs/GoalMembershipBase.md)
- - [GoalMembershipBaseGoal](docs/GoalMembershipBaseGoal.md)
  - [GoalMembershipCompact](docs/GoalMembershipCompact.md)
  - [GoalMembershipResponse](docs/GoalMembershipResponse.md)
+ - [GoalMembershipResponseUser](docs/GoalMembershipResponseUser.md)
+ - [GoalMembershipResponseWorkspace](docs/GoalMembershipResponseWorkspace.md)
  - [GoalMetricBase](docs/GoalMetricBase.md)
  - [GoalMetricCurrentValueRequest](docs/GoalMetricCurrentValueRequest.md)
  - [GoalMetricRequest](docs/GoalMetricRequest.md)
  - [GoalRelationshipBase](docs/GoalRelationshipBase.md)
  - [GoalRelationshipBaseSupportedGoal](docs/GoalRelationshipBaseSupportedGoal.md)
  - [GoalRelationshipBaseSupportingResource](docs/GoalRelationshipBaseSupportingResource.md)
  - [GoalRelationshipCompact](docs/GoalRelationshipCompact.md)
@@ -535,14 +525,18 @@
  - [JobBaseNewProjectTemplate](docs/JobBaseNewProjectTemplate.md)
  - [JobBaseNewTask](docs/JobBaseNewTask.md)
  - [JobCompact](docs/JobCompact.md)
  - [JobResponse](docs/JobResponse.md)
  - [JobResponseData](docs/JobResponseData.md)
  - [Like](docs/Like.md)
  - [MemberCompact](docs/MemberCompact.md)
+ - [MembershipCompact](docs/MembershipCompact.md)
+ - [MembershipCompactGoal](docs/MembershipCompactGoal.md)
+ - [MembershipCompactMember](docs/MembershipCompactMember.md)
+ - [MembershipCompactParent](docs/MembershipCompactParent.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [MembershipResponse](docs/MembershipResponse.md)
  - [MembershipResponseArray](docs/MembershipResponseArray.md)
  - [MembershipResponseData](docs/MembershipResponseData.md)
  - [MembershipsBody](docs/MembershipsBody.md)
  - [ModifyDependenciesRequest](docs/ModifyDependenciesRequest.md)
  - [ModifyDependentsRequest](docs/ModifyDependentsRequest.md)
@@ -579,15 +573,14 @@
  - [PortfolioResponseWorkspace](docs/PortfolioResponseWorkspace.md)
  - [PortfoliosBody](docs/PortfoliosBody.md)
  - [PortfoliosPortfolioGidBody](docs/PortfoliosPortfolioGidBody.md)
  - [Preview](docs/Preview.md)
  - [ProjectBase](docs/ProjectBase.md)
  - [ProjectBaseCurrentStatus](docs/ProjectBaseCurrentStatus.md)
  - [ProjectBaseCurrentStatusUpdate](docs/ProjectBaseCurrentStatusUpdate.md)
- - [ProjectBaseWorkspace](docs/ProjectBaseWorkspace.md)
  - [ProjectBriefBase](docs/ProjectBriefBase.md)
  - [ProjectBriefCompact](docs/ProjectBriefCompact.md)
  - [ProjectBriefRequest](docs/ProjectBriefRequest.md)
  - [ProjectBriefResponse](docs/ProjectBriefResponse.md)
  - [ProjectBriefResponseData](docs/ProjectBriefResponseData.md)
  - [ProjectBriefResponseProject](docs/ProjectBriefResponseProject.md)
  - [ProjectBriefsProjectBriefGidBody](docs/ProjectBriefsProjectBriefGidBody.md)
@@ -603,26 +596,27 @@
  - [ProjectGidRemoveCustomFieldSettingBody](docs/ProjectGidRemoveCustomFieldSettingBody.md)
  - [ProjectGidRemoveFollowersBody](docs/ProjectGidRemoveFollowersBody.md)
  - [ProjectGidRemoveMembersBody](docs/ProjectGidRemoveMembersBody.md)
  - [ProjectGidSaveAsTemplateBody](docs/ProjectGidSaveAsTemplateBody.md)
  - [ProjectGidSectionsBody](docs/ProjectGidSectionsBody.md)
  - [ProjectMembershipBase](docs/ProjectMembershipBase.md)
  - [ProjectMembershipCompact](docs/ProjectMembershipCompact.md)
- - [ProjectMembershipResponse](docs/ProjectMembershipResponse.md)
- - [ProjectMembershipResponseArray](docs/ProjectMembershipResponseArray.md)
- - [ProjectMembershipResponseData](docs/ProjectMembershipResponseData.md)
- - [ProjectMembershipResponseMember](docs/ProjectMembershipResponseMember.md)
+ - [ProjectMembershipCompactArray](docs/ProjectMembershipCompactArray.md)
+ - [ProjectMembershipCompactResponse](docs/ProjectMembershipCompactResponse.md)
+ - [ProjectMembershipNormalResponse](docs/ProjectMembershipNormalResponse.md)
+ - [ProjectMembershipNormalResponseData](docs/ProjectMembershipNormalResponseData.md)
  - [ProjectRequest](docs/ProjectRequest.md)
  - [ProjectResponse](docs/ProjectResponse.md)
  - [ProjectResponseArray](docs/ProjectResponseArray.md)
  - [ProjectResponseCompletedBy](docs/ProjectResponseCompletedBy.md)
  - [ProjectResponseCreatedFromTemplate](docs/ProjectResponseCreatedFromTemplate.md)
  - [ProjectResponseData](docs/ProjectResponseData.md)
  - [ProjectResponseProjectBrief](docs/ProjectResponseProjectBrief.md)
  - [ProjectResponseTeam](docs/ProjectResponseTeam.md)
+ - [ProjectResponseWorkspace](docs/ProjectResponseWorkspace.md)
  - [ProjectSaveAsTemplateRequest](docs/ProjectSaveAsTemplateRequest.md)
  - [ProjectSectionInsertRequest](docs/ProjectSectionInsertRequest.md)
  - [ProjectStatusBase](docs/ProjectStatusBase.md)
  - [ProjectStatusCompact](docs/ProjectStatusCompact.md)
  - [ProjectStatusRequest](docs/ProjectStatusRequest.md)
  - [ProjectStatusResponse](docs/ProjectStatusResponse.md)
  - [ProjectStatusResponseArray](docs/ProjectStatusResponseArray.md)
@@ -635,14 +629,15 @@
  - [ProjectTemplateGidInstantiateProjectBody](docs/ProjectTemplateGidInstantiateProjectBody.md)
  - [ProjectTemplateInstantiateProjectRequest](docs/ProjectTemplateInstantiateProjectRequest.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedDates](docs/ProjectTemplateInstantiateProjectRequestRequestedDates.md)
  - [ProjectTemplateInstantiateProjectRequestRequestedRoles](docs/ProjectTemplateInstantiateProjectRequestRequestedRoles.md)
  - [ProjectTemplateResponse](docs/ProjectTemplateResponse.md)
  - [ProjectTemplateResponseArray](docs/ProjectTemplateResponseArray.md)
  - [ProjectTemplateResponseData](docs/ProjectTemplateResponseData.md)
+ - [ProjectUpdateRequest](docs/ProjectUpdateRequest.md)
  - [ProjectsBody](docs/ProjectsBody.md)
  - [ProjectsProjectGidBody](docs/ProjectsProjectGidBody.md)
  - [RemoveCustomFieldSettingRequest](docs/RemoveCustomFieldSettingRequest.md)
  - [RemoveFollowersRequest](docs/RemoveFollowersRequest.md)
  - [RemoveMembersRequest](docs/RemoveMembersRequest.md)
  - [RequestedRoleRequest](docs/RequestedRoleRequest.md)
  - [RuleTriggerGidRunBody](docs/RuleTriggerGidRunBody.md)
```

### Comparing `asana-4.0.1/asana.egg-info/SOURCES.txt` & `asana-4.0.2/asana.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,16 @@
 asana/models/goal_gid_remove_supporting_relationship_body.py
 asana/models/goal_gid_set_metric_body.py
 asana/models/goal_gid_set_metric_current_value_body.py
 asana/models/goal_membership_base.py
 asana/models/goal_membership_base_goal.py
 asana/models/goal_membership_compact.py
 asana/models/goal_membership_response.py
+asana/models/goal_membership_response_user.py
+asana/models/goal_membership_response_workspace.py
 asana/models/goal_metric_base.py
 asana/models/goal_metric_current_value_request.py
 asana/models/goal_metric_request.py
 asana/models/goal_relationship_base.py
 asana/models/goal_relationship_base_supported_goal.py
 asana/models/goal_relationship_base_supporting_resource.py
 asana/models/goal_relationship_compact.py
@@ -181,14 +183,18 @@
 asana/models/job_base_new_project_template.py
 asana/models/job_base_new_task.py
 asana/models/job_compact.py
 asana/models/job_response.py
 asana/models/job_response_data.py
 asana/models/like.py
 asana/models/member_compact.py
+asana/models/membership_compact.py
+asana/models/membership_compact_goal.py
+asana/models/membership_compact_member.py
+asana/models/membership_compact_parent.py
 asana/models/membership_request.py
 asana/models/membership_response.py
 asana/models/membership_response_array.py
 asana/models/membership_response_data.py
 asana/models/memberships_body.py
 asana/models/modify_dependencies_request.py
 asana/models/modify_dependents_request.py
@@ -249,26 +255,31 @@
 asana/models/project_gid_remove_custom_field_setting_body.py
 asana/models/project_gid_remove_followers_body.py
 asana/models/project_gid_remove_members_body.py
 asana/models/project_gid_save_as_template_body.py
 asana/models/project_gid_sections_body.py
 asana/models/project_membership_base.py
 asana/models/project_membership_compact.py
+asana/models/project_membership_compact_array.py
+asana/models/project_membership_compact_response.py
+asana/models/project_membership_normal_response.py
+asana/models/project_membership_normal_response_data.py
 asana/models/project_membership_response.py
 asana/models/project_membership_response_array.py
 asana/models/project_membership_response_data.py
 asana/models/project_membership_response_member.py
 asana/models/project_request.py
 asana/models/project_response.py
 asana/models/project_response_array.py
 asana/models/project_response_completed_by.py
 asana/models/project_response_created_from_template.py
 asana/models/project_response_data.py
 asana/models/project_response_project_brief.py
 asana/models/project_response_team.py
+asana/models/project_response_workspace.py
 asana/models/project_save_as_template_request.py
 asana/models/project_section_insert_request.py
 asana/models/project_status_base.py
 asana/models/project_status_compact.py
 asana/models/project_status_request.py
 asana/models/project_status_response.py
 asana/models/project_status_response_array.py
@@ -281,14 +292,15 @@
 asana/models/project_template_gid_instantiate_project_body.py
 asana/models/project_template_instantiate_project_request.py
 asana/models/project_template_instantiate_project_request_requested_dates.py
 asana/models/project_template_instantiate_project_request_requested_roles.py
 asana/models/project_template_response.py
 asana/models/project_template_response_array.py
 asana/models/project_template_response_data.py
+asana/models/project_update_request.py
 asana/models/projects_body.py
 asana/models/projects_project_gid_body.py
 asana/models/remove_custom_field_setting_request.py
 asana/models/remove_followers_request.py
 asana/models/remove_members_request.py
 asana/models/requested_role_request.py
 asana/models/rule_trigger_gid_run_body.py
@@ -562,14 +574,16 @@
 test/test_goal_gid_remove_supporting_relationship_body.py
 test/test_goal_gid_set_metric_body.py
 test/test_goal_gid_set_metric_current_value_body.py
 test/test_goal_membership_base.py
 test/test_goal_membership_base_goal.py
 test/test_goal_membership_compact.py
 test/test_goal_membership_response.py
+test/test_goal_membership_response_user.py
+test/test_goal_membership_response_workspace.py
 test/test_goal_metric_base.py
 test/test_goal_metric_current_value_request.py
 test/test_goal_metric_request.py
 test/test_goal_relationship_base.py
 test/test_goal_relationship_base_supported_goal.py
 test/test_goal_relationship_base_supporting_resource.py
 test/test_goal_relationship_compact.py
@@ -604,14 +618,18 @@
 test/test_job_base_new_task.py
 test/test_job_compact.py
 test/test_job_response.py
 test/test_job_response_data.py
 test/test_jobs_api.py
 test/test_like.py
 test/test_member_compact.py
+test/test_membership_compact.py
+test/test_membership_compact_goal.py
+test/test_membership_compact_member.py
+test/test_membership_compact_parent.py
 test/test_membership_request.py
 test/test_membership_response.py
 test/test_membership_response_array.py
 test/test_membership_response_data.py
 test/test_memberships_api.py
 test/test_memberships_body.py
 test/test_modify_dependencies_request.py
@@ -677,27 +695,32 @@
 test/test_project_gid_remove_custom_field_setting_body.py
 test/test_project_gid_remove_followers_body.py
 test/test_project_gid_remove_members_body.py
 test/test_project_gid_save_as_template_body.py
 test/test_project_gid_sections_body.py
 test/test_project_membership_base.py
 test/test_project_membership_compact.py
+test/test_project_membership_compact_array.py
+test/test_project_membership_compact_response.py
+test/test_project_membership_normal_response.py
+test/test_project_membership_normal_response_data.py
 test/test_project_membership_response.py
 test/test_project_membership_response_array.py
 test/test_project_membership_response_data.py
 test/test_project_membership_response_member.py
 test/test_project_memberships_api.py
 test/test_project_request.py
 test/test_project_response.py
 test/test_project_response_array.py
 test/test_project_response_completed_by.py
 test/test_project_response_created_from_template.py
 test/test_project_response_data.py
 test/test_project_response_project_brief.py
 test/test_project_response_team.py
+test/test_project_response_workspace.py
 test/test_project_save_as_template_request.py
 test/test_project_section_insert_request.py
 test/test_project_status_base.py
 test/test_project_status_compact.py
 test/test_project_status_request.py
 test/test_project_status_response.py
 test/test_project_status_response_array.py
@@ -712,14 +735,15 @@
 test/test_project_template_instantiate_project_request.py
 test/test_project_template_instantiate_project_request_requested_dates.py
 test/test_project_template_instantiate_project_request_requested_roles.py
 test/test_project_template_response.py
 test/test_project_template_response_array.py
 test/test_project_template_response_data.py
 test/test_project_templates_api.py
+test/test_project_update_request.py
 test/test_projects_api.py
 test/test_projects_body.py
 test/test_projects_project_gid_body.py
 test/test_remove_custom_field_setting_request.py
 test/test_remove_followers_request.py
 test/test_remove_members_request.py
 test/test_requested_role_request.py
```

### Comparing `asana-4.0.1/setup.py` & `asana-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import os
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "asana"
-VERSION = "4.0.1"
+VERSION = "4.0.2"
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     LONG_DESCRIPTION = readme.read()
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
```

### Comparing `asana-4.0.1/test/test_add_custom_field_setting_request.py` & `asana-4.0.2/test/test_add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_add_followers_request.py` & `asana-4.0.2/test/test_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_add_members_request.py` & `asana-4.0.2/test/test_add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_project_response_owner.py` & `asana-4.0.2/test/test_all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_project_template_base_owner.py` & `asana-4.0.2/test/test_all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_project_template_response_owner.py` & `asana-4.0.2/test/test_all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_story_response_new_date_value.py` & `asana-4.0.2/test/test_all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_story_response_old_date_value.py` & `asana-4.0.2/test/test_all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_base_owner.py` & `asana-4.0.2/test/test_all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_base_workspace.py` & `asana-4.0.2/test/test_all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_compact_owner.py` & `asana-4.0.2/test/test_all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_compact_workspace.py` & `asana-4.0.2/test/test_all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_request_owner.py` & `asana-4.0.2/test/test_all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_request_workspace.py` & `asana-4.0.2/test/test_all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_response_owner.py` & `asana-4.0.2/test/test_all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_user_task_list_response_workspace.py` & `asana-4.0.2/test/test_all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_workspace_membership_response_user_task_list_owner.py` & `asana-4.0.2/test/test_all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_all_of_workspace_membership_response_user_task_list_workspace.py` & `asana-4.0.2/test/test_all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_asana_named_resource.py` & `asana-4.0.2/test/test_asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_asana_named_resource_array.py` & `asana-4.0.2/test/test_asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_asana_resource.py` & `asana-4.0.2/test/test_asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_base.py` & `asana-4.0.2/test/test_attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_compact.py` & `asana-4.0.2/test/test_attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_request.py` & `asana-4.0.2/test/test_attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_response.py` & `asana-4.0.2/test/test_attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_response_array.py` & `asana-4.0.2/test/test_attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_response_data.py` & `asana-4.0.2/test/test_attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachment_response_parent.py` & `asana-4.0.2/test/test_attachment_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_attachments_api.py` & `asana-4.0.2/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_api_api.py` & `asana-4.0.2/test/test_audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event.py` & `asana-4.0.2/test/test_audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event_actor.py` & `asana-4.0.2/test/test_audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event_array.py` & `asana-4.0.2/test/test_audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event_context.py` & `asana-4.0.2/test/test_audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event_details.py` & `asana-4.0.2/test/test_audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_audit_log_event_resource.py` & `asana-4.0.2/test/test_audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_api_api.py` & `asana-4.0.2/test/test_batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_body.py` & `asana-4.0.2/test/test_batch_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_request.py` & `asana-4.0.2/test/test_batch_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_request_action.py` & `asana-4.0.2/test/test_batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_request_actions.py` & `asana-4.0.2/test/test_batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_request_options.py` & `asana-4.0.2/test/test_batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_response.py` & `asana-4.0.2/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_batch_response_array.py` & `asana-4.0.2/test/test_batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_create_membership_request.py` & `asana-4.0.2/test/test_create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_create_time_tracking_entry_request.py` & `asana-4.0.2/test/test_create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_base.py` & `asana-4.0.2/test/test_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_base_date_value.py` & `asana-4.0.2/test/test_custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_base_enum_options.py` & `asana-4.0.2/test/test_custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_base_enum_value.py` & `asana-4.0.2/test/test_custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_compact.py` & `asana-4.0.2/test/test_custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_gid_enum_options_body.py` & `asana-4.0.2/test/test_custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_request.py` & `asana-4.0.2/test/test_custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_response.py` & `asana-4.0.2/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_response_array.py` & `asana-4.0.2/test/test_custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_response_created_by.py` & `asana-4.0.2/test/test_custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_response_data.py` & `asana-4.0.2/test/test_custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_response_people_value.py` & `asana-4.0.2/test/test_custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_base.py` & `asana-4.0.2/test/test_custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_compact.py` & `asana-4.0.2/test/test_custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response.py` & `asana-4.0.2/test/test_custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response_array.py` & `asana-4.0.2/test/test_custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response_custom_field.py` & `asana-4.0.2/test/test_custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response_data.py` & `asana-4.0.2/test/test_custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response_parent.py` & `asana-4.0.2/test/test_custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_setting_response_project.py` & `asana-4.0.2/test/test_custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_field_settings_api.py` & `asana-4.0.2/test/test_custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_fields_api.py` & `asana-4.0.2/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_fields_body.py` & `asana-4.0.2/test/test_custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_custom_fields_custom_field_gid_body.py` & `asana-4.0.2/test/test_custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_date_variable_compact.py` & `asana-4.0.2/test/test_date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_date_variable_request.py` & `asana-4.0.2/test/test_date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_empty_response.py` & `asana-4.0.2/test/test_empty_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_empty_response_data.py` & `asana-4.0.2/test/test_empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_option.py` & `asana-4.0.2/test/test_enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_option_base.py` & `asana-4.0.2/test/test_enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_option_data.py` & `asana-4.0.2/test/test_enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_option_insert_request.py` & `asana-4.0.2/test/test_enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_option_request.py` & `asana-4.0.2/test/test_enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_options_enum_option_gid_body.py` & `asana-4.0.2/test/test_enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_enum_options_insert_body.py` & `asana-4.0.2/test/test_enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_error.py` & `asana-4.0.2/test/test_error.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_error_response.py` & `asana-4.0.2/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_error_response_errors.py` & `asana-4.0.2/test/test_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response.py` & `asana-4.0.2/test/test_event_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response_array.py` & `asana-4.0.2/test/test_event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response_change.py` & `asana-4.0.2/test/test_event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response_parent.py` & `asana-4.0.2/test/test_event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response_resource.py` & `asana-4.0.2/test/test_event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_event_response_user.py` & `asana-4.0.2/test/test_event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_events_api.py` & `asana-4.0.2/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_add_subgoal_request.py` & `asana-4.0.2/test/test_goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_add_supporting_relationship_request.py` & `asana-4.0.2/test/test_goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_add_supporting_work_request.py` & `asana-4.0.2/test/test_goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_base.py` & `asana-4.0.2/test/test_goal_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_compact.py` & `asana-4.0.2/test/test_goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_add_followers_body.py` & `asana-4.0.2/test/test_goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_add_supporting_relationship_body.py` & `asana-4.0.2/test/test_goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_remove_followers_body.py` & `asana-4.0.2/test/test_goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_remove_supporting_relationship_body.py` & `asana-4.0.2/test/test_goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_set_metric_body.py` & `asana-4.0.2/test/test_goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_gid_set_metric_current_value_body.py` & `asana-4.0.2/test/test_goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_membership_base.py` & `asana-4.0.2/test/test_goal_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_membership_base_goal.py` & `asana-4.0.2/test/test_goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_membership_compact.py` & `asana-4.0.2/test/test_goal_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_membership_response.py` & `asana-4.0.2/test/test_goal_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_metric_base.py` & `asana-4.0.2/test/test_goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_metric_current_value_request.py` & `asana-4.0.2/test/test_goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_metric_request.py` & `asana-4.0.2/test/test_goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_base.py` & `asana-4.0.2/test/test_goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_base_supported_goal.py` & `asana-4.0.2/test/test_goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_base_supporting_resource.py` & `asana-4.0.2/test/test_goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_compact.py` & `asana-4.0.2/test/test_goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_request.py` & `asana-4.0.2/test/test_goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_response.py` & `asana-4.0.2/test/test_goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_response_array.py` & `asana-4.0.2/test/test_goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationship_response_data.py` & `asana-4.0.2/test/test_goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationships_api.py` & `asana-4.0.2/test/test_goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_relationships_goal_relationship_gid_body.py` & `asana-4.0.2/test/test_goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_remove_subgoal_request.py` & `asana-4.0.2/test/test_goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_remove_supporting_relationship_request.py` & `asana-4.0.2/test/test_goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_request.py` & `asana-4.0.2/test/test_goal_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_request_base.py` & `asana-4.0.2/test/test_goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response.py` & `asana-4.0.2/test/test_goal_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_array.py` & `asana-4.0.2/test/test_goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_current_status_update.py` & `asana-4.0.2/test/test_goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_data.py` & `asana-4.0.2/test/test_goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_likes.py` & `asana-4.0.2/test/test_goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_metric.py` & `asana-4.0.2/test/test_goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_team.py` & `asana-4.0.2/test/test_goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_time_period.py` & `asana-4.0.2/test/test_goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_response_workspace.py` & `asana-4.0.2/test/test_goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goal_update_request.py` & `asana-4.0.2/test/test_goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goals_api.py` & `asana-4.0.2/test/test_goals_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goals_body.py` & `asana-4.0.2/test/test_goals_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_goals_goal_gid_body.py` & `asana-4.0.2/test/test_goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_inline_response412.py` & `asana-4.0.2/test/test_inline_response412.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_inline_response412_errors.py` & `asana-4.0.2/test/test_inline_response412_errors.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_base.py` & `asana-4.0.2/test/test_job_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_base_new_project.py` & `asana-4.0.2/test/test_job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_base_new_project_template.py` & `asana-4.0.2/test/test_job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_base_new_task.py` & `asana-4.0.2/test/test_job_base_new_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_compact.py` & `asana-4.0.2/test/test_job_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_response.py` & `asana-4.0.2/test/test_job_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_job_response_data.py` & `asana-4.0.2/test/test_job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_jobs_api.py` & `asana-4.0.2/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_like.py` & `asana-4.0.2/test/test_like.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_member_compact.py` & `asana-4.0.2/test/test_member_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_membership_request.py` & `asana-4.0.2/test/test_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_membership_response.py` & `asana-4.0.2/test/test_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_membership_response_array.py` & `asana-4.0.2/test/test_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_membership_response_data.py` & `asana-4.0.2/test/test_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_memberships_api.py` & `asana-4.0.2/test/test_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_memberships_body.py` & `asana-4.0.2/test/test_memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_modify_dependencies_request.py` & `asana-4.0.2/test/test_modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_modify_dependents_request.py` & `asana-4.0.2/test/test_modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_next_page.py` & `asana-4.0.2/test/test_next_page.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_export_base.py` & `asana-4.0.2/test/test_organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_export_compact.py` & `asana-4.0.2/test/test_organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_export_request.py` & `asana-4.0.2/test/test_organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_export_response.py` & `asana-4.0.2/test/test_organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_export_response_data.py` & `asana-4.0.2/test/test_organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_exports_api.py` & `asana-4.0.2/test/test_organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_organization_exports_body.py` & `asana-4.0.2/test/test_organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_add_item_request.py` & `asana-4.0.2/test/test_portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_base.py` & `asana-4.0.2/test/test_portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_compact.py` & `asana-4.0.2/test/test_portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_add_custom_field_setting_body.py` & `asana-4.0.2/test/test_portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_add_item_body.py` & `asana-4.0.2/test/test_portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_add_members_body.py` & `asana-4.0.2/test/test_portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_remove_custom_field_setting_body.py` & `asana-4.0.2/test/test_portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_remove_item_body.py` & `asana-4.0.2/test/test_portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_gid_remove_members_body.py` & `asana-4.0.2/test/test_portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_base.py` & `asana-4.0.2/test/test_portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_base_portfolio.py` & `asana-4.0.2/test/test_portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_compact.py` & `asana-4.0.2/test/test_portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_response.py` & `asana-4.0.2/test/test_portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_response_array.py` & `asana-4.0.2/test/test_portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_membership_response_data.py` & `asana-4.0.2/test/test_portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_memberships_api.py` & `asana-4.0.2/test/test_portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_remove_item_request.py` & `asana-4.0.2/test/test_portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_request.py` & `asana-4.0.2/test/test_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response.py` & `asana-4.0.2/test/test_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_array.py` & `asana-4.0.2/test/test_portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_current_status_update.py` & `asana-4.0.2/test/test_portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_custom_field_settings.py` & `asana-4.0.2/test/test_portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_custom_fields.py` & `asana-4.0.2/test/test_portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_data.py` & `asana-4.0.2/test/test_portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolio_response_workspace.py` & `asana-4.0.2/test/test_portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolios_api.py` & `asana-4.0.2/test/test_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolios_body.py` & `asana-4.0.2/test/test_portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_portfolios_portfolio_gid_body.py` & `asana-4.0.2/test/test_portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_preview.py` & `asana-4.0.2/test/test_preview.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_base.py` & `asana-4.0.2/test/test_project_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_base_current_status.py` & `asana-4.0.2/test/test_project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_base_current_status_update.py` & `asana-4.0.2/test/test_project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_base_workspace.py` & `asana-4.0.2/test/test_project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_base.py` & `asana-4.0.2/test/test_project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_compact.py` & `asana-4.0.2/test/test_project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_request.py` & `asana-4.0.2/test/test_project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_response.py` & `asana-4.0.2/test/test_project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_response_data.py` & `asana-4.0.2/test/test_project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_brief_response_project.py` & `asana-4.0.2/test/test_project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_briefs_api.py` & `asana-4.0.2/test/test_project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_briefs_project_brief_gid_body.py` & `asana-4.0.2/test/test_project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_compact.py` & `asana-4.0.2/test/test_project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_duplicate_request.py` & `asana-4.0.2/test/test_project_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_duplicate_request_schedule_dates.py` & `asana-4.0.2/test/test_project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_add_custom_field_setting_body.py` & `asana-4.0.2/test/test_project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_add_followers_body.py` & `asana-4.0.2/test/test_project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_add_members_body.py` & `asana-4.0.2/test/test_project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_duplicate_body.py` & `asana-4.0.2/test/test_project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_project_briefs_body.py` & `asana-4.0.2/test/test_project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_project_statuses_body.py` & `asana-4.0.2/test/test_project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_remove_custom_field_setting_body.py` & `asana-4.0.2/test/test_project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_remove_followers_body.py` & `asana-4.0.2/test/test_project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_remove_members_body.py` & `asana-4.0.2/test/test_project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_save_as_template_body.py` & `asana-4.0.2/test/test_project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_gid_sections_body.py` & `asana-4.0.2/test/test_project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_base.py` & `asana-4.0.2/test/test_project_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_compact.py` & `asana-4.0.2/test/test_project_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_response.py` & `asana-4.0.2/test/test_project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_response_array.py` & `asana-4.0.2/test/test_project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_response_data.py` & `asana-4.0.2/test/test_project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_membership_response_member.py` & `asana-4.0.2/test/test_project_membership_response_member.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_memberships_api.py` & `asana-4.0.2/test/test_project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_request.py` & `asana-4.0.2/test/test_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response.py` & `asana-4.0.2/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_array.py` & `asana-4.0.2/test/test_project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_completed_by.py` & `asana-4.0.2/test/test_project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_created_from_template.py` & `asana-4.0.2/test/test_project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_data.py` & `asana-4.0.2/test/test_project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_project_brief.py` & `asana-4.0.2/test/test_project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_response_team.py` & `asana-4.0.2/test/test_project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_save_as_template_request.py` & `asana-4.0.2/test/test_project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_section_insert_request.py` & `asana-4.0.2/test/test_project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_base.py` & `asana-4.0.2/test/test_project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_compact.py` & `asana-4.0.2/test/test_project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_request.py` & `asana-4.0.2/test/test_project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_response.py` & `asana-4.0.2/test/test_project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_response_array.py` & `asana-4.0.2/test/test_project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_status_response_data.py` & `asana-4.0.2/test/test_project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_statuses_api.py` & `asana-4.0.2/test/test_project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_base.py` & `asana-4.0.2/test/test_project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_base_requested_dates.py` & `asana-4.0.2/test/test_project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_base_requested_roles.py` & `asana-4.0.2/test/test_project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_base_team.py` & `asana-4.0.2/test/test_project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_compact.py` & `asana-4.0.2/test/test_project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_gid_instantiate_project_body.py` & `asana-4.0.2/test/test_project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_instantiate_project_request.py` & `asana-4.0.2/test/test_project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_instantiate_project_request_requested_dates.py` & `asana-4.0.2/test/test_project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_instantiate_project_request_requested_roles.py` & `asana-4.0.2/test/test_project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_response.py` & `asana-4.0.2/test/test_project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_response_array.py` & `asana-4.0.2/test/test_project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_template_response_data.py` & `asana-4.0.2/test/test_project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_project_templates_api.py` & `asana-4.0.2/test/test_project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_projects_api.py` & `asana-4.0.2/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_projects_body.py` & `asana-4.0.2/test/test_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_projects_project_gid_body.py` & `asana-4.0.2/test/test_projects_project_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_remove_custom_field_setting_request.py` & `asana-4.0.2/test/test_remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_remove_followers_request.py` & `asana-4.0.2/test/test_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_remove_members_request.py` & `asana-4.0.2/test/test_remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_requested_role_request.py` & `asana-4.0.2/test/test_requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_rule_trigger_gid_run_body.py` & `asana-4.0.2/test/test_rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_rule_trigger_request.py` & `asana-4.0.2/test/test_rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_rule_trigger_response.py` & `asana-4.0.2/test/test_rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_rule_trigger_response_data.py` & `asana-4.0.2/test/test_rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_rules_api.py` & `asana-4.0.2/test/test_rules_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_base.py` & `asana-4.0.2/test/test_section_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_compact.py` & `asana-4.0.2/test/test_section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_gid_add_task_body.py` & `asana-4.0.2/test/test_section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_request.py` & `asana-4.0.2/test/test_section_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_response.py` & `asana-4.0.2/test/test_section_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_response_array.py` & `asana-4.0.2/test/test_section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_response_data.py` & `asana-4.0.2/test/test_section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_section_task_insert_request.py` & `asana-4.0.2/test/test_section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_sections_api.py` & `asana-4.0.2/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_sections_insert_body.py` & `asana-4.0.2/test/test_sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_sections_section_gid_body.py` & `asana-4.0.2/test/test_sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_base.py` & `asana-4.0.2/test/test_status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_compact.py` & `asana-4.0.2/test/test_status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_request.py` & `asana-4.0.2/test/test_status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_response.py` & `asana-4.0.2/test/test_status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_response_array.py` & `asana-4.0.2/test/test_status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_response_data.py` & `asana-4.0.2/test/test_status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_update_response_parent.py` & `asana-4.0.2/test/test_status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_updates_api.py` & `asana-4.0.2/test/test_status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_status_updates_body.py` & `asana-4.0.2/test/test_status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_stories_api.py` & `asana-4.0.2/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_stories_story_gid_body.py` & `asana-4.0.2/test/test_stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_base.py` & `asana-4.0.2/test/test_story_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_compact.py` & `asana-4.0.2/test/test_story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_request.py` & `asana-4.0.2/test/test_story_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response.py` & `asana-4.0.2/test/test_story_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_array.py` & `asana-4.0.2/test/test_story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_assignee.py` & `asana-4.0.2/test/test_story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_custom_field.py` & `asana-4.0.2/test/test_story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_data.py` & `asana-4.0.2/test/test_story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_dates.py` & `asana-4.0.2/test/test_story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_old_dates.py` & `asana-4.0.2/test/test_story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_old_enum_value.py` & `asana-4.0.2/test/test_story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_old_section.py` & `asana-4.0.2/test/test_story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_previews.py` & `asana-4.0.2/test/test_story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_project.py` & `asana-4.0.2/test/test_story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_story.py` & `asana-4.0.2/test/test_story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_tag.py` & `asana-4.0.2/test/test_story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_target.py` & `asana-4.0.2/test/test_story_response_target.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_story_response_task.py` & `asana-4.0.2/test/test_story_response_task.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_base.py` & `asana-4.0.2/test/test_tag_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_compact.py` & `asana-4.0.2/test/test_tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_request.py` & `asana-4.0.2/test/test_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_response.py` & `asana-4.0.2/test/test_tag_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_response_array.py` & `asana-4.0.2/test/test_tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tag_response_data.py` & `asana-4.0.2/test/test_tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tags_api.py` & `asana-4.0.2/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tags_body.py` & `asana-4.0.2/test/test_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_add_followers_request.py` & `asana-4.0.2/test/test_task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_add_project_request.py` & `asana-4.0.2/test/test_task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_add_tag_request.py` & `asana-4.0.2/test/test_task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base.py` & `asana-4.0.2/test/test_task_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base_completed_by.py` & `asana-4.0.2/test/test_task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base_dependencies.py` & `asana-4.0.2/test/test_task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base_external.py` & `asana-4.0.2/test/test_task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base_memberships.py` & `asana-4.0.2/test/test_task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_base_section.py` & `asana-4.0.2/test/test_task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_compact.py` & `asana-4.0.2/test/test_task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_count_response.py` & `asana-4.0.2/test/test_task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_count_response_data.py` & `asana-4.0.2/test/test_task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_duplicate_request.py` & `asana-4.0.2/test/test_task_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_add_dependencies_body.py` & `asana-4.0.2/test/test_task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_add_dependents_body.py` & `asana-4.0.2/test/test_task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_add_followers_body.py` & `asana-4.0.2/test/test_task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_add_project_body.py` & `asana-4.0.2/test/test_task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_add_tag_body.py` & `asana-4.0.2/test/test_task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_duplicate_body.py` & `asana-4.0.2/test/test_task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_remove_dependencies_body.py` & `asana-4.0.2/test/test_task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_remove_dependents_body.py` & `asana-4.0.2/test/test_task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_remove_followers_body.py` & `asana-4.0.2/test/test_task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_remove_project_body.py` & `asana-4.0.2/test/test_task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_remove_tag_body.py` & `asana-4.0.2/test/test_task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_set_parent_body.py` & `asana-4.0.2/test/test_task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_stories_body.py` & `asana-4.0.2/test/test_task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_subtasks_body.py` & `asana-4.0.2/test/test_task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_gid_time_tracking_entries_body.py` & `asana-4.0.2/test/test_task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_remove_followers_request.py` & `asana-4.0.2/test/test_task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_remove_project_request.py` & `asana-4.0.2/test/test_task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_remove_tag_request.py` & `asana-4.0.2/test/test_task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_request.py` & `asana-4.0.2/test/test_task_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response.py` & `asana-4.0.2/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_array.py` & `asana-4.0.2/test/test_task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_assignee_section.py` & `asana-4.0.2/test/test_task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_custom_fields.py` & `asana-4.0.2/test/test_task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_data.py` & `asana-4.0.2/test/test_task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_parent.py` & `asana-4.0.2/test/test_task_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_tags.py` & `asana-4.0.2/test/test_task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_response_workspace.py` & `asana-4.0.2/test/test_task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_task_set_parent_request.py` & `asana-4.0.2/test/test_task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tasks_api.py` & `asana-4.0.2/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tasks_body.py` & `asana-4.0.2/test/test_tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_tasks_task_gid_body.py` & `asana-4.0.2/test/test_tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_add_user_request.py` & `asana-4.0.2/test/test_team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_base.py` & `asana-4.0.2/test/test_team_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_compact.py` & `asana-4.0.2/test/test_team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_gid_add_user_body.py` & `asana-4.0.2/test/test_team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_gid_projects_body.py` & `asana-4.0.2/test/test_team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_gid_remove_user_body.py` & `asana-4.0.2/test/test_team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_membership_base.py` & `asana-4.0.2/test/test_team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_membership_compact.py` & `asana-4.0.2/test/test_team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_membership_response.py` & `asana-4.0.2/test/test_team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_membership_response_array.py` & `asana-4.0.2/test/test_team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_membership_response_data.py` & `asana-4.0.2/test/test_team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_memberships_api.py` & `asana-4.0.2/test/test_team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_remove_user_request.py` & `asana-4.0.2/test/test_team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_request.py` & `asana-4.0.2/test/test_team_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_response.py` & `asana-4.0.2/test/test_team_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_response_array.py` & `asana-4.0.2/test/test_team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_response_data.py` & `asana-4.0.2/test/test_team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_team_response_organization.py` & `asana-4.0.2/test/test_team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_teams_api.py` & `asana-4.0.2/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_teams_body.py` & `asana-4.0.2/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_teams_team_gid_body.py` & `asana-4.0.2/test/test_teams_team_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_template_role.py` & `asana-4.0.2/test/test_template_role.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_period_base.py` & `asana-4.0.2/test/test_time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_period_compact.py` & `asana-4.0.2/test/test_time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_period_response.py` & `asana-4.0.2/test/test_time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_period_response_array.py` & `asana-4.0.2/test/test_time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_period_response_data.py` & `asana-4.0.2/test/test_time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_periods_api.py` & `asana-4.0.2/test/test_time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entries_api.py` & `asana-4.0.2/test/test_time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entries_time_tracking_entry_gid_body.py` & `asana-4.0.2/test/test_time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entry_base.py` & `asana-4.0.2/test/test_time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entry_base_data.py` & `asana-4.0.2/test/test_time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entry_compact.py` & `asana-4.0.2/test/test_time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_time_tracking_entry_compact_array.py` & `asana-4.0.2/test/test_time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_typeahead_api.py` & `asana-4.0.2/test/test_typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_update_time_tracking_entry_request.py` & `asana-4.0.2/test/test_update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_base.py` & `asana-4.0.2/test/test_user_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_base_response.py` & `asana-4.0.2/test/test_user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_base_response_data.py` & `asana-4.0.2/test/test_user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_base_response_photo.py` & `asana-4.0.2/test/test_user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_compact.py` & `asana-4.0.2/test/test_user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_request.py` & `asana-4.0.2/test/test_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_response.py` & `asana-4.0.2/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_response_array.py` & `asana-4.0.2/test/test_user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_response_data.py` & `asana-4.0.2/test/test_user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_list_base.py` & `asana-4.0.2/test/test_user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_list_compact.py` & `asana-4.0.2/test/test_user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_list_request.py` & `asana-4.0.2/test/test_user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_list_response.py` & `asana-4.0.2/test/test_user_task_list_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_list_response_data.py` & `asana-4.0.2/test/test_user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_user_task_lists_api.py` & `asana-4.0.2/test/test_user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_users_api.py` & `asana-4.0.2/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_compact.py` & `asana-4.0.2/test/test_webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_compact_resource.py` & `asana-4.0.2/test/test_webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_filter.py` & `asana-4.0.2/test/test_webhook_filter.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_request.py` & `asana-4.0.2/test/test_webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_request_filters.py` & `asana-4.0.2/test/test_webhook_request_filters.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_response.py` & `asana-4.0.2/test/test_webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_response_array.py` & `asana-4.0.2/test/test_webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_response_data.py` & `asana-4.0.2/test/test_webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhook_update_request.py` & `asana-4.0.2/test/test_webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhooks_api.py` & `asana-4.0.2/test/test_webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhooks_body.py` & `asana-4.0.2/test/test_webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_webhooks_webhook_gid_body.py` & `asana-4.0.2/test/test_webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_add_user_request.py` & `asana-4.0.2/test/test_workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_base.py` & `asana-4.0.2/test/test_workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_compact.py` & `asana-4.0.2/test/test_workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_gid_add_user_body.py` & `asana-4.0.2/test/test_workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_gid_projects_body.py` & `asana-4.0.2/test/test_workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_gid_remove_user_body.py` & `asana-4.0.2/test/test_workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_gid_tags_body.py` & `asana-4.0.2/test/test_workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_base.py` & `asana-4.0.2/test/test_workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_compact.py` & `asana-4.0.2/test/test_workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_request.py` & `asana-4.0.2/test/test_workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_response.py` & `asana-4.0.2/test/test_workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_response_array.py` & `asana-4.0.2/test/test_workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_response_data.py` & `asana-4.0.2/test/test_workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_response_user_task_list.py` & `asana-4.0.2/test/test_workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_membership_response_vacation_dates.py` & `asana-4.0.2/test/test_workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_memberships_api.py` & `asana-4.0.2/test/test_workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_remove_user_request.py` & `asana-4.0.2/test/test_workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_request.py` & `asana-4.0.2/test/test_workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_response.py` & `asana-4.0.2/test/test_workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_response_array.py` & `asana-4.0.2/test/test_workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspace_response_data.py` & `asana-4.0.2/test/test_workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspaces_api.py` & `asana-4.0.2/test/test_workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana-4.0.1/test/test_workspaces_workspace_gid_body.py` & `asana-4.0.2/test/test_workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

