# Comparing `tmp/demisto-py-3.2.9.tar.gz` & `tmp/demisto_py-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demisto-py-3.2.9.tar", last modified: Sun Apr 16 07:08:54 2023, max compression
+gzip compressed data, was "demisto_py-3.3.0.tar", max compression
```

## Comparing `demisto-py-3.2.9.tar` & `demisto_py-3.3.0.tar`

### file list

```diff
@@ -1,413 +1,188 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.710667 demisto-py-3.2.9/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/.circleci/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1023 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.circleci/config.yml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      162 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.flake8
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/.github/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      497 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      340 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.github/pull_request_template.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1156 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.gitignore
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/.idea/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.idea/vcs.xml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      119 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.lgtm.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-04-16 07:03:54.000000 demisto-py-3.2.9/.swagger-codegen-ignore
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5494 2023-04-16 07:03:54.000000 demisto-py-3.2.9/CHANGELOG.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-16 07:03:54.000000 demisto-py-3.2.9/LICENSE
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8296 2023-04-16 07:08:54.710667 demisto-py-3.2.9/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7550 2023-04-16 07:03:54.000000 demisto-py-3.2.9/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/demisto_client/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14912 2023-04-16 07:03:54.000000 demisto-py-3.2.9/demisto_client/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/demisto_client/demisto_api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      120 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15394 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.686668 demisto-py-3.2.9/demisto_client/demisto_api/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   302450 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/api/default_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26965 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9985 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/configuration.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.698668 demisto-py-3.2.9/demisto_client/demisto_api/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15151 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5253 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/advance_arg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7431 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/arg_atomic_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4001 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/arg_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5346 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/arg_transformer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10358 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/argument.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3921 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/array_positions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7111 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/attachment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9340 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/audit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5217 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/audit_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31379 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19235 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10406 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6473 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_filter_wrapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7276 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11959 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6493 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/common_fields.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6751 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/complex_arg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3921 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/config_data_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9067 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/config_field.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    47601 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/create_incident_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/custom_fields.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9801 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/d_bot_score.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16016 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/dashboard.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8202 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/data_collection_form.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6751 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/date_range.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7677 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/date_range_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4645 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/delete_evidence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/docker_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4711 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/docker_images_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5278 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/download_entry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3897 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/duration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/ending_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39209 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3917 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry_category.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6694 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry_history.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5771 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry_reputation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/entry_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16972 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/evidence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6942 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/evidence_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/evidences.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5543 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/evidences_filter_wrapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5423 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/evidences_search_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3929 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_policy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3961 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_settings_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9884 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18606 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4016 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7299 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicators_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/field_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5296 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/field_mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4043 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/field_term_location_map.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9387 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/file_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3909 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/filter_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3929 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/filter_operator_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10778 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/form_display.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9105 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/generic_indicator_update_batch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13550 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/generic_string_date_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9511 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/generic_string_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10615 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/grid_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5827 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3969 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9137 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/human_cron.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6273 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/important.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    44785 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33707 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_field.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36806 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6290 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_search_response_wrapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3921 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22837 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46847 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incident_wrapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/incidents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6906 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_context.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5303 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_edit_bulk_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17356 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5372 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5264 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inline_response200.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8045 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/insight_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21755 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/instance_classifier.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/integration_script.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6658 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_assignee.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6512 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_due.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12791 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_task_complete_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_task_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10242 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/inv_task_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33853 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22815 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27014 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16597 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3969 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49701 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7885 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_tasks_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5471 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_search_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3933 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4015 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/investigations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21442 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/ioc_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/ioc_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5003 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18544 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/layout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5784 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/layout_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9344 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/layout_field.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13386 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/layout_section.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/locations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6002 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/mapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3903 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/module_args.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28332 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/module_configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6537 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/new_docker_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4594 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/new_docker_image_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10623 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/notifiable_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6436 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/notify_timings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5369 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/operator_argument.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5654 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/order.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/output_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7649 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/period.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32551 2023-04-16 07:08:46.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6574 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_input.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4016 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6085 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4022 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_outputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26685 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3913 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_view.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11263 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/question.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/quiet_mode.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3927 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/raw_feed_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/raw_message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3909 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/reliability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3909 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/remote_repos.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34892 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6453 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/report_automation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/report_fields_decoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6466 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/report_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38649 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/reputation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3933 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/reputation_calc_alg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6639 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/reputation_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5462 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/reputations_with_errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/run_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19825 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/script_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3917 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/script_sub_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3913 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/script_target.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/script_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5463 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/search_incidents_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11966 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/section.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9897 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/section_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3897 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/severity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5540 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/sla.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3897 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/sla_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5524 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/stats_query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5456 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/stats_text_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5309 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/stats_trends_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15471 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4680 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/system_agent.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5322 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task_condition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9670 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task_loop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3897 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3897 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/task_view.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4009 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/term_location_map.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8964 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/terminal_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3909 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/timer_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5341 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/timer_trigger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3949 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/transformer_operator_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12486 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/update_data_batch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7832 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/update_entry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6558 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/update_entry_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10200 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/update_indicator_reputation_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5387 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/update_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6019 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/uploaded_entry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5085 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19555 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/widget.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8388 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/widget_cell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3998 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/models/widget_cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15344 2023-04-16 07:08:47.000000 demisto-py-3.2.9/demisto_client/demisto_api/rest.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.698668 demisto-py-3.2.9/demisto_py.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8296 2023-04-16 07:08:54.000000 demisto-py-3.2.9/demisto_py.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14388 2023-04-16 07:08:54.000000 demisto-py-3.2.9/demisto_py.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 07:08:54.000000 demisto-py-3.2.9/demisto_py.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      100 2023-04-16 07:08:54.000000 demisto-py-3.2.9/demisto_py.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       15 2023-04-16 07:08:54.000000 demisto-py-3.2.9/demisto_py.egg-info/top_level.txt
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      654 2023-04-16 07:03:54.000000 demisto-py-3.2.9/deploy.sh
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.710667 demisto-py-3.2.9/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      380 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AdvanceArg.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ArgAtomicFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ArgFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ArgTransformer.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Argument.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ArrayPositions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Attachment.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Audit.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      375 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AuditResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2262 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AutomationScript.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1296 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AutomationScriptAPI.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      903 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AutomationScriptFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      498 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AutomationScriptFilterWrapper.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      535 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/AutomationScriptResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Command.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/CommonFields.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ComplexArg.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ConfigDataType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      629 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ConfigField.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4067 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/CreateIncidentRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/CustomFields.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DBotScore.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1082 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Dashboard.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DataCollectionForm.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DateRange.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      544 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DateRangeFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)   124629 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DefaultApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      326 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DeleteEvidence.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DockerImage.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DockerImagesResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      364 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/DownloadEntry.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Duration.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EndingType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3536 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Entry.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EntryCategory.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EntryHistory.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EntryReputation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EntryTask.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EntryType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Evidence.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      587 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EvidenceData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Evidences.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EvidencesFilterWrapper.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/EvidencesSearchResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ExpirationPolicy.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ExpirationSettingsSource.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ExpirationSource.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FeedIndicator.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FeedIndicators.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FeedIndicatorsRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FieldGroup.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FieldMapping.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FieldTermLocationMap.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FileMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FilterCache.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FilterOperatorID.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      683 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/FormDisplay.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/GenericIndicatorUpdateBatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/GenericStringDateFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/GenericStringFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/GridColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      457 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Group.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Groups.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/HumanCron.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Important.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4084 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Incident.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2233 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentField.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentSearchResponseWrapper.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentStatus.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4103 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IncidentWrapper.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Incidents.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IndicatorContext.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      370 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IndicatorEditBulkResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1491 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IndicatorFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IndicatorResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InlineResponse200.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InsightCache.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1437 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InstanceClassifier.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IntegrationScript.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      447 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvPlaybookAssignee.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      444 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvPlaybookDue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvPlaybookTaskCompleteData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvPlaybookTaskData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvTaskInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3525 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Investigation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1785 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2183 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationPlaybook.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1313 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationPlaybookData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationPlaybookState.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3820 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationPlaybookTask.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      577 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationPlaybookTasksAPI.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationSearchResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationStatus.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      286 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/InvestigationType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Investigations.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1464 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IocObject.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/IocObjects.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      347 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Label.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Layout.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/LayoutAPI.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/LayoutField.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/LayoutSection.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Location.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Locations.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Mapper.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ModuleArgs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1779 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ModuleConfiguration.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/NewDockerImage.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      327 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/NewDockerImageResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      830 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/NotifiableItem.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/NotifyTimings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/OperatorArgument.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Order.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Output.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/OutputType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Period.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2504 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Playbook.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookInput.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookOutput.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookOutputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookTask.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/PlaybookView.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      798 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Question.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/QuietMode.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-04-16 07:08:48.000000 demisto-py-3.2.9/docs/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/RawFeedIndicator.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/RawMessage.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Reliability.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/RemoteRepos.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2369 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Report.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReportAutomation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReportFieldsDecoder.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReportQuery.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Reputation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      286 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReputationCalcAlg.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReputationData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      400 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ReputationsWithErrors.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/RunStatus.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      382 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/SLA.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/SLAState.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ScriptAPI.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ScriptSubType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ScriptTarget.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/ScriptType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/SearchIncidentsData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      844 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Section.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/SectionItem.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Severity.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/StatsQueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/StatsTextResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/StatsTrendsResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/System.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/SystemAgent.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Task.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TaskCondition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      681 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TaskLoop.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TaskState.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TaskType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TaskView.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TermLocationMap.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TerminalOptions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TimerAction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TimerTrigger.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/TransformerOperatorID.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UpdateDataBatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      549 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UpdateEntry.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      447 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UpdateEntryTags.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      646 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UpdateIndicatorReputationData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      375 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UpdateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/UploadedEntry.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Version.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/Widget.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      576 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/WidgetCell.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      280 2023-04-16 07:08:47.000000 demisto-py-3.2.9/docs/WidgetCells.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.710667 demisto-py-3.2.9/examples/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      840 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/batch_util_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2651 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/create_incident_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1023 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/download_file_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      904 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/incidents_search_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/indicators_search_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1331 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/update_automation_example.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      770 2023-04-16 07:03:54.000000 demisto-py-3.2.9/examples/widget_upload.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    10023 2023-04-16 07:03:54.000000 demisto-py-3.2.9/gen-code.sh
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       99 2023-04-16 07:03:54.000000 demisto-py-3.2.9/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   284515 2023-04-16 07:03:54.000000 demisto-py-3.2.9/server_api_swagger.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2023-04-16 07:08:54.710667 demisto-py-3.2.9/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-04-16 07:03:54.000000 demisto-py-3.2.9/setup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      174 2023-04-16 07:03:54.000000 demisto-py-3.2.9/swagger-config.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       52 2023-04-16 07:03:54.000000 demisto-py-3.2.9/test-requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.710667 demisto-py-3.2.9/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      688 2023-04-16 07:03:54.000000 demisto-py-3.2.9/tests/examples_test.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27611 2023-04-16 07:03:54.000000 demisto-py-3.2.9/tests/mocks_test.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 07:08:54.710667 demisto-py-3.2.9/tests_data/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7685 2023-04-16 07:03:54.000000 demisto-py-3.2.9/tests_data/layout-details-test-V2.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7688 2023-04-16 07:03:54.000000 demisto-py-3.2.9/tests_data/layoutscontainer-test.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2023-04-16 07:03:54.000000 demisto-py-3.2.9/tox.ini
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      570 2023-04-16 07:03:54.000000 demisto-py-3.2.9/verify.sh
+-rw-r--r--   0        0        0    11357 2023-08-02 11:59:08.839490 demisto_py-3.3.0/LICENSE
+-rw-r--r--   0        0        0     7587 2023-08-02 11:59:08.839490 demisto_py-3.3.0/README.md
+-rw-r--r--   0        0        0    15398 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/README.md
+-rw-r--r--   0        0        0    15394 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/__init__.py
+-rw-r--r--   0        0        0      153 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/api/__init__.py
+-rw-r--r--   0        0        0   302450 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/api/default_api.py
+-rw-r--r--   0        0        0    27616 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/api_client.py
+-rw-r--r--   0        0        0     9985 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/configuration.py
+-rw-r--r--   0        0        0    15151 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/models/__init__.py
+-rw-r--r--   0        0        0     5253 2023-08-02 11:59:08.839490 demisto_py-3.3.0/demisto_client/demisto_api/models/advance_arg.py
+-rw-r--r--   0        0        0     7431 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/arg_atomic_filter.py
+-rw-r--r--   0        0        0     4001 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/arg_filter.py
+-rw-r--r--   0        0        0     5346 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/arg_transformer.py
+-rw-r--r--   0        0        0    10358 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/argument.py
+-rw-r--r--   0        0        0     3921 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/array_positions.py
+-rw-r--r--   0        0        0     7111 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/attachment.py
+-rw-r--r--   0        0        0     9340 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/audit.py
+-rw-r--r--   0        0        0     5217 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/audit_result.py
+-rw-r--r--   0        0        0    31379 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script.py
+-rw-r--r--   0        0        0    19235 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_api.py
+-rw-r--r--   0        0        0    10406 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_filter.py
+-rw-r--r--   0        0        0     6473 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_filter_wrapper.py
+-rw-r--r--   0        0        0     7276 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_result.py
+-rw-r--r--   0        0        0    11959 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/command.py
+-rw-r--r--   0        0        0     6493 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/common_fields.py
+-rw-r--r--   0        0        0     6751 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/complex_arg.py
+-rw-r--r--   0        0        0     3921 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/config_data_type.py
+-rw-r--r--   0        0        0     9067 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/config_field.py
+-rw-r--r--   0        0        0    47601 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/create_incident_request.py
+-rw-r--r--   0        0        0     3911 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/custom_fields.py
+-rw-r--r--   0        0        0     9801 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/d_bot_score.py
+-rw-r--r--   0        0        0    16016 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/dashboard.py
+-rw-r--r--   0        0        0     8202 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/data_collection_form.py
+-rw-r--r--   0        0        0     6751 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/date_range.py
+-rw-r--r--   0        0        0     7677 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/date_range_filter.py
+-rw-r--r--   0        0        0     4645 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/delete_evidence.py
+-rw-r--r--   0        0        0     7705 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/docker_image.py
+-rw-r--r--   0        0        0     4711 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/docker_images_result.py
+-rw-r--r--   0        0        0     5278 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/download_entry.py
+-rw-r--r--   0        0        0     3897 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/duration.py
+-rw-r--r--   0        0        0     3905 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/ending_type.py
+-rw-r--r--   0        0        0    39209 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry.py
+-rw-r--r--   0        0        0     3917 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry_category.py
+-rw-r--r--   0        0        0     6694 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry_history.py
+-rw-r--r--   0        0        0     5771 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry_reputation.py
+-rw-r--r--   0        0        0     6637 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry_task.py
+-rw-r--r--   0        0        0     3901 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/entry_type.py
+-rw-r--r--   0        0        0    16972 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/evidence.py
+-rw-r--r--   0        0        0     6942 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/evidence_data.py
+-rw-r--r--   0        0        0     3985 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/evidences.py
+-rw-r--r--   0        0        0     5543 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/evidences_filter_wrapper.py
+-rw-r--r--   0        0        0     5423 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/evidences_search_response.py
+-rw-r--r--   0        0        0     3929 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_policy.py
+-rw-r--r--   0        0        0     3961 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_settings_source.py
+-rw-r--r--   0        0        0     9884 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_source.py
+-rw-r--r--   0        0        0    18606 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicator.py
+-rw-r--r--   0        0        0     4016 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicators.py
+-rw-r--r--   0        0        0     7299 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicators_request.py
+-rw-r--r--   0        0        0     3905 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/field_group.py
+-rw-r--r--   0        0        0     5296 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/field_mapping.py
+-rw-r--r--   0        0        0     4043 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/field_term_location_map.py
+-rw-r--r--   0        0        0     9387 2023-08-02 11:59:08.843490 demisto_py-3.3.0/demisto_client/demisto_api/models/file_metadata.py
+-rw-r--r--   0        0        0     3909 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/filter_cache.py
+-rw-r--r--   0        0        0     3929 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/filter_operator_id.py
+-rw-r--r--   0        0        0    10778 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/form_display.py
+-rw-r--r--   0        0        0     9105 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/generic_indicator_update_batch.py
+-rw-r--r--   0        0        0    13550 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/generic_string_date_filter.py
+-rw-r--r--   0        0        0     9511 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/generic_string_filter.py
+-rw-r--r--   0        0        0    10615 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/grid_column.py
+-rw-r--r--   0        0        0     5827 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/group.py
+-rw-r--r--   0        0        0     3969 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/groups.py
+-rw-r--r--   0        0        0     9137 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/human_cron.py
+-rw-r--r--   0        0        0     6273 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/important.py
+-rw-r--r--   0        0        0    44785 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident.py
+-rw-r--r--   0        0        0    33707 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_field.py
+-rw-r--r--   0        0        0    36806 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_filter.py
+-rw-r--r--   0        0        0     6290 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_search_response_wrapper.py
+-rw-r--r--   0        0        0     3921 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_status.py
+-rw-r--r--   0        0        0    22837 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_type.py
+-rw-r--r--   0        0        0    46847 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incident_wrapper.py
+-rw-r--r--   0        0        0     3901 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/incidents.py
+-rw-r--r--   0        0        0     6906 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_context.py
+-rw-r--r--   0        0        0     5303 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_edit_bulk_response.py
+-rw-r--r--   0        0        0    17356 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_filter.py
+-rw-r--r--   0        0        0     5372 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_result.py
+-rw-r--r--   0        0        0     5264 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inline_response200.py
+-rw-r--r--   0        0        0     8045 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/insight_cache.py
+-rw-r--r--   0        0        0    21755 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/instance_classifier.py
+-rw-r--r--   0        0        0    12255 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/integration_script.py
+-rw-r--r--   0        0        0     6658 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_assignee.py
+-rw-r--r--   0        0        0     6512 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_due.py
+-rw-r--r--   0        0        0    12791 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_task_complete_data.py
+-rw-r--r--   0        0        0     9453 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_task_data.py
+-rw-r--r--   0        0        0    10242 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/inv_task_info.py
+-rw-r--r--   0        0        0    33853 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation.py
+-rw-r--r--   0        0        0    22815 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_filter.py
+-rw-r--r--   0        0        0    27014 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook.py
+-rw-r--r--   0        0        0    16597 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_data.py
+-rw-r--r--   0        0        0     3969 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_state.py
+-rw-r--r--   0        0        0    49701 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_task.py
+-rw-r--r--   0        0        0     7885 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_tasks_api.py
+-rw-r--r--   0        0        0     5471 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_search_response.py
+-rw-r--r--   0        0        0     3941 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_status.py
+-rw-r--r--   0        0        0     3933 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_type.py
+-rw-r--r--   0        0        0     4015 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/investigations.py
+-rw-r--r--   0        0        0    21442 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/ioc_object.py
+-rw-r--r--   0        0        0     3992 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/ioc_objects.py
+-rw-r--r--   0        0        0     5003 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/label.py
+-rw-r--r--   0        0        0    18544 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/layout.py
+-rw-r--r--   0        0        0     5784 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/layout_api.py
+-rw-r--r--   0        0        0     9344 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/layout_field.py
+-rw-r--r--   0        0        0    13386 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/layout_section.py
+-rw-r--r--   0        0        0     6807 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/location.py
+-rw-r--r--   0        0        0     3985 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/locations.py
+-rw-r--r--   0        0        0     6002 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/mapper.py
+-rw-r--r--   0        0        0     3903 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/module_args.py
+-rw-r--r--   0        0        0    28332 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/module_configuration.py
+-rw-r--r--   0        0        0     6537 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/new_docker_image.py
+-rw-r--r--   0        0        0     4594 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/new_docker_image_result.py
+-rw-r--r--   0        0        0    10623 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/notifiable_item.py
+-rw-r--r--   0        0        0     6436 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/notify_timings.py
+-rw-r--r--   0        0        0     5369 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/operator_argument.py
+-rw-r--r--   0        0        0     5654 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/order.py
+-rw-r--r--   0        0        0     6852 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/output.py
+-rw-r--r--   0        0        0     3905 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/output_type.py
+-rw-r--r--   0        0        0     7649 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/period.py
+-rw-r--r--   0        0        0    32551 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook.py
+-rw-r--r--   0        0        0     6574 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_input.py
+-rw-r--r--   0        0        0     4016 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_inputs.py
+-rw-r--r--   0        0        0     6085 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_output.py
+-rw-r--r--   0        0        0     4022 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_outputs.py
+-rw-r--r--   0        0        0    26685 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_task.py
+-rw-r--r--   0        0        0     3913 2023-08-02 11:59:08.847490 demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_view.py
+-rw-r--r--   0        0        0    11263 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/question.py
+-rw-r--r--   0        0        0     3901 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/quiet_mode.py
+-rw-r--r--   0        0        0     3927 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/raw_feed_indicator.py
+-rw-r--r--   0        0        0     3905 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/raw_message.py
+-rw-r--r--   0        0        0     3909 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/reliability.py
+-rw-r--r--   0        0        0     3909 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/remote_repos.py
+-rw-r--r--   0        0        0    34892 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/report.py
+-rw-r--r--   0        0        0     6453 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/report_automation.py
+-rw-r--r--   0        0        0     5171 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/report_fields_decoder.py
+-rw-r--r--   0        0        0     6466 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/report_query.py
+-rw-r--r--   0        0        0    38649 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/reputation.py
+-rw-r--r--   0        0        0     3933 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/reputation_calc_alg.py
+-rw-r--r--   0        0        0     6639 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/reputation_data.py
+-rw-r--r--   0        0        0     5462 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/reputations_with_errors.py
+-rw-r--r--   0        0        0     3901 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/run_status.py
+-rw-r--r--   0        0        0    19825 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/script_api.py
+-rw-r--r--   0        0        0     3917 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/script_sub_type.py
+-rw-r--r--   0        0        0     3913 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/script_target.py
+-rw-r--r--   0        0        0     3905 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/script_type.py
+-rw-r--r--   0        0        0     5463 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/search_incidents_data.py
+-rw-r--r--   0        0        0    11966 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/section.py
+-rw-r--r--   0        0        0     9897 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/section_item.py
+-rw-r--r--   0        0        0     3897 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/severity.py
+-rw-r--r--   0        0        0     5540 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/sla.py
+-rw-r--r--   0        0        0     3897 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/sla_state.py
+-rw-r--r--   0        0        0     5524 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/stats_query_response.py
+-rw-r--r--   0        0        0     5456 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/stats_text_response.py
+-rw-r--r--   0        0        0     5309 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/stats_trends_response.py
+-rw-r--r--   0        0        0    15471 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/system.py
+-rw-r--r--   0        0        0     4680 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/system_agent.py
+-rw-r--r--   0        0        0    15422 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task.py
+-rw-r--r--   0        0        0     5322 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task_condition.py
+-rw-r--r--   0        0        0     9670 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task_loop.py
+-rw-r--r--   0        0        0     3901 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task_state.py
+-rw-r--r--   0        0        0     3897 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task_type.py
+-rw-r--r--   0        0        0     3897 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/task_view.py
+-rw-r--r--   0        0        0     4009 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/term_location_map.py
+-rw-r--r--   0        0        0     8964 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/terminal_options.py
+-rw-r--r--   0        0        0     3909 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/timer_action.py
+-rw-r--r--   0        0        0     5341 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/timer_trigger.py
+-rw-r--r--   0        0        0     3949 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/transformer_operator_id.py
+-rw-r--r--   0        0        0    12486 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/update_data_batch.py
+-rw-r--r--   0        0        0     7832 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/update_entry.py
+-rw-r--r--   0        0        0     6558 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/update_entry_tags.py
+-rw-r--r--   0        0        0    10200 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/update_indicator_reputation_data.py
+-rw-r--r--   0        0        0     5387 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/update_response.py
+-rw-r--r--   0        0        0     6019 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/uploaded_entry.py
+-rw-r--r--   0        0        0     5085 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/version.py
+-rw-r--r--   0        0        0    19555 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/widget.py
+-rw-r--r--   0        0        0     8388 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/widget_cell.py
+-rw-r--r--   0        0        0     3998 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/models/widget_cells.py
+-rw-r--r--   0        0        0    15452 2023-08-02 11:59:08.851490 demisto_py-3.3.0/demisto_client/demisto_api/rest.py
+-rw-r--r--   0        0        0     1176 2023-08-02 11:59:08.859490 demisto_py-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8662 1970-01-01 00:00:00.000000 demisto_py-3.3.0/PKG-INFO
```

### Comparing `demisto-py-3.2.9/LICENSE` & `demisto_py-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/PKG-INFO` & `demisto_py-3.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: demisto-py
-Version: 3.2.9
-Summary: A Python library for the Demisto API
-Home-page: https://github.com/demisto/demisto-py
-Author-email: 
-License: Apache Software License
-Keywords: Swagger,Demisto API
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/demisto-py.svg)](https://badge.fury.io/py/demisto-py)
 [![CircleCI](https://circleci.com/gh/demisto/demisto-py/tree/master.svg?style=svg)](https://circleci.com/gh/demisto/demisto-py/tree/master)
 
 # Demisto Client for Python
 
 A Python library for the Demisto API.
 
@@ -40,19 +19,20 @@
 2. Click the **Generate Your Key** button.
 
 To avoid hard coding configurations in your code, it is possible to specify configuration params
 as the following environment variables (env variables will be used if parameters are not specified):
 
 * DEMISTO_BASE_URL
 * DEMISTO_API_KEY
+* DEMISTO_ADVANCED_API_KEY
 * DEMISTO_USERNAME
 * DEMISTO_PASSWORD
 * DEMISTO_HTTP_HEADERS (must be in the form of: header1=value1,header2=value2,header3=value3,...headerN=valueN)
 * DEMISTO_VERIFY_SSL (true/false. Default: true)
-* XSIAM_AUTH_ID (for Cortex XSIAM only. If set, Cortex XSIAM API will be used)
+* DEMISTO_API_KEY_ID (for Cortex XSIAM only. If set, Cortex XSIAM API will be used)
 * SSL_CERT_FILE (specify an alternate certificate bundle)
 
 ### 2. Create a Demisto client instance with the api-key and server-url
 
 ```python
 import demisto_client
 
@@ -64,15 +44,15 @@
 
 ```
 
 **For Cortex XSIAM, we need to set the auth_id**
 ```python
 import demisto_client
 
-# Also possible to set env variables: DEMISTO_API_KEY, DEMISTO_BASE_URL and XSIAM_AUTH_ID
+# Also possible to set env variables: DEMISTO_API_KEY, DEMISTO_BASE_URL and DEMISTO_API_KEY_ID
 api_key = 'YOUR_API_KEY'
 auth_id = 'THE AUTHORIZATION ID'
 host = 'https://YOUR_XSIAM_HOST'
 
 api_instance = demisto_client.configure(base_url=host, api_key=api_key, auth_id=auth_id)
 
 ```
@@ -242,9 +222,7 @@
 * Update GitHub releases: go to [tags page](https://github.com/demisto/demisto-py/tags) and for the relevant tag choose from the right drop down menu: `Create release`. Name the release the same as the tag. Copy the text from previous releases for the description.
 
 Congratulations! The release is now public.
 
 ## License
 
 Apache 2.0 - See [LICENSE](LICENSE) for more information.
-
-
```

### Comparing `demisto-py-3.2.9/README.md` & `demisto_py-3.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: demisto-py
+Version: 3.3.0
+Summary: "A Python library for the Demisto SDK"
+Home-page: https://github.com/demisto/demisto-py
+License: Apache Software License
+Keywords: Swagger,Demisto API
+Author: Demisto
+Requires-Python: >=3.8.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: certifi (>=2017.4.17)
+Requires-Dist: python-dateutil (>=2.5.3)
+Requires-Dist: setuptools (>=21.0.0)
+Requires-Dist: six (>=1.10)
+Requires-Dist: tzlocal (>=4.0.0,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.7)
+Description-Content-Type: text/markdown
+
 [![PyPI version](https://badge.fury.io/py/demisto-py.svg)](https://badge.fury.io/py/demisto-py)
 [![CircleCI](https://circleci.com/gh/demisto/demisto-py/tree/master.svg?style=svg)](https://circleci.com/gh/demisto/demisto-py/tree/master)
 
 # Demisto Client for Python
 
 A Python library for the Demisto API.
 
@@ -19,19 +47,20 @@
 2. Click the **Generate Your Key** button.
 
 To avoid hard coding configurations in your code, it is possible to specify configuration params
 as the following environment variables (env variables will be used if parameters are not specified):
 
 * DEMISTO_BASE_URL
 * DEMISTO_API_KEY
+* DEMISTO_ADVANCED_API_KEY
 * DEMISTO_USERNAME
 * DEMISTO_PASSWORD
 * DEMISTO_HTTP_HEADERS (must be in the form of: header1=value1,header2=value2,header3=value3,...headerN=valueN)
 * DEMISTO_VERIFY_SSL (true/false. Default: true)
-* XSIAM_AUTH_ID (for Cortex XSIAM only. If set, Cortex XSIAM API will be used)
+* DEMISTO_API_KEY_ID (for Cortex XSIAM only. If set, Cortex XSIAM API will be used)
 * SSL_CERT_FILE (specify an alternate certificate bundle)
 
 ### 2. Create a Demisto client instance with the api-key and server-url
 
 ```python
 import demisto_client
 
@@ -43,15 +72,15 @@
 
 ```
 
 **For Cortex XSIAM, we need to set the auth_id**
 ```python
 import demisto_client
 
-# Also possible to set env variables: DEMISTO_API_KEY, DEMISTO_BASE_URL and XSIAM_AUTH_ID
+# Also possible to set env variables: DEMISTO_API_KEY, DEMISTO_BASE_URL and DEMISTO_API_KEY_ID
 api_key = 'YOUR_API_KEY'
 auth_id = 'THE AUTHORIZATION ID'
 host = 'https://YOUR_XSIAM_HOST'
 
 api_instance = demisto_client.configure(base_url=host, api_key=api_key, auth_id=auth_id)
 
 ```
@@ -221,7 +250,8 @@
 * Update GitHub releases: go to [tags page](https://github.com/demisto/demisto-py/tags) and for the relevant tag choose from the right drop down menu: `Create release`. Name the release the same as the tag. Copy the text from previous releases for the description.
 
 Congratulations! The release is now public.
 
 ## License
 
 Apache 2.0 - See [LICENSE](LICENSE) for more information.
+
```

### Comparing `demisto-py-3.2.9/demisto_client/__init__.py` & `demisto_py-3.3.0/demisto_client/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,60 +18,59 @@
     # package is not installed
     __version__ = 'dev'
 
 
 DEMISTO_HTTP_HEADERS_REGEX_PATTERN = r'^([\w-]+=[^=,\n]+)(,[\w-]+=[^=,\n]+)*$'
 
 
-def configure(base_url=None, api_key=None, verify_ssl=None, proxy=None, username=None, password=None,
+def configure(base_url=None, api_key=None, advanced_api_key=None, verify_ssl=None, proxy=None, username=None, password=None,
               ssl_ca_cert=None, debug=False, connection_pool_maxsize=None, auth_id=None, additional_headers=None):
     """
     This wrapper provides an easier to use method of configuring the API client. The base
     Configuration method is still exposed if you wish to further configure the API Client.
 
     To avoid hard coding configurations in your code, it is possible to specify configuration params
     as the following environment variables (env variables will be used if parameters are not specified):
 
     * DEMISTO_BASE_URL
     * DEMISTO_API_KEY
+    * DEMISTO_ADVANCED_API_KEY
     * DEMISTO_USERNAME
     * DEMISTO_PASSWORD
     * DEMISTO_VERIFY_SSL (true/false. Default: true)
     * DEMISTO_HTTP_HEADERS (must be in the form of: header1=value1,header2=value2,header3=value3,...headerN=valueN)
-    * XSIAM_AUTH_ID
+    * DEMISTO_API_KEY_ID
     * SSL_CERT_FILE (specify an alternate certificate bundle)
     * DEMISTO_CONNECTION_POOL_MAXSIZE (specify a connection pool max size)
     * HTTP_PROXY or HTTPS_PROXY (If you are using a proxy)
 
     :param base_url: str - Base url of your Demisto instance.
     :param api_key: str - API key generated by your instance.
+    :param advanced_api_key: str - Advanced API key generated by your instance.
     :param username: str - Username of the user account.
     :param password: str - Password of the user account.
     :param verify_ssl: bool - Indicates if valid SSLs are required for connection. If not specified (None)
         will default to True.
     :param proxy: str - The URL of the proxy to be used.
     :param ssl_ca_cert: str - specify an alternate certificate bundle
     :param debug: bool - Include verbose logging.
     :param connection_pool_maxsize: int - specify a connection max pool size
     :param auth_id: str - api_key_id only for the xsiam
     :param additional_headers: dict - any additional headers to send to every http request to demisto.
     :return: Returns an API client configuration identical to the Configuration() method.
     """
-    if base_url is None:
-        base_url = os.getenv('DEMISTO_BASE_URL')
-        if not base_url:
-            raise RuntimeError('the DEMISTO_BASE_URL value is not set.')
-    if api_key is None:
-        api_key = os.getenv('DEMISTO_API_KEY')
-    if auth_id is None:
-        auth_id = os.getenv('XSIAM_AUTH_ID')
-    if username is None:
-        username = os.getenv('DEMISTO_USERNAME')
-    if password is None:
-        password = os.getenv('DEMISTO_PASSWORD')
+    base_url = base_url or os.getenv('DEMISTO_BASE_URL')
+    if not base_url:
+        raise RuntimeError('the DEMISTO_BASE_URL value is not set.')
+    api_key = api_key or os.getenv('DEMISTO_API_KEY')
+    auth_id = auth_id or os.getenv('DEMISTO_API_KEY_ID') or os.getenv('XSIAM_AUTH_ID')
+    username = username or os.getenv('DEMISTO_USERNAME')
+    password = password or os.getenv('DEMISTO_PASSWORD')
+    advanced_api_key = advanced_api_key or os.getenv('DEMISTO_ADVANCED_API_KEY')
+
     if additional_headers is None:
         if headers := os.getenv('DEMISTO_HTTP_HEADERS'):
             if re.match(r'^ *$', headers):  # catch any case of empty string
                 additional_headers = {}
             elif re.match(DEMISTO_HTTP_HEADERS_REGEX_PATTERN, headers):
                 additional_headers = dict(header.strip().split('=') for header in headers.split(','))
             else:
@@ -100,25 +99,30 @@
                 err_msg = ('DEMISTO_CONNECTION_POOL_MAXSIZE env variable should be set to a number'
                            f' but instead received "{connection_pool_maxsize}"')
                 raise ValueError(err_msg)
             else:
                 connection_pool_maxsize = int(connection_pool_maxsize)
     if not base_url:
         raise ValueError('You must specify base_url either as a parameter or via env variable: DEMISTO_BASE_URL')
-    if not api_key and not username:
-        raise ValueError('You must specify either api_key or username/password either as parameters or use env variables:\n'
+    if not api_key and not username and not advanced_api_key:
+        raise ValueError('You must specify either api_key or advanced_api_key or username/password either as parameters or use env variables:\n'
                          '* DEMISTO_API_KEY\n'
+                         '* DEMISTO_ADVANCED_API_KEY\n'
                          '* DEMISTO_USERNAME\n'
                          '* DEMISTO_PASSWORD'
                          )
-    if auth_id and not api_key:
-        raise ValueError('You must specify either api_key or use env variable DEMISTO_API_KEY to use Cortex XSIAM api, '
-                         'or remove the auth_id and/or the env variable XSIAM_AUTH_ID to use Cortex XSOAR api:\n')
+    if auth_id and not (api_key or advanced_api_key):
+        raise ValueError('You must specify either api_key or advanced_api_key or use env variable DEMISTO_API_KEY or DEMISTO_ADVANCED_API_KEY ' 
+                         'to use Cortex XSIAM api or XSOAR 8+, or remove the auth_id and/or the env variable DEMISTO_API_KEY_ID '
+                         'to use Cortex XSOAR api:\n')
     configuration = Configuration()
-    configuration.api_key['Authorization'] = api_key
+    if advanced_api_key:
+        setattr(configuration, 'auth_signed_key', advanced_api_key)
+    else:
+        configuration.api_key['Authorization'] = api_key
     configuration.host = os.path.join(base_url)
     if auth_id:
         configuration.api_key['x-xdr-auth-id'] = auth_id
         configuration.host = os.path.join(configuration.host, 'xsoar')
         if not configuration.host.startswith("https://api-"):
             configuration.host = configuration.host.replace('https://', 'https://api-')
     configuration.verify_ssl = verify_ssl
@@ -336,8 +340,7 @@
         _preload_content=params.get(
         '_preload_content', True))
     if 200 == status_code:
         server_details = json.loads(server_details.replace('\'', '"'))
         if LooseVersion(server_details.get('demistoVersion')) >= LooseVersion('6.0.0'):
             url = '/layouts/import'
     return url
-
```

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/__init__.py` & `demisto_py-3.3.0/demisto_client/demisto_api/__init__.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/api/default_api.py` & `demisto_py-3.3.0/demisto_client/demisto_api/api/default_api.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/api_client.py` & `demisto_py-3.3.0/demisto_client/demisto_api/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 import six
 from six.moves.urllib.parse import quote
 
 from demisto_client.demisto_api.configuration import Configuration
 import demisto_client.demisto_api.models
 from demisto_client.demisto_api import rest
 
+import secrets
+import string
+from hashlib import sha256
+
+NONCE_POSSIBLE_VALUES = string.ascii_letters + string.digits
+
 
 class ApiClient(object):
     """Generic API client for Swagger client library builds.
 
     Swagger generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the Swagger
@@ -108,14 +114,23 @@
             _preload_content=True, _request_timeout=None):
 
         config = self.configuration; body = demisto_client.to_extended_dict(body)  # noqa: E702
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
+        auth_signed_key = getattr(self.configuration, 'auth_signed_key', None)
+        if auth_signed_key:
+            nonce: str = ''.join(secrets.choice(NONCE_POSSIBLE_VALUES) for _ in range(64))
+            timestamp = str(int(datetime.datetime.now(datetime.timezone.utc).timestamp()) * 1000)
+            header_params.update({
+                'x-xdr-timestamp': timestamp,
+                'x-xdr-nonce': nonce,
+                'Authorization': sha256(f'{auth_signed_key}{nonce}{timestamp}'.encode()).hexdigest(),
+            })
         if self.cookie:
             header_params['Cookie'] = self.cookie
         if header_params:
             header_params = self.sanitize_for_serialization(header_params)
             header_params = dict(self.parameters_to_tuples(header_params,
                                                            collection_formats))
```

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/configuration.py` & `demisto_py-3.3.0/demisto_client/demisto_api/configuration.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/__init__.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/advance_arg.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/advance_arg.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/arg_atomic_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/arg_atomic_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/arg_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/arg_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/arg_transformer.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/arg_transformer.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/argument.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/argument.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/array_positions.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/array_positions.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/attachment.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/attachment.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/audit.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/audit.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/audit_result.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/audit_result.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_api.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_api.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_filter_wrapper.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/automation_script_result.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/automation_script_result.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/command.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/command.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/common_fields.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/common_fields.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/complex_arg.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/complex_arg.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/config_data_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/config_data_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/config_field.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/config_field.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/create_incident_request.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/create_incident_request.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/custom_fields.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/custom_fields.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/d_bot_score.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/d_bot_score.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/dashboard.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/data_collection_form.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/data_collection_form.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/date_range.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/date_range.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/date_range_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/date_range_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/delete_evidence.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/delete_evidence.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/docker_image.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/docker_image.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/docker_images_result.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/docker_images_result.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/download_entry.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/download_entry.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/duration.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/duration.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/ending_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/ending_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry_category.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry_category.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry_history.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry_history.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry_reputation.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry_reputation.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry_task.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry_task.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/entry_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/entry_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/evidence.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/evidence.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/evidence_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/evidence_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/evidences.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/evidences.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/evidences_filter_wrapper.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/evidences_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/evidences_search_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/evidences_search_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_policy.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_policy.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_settings_source.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_settings_source.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/expiration_source.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/expiration_source.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicator.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicator.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicators.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicators.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/feed_indicators_request.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/feed_indicators_request.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/field_group.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/field_group.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/field_mapping.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/field_mapping.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/field_term_location_map.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/field_term_location_map.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/file_metadata.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/file_metadata.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/filter_cache.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/filter_cache.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/filter_operator_id.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/filter_operator_id.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/form_display.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/form_display.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/generic_indicator_update_batch.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/generic_indicator_update_batch.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/generic_string_date_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/generic_string_date_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/generic_string_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/generic_string_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/grid_column.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/grid_column.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/group.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/group.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/groups.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/groups.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/human_cron.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/human_cron.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/important.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/important.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_field.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_field.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_search_response_wrapper.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_search_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_status.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_status.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incident_wrapper.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incident_wrapper.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/incidents.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_context.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_context.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_edit_bulk_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_edit_bulk_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/indicator_result.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/indicator_result.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inline_response200.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/insight_cache.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/insight_cache.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/instance_classifier.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/instance_classifier.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/integration_script.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/integration_script.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_assignee.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_assignee.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_due.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_due.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_task_complete_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_task_complete_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inv_playbook_task_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inv_playbook_task_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/inv_task_info.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/inv_task_info.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_filter.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_filter.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_state.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_state.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_task.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_task.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_playbook_tasks_api.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_playbook_tasks_api.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_search_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_search_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_status.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_status.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigation_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigation_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/investigations.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/investigations.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/ioc_object.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/ioc_object.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/ioc_objects.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/ioc_objects.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/label.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/label.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/layout.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/layout.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/layout_api.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/layout_api.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/layout_field.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/layout_field.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/layout_section.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/layout_section.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/location.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/location.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/locations.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/locations.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/mapper.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/mapper.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/module_args.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/module_args.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/module_configuration.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/module_configuration.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/new_docker_image.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/new_docker_image.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/new_docker_image_result.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/new_docker_image_result.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/notifiable_item.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/notifiable_item.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/notify_timings.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/notify_timings.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/operator_argument.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/operator_argument.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/order.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/order.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/output.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/output.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/output_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/output_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/period.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/period.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_input.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_input.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_inputs.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_inputs.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_output.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_output.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_outputs.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_outputs.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_task.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_task.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/playbook_view.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/playbook_view.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/question.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/question.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/quiet_mode.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/quiet_mode.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/raw_feed_indicator.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/raw_feed_indicator.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/raw_message.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/raw_message.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/reliability.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/reliability.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/remote_repos.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/remote_repos.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/report.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/report.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/report_automation.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/report_automation.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/report_fields_decoder.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/report_fields_decoder.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/report_query.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/report_query.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/reputation.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/reputation.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/reputation_calc_alg.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/reputation_calc_alg.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/reputation_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/reputation_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/reputations_with_errors.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/reputations_with_errors.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/run_status.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/run_status.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/script_api.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/script_api.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/script_sub_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/script_sub_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/script_target.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/script_target.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/script_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/script_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/search_incidents_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/search_incidents_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/section.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/section.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/section_item.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/section_item.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/severity.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/severity.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/sla.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/sla.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/sla_state.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/sla_state.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/stats_query_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/stats_query_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/stats_text_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/stats_text_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/stats_trends_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/stats_trends_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/system.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/system.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/system_agent.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/system_agent.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task_condition.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task_condition.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task_loop.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task_loop.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task_state.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task_state.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task_type.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task_type.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/task_view.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/task_view.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/term_location_map.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/term_location_map.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/terminal_options.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/terminal_options.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/timer_action.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/timer_action.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/timer_trigger.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/timer_trigger.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/transformer_operator_id.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/transformer_operator_id.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/update_data_batch.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/update_data_batch.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/update_entry.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/update_entry.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/update_entry_tags.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/update_entry_tags.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/update_indicator_reputation_data.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/update_indicator_reputation_data.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/update_response.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/update_response.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/uploaded_entry.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/uploaded_entry.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/version.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/version.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/widget.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/widget.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/widget_cell.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/widget_cell.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/models/widget_cells.py` & `demisto_py-3.3.0/demisto_client/demisto_api/models/widget_cells.py`

 * *Files identical despite different names*

### Comparing `demisto-py-3.2.9/demisto_client/demisto_api/rest.py` & `demisto_py-3.3.0/demisto_client/demisto_api/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import certifi
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import urlencode
 
 try:
     import urllib3
+    import urllib
 except ImportError:
     raise ImportError('Swagger python client requires urllib3.')
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -84,15 +85,16 @@
                 maxsize = 4
 
         # https pool manager
         if configuration.proxy:
             proxy_headers = None
             parsed_proxy_url = urllib3.util.parse_url(configuration.proxy)
             if parsed_proxy_url.auth is not None:
-                proxy_headers = urllib3.util.make_headers(proxy_basic_auth=parsed_proxy_url.auth)
+                configuration.proxy_auth = urllib.parse.unquote(parsed_proxy_url.auth)
+                proxy_headers = urllib3.util.make_headers(proxy_basic_auth=configuration.proxy_auth)
 
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
```

