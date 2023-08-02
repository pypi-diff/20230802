# Comparing `tmp/nautobot_device_lifecycle_mgmt-1.3.1.tar.gz` & `tmp/nautobot_device_lifecycle_mgmt-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.3.1.tar", max compression
+gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.3.2.tar", max compression
```

## Comparing `nautobot_device_lifecycle_mgmt-1.3.1.tar` & `nautobot_device_lifecycle_mgmt-1.3.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0      591 2023-07-31 20:13:08.289233 nautobot_device_lifecycle_mgmt-1.3.1/LICENSE
--rw-r--r--   0        0        0     5939 2023-07-31 20:13:08.289233 nautobot_device_lifecycle_mgmt-1.3.1/README.md
--rw-r--r--   0        0        0     1418 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/__init__.py
--rw-r--r--   0        0        0       65 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/__init__.py
--rw-r--r--   0        0        0     3052 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
--rw-r--r--   0        0        0    11145 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/serializers.py
--rw-r--r--   0        0        0     1234 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/urls.py
--rw-r--r--   0        0        0     4602 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/views.py
--rw-r--r--   0        0        0     2141 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/choices.py
--rw-r--r--   0        0        0     1188 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/const.py
--rw-r--r--   0        0        0    29610 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/filters.py
--rw-r--r--   0        0        0    40734 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/forms.py
--rw-r--r--   0        0        0      685 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/graphql/types.py
--rw-r--r--   0        0        0      327 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/__init__.py
--rw-r--r--   0        0        0     3191 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
--rw-r--r--   0        0        0     3287 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
--rw-r--r--   0        0        0     9475 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/metrics.py
--rw-r--r--   0        0        0     3449 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
--rw-r--r--   0        0        0     4319 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
--rw-r--r--   0        0        0     5580 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
--rw-r--r--   0        0        0     2378 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
--rw-r--r--   0        0        0     4405 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
--rw-r--r--   0        0        0     4794 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
--rw-r--r--   0        0        0     3131 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
--rw-r--r--   0        0        0     1123 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
--rw-r--r--   0        0        0      612 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
--rw-r--r--   0        0        0      463 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
--rw-r--r--   0        0        0      984 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
--rw-r--r--   0        0        0      902 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
--rw-r--r--   0        0        0      568 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py
--rw-r--r--   0        0        0        0 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/__init__.py
--rw-r--r--   0        0        0    31341 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/models.py
--rw-r--r--   0        0        0    14180 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/navigation.py
--rw-r--r--   0        0        0     5407 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/signals.py
--rw-r--r--   0        0        0     2995 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software.py
--rw-r--r--   0        0        0     8101 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software_filters.py
--rw-r--r--   0        0        0    20020 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tables.py
--rw-r--r--   0        0        0     5526 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/template_content.py
--rw-r--r--   0        0        0     2094 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
--rw-r--r--   0        0        0     5904 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
--rw-r--r--   0        0        0     2429 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
--rw-r--r--   0        0        0      492 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
--rw-r--r--   0        0        0     2613 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
--rw-r--r--   0        0        0      939 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
--rw-r--r--   0        0        0     1523 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
--rw-r--r--   0        0        0     5632 2023-07-31 20:13:08.313233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
--rw-r--r--   0        0        0     2160 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
--rw-r--r--   0        0        0      513 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
--rw-r--r--   0        0        0     1113 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
--rw-r--r--   0        0        0      747 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
--rw-r--r--   0        0        0      365 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
--rw-r--r--   0        0        0      505 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
--rw-r--r--   0        0        0     3605 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
--rw-r--r--   0        0        0     5075 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
--rw-r--r--   0        0        0      263 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
--rw-r--r--   0        0        0     1971 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
--rw-r--r--   0        0        0       92 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
--rw-r--r--   0        0        0     3138 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
--rw-r--r--   0        0        0      251 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
--rw-r--r--   0        0        0       86 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
--rw-r--r--   0        0        0      392 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
--rw-r--r--   0        0        0     5784 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
--rw-r--r--   0        0        0     5885 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
--rw-r--r--   0        0        0     5686 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
--rw-r--r--   0        0        0      269 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
--rw-r--r--   0        0        0     1942 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
--rw-r--r--   0        0        0       96 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
--rw-r--r--   0        0        0     1599 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
--rw-r--r--   0        0        0      615 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
--rw-r--r--   0        0        0       67 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/__init__.py
--rw-r--r--   0        0        0     5277 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/conftest.py
--rw-r--r--   0        0        0    27988 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_api.py
--rw-r--r--   0        0        0     1535 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_basic.py
--rw-r--r--   0        0        0    30831 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py
--rw-r--r--   0        0        0    23393 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py
--rw-r--r--   0        0        0    32901 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_model.py
--rw-r--r--   0        0        0    11840 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
--rw-r--r--   0        0        0    16523 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_views.py
--rw-r--r--   0        0        0    11497 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/urls.py
--rw-r--r--   0        0        0      423 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/utils.py
--rw-r--r--   0        0        0    43490 2023-07-31 20:13:08.317233 nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/views.py
--rw-r--r--   0        0        0     2771 2023-07-31 20:13:26.713583 nautobot_device_lifecycle_mgmt-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-08-02 14:58:06.386102 nautobot_device_lifecycle_mgmt-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5939 2023-08-02 14:58:06.386102 nautobot_device_lifecycle_mgmt-1.3.2/README.md
+-rw-r--r--   0        0        0     1418 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/__init__.py
+-rw-r--r--   0        0        0     3052 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
+-rw-r--r--   0        0        0    11145 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/serializers.py
+-rw-r--r--   0        0        0     1234 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/urls.py
+-rw-r--r--   0        0        0     4602 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/views.py
+-rw-r--r--   0        0        0     2141 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/choices.py
+-rw-r--r--   0        0        0     1188 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/const.py
+-rw-r--r--   0        0        0    29610 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/filters.py
+-rw-r--r--   0        0        0    40734 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/forms.py
+-rw-r--r--   0        0        0      685 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/graphql/types.py
+-rw-r--r--   0        0        0      327 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/jobs/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
+-rw-r--r--   0        0        0     3287 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
+-rw-r--r--   0        0        0     9475 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/metrics.py
+-rw-r--r--   0        0        0     3449 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
+-rw-r--r--   0        0        0     4319 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
+-rw-r--r--   0        0        0     5580 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
+-rw-r--r--   0        0        0     2378 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
+-rw-r--r--   0        0        0     4405 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
+-rw-r--r--   0        0        0     4794 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
+-rw-r--r--   0        0        0     3131 2023-08-02 14:58:06.406102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
+-rw-r--r--   0        0        0     1123 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
+-rw-r--r--   0        0        0      612 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
+-rw-r--r--   0        0        0      463 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
+-rw-r--r--   0        0        0      984 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
+-rw-r--r--   0        0        0      902 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
+-rw-r--r--   0        0        0      568 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/__init__.py
+-rw-r--r--   0        0        0    31920 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/models.py
+-rw-r--r--   0        0        0    14180 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/navigation.py
+-rw-r--r--   0        0        0     5407 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/signals.py
+-rw-r--r--   0        0        0     2995 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/software.py
+-rw-r--r--   0        0        0     8101 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/software_filters.py
+-rw-r--r--   0        0        0    21032 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tables.py
+-rw-r--r--   0        0        0     5526 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/template_content.py
+-rw-r--r--   0        0        0     2094 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
+-rw-r--r--   0        0        0     5904 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
+-rw-r--r--   0        0        0     2429 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
+-rw-r--r--   0        0        0      492 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     2613 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
+-rw-r--r--   0        0        0      939 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
+-rw-r--r--   0        0        0     1523 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
+-rw-r--r--   0        0        0     5632 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
+-rw-r--r--   0        0        0     2160 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
+-rw-r--r--   0        0        0      513 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
+-rw-r--r--   0        0        0     1113 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
+-rw-r--r--   0        0        0      747 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
+-rw-r--r--   0        0        0      365 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
+-rw-r--r--   0        0        0      505 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     3605 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
+-rw-r--r--   0        0        0     5075 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
+-rw-r--r--   0        0        0      263 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
+-rw-r--r--   0        0        0     1971 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
+-rw-r--r--   0        0        0       92 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
+-rw-r--r--   0        0        0     3138 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
+-rw-r--r--   0        0        0      251 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
+-rw-r--r--   0        0        0       86 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
+-rw-r--r--   0        0        0      392 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
+-rw-r--r--   0        0        0     5784 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
+-rw-r--r--   0        0        0     5885 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
+-rw-r--r--   0        0        0     5686 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
+-rw-r--r--   0        0        0      269 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
+-rw-r--r--   0        0        0     1942 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
+-rw-r--r--   0        0        0       96 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
+-rw-r--r--   0        0        0     1599 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
+-rw-r--r--   0        0        0      615 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
+-rw-r--r--   0        0        0       67 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/__init__.py
+-rw-r--r--   0        0        0     5277 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_api.py
+-rw-r--r--   0        0        0     1535 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_basic.py
+-rw-r--r--   0        0        0    30831 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_filters.py
+-rw-r--r--   0        0        0    23393 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_forms.py
+-rw-r--r--   0        0        0    32901 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_model.py
+-rw-r--r--   0        0        0    11840 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
+-rw-r--r--   0        0        0    16523 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_views.py
+-rw-r--r--   0        0        0    11497 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/urls.py
+-rw-r--r--   0        0        0      423 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/utils.py
+-rw-r--r--   0        0        0    43709 2023-08-02 14:58:06.410102 nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/views.py
+-rw-r--r--   0        0        0     2771 2023-08-02 14:58:20.086141 nautobot_device_lifecycle_mgmt-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.3.2/PKG-INFO
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/LICENSE` & `nautobot_device_lifecycle_mgmt-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/README.md` & `nautobot_device_lifecycle_mgmt-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/__init__.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/nested_serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/serializers.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/api/views.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/choices.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/const.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/const.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/filters.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/forms.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/graphql/types.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/graphql/types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/metrics.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/models.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,14 +515,16 @@
     run_type = models.CharField(max_length=50, choices=choices.ReportRunTypeChoices)
     valid_software = models.ManyToManyField(
         to="ValidatedSoftwareLCM", related_name="inventory_item_software_validation_results"
     )
 
     csv_headers = [
         "inventory_item",
+        "item_name",
+        "device",
         "software",
         "valid",
         "last_run",
         "run_type",
         "approved_software",
     ]
 
