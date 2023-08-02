# Comparing `tmp/johnsnowlabs-5.0.0.tar.gz` & `tmp/johnsnowlabs-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-5.0.0.tar", last modified: Thu Jul 13 10:19:17 2023, max compression
+gzip compressed data, was "johnsnowlabs-5.0.1.tar", last modified: Wed Aug  2 19:54:41 2023, max compression
```

## Comparing `johnsnowlabs-5.0.0.tar` & `johnsnowlabs-5.0.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.533043 johnsnowlabs-5.0.0/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-5.0.0/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-07-13 10:19:17.533043 johnsnowlabs-5.0.0/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-5.0.0/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-5.0.0/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-07-04 19:15:47.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-06-19 13:38:29.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs-5.0.0/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4853 2023-07-11 11:56:33.000000 johnsnowlabs-5.0.0/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4800 2023-07-13 10:13:05.000000 johnsnowlabs-5.0.0/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4798 2023-07-13 10:12:42.000000 johnsnowlabs-5.0.0/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-5.0.0/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    33315 2023-07-04 22:09:34.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs-5.0.0/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2237 2023-07-13 09:15:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.533043 johnsnowlabs-5.0.0/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2023-07-04 22:00:25.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-06-14 20:24:15.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.533043 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-5.0.0/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-07-04 21:29:57.000000 johnsnowlabs-5.0.0/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.0/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-13 10:19:17.529043 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-07-13 10:19:17.000000 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-07-13 10:19:17.000000 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-07-13 10:19:17.000000 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      135 2023-07-13 10:19:17.000000 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-07-13 10:19:17.000000 johnsnowlabs-5.0.0/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-07-13 10:19:17.533043 johnsnowlabs-5.0.0/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2101 2023-07-13 10:19:08.000000 johnsnowlabs-5.0.0/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.744137 johnsnowlabs-5.0.1/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-5.0.1/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-08-02 19:54:41.744137 johnsnowlabs-5.0.1/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-5.0.1/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-5.0.1/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-07-04 19:15:47.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-06-19 13:38:29.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3192 2023-08-02 19:28:44.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs-5.0.1/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4853 2023-07-11 11:56:33.000000 johnsnowlabs-5.0.1/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4800 2023-07-13 10:13:05.000000 johnsnowlabs-5.0.1/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4798 2023-07-13 10:12:42.000000 johnsnowlabs-5.0.1/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-5.0.1/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    33315 2023-07-04 22:09:34.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs-5.0.1/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2237 2023-08-02 19:25:05.000000 johnsnowlabs-5.0.1/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6668 2023-08-02 19:42:36.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2023-07-04 22:00:25.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8150 2023-08-02 19:47:23.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.744137 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-5.0.1/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-07-04 21:29:57.000000 johnsnowlabs-5.0.1/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-5.0.1/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-08-02 19:54:41.740137 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-08-02 19:54:41.000000 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-08-02 19:54:41.000000 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-08-02 19:54:41.000000 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      135 2023-08-02 19:54:41.000000 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-08-02 19:54:41.000000 johnsnowlabs-5.0.1/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-08-02 19:54:41.744137 johnsnowlabs-5.0.1/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2101 2023-07-13 10:19:08.000000 johnsnowlabs-5.0.1/setup.py
```

### Comparing `johnsnowlabs-5.0.0/LICENSE` & `johnsnowlabs-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/PKG-INFO` & `johnsnowlabs-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 5.0.0
+Version: 5.0.1
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-5.0.0/README.md` & `johnsnowlabs-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/__init__.py` & `johnsnowlabs-5.0.1/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-5.0.1/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 dependency_type=JvmHardwareTarget.gpu,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
             JvmHardwareTarget.m1: UrlDependency(
-                url="https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/jars/spark-nlp-m1-assembly-{lib_version}.jar",
+                url="https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/jars/spark-nlp-silicon-assembly-{lib_version}.jar",
                 dependency_type=JvmHardwareTarget.m1,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
             JvmHardwareTarget.cpu: UrlDependency(
```

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-5.0.1/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/finance.py` & `johnsnowlabs-5.0.1/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/legal.py` & `johnsnowlabs-5.0.1/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/medical.py` & `johnsnowlabs-5.0.1/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/nlp.py` & `johnsnowlabs-5.0.1/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-5.0.1/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-5.0.1/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-5.0.1/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-5.0.1/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/settings.py` & `johnsnowlabs-5.0.1/johnsnowlabs/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,27 @@
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
 
 
-raw_version_jsl_lib = "5.0.0"
-raw_version_nlp = "5.0.0"
+raw_version_jsl_lib = "5.0.1"
+raw_version_nlp = "5.0.1"
 
 raw_version_nlu = "4.2.2"
 
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "5.0.0"
-raw_version_secret_medical = "5.0.0"
+raw_version_medical = "5.0.1"
+raw_version_secret_medical = "5.0.1"
 
-raw_version_secret_ocr = "4.4.3"
-raw_version_ocr = "4.4.3"
+raw_version_secret_ocr = "4.4.4"
+raw_version_ocr = "4.4.4"
 raw_version_pydantic = "1.10.11"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
```

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/enums.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ERROR = "ERROR"
     UNKNOWN = "UNKNOWN"
 
 
 class JvmHardwareTarget(BaseEnum):
     gpu = "gpu"
     cpu = "cpu"
-    m1 = "m1"
+    m1 = "apple_silicon"
     aarch = "aarch"
 
     @classmethod
     def bool_choice_to_hardware(
         cls, gpu: bool = False, cpu: bool = False, m1: bool = False
     ) -> "JvmHardwareTarget":
         if gpu:
```

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/functional.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/sparksession_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
             )
 
     launched_products: List[str] = []
     hardware_target = JvmHardwareTarget.from_str(hardware_target)
 
     # Get all Local Jar Paths, downloads them if missing
     suite = get_install_suite_from_jsl_home(
+        visual=visual,
         create_jsl_home_if_missing=create_jsl_home_if_missing,
         only_jars=True,
         jvm_hardware_target=hardware_target,
         force_browser=browser_login,
         browser_login=browser_login,
         access_token=access_token,
         local_license_number=local_license_number,
```

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-5.0.1/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs/visual.py` & `johnsnowlabs-5.0.1/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-5.0.1/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 5.0.0
+Version: 5.0.1
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-5.0.0/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-5.0.1/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.0.0/setup.py` & `johnsnowlabs-5.0.1/setup.py`

 * *Files identical despite different names*