@@ -532,21 +534,34 @@
         verbose_name = "Inventory Item Software Validation Report"
         ordering = ("inventory_item",)
 
     def to_csv(self):
         """Indicates model fields to return as csv."""
         return (
             self.inventory_item.part_id,
+            self.inventory_item.name,
+            self.inventory_item.device.name,
             self.software if self.software else "None",
             str(self.is_validated),
             self.last_run.strftime("%Y-%m-%d %H:%M:%S") if self.last_run else "-",
             self.run_type,
             ",".join(str(valid.software) for valid in ValidatedSoftwareLCM.objects.get_for_object(self.inventory_item)),
         )
 
+    def __str__(self):
+        """String representation of InventoryItemSoftwareValidationResult."""
+        if self.is_validated:
+            msg = f"Inventory Item: {self.inventory_item.name} - " f"Device: {self.inventory_item.device.name} - Valid"
+        else:
+            msg = (
+                f"Inventory Item: {self.inventory_item.name} - "
+                f"Device: {self.inventory_item.device.name} - Not Valid"
+            )
+        return msg
+
 
 @extras_features(
     "custom_fields",
     "custom_links",
     "custom_validators",
     "export_templates",
     "graphql",
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/navigation.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/signals.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/software.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tables.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,15 +226,17 @@
 
 
 class DeviceSoftwareValidationResultTable(BaseTable):
     """Table for device software validation report."""
 
     name = tables.TemplateColumn(
         template_code='<a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/'
-        '?&device_type={{ record.device__device_type__model }}">{{ record.device__device_type__model }}</a>'
+        '?&device_type={{ record.device__device_type__model }}">{{ record.device__device_type__model }}</a>',
+        orderable=True,
+        accessor="device__device_type__model",
     )
     total = tables.TemplateColumn(
         template_code='<a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/'
         '?&device_type={{ record.device__device_type__model }}">{{ record.total }}</a>'
     )
     valid = tables.TemplateColumn(
         template_code='<a href="/plugins/nautobot-device-lifecycle-mgmt/device-validated-software-result/'
@@ -309,15 +311,27 @@
     """Table for InventoryItemSoftwareValidationResultTable."""
 
     part_id = tables.TemplateColumn(
         template_code="""{% if record.inventory_item__part_id  %}
         <a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/?&part_id={{ record.inventory_item__part_id }}">{{ record.inventory_item__part_id }}</a>
         {% else %}
         Please assign Part ID value to Inventory Item
-        {% endif %}"""
+        {% endif %}""",
+        orderable=True,
+        accessor="inventory_item__part_id",
+    )
+    part_name = tables.TemplateColumn(
+        template_code="{{ record.inventory_item__name }}",
+        orderable=True,
+        accessor="inventory_item__name",
+    )
+    device = tables.TemplateColumn(
+        template_code="{{ record.inventory_item__device__name }}",
+        orderable=True,
+        accessor="inventory_item__device__name",
     )
     total = tables.TemplateColumn(
         template_code='<a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/'
         '?&part_id={{ record.inventory_item__part_id }}">{{ record.total }}</a>'
     )
     valid = tables.TemplateColumn(
         template_code='<a href="/plugins/nautobot-device-lifecycle-mgmt/inventory-item-validated-software-result/'
@@ -338,17 +352,19 @@
         verbose_name="Export Data",
     )
 
     class Meta(BaseTable.Meta):  # pylint: disable=too-few-public-methods
         """Metaclass attributes of InventoryItemSoftwareValidationResultTable."""
 
         model = InventoryItemSoftwareValidationResult
-        fields = ["part_id", "total", "valid", "invalid", "no_software", "valid_percent"]
+        fields = ["part_id", "part_name", "device", "total", "valid", "invalid", "no_software", "valid_percent"]
         default_columns = [
             "part_id",
+            "part_name",
+            "device",
             "total",
             "valid",
             "invalid",
             "no_software",
             "valid_percent",
             "actions",
         ]
@@ -358,14 +374,21 @@
     """Table for a list of intenotry items to software validation report."""
 
     part_id = tables.Column(
         accessor="inventory_item__part_id",
         verbose_name="Part ID",
         default="Please assign Part ID value to Inventory Item",
     )
+    part_name = tables.TemplateColumn(
+        template_code="""<a href='/dcim/inventory-items/{{ record.inventory_item.pk }}'>
+                        {{ record.inventory_item.name }}</a>""",
+        verbose_name="Part Name",
+        accessor="inventory_item__name",
+    )
+    device_name = tables.Column(accessor="inventory_item__device__name", verbose_name="Device")
     software = tables.Column(accessor="software", verbose_name="Current Software", linkify=True)
     valid = tables.Column(accessor="is_validated", verbose_name="Valid")
     last_run = tables.Column(accessor="last_run", verbose_name="Last Run")
     run_type = tables.Column(accessor="run_type", verbose_name="Run Type")
     valid_software = tables.TemplateColumn(
         template_code="""{% for valid_software in record.valid_software.all %}
                     <a href="/plugins/nautobot-device-lifecycle-mgmt/validated-software/{{ valid_software.id }}"
@@ -377,17 +400,19 @@
         orderable=True,
     )
 
     class Meta(BaseTable.Meta):  # pylint: disable=too-few-public-methods
         """Metaclass attributes of InventoryItemSoftwareValidationResultTable."""
 
         model = InventoryItemSoftwareValidationResult
-        fields = ["part_id", "software", "valid", "last_run", "run_type", "valid_software"]
+        fields = ["part_id", "part_name", "device_name", "software", "valid", "last_run", "run_type", "valid_software"]
         default_columns = [
             "part_id",
+            "part_name",
+            "device_name",
             "software",
             "valid",
             "last_run",
             "run_type",
             "valid_software",
         ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/template_content.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/conftest.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_api.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_basic.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_model.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/tests/test_views.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/urls.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/nautobot_device_lifecycle_mgmt/views.py` & `nautobot_device_lifecycle_mgmt-1.3.2/nautobot_device_lifecycle_mgmt/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,15 +715,17 @@
     """View for executive report on inventory item software validation."""
 
     filterset = InventoryItemSoftwareValidationResultFilterSet
     filterset_form = InventoryItemSoftwareValidationResultFilterForm
     table = InventoryItemSoftwareValidationResultTable
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html"
     queryset = (
-        InventoryItemSoftwareValidationResult.objects.values("inventory_item__part_id", "inventory_item__pk")
+        InventoryItemSoftwareValidationResult.objects.values(
+            "inventory_item__part_id", "inventory_item__name", "inventory_item__pk", "inventory_item__device__name"
+        )
         .distinct()
         .annotate(
             total=Count("inventory_item__part_id"),
             valid=Count("inventory_item__part_id", filter=Q(is_validated=True)),
             invalid=Count("inventory_item__part_id", filter=Q(is_validated=False) & ~Q(software=None)),
             no_software=Count("inventory_item__part_id", filter=Q(software=None)),
             valid_percent=ExpressionWrapper(100 * F("valid") / (F("total")), output_field=FloatField()),
@@ -824,15 +826,22 @@
                     if key != "name"
                 ]
             )
         )
         csv_data.append(",".join([]))
 
         qs = self.queryset.values(
-            "inventory_item__part_id", "total", "valid", "invalid", "no_software", "valid_percent"
+            "inventory_item__part_id",
+            "inventory_item__name",
+            "inventory_item__device__name",
+            "total",
+            "valid",
+            "invalid",
+            "no_software",
+            "valid_percent",
         )
         csv_data.append(
             ",".join(
                 [
                     "Part ID" if item == "inventory_item__part_id" else item.replace("_", " ").title()
                     for item in qs[0].keys()
                 ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/pyproject.toml` & `nautobot_device_lifecycle_mgmt-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-device-lifecycle-mgmt"
-version = "v1.3.1"
+version = "v1.3.2"
 description = "Manages device lifecycles for platforms and software."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 repository = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.3.1/PKG-INFO` & `nautobot_device_lifecycle_mgmt-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-device-lifecycle-mgmt
-Version: 1.3.1
+Version: 1.3.2
 Summary: Manages device lifecycles for platforms and software.
 Home-page: https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.3.1
+Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 1.3.2
 Summary: Manages device lifecycles for platforms and software. Home-page:
 https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt License:
 Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network to Code, LLC
 Author-email: opensource@networktocode.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

