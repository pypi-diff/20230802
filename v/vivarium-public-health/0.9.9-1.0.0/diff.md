# Comparing `tmp/vivarium_public_health-0.9.9.tar.gz` & `tmp/vivarium_public_health-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vivarium_public_health-0.9.9.tar", last modified: Thu Mar 28 22:20:21 2019, max compression
+gzip compressed data, was "vivarium_public_health-1.0.0.tar", last modified: Wed Aug  2 21:41:03 2023, max compression
```

## Comparing `vivarium_public_health-0.9.9.tar` & `vivarium_public_health-1.0.0.tar`

### file list

```diff
@@ -1,154 +1,175 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35146 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/LICENSE.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/requirements-doc.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/util.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/healthcare_access.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/mass_treatment_campaign.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/base_treatment.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/schedule.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/disability.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/sample_history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/inspector.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/dataset_manager.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/add_new_birth_cohort.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/mortality.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/base_population.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/data_transformations.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/base_risk.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/effect.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/distributions.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/
--rw-rw-r--   0 travis    (2000) travis    (2000)       90 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/mock_artifact.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/utils.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/model.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/transition.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/state.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5936 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2827 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9170 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_base_treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_healthcare_access_module.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7165 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/test_disability.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21799 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/test_utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7376 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5502 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_add_new_birth_cohort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11808 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_base_population.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2205 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_base_risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6287 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_distributions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7529 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20366 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_effect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      987 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/dataset_manager/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15064 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   172261 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/artifact.hdf
--rw-rw-r--   0 travis    (2000) travis    (2000)     8585 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_hdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_dataset_manager.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18145 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/test_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5544 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/test_special_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/test_utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4549 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      283 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3267 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CODE_OF_CONDUCT.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/__about__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8062 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/healthcare_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/therapeutic_inertia.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4533 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4715 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/mass_treatment_campaign.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6017 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/base_treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/magic_wand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1289 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/mortality.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3589 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/sample_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2616 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4085 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disability.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/inspector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14341 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/base_population.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3167 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/mortality.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19770 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7986 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/add_new_birth_cohorts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/interactive.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17827 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/base_risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/effect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5883 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/distributions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/magic_wand_components.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10471 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3924 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/intervention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14284 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/delay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2090 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/population.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13473 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/observer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6923 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/hdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8160 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/dataset_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      331 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9955 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/artifact.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3813 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/mock_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17569 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8247 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8114 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/special_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8807 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3318 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/transition.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/special_disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/state.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/disease/transition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.770962 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/disability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/mortality.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/risk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/metrics/stratification.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/delay.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/disease.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/intervention.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/magic_wand_components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/observer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/mslt/population.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/add_new_birth_cohorts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/base_population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/data_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/population/mortality.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/base_risk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/data_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/effect.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/implementations/low_birth_weight_and_short_gestation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/risks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.774962 vivarium_public_health-1.0.0/docs/source/api_reference/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/mock_artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/testing/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/magic_wand.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/scale_up.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/treatment/therapeutic_inertia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/api_reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/docs/source/tutorials/risk_exposure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.766962 vivarium_public_health-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/special_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/disease/transition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/mortality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/stratification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/magic_wand_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.782962 vivarium_public_health-1.0.0/src/vivarium_public_health/population/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/add_new_birth_cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/base_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21804 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/population/mortality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/base_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/risks/implementations/low_birth_weight_and_short_gestation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/mock_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/magic_wand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/scale_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/therapeutic_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/src/vivarium_public_health/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.778962 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 21:41:03.000000 vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.786962 vivarium_public_health-1.0.0/tests/disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/test_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/disease/test_special_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.790962 vivarium_public_health-1.0.0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_categorical_risk_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disability_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_disease_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_mortality_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/metrics/test_stratification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.794962 vivarium_public_health-1.0.0/tests/population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_add_new_birth_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_base_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/population/test_data_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/tests/risks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_base_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_data_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20333 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/risks/test_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:03.798962 vivarium_public_health-1.0.0/tests/treatment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tests/treatment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 21:40:47.000000 vivarium_public_health-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vivarium_public_health-0.9.9/docs/Makefile` & `vivarium_public_health-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.9/docs/source/conf.py` & `vivarium_public_health-1.0.0/docs/source/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,125 +6,130 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
+import sys
+
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
+from pathlib import Path
 
-import os
-import sys
+from docutils.nodes import Text
+from sphinx.ext.intersphinx import missing_reference
 
 import vivarium_public_health
 
-src_dir = os.path.dirname(vivarium_public_health.__file__)
+base_dir = Path(vivarium_public_health.__file__).parent
 
 about = {}
-with open(os.path.join(src_dir, "__about__.py")) as f:
+with (base_dir / "__about__.py").open() as f:
     exec(f.read(), about)
 
-sys.path.insert(0, os.path.abspath('..'))
+sys.path.insert(0, str(Path("..").resolve()))
 
 # -- Project information -----------------------------------------------------
 
-project = about['__title__']
-copyright = f'2018, {about["__author__"]}'
+project = about["__title__"]
+copyright = f'2023, {about["__author__"]}'
 author = about["__author__"]
 
 # The short X.Y version.
-version = about["__version__"]
+version = vivarium_public_health.__version__
 # The full version, including alpha/beta/rc tags.
-release = about["__version__"]
+release = vivarium_public_health.__version__
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 
-needs_sphinx = '1.5'
+needs_sphinx = "4.0"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode',
-    'sphinx_autodoc_typehints',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.viewcode",
+    "sphinx_click.ext",
+    "matplotlib.sphinxext.plot_directive",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
-html_theme_path = ['_theme']
-html_theme = 'sphinx_rtd_theme'
+html_theme_path = ["_theme"]
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # This is required for the alabaster theme
 # refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
 html_sidebars = {
-    '**': [
-        'globaltoc.html',  # needs 'show_related': True theme option to display
-        'searchbox.html',
+    "**": [
+        "globaltoc.html",  # needs 'show_related': True theme option to display
+        "searchbox.html",
     ]
 }
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
@@ -133,65 +138,118 @@
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, f'{about["__title__"]}.tex', f'{about["__title__"]} Documentation',
-     about["__author__"], 'manual'),
+    (
+        master_doc,
+        f'{about["__title__"]}.tex',
+        f'{about["__title__"]} Documentation',
+        about["__author__"],
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, f'{about["__title__"]}', f'{about["__title__"]} Documentation',
-     [author], 1)
+    (master_doc, f'{about["__title__"]}', f'{about["__title__"]} Documentation', [author], 1)
 ]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, f'{about["__title__"]}', f'{about["__title__"]} Documentation',
-     author, f'{about["__title__"]}', about["__summary__"],
-     'Miscellaneous'),
+    (
+        master_doc,
+        f'{about["__title__"]}',
+        f'{about["__title__"]} Documentation',
+        author,
+        f'{about["__title__"]}',
+        about["__summary__"],
+        "Miscellaneous",
+    ),
 ]
 
-# Example configuration for intersphinx: refer to the Python standard library.
-# intersphinx_mapping = {'https://docs.python.org/': None}
+# Other docs we can link to
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3.8", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
+    "tables": ("https://www.pytables.org/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "vivarium": ("https://vivarium.readthedocs.io/en/latest/", None),
+}
 
 
 # -- Autodoc configuration ------------------------------------------------
 
-# Sort order of members listed by autodoc
-# options are: 'alphabetical', 'groupwise', or 'bysource'
-autodoc_member_order = 'bysource'
-
-# Defaults for automodule and autoclass
-# To negate add `:no-undoc-members:` flag to a particular instance
-autodoc_default_flags = ['members', 'undoc-members' ]
+autodoc_default_options = {
+    # Automatically document members (e.g. classes in a module,
+    # methods in a class, etc.)
+    "members": True,
+    # Order of items documented is determined by the order
+    # of appearance in the source code
+    "member-order": "bysource",
+    # Generate docs even if an item has no docstring.
+    "undoc-members": True,
+    # Don't document things with a leading underscore.
+    "private-members": False,
+}
+
+# Display type hints in the description instead of the signature.
+autodoc_typehints = "description"
+
+
+# -- nitpicky mode --------------------------------------------------------
+# Ensures that all references in the docs resolve.
 
+nitpicky = True
+nitpick_ignore = []
+
+for line in open("../nitpick-exceptions"):
+    if line.strip() == "" or line.startswith("#"):
+        continue
+    dtype, target = line.split(None, 1)
+    target = target.strip()
+    nitpick_ignore.append((dtype, target))
+
+
+# Fix sphinx warnings when for literal Ellipses in type hints.
+def setup(app):
+    app.connect("missing-reference", __sphinx_issue_8127)
+
+
+def __sphinx_issue_8127(app, env, node, contnode):
+    reftarget = node.get("reftarget", None)
+    if reftarget == "..":
+        node["reftype"] = "data"
+        node["reftarget"] = "Ellipsis"
+        text_node = next(iter(contnode.traverse(lambda n: n.tagname == "#text")))
+        replacement_node = Text("...", "")
+        if text_node.parent is not None:
+            text_node.parent.replace(text_node, replacement_node)
+        else:  # e.g. happens in rtype fields
+            contnode = replacement_node
+        return missing_reference(app, env, node, contnode)
```

### Comparing `vivarium_public_health-0.9.9/README.rst` & `vivarium_public_health-1.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Vivarium Public Health
 ======================
 
 .. image:: https://badge.fury.io/py/vivarium-public-health.svg
     :target: https://badge.fury.io/py/vivarium-public-health
 
-.. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=develop
+.. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=master
     :target: https://travis-ci.org/ihmeuw/vivarium_public_health
     :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/vivarium_public_health/badge/?version=latest
     :target: https://vivarium_public_health.readthedocs.io/en/latest/?badge=latest
     :alt: Latest Docs
```

### Comparing `vivarium_public_health-0.9.9/setup.py` & `vivarium_public_health-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,88 @@
 #!/usr/bin/env python
 import os
 
-from setuptools import setup, find_packages
-
+from setuptools import find_packages, setup
 
 if __name__ == "__main__":
-
     base_dir = os.path.dirname(__file__)
     src_dir = os.path.join(base_dir, "src")
 
     about = {}
     with open(os.path.join(src_dir, "vivarium_public_health", "__about__.py")) as f:
         exec(f.read(), about)
 
     with open(os.path.join(base_dir, "README.rst")) as f:
         long_description = f.read()
 
     install_requirements = [
-        'vivarium>=0.8.18',
-        # FIXME: Newer versions of numpy have conflicting dependencies
-        # with pytables.
-        'numpy<=1.15.4',
-        'pandas',
-        'scipy',
-        # FIXME: Requirement imposed by our standard data sources.
-        'tables<=3.4.0',
-        'risk_distributions>=2.0.0',
+        "vivarium>=1.2.1",
+        "numpy",
+        "pandas",
+        "scipy",
+        "tables",
+        "risk_distributions>=2.0.11",
     ]
 
+    setup_requires = ["setuptools_scm"]
+
     test_requirements = [
-        'pytest',
-        'pytest-mock',
-        'hypothesis',
+        "pytest",
+        "pytest-mock",
+        "hypothesis",
     ]
 
     doc_requirements = [
-        'sphinx',
-        'sphinx-autodoc-typehints',
-        'sphinx-rtd-theme',
+        "sphinx>=4.0",
+        "sphinx-rtd-theme",
+        "sphinx-click",
+        "IPython",
+        "matplotlib",
     ]
 
     setup(
-        name=about['__title__'],
-        version=about['__version__'],
-
-        description=about['__summary__'],
+        name=about["__title__"],
+        description=about["__summary__"],
         long_description=long_description,
-        license=about['__license__'],
+        license=about["__license__"],
         url=about["__uri__"],
-
         author=about["__author__"],
         author_email=about["__email__"],
-
         classifiers=[
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
             "Natural Language :: English",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: POSIX",
             "Operating System :: POSIX :: BSD",
             "Operating System :: POSIX :: Linux",
             "Operating System :: Microsoft :: Windows",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: Implementation :: CPython",
             "Topic :: Education",
             "Topic :: Scientific/Engineering",
             "Topic :: Scientific/Engineering :: Artificial Life",
             "Topic :: Scientific/Engineering :: Mathematics",
             "Topic :: Scientific/Engineering :: Medical Science Apps.",
             "Topic :: Scientific/Engineering :: Physics",
             "Topic :: Software Development :: Libraries",
         ],
-
-        package_dir={'': 'src'},
-        packages=find_packages(where='src'),
+        package_dir={"": "src"},
+        packages=find_packages(where="src"),
         include_package_data=True,
-
         install_requires=install_requirements,
         tests_require=test_requirements,
         extras_require={
-            'docs': doc_requirements,
-            'test': test_requirements,
-            'dev': doc_requirements + test_requirements,
+            "docs": doc_requirements,
+            "test": test_requirements,
+            "dev": doc_requirements + test_requirements,
         },
-
         zip_safe=False,
+        use_scm_version={
+            "write_to": "src/vivarium_public_health/_version.py",
+            "write_to_template": '__version__ = "{version}"\n',
+            "tag_regex": r"^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
+        },
+        setup_requires=setup_requires,
     )
```

### Comparing `vivarium_public_health-0.9.9/tests/metrics/test_disability.py` & `vivarium_public_health-1.0.0/tests/metrics/test_disability.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #     year_end = base_config.time.end.year
 #     n_simulants = 1000
 #
 #     asymp_data_funcs = {'prevalence': lambda _, __: build_table(1.0, year_start-1, year_end,
 #                                                                 ['age', 'year', 'sex', 'value']),
 #                         'disability_weight': lambda _, __: 0.0,
 #                         'dwell_time': lambda _, __: pd.Timedelta(days=1),
-#                         'excess_mortality': lambda _, __: build_table(0, year_start-1, year_end)}
+#                         'excess_mortality_rate': lambda _, __: build_table(0, year_start-1, year_end)}
 #
 #     asymptomatic_disease_state = ExcessMortalityState('asymptomatic', get_data_functions=asymp_data_funcs)
 #     asymptomatic_disease_model = DiseaseModel('asymptomatic',
 #                                               states=[asymptomatic_disease_state],
 #                                               initial_state=asymptomatic_disease_state,
 #                                               get_data_functions={
 #                                                   'csmr': lambda _, __: build_table(0, year_start-1, year_end)})
@@ -43,39 +43,39 @@
 #     components = [TestPopulation(), asymptomatic_disease_model, disability]
 #
 #     if flu:
 #         flu_data_funcs = {'prevalence': lambda _, __: build_table(1.0, year_start-1, year_end,
 #                                                                   ['age', 'year', 'sex', 'value']),
 #                           'disability_weight': lambda _, __: 0.2,
 #                           'dwell_time': lambda _, __: pd.Timedelta(days=1),
-#                           'excess_mortality': lambda _, __: build_table(0, year_start-1, year_end)}
+#                           'excess_mortality_rate': lambda _, __: build_table(0, year_start-1, year_end)}
 #         flu = ExcessMortalityState('flu', get_data_functions=flu_data_funcs)
 #         flu_model = DiseaseModel('flu', states=[flu],
 #                                  initial_state=flu,
 #                                  get_data_functions={'csmr': lambda _, __: build_table(0, year_start-1, year_end)})
 #         components.append(flu_model)
 #
 #     if mumps:
 #         mumps_data_funcs = {'prevalence': lambda _, __: build_table(1.0, year_start-1, year_end,
 #                                                                     ['age', 'year', 'sex', 'value']),
 #                             'disability_weight': lambda _, __: 0.4,
 #                             'dwell_time': lambda _, __: pd.Timedelta(days=1),
-#                             'excess_mortality': lambda _, __: build_table(0, year_start-1, year_end)}
+#                             'excess_mortality_rate': lambda _, __: build_table(0, year_start-1, year_end)}
 #         mumps = ExcessMortalityState('mumps', get_data_functions=mumps_data_funcs)
 #         mumps_model = DiseaseModel('mumps', states=[mumps],
 #                                    initial_state=mumps,
 #                                    get_data_functions={'csmr': lambda _, __: build_table(0, year_start-1, year_end)})
 #         components.append(mumps_model)
 #
 #     if deadly:
 #         deadly_data_funcs = {'prevalence': lambda _, __: build_table(0.1, year_start-1, year_end,
 #                                                                      ['age', 'year', 'sex', 'value']),
 #                              'disability_weight': lambda _, __: 0.4,
 #                              'dwell_time': lambda _, __: pd.Timedelta(days=1),
-#                              'excess_mortality': lambda _, __: build_table(0.005, year_start-1, year_end)}
+#                              'excess_mortality_rate': lambda _, __: build_table(0.005, year_start-1, year_end)}
 #         deadly = ExcessMortalityState('deadly', get_data_functions=deadly_data_funcs)
 #         healthy = DiseaseState('healthy', get_data_functions=deadly_data_funcs)
 #         deadly_model = DiseaseModel('deadly', initial_state=healthy,
 #                                     states=[deadly, healthy],
 #                                     get_data_functions={
 #                                         'csmr': lambda _, __: build_table(0.0005, year_start-1, year_end)
 #                                     })
```

### Comparing `vivarium_public_health-0.9.9/tests/population/test_add_new_birth_cohort.py` & `vivarium_public_health-1.0.0/tests/population/test_add_new_birth_cohort.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,211 @@
-import pytest
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
+import pytest
+from vivarium import InteractiveContext
+from vivarium.testing_utilities import TestPopulation, build_table, metadata
 
-from vivarium.testing_utilities import TestPopulation, metadata, build_table
-from vivarium.interface.interactive import setup_simulation, initialize_simulation
-
-from vivarium_public_health.population import FertilityDeterministic, FertilityCrudeBirthRate, FertilityAgeSpecificRates
+from vivarium_public_health import utilities
+from vivarium_public_health.population import (
+    FertilityAgeSpecificRates,
+    FertilityCrudeBirthRate,
+    FertilityDeterministic,
+)
 
 
 @pytest.fixture()
 def config(base_config):
-    base_config.update({
-        'population': {
-            'population_size': 10000,
-            'age_start': 0,
-            'age_end': 125,
+    base_config.update(
+        {
+            "population": {
+                "population_size": 10000,
+                "age_start": 0,
+                "age_end": 125,
+            },
+            "time": {
+                "step_size": 10,
+            },
         },
-        'time': {
-            'step_size': 10,
-            }
-        }, **metadata(__file__))
+        source=str(Path(__file__).resolve()),
+        layer="override",
+    )
     return base_config
 
 
 def crude_birth_rate_data(live_births=500):
-    return (build_table(['mean_value', live_births], 1990, 2017, ('age', 'year', 'sex', 'parameter', 'value'))
-            .query('age_group_start == 25 and sex != "Both"')
-            .drop(['age_group_start', 'age_group_end'], 'columns'))
+    return (
+        build_table(
+            ["mean_value", live_births],
+            1990,
+            2017,
+            ("age", "year", "sex", "parameter", "value"),
+        )
+        .query('age_start == 25 and sex != "Both"')
+        .drop(columns=["age_start", "age_end"])
+    )
 
 
 def test_FertilityDeterministic(config):
     pop_size = config.population.population_size
     annual_new_simulants = 1000
     step_size = config.time.step_size
     num_days = 100
 
-    config.update({
-        'fertility': {
-            'number_of_new_simulants_each_year': annual_new_simulants
-        }
-    }, **metadata(__file__))
+    config.update(
+        {"fertility": {"number_of_new_simulants_each_year": annual_new_simulants}},
+        **metadata(__file__)
+    )
 
     components = [TestPopulation(), FertilityDeterministic()]
-    simulation = setup_simulation(components, config)
+    simulation = InteractiveContext(components=components, configuration=config)
     num_steps = simulation.run_for(duration=pd.Timedelta(days=num_days))
     pop = simulation.get_population()
 
     assert num_steps == num_days // step_size
-    assert np.all(pop.alive == 'alive')
-    assert int(num_days * annual_new_simulants / 365) == len(pop.age) - pop_size
+    assert np.all(pop.alive == "alive")
+    assert (
+        int(num_days * annual_new_simulants / utilities.DAYS_PER_YEAR)
+        == len(pop.age) - pop_size
+    )
 
 
 def test_FertilityCrudeBirthRate(config, base_plugins):
     pop_size = config.population.population_size
     num_days = 100
     components = [TestPopulation(), FertilityCrudeBirthRate()]
-    simulation = initialize_simulation(components, config, base_plugins)
-    simulation.data.write("covariate.live_births_by_sex.estimate", crude_birth_rate_data())
+    simulation = InteractiveContext(
+        components=components,
+        configuration=config,
+        plugin_configuration=base_plugins,
+        setup=False,
+    )
+    simulation._data.write("covariate.live_births_by_sex.estimate", crude_birth_rate_data())
 
     simulation.setup()
     simulation.run_for(duration=pd.Timedelta(days=num_days))
     pop = simulation.get_population()
 
-    assert np.all(pop.alive == 'alive')
+    assert np.all(pop.alive == "alive")
     assert len(pop.age) > pop_size
 
 
 def test_FertilityCrudeBirthRate_extrapolate_fail(config, base_plugins):
-    config.update({
-        'interpolation': {
-            'extrapolate': False
-        },
-        'time': {
-            'start': {'year': 2016},
-            'end': {'year': 2025},
-            'step_size': 30,
-        },
-    })
+    config.update(
+        {
+            "interpolation": {"extrapolate": False},
+            "time": {
+                "start": {"year": 2016},
+                "end": {"year": 2025},
+            },
+        }
+    )
     components = [TestPopulation(), FertilityCrudeBirthRate()]
 
-    simulation = initialize_simulation(components, config, base_plugins)
-    simulation.data.write("covariate.live_births_by_sex.estimate", crude_birth_rate_data())
+    simulation = InteractiveContext(
+        components=components,
+        configuration=config,
+        plugin_configuration=base_plugins,
+        setup=False,
+    )
+    simulation._data.write("covariate.live_births_by_sex.estimate", crude_birth_rate_data())
 
     with pytest.raises(ValueError):
         simulation.setup()
 
 
-def test_FertilityCrudeBirthRate_extrapolate(config, base_plugins):
-    config.update({
-        'interpolation': {
-            'extrapolate': True
-        },
-        'time': {
-            'start': {'year': 2016},
-            'end': {'year': 2026},
-            'step_size': 365,
-        },
-    })
-    pop_size = config.population.population_size
-    true_pop_size = 8000  # What's available in the mock artifact
+def test_FertilityCrudeBirthRate_extrapolate(base_config, base_plugins):
+    base_config.update(
+        {
+            "population": {
+                "population_size": 10000,
+                "age_start": 0,
+                "age_end": 125,
+            },
+            "interpolation": {"extrapolate": True},
+            "time": {
+                "start": {"year": 2016},
+                "end": {"year": 2026},
+                "step_size": 365,
+            },
+        }
+    )
+    pop_size = base_config.population.population_size
+    true_pop_size = 50000  # What's available in the mock artifact
     live_births_by_sex = 500
     components = [TestPopulation(), FertilityCrudeBirthRate()]
 
-    simulation = initialize_simulation(components, config, base_plugins)
-    simulation.data.write("covariate.live_births_by_sex.estimate", crude_birth_rate_data(live_births_by_sex))
+    simulation = InteractiveContext(
+        components=components,
+        configuration=base_config,
+        plugin_configuration=base_plugins,
+        setup=False,
+    )
+    simulation._data.write(
+        "covariate.live_births_by_sex.estimate", crude_birth_rate_data(live_births_by_sex)
+    )
     simulation.setup()
 
     birth_rate = []
     for i in range(10):
         pop_start = len(simulation.get_population())
         simulation.step()
         pop_end = len(simulation.get_population())
-        birth_rate.append((pop_end - pop_start)/pop_size)
+        birth_rate.append((pop_end - pop_start) / pop_size)
 
-    given_birth_rate = 2*live_births_by_sex / true_pop_size
+    given_birth_rate = 2 * live_births_by_sex / true_pop_size
     np.testing.assert_allclose(birth_rate, given_birth_rate, atol=0.01)
 
 
 def test_fertility_module(base_config, base_plugins):
     start_population_size = 1000
     num_days = 1000
     time_step = 10  # Days
-    base_config.update({
-        'population': {
-            'population_size': start_population_size,
-            'age_start': 0,
-            'age_end': 125},
-        'time': {'step_size': time_step}
-    }, layer='override')
+    base_config.update(
+        {
+            "population": {
+                "population_size": start_population_size,
+                "age_start": 0,
+                "age_end": 125,
+            },
+            "time": {"step_size": time_step},
+        },
+        layer="override",
+    )
 
     components = [TestPopulation(), FertilityAgeSpecificRates()]
-    simulation = initialize_simulation(components, base_config, base_plugins)
+    simulation = simulation = InteractiveContext(
+        components=components,
+        configuration=base_config,
+        plugin_configuration=base_plugins,
+        setup=False,
+    )
 
-    asfr_data = build_table(0.05, 1990, 2017).rename(columns={'value': 'mean_value'})
-    simulation.data.write("covariate.age_specific_fertility_rate.estimate", asfr_data)
+    asfr_data = build_table(0.05, 1990, 2017).rename(columns={"value": "mean_value"})
+    simulation._data.write("covariate.age_specific_fertility_rate.estimate", asfr_data)
 
     simulation.setup()
 
-    time_start = simulation.clock.time
+    time_start = simulation._clock.time
 
-    assert 'last_birth_time' in simulation.get_population().columns,\
-        'expect Fertility module to update state table.'
-    assert 'parent_id' in simulation.get_population().columns, \
-        'expect Fertility module to update state table.'
+    assert (
+        "last_birth_time" in simulation.get_population().columns
+    ), "expect Fertility module to update state table."
+    assert (
+        "parent_id" in simulation.get_population().columns
+    ), "expect Fertility module to update state table."
 
     simulation.run_for(duration=pd.Timedelta(days=num_days))
     pop = simulation.get_population()
 
     # No death in this model.
-    assert np.all(pop.alive == 'alive'), 'expect all simulants to be alive'
+    assert np.all(pop.alive == "alive"), "expect all simulants to be alive"
 
     # TODO: Write a more rigorous test.
-    assert len(pop.age) > start_population_size, 'expect new simulants'
+    assert len(pop.age) > start_population_size, "expect new simulants"
 
     for i in range(start_population_size, len(pop)):
-        assert pop.loc[pop.iloc[i].parent_id].last_birth_time >= time_start, 'expect all children to have mothers who' \
-                                                                          ' gave birth after the simulation starts.'
+        assert pop.loc[pop.iloc[i].parent_id].last_birth_time >= time_start, (
+            "expect all children to have mothers who"
+            " gave birth after the simulation starts."
+        )
```

### Comparing `vivarium_public_health-0.9.9/tests/population/test_base_population.py` & `vivarium_public_health-1.0.0/tests/population/test_base_population.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,277 +1,376 @@
 import math
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pytest
-
-from vivarium.testing_utilities import get_randomness, metadata
-from vivarium.interface.interactive import setup_simulation
+from vivarium import InteractiveContext
+from vivarium.testing_utilities import get_randomness
 
 import vivarium_public_health.population.base_population as bp
 import vivarium_public_health.population.data_transformations as dt
+from vivarium_public_health import utilities
 from vivarium_public_health.testing.utils import make_uniform_pop_data
 
 
 @pytest.fixture
 def config(base_config):
-    base_config.update({
-        'population': {
-            'age_start': 0,
-            'age_end': 110,
+    base_config.update(
+        {
+            "population": {
+                "age_start": 0,
+                "age_end": 110,
+            },
         },
-        'input_data': {
-            'location_id': 180,
-            'use_subregions': False,
-        }
-    }, **metadata(__file__))
+        source=str(Path(__file__).resolve()),
+        layer="model_override",
+    )
     return base_config
 
 
 @pytest.fixture
 def generate_population_mock(mocker):
-    return mocker.patch('vivarium_public_health.population.base_population.generate_population')
+    return mocker.patch(
+        "vivarium_public_health.population.base_population.generate_population"
+    )
 
 
 @pytest.fixture
 def age_bounds_mock(mocker):
-    return mocker.patch('vivarium_public_health.population.base_population._assign_demography_with_age_bounds')
+    return mocker.patch(
+        "vivarium_public_health.population.base_population._assign_demography_with_age_bounds"
+    )
 
 
 @pytest.fixture
 def initial_age_mock(mocker):
-    return mocker.patch('vivarium_public_health.population.base_population._assign_demography_with_initial_age')
+    return mocker.patch(
+        "vivarium_public_health.population.base_population._assign_demography_with_initial_age"
+    )
 
 
 def make_base_simulants():
     simulant_ids = range(100000)
     creation_time = pd.Timestamp(1990, 7, 2)
-    return pd.DataFrame({'entrance_time': pd.Series(pd.Timestamp(creation_time), index=simulant_ids),
-                         'exit_time': pd.Series(pd.NaT, index=simulant_ids),
-                         'alive': pd.Series('alive', index=simulant_ids)},
-                        index=simulant_ids)
+    return pd.DataFrame(
+        {
+            "entrance_time": pd.Series(pd.Timestamp(creation_time), index=simulant_ids),
+            "exit_time": pd.Series(pd.NaT, index=simulant_ids),
+            "alive": pd.Series("alive", index=simulant_ids),
+        },
+        index=simulant_ids,
+    )
 
 
 def make_full_simulants():
     base_simulants = make_base_simulants()
-    base_simulants['location'] = pd.Series(1, index=base_simulants.index)
-    base_simulants['sex'] = pd.Series('Male', index=base_simulants.index).astype(
-        pd.api.types.CategoricalDtype(categories=['Male', 'Female'], ordered=False))
-    base_simulants['age'] = np.random.uniform(0, 100, len(base_simulants))
-    base_simulants['tracked'] = pd.Series(True, index=base_simulants.index)
+    base_simulants["location"] = pd.Series(1, index=base_simulants.index)
+    base_simulants["sex"] = pd.Series("Male", index=base_simulants.index).astype(
+        pd.api.types.CategoricalDtype(categories=["Male", "Female"], ordered=False)
+    )
+    base_simulants["age"] = np.random.uniform(0, 100, len(base_simulants))
+    base_simulants["tracked"] = pd.Series(True, index=base_simulants.index)
     return base_simulants
 
 
 def test_select_sub_population_data():
-    data = pd.DataFrame({'year_start': [1990, 1995, 2000, 2005],
-                         'year_end': [1995, 2000, 2005, 2010],
-                         'population': [100, 110, 120, 130]})
+    data = pd.DataFrame(
+        {
+            "year_start": [1990, 1995, 2000, 2005],
+            "year_end": [1995, 2000, 2005, 2010],
+            "population": [100, 110, 120, 130],
+        }
+    )
 
-    sub_pop = bp.BasePopulation.select_sub_population_data(data, 1997)
+    sub_pop = bp.BasePopulation.get_demographic_proportions_for_creation_time(data, 1997)
 
     assert sub_pop.year_start.values.item() == 1995
 
 
-def test_BasePopulation(config, base_plugins, generate_population_mock):
+def test_BasePopulation(config, base_plugins, generate_population_mock, include_sex):
     num_days = 600
     time_step = 100  # Days
     sims = make_full_simulants()
     start_population_size = len(sims)
 
-    generate_population_mock.return_value = sims
+    generate_population_mock.return_value = sims.drop(columns=["tracked"])
 
     base_pop = bp.BasePopulation()
 
     components = [base_pop]
-    config.update({'population': {'population_size': start_population_size},
-                   'time': {'step_size': time_step}}, layer='override')
-    simulation = setup_simulation(components, input_config=config, plugin_config=base_plugins)
-    time_start = simulation.clock.time
-
-    pop_structure = simulation.data.load('population.structure')
-    pop_structure['location'] = simulation.configuration.input_data.location
-    uniform_pop = dt.assign_demographic_proportions(pop_structure)
-
-    assert base_pop.population_data.equals(uniform_pop)
-
-    age_params = {'age_start': config.population.age_start,
-                  'age_end': config.population.age_end}
-    sub_pop = bp.BasePopulation.select_sub_population_data(uniform_pop, time_start.year)
+    config.update(
+        {
+            "population": {
+                "population_size": start_population_size,
+                "include_sex": include_sex,
+            },
+            "time": {"step_size": time_step},
+        },
+        layer="override",
+    )
+    simulation = InteractiveContext(
+        components=components, configuration=config, plugin_configuration=base_plugins
+    )
+    time_start = simulation._clock.time
+
+    pop_structure = simulation._data.load("population.structure")
+    uniform_pop = dt.assign_demographic_proportions(pop_structure, include_sex)
+
+    assert base_pop.demographic_proportions.equals(uniform_pop)
+
+    age_params = {
+        "age_start": config.population.age_start,
+        "age_end": config.population.age_end,
+    }
+    sub_pop = bp.BasePopulation.get_demographic_proportions_for_creation_time(
+        uniform_pop, time_start.year
+    )
 
     generate_population_mock.assert_called_once()
     # Get a dictionary of the arguments used in the call
     mock_args = generate_population_mock.call_args[1]
-    assert mock_args['creation_time'] == time_start - simulation.clock.step_size
-    assert mock_args['age_params'] == age_params
-    assert mock_args['population_data'].equals(sub_pop)
-    assert mock_args['randomness_streams'] == base_pop.randomness
+    assert mock_args["creation_time"] == time_start - simulation._clock.step_size
+    assert mock_args["age_params"] == age_params
+    assert mock_args["demographic_proportions"].equals(sub_pop)
+    assert mock_args["randomness_streams"] == base_pop.randomness
     pop = simulation.get_population()
     for column in pop:
         assert pop[column].equals(sims[column])
 
-    final_ages = pop.age + num_days/365
+    final_ages = pop.age + num_days / utilities.DAYS_PER_YEAR
 
     simulation.run_for(duration=pd.Timedelta(days=num_days))
 
     pop = simulation.get_population()
-    assert np.allclose(pop.age, final_ages, atol=0.5/365)  # Within a half of a day.
+    assert np.allclose(
+        pop.age, final_ages, atol=0.5 / utilities.DAYS_PER_YEAR
+    )  # Within a half of a day.
 
 
 def test_age_out_simulants(config, base_plugins):
     start_population_size = 10000
     num_days = 600
     time_step = 100  # Days
-    config.update({'population': {
-        'population_size': start_population_size,
-        'age_start': 4,
-        'age_end': 4,
-        'exit_age': 5,
-    },
-        'time': {'step_size': time_step}
-    }, layer='override')
+    config.update(
+        {
+            "population": {
+                "population_size": start_population_size,
+                "age_start": 4,
+                "age_end": 4,
+                "exit_age": 5,
+            },
+            "time": {"step_size": time_step},
+        },
+        layer="override",
+    )
     components = [bp.BasePopulation()]
-    simulation = setup_simulation(components, input_config=config, plugin_config=base_plugins)
-    time_start = simulation.clock.time
-
+    simulation = InteractiveContext(
+        components=components, configuration=config, plugin_configuration=base_plugins
+    )
+    time_start = simulation._clock.time
     assert len(simulation.get_population()) == len(simulation.get_population().age.unique())
     simulation.run_for(duration=pd.Timedelta(days=num_days))
     pop = simulation.get_population()
     assert len(pop) == len(pop[~pop.tracked])
-    exit_after_300_days = pop.exit_time >= time_start + pd.Timedelta(300, unit='D')
-    exit_before_400_days = pop.exit_time <= time_start + pd.Timedelta(400, unit='D')
+    exit_after_300_days = pop.exit_time >= time_start + pd.Timedelta(300, unit="D")
+    exit_before_400_days = pop.exit_time <= time_start + pd.Timedelta(400, unit="D")
     assert len(pop) == len(pop[exit_after_300_days & exit_before_400_days])
 
 
-def test_generate_population_age_bounds(age_bounds_mock, initial_age_mock):
+def test_generate_population_age_bounds(age_bounds_mock, initial_age_mock, include_sex):
     creation_time = pd.Timestamp(1990, 7, 2)
     step_size = pd.Timedelta(days=1)
-    age_params = {'age_start': 0,
-                  'age_end': 120}
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
+    age_params = {"age_start": 0, "age_end": 120}
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
     sims = make_base_simulants()
     simulant_ids = sims.index
 
-    bp.generate_population(simulant_ids, creation_time, step_size,
-                           age_params, pop_data, r, lambda *args, **kwargs: None)
+    bp.generate_population(
+        simulant_ids,
+        creation_time,
+        step_size,
+        age_params,
+        pop_data,
+        r,
+        lambda *args, **kwargs: None,
+    )
 
     age_bounds_mock.assert_called_once()
     mock_args = age_bounds_mock.call_args[0]
     assert mock_args[0].equals(sims)
     assert mock_args[1].equals(pop_data)
-    assert mock_args[2] == float(age_params['age_start'])
-    assert mock_args[3] == float(age_params['age_end'])
+    assert mock_args[2] == float(age_params["age_start"])
+    assert mock_args[3] == float(age_params["age_end"])
     assert mock_args[4] == r
     initial_age_mock.assert_not_called()
 
 
-def test_generate_population_initial_age(age_bounds_mock, initial_age_mock):
+def test_generate_population_initial_age(age_bounds_mock, initial_age_mock, include_sex):
     creation_time = pd.Timestamp(1990, 7, 2)
     step_size = pd.Timedelta(days=1)
-    age_params = {'age_start': 0,
-                  'age_end': 0}
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
+    age_params = {"age_start": 0, "age_end": 0}
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
     sims = make_base_simulants()
     simulant_ids = sims.index
 
-    bp.generate_population(simulant_ids, creation_time, step_size,
-                           age_params, pop_data, r, lambda *args, **kwargs: None)
+    bp.generate_population(
+        simulant_ids,
+        creation_time,
+        step_size,
+        age_params,
+        pop_data,
+        r,
+        lambda *args, **kwargs: None,
+    )
 
     initial_age_mock.assert_called_once()
     mock_args = initial_age_mock.call_args[0]
     assert mock_args[0].equals(sims)
     assert mock_args[1].equals(pop_data)
 
-    assert mock_args[2] == float(age_params['age_start'])
+    assert mock_args[2] == float(age_params["age_start"])
     assert mock_args[3] == step_size
     assert mock_args[4] == r
     age_bounds_mock.assert_not_called()
 
 
-def test__assign_demography_with_initial_age(config):
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
+def test__assign_demography_with_initial_age(config, include_sex):
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
     pop_data = pop_data[pop_data.year_start == 1990]
     simulants = make_base_simulants()
     initial_age = 20
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
     step_size = pd.Timedelta(days=config.time.step_size)
 
-    simulants = bp._assign_demography_with_initial_age(simulants, pop_data, initial_age,
-                                                       step_size, r, lambda *args, **kwargs: None)
+    simulants = bp._assign_demography_with_initial_age(
+        simulants, pop_data, initial_age, step_size, r, lambda *args, **kwargs: None
+    )
+    _check_population(simulants, initial_age, step_size, include_sex)
 
-    assert len(simulants) == len(simulants.age.unique())
-    assert simulants.age.min() > initial_age
-    assert simulants.age.max() < initial_age + step_size.days/365.0
-    assert math.isclose(len(simulants[simulants.sex == 'Male']) / len(simulants), 0.5, abs_tol=0.01)
-    for location in simulants.location.unique():
-        assert math.isclose(len(simulants[simulants.location == location]) / len(simulants),
-                            1 / len(simulants.location.unique()), abs_tol=0.01)
 
-
-def test__assign_demography_with_initial_age_zero(config):
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
+def test__assign_demography_with_initial_age_zero(config, include_sex):
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
     pop_data = pop_data[pop_data.year_start == 1990]
     simulants = make_base_simulants()
     initial_age = 0
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
-    step_size = pd.Timedelta(days=config.time.step_size)
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
+    step_size = utilities.to_time_delta(config.time.step_size)
 
-    simulants = bp._assign_demography_with_initial_age(simulants, pop_data, initial_age,
-                                                       step_size, r, lambda *args, **kwargs: None)
-
-    assert len(simulants) == len(simulants.age.unique())
-    assert simulants.age.min() > initial_age
-    assert simulants.age.max() < initial_age + step_size.days / 365.0
-    assert math.isclose(len(simulants[simulants.sex == 'Male']) / len(simulants), 0.5, abs_tol=0.01)
-    for location in simulants.location.unique():
-        assert math.isclose(len(simulants[simulants.location == location]) / len(simulants),
-                            1 / len(simulants.location.unique()), abs_tol=0.01)
+    simulants = bp._assign_demography_with_initial_age(
+        simulants, pop_data, initial_age, step_size, r, lambda *args, **kwargs: None
+    )
+    _check_population(simulants, initial_age, step_size, include_sex)
 
 
-def test__assign_demography_with_initial_age_error():
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
+def test__assign_demography_with_initial_age_error(include_sex):
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
     pop_data = pop_data[pop_data.year_start == 1990]
     simulants = make_base_simulants()
     initial_age = 200
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
     step_size = pd.Timedelta(days=1)
 
     with pytest.raises(ValueError):
-        bp._assign_demography_with_initial_age(simulants, pop_data, initial_age,
-                                               step_size, r, lambda *args, **kwargs: None)
+        bp._assign_demography_with_initial_age(
+            simulants, pop_data, initial_age, step_size, r, lambda *args, **kwargs: None
+        )
 
 
-def test__assign_demography_with_age_bounds():
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
+@pytest.mark.parametrize(["age_start", "age_end"], [[0, 180], [5, 50], [12, 57]])
+def test__assign_demography_with_age_bounds(include_sex, age_start, age_end):
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
     pop_data = pop_data[pop_data.year_start == 1990]
     simulants = make_base_simulants()
-    age_start, age_end = 0, 180
-    r = {k: get_randomness(k) for k in ['general_purpose', 'bin_selection', 'age_smoothing', 'age_smoothing_age_bounds']}
+    r = {
+        k: get_randomness(k)
+        for k in [
+            "general_purpose",
+            "bin_selection",
+            "age_smoothing",
+            "age_smoothing_age_bounds",
+        ]
+    }
+
+    simulants = bp._assign_demography_with_age_bounds(
+        simulants, pop_data, age_start, age_end, r, lambda *args, **kwargs: None
+    )
 
-    simulants = bp._assign_demography_with_age_bounds(simulants, pop_data, age_start,
-                                                      age_end, r, lambda *args, **kwargs: None)
+    _check_sexes(simulants, include_sex)
+    _check_locations(simulants)
 
-    assert math.isclose(len(simulants[simulants.sex == 'Male']) / len(simulants), 0.5, abs_tol=0.01)
-
-    for location in simulants.location.unique():
-        assert math.isclose(len(simulants[simulants.location == location]) / len(simulants),
-                            1 / len(simulants.location.unique()), abs_tol=0.01)
     ages = np.sort(simulants.age.values)
     age_deltas = ages[1:] - ages[:-1]
 
-    age_bin_width = 5  # See `make_uniform_pop_data`
-    num_bins = len(pop_data.age.unique())
-    n = len(simulants)
-    assert math.isclose(age_deltas.mean(), age_bin_width * num_bins / n, rel_tol=1e-3)
-    assert age_deltas.max() < 100 * age_bin_width * num_bins / n  # Make sure there are no big age gaps.
+    age_start = max(pop_data.age_start.min(), age_start)
+    age_end = min(pop_data.age_end.max(), age_end)
+    expected_average_delta = (age_end - age_start) / len(simulants)
+
+    assert math.isclose(age_deltas.mean(), expected_average_delta, rel_tol=1e-2)
+    # Make sure there are no big age gaps.
+    assert age_deltas.max() < 100 * expected_average_delta
 
 
-def test__assign_demography_withq_age_bounds_error():
-    pop_data = dt.assign_demographic_proportions(make_uniform_pop_data(age_bin_midpoint=True))
+def test__assign_demography_with_age_bounds_error(include_sex):
+    pop_data = dt.assign_demographic_proportions(
+        make_uniform_pop_data(age_bin_midpoint=True),
+        include_sex=include_sex,
+    )
     simulants = make_base_simulants()
-    age_start, age_end = 110, 120
-    r = {k: get_randomness() for k in ['general_purpose', 'bin_selection', 'age_smoothing']}
+    age_start, age_end = 130, 140
+    r = {k: get_randomness() for k in ["general_purpose", "bin_selection", "age_smoothing"]}
 
     with pytest.raises(ValueError):
-        bp._assign_demography_with_age_bounds(simulants, pop_data, age_start,
-                                              age_end, r, lambda *args, **kwargs: None)
+        bp._assign_demography_with_age_bounds(
+            simulants, pop_data, age_start, age_end, r, lambda *args, **kwargs: None
+        )
+
+
+def _check_population(simulants, initial_age, step_size, include_sex):
+    assert len(simulants) == len(simulants.age.unique())
+    assert simulants.age.min() > initial_age
+    assert simulants.age.max() < initial_age + utilities.to_years(step_size)
+    _check_sexes(simulants, include_sex)
+    _check_locations(simulants)
+
+
+def _check_sexes(simulants, include_sex):
+    male_prob, female_prob = {
+        "Male": (1.0, 0.0),
+        "Female": (0.0, 1.0),
+        "Both": (0.5, 0.5),
+    }[include_sex]
+    for sex, prob in [("Male", male_prob), ("Female", female_prob)]:
+        assert math.isclose(
+            len(simulants[simulants.sex == sex]) / len(simulants),
+            prob,
+            abs_tol=0.01,
+        )
+
+
+def _check_locations(simulants):
+    for location in simulants.location.unique():
+        assert math.isclose(
+            len(simulants[simulants.location == location]) / len(simulants),
+            1 / len(simulants.location.unique()),
+            abs_tol=0.01,
+        )
```

### Comparing `vivarium_public_health-0.9.9/tests/risks/test_base_risk.py` & `vivarium_public_health-1.0.0/tests/risks/test_base_risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.9/tests/risks/test_distributions.py` & `vivarium_public_health-1.0.0/tests/risks/test_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 #     test_df = pd.concat(test_df)
 #
 #     expected = []
 #
 #     for cat, value in zip (['cat1', 'cat2'], [0.6, 0.4]):
 #         expected.append(build_table([cat, value], year_start, year_end, ('age', 'year', 'sex', 'parameter', 'value')))
 #
-#     expected = pd.concat(expected).loc[:, ['age_group_start', 'age_group_end', 'year_start',
+#     expected = pd.concat(expected).loc[:, ['age_start', 'age_end', 'year_start',
 #                                            'year_end', 'sex', 'parameter', 'value']]
 #     rebinned = distributions.rebin_exposure_data(test_df).loc[:, expected.columns]
-#     expected = expected.set_index(['age_group_start', 'year_start', 'sex'])
-#     rebinned = rebinned.set_index(['age_group_start', 'year_start', 'sex'])
+#     expected = expected.set_index(['age_start', 'year_start', 'sex'])
+#     rebinned = rebinned.set_index(['age_start', 'year_start', 'sex'])
 #
 #     assert np.allclose(expected.value[expected.parameter == 'cat1'], rebinned.value[rebinned.parameter=='cat1'])
 #     assert np.allclose(expected.value[expected.parameter == 'cat2'], rebinned.value[rebinned.parameter == 'cat2'])
 #
 #
 # def test_get_distribution_dichotomous_risk():
 #
```

### Comparing `vivarium_public_health-0.9.9/tests/risks/conftest.py` & `vivarium_public_health-1.0.0/tests/risks/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,186 +1,251 @@
-import pytest
 from typing import List
-import pandas as pd
 
+import pandas as pd
+import pytest
 from vivarium.testing_utilities import build_table
+
 from vivarium_public_health.risks.base_risk import Risk
 
 
-def make_test_data_table(values: List, parameter='cat') -> pd.DataFrame:
+def make_test_data_table(values: List, parameter="cat") -> pd.DataFrame:
     year_start = 1990  # same as the base config
     year_end = 2010
 
     if len(values) == 1:
-        df = build_table(values[0], year_start, year_end, ('age', 'year', 'sex', 'value'))
+        df = build_table(values[0], year_start, year_end, ("age", "year", "sex", "value"))
     else:
-        cats = [f'{parameter}{i+1}' for i in range(len(values))] if parameter == 'cat' else parameter
+        cats = (
+            [f"{parameter}{i+1}" for i in range(len(values))]
+            if parameter == "cat"
+            else parameter
+        )
         df = []
         for cat, value in zip(cats, values):
-            df.append(build_table([cat, value], year_start, year_end, ('age','year', 'sex', 'parameter', 'value')))
+            df.append(
+                build_table(
+                    [cat, value],
+                    year_start,
+                    year_end,
+                    ("age", "year", "sex", "parameter", "value"),
+                )
+            )
         df = pd.concat(df)
     return df
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def continuous_risk():
     year_start = 1990
     year_end = 2010
-    risk = 'test_risk'
+    risk = "test_risk"
     risk_data = dict()
     exposure_mean = make_test_data_table([130])
     exposure_sd = make_test_data_table([15])
     affected_causes = ["test_cause_1", "test_cause_2"]
     rr_data = []
     paf_data = []
     for cause in affected_causes:
         rr_data.append(
-            build_table([1.01, cause], year_start, year_end, ['age', 'sex', 'year', 'value', 'cause'],
-                        ).melt(id_vars=('age_group_start', 'age_group_end', 'year_start',
-                                        'year_end', 'sex', 'cause'), var_name='parameter', value_name='value')
+            build_table(
+                [1.01, cause],
+                year_start,
+                year_end,
+                ["age", "sex", "year", "value", "cause"],
+            ).melt(
+                id_vars=("age_start", "age_end", "year_start", "year_end", "sex", "cause"),
+                var_name="parameter",
+                value_name="value",
+            )
+        )
+        paf_data.append(
+            build_table(
+                [1, cause], year_start, year_end, ["age", "sex", "year", "value", "cause"]
+            )
         )
-        paf_data.append(build_table([1, cause], year_start, year_end, ['age', 'sex', 'year', 'value', 'cause']))
     rr_data = pd.concat(rr_data)
     paf_data = pd.concat(paf_data)
-    paf_data['affected_measure'] = 'incidence_rate'
-    rr_data['affected_measure'] = 'incidence_rate'
-    risk_data['exposure'] = exposure_mean
-    risk_data['exposure_standard_deviation'] = exposure_sd
-    risk_data['relative_risk'] = rr_data
-    risk_data['population_attributable_fraction'] = paf_data
-    risk_data['affected_causes'] = affected_causes
-    risk_data['affected_risk_factors'] = []
+    paf_data["affected_measure"] = "incidence_rate"
+    rr_data["affected_measure"] = "incidence_rate"
+    risk_data["exposure"] = exposure_mean
+    risk_data["exposure_standard_deviation"] = exposure_sd
+    risk_data["relative_risk"] = rr_data
+    risk_data["population_attributable_fraction"] = paf_data
+    risk_data["affected_causes"] = affected_causes
+    risk_data["affected_risk_factors"] = []
 
     tmred = {
-        "distribution": 'uniform',
+        "distribution": "uniform",
         "min": 110.0,
         "max": 115.0,
         "inverted": False,
     }
     exposure_parameters = {
         "scale": 10.0,
         "max_rr": 200.0,
         "max_val": 300.0,
         "min_val": 50.0,
     }
     tmrel = 0.5 * (tmred["max"] + tmred["min"])
-    risk_data['tmred'] = tmred
-    risk_data['tmrel'] = tmrel
-    risk_data['exposure_parameters'] = exposure_parameters
-    risk_data['distribution'] = 'normal'
+    risk_data["tmred"] = tmred
+    risk_data["tmrel"] = tmrel
+    risk_data["exposure_parameters"] = exposure_parameters
+    risk_data["distribution"] = "normal"
 
     return Risk(f"risk_factor.{risk}"), risk_data
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def dichotomous_risk():
     year_start = 1990
     year_end = 2010
-    risk = 'test_risk'
+    risk = "test_risk"
     risk_data = dict()
     exposure_data = build_table(
-        0.5, year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2']
-    ).melt(id_vars=('age_group_start', 'age_group_end',
-                    'year_start', 'year_end', 'sex'), var_name='parameter', value_name='value')
+        0.5, year_start, year_end, ["age", "year", "sex", "cat1", "cat2"]
+    ).melt(
+        id_vars=("age_start", "age_end", "year_start", "year_end", "sex"),
+        var_name="parameter",
+        value_name="value",
+    )
 
     affected_causes = ["test_cause_1", "test_cause_2"]
     rr_data = []
     paf_data = []
     for cause in affected_causes:
         rr_data.append(
             build_table(
-                [1.01, 1, cause], year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2', 'cause']
-            ).melt(id_vars=('age_group_start', 'age_group_end', 'year_start',
-                            'year_end', 'sex', 'cause'), var_name='parameter', value_name='value')
+                [1.01, 1, cause],
+                year_start,
+                year_end,
+                ["age", "year", "sex", "cat1", "cat2", "cause"],
+            ).melt(
+                id_vars=("age_start", "age_end", "year_start", "year_end", "sex", "cause"),
+                var_name="parameter",
+                value_name="value",
+            )
+        )
+        paf_data.append(
+            build_table(
+                [1, cause], year_start, year_end, ["age", "sex", "year", "value", "cause"]
+            )
         )
-        paf_data.append(build_table([1, cause], year_start, year_end, ['age', 'sex', 'year', 'value', 'cause']))
     rr_data = pd.concat(rr_data)
     paf_data = pd.concat(paf_data)
-    paf_data['affected_measure'] = 'incidence_rate'
-    rr_data['affected_measure'] = 'incidence_rate'
-    risk_data['exposure'] = exposure_data
-    risk_data['relative_risk'] = rr_data
-    risk_data['population_attributable_fraction'] = paf_data
-    risk_data['affected_causes'] = affected_causes
-    risk_data['affected_risk_factors'] = []
+    paf_data["affected_measure"] = "incidence_rate"
+    rr_data["affected_measure"] = "incidence_rate"
+    risk_data["exposure"] = exposure_data
+    risk_data["relative_risk"] = rr_data
+    risk_data["population_attributable_fraction"] = paf_data
+    risk_data["affected_causes"] = affected_causes
+    risk_data["affected_risk_factors"] = []
     incidence_rate = build_table(0.01, year_start, year_end)
-    risk_data['incidence_rate'] = incidence_rate
-    risk_data['distribution'] = 'dichotomous'
-    return Risk(f'risk_factor.{risk}'), risk_data
+    risk_data["incidence_rate"] = incidence_rate
+    risk_data["distribution"] = "dichotomous"
+    return Risk(f"risk_factor.{risk}"), risk_data
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def polytomous_risk():
     year_start = 1990
     year_end = 2010
-    risk = 'test_risk'
+    risk = "test_risk"
     risk_data = dict()
     exposure_data = build_table(
-        0.25, year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2', 'cat3', 'cat4']
-    ).melt(id_vars=('age_group_start', 'age_group_end',
-                    'year_start', 'year_end', 'sex'), var_name='parameter', value_name='value')
+        0.25, year_start, year_end, ["age", "year", "sex", "cat1", "cat2", "cat3", "cat4"]
+    ).melt(
+        id_vars=("age_start", "age_end", "year_start", "year_end", "sex"),
+        var_name="parameter",
+        value_name="value",
+    )
 
     affected_causes = ["test_cause_1", "test_cause_2"]
     rr_data = []
     paf_data = []
     for cause in affected_causes:
         rr_data.append(
             build_table(
-                [1.03, 1.02, 1.01, 1, cause], year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2', 'cat3', 'cat4', 'cause']
-            ).melt(id_vars=('age_group_start', 'age_group_end', 'year_start',
-                            'year_end', 'sex', 'cause'), var_name='parameter', value_name='value')
+                [1.03, 1.02, 1.01, 1, cause],
+                year_start,
+                year_end,
+                ["age", "year", "sex", "cat1", "cat2", "cat3", "cat4", "cause"],
+            ).melt(
+                id_vars=("age_start", "age_end", "year_start", "year_end", "sex", "cause"),
+                var_name="parameter",
+                value_name="value",
+            )
+        )
+        paf_data.append(
+            build_table(
+                [1, cause], year_start, year_end, ["age", "sex", "year", "value", "cause"]
+            )
         )
-        paf_data.append(build_table([1, cause], year_start, year_end, ['age', 'sex', 'year', 'value', 'cause']))
     rr_data = pd.concat(rr_data)
     paf_data = pd.concat(paf_data)
-    paf_data['affected_measure'] = 'incidence_rate'
-    rr_data['affected_measure'] = 'incidence_rate'
-    risk_data['exposure'] = exposure_data
-    risk_data['relative_risk'] = rr_data
-    risk_data['population_attributable_fraction'] = paf_data
-    risk_data['affected_causes'] = affected_causes
-    risk_data['affected_risk_factors'] = []
+    paf_data["affected_measure"] = "incidence_rate"
+    rr_data["affected_measure"] = "incidence_rate"
+    risk_data["exposure"] = exposure_data
+    risk_data["relative_risk"] = rr_data
+    risk_data["population_attributable_fraction"] = paf_data
+    risk_data["affected_causes"] = affected_causes
+    risk_data["affected_risk_factors"] = []
     incidence_rate = build_table(0.01, year_start, year_end)
-    risk_data['incidence_rate'] = incidence_rate
-    risk_data['distribution'] = 'polytomous'
-    return Risk(f'risk_factor.{risk}'), risk_data
+    risk_data["incidence_rate"] = incidence_rate
+    risk_data["distribution"] = "polytomous"
+    return Risk(f"risk_factor.{risk}"), risk_data
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def coverage_gap():
     year_start = 1990
     year_end = 2010
-    cg = 'test_coverage_gap'
+    cg = "test_coverage_gap"
     cg_data = dict()
     cg_exposed = 0.6
     cg_exposure_data = build_table(
-        [cg_exposed, 1 - cg_exposed], year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2']
-    ).melt(id_vars=('age_group_start', 'age_group_end', 'year_start',
-                    'year_end', 'sex',), var_name='parameter', value_name='value')
-
-
+        [cg_exposed, 1 - cg_exposed],
+        year_start,
+        year_end,
+        ["age", "year", "sex", "cat1", "cat2"],
+    ).melt(
+        id_vars=(
+            "age_start",
+            "age_end",
+            "year_start",
+            "year_end",
+            "sex",
+        ),
+        var_name="parameter",
+        value_name="value",
+    )
 
     rr = 2
     rr_data = build_table(
-        [rr, 1], year_start, year_end, ['age', 'year', 'sex', 'cat1', 'cat2']
-    ).melt(id_vars=('age_group_start', 'age_group_end',
-                    'year_start', 'year_end', 'sex'), var_name='parameter', value_name='value')
+        [rr, 1], year_start, year_end, ["age", "year", "sex", "cat1", "cat2"]
+    ).melt(
+        id_vars=("age_start", "age_end", "year_start", "year_end", "sex"),
+        var_name="parameter",
+        value_name="value",
+    )
 
     # paf is (sum(exposure(category)*rr(category) -1 )/ (sum(exposure(category)* rr(category)
     paf = (rr * cg_exposed + (1 - cg_exposed) - 1) / (rr * cg_exposed + (1 - cg_exposed))
 
     paf_data = build_table(
-        paf, year_start, year_end, ['age', 'year', 'sex', 'population_attributable_fraction']
-    ).melt(id_vars=('age_group_start', 'age_group_end', 'year_start',
-                    'year_end', 'sex'), var_name='population_attributable_fraction', value_name='value')
-
-    paf_data['risk_factor'] = 'test_risk'
-    paf_data['affected_measure'] = 'exposure_parameters'
-    rr_data['affected_measure'] = 'exposure_parameters'
-    cg_data['exposure'] = cg_exposure_data
-    rr_data['risk_factor'] = 'test_risk'
-    cg_data['relative_risk'] = rr_data
-    cg_data['population_attributable_fraction'] = paf_data
-    cg_data['affected_causes'] = []
-    cg_data['affected_risk_factors'] = ['test_risk']
-    cg_data['distribution'] = 'dichotomous'
-    return Risk(f'coverage_gap.{cg}') , cg_data
+        paf, year_start, year_end, ["age", "year", "sex", "population_attributable_fraction"]
+    ).melt(
+        id_vars=("age_start", "age_end", "year_start", "year_end", "sex"),
+        var_name="population_attributable_fraction",
+        value_name="value",
+    )
+
+    paf_data["risk_factor"] = "test_risk"
+    paf_data["affected_measure"] = "exposure_parameters"
+    rr_data["affected_measure"] = "exposure_parameters"
+    cg_data["exposure"] = cg_exposure_data
+    rr_data["risk_factor"] = "test_risk"
+    cg_data["relative_risk"] = rr_data
+    cg_data["population_attributable_fraction"] = paf_data
+    cg_data["affected_causes"] = []
+    cg_data["affected_risk_factors"] = ["test_risk"]
+    cg_data["distribution"] = "dichotomous"
+    return Risk(f"coverage_gap.{cg}"), cg_data
```

### Comparing `vivarium_public_health-0.9.9/tests/risks/test_effect.py` & `vivarium_public_health-1.0.0/tests/risks/test_effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 #
 #     effect.exposure_effect = test_function
 #
 #     # This one should be affected by our RiskEffect
 #     rates = simulation.values.register_rate_producer('test_cause.incidence_rate')
 #     rates.source = simulation.tables.build_table(build_table(0.01, year_start, year_end),
 #                                                  key_columns=('sex',),
-#                                                  parameter_columns=[('age', 'age_group_start', 'age_group_end'),
+#                                                  parameter_columns=[('age', 'age_start', 'age_end'),
 #                                                                     ('year', 'year_start', 'year_end')],
 #                                                  value_columns=None)
 #
 #     # This one should not
 #     other_rates = simulation.values.register_rate_producer('some_other_cause.incidence_rate')
 #     other_rates.source = simulation.tables.build_table(build_table(0.01, year_start, year_end),
 #                                                        key_columns=('sex',),
-#                                                        parameter_columns=[('age', 'age_group_start', 'age_group_end'),
+#                                                        parameter_columns=[('age', 'age_start', 'age_end'),
 #                                                                           ('year', 'year_start', 'year_end')],
 #                                                        value_columns=None)
 #
 #     assert np.allclose(rates(simulation.get_population().index), from_yearly(0.01, time_step))
 #     assert np.allclose(other_rates(simulation.get_population().index), from_yearly(0.01, time_step))
 #
 #     test_exposure[0] = 1
@@ -211,15 +211,15 @@
 #     for key, value in risk_data.items():
 #         simulation.data.write(f'risk_factor.test_risk.{key}', value)
 #
 #     simulation.setup()
 #
 #     incidence_rate = simulation.values.register_rate_producer(affected_causes[0]+'.incidence_rate')
 #     incidence_rate.source = simulation.tables.build_table(risk_data['incidence_rate'], key_columns=('sex',),
-#                                                           parameter_columns=[('age', 'age_group_start', 'age_group_end'),
+#                                                           parameter_columns=[('age', 'age_start', 'age_end'),
 #                                                                              ('year', 'year_start', 'year_end')],
 #                                                           value_columns=None)
 #
 #     categories = simulation.values.get_value('test_risk.exposure')(simulation.get_population().index)
 #     assert np.isclose(categories.value_counts()['cat1'] / len(simulation.get_population()), 0.5, rtol=0.01)
 #
 #     expected_exposed_value = 0.01 * 1.01
@@ -247,15 +247,15 @@
 #         simulation.data.write(f'risk_factor.test_risk.{key}', value)
 #
 #     simulation.setup()
 #
 #     incidence_rate = simulation.values.register_rate_producer(affected_causes[0]+'.incidence_rate')
 #     incidence_rate.source = simulation.tables.build_table(risk_data['incidence_rate'],
 #                                                           key_columns=('sex',),
-#                                                           parameter_columns=[('age', 'age_group_start', 'age_group_end'),
+#                                                           parameter_columns=[('age', 'age_start', 'age_end'),
 #                                                                              ('year', 'year_start', 'year_end')],
 #                                                           value_columns=None)
 #
 #     categories = simulation.values.get_value('test_risk.exposure')(simulation.get_population().index)
 #
 #     for category in ['cat1', 'cat2', 'cat3', 'cat4']:
 #         assert np.isclose(categories.value_counts()[category] / len(simulation.get_population()), 0.25, rtol=0.02)
@@ -380,21 +380,21 @@
 #
 #     assert np.allclose(rates(simulation.get_population().index), from_yearly(0.01, time_step)*50)
 #     assert np.allclose(other_rates(simulation.get_population().index), from_yearly(0.01, time_step))
 #
 #
 # def test_RiskEffect_excess_mortality(base_config, base_plugins):
 #     dummy_risk = Risk("risk_factor.test_risk")
-#     dummy_effect = RiskEffect("risk_factor.test_risk", "cause.test_cause.excess_mortality")
+#     dummy_effect = RiskEffect("risk_factor.test_risk", "cause.test_cause.excess_mortality_rate")
 #     time_step = pd.Timedelta(days=base_config.time.step_size)
 #
 #     base_config.update({'test_risk': {'exposure': 1}}, layer='override')
-#     base_config.update({'effect_of_test_risk_on_test_cause': {'excess_mortality': 50}})
+#     base_config.update({'effect_of_test_risk_on_test_cause': {'excess_mortality_rate': 50}})
 #
 #     simulation = initialize_simulation([TestPopulation(), dummy_risk, dummy_effect],
 #                                        input_config=base_config, plugin_config=base_plugins)
 #     simulation.setup()
 #
-#     em = simulation.values.register_rate_producer('test_cause.excess_mortality',
+#     em = simulation.values.register_rate_producer('test_cause.excess_mortality_rate',
 #                                                   source=lambda index: pd.Series(0.1, index=index))
 #
 #     assert np.allclose(from_yearly(0.1, time_step)*50, em(simulation.get_population().index))
```

### Comparing `vivarium_public_health-0.9.9/tests/disease/test_special_disease.py` & `vivarium_public_health-1.0.0/tests/disease/test_special_disease.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,108 +1,145 @@
+from operator import gt, lt
+
 import numpy as np
 import pandas as pd
-from operator import gt, lt
 import pytest
+
 from vivarium_public_health.disease import RiskAttributableDisease
+from vivarium_public_health.disease.transition import TransitionString
 
 
 @pytest.fixture
 def disease_mock(mocker):
     def disease_with_distribution(distribution):
-        test_disease = RiskAttributableDisease('cause.test_cause', 'risk_factor.test_risk')
+        test_disease = RiskAttributableDisease("cause.test_cause", "risk_factor.test_risk")
         test_disease.distribution = distribution
         test_disease.population_view = mocker.Mock()
-        test_disease._mortality = mocker.Mock()
+        test_disease.excess_mortality_rate = mocker.Mock()
         return test_disease
+
     return disease_with_distribution
 
 
-test_data = [('ordered_polytomous', ['cat1', 'cat2', 'cat3', 'cat4'], ['cat1']),
-             ('ordered_polytomous', ['cat1', 'cat2', 'cat3', 'cat4'], ['cat1', 'cat2']),
-             ('ordered_polytomous', ['cat1', 'cat2', 'cat3', 'cat4'], ['cat1', 'cat2', 'cat3']),
-             ('dichotomous', ['cat1', 'cat2'], ['cat1'])]
+test_data = [
+    ("ordered_polytomous", ["cat1", "cat2", "cat3", "cat4"], ["cat1"]),
+    ("ordered_polytomous", ["cat1", "cat2", "cat3", "cat4"], ["cat1", "cat2"]),
+    ("ordered_polytomous", ["cat1", "cat2", "cat3", "cat4"], ["cat1", "cat2", "cat3"]),
+    ("dichotomous", ["cat1", "cat2"], ["cat1"]),
+]
 
 
-@pytest.mark.parametrize('distribution, categories, threshold', test_data)
-def test_filter_by_exposure_categorical(disease_mock, mocker, distribution, categories, threshold):
+@pytest.mark.parametrize("distribution, categories, threshold", test_data)
+def test_filter_by_exposure_categorical(
+    disease_mock, mocker, distribution, categories, threshold
+):
     disease = disease_mock(distribution)
     test_index = range(500)
     per_cat = len(test_index) // len(categories)
     infected = threshold * per_cat
     susceptible = list(set(categories) - set(threshold)) * per_cat
     current_exposure = lambda index: pd.Series(infected + susceptible, index=index)
     filter_func = disease.get_exposure_filter(distribution, current_exposure, threshold)
     expected = lambda index: current_exposure(index).isin(infected)
 
     assert np.all(expected(test_index) == filter_func(test_index))
 
 
-test_data = [('ensemble', '>=7'), ('ensemble', '<=7.5'), ('lognormal', '=2.5'), ('normal', '4'), ('normal', '+4'),
-             ('lognormal', '>=')]
+test_data = [
+    ("ensemble", ">=7"),
+    ("ensemble", "<=7.5"),
+    ("lognormal", "=2.5"),
+    ("normal", "4"),
+    ("normal", "+4"),
+    ("lognormal", ">="),
+]
 
 
-@pytest.mark.parametrize('distribution, threshold', test_data)
-def test_filter_by_exposure_continuous_incorrect_operator(disease_mock, distribution, threshold):
+@pytest.mark.parametrize("distribution, threshold", test_data)
+def test_filter_by_exposure_continuous_incorrect_operator(
+    disease_mock, distribution, threshold
+):
     disease = disease_mock(distribution)
     disease.threshold = threshold
-    with pytest.raises(ValueError, match='incorrect threshold'):
+    with pytest.raises(ValueError, match="incorrect threshold"):
         disease.get_exposure_filter(distribution, lambda index: index, threshold)
 
 
-test_data = [('ensemble', '>7'), ('ensemble', '<5'), ('lognormal', '<3.5'), ('normal', '>5.5')]
+test_data = [
+    ("ensemble", ">7"),
+    ("ensemble", "<5"),
+    ("lognormal", "<3.5"),
+    ("normal", ">5.5"),
+]
 
 
-@pytest.mark.parametrize('distribution, threshold', test_data)
+@pytest.mark.parametrize("distribution, threshold", test_data)
 def test_filter_by_exposure_continuous(disease_mock, distribution, threshold):
     disease = disease_mock(distribution)
     disease.threshold = threshold
-    op = {'>', '<'}.intersection(list(threshold)).pop()
+    op = {">", "<"}.intersection(list(threshold)).pop()
     threshold_val = float(threshold.split(op)[-1])
     threshold_op = gt if op == ">" else lt
 
     test_index = range(500)
 
-    current_exposure = lambda index: pd.Series([threshold_val - 0.2, threshold_val - 0.1, threshold_val,
-                                                threshold_val + 0.1, threshold_val + 0.2] *100, index=test_index)
+    current_exposure = lambda index: pd.Series(
+        [
+            threshold_val - 0.2,
+            threshold_val - 0.1,
+            threshold_val,
+            threshold_val + 0.1,
+            threshold_val + 0.2,
+        ]
+        * 100,
+        index=test_index,
+    )
 
     filter_func = disease.get_exposure_filter(distribution, current_exposure, threshold)
     expected = lambda index: threshold_op(current_exposure(index), threshold_val)
 
     assert np.all(expected(test_index) == filter_func(test_index))
 
 
-def test_mortality_rate_pandas_series(disease_mock):
-    disease = disease_mock('enesmble')
-    num_sims = 500
-    test_index = range(num_sims)
-    current_disease_status = [disease.cause.name] * int(0.2 * num_sims) + \
-                             [f'susceptible_to_{disease.cause.name}'] * int(num_sims * 0.8)
-    disease.population_view.get.side_effect =lambda index: pd.DataFrame({disease.cause.name: current_disease_status,
-                                                                        'alive': 'alive'}, index=index)
-    expected_mortality_values = pd.Series(current_disease_status, name=disease.cause.name,
-                                          index=test_index).map({disease.cause.name: 0.05,
-                                                                 f'susceptible_to_{disease.cause.name}': 0})
-    disease._mortality.return_value = expected_mortality_values
-    rates_df = pd.Series(0, index=test_index, name='death_due_to_other_causes')
-    expected = pd.DataFrame({'death_due_to_other_causes': 0, disease.cause.name: expected_mortality_values},
-                            index=test_index)
-
-    assert np.all(expected == disease.mortality_rates(test_index, rates_df))
-
-
 def test_mortality_rate_pandas_dataframe(disease_mock):
-    disease = disease_mock('enesmble')
+    disease = disease_mock("enesmble")
     num_sims = 500
     test_index = range(num_sims)
-    current_disease_status = [disease.cause.name] * int(0.2 * num_sims) + \
-                             [f'susceptible_to_{disease.cause.name}'] * int(num_sims * 0.8)
-    disease.population_view.get.side_effect = lambda index: pd.DataFrame({disease.cause.name: current_disease_status,
-                                                                          'alive': 'alive'}, index=index)
-    expected_mortality_values = pd.Series(current_disease_status, name=disease.cause.name,
-                                          index=test_index).map({disease.cause.name: 0.05,
-                                                                 f'susceptible_to_{disease.cause.name}': 0})
-    disease._mortality.return_value = expected_mortality_values
-    rates_df = pd.DataFrame({'death_due_to_other_causes': 0, 'another_test_cause': 0.001}, index=test_index)
-    expected = pd.DataFrame({'death_due_to_other_causes': 0, 'another_test_cause': 0.001,
-                             disease.cause.name: expected_mortality_values}, index=test_index)
-
-    assert np.all(expected == disease.mortality_rates(test_index, rates_df))
+    current_disease_status = [disease.cause.name] * int(0.2 * num_sims) + [
+        f"susceptible_to_{disease.cause.name}"
+    ] * int(num_sims * 0.8)
+    disease.population_view.get.side_effect = lambda index: pd.DataFrame(
+        {disease.cause.name: current_disease_status, "alive": "alive"}, index=index
+    )
+    expected_mortality_values = pd.Series(
+        current_disease_status, name=disease.cause.name, index=test_index
+    ).map({disease.cause.name: 0.05, f"susceptible_to_{disease.cause.name}": 0})
+    disease.excess_mortality_rate.return_value = expected_mortality_values
+    rates_df = pd.DataFrame(
+        {"other_causes": 0, "another_test_cause": 0.001}, index=test_index
+    )
+    expected = pd.DataFrame(
+        {
+            "other_causes": 0,
+            "another_test_cause": 0.001,
+            disease.cause.name: expected_mortality_values,
+        },
+        index=test_index,
+    )
+
+    assert np.all(expected == disease.adjust_mortality_rate(test_index, rates_df))
+
+
+test_data = [("disease_no_recovery", False), ("disease_with_recovery", True)]
+
+
+@pytest.mark.parametrize("disease, recoverable", test_data)
+def test_state_transition_names(disease, recoverable):
+    model = RiskAttributableDisease(f"cause.{disease}", f"risk_factor.{disease}")
+    model.recoverable = recoverable
+    model.adjust_state_and_transitions()
+    states = [disease, f"susceptible_to_{disease}"]
+    transitions = [TransitionString(f"susceptible_to_{disease}_TO_{disease}")]
+    if recoverable:
+        transitions.append(TransitionString(f"{disease}_TO_susceptible_to_{disease}"))
+    assert set(model.state_names) == set(states)
+    assert set(model.transition_names) == set(transitions)
```

### Comparing `vivarium_public_health-0.9.9/tests/test_utilities.py` & `vivarium_public_health-1.0.0/tests/test_utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from hypothesis import given
 import hypothesis.strategies as st
 import pytest
+from hypothesis import given
 
 from vivarium_public_health.utilities import EntityString, TargetString
 
 
 @st.composite
 def component_string(draw, min_components=0, max_components=None):
-    alphabet = st.characters(blacklist_characters=['.'])
-    string_parts = draw(st.lists(st.text(alphabet=alphabet), min_size=min_components, max_size=max_components))
-    return '.'.join(string_parts)
+    alphabet = st.characters(blacklist_characters=["."])
+    string_parts = draw(
+        st.lists(st.text(alphabet=alphabet), min_size=min_components, max_size=max_components)
+    )
+    return ".".join(string_parts)
 
 
-@given(component_string().filter(lambda x: len(x.split('.')) != 2))
+@given(component_string().filter(lambda x: len(x.split(".")) != 2))
 def test_EntityString_fail(s):
     with pytest.raises(ValueError):
         EntityString(s)
 
 
 @given(component_string(2, 2))
 def test_EntityString_pass(s):
-    entity_type, entity_name = s.split('.')
+    entity_type, entity_name = s.split(".")
     r = EntityString(s)
     assert r.type == entity_type
     assert r.name == entity_name
 
 
-@given(component_string().filter(lambda x: len(x.split('.')) != 3))
+@given(component_string().filter(lambda x: len(x.split(".")) != 3))
 def test_TargetString_fail(s):
     with pytest.raises(ValueError):
         TargetString(s)
 
 
 @given(component_string(3, 3))
 def test_TargetString_pass(s):
-    target_type, target_name, target_measure = s.split('.')
+    target_type, target_name, target_measure = s.split(".")
     t = TargetString(s)
     assert t.type == target_type
     assert t.name == target_name
     assert t.measure == target_measure
-
-
```

### Comparing `vivarium_public_health-0.9.9/PKG-INFO` & `vivarium_public_health-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 Metadata-Version: 2.1
 Name: vivarium_public_health
-Version: 0.9.9
+Version: 1.0.0
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
-Author: The vivarium_public_health developers
+Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: GNU GPLv3
-Description: Vivarium Public Health
-        ======================
-        
-        .. image:: https://badge.fury.io/py/vivarium-public-health.svg
-            :target: https://badge.fury.io/py/vivarium-public-health
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=develop
-            :target: https://travis-ci.org/ihmeuw/vivarium_public_health
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium_public_health/badge/?version=latest
-            :target: https://vivarium_public_health.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        .. image:: https://zenodo.org/badge/141212278.svg
-           :target: https://zenodo.org/badge/latestdoi/141212278
-        
-        This library contains several components for for modelling diseases and their interventions.
-        
-        You can install ``vivarium_public_health`` from PyPI with pip:
-        
-          ``> pip install vivarium_public_health``
-        
-        or build it from source with
-        
-          ``> git clone https://github.com/ihmeuw/vivarium_public_health.git``
-        
-          ``> cd vivarium_public_health``
-        
-          ``> python setup.py install``
-        
-        Documentation
-        ======================
-        You can view documentation at https://vivarium_public_health.readthedocs.io/en/latest/
-        
-Platform: UNKNOWN
+License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: dev
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+Vivarium Public Health
+======================
+
+.. image:: https://badge.fury.io/py/vivarium-public-health.svg
+    :target: https://badge.fury.io/py/vivarium-public-health
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/vivarium_public_health
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium_public_health/badge/?version=latest
+    :target: https://vivarium_public_health.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+.. image:: https://zenodo.org/badge/141212278.svg
+   :target: https://zenodo.org/badge/latestdoi/141212278
+
+This library contains several components for for modelling diseases and their interventions.
+
+You can install ``vivarium_public_health`` from PyPI with pip:
+
+  ``> pip install vivarium_public_health``
+
+or build it from source with
+
+  ``> git clone https://github.com/ihmeuw/vivarium_public_health.git``
+
+  ``> cd vivarium_public_health``
+
+  ``> python setup.py install``
+
+Documentation
+======================
+You can view documentation at https://vivarium_public_health.readthedocs.io/en/latest/
```

### Comparing `vivarium_public_health-0.9.9/CODE_OF_CONDUCT.rst` & `vivarium_public_health-1.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/therapeutic_inertia.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/treatment/therapeutic_inertia.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,68 @@
+"""
+=========================
+Therapeutic Inertia Model
+=========================
+
+This module contains a model for therapeutic inertia which represents the
+variety of reasons why a treatment algorithm might deviate from guidelines.
+
+"""
 import pandas as pd
 import scipy.stats
 
 
 class TherapeuticInertia:
     """Expose a therapeutic inertia pipeline that defines
     a population-level therapeutic inertia.
     This is the probability of treatment during a healthcare visit."""
 
     configuration_defaults = {
-        'therapeutic_inertia': {
-            'triangle_min': 0.65,
-            'triangle_max': 0.9,
-            'triangle_mode': 0.875
+        "therapeutic_inertia": {
+            "triangle_min": 0.65,
+            "triangle_max": 0.9,
+            "triangle_mode": 0.875,
         }
     }
 
+    @property
+    def name(self):
+        return "therapeutic_inertia"
+
     def setup(self, builder):
-        self.name = 'therapeutic_inertia'
         self.therapeutic_inertia_parameters = builder.configuration.therapeutic_inertia
 
-        self.randomness = builder.randomness.get_stream(self.name)
-
-        self._therapeutic_inertia = self.initialize_therapeutic_inertia()
+        self._therapeutic_inertia = self.initialize_therapeutic_inertia(builder)
         ti_source = lambda index: pd.Series(self._therapeutic_inertia, index=index)
-        self.therapeutic_inertia = builder.value.register_value_producer('therapeutic_inertia', source=ti_source)
+        self.therapeutic_inertia = builder.value.register_value_producer(
+            "therapeutic_inertia", source=ti_source
+        )
 
-    def initialize_therapeutic_inertia(self):
+    def initialize_therapeutic_inertia(self, builder):
         triangle_min = self.therapeutic_inertia_parameters.triangle_min
         triangle_max = self.therapeutic_inertia_parameters.triangle_max
         triangle_mode = self.therapeutic_inertia_parameters.triangle_mode
 
         # convert to scipy params
         loc = triangle_min
         scale = triangle_max - triangle_min
         if scale == 0:
             c = 0
         else:
             c = (triangle_mode - loc) / scale
 
-        seed = self.randomness.get_seed()
-        therapeutic_inertia = scipy.stats.triang(c, loc=loc, scale=scale).rvs(random_state=seed)
+        seed = builder.randomness.get_seed(self.name)
+        therapeutic_inertia = scipy.stats.triang(c, loc=loc, scale=scale).rvs(
+            random_state=seed
+        )
 
         return therapeutic_inertia
+
+    def __str__(self):
+        return (
+            f"TherapeuticInertia(triangle_min={self.therapeutic_inertia_parameters.triangle_min}, "
+            f"triangle_max={self.therapeutic_inertia_parameters.triangle_max}, "
+            f"triangle_mode={self.therapeutic_inertia_parameters.triangle_mode})"
+        )
+
+    def __repr__(self):
+        return "TherapeuticInertia()"
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disability.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/metrics/disability.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,113 @@
-from collections import Counter
+"""
+===================
+Disability Observer
+===================
+
+This module contains tools for observing years lived with disability (YLDs)
+in the simulation.
+
+"""
+from typing import List
 
 import pandas as pd
-from vivarium.framework.values import list_combiner, joint_value_post_processor, rescale_post_processor
+from vivarium.framework.engine import Builder
+from vivarium.framework.values import (
+    NumberLike,
+    Pipeline,
+    list_combiner,
+    rescale_post_processor,
+    union_post_processor,
+)
 
-from vivarium_public_health.disease import DiseaseModel
-from .utilities import get_age_bins, get_years_lived_with_disability
+from vivarium_public_health.disease import DiseaseState, RiskAttributableDisease
+from vivarium_public_health.utilities import to_years
 
 
-class Disability:
+class DisabilityObserver:
     """Counts years lived with disability.
 
     By default, this counts both aggregate and cause-specific years lived
-    with disability over the full course of the simulation. It can be
-    configured to bin the cause-specific YLDs into age groups, sexes, and years
-    by setting the ``by_age``, ``by_sex``, and ``by_year`` flags, respectively.
+    with disability over the full course of the simulation.
 
     In the model specification, your configuration for this component should
     be specified as, e.g.:
 
-    configuration:
-        metrics:
-            disability:
-                by_age: True
-                by_year: False
-                by_sex: True
+    .. code-block:: yaml
 
+        configuration:
+            observers:
+                disability:
+                    exclude:
+                        - "sex"
+                    include:
+                        - "sample_stratification"
     """
+
     configuration_defaults = {
-        'metrics': {
-            'disability': {
-                'by_age': False,
-                'by_year': False,
-                'by_sex': False,
+        "stratification": {
+            "disability": {
+                "exclude": [],
+                "include": [],
             }
         }
     }
 
     def __init__(self):
-        self.name = 'disability_observer'
+        self.disability_weight_pipeline_name = "disability_weight"
 
-    def setup(self, builder):
-        self.config = builder.configuration.metrics.disability
-        self.age_bins = get_age_bins(builder)
-        self.clock = builder.time.clock()
-        self.step_size = builder.time.step_size()
-        self.causes = [c.state_column for c in builder.components.get_components(DiseaseModel)]
-        self.years_lived_with_disability = Counter()
-        self.disability_weight_pipelines = {cause: builder.value.get_value(f'{cause}.disability_weight')
-                                            for cause in self.causes}
+    def __repr__(self):
+        return "DisabilityObserver()"
 
-        self.disability_weight = builder.value.register_value_producer(
-            'disability_weight',
+    @property
+    def name(self):
+        return "disability_observer"
+
+    @property
+    def disease_classes(self) -> List:
+        return [DiseaseState, RiskAttributableDisease]
+
+    # noinspection PyAttributeOutsideInit
+    def setup(self, builder: Builder):
+        self.config = builder.configuration.stratification.disability
+        self.step_size = pd.Timedelta(days=builder.configuration.time.step_size)
+        self.disability_weight = self.get_disability_weight_pipeline(builder)
+        cause_states = builder.components.get_components_by_type(tuple(self.disease_classes))
+
+        builder.results.register_observation(
+            name="ylds_due_to_all_causes",
+            pop_filter='tracked == True and alive == "alive"',
+            aggregator_sources=[self.disability_weight_pipeline_name],
+            aggregator=self._disability_weight_aggregator,
+            requires_columns=["alive"],
+            requires_values=["disability_weight"],
+            additional_stratifications=self.config.include,
+            excluded_stratifications=self.config.exclude,
+            when="time_step__prepare",
+        )
+
+        for cause_state in cause_states:
+            cause_disability_weight_pipeline_name = (
+                f"{cause_state.state_id}.disability_weight"
+            )
+            builder.results.register_observation(
+                name=f"ylds_due_to_{cause_state.state_id}",
+                pop_filter='tracked == True and alive == "alive"',
+                aggregator_sources=[cause_disability_weight_pipeline_name],
+                aggregator=self._disability_weight_aggregator,
+                requires_columns=["alive"],
+                requires_values=[cause_disability_weight_pipeline_name],
+                additional_stratifications=self.config.include,
+                excluded_stratifications=self.config.exclude,
+                when="time_step__prepare",
+            )
+
+    def get_disability_weight_pipeline(self, builder: Builder) -> Pipeline:
+        return builder.value.register_value_producer(
+            self.disability_weight_pipeline_name,
             source=lambda index: [pd.Series(0.0, index=index)],
             preferred_combiner=list_combiner,
-            preferred_post_processor=_disability_post_processor)
-
-        columns_required = ['tracked', 'alive', 'years_lived_with_disability']
-        if self.config.by_age:
-            columns_required += ['age']
-        if self.config.by_sex:
-            columns_required += ['sex']
-        self.population_view = builder.population.get_view(columns_required)
-        builder.population.initializes_simulants(self.initialize_disability,
-                                                 creates_columns=['years_lived_with_disability'])
-        # FIXME: The state table is modified before the clock advances.
-        # In order to get an accurate representation of person time we need to look at
-        # the state table before anything happens.
-        builder.event.register_listener('time_step__prepare', self.on_time_step_prepare)
-        builder.value.register_value_modifier('metrics', modifier=self.metrics)
-
-    def initialize_disability(self, pop_data):
-        self.population_view.update(pd.Series(0., index=pop_data.index, name='years_lived_with_disability'))
-
-    def on_time_step_prepare(self, event):
-        pop = self.population_view.get(event.index, query='tracked == True and alive == "alive"')
-        ylds_this_step = get_years_lived_with_disability(pop, self.config.to_dict(),
-                                                         self.clock().year, self.step_size(),
-                                                         self.age_bins, self.disability_weight_pipelines, self.causes)
-        self.years_lived_with_disability.update(ylds_this_step)
-
-        pop.loc[:, 'years_lived_with_disability'] += self.disability_weight(pop.index)
-        self.population_view.update(pop)
-
-    def metrics(self, index, metrics):
-        total_ylds = self.population_view.get(index)['years_lived_with_disability'].sum()
-        metrics['years_lived_with_disability'] = total_ylds
-        metrics.update(self.years_lived_with_disability)
-        return metrics
-
+            preferred_post_processor=union_post_processor,
+        )
 
-def _disability_post_processor(value, step_size):
-    return rescale_post_processor(joint_value_post_processor(value, step_size), step_size)
+    def _disability_weight_aggregator(self, dw: pd.DataFrame) -> float:
+        return (dw * to_years(self.step_size)).sum().squeeze()
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/population/base_population.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/population/base_population.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,284 +1,416 @@
-import pandas as pd
-import numpy as np
+"""
+=========================
+The Core Population Model
+=========================
+
+This module contains tools for sampling and assigning core demographic
+characteristics to simulants.
 
-from .data_transformations import (assign_demographic_proportions, rescale_binned_proportions,
-                                   smooth_ages, load_population_structure)
+"""
+from typing import Callable, Dict, Iterable, List
 
-SECONDS_PER_YEAR = 365.25*24*60*60
+import numpy as np
+import pandas as pd
+from vivarium.framework.engine import Builder
+from vivarium.framework.event import Event
+from vivarium.framework.population import PopulationView, SimulantData
+from vivarium.framework.randomness import RandomnessStream
+
+from vivarium_public_health import utilities
+from vivarium_public_health.population.data_transformations import (
+    assign_demographic_proportions,
+    load_population_structure,
+    rescale_binned_proportions,
+    smooth_ages,
+)
 
 
 class BasePopulation:
     """Component for producing and aging simulants based on demographic data."""
 
     configuration_defaults = {
-        'population': {
-            'age_start': 0,
-            'age_end': 125,
-            'exit_age': None,
+        "population": {
+            "age_start": 0,
+            "age_end": 125,
+            "exit_age": None,
+            "include_sex": "Both",  # Either Female, Male, or Both
         }
     }
 
-    def setup(self, builder):
-        self.config = builder.configuration.population
-        input_config = builder.configuration.input_data
+    def __init__(self):
+        self._sub_components = [AgeOutSimulants()]
 
-        self.randomness = {'general_purpose': builder.randomness.get_stream('population_generation'),
-                           'bin_selection': builder.randomness.get_stream('bin_selection', for_initialization=True),
-                           'age_smoothing': builder.randomness.get_stream('age_smoothing', for_initialization=True),
-                           'age_smoothing_age_bounds': builder.randomness.get_stream('age_smoothing_age_bounds',
-                                                                                     for_initialization=True)}
-        self.register_simulants = builder.randomness.register_simulants
+    def __repr__(self) -> str:
+        return "BasePopulation()"
 
-        columns = ['age', 'sex', 'alive', 'location', 'entrance_time', 'exit_time']
+    ##############
+    # Properties #
+    ##############
+
+    @property
+    def name(self) -> str:
+        return "base_population"
+
+    @property
+    def sub_components(self) -> List:
+        return self._sub_components
+
+    @property
+    def columns_created(self) -> List[str]:
+        return ["age", "sex", "alive", "location", "entrance_time", "exit_time"]
+
+    #################
+    # Setup methods #
+    #################
 
-        self.population_view = builder.population.get_view(columns)
-        builder.population.initializes_simulants(self.generate_base_population, creates_columns=columns)
+    # noinspection PyAttributeOutsideInit
+    def setup(self, builder: Builder) -> None:
+        self.config = builder.configuration.population
+        self.key_columns = builder.configuration.randomness.key_columns
+        if self.config.include_sex not in ["Male", "Female", "Both"]:
+            raise ValueError(
+                "Configuration key 'population.include_sex' must be one "
+                "of ['Male', 'Female', 'Both']. "
+                f"Provided value: {self.config.include_sex}."
+            )
 
         source_population_structure = load_population_structure(builder)
-        source_population_structure['location'] = input_config.location
+        self.demographic_proportions = assign_demographic_proportions(
+            source_population_structure,
+            include_sex=self.config.include_sex,
+        )
 
-        self.population_data = _build_population_data_table(source_population_structure)
+        self.randomness = self.get_randomness_streams(builder)
+        self.register_simulants = builder.randomness.register_simulants
+        self.population_view = self.get_population_view(builder)
+        builder.population.initializes_simulants(
+            self.on_initialize_simulants, creates_columns=self.columns_created
+        )
 
-        builder.event.register_listener('time_step', self.on_time_step, priority=8)
-        if self.config.exit_age is not None:
-            builder.components.add_components([AgeOutSimulants()])
+        builder.event.register_listener("time_step", self.on_time_step, priority=8)
 
     @staticmethod
-    def select_sub_population_data(reference_population_data, year):
-        reference_years = sorted(set(reference_population_data.year_start))
-        ref_year_index = np.digitize(year, reference_years).item()-1
-        return reference_population_data[reference_population_data.year_start == reference_years[ref_year_index]]
+    def get_randomness_streams(builder: Builder) -> Dict[str, RandomnessStream]:
+        return {
+            "general_purpose": builder.randomness.get_stream("population_generation"),
+            "bin_selection": builder.randomness.get_stream(
+                "bin_selection", initializes_crn_attributes=True
+            ),
+            "age_smoothing": builder.randomness.get_stream(
+                "age_smoothing", initializes_crn_attributes=True
+            ),
+            "age_smoothing_age_bounds": builder.randomness.get_stream(
+                "age_smoothing_age_bounds", initializes_crn_attributes=True
+            ),
+        }
+
+    def get_population_view(self, builder: Builder) -> PopulationView:
+        return builder.population.get_view(self.columns_created)
+
+    ########################
+    # Event-driven methods #
+    ########################
 
     # TODO: Move most of this docstring to an rst file.
-    def generate_base_population(self, pop_data):
+    def on_initialize_simulants(self, pop_data: SimulantData) -> None:
         """Creates a population with fundamental demographic and simulation properties.
 
         When the simulation framework creates new simulants (essentially producing a new
         set of simulant ids) and this component is being used, the newly created simulants
-        arrive here first and are assigned the demographic qualities 'age', 'sex', and 'location'
-        in a way that is consistent with the demographic distributions represented by the
-        population-level data.  Additionally, the simulants are assigned the simulation properties
-        'alive', 'entrance_time', and 'exit_time'.
+        arrive here first and are assigned the demographic qualities 'age', 'sex',
+        and 'location' in a way that is consistent with the demographic distributions
+        represented by the population-level data.  Additionally, the simulants are assigned
+        the simulation properties 'alive', 'entrance_time', and 'exit_time'.
 
         The 'alive' parameter is alive or dead.
         In general, most simulation components (except for those computing summary statistics)
         ignore simulants if they are not in the 'alive' category. The 'entrance_time' and
         'exit_time' categories simply mark when the simulant enters or leaves the simulation,
-        respectively.  Here we are agnostic to the methods of entrance and exit (e.g birth,
+        respectively.  Here we are agnostic to the methods of entrance and exit (e.g., birth,
         migration, death, etc.) as these characteristics can be inferred from this column and
         other information about the simulant and the simulation parameters.
 
-        Parameters
-        ----------
-        pop_data
         """
 
-        age_params = {'age_start': pop_data.user_data.get('age_start', self.config.age_start),
-                      'age_end': pop_data.user_data.get('age_end', self.config.age_end)}
+        age_params = {
+            "age_start": pop_data.user_data.get("age_start", self.config.age_start),
+            "age_end": pop_data.user_data.get("age_end", self.config.age_end),
+        }
 
-        sub_pop_data = self.select_sub_population_data(self.population_data, pop_data.creation_time.year)
+        demographic_proportions = self.get_demographic_proportions_for_creation_time(
+            self.demographic_proportions, pop_data.creation_time.year
+        )
+
+        self.population_view.update(
+            generate_population(
+                simulant_ids=pop_data.index,
+                creation_time=pop_data.creation_time,
+                step_size=pop_data.creation_window,
+                age_params=age_params,
+                demographic_proportions=demographic_proportions,
+                randomness_streams=self.randomness,
+                register_simulants=self.register_simulants,
+                key_columns=self.key_columns,
+            )
+        )
 
-        self.population_view.update(generate_population(simulant_ids=pop_data.index,
-                                                        creation_time=pop_data.creation_time,
-                                                        step_size=pop_data.creation_window,
-                                                        age_params=age_params,
-                                                        population_data=sub_pop_data,
-                                                        randomness_streams=self.randomness,
-                                                        register_simulants=self.register_simulants))
-
-    def on_time_step(self, event):
-        """Ages simulants each time step.
-
-        Parameters
-        ----------
-        event : vivarium.framework.population.PopulationEvent
-        """
-        step_size = event.step_size/pd.Timedelta(seconds=1)
+    def on_time_step(self, event: Event) -> None:
+        """Ages simulants each time step."""
         population = self.population_view.get(event.index, query="alive == 'alive'")
-        population['age'] += step_size / SECONDS_PER_YEAR
+        population["age"] += utilities.to_years(event.step_size)
         self.population_view.update(population)
 
+    ##################
+    # Helper methods #
+    ##################
+
+    @staticmethod
+    def get_demographic_proportions_for_creation_time(
+        demographic_proportions, year: int
+    ) -> pd.DataFrame:
+        reference_years = sorted(set(demographic_proportions.year_start))
+        ref_year_index = np.digitize(year, reference_years).item() - 1
+        return demographic_proportions[
+            demographic_proportions.year_start == reference_years[ref_year_index]
+        ]
+
 
 class AgeOutSimulants:
     """Component for handling aged-out simulants"""
 
-    def setup(self, builder):
+    @property
+    def name(self) -> str:
+        return "age_out_simulants"
+
+    # noinspection PyAttributeOutsideInit
+    def setup(self, builder: Builder) -> None:
+        if builder.configuration.population.exit_age is None:
+            return
         self.config = builder.configuration.population
-        self.population_view = builder.population.get_view(['age', 'exit_time', 'tracked'])
-        builder.event.register_listener('time_step__cleanup', self.on_time_step_cleanup)
+        self.population_view = builder.population.get_view(["age", "exit_time", "tracked"])
+        builder.event.register_listener("time_step__cleanup", self.on_time_step_cleanup)
 
-    def on_time_step_cleanup(self, event):
+    def on_time_step_cleanup(self, event: Event) -> None:
         population = self.population_view.get(event.index)
         max_age = float(self.config.exit_age)
-        pop = population[(population['age'] >= max_age) & population['tracked']].copy()
+        pop = population[(population["age"] >= max_age) & population["tracked"]].copy()
         if len(pop) > 0:
-            pop['tracked'] = pd.Series(False, index=pop.index)
-            pop['exit_time'] = event.time
+            pop["tracked"] = pd.Series(False, index=pop.index)
+            pop["exit_time"] = event.time
             self.population_view.update(pop)
 
+    def __repr__(self) -> str:
+        return "AgeOutSimulants()"
 
-def generate_population(simulant_ids, creation_time, step_size, age_params,
-                        population_data, randomness_streams, register_simulants):
-    """Produces a randomly generated set of simulants sampled from the provided `population_data`.
+
+def generate_population(
+    simulant_ids: pd.Index,
+    creation_time: pd.Timestamp,
+    step_size: pd.Timedelta,
+    age_params: Dict[str, float],
+    demographic_proportions: pd.DataFrame,
+    randomness_streams: Dict[str, RandomnessStream],
+    register_simulants: Callable[[pd.DataFrame], None],
+    key_columns: Iterable[str] = ("entrance_time", "age"),
+) -> pd.DataFrame:
+    """Produces a random set of simulants sampled from the provided `population_data`.
 
     Parameters
     ----------
-    simulant_ids : iterable of ints
+    simulant_ids
         Values to serve as the index in the newly generated simulant DataFrame.
-    creation_time : pandas.Timestamp
+    creation_time
         The simulation time when the simulants are created.
-    age_params : dict
+    age_params
         Dictionary with keys
             age_start : Start of an age range
             age_end : End of an age range
+
         The latter two keys can have values specified to generate simulants over an age range.
-    population_data : pandas.DataFrame
-        Table with columns 'age', 'age_group_start', 'age_group_end', 'sex', 'year',
-        'location', 'population', 'P(sex, location, age| year)', 'P(sex, location | age, year)'
-    randomness_streams : Dict[str, vivarium.framework.randomness.RandomnessStream]
+    demographic_proportions
+        Table with columns 'age', 'age_start', 'age_end', 'sex', 'year',
+        'location', 'population', 'P(sex, location, age| year)',
+        'P(sex, location | age, year)'.
+    randomness_streams
         Source of random number generation within the vivarium common random number framework.
-    step_size : float
+    step_size
         The size of the initial time step.
-    register_simulants : Callable
+    register_simulants
         A function to register the new simulants with the CRN framework.
+    key_columns
+        A list of key columns for random number generation.
 
     Returns
     -------
-    simulants : pandas.DataFrame
+    pandas.DataFrame
         Table with columns
-            'entrance_time' : The `pandas.Timestamp` describing when the simulant entered
+            'entrance_time'
+                The `pandas.Timestamp` describing when the simulant entered
                 the simulation. Set to `creation_time` for all simulants.
-            'exit_time' : The `pandas.Timestamp` describing when the simulant exited
+            'exit_time'
+                The `pandas.Timestamp` describing when the simulant exited
                 the simulation. Set initially to `pandas.NaT`.
-            'alive' : One of 'alive' or 'dead' indicating how the simulation
+            'alive'
+                One of 'alive' or 'dead' indicating how the simulation
                 interacts with the simulant.
-            'age' : The age of the simulant at the current time step.
-            'location' : The location indicating where the simulant resides.
-            'sex' : Either 'Male' or 'Female'.  The sex of the simulant.
+            'age'
+                The age of the simulant at the current time step.
+            'location'
+                The location indicating where the simulant resides.
+            'sex'
+                Either 'Male' or 'Female'.  The sex of the simulant.
+
     """
-    simulants = pd.DataFrame({'entrance_time': pd.Series(creation_time, index=simulant_ids),
-                              'exit_time': pd.Series(pd.NaT, index=simulant_ids),
-                              'alive': pd.Series('alive', index=simulant_ids)},
-                             index=simulant_ids)
-    age_start = float(age_params['age_start'])
-    age_end = float(age_params['age_end'])
+    simulants = pd.DataFrame(
+        {
+            "entrance_time": pd.Series(creation_time, index=simulant_ids),
+            "exit_time": pd.Series(pd.NaT, index=simulant_ids),
+            "alive": pd.Series("alive", index=simulant_ids),
+        },
+        index=simulant_ids,
+    )
+    age_start = float(age_params["age_start"])
+    age_end = float(age_params["age_end"])
     if age_start == age_end:
-        return _assign_demography_with_initial_age(simulants, population_data, age_start,
-                                                   step_size, randomness_streams, register_simulants)
+        return _assign_demography_with_initial_age(
+            simulants,
+            demographic_proportions,
+            age_start,
+            step_size,
+            randomness_streams,
+            register_simulants,
+        )
     else:  # age_params['age_start'] is not None and age_params['age_end'] is not None
-        return _assign_demography_with_age_bounds(simulants, population_data, age_start,
-                                                  age_end, randomness_streams, register_simulants)
-
-
-def _assign_demography_with_initial_age(simulants, pop_data, initial_age,
-                                        step_size, randomness_streams, register_simulants):
+        return _assign_demography_with_age_bounds(
+            simulants,
+            demographic_proportions,
+            age_start,
+            age_end,
+            randomness_streams,
+            register_simulants,
+            key_columns,
+        )
+
+
+def _assign_demography_with_initial_age(
+    simulants: pd.DataFrame,
+    pop_data: pd.DataFrame,
+    initial_age: float,
+    step_size: pd.Timedelta,
+    randomness_streams: Dict[str, RandomnessStream],
+    register_simulants: Callable[[pd.DataFrame], None],
+) -> pd.DataFrame:
     """Assigns age, sex, and location information to the provided simulants given a fixed age.
 
     Parameters
     ----------
-    simulants : pandas.DataFrame
+    simulants
         Table that represents the new cohort of agents being added to the simulation.
-    pop_data : pandas.DataFrame
-        Table with columns 'age', 'age_group_start', 'age_group_end', 'sex', 'year',
-        'location', 'population', 'P(sex, location, age| year)', 'P(sex, location | age, year)'
-    initial_age : float
+    pop_data
+        Table with columns 'age', 'age_start', 'age_end', 'sex', 'year',
+        'location', 'population', 'P(sex, location, age| year)',
+        'P(sex, location | age, year)'
+    initial_age
         The age to assign the new simulants.
-    randomness_streams : Dict[str, vivarium.framework.randomness.RandomnessStream]
+    randomness_streams
         Source of random number generation within the vivarium common random number framework.
-    step_size : float
+    step_size
         The size of the initial time step.
-    register_simulants : Callable
+    register_simulants
         A function to register the new simulants with the CRN framework.
 
     Returns
     -------
     pandas.DataFrame
-        Table with same columns as `simulants` and with the additional columns 'age', 'sex',  and 'location'.
+        Table with same columns as `simulants` and with the additional
+        columns 'age', 'sex',  and 'location'.
     """
-    pop_data = pop_data[(pop_data.age_group_start <= initial_age) & (pop_data.age_group_end >= initial_age)]
+    pop_data = pop_data[
+        (pop_data.age_start <= initial_age) & (pop_data.age_end >= initial_age)
+    ]
 
     if pop_data.empty:
-        raise ValueError('The age {} is not represented by the population data structure'.format(initial_age))
-
-    age_fuzz = randomness_streams['age_smoothing'].get_draw(simulants.index) * step_size / pd.Timedelta(days=365)
-    simulants['age'] = initial_age + age_fuzz
-    register_simulants(simulants[['entrance_time', 'age']])
+        raise ValueError(
+            "The age {} is not represented by the population data structure".format(
+                initial_age
+            )
+        )
+
+    age_fuzz = randomness_streams["age_smoothing"].get_draw(
+        simulants.index
+    ) * utilities.to_years(step_size)
+    simulants["age"] = initial_age + age_fuzz
+    register_simulants(simulants[["entrance_time", "age"]])
 
     # Assign a demographically accurate location and sex distribution.
-    choices = pop_data.set_index(['sex', 'location'])['P(sex, location | age, year)'].reset_index()
-    decisions = randomness_streams['general_purpose'].choice(simulants.index,
-                                                             choices=choices.index,
-                                                             p=choices['P(sex, location | age, year)'])
+    choices = pop_data.set_index(["sex", "location"])[
+        "P(sex, location | age, year)"
+    ].reset_index()
+    decisions = randomness_streams["general_purpose"].choice(
+        simulants.index, choices=choices.index, p=choices["P(sex, location | age, year)"]
+    )
 
-    simulants['sex'] = choices.loc[decisions, 'sex'].values
-    simulants['location'] = choices.loc[decisions, 'location'].values
+    simulants["sex"] = choices.loc[decisions, "sex"].values
+    simulants["location"] = choices.loc[decisions, "location"].values
 
     return simulants
 
 
-def _assign_demography_with_age_bounds(simulants, pop_data, age_start, age_end, randomness_streams, register_simulants):
-    """Assigns age, sex, and location information to the provided simulants given a range of ages.
+def _assign_demography_with_age_bounds(
+    simulants: pd.DataFrame,
+    pop_data: pd.DataFrame,
+    age_start: float,
+    age_end: float,
+    randomness_streams: Dict[str, RandomnessStream],
+    register_simulants: Callable[[pd.DataFrame], None],
+    key_columns: Iterable[str] = ("entrance_time", "age"),
+) -> pd.DataFrame:
+    """Assigns an age, sex, and location to the provided simulants given a range of ages.
 
     Parameters
     ----------
-    simulants : pandas.DataFrame
+    simulants
         Table that represents the new cohort of agents being added to the simulation.
-    pop_data : pandas.DataFrame
-        Table with columns 'age', 'age_group_start', 'age_group_end', 'sex', 'year',
-        'location', 'population', 'P(sex, location, age| year)', 'P(sex, location | age, year)'
-    age_start, age_end : float
+    pop_data
+        Table with columns 'age', 'age_start', 'age_end', 'sex', 'year',
+        'location', 'population', 'P(sex, location, age| year)',
+        'P(sex, location | age, year)'
+    age_start, age_end
         The start and end of the age range of interest, respectively.
-    randomness_streams : Dict[str, vivarium.framework.randomness.RandomnessStream]
+    randomness_streams
         Source of random number generation within the vivarium common random number framework.
-    register_simulants : Callable
+    register_simulants
         A function to register the new simulants with the CRN framework.
+    key_columns
+        A list of key columns for random number generation.
 
     Returns
     -------
     pandas.DataFrame
-        Table with same columns as `simulants` and with the additional columns 'age', 'sex',  and 'location'.
+        Table with same columns as `simulants` and with the additional columns
+        'age', 'sex',  and 'location'.
+
     """
     pop_data = rescale_binned_proportions(pop_data, age_start, age_end)
     if pop_data.empty:
         raise ValueError(
-            'The age range ({}, {}) is not represented by the population data structure'.format(age_start, age_end))
+            f"The age range ({age_start}, {age_end}) is not represented by the "
+            f"population data structure."
+        )
 
     # Assign a demographically accurate age, location, and sex distribution.
-    sub_pop_data = pop_data[(pop_data.age_group_start >= age_start) & (pop_data.age_group_end <= age_end)]
-    choices = sub_pop_data.set_index(['age', 'sex', 'location'])['P(sex, location, age| year)'].reset_index()
-    decisions = randomness_streams['bin_selection'].choice(simulants.index,
-                                                           choices=choices.index,
-                                                           p=choices['P(sex, location, age| year)'])
-    simulants['age'] = choices.loc[decisions, 'age'].values
-    simulants['sex'] = choices.loc[decisions, 'sex'].values
-    simulants['location'] = choices.loc[decisions, 'location'].values
-    simulants = smooth_ages(simulants, pop_data, randomness_streams['age_smoothing_age_bounds'])
-    register_simulants(simulants[['entrance_time', 'age']])
+    sub_pop_data = pop_data[(pop_data.age_start >= age_start) & (pop_data.age_end <= age_end)]
+    choices = sub_pop_data.set_index(["age", "sex", "location"])[
+        "P(sex, location, age| year)"
+    ].reset_index()
+    decisions = randomness_streams["bin_selection"].choice(
+        simulants.index, choices=choices.index, p=choices["P(sex, location, age| year)"]
+    )
+    simulants["age"] = choices.loc[decisions, "age"].values
+    simulants["sex"] = choices.loc[decisions, "sex"].values
+    simulants["location"] = choices.loc[decisions, "location"].values
+    simulants = smooth_ages(
+        simulants, pop_data, randomness_streams["age_smoothing_age_bounds"]
+    )
+    register_simulants(simulants[list(key_columns)])
     return simulants
-
-
-def _build_population_data_table(data):
-    """Constructs a population data table for use as a population distribution over demographic characteristics.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        Population structure data
-
-    Returns
-    -------
-    pandas.DataFrame
-        Table with columns
-            'age' : Midpoint of the age group,
-            'age_group_start' : Lower bound of the age group,
-            'age_group_end' : Upper bound of the age group,
-            'sex' : 'Male' or 'Female',
-            'location' : location,
-            'year' : Year,
-            'population' : Total population estimate,
-            'P(sex, location | age, year)' : Conditional probability of sex and location given age and year,
-            'P(sex, location, age | year)' : Conditional probability of sex, location, and age given year,
-            'P(age | year, sex, location)' : Conditional probability of age given year, sex, and location.
-    """
-    return assign_demographic_proportions(data)
-
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/population/data_transformations.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/population/data_transformations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,428 +1,578 @@
+"""
+===============================
+Population Data Transformations
+===============================
+
+This module contains tools for handling raw demographic data and transforming
+it into different distributions for sampling.
+
+"""
 from collections import namedtuple
+from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
+from vivarium.framework.randomness import RandomnessStream
 
+_SORT_ORDER = ["location", "year_start", "sex", "age_start"]
 
-def assign_demographic_proportions(population_data):
-    """Calculates conditional probabilities on the provided population data for use in sampling.
+
+def assign_demographic_proportions(
+    population_data: pd.DataFrame,
+    include_sex: str,
+) -> pd.DataFrame:
+    """Calculates conditional probabilities on the provided population data for sampling.
 
     Parameters
     ----------
-    population_data : pandas.DataFrame
-        Table with columns 'age', 'sex', 'year', 'location', and 'population'
+    population_data
+        Table with columns 'age', 'sex', 'year', 'location', and 'value'
+    include_sex
+        'Female', 'Male', or 'Both'.  Sexes to include in the distribution.
 
     Returns
     -------
     pandas.DataFrame
-        Table with the same columns as `population_data` and additionally with columns
-        'P(sex, location, age| year)', 'P(sex, location | age, year)', and
-        'P(age | year, sex, location)' with values calculated from the
-        various population levels.
+        Table with columns
+            'age' : Midpoint of the age group,
+            'age_start' : Lower bound of the age group,
+            'age_end' : Upper bound of the age group,
+            'sex' : 'Male' or 'Female',
+            'location' : location,
+            'year' : Year,
+            'population' : Total population estimate,
+            'P(sex, location | age, year)' : Conditional probability of sex and
+            location given age and year,
+            'P(sex, location, age | year)' : Conditional probability of sex, location,
+            and age given year,
+            'P(age | year, sex, location)' : Conditional probability of age given
+            year, sex, and location.
     """
+    population_data = population_data.copy()
+    if include_sex != "Both":
+        population_data.loc[population_data.sex != include_sex, "value"] = 0.0
+
+    population_data["P(sex, location, age| year)"] = (
+        population_data.groupby("year_start", as_index=False)
+        .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
+        .reset_index(level=0)
+        .value.fillna(0.0)
+    )
 
-    population_data['P(sex, location, age| year)'] = (
-        population_data
-            .groupby('year_start', as_index=False)
-            .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
-            .reset_index(level=0).value
-    )
-
-    population_data['P(sex, location | age, year)'] = (
-        population_data
-            .groupby(['age', 'year_start'], as_index=False)
-            .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
-            .reset_index(level=0).value
-    )
-
-    population_data['P(age | year, sex, location)'] = (
-        population_data
-            .groupby(['year_start', 'sex', 'location'], as_index=False)
-            .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
-            .reset_index(level=0).value
+    population_data["P(sex, location | age, year)"] = (
+        population_data.groupby(["age", "year_start"], as_index=False)
+        .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
+        .reset_index(level=0)
+        .value.fillna(0.0)
     )
 
-    return population_data
+    population_data["P(age | year, sex, location)"] = (
+        population_data.groupby(["year_start", "sex", "location"], as_index=False)
+        .apply(lambda sub_pop: sub_pop.value / sub_pop.value.sum())
+        .reset_index(level=0)
+        .value.fillna(0.0)
+    )
 
+    return population_data.sort_values(_SORT_ORDER).reset_index(drop=True)
 
-#  FIXME: This step should definitely be happening after we get some approximation of the underlying
-# distribution.  It makes an assumption of uniformity in the age bin.  This only happens at the edges,
-# and is unlikely to be used to clip a neonatal age bin where the impact would be significant.
-def rescale_binned_proportions(pop_data, age_start, age_end):
-    """Reshapes the distribution so that bin edges fall cleanly on the specified age_start and age_end.
+
+#  FIXME: This step should definitely be happening after we get some approximation of the
+#   underlying distribution.  It makes an assumption of uniformity in the age bin.
+#   This only happens at the edges, and is unlikely to be used to clip a neonatal age bin
+#   where the impact would be significant.
+def rescale_binned_proportions(
+    pop_data: pd.DataFrame,
+    age_start: float,
+    age_end: float,
+) -> pd.DataFrame:
+    """Reshapes the distribution so that bin edges fall on the age_start and age_end.
 
     Parameters
     ----------
-    pop_data : pandas.DataFrame
-        Table with columns 'age', 'age_group_start', 'age_group_end', 'sex', 'year',
-        'location', 'population', 'P(sex, location, age| year)', 'P(sex, location | age, year)',
-        'P(age | year, sex, location)'
-    age_start : float
+    pop_data
+        Table with columns 'age', 'age_start', 'age_end', 'sex', 'year',
+        'location', 'population', 'P(sex, location, age| year)',
+        'P(sex, location | age, year)', 'P(age | year, sex, location)'
+    age_start
         The starting age for the rescaled bins.
-    age_end : float
+    age_end
         The terminal age for the rescaled bins.
 
     Returns
     -------
     pandas.DataFrame
         Table with the same columns as `pop_data` where all bins outside the range
         (age_start, age_end) have been discarded.  If age_start and age_end
         don't fall cleanly on age boundaries, the bins in which they lie are clipped and
         the 'population', 'P(sex, location, age| year)', and 'P(age | year, sex, location)'
         values are rescaled to reflect their smaller representation.
     """
-    if age_start > pop_data.age_group_end.max():
-        raise ValueError('Provided population data is insufficient to model the requested age range.')
+    col_order = pop_data.columns.copy()
+    if age_start > pop_data["age_end"].max():
+        raise ValueError(
+            "Provided population data is insufficient to model the requested age range."
+        )
 
-    age_start = max(pop_data.age_group_start.min(), age_start)
-    age_end = min(pop_data.age_group_end.max(), age_end) - 1e-8
+    age_start = max(pop_data["age_start"].min(), age_start)
+    age_end = min(pop_data["age_end"].max(), age_end) - 1e-8
     pop_data = _add_edge_age_groups(pop_data.copy())
 
-    columns_to_scale = ['P(sex, location, age| year)', 'P(age | year, sex, location)', 'value']
-    for _, sub_pop in pop_data.groupby(['sex', 'location']):
-
-        min_bin = sub_pop[(sub_pop.age_group_start <= age_start) & (age_start < sub_pop.age_group_end)]
-        padding_bin = sub_pop[sub_pop.age_group_end == float(min_bin.age_group_start)]
-
-        min_scale = ((float(min_bin.age_group_end) - age_start)
-                     / float(min_bin.age_group_end - min_bin.age_group_start))
+    columns_to_scale = [
+        "P(sex, location, age| year)",
+        "P(age | year, sex, location)",
+        "value",
+    ]
+    for _, sub_pop in pop_data.groupby(["sex", "location"]):
+        min_bin = sub_pop[
+            (sub_pop["age_start"] <= age_start) & (age_start < sub_pop["age_end"])
+        ]
+        padding_bin = sub_pop[sub_pop["age_end"] == float(min_bin["age_start"].iloc[0])]
+
+        min_scale = (float(min_bin["age_end"].iloc[0]) - age_start) / float(
+            min_bin["age_end"].iloc[0] - min_bin["age_start"].iloc[0]
+        )
 
         remainder = pop_data.loc[min_bin.index, columns_to_scale].values * (1 - min_scale)
         pop_data.loc[min_bin.index, columns_to_scale] *= min_scale
         pop_data.loc[padding_bin.index, columns_to_scale] += remainder
 
-        pop_data.loc[min_bin.index, 'age_group_start'] = age_start
-        pop_data.loc[padding_bin.index, 'age_group_end'] = age_start
+        pop_data.loc[min_bin.index, "age_start"] = age_start
+        pop_data.loc[padding_bin.index, "age_end"] = age_start
 
-        max_bin = sub_pop[(sub_pop.age_group_end > age_end) & (age_end >= sub_pop.age_group_start)]
-        padding_bin = sub_pop[sub_pop.age_group_start == float(max_bin.age_group_end)]
+        max_bin = sub_pop[(sub_pop["age_end"] > age_end) & (age_end >= sub_pop["age_start"])]
+        padding_bin = sub_pop[sub_pop["age_start"] == float(max_bin["age_end"].iloc[0])]
 
-        max_scale = ((age_end - float(max_bin.age_group_start))
-                     / float(max_bin.age_group_end - max_bin.age_group_start))
+        max_scale = (age_end - float(max_bin["age_start"].iloc[0])) / float(
+            max_bin["age_end"].iloc[0] - max_bin["age_start"].iloc[0]
+        )
 
         remainder = pop_data.loc[max_bin.index, columns_to_scale] * (1 - max_scale)
         pop_data.loc[max_bin.index, columns_to_scale] *= max_scale
         pop_data.loc[padding_bin.index, columns_to_scale] += remainder.values
 
-        pop_data.loc[max_bin.index, 'age_group_end'] = age_end
-        pop_data.loc[padding_bin.index, 'age_group_start'] = age_end
+        pop_data.loc[max_bin.index, "age_end"] = age_end
+        pop_data.loc[padding_bin.index, "age_start"] = age_end
 
-    return pop_data
+    return pop_data[col_order].sort_values(_SORT_ORDER).reset_index(drop=True)
 
 
-def _add_edge_age_groups(pop_data):
-    """
-    Pads the population data with age groups that enforce constant left interpolation
-    and interpolation to zero on the right.
-
-    Parameters
-    ----------
-    pop_data : pandas.DataFrame
+def _add_edge_age_groups(pop_data: pd.DataFrame) -> pd.DataFrame:
+    """Pads the population data with age groups that enforce constant
+    left interpolation and interpolation to zero on the right.
 
-    Returns
-    -------
-    pandas.DataFrame
     """
-    index_cols = ['location', 'year_start', 'year_end', 'sex']
-    age_cols = ['age', 'age_group_start', 'age_group_end']
+    index_cols = ["location", "year_start", "year_end", "sex"]
+    age_cols = ["age", "age_start", "age_end"]
     other_cols = [c for c in pop_data.columns if c not in index_cols + age_cols]
     pop_data = pop_data.set_index(index_cols)
 
     # For the lower bin, we want constant interpolation off the left side
-    min_valid_age = pop_data['age_group_start'].min()
+    min_valid_age = pop_data["age_start"].min()
     # This bin width needs to be the same as the lowest bin.
-    min_pad_age = min_valid_age - (pop_data['age_group_end'].min() - min_valid_age)
+    min_pad_age = min_valid_age - (pop_data["age_end"].min() - min_valid_age)
     min_pad_age_midpoint = (min_valid_age + min_pad_age) * 0.5
 
-    lower_bin = pd.DataFrame({'age_group_start': min_pad_age,
-                              'age_group_end': min_valid_age,
-                              'age': min_pad_age_midpoint}, index=pop_data.index.unique())
-    lower_bin[other_cols] = pop_data.loc[pop_data['age_group_start'] == min_valid_age, other_cols]
+    lower_bin = pd.DataFrame(
+        {"age_start": min_pad_age, "age_end": min_valid_age, "age": min_pad_age_midpoint},
+        index=pop_data.index.unique(),
+    )
+    lower_bin[other_cols] = pop_data.loc[pop_data["age_start"] == min_valid_age, other_cols]
 
     # For the upper bin, we want our interpolation to go to zero.
-    max_valid_age = pop_data['age_group_end'].max()
-    # This bin width is not arbitrary.  It effects the rate at which our interpolation zeros out.
-    # Since for the 2016 round the maximum age is 125, we're assuming almost no one lives past that age,
-    # so we make this bin 1 week.  A more robust technique for this would be better.
-    max_pad_age = max_valid_age + 7/365
+    max_valid_age = pop_data["age_end"].max()
+    # This bin width is not arbitrary.  It effects the rate at which our interpolation
+    # zeros out. Since for the 2016 round the maximum age is 125, we're assuming almost no
+    # one lives past that age, so we make this bin 1 week.  A more robust technique for
+    # this would be better.
+    max_pad_age = max_valid_age + 7 / 365
     max_pad_age_midpoint = (max_valid_age + max_pad_age) * 0.5
 
-    upper_bin = pd.DataFrame({'age_group_start': max_valid_age,
-                              'age_group_end': max_pad_age,
-                              'age': max_pad_age_midpoint}, index=pop_data.index.unique())
+    upper_bin = pd.DataFrame(
+        {"age_start": max_valid_age, "age_end": max_pad_age, "age": max_pad_age_midpoint},
+        index=pop_data.index.unique(),
+    )
     # We're doing the multiplication to ensure we get the correct data shape and index.
-    upper_bin[other_cols] = 0 * pop_data.loc[pop_data['age_group_end'] == max_valid_age, other_cols]
+    upper_bin[other_cols] = 0 * pop_data.loc[pop_data["age_end"] == max_valid_age, other_cols]
 
-    pop_data = pd.concat([lower_bin, pop_data, upper_bin]).reset_index()
+    pop_data = pd.concat([lower_bin, pop_data, upper_bin], sort=False).reset_index()
 
-    pop_data = pop_data.rename(columns={'level_0': 'location', 'level_1': 'year_start',
-                                        'level_2': 'year_end', 'level_3': 'sex'})
-    return pop_data[index_cols + age_cols + other_cols].sort_values(
-        by=['location', 'year_start', 'year_end', 'age']).reset_index(drop=True)
+    pop_data = pop_data.rename(
+        columns={
+            "level_0": "location",
+            "level_1": "year_start",
+            "level_2": "year_end",
+            "level_3": "sex",
+        }
+    )
+    return (
+        pop_data[index_cols + age_cols + other_cols]
+        .sort_values(by=["location", "year_start", "year_end", "age"])
+        .reset_index(drop=True)
+    )
 
 
-AgeValues = namedtuple('AgeValues', ['current', 'young', 'old'])
-EndpointValues = namedtuple('EndpointValues', ['left', 'right'])
+AgeValues = namedtuple("AgeValues", ["current", "young", "old"])
+EndpointValues = namedtuple("EndpointValues", ["left", "right"])
 
 
-def smooth_ages(simulants, population_data, randomness):
+def smooth_ages(
+    simulants: pd.DataFrame,
+    population_data: pd.DataFrame,
+    randomness: RandomnessStream,
+) -> pd.DataFrame:
     """Distributes simulants among ages within their assigned age bins.
 
     Parameters
     ----------
-    simulants : pandas.DataFrame
+    simulants
         Table with columns 'age', 'sex', and 'location'
-    population_data : pandas.DataFrame
+    population_data
         Table with columns 'age', 'sex', 'year', 'location', 'population',
         'P(sex, location, age| year)', 'P(sex, location | age, year)',
         'P(age | year, sex, location)'
-    randomness : vivarium.framework.randomness.RandomnessStream
+    randomness
         Source of random number generation within the vivarium common random number framework.
 
     Returns
     -------
     pandas.DataFrame
         Table with same columns as `simulants` with ages smoothed out within the age bins.
     """
     simulants = simulants.copy()
-    for (sex, location), sub_pop in population_data.groupby(['sex', 'location']):
-
-        ages = sorted(sub_pop.age.unique())
-        younger = [float(sub_pop.loc[sub_pop.age == ages[0], 'age_group_start'])] + ages[:-1]
-        older = ages[1:] + [float(sub_pop.loc[sub_pop.age == ages[-1], 'age_group_end'])]
+    for (sex, location), sub_pop in population_data.groupby(["sex", "location"]):
+        ages = sorted(sub_pop["age"].unique())
+        younger = [float(sub_pop.loc[sub_pop["age"] == ages[0], "age_start"].iloc[0])] + ages[
+            :-1
+        ]
+        older = ages[1:] + [float(sub_pop.loc[sub_pop["age"] == ages[-1], "age_end"].iloc[0])]
 
         uniform_all = randomness.get_draw(simulants.index)
 
         for age_set in zip(ages, younger, older):
             age = AgeValues(*age_set)
 
-            has_correct_demography = ((simulants.age == age.current)
-                                      & (simulants.sex == sex) & (simulants.location == location))
+            has_correct_demography = (
+                (simulants["age"] == age.current)
+                & (simulants["sex"] == sex)
+                & (simulants["location"] == location)
+            )
             affected = simulants[has_correct_demography]
 
             if affected.empty:
                 continue
 
             # bin endpoints
             endpoints, proportions = _get_bins_and_proportions(sub_pop, age)
-            pdf, slope, area, cdf_inflection_point = _construct_sampling_parameters(age, endpoints, proportions)
+            pdf, slope, area, cdf_inflection_point = _construct_sampling_parameters(
+                age, endpoints, proportions
+            )
 
             # Make a draw from a uniform distribution
             uniform_rv = uniform_all.loc[affected.index]
 
             left_sims = affected[uniform_rv <= cdf_inflection_point]
             right_sims = affected[uniform_rv > cdf_inflection_point]
 
-            simulants.loc[left_sims.index, 'age'] = _compute_ages(uniform_rv[left_sims.index],
-                                                                  endpoints.left, pdf.left, slope.left, area)
-            simulants.loc[right_sims.index, 'age'] = _compute_ages(uniform_rv[right_sims.index] - cdf_inflection_point,
-                                                                   age.current, proportions.current, slope.right, area)
+            simulants.loc[left_sims.index, "age"] = _compute_ages(
+                uniform_rv[left_sims.index], endpoints.left, pdf.left, slope.left, area
+            )
+            simulants.loc[right_sims.index, "age"] = _compute_ages(
+                uniform_rv[right_sims.index] - cdf_inflection_point,
+                age.current,
+                proportions.current,
+                slope.right,
+                area,
+            )
 
     return simulants
 
 
-def _get_bins_and_proportions(pop_data, age):
-    """Finds and returns the bin edges and the population proportions in the current and neighboring bins.
+def _get_bins_and_proportions(
+    pop_data: pd.DataFrame,
+    age: AgeValues,
+) -> Tuple[EndpointValues, AgeValues]:
+    """Finds and returns the bin edges and the population proportions in
+    the current and neighboring bins.
 
     Parameters
     ----------
-    pop_data : pandas.DataFrame
+    pop_data
         Table with columns 'age', 'sex', 'year', 'location', 'population',
         'P(sex, location, age| year)', 'P(sex, location | age, year)',
         'P(age | year, sex, location)'
-    age : AgeValues
-        Tuple with values
-            (midpoint of current age bin, midpoint of previous age bin, midpoint of next age bin)
+    age
+        Tuple with values (
+            midpoint of current age bin,
+            midpoint of previous age bin,
+            midpoint of next age bin,
+        )
 
     Returns
     -------
-    (EndpointValues, AgeValues)
-        The `EndpointValues` tuple has values
-            (age at left edge of bin, age at right edge of bin)
-        The `AgeValues` tuple has values
-            (proportion of pop in current bin, proportion of pop in previous bin, proportion of pop in next bin)
+    Tuple[EndpointValues, AgeValues]
+        The `EndpointValues` tuple has values (
+            age at left edge of bin,
+            age at right edge of bin,
+        )
+        The `AgeValues` tuple has values (
+            proportion of pop in current bin,
+            proportion of pop in previous bin,
+            proportion of pop in next bin,
+        )
+
     """
-    left = float(pop_data.loc[pop_data.age == age.current, 'age_group_start'])
-    right = float(pop_data.loc[pop_data.age == age.current, 'age_group_end'])
+    left = float(pop_data.loc[pop_data["age"] == age.current, "age_start"].iloc[0])
+    right = float(pop_data.loc[pop_data["age"] == age.current, "age_end"].iloc[0])
 
-    if not pop_data.loc[pop_data.age == age.young, 'age_group_start'].empty:
-        lower_left = float(pop_data.loc[pop_data.age == age.young, 'age_group_start'])
+    if not pop_data.loc[pop_data["age"] == age.young, "age_start"].empty:
+        lower_left = float(pop_data.loc[pop_data["age"] == age.young, "age_start"].iloc[0])
     else:
         lower_left = left
-    if not pop_data.loc[pop_data.age == age.old, 'age_group_end'].empty:
-        upper_right = float(pop_data.loc[pop_data.age == age.old, 'age_group_end'])
+    if not pop_data.loc[pop_data["age"] == age.old, "age_end"].empty:
+        upper_right = float(pop_data.loc[pop_data["age"] == age.old, "age_end"].iloc[0])
     else:
         upper_right = right
 
     # proportion in this bin and the neighboring bins
-    proportion_column = 'P(age | year, sex, location)'
-    # Here we make the assumption that P(left < age < right | year, sex, location)  = p * (right - left)
-    # in order to back out a point estimate for the probability density at the center of the interval.
-    # This not the best assumption, but it'll do.
-    p_age = float(pop_data.loc[pop_data.age == age.current, proportion_column]/(right - left))
-    p_young = float(pop_data.loc[pop_data.age == age.young, proportion_column]/(left - lower_left)) if age.young != left else p_age
-    p_old = float(pop_data.loc[pop_data.age == age.old, proportion_column]/(upper_right - right)) if age.old != right else 0
+    proportion_column = "P(age | year, sex, location)"
+    # Here we make the assumption that
+    # P(left < age < right | year, sex, location)  = p * (right - left)
+    # in order to back out a point estimate for the probability density at the center
+    # of the interval. This not the best assumption, but it'll do.
+    p_age = float(
+        pop_data.loc[pop_data["age"] == age.current, proportion_column].iloc[0]
+        / (right - left)
+    )
+    p_young = (
+        float(
+            pop_data.loc[pop_data["age"] == age.young, proportion_column].iloc[0]
+            / (left - lower_left)
+        )
+        if age.young != left
+        else p_age
+    )
+    p_old = (
+        float(
+            pop_data.loc[pop_data["age"] == age.old, proportion_column].iloc[0]
+            / (upper_right - right)
+        )
+        if age.old != right
+        else 0
+    )
 
     return EndpointValues(left, right), AgeValues(p_age, p_young, p_old)
 
 
-def _construct_sampling_parameters(age, endpoint, proportion):
+def _construct_sampling_parameters(
+    age: AgeValues, endpoint: EndpointValues, proportion: AgeValues
+) -> Tuple[EndpointValues, EndpointValues, float, float]:
     """Calculates some sampling distribution parameters from known values.
 
     Parameters
     ----------
-    age : AgeValues
-        Tuple with values
-            (midpoint of current age bin, midpoint of previous age bin, midpoint of next age bin)
+    age
+        Tuple with values (
+            midpoint of current age bin,
+            midpoint of previous age bin,
+            midpoint of next age bin,
+        )
     endpoint : EndpointValues
-        Tuple with values
-            (age at left edge of bin, age at right edge of bin)
+        Tuple with values (
+            age at left edge of bin,
+            age at right edge of bin,
+        )
     proportion : AgeValues
-        Tuple with values
-            (proportion of pop in current bin, proportion of pop in previous bin, proportion of pop in next bin)
+        Tuple with values (
+            proportion of pop in current bin,
+            proportion of pop in previous bin,
+            proportion of pop in next bin,
+        )
 
     Returns
     -------
-    (pdf, slope, area, cdf_inflection_point) : (EndpointValues, EndpointValues, float, float)
-        pdf is a tuple with values
-            (pdf evaluated at left bin edge, pdf evaluated at right bin edge)
-        slope is a tuple with values
-            (slope of pdf in left half bin, slope of pdf in right half bin)
-        area is the total area under the pdf, used for normalization
-        cdf_inflection_point is the value of the cdf at the midpoint of the age bin.
+    Tuple[EndpointValues, EndpointValues, float, float]
+        A tuple of (pdf, slope, area, cdf_inflection_point) where
+            pdf is a tuple with values (
+                pdf evaluated at left bin edge,
+                pdf evaluated at right bin edge,
+            )
+            slope is a tuple with values (
+                slope of pdf in left half bin,
+                slope of pdf in right half bin,
+            )
+            area is the total area under the pdf, used for normalization
+            cdf_inflection_point is the value of the cdf at the midpoint of the age bin.
+
     """
     # pdf value at bin endpoints
-
-    pdf_left = ((proportion.current - proportion.young) / (age.current - age.young)
-                * (endpoint.left - age.young) + proportion.young)
-    pdf_right = ((proportion.old - proportion.current) / (age.old - age.current)
-                 * (endpoint.right - age.current) + proportion.current)
-    area = 0.5 * ((proportion.current + pdf_left) * (age.current - endpoint.left)
-                  + (pdf_right + proportion.current) * (endpoint.right - age.current))
+    pdf_left = (proportion.current - proportion.young) / (age.current - age.young) * (
+        endpoint.left - age.young
+    ) + proportion.young
+    pdf_right = (proportion.old - proportion.current) / (age.old - age.current) * (
+        endpoint.right - age.current
+    ) + proportion.current
+    area = 0.5 * (
+        (proportion.current + pdf_left) * (age.current - endpoint.left)
+        + (pdf_right + proportion.current) * (endpoint.right - age.current)
+    )
 
     pdf = EndpointValues(pdf_left, pdf_right)
 
     # pdf slopes.
     m_left = (proportion.current - pdf.left) / (age.current - endpoint.left)
     m_right = (pdf.right - proportion.current) / (endpoint.right - age.current)
     slope = EndpointValues(m_left, m_right)
 
     # The decision bound on the uniform rv.
-    cdf_inflection_point = 1 / (2 * area) * (proportion.current + pdf.left) * (age.current - endpoint.left)
+    cdf_inflection_point = (
+        1 / (2 * area) * (proportion.current + pdf.left) * (age.current - endpoint.left)
+    )
 
     return pdf, slope, area, cdf_inflection_point
 
 
-def _compute_ages(uniform_rv, start, height, slope, normalization):
+def _compute_ages(
+    uniform_rv: Union[np.ndarray, float],
+    start: float,
+    height: float,
+    slope: float,
+    normalization: float,
+) -> Union[np.ndarray, float]:
     """Produces samples from the local age distribution.
 
     Parameters
     ----------
-    uniform_rv : numpy.ndarray or float
-        Values pulled from a uniform distribution and belonging to either the left or right half
-        of the local distribution.  The halves are determined by the the point Z in [0, 1] such that
-        Q(Z) = the midpoint of the age bin in question, where Q is inverse of the local
-        cumulative distribution function.
-    start : float
+    uniform_rv
+        Values pulled from a uniform distribution and belonging to either the left or
+        right half of the local distribution. The halves are determined by the point Z
+        in [0, 1] such that Q(Z) = the midpoint of the age bin in question, where Q is
+        inverse of the local cumulative distribution function.
+    start
         Either the left edge of the age bin (if we're in the left half of the distribution) or
         the midpoint of the age bin (if we're in the right half of the distribution).
-    height : float
+    height
         The value of the local distribution at `start`
-    slope : float
+    slope
         The slope of the local distribution.
-    normalization : float
+    normalization
         The total area under the distribution.
 
     Returns
     -------
-    numpy.ndarray or float
+    Union[np.ndarray, float]
         Smoothed ages from one half of the age bin distribution.
     """
-    if slope == 0:
+    if abs(slope) < np.finfo(np.float32).eps:
         return start + normalization / height * uniform_rv
     else:
-        return start + height / slope * (np.sqrt(1 + 2 * normalization * slope / height ** 2 * uniform_rv) - 1)
+        return start + height / slope * (
+            np.sqrt(1 + 2 * normalization * slope / height**2 * uniform_rv) - 1
+        )
 
 
-def get_cause_deleted_mortality(all_cause_mortality, list_of_csmrs):
-    index_cols = ['age_group_start', 'age_group_end', 'sex', 'year_start', 'year_end']
-    all_cause_mortality = all_cause_mortality.set_index(index_cols).copy()
+def get_cause_deleted_mortality_rate(all_cause_mortality_rate, list_of_csmrs):
+    index_cols = ["age_start", "age_end", "sex", "year_start", "year_end"]
+    all_cause_mortality_rate = all_cause_mortality_rate.set_index(index_cols).copy()
     for csmr in list_of_csmrs:
         if csmr is None:
             continue
-        all_cause_mortality = all_cause_mortality.subtract(csmr.set_index(index_cols)).dropna()
+        all_cause_mortality_rate = all_cause_mortality_rate.subtract(
+            csmr.set_index(index_cols)
+        ).dropna()
 
-    return all_cause_mortality.reset_index().rename(columns={'value': 'death_due_to_other_causes'})
+    return all_cause_mortality_rate.reset_index().rename(
+        columns={"value": "death_due_to_other_causes"}
+    )
 
 
 def load_population_structure(builder):
     data = builder.data.load("population.structure")
     # create an age column which is the midpoint of the age group
-    data['age'] = data.apply(lambda row: (row['age_group_start'] + row['age_group_end']) / 2, axis=1)
+    data["age"] = data.apply(lambda row: (row["age_start"] + row["age_end"]) / 2, axis=1)
+    data["location"] = builder.data.load("population.location")
     return data
 
 
 def get_live_births_per_year(builder):
     population_data = load_population_structure(builder)
     birth_data = builder.data.load("covariate.live_births_by_sex.estimate")
 
     validate_crude_birth_rate_data(builder, population_data.year_end.max())
     population_data = rescale_final_age_bin(builder, population_data)
 
     initial_population_size = builder.configuration.population.population_size
-    population_data = population_data.groupby(['year_start'])['value'].sum()
-    birth_data = (birth_data[birth_data.parameter == 'mean_value']
-                  .drop('parameter', 'columns')
-                  .groupby(['year_start'])['value'].sum())
+    population_data = population_data.groupby(["year_start"])["value"].sum()
+    birth_data = (
+        birth_data[birth_data.parameter == "mean_value"]
+        .drop(columns=["parameter"])
+        .groupby(["year_start"])["value"]
+        .sum()
+    )
 
     start_year = builder.configuration.time.start.year
-    if builder.configuration.interpolation.extrapolate and start_year > birth_data.index.max():
+    if (
+        builder.configuration.interpolation.extrapolate
+        and start_year > birth_data.index.max()
+    ):
         start_year = birth_data.index.max()
 
     if not builder.configuration.fertility.time_dependent_live_births:
         birth_data = birth_data.at[start_year]
 
     if not builder.configuration.fertility.time_dependent_population_fraction:
         population_data = population_data.at[start_year]
 
     live_birth_rate = initial_population_size / population_data * birth_data
 
     if isinstance(live_birth_rate, (int, float)):
-        live_birth_rate = pd.Series(live_birth_rate, index=pd.RangeIndex(builder.configuration.time.start.year,
-                                                                         builder.configuration.time.end.year + 1,
-                                                                         name='year'))
+        live_birth_rate = pd.Series(
+            live_birth_rate,
+            index=pd.RangeIndex(
+                builder.configuration.time.start.year,
+                builder.configuration.time.end.year + 1,
+                name="year",
+            ),
+        )
     else:
-        live_birth_rate = (live_birth_rate
-                           .reset_index()
-                           .rename(columns={'year_start': 'year'})
-                           .set_index('year')
-                           .value)
+        live_birth_rate = (
+            live_birth_rate.reset_index()
+            .rename(columns={"year_start": "year"})
+            .set_index("year")
+            .value
+        )
         exceeds_data = builder.configuration.time.end.year > live_birth_rate.index.max()
         if exceeds_data:
-            new_index = pd.RangeIndex(live_birth_rate.index.min(), builder.configuration.time.end.year + 1)
-            live_birth_rate = live_birth_rate.reindex(new_index,
-                                                      fill_value=live_birth_rate.at[live_birth_rate.index.max()])
+            new_index = pd.RangeIndex(
+                live_birth_rate.index.min(), builder.configuration.time.end.year + 1
+            )
+            live_birth_rate = live_birth_rate.reindex(
+                new_index, fill_value=live_birth_rate.at[live_birth_rate.index.max()]
+            )
     return live_birth_rate
 
 
 def rescale_final_age_bin(builder, population_data):
-    exit_age = builder.configuration.population.to_dict().get('exit_age', None)
+    exit_age = builder.configuration.population.to_dict().get("exit_age", None)
     if exit_age:
-        cut_bin = population_data[(population_data.age_group_start < exit_age)
-                                  & (population_data.age_group_end >= exit_age)]
-        cut_bin.value *= (exit_age - cut_bin.age_group_start) / (cut_bin.age_group_end - cut_bin.age_group_start)
-        cut_bin.loc[:, 'age_group_end'] = exit_age
-        population_data = population_data[population_data.age_group_end < exit_age]
-        population_data = pd.concat([population_data, cut_bin], ignore_index=True)
+        population_data = population_data.loc[population_data["age_start"] < exit_age].copy()
+        cut_bin_idx = exit_age <= population_data["age_end"]
+        cut_age_start = population_data.loc[cut_bin_idx, "age_start"]
+        cut_age_end = population_data.loc[cut_bin_idx, "age_end"]
+        population_data.loc[cut_bin_idx, "value"] *= (exit_age - cut_age_start) / (
+            cut_age_end - cut_age_start
+        )
+        population_data.loc[cut_bin_idx, "age_end"] = exit_age
     return population_data
 
 
 def validate_crude_birth_rate_data(builder, data_year_max):
-    exit_age = builder.configuration.population.to_dict().get('exit_age', None)
+    exit_age = builder.configuration.population.to_dict().get("exit_age", None)
     if exit_age and builder.configuration.population.age_end != exit_age:
-        raise ValueError('If you specify an exit age, the initial population age end must be the same '
-                         'for the crude birth rate calculation to work.')
+        raise ValueError(
+            "If you specify an exit age, the initial population age end must be the same "
+            "for the crude birth rate calculation to work."
+        )
 
     exceeds_data = builder.configuration.time.end.year > data_year_max
     if exceeds_data and not builder.configuration.interpolation.extrapolate:
-        raise ValueError('Trying to extrapolate beyond the end of available birth data.')
+        raise ValueError("Trying to extrapolate beyond the end of available birth data.")
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/population/add_new_birth_cohorts.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/population/add_new_birth_cohorts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,77 @@
-"""This module contains several components that  model birth rates."""
-import pandas as pd
+"""
+================
+Fertility Models
+================
+
+This module contains several different models of fertility.
+
+"""
 import numpy as np
-from vivarium_public_health.population.data_transformations import get_live_births_per_year
+import pandas as pd
+
+from vivarium_public_health import utilities
+from vivarium_public_health.population.data_transformations import (
+    get_live_births_per_year,
+)
 
-SECONDS_PER_YEAR = 365.25*24*60*60
 # TODO: Incorporate better data into gestational model (probably as a separate component)
-PREGNANCY_DURATION = pd.Timedelta(days=9*30.5)
+PREGNANCY_DURATION = pd.Timedelta(days=9 * utilities.DAYS_PER_MONTH)
 
 
 class FertilityDeterministic:
     """Deterministic model of births."""
 
     configuration_defaults = {
-        'fertility': {
-            'number_of_new_simulants_each_year': 1000,
+        "fertility": {
+            "number_of_new_simulants_each_year": 1000,
         },
     }
 
+    @property
+    def name(self):
+        return "deterministic_fertility"
+
     def setup(self, builder):
         self.fractional_new_births = 0
-        self.simulants_per_year = builder.configuration.fertility.number_of_new_simulants_each_year
+        self.simulants_per_year = (
+            builder.configuration.fertility.number_of_new_simulants_each_year
+        )
 
         self.simulant_creator = builder.population.get_simulant_creator()
 
-        builder.event.register_listener('time_step', self.on_time_step)
+        builder.event.register_listener("time_step", self.on_time_step)
 
     def on_time_step(self, event):
         """Adds a set number of simulants to the population each time step.
 
         Parameters
         ----------
         event
             The event that triggered the function call.
         """
         # Assume births are uniformly distributed throughout the year.
-        step_size = event.step_size/pd.Timedelta(seconds=SECONDS_PER_YEAR)
-        simulants_to_add = self.simulants_per_year*step_size + self.fractional_new_births
+        step_size = utilities.to_years(event.step_size)
+        simulants_to_add = self.simulants_per_year * step_size + self.fractional_new_births
 
         self.fractional_new_births = simulants_to_add % 1
         simulants_to_add = int(simulants_to_add)
 
         if simulants_to_add > 0:
-            self.simulant_creator(simulants_to_add,
-                                  population_configuration={
-                                      'age_start': 0,
-                                      'age_end': 0,
-                                  })
+            self.simulant_creator(
+                simulants_to_add,
+                population_configuration={
+                    "age_start": 0,
+                    "age_end": 0,
+                    "sim_state": "time_step",
+                },
+            )
+
+    def __repr__(self):
+        return "FertilityDeterministic()"
 
 
 class FertilityCrudeBirthRate:
     """Population-level model of births using crude birth rate.
 
     The number of births added each time step is calculated as
 
@@ -63,128 +85,170 @@
 
     This component has configuration flags that determine whether the
     live births and the true population size should vary with time.
 
     Notes
     -----
     The OECD definition of crude birth rate can be found on their
-    website_, while a more thorough discussion of fertility and
-    birth rate models can be found on Wikipedia_ or in demography
+    `website <https://stats.oecd.org/glossary/detail.asp?ID=490>`_,
+    while a more thorough discussion of fertility and
+    birth rate models can be found on
+    `Wikipedia <https://en.wikipedia.org/wiki/Birth_rate>`_ or in demography
     textbooks.
-    .. _website: https://stats.oecd.org/glossary/detail.asp?ID=490
-    .. _Wikipedia: https://en.wikipedia.org/wiki/Birth_rate
+
     """
 
     configuration_defaults = {
-        'fertility': {
-            'time_dependent_live_births': True,
-            'time_dependent_population_fraction': False,
+        "fertility": {
+            "time_dependent_live_births": True,
+            "time_dependent_population_fraction": False,
         }
     }
 
-    def setup(self, builder):
-        self.clock = builder.time.clock()
+    @property
+    def name(self):
+        return "crude_birthrate_fertility"
 
+    def setup(self, builder):
         self.birth_rate = get_live_births_per_year(builder)
 
-        self.randomness = builder.randomness.get_stream('crude_birth_rate')
-
+        self.clock = builder.time.clock()
+        self.randomness = builder.randomness
         self.simulant_creator = builder.population.get_simulant_creator()
 
-        builder.event.register_listener('time_step', self.on_time_step)
+        builder.event.register_listener("time_step", self.on_time_step)
 
     def on_time_step(self, event):
         """Adds new simulants every time step based on the Crude Birth Rate
         and an assumption that birth is a Poisson process
         Parameters
         ----------
         event
             The event that triggered the function call.
         """
         birth_rate = self.birth_rate.at[self.clock().year]
-        step_size = event.step_size / pd.Timedelta(seconds=SECONDS_PER_YEAR)
+        step_size = utilities.to_years(event.step_size)
 
         mean_births = birth_rate * step_size
         # Assume births occur as a Poisson process
-        r = np.random.RandomState(seed=self.randomness.get_seed())
+        r = np.random.RandomState(seed=self.randomness.get_seed("crude_birth_rate"))
         simulants_to_add = r.poisson(mean_births)
 
         if simulants_to_add > 0:
-            self.simulant_creator(simulants_to_add,
-                                  population_configuration={
-                                      'age_start': 0,
-                                      'age_end': 0,
-                                  })
+            self.simulant_creator(
+                simulants_to_add,
+                population_configuration={
+                    "age_start": 0,
+                    "age_end": 0,
+                    "sim_state": "time_step",
+                },
+            )
+
+    def __repr__(self):
+        return "FertilityCrudeBirthRate()"
 
 
 class FertilityAgeSpecificRates:
     """
     A simulant-specific model for fertility and pregnancies.
     """
 
+    @property
+    def name(self):
+        return "age_specific_fertility"
+
     def setup(self, builder):
-        """ Setup the common randomness stream and
+        """Setup the common randomness stream and
         age-specific fertility lookup tables.
         Parameters
         ----------
         builder : vivarium.engine.Builder
             Framework coordination object.
         """
-        self.randomness = builder.randomness.get_stream('fertility')
-        asfr_data = builder.data.load("covariate.age_specific_fertility_rate.estimate")
-        asfr_data = asfr_data[asfr_data.sex == 'Female'][['year_start', 'year_end',
-                                                          'age_group_start', 'age_group_end', 'mean_value']]
-        asfr_source = builder.lookup.build_table(asfr_data, key_columns=(),
-                                                 parameter_columns=[('age', 'age_group_start', 'age_group_end'),
-                                                                    ('year', 'year_start', 'year_end')],)
-        self.asfr = builder.value.register_rate_producer('fertility rate', source=asfr_source)
-        self.population_view = builder.population.get_view(['last_birth_time', 'sex', 'parent_id'])
+        age_specific_fertility_rate = self.load_age_specific_fertility_rate_data(builder)
+        fertility_rate = builder.lookup.build_table(
+            age_specific_fertility_rate, parameter_columns=["age", "year"]
+        )
+        self.fertility_rate = builder.value.register_rate_producer(
+            "fertility rate", source=fertility_rate, requires_columns=["age"]
+        )
+
+        self.randomness = builder.randomness.get_stream("fertility")
+
+        self.population_view = builder.population.get_view(
+            ["last_birth_time", "sex", "parent_id"]
+        )
         self.simulant_creator = builder.population.get_simulant_creator()
-        builder.population.initializes_simulants(self.update_state_table,
-                                                 creates_columns=['last_birth_time', 'parent_id'],
-                                                 requires_columns=['sex'])
-
-        builder.event.register_listener('time_step', self.step)
-
-    def update_state_table(self, pop_data):
-        """ Adds 'last_birth_time' and 'parent' columns to the state table."""
-
-        women = self.population_view.get(pop_data.index, query="sex == 'Female'", omit_missing_columns=True).index
-        last_birth_time = pd.Series(pd.NaT, name='last_birth_time', index=pop_data.index)
 
+        builder.population.initializes_simulants(
+            self.on_initialize_simulants,
+            creates_columns=["last_birth_time", "parent_id"],
+            requires_columns=["sex"],
+        )
+
+        builder.event.register_listener("time_step", self.on_time_step)
+
+    def on_initialize_simulants(self, pop_data):
+        """Adds 'last_birth_time' and 'parent' columns to the state table."""
+        pop = self.population_view.subview(["sex"]).get(pop_data.index)
+        women = pop.loc[pop.sex == "Female"].index
+
+        if pop_data.user_data["sim_state"] == "setup":
+            parent_id = -1
+        else:  # 'sim_state' == 'time_step'
+            parent_id = pop_data.user_data["parent_ids"]
+        pop_update = pd.DataFrame(
+            {"last_birth_time": pd.NaT, "parent_id": parent_id}, index=pop_data.index
+        )
+        # FIXME: This is a misuse of the column and makes it invalid for
+        #    tracking metrics.
         # Do the naive thing, set so all women can have children
         # and none of them have had a child in the last year.
-        last_birth_time[women] = pop_data.creation_time - pd.Timedelta(seconds=SECONDS_PER_YEAR)
+        pop_update.loc[women, "last_birth_time"] = pop_data.creation_time - pd.Timedelta(
+            days=utilities.DAYS_PER_YEAR
+        )
 
-        self.population_view.update(last_birth_time)
-        self.population_view.update(pd.Series(-1, name='parent_id', index=pop_data.index, dtype=np.int64))
+        self.population_view.update(pop_update)
 
-    def step(self, event):
+    def on_time_step(self, event):
         """Produces new children and updates parent status on time steps.
         Parameters
         ----------
         event : vivarium.population.PopulationEvent
             The event that triggered the function call.
         """
         # Get a view on all living women who haven't had a child in at least nine months.
         nine_months_ago = pd.Timestamp(event.time - PREGNANCY_DURATION)
-        population = self.population_view.get(event.index, query='alive == "alive" and sex =="Female"')
+        population = self.population_view.get(
+            event.index, query='alive == "alive" and sex =="Female"'
+        )
         can_have_children = population.last_birth_time < nine_months_ago
         eligible_women = population[can_have_children]
 
-        rate_series = self.asfr(eligible_women.index)
+        rate_series = self.fertility_rate(eligible_women.index)
         had_children = self.randomness.filter_for_rate(eligible_women, rate_series).copy()
 
-        had_children.loc[:, 'last_birth_time'] = event.time
-        self.population_view.update(had_children['last_birth_time'])
+        had_children.loc[:, "last_birth_time"] = event.time
+        self.population_view.update(had_children["last_birth_time"])
 
         # If children were born, add them to the state table and record
         # who their mother was.
         num_babies = len(had_children)
         if num_babies:
-            idx = self.simulant_creator(num_babies,
-                                        population_configuration={
-                                            'age_start': 0,
-                                            'age_end': 0,
-                                        })
-            parents = pd.Series(data=had_children.index, index=idx, name='parent_id')
-            self.population_view.update(parents)
+            self.simulant_creator(
+                num_babies,
+                population_configuration={
+                    "age_start": 0,
+                    "age_end": 0,
+                    "sim_state": "time_step",
+                    "parent_ids": had_children.index,
+                },
+            )
+
+    def load_age_specific_fertility_rate_data(self, builder):
+        asfr_data = builder.data.load("covariate.age_specific_fertility_rate.estimate")
+        columns = ["year_start", "year_end", "age_start", "age_end", "mean_value"]
+        asfr_data = asfr_data.loc[asfr_data.sex == "Female"][columns]
+        return asfr_data
+
+    def __repr__(self):
+        return "FertilityAgeSpecificRates()"
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/data_transformations.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/data_transformations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,380 +1,513 @@
+"""
+=========================
+Risk Data Transformations
+=========================
+
+This module contains tools for handling raw risk exposure and relative
+risk data and performing any necessary data transformations.
+
+"""
+
 from typing import Union
 
 import numpy as np
 import pandas as pd
+from loguru import logger
 
-from vivarium.framework.randomness import RandomnessStream
-from vivarium_public_health.risks import distributions
 from vivarium_public_health.utilities import EntityString, TargetString
 
-
 #############
 # Utilities #
 #############
 
+
 def pivot_categorical(data: pd.DataFrame) -> pd.DataFrame:
     """Pivots data that is long on categories to be wide."""
-    key_cols = ['sex', 'age_group_start', 'age_group_end', 'year_start', 'year_end']
-    data = data.pivot_table(index=key_cols, columns='parameter', values='value').reset_index()
+    key_cols = ["sex", "age_start", "age_end", "year_start", "year_end"]
+    key_cols = [k for k in key_cols if k in data.columns]
+    data = data.pivot_table(index=key_cols, columns="parameter", values="value").reset_index()
     data.columns.name = None
     return data
 
 
 ##########################
 # Exposure data handlers #
 ##########################
 
-def get_distribution(builder, risk: EntityString):
+
+def get_distribution_data(builder, risk: EntityString):
     validate_distribution_data_source(builder, risk)
     data = load_distribution_data(builder, risk)
-    return distributions.get_distribution(risk.name, **data)
+    return data
 
 
 def get_exposure_post_processor(builder, risk: EntityString):
-    thresholds = builder.configuration[risk.name]['category_thresholds']
+    thresholds = builder.configuration[risk.name]["category_thresholds"]
 
     if thresholds:
         thresholds = [-np.inf] + thresholds + [np.inf]
-        categories = [f'cat{i}' for i in range(1, len(thresholds))]
+        categories = [f"cat{i}" for i in range(1, len(thresholds))]
 
         def post_processor(exposure, _):
-            return pd.Series(pd.cut(exposure, thresholds, labels=categories), index=exposure.index).astype(str)
+            return pd.Series(
+                pd.cut(exposure, thresholds, labels=categories), index=exposure.index
+            ).astype(str)
+
     else:
         post_processor = None
 
     return post_processor
 
 
 def load_distribution_data(builder, risk: EntityString):
     exposure_data = get_exposure_data(builder, risk)
 
-    data = {'distribution_type': get_distribution_type(builder, risk),
-            'exposure': exposure_data,
-            'exposure_standard_deviation': get_exposure_standard_deviation_data(builder, risk),
-            'weights': get_exposure_distribution_weights(builder, risk)}
+    data = {
+        "distribution_type": get_distribution_type(builder, risk),
+        "exposure": exposure_data,
+        "exposure_standard_deviation": get_exposure_standard_deviation_data(builder, risk),
+        "weights": get_exposure_distribution_weights(builder, risk),
+    }
     return data
 
 
 def get_distribution_type(builder, risk: EntityString):
     risk_config = builder.configuration[risk.name]
 
-    if risk_config['exposure'] == 'data' and not risk_config['rebinned_exposed']:
-        distribution_type = builder.data.load(f'{risk}.distribution')
+    if risk_config["exposure"] == "data" and not risk_config["rebinned_exposed"]:
+        distribution_type = builder.data.load(f"{risk}.distribution")
     else:
-        distribution_type = 'dichotomous'
+        distribution_type = "dichotomous"
 
     return distribution_type
 
 
 def get_exposure_data(builder, risk: EntityString):
     exposure_data = load_exposure_data(builder, risk)
     exposure_data = rebin_exposure_data(builder, risk, exposure_data)
 
-    if get_distribution_type(builder, risk) in ['dichotomous', 'ordered_polytomous', 'unordered_polytomous']:
+    if get_distribution_type(builder, risk) in [
+        "dichotomous",
+        "ordered_polytomous",
+        "unordered_polytomous",
+        "lbwsg",
+    ]:
         exposure_data = pivot_categorical(exposure_data)
 
     return exposure_data
 
 
 def load_exposure_data(builder, risk: EntityString):
     risk_config = builder.configuration[risk.name]
-    exposure_source = risk_config['exposure']
+    exposure_source = risk_config["exposure"]
 
-    if exposure_source == 'data':
-        exposure_data = builder.data.load(f'{risk}.exposure')
+    if exposure_source == "data":
+        exposure_data = builder.data.load(f"{risk}.exposure")
     else:
         if isinstance(exposure_source, str):  # Build from covariate
-            cat1 = builder.data.load(f'{exposure_source}.estimate')
+            cat1 = builder.data.load(f"{exposure_source}.estimate")
             # TODO: Generate a draw.
-            cat1 = cat1[cat1['parameter'] == 'mean_value']
-            cat1['parameter'] = 'cat1'
+            cat1 = cat1[cat1["parameter"] == "mean_value"]
+            cat1["parameter"] = "cat1"
         else:  # We have a numerical value
-            cat1 = builder.data.load('population.demographic_dimensions')
-            cat1['parameter'] = 'cat1'
-            cat1['value'] = float(exposure_source)
+            cat1 = builder.data.load("population.demographic_dimensions")
+            cat1["parameter"] = "cat1"
+            cat1["value"] = float(exposure_source)
         cat2 = cat1.copy()
-        cat2['parameter'] = 'cat2'
-        cat2['value'] = 1 - cat2['value']
+        cat2["parameter"] = "cat2"
+        cat2["value"] = 1 - cat2["value"]
         exposure_data = pd.concat([cat1, cat2], ignore_index=True)
 
     return exposure_data
 
 
 def get_exposure_standard_deviation_data(builder, risk: EntityString):
     distribution_type = get_distribution_type(builder, risk)
-    if distribution_type in ['normal', 'lognormal', 'ensemble']:
-        exposure_sd = builder.data.load(f'{risk}.exposure_standard_deviation')
+    if distribution_type in ["normal", "lognormal", "ensemble"]:
+        exposure_sd = builder.data.load(f"{risk}.exposure_standard_deviation")
     else:
         exposure_sd = None
     return exposure_sd
 
 
 def get_exposure_distribution_weights(builder, risk: EntityString):
     distribution_type = get_distribution_type(builder, risk)
-    if distribution_type == 'ensemble':
-        weights = builder.data.load(f'{risk}.exposure_distribution_weights')
+    if distribution_type == "ensemble":
+        weights = builder.data.load(f"{risk}.exposure_distribution_weights")
         weights = pivot_categorical(weights)
-        if 'glnorm' in weights.columns:
-            if np.any(weights['glnorm']):
-                raise NotImplementedError('glnorm distribution is not supported')
-            weights = weights.drop(columns='glnorm')
+        if "glnorm" in weights.columns:
+            if np.any(weights["glnorm"]):
+                raise NotImplementedError("glnorm distribution is not supported")
+            weights = weights.drop(columns=["glnorm"])
     else:
         weights = None
     return weights
 
 
 def rebin_exposure_data(builder, risk: EntityString, exposure_data: pd.DataFrame):
     validate_rebin_source(builder, risk, exposure_data)
-    rebin_exposed_categories = set(builder.configuration[risk.name]['rebinned_exposed'])
+    rebin_exposed_categories = set(builder.configuration[risk.name]["rebinned_exposed"])
 
     if rebin_exposed_categories:
         exposure_data = _rebin_exposure_data(exposure_data, rebin_exposed_categories)
 
     return exposure_data
 
 
-def _rebin_exposure_data(exposure_data: pd.DataFrame, rebin_exposed_categories: set) -> pd.DataFrame:
-    exposure_data["parameter"] = (exposure_data["parameter"]
-                                  .map(lambda p: 'cat1' if p in rebin_exposed_categories else 'cat2'))
-    return exposure_data.groupby(list(exposure_data.columns.difference(['value']))).sum().reset_index()
+def _rebin_exposure_data(
+    exposure_data: pd.DataFrame, rebin_exposed_categories: set
+) -> pd.DataFrame:
+    exposure_data["parameter"] = exposure_data["parameter"].map(
+        lambda p: "cat1" if p in rebin_exposed_categories else "cat2"
+    )
+    return (
+        exposure_data.groupby(list(exposure_data.columns.difference(["value"])))
+        .sum()
+        .reset_index()
+    )
 
 
 ###############################
 # Relative risk data handlers #
 ###############################
 
-def get_relative_risk_data(builder, risk: EntityString, target: TargetString, randomness: RandomnessStream):
+
+def get_relative_risk_data(builder, risk: EntityString, target: TargetString):
     source_type = validate_relative_risk_data_source(builder, risk, target)
-    relative_risk_data = load_relative_risk_data(builder, risk, target, source_type, randomness)
+    relative_risk_data = load_relative_risk_data(builder, risk, target, source_type)
+    validate_relative_risk_rebin_source(builder, risk, target, relative_risk_data)
     relative_risk_data = rebin_relative_risk_data(builder, risk, relative_risk_data)
 
-    if get_distribution_type(builder, risk) in ['dichotomous', 'ordered_polytomous', 'unordered_polytomous']:
+    if get_distribution_type(builder, risk) in [
+        "dichotomous",
+        "ordered_polytomous",
+        "unordered_polytomous",
+    ]:
         relative_risk_data = pivot_categorical(relative_risk_data)
+        # Check if any values for relative risk are below expected boundary of 1.0
+        category_columns = [c for c in relative_risk_data.columns if "cat" in c]
+        if not relative_risk_data[
+            (relative_risk_data[category_columns] < 1.0).any(axis=1)
+        ].empty:
+            logger.warning(
+                f"WARNING: Some data values are below the expected boundary of 1.0 for {risk}.relative_risk"
+            )
 
     else:
-        relative_risk_data = relative_risk_data.drop(['parameter'], 'columns')
+        relative_risk_data = relative_risk_data.drop(columns=["parameter"])
 
     return relative_risk_data
 
 
-def load_relative_risk_data(builder, risk: EntityString, target: TargetString,
-                            source_type: str, randomness: RandomnessStream):
-    relative_risk_source = builder.configuration[f'effect_of_{risk.name}_on_{target.name}'][target.measure]
-
-    if source_type == 'data':
-        relative_risk_data = builder.data.load(f'{risk}.relative_risk')
-        correct_target = ((relative_risk_data['affected_entity'] == target.name)
-                          & (relative_risk_data['affected_measure'] == target.measure))
-        relative_risk_data = (relative_risk_data[correct_target]
-                              .drop(['affected_entity', 'affected_measure'], 'columns'))
-
-    elif source_type == 'relative risk value':
-        relative_risk_data = _make_relative_risk_data(builder, float(relative_risk_source['relative_risk']))
+def load_relative_risk_data(
+    builder, risk: EntityString, target: TargetString, source_type: str
+):
+    relative_risk_source = builder.configuration[f"effect_of_{risk.name}_on_{target.name}"][
+        target.measure
+    ]
+
+    if source_type == "data":
+        relative_risk_data = builder.data.load(f"{risk}.relative_risk")
+        correct_target = (relative_risk_data["affected_entity"] == target.name) & (
+            relative_risk_data["affected_measure"] == target.measure
+        )
+        relative_risk_data = relative_risk_data[correct_target].drop(
+            columns=["affected_entity", "affected_measure"]
+        )
+
+    elif source_type == "relative risk value":
+        relative_risk_data = _make_relative_risk_data(
+            builder, float(relative_risk_source["relative_risk"])
+        )
 
     else:  # distribution
-        parameters = {k: v.get_value() for k, v in relative_risk_source.items() if v.get_value() is not None}
-        random_state = np.random.RandomState(randomness.get_seed())
+        parameters = {
+            k: v for k, v in relative_risk_source.to_dict().items() if v is not None
+        }
+        random_state = np.random.RandomState(
+            builder.randomness.get_seed(
+                f"effect_of_{risk.name}_on_{target.name}.{target.measure}"
+            )
+        )
         cat1_value = generate_relative_risk_from_distribution(random_state, parameters)
         relative_risk_data = _make_relative_risk_data(builder, cat1_value)
 
     return relative_risk_data
 
 
-def generate_relative_risk_from_distribution(random_state: np.random.RandomState,
-                                             parameters: dict) -> Union[float, pd.Series, np.ndarray]:
+def generate_relative_risk_from_distribution(
+    random_state: np.random.RandomState, parameters: dict
+) -> Union[float, pd.Series, np.ndarray]:
     first = pd.Series(list(parameters.values())[0])
     length = len(first)
     index = first.index
 
     for v in parameters.values():
         if length != len(pd.Series(v)) or not index.equals(pd.Series(v).index):
-            raise ValueError('If specifying vectorized parameters, all parameters '
-                             'must be the same length and have the same index.')
-
-    if 'mean' in parameters:  # normal distribution
-        rr_value = random_state.normal(parameters['mean'], parameters['se'])
-    elif 'log_mean' in parameters:  # log distribution
-        rr_value = np.exp(parameters['log_se'] * random_state.randn()
-                          + parameters['log_mean'] + random_state.normal(0, parameters['tau_squared']))
-    else:
-        raise NotImplementedError(f'Only normal distributions (supplying mean and se) and log distributions '
-                                  f'(supplying log_mean, log_se, and tau_squared) are currently supported.')
+            raise ValueError(
+                "If specifying vectorized parameters, all parameters "
+                "must be the same length and have the same index."
+            )
+
+    if "mean" in parameters:  # normal distribution
+        rr_value = random_state.normal(parameters["mean"], parameters["se"])
+    elif "log_mean" in parameters:  # log distribution
+        log_value = parameters["log_mean"] + parameters["log_se"] * random_state.randn()
+        if parameters["tau_squared"]:
+            log_value += random_state.normal(0, parameters["tau_squared"])
+        rr_value = np.exp(log_value)
+    else:
+        raise NotImplementedError(
+            f"Only normal distributions (supplying mean and se) and log distributions "
+            f"(supplying log_mean, log_se, and tau_squared) are currently supported."
+        )
 
     rr_value = np.maximum(1, rr_value)
 
     return rr_value
 
 
 def _make_relative_risk_data(builder, cat1_value: float) -> pd.DataFrame:
-    cat1 = builder.data.load('population.demographic_dimensions')
-    cat1['parameter'] = 'cat1'
-    cat1['value'] = cat1_value
+    cat1 = builder.data.load("population.demographic_dimensions")
+    cat1["parameter"] = "cat1"
+    cat1["value"] = cat1_value
     cat2 = cat1.copy()
-    cat2['parameter'] = 'cat2'
-    cat2['value'] = 1
+    cat2["parameter"] = "cat2"
+    cat2["value"] = 1
     return pd.concat([cat1, cat2], ignore_index=True)
 
 
-def rebin_relative_risk_data(builder, risk: EntityString, relative_risk_data: pd.DataFrame) -> pd.DataFrame:
-    """ When the polytomous risk is rebinned, matching relative risk needs to be rebinned.
-        After rebinning, rr for both exposed and unexposed categories should be the weighted sum of relative risk
-        of the component categories where weights are relative proportions of exposure of those categories.
-        For example, if cat1, cat2, cat3 are exposed categories and cat4 is unexposed with exposure [0.1,0.2,0.3,0.4],
-        for the matching rr = [rr1, rr2, rr3, 1], rebinned rr for the rebinned cat1 should be:
-        (0.1 *rr1 + 0.2 * rr2 + 0.3* rr3) / (0.1+0.2+0.3)
+def rebin_relative_risk_data(
+    builder, risk: EntityString, relative_risk_data: pd.DataFrame
+) -> pd.DataFrame:
+    """When the polytomous risk is rebinned, matching relative risk needs to be rebinned.
+    After rebinning, rr for both exposed and unexposed categories should be the weighted sum of relative risk
+    of the component categories where weights are relative proportions of exposure of those categories.
+    For example, if cat1, cat2, cat3 are exposed categories and cat4 is unexposed with exposure [0.1,0.2,0.3,0.4],
+    for the matching rr = [rr1, rr2, rr3, 1], rebinned rr for the rebinned cat1 should be:
+    (0.1 *rr1 + 0.2 * rr2 + 0.3* rr3) / (0.1+0.2+0.3)
     """
-    rebin_exposed_categories = set(builder.configuration[risk.name]['rebinned_exposed'])
-    validate_rebin_source(builder, risk, relative_risk_data)
+    rebin_exposed_categories = set(builder.configuration[risk.name]["rebinned_exposed"])
 
     if rebin_exposed_categories:
         exposure_data = load_exposure_data(builder, risk)
-        relative_risk_data = _rebin_relative_risk_data(relative_risk_data, exposure_data, rebin_exposed_categories)
+        relative_risk_data = _rebin_relative_risk_data(
+            relative_risk_data, exposure_data, rebin_exposed_categories
+        )
 
     return relative_risk_data
 
 
-def _rebin_relative_risk_data(relative_risk_data: pd.DataFrame, exposure_data: pd.DataFrame,
-                              rebin_exposed_categories: set) -> pd.DataFrame:
-    cols = list(exposure_data.columns.difference(['value']))
+def _rebin_relative_risk_data(
+    relative_risk_data: pd.DataFrame,
+    exposure_data: pd.DataFrame,
+    rebin_exposed_categories: set,
+) -> pd.DataFrame:
+    cols = list(exposure_data.columns.difference(["value"]))
 
     relative_risk_data = relative_risk_data.merge(exposure_data, on=cols)
-    relative_risk_data['value_x'] = relative_risk_data.value_x.multiply(relative_risk_data.value_y)
-    relative_risk_data.parameter = (relative_risk_data["parameter"]
-                                    .map(lambda p: 'cat1' if p in rebin_exposed_categories else 'cat2'))
+    relative_risk_data["value_x"] = relative_risk_data.value_x.multiply(
+        relative_risk_data.value_y
+    )
+    relative_risk_data.parameter = relative_risk_data["parameter"].map(
+        lambda p: "cat1" if p in rebin_exposed_categories else "cat2"
+    )
     relative_risk_data = relative_risk_data.groupby(cols).sum().reset_index()
-    relative_risk_data['value'] = relative_risk_data.value_x.divide(relative_risk_data.value_y).fillna(0)
-    return relative_risk_data.drop(['value_x', 'value_y'], 'columns')
+    relative_risk_data["value"] = relative_risk_data.value_x.divide(
+        relative_risk_data.value_y
+    ).fillna(0)
+    return relative_risk_data.drop(columns=["value_x", "value_y"])
 
 
 def get_exposure_effect(builder, risk: EntityString):
     distribution_type = get_distribution_type(builder, risk)
-    risk_exposure = builder.value.get_value(f'{risk.name}.exposure')
+    risk_exposure = builder.value.get_value(f"{risk.name}.exposure")
 
-    if distribution_type in ['normal', 'lognormal', 'ensemble']:
+    if distribution_type in ["normal", "lognormal", "ensemble"]:
         tmred = builder.data.load(f"{risk}.tmred")
         tmrel = 0.5 * (tmred["min"] + tmred["max"])
         scale = builder.data.load(f"{risk}.relative_risk_scalar")
 
         def exposure_effect(rates, rr):
             exposure = risk_exposure(rr.index)
             relative_risk = np.maximum(rr.values ** ((exposure - tmrel) / scale), 1)
             return rates * relative_risk
+
     else:
-        def exposure_effect(rates, rr):
-            exposure = risk_exposure(rr.index)
-            return rates * (rr.lookup(exposure.index, exposure))
+
+        def exposure_effect(rates, rr: pd.DataFrame) -> pd.Series:
+            index_columns = ["index", risk.name]
+
+            exposure = risk_exposure(rr.index).reset_index()
+            exposure.columns = index_columns
+            exposure = exposure.set_index(index_columns)
+
+            relative_risk = rr.stack().reset_index()
+            relative_risk.columns = index_columns + ["value"]
+            relative_risk = relative_risk.set_index(index_columns)
+
+            effect = relative_risk.loc[exposure.index, "value"].droplevel(risk.name)
+            affected_rates = rates * effect
+            return affected_rates
 
     return exposure_effect
 
 
 ##################################################
 # Population attributable fraction data handlers #
 ##################################################
 
-def get_population_attributable_fraction_data(builder, risk: EntityString,
-                                              target: TargetString, randomness: RandomnessStream):
-    exposure_source = builder.configuration[f'{risk.name}']['exposure']
+
+def get_population_attributable_fraction_data(
+    builder, risk: EntityString, target: TargetString
+):
+    exposure_source = builder.configuration[f"{risk.name}"]["exposure"]
     rr_source_type = validate_relative_risk_data_source(builder, risk, target)
 
-    if exposure_source == 'data' and rr_source_type == 'data' and risk.type == 'risk_factor':
-        paf_data = builder.data.load(f'{risk}.population_attributable_fraction')
-        correct_target = ((paf_data['affected_entity'] == target.name)
-                          & (paf_data['affected_measure'] == target.measure))
-        paf_data = (paf_data[correct_target]
-                    .drop(['affected_entity', 'affected_measure'], 'columns'))
+    if exposure_source == "data" and rr_source_type == "data" and risk.type == "risk_factor":
+        paf_data = builder.data.load(f"{risk}.population_attributable_fraction")
+        correct_target = (paf_data["affected_entity"] == target.name) & (
+            paf_data["affected_measure"] == target.measure
+        )
+        paf_data = paf_data[correct_target].drop(
+            columns=["affected_entity", "affected_measure"]
+        )
     else:
-        key_cols = ['sex', 'age_group_start', 'age_group_end', 'year_start', 'year_end']
+        key_cols = ["sex", "age_start", "age_end", "year_start", "year_end"]
         exposure_data = get_exposure_data(builder, risk).set_index(key_cols)
-        relative_risk_data = get_relative_risk_data(builder, risk, target, randomness).set_index(key_cols)
+        relative_risk_data = get_relative_risk_data(builder, risk, target).set_index(key_cols)
         mean_rr = (exposure_data * relative_risk_data).sum(axis=1)
-        paf_data = ((mean_rr - 1)/mean_rr).reset_index().rename(columns={0: 'value'})
+        paf_data = ((mean_rr - 1) / mean_rr).reset_index().rename(columns={0: "value"})
     return paf_data
 
 
 ##############
 # Validators #
 ##############
 
+
 def validate_distribution_data_source(builder, risk: EntityString):
     """Checks that the exposure distribution specification is valid."""
-    exposure_type = builder.configuration[risk.name]['exposure']
-    rebin = builder.configuration[risk.name]['rebin']
-    category_thresholds = builder.configuration[risk.name]['category_thresholds']
-
-    if risk.type == 'alternative_risk_factor':
-        if exposure_type != 'data' or rebin:
-            raise ValueError('Parameterized risk components are not available for alternative risks.')
+    exposure_type = builder.configuration[risk.name]["exposure"]
+    rebin = builder.configuration[risk.name]["rebinned_exposed"]
+    category_thresholds = builder.configuration[risk.name]["category_thresholds"]
+
+    if risk.type == "alternative_risk_factor":
+        if exposure_type != "data" or rebin:
+            raise ValueError(
+                "Parameterized risk components are not available for alternative risks."
+            )
 
         if not category_thresholds:
-            raise ValueError('Must specify category thresholds to use alternative risks.')
+            raise ValueError("Must specify category thresholds to use alternative risks.")
 
-    elif risk.type in ['risk_factor', 'coverage_gap']:
+    elif risk.type in ["risk_factor", "coverage_gap"]:
         if isinstance(exposure_type, (int, float)) and not 0 <= exposure_type <= 1:
             raise ValueError(f"Exposure should be in the range [0, 1]")
-        elif isinstance(exposure_type, str) and exposure_type.split('.')[0] not in ['covariate', 'data']:
-            raise ValueError(f"Exposure must be specified as 'data', an integer or float value, "
-                             f"or as a string in the format covariate.covariate_name")
+        elif isinstance(exposure_type, str) and exposure_type.split(".")[0] not in [
+            "covariate",
+            "data",
+        ]:
+            raise ValueError(
+                f"Exposure must be specified as 'data', an integer or float value, "
+                f"or as a string in the format covariate.covariate_name"
+            )
         else:
             pass  # All good
     else:
-        raise ValueError(f'Unknown risk type {risk.type} for risk {risk.name}')
+        raise ValueError(f"Unknown risk type {risk.type} for risk {risk.name}")
 
 
 def validate_relative_risk_data_source(builder, risk: EntityString, target: TargetString):
-    source_key = f'effect_of_{risk.name}_on_{target.name}'
+    source_key = f"effect_of_{risk.name}_on_{target.name}"
     relative_risk_source = builder.configuration[source_key][target.measure]
 
-    provided_keys = set(k for k, v in relative_risk_source.items() if isinstance(v.get_value(), (int, float)))
-
-    source_map = {'data': set(),
-                  'relative risk value': {'relative_risk'},
-                  'normal distribution': {'mean', 'se'},
-                  'log distribution': {'log_mean', 'log_se', 'tau_squared'}}
+    provided_keys = set(
+        k for k, v in relative_risk_source.to_dict().items() if isinstance(v, (int, float))
+    )
+
+    source_map = {
+        "data": set(),
+        "relative risk value": {"relative_risk"},
+        "normal distribution": {"mean", "se"},
+        "log distribution": {"log_mean", "log_se", "tau_squared"},
+    }
 
     if provided_keys not in source_map.values():
-        raise ValueError(f'The acceptable parameter options for specifying relative risk are: '
-                         f'{source_map.values()}. You provided {provided_keys} for {source_key}.')
+        raise ValueError(
+            f"The acceptable parameter options for specifying relative risk are: "
+            f"{source_map.values()}. You provided {provided_keys} for {source_key}."
+        )
 
     source_type = [k for k, v in source_map.items() if provided_keys == v][0]
 
-    if source_type == 'relative risk value':
-        if not 1 <= relative_risk_source['relative_risk'] <= 100:
-            raise ValueError(f"If specifying a single value for relative risk, it should be in the "
-                             f"range [1, 100]. You provided {relative_risk_source['relative_risk']} for {source_key}.")
-    elif source_type == 'normal distribution':
-        if relative_risk_source['mean'] <= 0 or relative_risk_source['se'] <= 0:
-            raise ValueError(f"To specify parameters for a normal distribution for a risk effect, you must provide"
-                             f"both mean and se above 0. This is not the case for {source_key}.")
-    elif source_type == 'log distribution':
-        if relative_risk_source['log_mean'] <= 0 or relative_risk_source['log_se'] <= 0:
-            raise ValueError(f"To specify parameters for a log distribution for a risk effect, you must provide"
-                             f"both log_mean and log_se above 0. This is not the case for {source_key}.")
-        if relative_risk_source['tau_squared'] < 0:
-            raise ValueError(f"To specify parameters for a log distribution for a risk effect, you must provide"
-                             f"tau_squared >= 0. This is not the case for {source_key}.")
+    if source_type == "relative risk value":
+        if not 1 <= relative_risk_source["relative_risk"] <= 100:
+            raise ValueError(
+                f"If specifying a single value for relative risk, it should be in the "
+                f"range [1, 100]. You provided {relative_risk_source['relative_risk']} for {source_key}."
+            )
+    elif source_type == "normal distribution":
+        if relative_risk_source["mean"] <= 0 or relative_risk_source["se"] <= 0:
+            raise ValueError(
+                f"To specify parameters for a normal distribution for a risk effect, you must provide"
+                f"both mean and se above 0. This is not the case for {source_key}."
+            )
+    elif source_type == "log distribution":
+        if relative_risk_source["log_mean"] <= 0 or relative_risk_source["log_se"] <= 0:
+            raise ValueError(
+                f"To specify parameters for a log distribution for a risk effect, you must provide"
+                f"both log_mean and log_se above 0. This is not the case for {source_key}."
+            )
+        if relative_risk_source["tau_squared"] < 0:
+            raise ValueError(
+                f"To specify parameters for a log distribution for a risk effect, you must provide"
+                f"tau_squared >= 0. This is not the case for {source_key}."
+            )
     else:
         pass
 
     return source_type
 
 
+def validate_relative_risk_rebin_source(
+    builder, risk: EntityString, target: TargetString, data: pd.DataFrame
+):
+    if data.index.size == 0:
+        raise ValueError(
+            f"Subsetting {risk} relative risk data to {target.name} {target.measure} "
+            "returned an empty DataFrame. Check your artifact."
+        )
+    validate_rebin_source(builder, risk, data)
+
+
 def validate_rebin_source(builder, risk: EntityString, data: pd.DataFrame):
-    rebin_exposed_categories = set(builder.configuration[risk.name]['rebinned_exposed'])
+    rebin_exposed_categories = set(builder.configuration[risk.name]["rebinned_exposed"])
 
-    if rebin_exposed_categories and builder.configuration[risk.name]['category_thresholds']:
-        raise ValueError(f'Rebinning and category thresholds are mutually exclusive. '
-                         f'You provided both for {risk.name}.')
-
-    if rebin_exposed_categories and 'polytomous' not in builder.data.load(f'{risk}.distribution'):
-        raise ValueError(f'Rebinning is only supported for polytomous risks. You provided rebinning exposed categories'
-                         f'for {risk.name}, which is of type {builder.data.load(f"{risk}.distribution")}.')
+    if rebin_exposed_categories and builder.configuration[risk.name]["category_thresholds"]:
+        raise ValueError(
+            f"Rebinning and category thresholds are mutually exclusive. "
+            f"You provided both for {risk.name}."
+        )
+
+    if rebin_exposed_categories and "polytomous" not in builder.data.load(
+        f"{risk}.distribution"
+    ):
+        raise ValueError(
+            f"Rebinning is only supported for polytomous risks. You provided rebinning exposed categories"
+            f'for {risk.name}, which is of type {builder.data.load(f"{risk}.distribution")}.'
+        )
 
     invalid_cats = rebin_exposed_categories.difference(set(data.parameter))
     if invalid_cats:
-        raise ValueError(f'The following provided categories for the rebinned exposed category of {risk.name} '
-                         f'are not found in the exposure data: {invalid_cats}.')
+        raise ValueError(
+            f"The following provided categories for the rebinned exposed category of {risk.name} "
+            f"are not found in the exposure data: {invalid_cats}."
+        )
 
     if rebin_exposed_categories == set(data.parameter):
-        raise ValueError(f'The provided categories for the rebinned exposed category of {risk.name} comprise all '
-                         f'categories for the exposure data. At least one category must be left out of the provided '
-                         f'categories to be rebinned into the unexposed category.')
+        raise ValueError(
+            f"The provided categories for the rebinned exposed category of {risk.name} comprise all "
+            f"categories for the exposure data. At least one category must be left out of the provided "
+            f"categories to be rebinned into the unexposed category."
+        )
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/distributions.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/effect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,182 @@
-import numpy as np
-import pandas as pd
-
-from risk_distributions import EnsembleDistribution, Normal, LogNormal
-
-from vivarium.framework.values import list_combiner, joint_value_post_processor
+"""
+==================
+Risk Effect Models
+==================
 
+This module contains tools for modeling the relationship between risk
+exposure models and disease models.
 
-class MissingDataError(Exception):
-    pass
+"""
 
+from typing import Callable, Dict
 
-class EnsembleSimulation:
-    def __init__(self, weights, mean, sd):
-        self._weights, self._parameters = self._get_parameters(weights, mean, sd)
-
-    def setup(self, builder):
-        self.weights = builder.lookup.build_table(self._weights)
-        self.parameters = {k: builder.lookup.build_table(v) for k, v in self._parameters.items()}
-
-    def _get_parameters(self, weights, mean, sd):
-        index_cols = ['sex', 'age_group_start', 'age_group_end', 'year_start', 'year_end']
-        weights = weights.set_index(index_cols)
-        mean = mean.set_index(index_cols)['value']
-        sd = sd.set_index(index_cols)['value']
-        weights, parameters = EnsembleDistribution.get_parameters(weights, mean=mean, sd=sd)
-        return weights.reset_index(), {name: p.reset_index() for name, p in parameters.items()}
-
-    def ppf(self, q):
-        if not q.empty:
-            # We limit valid propensity to [0.001 0.999]. Beyond that bound values return NaN and then become zero,
-            # which is nonsensical. We avoid the inclusive limit to protect ourselves from a math error.
-            q[q >= 0.999] = 0.998
-            q[q <= 0.001] = 0.0011
-            weights = self.weights(q.index)
-            parameters = {name: parameter(q.index) for name, parameter in self.parameters.items()}
-            x = EnsembleDistribution(weights, parameters).ppf(q)
-            x[x.isnull()] = 0
-        else:
-            x = pd.Series([])
-        return x
+import numpy as np
+import pandas as pd
+from vivarium.framework.engine import Builder
+from vivarium.framework.lookup import LookupTable
 
+from vivarium_public_health.risks.data_transformations import (
+    get_distribution_type,
+    get_population_attributable_fraction_data,
+    get_relative_risk_data,
+)
+from vivarium_public_health.utilities import EntityString, TargetString
+
+
+class RiskEffect:
+    """A component to model the impact of a risk factor on the target rate of
+    some affected entity. This component can source data either from
+    builder.data or from parameters supplied in the configuration.
+    For a risk named 'risk' that affects 'affected_risk' and 'affected_cause',
+    the configuration would look like:
+
+    .. code-block:: yaml
+
+       configuration:
+           effect_of_risk_on_affected_risk:
+               exposure_parameters: 2
+               incidence_rate: 10
+
+    """
+
+    configuration_defaults = {
+        "effect_of_risk_on_target": {
+            "measure": {
+                "relative_risk": None,
+                "mean": None,
+                "se": None,
+                "log_mean": None,
+                "log_se": None,
+                "tau_squared": None,
+            }
+        }
+    }
+
+    def __init__(self, risk: str, target: str):
+        """
+        Parameters
+        ----------
+        risk :
+            Type and name of risk factor, supplied in the form
+            "risk_type.risk_name" where risk_type should be singular (e.g.,
+            risk_factor instead of risk_factors).
+        target :
+            Type, name, and target rate of entity to be affected by risk factor,
+            supplied in the form "entity_type.entity_name.measure"
+            where entity_type should be singular (e.g., cause instead of causes).
+        """
+        self.risk = EntityString(risk)
+        self.target = TargetString(target)
+        self.configuration_defaults = self._get_configuration_defaults()
+
+        self.exposure_pipeline_name = f"{self.risk.name}.exposure"
+        self.target_pipeline_name = f"{self.target.name}.{self.target.measure}"
+        self.target_paf_pipeline_name = f"{self.target_pipeline_name}.paf"
+
+    def __repr__(self):
+        return f"RiskEffect(risk={self.risk}, target={self.target})"
+
+    ##########################
+    # Initialization methods #
+    ##########################
+
+    def _get_configuration_defaults(self) -> Dict[str, Dict]:
+        return {
+            f"effect_of_{self.risk.name}_on_{self.target.name}": {
+                self.target.measure: RiskEffect.configuration_defaults[
+                    "effect_of_risk_on_target"
+                ]["measure"]
+            }
+        }
+
+    ##############
+    # Properties #
+    ##############
+
+    @property
+    def name(self) -> str:
+        return f"risk_effect.{self.risk}.{self.target}"
+
+    #################
+    # Setup methods #
+    #################
+
+    # noinspection PyAttributeOutsideInit
+    def setup(self, builder: Builder) -> None:
+        self.exposure_distribution_type = self._get_distribution_type(builder)
+        self.exposure = self._get_risk_exposure(builder)
+        self.relative_risk = self._get_relative_risk_source(builder)
+        self.population_attributable_fraction = (
+            self._get_population_attributable_fraction_source(builder)
+        )
+
+        self.target_modifier = self._get_target_modifier(builder)
+
+        self._register_target_modifier(builder)
+        self._register_paf_modifier(builder)
+
+    def _get_distribution_type(self, builder: Builder) -> str:
+        return get_distribution_type(builder, self.risk)
+
+    def _get_risk_exposure(self, builder: Builder) -> Callable[[pd.Index], pd.Series]:
+        return builder.value.get_value(self.exposure_pipeline_name)
+
+    def _get_relative_risk_source(self, builder: Builder) -> LookupTable:
+        relative_risk_data = get_relative_risk_data(builder, self.risk, self.target)
+        return builder.lookup.build_table(
+            relative_risk_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+
+    def _get_population_attributable_fraction_source(self, builder: Builder) -> LookupTable:
+        paf_data = get_population_attributable_fraction_data(builder, self.risk, self.target)
+        return builder.lookup.build_table(
+            paf_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+
+    def _get_target_modifier(
+        self, builder: Builder
+    ) -> Callable[[pd.Index, pd.Series], pd.Series]:
+        if self.exposure_distribution_type in ["normal", "lognormal", "ensemble"]:
+            tmred = builder.data.load(f"{self.risk}.tmred")
+            tmrel = 0.5 * (tmred["min"] + tmred["max"])
+            scale = builder.data.load(f"{self.risk}.relative_risk_scalar")
+
+            def adjust_target(index: pd.Index, target: pd.Series) -> pd.Series:
+                rr = self.relative_risk(index)
+                exposure = self.exposure(index)
+                relative_risk = np.maximum(rr.values ** ((exposure - tmrel) / scale), 1)
+                return target * relative_risk
 
-class SimulationDistribution:
-    def __init__(self, mean, sd, distribution=None):
-        self.distribution = distribution
-        self._parameters = self._get_parameters(mean, sd)
-
-    def setup(self, builder):
-        self.parameters = builder.lookup.build_table(self._parameters)
-
-    def _get_parameters(self, mean, sd):
-        index = ['sex', 'age_group_start', 'age_group_end', 'year_start', 'year_end']
-        mean = mean.set_index(index)['value']
-        sd = sd.set_index(index)['value']
-        return self.distribution.get_params(mean, sd).reset_index()
-
-    def ppf(self, q):
-        if not q.empty:
-            x = self.distribution(params=self.parameters(q.index)).ppf(q)
-            x[x.x.isnull()] = 0
         else:
-            x = pd.Series([])
-        return x
-
+            index_columns = ["index", self.risk.name]
 
-class PolytomousDistribution:
-    def __init__(self, risk: str, exposure_data: pd.DataFrame):
-        self.risk = risk
-        self.exposure_data = exposure_data
-        self.categories = sorted([column for column in self.exposure_data if 'cat' in column],
-                                 key=lambda column: int(column[3:]))
-
-    def setup(self, builder):
-        self.exposure = builder.value.register_value_producer(f'{self.risk}.exposure_parameters',
-                                                              source=builder.lookup.build_table(self.exposure_data))
-
-    def ppf(self, x):
-        exposure = self.exposure(x.index)
-        sorted_exposures = exposure[self.categories]
-        if not np.allclose(1, np.sum(sorted_exposures, axis=1)):
-            raise MissingDataError('All exposure data returned as 0.')
-        exposure_sum = sorted_exposures.cumsum(axis='columns')
-        category_index = (exposure_sum.T < x).T.sum('columns')
-        return pd.Series(np.array(self.categories)[category_index], name=self.risk + '_exposure', index=x.index)
-
-
-class DichotomousDistribution:
-    def __init__(self, risk: str, exposure_data: pd.DataFrame):
-        self.risk = risk
-        self.exposure_data = exposure_data.drop('cat2', axis=1)
-
-    def setup(self, builder):
-        self._base_exposure = builder.lookup.build_table(self.exposure_data)
-        self.exposure_proportion = builder.value.register_value_producer(f'{self.risk}.exposure_parameters',
-                                                                         source=self.exposure)
-        self.joint_paf = builder.value.register_value_producer(f'{self.risk}.exposure_parameters.paf',
-                                                               source=lambda index: [builder.lookup.build_table(0)(index)],
-                                                               preferred_combiner=list_combiner,
-                                                               preferred_post_processor=joint_value_post_processor)
-
-    def exposure(self, index):
-        base_exposure = self._base_exposure(index).values
-        joint_paf = self.joint_paf(index).values
-        return pd.Series(base_exposure * (1-joint_paf), index=index, name='values')
-
-    def ppf(self, x):
-        exposed = x < self.exposure_proportion(x.index)
-        return pd.Series(exposed.replace({True: 'cat1', False: 'cat2'}), name=self.risk + '_exposure', index=x.index)
-
-
-def get_distribution(risk, distribution_type, exposure, exposure_standard_deviation, weights):
-    if distribution_type == 'dichotomous':
-        distribution = DichotomousDistribution(risk, exposure)
-    elif 'polytomous' in distribution_type:
-        distribution = PolytomousDistribution(risk, exposure)
-    elif distribution_type == 'normal':
-        distribution = SimulationDistribution(mean=exposure, sd=exposure_standard_deviation,
-                                              distribution=Normal)
-    elif distribution_type == 'lognormal':
-        distribution = SimulationDistribution(mean=exposure, sd=exposure_standard_deviation,
-                                              distribution=LogNormal)
-    elif distribution_type == 'ensemble':
-        distribution = EnsembleSimulation(weights, mean=exposure, sd=exposure_standard_deviation,)
-    else:
-        raise NotImplementedError(f"Unhandled distribution type {distribution_type}")
-    return distribution
+            def adjust_target(index: pd.Index, target: pd.Series) -> pd.Series:
+                rr = self.relative_risk(index)
+                exposure = self.exposure(index).reset_index()
+                exposure.columns = index_columns
+                exposure = exposure.set_index(index_columns)
+
+                relative_risk = rr.stack().reset_index()
+                relative_risk.columns = index_columns + ["value"]
+                relative_risk = relative_risk.set_index(index_columns)
+
+                effect = relative_risk.loc[exposure.index, "value"].droplevel(self.risk.name)
+                affected_rates = target * effect
+                return affected_rates
+
+        return adjust_target
+
+    def _register_target_modifier(self, builder: Builder) -> None:
+        builder.value.register_value_modifier(
+            self.target_pipeline_name,
+            modifier=self.target_modifier,
+            requires_values=[f"{self.risk.name}.exposure"],
+            requires_columns=["age", "sex"],
+        )
+
+    def _register_paf_modifier(self, builder: Builder) -> None:
+        builder.value.register_value_modifier(
+            self.target_paf_pipeline_name,
+            modifier=self.population_attributable_fraction,
+            requires_columns=["age", "sex"],
+        )
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/delay.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/disease.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,330 +1,383 @@
-"""Provide components to represent delayed effects."""
+"""
+==============
+Disease Models
+==============
+
+This module contains tools for modeling diseases in multi-state lifetable
+simulations.
+
+"""
+import numpy as np
 import pandas as pd
 
 
-class DelayedRisk:
+class AcuteDisease:
     """
-    A delayed risk represents an exposure whose impact takes time to come into
-    effect (e.g., smoking uptake and cessation).
+    An acute disease has a sufficiently short duration, relative to the
+    time-step size, that it is not meaningful to talk about prevalence.
+    Instead, it simply contributes an excess mortality rate, and/or a
+    disability rate.
+
+    Interventions may affect these rates:
+
+    - `<disease>_intervention.excess_mortality`
+    - `<disease>_intervention.yld_rate`
+
+    where `<disease>` is the name as provided to the constructor.
+
+    Parameters
+    ----------
+    name
+        The disease name (referred to as `<disease>` here).
 
-    The data required by this component are:
+    """
 
-    - Initial prevalence: the initial level of exposure and post-exposure.
-    - Incidence rate: the rate at which people begin to be exposed;
+    def __init__(self, name):
+        self._name = name
 
-      - This should be specified separately for the BAU and the intervention
-        scenario.
-
-    - Remission rate: the rate at which people stop being exposed;
-
-      - This should be specified separately for the BAU and the intervention
-        scenario.
-
-    - Relative risk of mortality for:
-
-      - Currently exposed (e.g., currently smoking); and
-      - Post-exposure (e.g., stopped smoking :math:`0..N` years ago).
-
-    - Disease-specific relative risks for:
-
-      - Currently exposed (e.g., currently smoking); and
-      - Post-exposure (e.g., stopped smoking :math:`0..N` years ago).
-
-    .. note:: The relative risks are defined in relation to the pre-exposure
-       group (whose relative risks are therefore defined to be :math:`1`).
-
-    Identify the disease(s) for which this delayed risk will have an effect in
-    the simulation configuration. For example, to modify the incidence of CHD
-    and stroke, this would look like:
-
-    .. code-block:: yaml
-
-       components:
-           mslt_port:
-               population:
-                   - BasePopulation()
-                   - Mortality()
-                   - Disability()
-               disease:
-                   - Disease('chd')
-                   - Disease('stroke')
-               delay:
-                   - DelayedRisk('tobacco')
-               ...
-       configuration:
-           tobacco:
-               affects:
-                   # This is where the affected diseases should be listed.
-                   stroke:
-    """
+    @property
+    def name(self):
+        return self._name
 
-    def __init__(self, name, bin_years=20):
+    def setup(self, builder):
+        """Load the morbidity and mortality data."""
+        mty_data = builder.data.load(f"acute_disease.{self.name}.mortality")
+        mty_rate = builder.lookup.build_table(
+            mty_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        yld_data = builder.data.load(f"acute_disease.{self.name}.morbidity")
+        yld_rate = builder.lookup.build_table(
+            yld_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.excess_mortality = builder.value.register_rate_producer(
+            f"{self.name}.excess_mortality", source=mty_rate
+        )
+        self.int_excess_mortality = builder.value.register_rate_producer(
+            f"{self.name}_intervention.excess_mortality", source=mty_rate
+        )
+        self.disability_rate = builder.value.register_rate_producer(
+            f"{self.name}.yld_rate", source=yld_rate
+        )
+        self.int_disability_rate = builder.value.register_rate_producer(
+            f"{self.name}_intervention.yld_rate", source=yld_rate
+        )
+        builder.value.register_value_modifier("mortality_rate", self.mortality_adjustment)
+        builder.value.register_value_modifier("yld_rate", self.disability_adjustment)
+
+    def mortality_adjustment(self, index, mortality_rate):
         """
-        :param name: The name of the exposure (e.g., ``"tobacco"``).
-        :param bin_years: The number of years over which the risk changes
-            (default: 20).
+        Adjust the all-cause mortality rate in the intervention scenario, to
+        account for any change in prevalence (relative to the BAU scenario).
         """
-        self.name = name
-        self.bin_years = bin_years
+        delta = self.int_excess_mortality(index) - self.excess_mortality(index)
+        return mortality_rate + delta
 
-    def setup(self, builder):
+    def disability_adjustment(self, index, yld_rate):
         """
-        Configure the delayed risk component.
-
-        This involves loading the required data tables, registering event
-        handlers and rate modifiers, and setting up the population view.
+        Adjust the years lost due to disability (YLD) rate in the intervention
+        scenario, to account for any change in prevalence (relative to the BAU
+        scenario).
         """
-        self.config = builder.configuration
+        delta = self.int_disability_rate(index) - self.disability_rate(index)
+        return yld_rate + delta
 
-        # Read in the delay duration from the configuration, if present.
-        if 'delay' in self.config[self.name]:
-            self.bin_years = int(self.config[self.name]['delay'])
-
-        # Load the initial prevalence.
-        prev_data = builder.data.load(f'risk_factor.{self.name}.prevalence')
-        self.initial_prevalence = builder.lookup.build_table(prev_data)
-
-        # Load the incidence rates for the BAU and intervention scenarios.
-        inc_data = builder.lookup.build_table(
-            builder.data.load(f'risk_factor.{self.name}.incidence')
-        )
-        inc_name = '{}.incidence'.format(self.name)
-        inc_int_name = '{}_intervention.incidence'.format(self.name)
-        self.incidence = builder.value.register_rate_producer(inc_name, source=inc_data)
-        self.int_incidence = builder.value.register_rate_producer(inc_int_name, source=inc_data)
-
-        # Load the remission rates for the BAU and intervention scenarios.
-        rem_data = builder.lookup.build_table(
-            builder.data.load(f'risk_factor.{self.name}.remission')
-        )
-        rem_name = '{}.remission'.format(self.name)
-        rem_int_name = '{}_intervention.remission'.format(self.name)
-        self.remission = builder.value.register_rate_producer(rem_name, source=rem_data)
-        self.int_remission = builder.value.register_rate_producer(rem_int_name, source=rem_data)
-
-        # We apply separate mortality rates to the different exposure bins.
-        # This requires having access to the life table mortality rate, and
-        # also the relative risks associated with each bin.
-        self.acm_rate = builder.value.get_value('mortality_rate')
-        mort_rr_data = builder.data.load(f'risk_factor.{self.name}.mortality_relative_risk')
-        self.mortality_rr = builder.lookup.build_table(mort_rr_data)
-
-        # Register a modifier for each disease affected by this delayed risk.
-        diseases = self.config[self.name].affects.keys()
-        for ix, disease in enumerate(diseases):
-            self.register_modifier(builder, disease)
-
-        # Load the disease-specific relative risks for each exposure bin.
-        dis_rr_data = builder.data.load(f'risk_factor.{self.name}.disease_relative_risk')
-        key_columns = ['age', 'sex', 'year']
-        self.dis_rr = {}
-        for disease in diseases:
-            dis_columns = [c for c in dis_rr_data.columns
-                           if c.startswith(disease)]
-            dis_keys = [c for c in dis_rr_data.columns
-                        if c in key_columns]
-            if not dis_columns or not dis_keys:
-                msg = 'No {} relative risks for disease {}'
-                raise ValueError(msg.format(self.name, disease))
-            rr_data = dis_rr_data.loc[:, dis_keys + dis_columns]
-            dis_prefix = '{}_'.format(disease)
-            bau_prefix = '{}.'.format(self.name)
-            int_prefix = '{}_intervention.'.format(self.name)
-            bau_col = {c: c.replace(dis_prefix, bau_prefix).replace('post_', '')
-                       for c in dis_columns}
-            int_col = {c: c.replace(dis_prefix, int_prefix).replace('post_', '')
-                       for c in dis_columns}
-            for column in dis_columns:
-                # NOTE: avoid SettingWithCopyWarning
-                rr_data.loc[:, int_col[column]] = rr_data[column]
-            rr_data = rr_data.rename(columns=bau_col)
-            self.dis_rr[disease] = builder.lookup.build_table(rr_data)
-
-        # Add a handler to create the exposure bin columns.
-        req_columns = ['age', 'sex', 'population']
-        new_columns = self.get_bin_names()
-        builder.population.initializes_simulants(
-            self.on_initialize_simulants,
-            creates_columns=new_columns,
-            requires_columns=req_columns)
 
-        # Add a handler to move people from one bin to the next.
-        builder.event.register_listener('time_step__prepare',
-                                        self.on_time_step_prepare)
-
-        # Define the columns that we need to access during the simulation.
-        view_columns = req_columns + new_columns
-        self.population_view = builder.population.get_view(view_columns)
+class Disease:
+    """This component characterises a chronic disease.
 
-    def get_bin_names(self):
-        """
-        Return the bin names for both the BAU and the intervention scenario.
+    It defines the following rates, which may be affected by interventions:
 
-        These names take the following forms:
+    - `<disease>_intervention.incidence`
+    - `<disease>_intervention.remission`
+    - `<disease>_intervention.mortality`
+    - `<disease>_intervention.morbidity`
 
-        - ``"name.no"``: The number of people who have never been exposed.
-        - ``"name.yes"``: The number of people currently exposed.
-        - ``"name.N"``: The number of people N years post-exposure.
+    where `<disease>` is the name as provided to the constructor.
 
-          - The final bin is the number of people :math:`\ge N` years
-            post-exposure.
+    Parameters
+    ----------
+    name
+        The disease name (referred to as `<disease>` here).
 
-        The intervention bin names take the form ``"name_intervention.X"``.
-        """
-        if self.bin_years == 0:
-            delay_bins = [str(0)]
-        else:
-            delay_bins = [str(s) for s in range(self.bin_years + 2)]
-        bins = ['no', 'yes'] + delay_bins
-        bau_bins = ['{}.{}'.format(self.name, bin) for bin in bins]
-        int_bins = ['{}_intervention.{}'.format(self.name, bin) for bin in bins]
-        all_bins = bau_bins + int_bins
-        return all_bins
+    """
+
+    def __init__(self, name):
+        self._name = name
+        self.configuration_defaults = {
+            self.name: {
+                "simplified_no_remission_equations": False,
+            },
+        }
+
+    @property
+    def name(self):
+        return self._name
+
+    def setup(self, builder):
+        """Load the disease prevalence and rates data."""
+        data_prefix = "chronic_disease.{}.".format(self.name)
+        bau_prefix = self.name + "."
+        int_prefix = self.name + "_intervention."
+
+        self.clock = builder.time.clock()
+        self.start_year = builder.configuration.time.start.year
+        self.simplified_equations = builder.configuration[
+            self.name
+        ].simplified_no_remission_equations
+
+        inc_data = builder.data.load(data_prefix + "incidence")
+        i = builder.lookup.build_table(
+            inc_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.incidence = builder.value.register_rate_producer(
+            bau_prefix + "incidence", source=i
+        )
+        self.incidence_intervention = builder.value.register_rate_producer(
+            int_prefix + "incidence", source=i
+        )
+
+        rem_data = builder.data.load(data_prefix + "remission")
+        r = builder.lookup.build_table(
+            rem_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.remission = builder.value.register_rate_producer(
+            bau_prefix + "remission", source=r
+        )
+
+        mty_data = builder.data.load(data_prefix + "mortality")
+        f = builder.lookup.build_table(
+            mty_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.excess_mortality = builder.value.register_rate_producer(
+            bau_prefix + "excess_mortality", source=f
+        )
+
+        yld_data = builder.data.load(data_prefix + "morbidity")
+        yld_rate = builder.lookup.build_table(
+            yld_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.disability_rate = builder.value.register_rate_producer(
+            bau_prefix + "yld_rate", source=yld_rate
+        )
+
+        prev_data = builder.data.load(data_prefix + "prevalence")
+        self.initial_prevalence = builder.lookup.build_table(
+            prev_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+
+        builder.value.register_value_modifier("mortality_rate", self.mortality_adjustment)
+        builder.value.register_value_modifier("yld_rate", self.disability_adjustment)
+
+        columns = []
+        for scenario in ["", "_intervention"]:
+            for rate in ["_S", "_C"]:
+                for when in ["", "_previous"]:
+                    columns.append(self.name + rate + scenario + when)
+
+        builder.population.initializes_simulants(
+            self.on_initialize_simulants,
+            creates_columns=columns,
+            requires_columns=["age", "sex"],
+        )
+        self.population_view = builder.population.get_view(columns)
+
+        builder.event.register_listener("time_step__prepare", self.on_time_step_prepare)
 
     def on_initialize_simulants(self, pop_data):
-        """
-        Define the initial distribution of the population across the bins, in
-        both the BAU and the intervention scenario.
-        """
-        # Set all bins to zero, in order to create the required columns.
-        pop = pd.DataFrame({}, index=pop_data.index)
-        for column in self.get_bin_names():
-            pop[column] = 0
+        """Initialize the test population for which this disease is modeled."""
+        C = 1000 * self.initial_prevalence(pop_data.index)
+        S = 1000 - C
+
+        pop = pd.DataFrame(
+            {
+                f"{self.name}_S": S,
+                f"{self.name}_C": C,
+                f"{self.name}_S_previous": S,
+                f"{self.name}_C_previous": C,
+                f"{self.name}_S_intervention": S,
+                f"{self.name}_C_intervention": C,
+                f"{self.name}_S_intervention_previous": S,
+                f"{self.name}_C_intervention_previous": C,
+            },
+            index=pop_data.index,
+        )
 
-        # Update the life table, so that we can then obtain a view that
-        # includes the population counts.
         self.population_view.update(pop)
-        pop = self.population_view.get(pop_data.index)
-
-        # Calculate the absolute prevalence by multiplying the fractional
-        # prevalence by the population size for each cohort.
-        prev = self.initial_prevalence(pop_data.index).mul(pop['population'], axis=0)
-        self.population_view.update(prev)
-
-        # Rename the columns and apply the same initial prevalence for the
-        # intervention.
-        bau_prefix = '{}.'.format(self.name)
-        int_prefix = '{}_intervention.'.format(self.name)
-        rename_to = {c: c.replace(bau_prefix, int_prefix)
-                     for c in prev.columns if c.startswith(bau_prefix)}
-        int_prev = prev.rename(columns=rename_to)
-        self.population_view.update(int_prev)
 
     def on_time_step_prepare(self, event):
         """
-        Account for transitions between bins, and for mortality rates.
+        Update the disease status for both the BAU and intervention scenarios.
+        """
+        # Do not update the disease status in the first year, the initial data
+        # describe the disease state at the end of the year.
+        if self.clock().year == self.start_year:
+            return
+        pop = self.population_view.get(event.index)
+        if pop.empty:
+            return
+        idx = pop.index
+        S_bau, C_bau = pop[f"{self.name}_S"], pop[f"{self.name}_C"]
+        S_int = pop[f"{self.name}_S_intervention"]
+        C_int = pop[f"{self.name}_C_intervention"]
+
+        # Extract all of the required rates *once only*.
+        i_bau = self.incidence(idx)
+        i_int = self.incidence_intervention(idx)
+        r = self.remission(idx)
+        f = self.excess_mortality(idx)
+
+        # NOTE: if the remission rate is always zero, which is the case for a
+        # number of chronic diseases, we can make some simplifications.
+        if np.all(r == 0):
+            r = 0
+            if self.simplified_equations:
+                # NOTE: for the 'mslt_reduce_chd' experiment, this results in a
+                # slightly lower HALY gain than that obtained when using the
+                # full equations (below).
+                new_S_bau = S_bau * np.exp(-i_bau)
+                new_S_int = S_int * np.exp(-i_int)
+                new_C_bau = C_bau * np.exp(-f) + S_bau - new_S_bau
+                new_C_int = C_int * np.exp(-f) + S_int - new_S_int
+                pop_update = pd.DataFrame(
+                    {
+                        f"{self.name}_S": new_S_bau,
+                        f"{self.name}_C": new_C_bau,
+                        f"{self.name}_S_previous": S_bau,
+                        f"{self.name}_C_previous": C_bau,
+                        f"{self.name}_S_intervention": new_S_int,
+                        f"{self.name}_C_intervention": new_C_int,
+                        f"{self.name}_S_intervention_previous": S_int,
+                        f"{self.name}_C_intervention_previous": C_int,
+                    },
+                    index=pop.index,
+                )
+                self.population_view.update(pop_update)
+                return
+
+        # Calculate common factors.
+        i_bau2 = i_bau**2
+        i_int2 = i_int**2
+        r2 = r**2
+        f2 = f**2
+        f_r = f * r
+        i_bau_r = i_bau * r
+        i_int_r = i_int * r
+        i_bau_f = i_bau * f
+        i_int_f = i_int * f
+        f_plus_r = f + r
+
+        # Calculate convenience terms.
+        l_bau = i_bau + f_plus_r
+        l_int = i_int + f_plus_r
+        q_bau = np.sqrt(i_bau2 + r2 + f2 + 2 * i_bau_r + 2 * f_r - 2 * i_bau_f)
+        q_int = np.sqrt(i_int2 + r2 + f2 + 2 * i_int_r + 2 * f_r - 2 * i_int_f)
+        w_bau = np.exp(-(l_bau + q_bau) / 2)
+        w_int = np.exp(-(l_int + q_int) / 2)
+        v_bau = np.exp(-(l_bau - q_bau) / 2)
+        v_int = np.exp(-(l_int - q_int) / 2)
+
+        # Identify where the denominators are non-zero.
+        nz_bau = q_bau != 0
+        nz_int = q_int != 0
+        denom_bau = 2 * q_bau
+        denom_int = 2 * q_int
+
+        new_S_bau = S_bau.copy()
+        new_C_bau = C_bau.copy()
+        new_S_int = S_int.copy()
+        new_C_int = C_int.copy()
+
+        # Calculate new_S_bau, new_C_bau, new_S_int, new_C_int.
+        num_S_bau = 2 * (v_bau - w_bau) * (S_bau * f_plus_r + C_bau * r) + S_bau * (
+            v_bau * (q_bau - l_bau) + w_bau * (q_bau + l_bau)
+        )
+        num_S_int = 2 * (v_int - w_int) * (S_int * f_plus_r + C_int * r) + S_int * (
+            v_int * (q_int - l_int) + w_int * (q_int + l_int)
+        )
+        new_S_bau[nz_bau] = num_S_bau[nz_bau] / denom_bau[nz_bau]
+        new_S_int[nz_int] = num_S_int[nz_int] / denom_int[nz_int]
 
-        These transitions include:
+        num_C_bau = -(
+            (v_bau - w_bau)
+            * (2 * (f_plus_r * (S_bau + C_bau) - l_bau * S_bau) - l_bau * C_bau)
+            - (v_bau + w_bau) * q_bau * C_bau
+        )
+        num_C_int = -(
+            (v_int - w_int)
+            * (2 * (f_plus_r * (S_int + C_int) - l_int * S_int) - l_int * C_int)
+            - (v_int + w_int) * q_int * C_int
+        )
+        new_C_bau[nz_bau] = num_C_bau[nz_bau] / denom_bau[nz_bau]
+        new_C_int[nz_int] = num_C_int[nz_int] / denom_int[nz_int]
+
+        pop_update = pd.DataFrame(
+            {
+                f"{self.name}_S": new_S_bau,
+                f"{self.name}_C": new_C_bau,
+                f"{self.name}_S_previous": S_bau,
+                f"{self.name}_C_previous": C_bau,
+                f"{self.name}_S_intervention": new_S_int,
+                f"{self.name}_C_intervention": new_C_int,
+                f"{self.name}_S_intervention_previous": S_int,
+                f"{self.name}_C_intervention_previous": C_int,
+            },
+            index=pop.index,
+        )
+        self.population_view.update(pop_update)
 
-        - New exposures;
-        - Cessation of exposure; and
-        - Increased duration of time since exposure.
+    def mortality_adjustment(self, index, mortality_rate):
         """
-        idx = event.index
-        pop = self.population_view.get(idx)
-        acmr = self.acm_rate(idx)
-        inc_rate = self.incidence(idx)
-        rem_rate = self.remission(idx)
-        int_inc_rate = self.int_incidence(idx)
-        int_rem_rate = self.int_remission(idx)
-
-        # Calculate the survival rate for each bin.
-        pop = self.population_view.get(idx)
-        bin_cols = self.get_bin_names()
-        base_surv_rate = (1 - acmr)
-        surv_rate = self.mortality_rr(idx).rpow(base_surv_rate, axis=0)
-
-        # Account for mortality in each bin.
-        pop[bin_cols] = pop[bin_cols].mul(surv_rate[bin_cols])
-
-        # Account for transitions between bins.
-        # Note that the order of evaluation matters.
-        suffixes = ['', '_intervention']
-        # First, accumulate the final post-exposure bin.
-        if self.bin_years > 0:
-            for suffix in suffixes:
-                accum_col = '{}{}.{}'.format(self.name, suffix, self.bin_years + 1)
-                from_col = '{}{}.{}'.format(self.name, suffix, self.bin_years)
-                pop[accum_col] += pop[from_col]
-        # Then increase time since exposure for all other post-exposure bins.
-        for n_years in reversed(range(self.bin_years)):
-            for suffix in suffixes:
-                source_col = '{}{}.{}'.format(self.name, suffix, n_years)
-                dest_col = '{}{}.{}'.format(self.name, suffix, n_years + 1)
-                pop[dest_col] = pop[source_col]
-
-        # Account for incidence and remission.
-        col_no = '{}.no'.format(self.name)
-        col_int_no = '{}_intervention.no'.format(self.name)
-        col_yes = '{}.yes'.format(self.name)
-        col_int_yes = '{}_intervention.yes'.format(self.name)
-        col_zero = '{}.0'.format(self.name)
-        col_int_zero = '{}_intervention.0'.format(self.name)
-
-        inc = inc_rate * pop[col_no]
-        int_inc = int_inc_rate * pop[col_int_no]
-        rem = rem_rate * pop[col_yes]
-        int_rem = int_rem_rate * pop[col_int_yes]
-        pop[col_no] = pop[col_no] - inc
-        pop[col_int_no] = pop[col_int_no] - int_inc
-        pop[col_yes] = pop[col_yes] + inc - rem
-        pop[col_int_yes] = pop[col_int_yes] + int_inc - int_rem
-        pop[col_zero] = rem
-        pop[col_int_zero] = int_rem
+        Adjust the all-cause mortality rate in the intervention scenario, to
+        account for any change in disease prevalence (relative to the BAU
+        scenario).
+        """
+        pop = self.population_view.get(index)
 
-        self.population_view.update(pop)
+        S, C = pop[f"{self.name}_S"], pop[f"{self.name}_C"]
+        S_prev, C_prev = pop[f"{self.name}_S_previous"], pop[f"{self.name}_C_previous"]
+        D, D_prev = 1000 - S - C, 1000 - S_prev - C_prev
+
+        S_int, C_int = pop[f"{self.name}_S_intervention"], pop[f"{self.name}_C_intervention"]
+        S_int_prev, C_int_prev = (
+            pop[f"{self.name}_S_intervention_previous"],
+            pop[f"{self.name}_C_intervention_previous"],
+        )
+        D_int, D_int_prev = 1000 - S_int - C_int, 1000 - S_int_prev - C_int_prev
 
-    def register_modifier(self, builder, disease):
-        """
-        Register that a disease incidence rate will be modified by this
-        delayed risk in the intervention scenario.
+        # NOTE: as per the spreadsheet, the denominator is from the same point
+        # in time as the term being subtracted in the numerator.
+        mortality_risk = (D - D_prev) / (S_prev + C_prev)
+        mortality_risk_int = (D_int - D_int_prev) / (S_int_prev + C_int_prev)
 
-        :param builder: The builder object for the simulation, which provides
-            access to event handlers and rate modifiers.
-        :param disease: The name of the disease whose incidence rate will be
-            modified.
-        """
-        # NOTE: we need to modify different rates for chronic and acute
-        # diseases. For now, register modifiers for all possible rates.
-        rate_templates = ['{}_intervention.incidence',
-                          '{}_intervention.excess_mortality',
-                          '{}_intervention.yld_rate']
-        for template in rate_templates:
-            rate_name = template.format(disease)
-            modifier = lambda ix, rate: self.incidence_adjustment(disease, ix, rate)
-            builder.value.register_value_modifier(rate_name, modifier)
+        delta = np.log((1 - mortality_risk) / (1 - mortality_risk_int))
 
-    def incidence_adjustment(self, disease, index, incidence_rate):
-        """
-        Modify a disease incidence rate in the intervention scenario.
+        return mortality_rate + delta
 
-        :param disease: The name of the disease.
-        :param index: The index into the population life table.
-        :param incidence_rate: The un-adjusted disease incidence rate.
+    def disability_adjustment(self, index, yld_rate):
+        """
+        Adjust the years lost due to disability (YLD) rate in the intervention
+        scenario, to account for any change in disease prevalence (relative to
+        the BAU scenario).
         """
-        # Multiply the population in each bin by the associated relative risk.
-        bin_cols = self.get_bin_names()
-        incidence_rr = self.dis_rr[disease](index)[bin_cols]
         pop = self.population_view.get(index)
-        rr_values = pop[bin_cols] * incidence_rr
 
-        # Calculate the mean relative-risk for the BAU scenario.
-        bau_prefix = '{}.'.format(self.name)
-        bau_cols = [c for c in bin_cols if c.startswith(bau_prefix)]
-        # Sum over all of the bins in each row.
-        mean_bau_rr = rr_values[bau_cols].sum(axis=1) / pop[bau_cols].sum(axis=1)
-        # Handle cases where the population size is zero.
-        mean_bau_rr = mean_bau_rr.fillna(1.0)
-
-        # Calculate the mean relative-risk for the intervention scenario.
-        int_prefix = '{}_intervention.'.format(self.name)
-        int_cols = [c for c in bin_cols if c.startswith(int_prefix)]
-        # Sum over all of the bins in each row.
-        mean_int_rr = rr_values[int_cols].sum(axis=1) / pop[int_cols].sum(axis=1)
-        # Handle cases where the population size is zero.
-        mean_int_rr = mean_int_rr.fillna(1.0)
-
-        # Calculate the disease incidence PIF for the intervention scenario.
-        pif = (mean_bau_rr - mean_int_rr) / mean_bau_rr
-        pif = pif.fillna(0.0)
-        return incidence_rate * (1 - pif)
+        S, S_prev = pop[f"{self.name}_S"], pop[f"{self.name}_S_previous"]
+        C, C_prev = pop[f"{self.name}_C"], pop[f"{self.name}_C_previous"]
+        S_int, S_int_prev = (
+            pop[f"{self.name}_S_intervention"],
+            pop[f"{self.name}_S_intervention_previous"],
+        )
+        C_int, C_int_prev = (
+            pop[f"{self.name}_C_intervention"],
+            pop[f"{self.name}_C_intervention_previous"],
+        )
+
+        # The prevalence rate is the mean number of diseased people over the
+        # year, divided by the mean number of alive people over the year.
+        # The 0.5 multipliers in the numerator and denominator therefore cancel
+        # each other out, and can be removed.
+        prevalence_rate = (C + C_prev) / (S + C + S_prev + C_prev)
+        prevalence_rate_int = (C_int + C_int_prev) / (S_int + C_int + S_int_prev + C_int_prev)
+
+        delta = prevalence_rate_int - prevalence_rate
+        return yld_rate + self.disability_rate(index) * delta
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/observer.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/mslt/observer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,308 +1,392 @@
-"""This module provides classes that record various outputs of interest."""
+"""
+=========
+Observers
+=========
 
-import numpy as np
+This module contains tools for recording various outputs of interest in
+multi-state lifetable simulations.
+
+"""
 import pandas as pd
-import itertools
+
+
+def output_file(config, suffix, sep="_", ext="csv"):
+    """
+    Determine the output file name for an observer, based on the prefix
+    defined in ``config.observer.output_prefix`` and the (optional)
+    ``config.input_data.input_draw_number``.
+
+    Parameters
+    ----------
+    config
+        The builder configuration object.
+    suffix
+        The observer-specific suffix.
+    sep
+        The separator between prefix, suffix, and draw number.
+    ext
+        The output file extension.
+
+    """
+    if "observer" not in config:
+        raise ValueError("observer.output_prefix not defined")
+    if "output_prefix" not in config.observer:
+        raise ValueError("observer.output_prefix not defined")
+    prefix = config.observer.output_prefix
+    if "input_draw_number" in config.input_data:
+        draw = config.input_data.input_draw_number
+    else:
+        draw = 0
+    out_file = prefix + sep + suffix
+    if draw > 0:
+        out_file += "{}{}".format(sep, draw)
+    out_file += ".{}".format(ext)
+    return out_file
 
 
 class MorbidityMortality:
     """
     This class records the all-cause morbidity and mortality rates for each
     cohort at each year of the simulation.
+
+    Parameters
+    ----------
+    output_suffix
+        The suffix for the CSV file in which to record the
+        morbidity and mortality data.
+
     """
 
-    def __init__(self, output_file):
-        """
-        :param output_file: The name of the CSV file in which to record the
-            morbidity and mortality data.
-        """
-        self.output_file = output_file
+    def __init__(self, output_suffix="mm"):
+        self.output_suffix = output_suffix
+
+    @property
+    def name(self):
+        return "morbidity_mortality_observer"
 
     def setup(self, builder):
-        columns = ['age', 'sex']
+        # Record the key columns from the core multi-state life table.
+        columns = [
+            "age",
+            "sex",
+            "population",
+            "bau_population",
+            "acmr",
+            "bau_acmr",
+            "pr_death",
+            "bau_pr_death",
+            "deaths",
+            "bau_deaths",
+            "yld_rate",
+            "bau_yld_rate",
+            "person_years",
+            "bau_person_years",
+            "HALY",
+            "bau_HALY",
+        ]
         self.population_view = builder.population.get_view(columns)
-        self.yld_rate = builder.value.get_value('yld_rate')
-        self.acm_rate = builder.value.get_value('mortality_rate')
         self.clock = builder.time.clock()
-        builder.event.register_listener('collect_metrics', self.on_collect_metrics)
-        builder.event.register_listener('simulation_end', self.write_output)
+        builder.event.register_listener("collect_metrics", self.on_collect_metrics)
+        builder.event.register_listener("simulation_end", self.write_output)
         self.tables = []
-        self.table_cols = ['sex', 'age', 'year',
-                           'bau_yld_rate', 'bau_mortality_rate',
-                           'int_yld_rate', 'int_mortality_rate']
+        self.table_cols = [
+            "sex",
+            "age",
+            "year",
+            "population",
+            "bau_population",
+            "prev_population",
+            "bau_prev_population",
+            "acmr",
+            "bau_acmr",
+            "pr_death",
+            "bau_pr_death",
+            "deaths",
+            "bau_deaths",
+            "yld_rate",
+            "bau_yld_rate",
+            "person_years",
+            "bau_person_years",
+            "HALY",
+            "bau_HALY",
+        ]
+
+        self.output_file = output_file(builder.configuration, self.output_suffix)
 
     def on_collect_metrics(self, event):
         pop = self.population_view.get(event.index)
         if len(pop.index) == 0:
             # No tracked population remains.
             return
 
-        pop['year'] = self.clock().year
-        pop['bau_yld_rate'] = self.yld_rate.source(event.index)
-        pop['bau_mortality_rate'] = self.acm_rate.source(event.index)
-        pop['int_yld_rate'] = self.yld_rate(event.index)
-        pop['int_mortality_rate'] = self.acm_rate(event.index)
+        pop["year"] = self.clock().year
+        # Record the population size prior to the deaths.
+        pop["prev_population"] = pop["population"] + pop["deaths"]
+        pop["bau_prev_population"] = pop["bau_population"] + pop["bau_deaths"]
         self.tables.append(pop[self.table_cols])
 
+    def calculate_LE(self, table, py_col, denom_col):
+        """Calculate the life expectancy for each cohort at each time-step.
+
+        Parameters
+        ----------
+        table
+            The population life table.
+        py_col
+            The name of the person-years column.
+        denom_col
+            The name of the population denominator column.
+
+        Returns
+        -------
+            The life expectancy for each table row, represented as a
+            pandas.Series object.
+
+        """
+        # Group the person-years by cohort.
+        group_cols = ["year_of_birth", "sex"]
+        subset_cols = group_cols + [py_col]
+        grouped = table.loc[:, subset_cols].groupby(by=group_cols)[py_col]
+        # Calculate the reverse-cumulative sums of the adjusted person-years
+        # (i.e., the present and future person-years) by:
+        #   (a) reversing the adjusted person-years values in each cohort;
+        #   (b) calculating the cumulative sums in each cohort; and
+        #   (c) restoring the original order.
+        cumsum = grouped.apply(lambda x: pd.Series(x[::-1].cumsum()).iloc[::-1])
+        return cumsum / table[denom_col]
+
     def write_output(self, event):
         data = pd.concat(self.tables, ignore_index=True)
-        data['year_of_birth'] = data['year'] - data['age']
+        data["year_of_birth"] = data["year"] - data["age"]
         # Sort the table by cohort (i.e., generation and sex), and then by
         # calendar year, so that results are output in the same order as in
         # the spreadsheet models.
-        data = data.sort_values(by=['year_of_birth', 'sex', 'age'], axis=0)
+        data = data.sort_values(by=["year_of_birth", "sex", "age"], axis=0)
         data = data.reset_index(drop=True)
         # Re-order the table columns.
-        cols = ['year_of_birth'] + self.table_cols
+        cols = ["year_of_birth"] + self.table_cols
         data = data[cols]
+        # Calculate life expectancy and HALE for the BAU and intervention,
+        # with respect to the initial population, not the survivors.
+        data["LE"] = self.calculate_LE(data, "person_years", "prev_population")
+        data["bau_LE"] = self.calculate_LE(data, "bau_person_years", "bau_prev_population")
+        data["HALE"] = self.calculate_LE(data, "HALY", "prev_population")
+        data["bau_HALE"] = self.calculate_LE(data, "bau_HALY", "bau_prev_population")
         data.to_csv(self.output_file, index=False)
 
 
 class Disease:
     """
     This class records the disease incidence rate and disease prevalence for
     each cohort at each year of the simulation.
+
+    Parameters
+    ----------
+    name
+        The name of the chronic disease.
+    output_suffix
+        The suffix for the CSV file in which to record the
+        disease data.
+
     """
 
-    def __init__(self, name, output_file):
-        """
-        :param name: The name of the disease.
-        :param output_file: The name of the CSV file in which to record the
-            disease data.
-        """
-        self.name = name
-        self.output_file = output_file
+    def __init__(self, name, output_suffix=None):
+        self._name = name
+        if output_suffix is None:
+            output_suffix = name.lower()
+        self.output_suffix = output_suffix
+
+    @property
+    def name(self):
+        return f"{self._name}_observer"
 
     def setup(self, builder):
-        bau_incidence_value = '{}.incidence'.format(self.name)
-        int_incidence_value = '{}_intervention.incidence'.format(self.name)
+        bau_incidence_value = "{}.incidence".format(self._name)
+        int_incidence_value = "{}_intervention.incidence".format(self._name)
         self.bau_incidence = builder.value.get_value(bau_incidence_value)
         self.int_incidence = builder.value.get_value(int_incidence_value)
 
-        self.bau_S_col = '{}_S'.format(self.name)
-        self.bau_C_col = '{}_C'.format(self.name)
-        self.int_S_col = '{}_S_intervention'.format(self.name)
-        self.int_C_col = '{}_C_intervention'.format(self.name)
-
-        columns = ['age', 'sex',
-                   self.bau_S_col, self.bau_C_col,
-                   self.int_S_col, self.int_C_col]
+        self.bau_S_col = "{}_S".format(self._name)
+        self.bau_C_col = "{}_C".format(self._name)
+        self.int_S_col = "{}_S_intervention".format(self._name)
+        self.int_C_col = "{}_C_intervention".format(self._name)
+
+        columns = [
+            "age",
+            "sex",
+            self.bau_S_col,
+            self.bau_C_col,
+            self.int_S_col,
+            self.int_C_col,
+        ]
         self.population_view = builder.population.get_view(columns)
 
-        builder.event.register_listener('collect_metrics', self.on_collect_metrics)
-        builder.event.register_listener('simulation_end', self.write_output)
+        builder.event.register_listener("collect_metrics", self.on_collect_metrics)
+        builder.event.register_listener("simulation_end", self.write_output)
 
         self.tables = []
-        self.table_cols = ['sex', 'age', 'year',
-                           'bau_incidence', 'int_incidence',
-                           'bau_prevalence', 'int_prevalence']
+        self.table_cols = [
+            "sex",
+            "age",
+            "year",
+            "bau_incidence",
+            "int_incidence",
+            "bau_prevalence",
+            "int_prevalence",
+            "bau_deaths",
+            "int_deaths",
+        ]
         self.clock = builder.time.clock()
+        self.output_file = output_file(builder.configuration, self.output_suffix)
 
     def on_collect_metrics(self, event):
         pop = self.population_view.get(event.index)
         if len(pop.index) == 0:
             # No tracked population remains.
             return
 
-        pop['year'] = self.clock().year
-        pop['bau_incidence'] = self.bau_incidence(event.index)
-        pop['int_incidence'] = self.int_incidence(event.index)
-        pop['bau_prevalence'] = pop[self.bau_C_col] / (pop[self.bau_C_col] + pop[self.bau_S_col])
-        pop['int_prevalence'] = pop[self.int_C_col] / (pop[self.bau_C_col] + pop[self.bau_S_col])
+        pop["year"] = self.clock().year
+        pop["bau_incidence"] = self.bau_incidence(event.index)
+        pop["int_incidence"] = self.int_incidence(event.index)
+        pop["bau_prevalence"] = pop[self.bau_C_col] / (
+            pop[self.bau_C_col] + pop[self.bau_S_col]
+        )
+        pop["int_prevalence"] = pop[self.int_C_col] / (
+            pop[self.bau_C_col] + pop[self.bau_S_col]
+        )
+        pop["bau_deaths"] = 1000 - pop[self.bau_S_col] - pop[self.bau_C_col]
+        pop["int_deaths"] = 1000 - pop[self.int_S_col] - pop[self.int_C_col]
         self.tables.append(pop.loc[:, self.table_cols])
 
     def write_output(self, event):
         data = pd.concat(self.tables, ignore_index=True)
-        data['diff_incidence'] = data['int_incidence'] - data['bau_incidence']
-        data['diff_prevalence'] = data['int_prevalence'] - data['bau_prevalence']
-        data['year_of_birth'] = data['year'] - data['age']
-        data['disease'] = self.name
+        data["diff_incidence"] = data["int_incidence"] - data["bau_incidence"]
+        data["diff_prevalence"] = data["int_prevalence"] - data["bau_prevalence"]
+        data["year_of_birth"] = data["year"] - data["age"]
+        data["disease"] = self._name
         # Sort the table by cohort (i.e., generation and sex), and then by
         # calendar year, so that results are output in the same order as in
         # the spreadsheet models.
-        data = data.sort_values(by=['year_of_birth', 'sex', 'age'], axis=0)
+        data = data.sort_values(by=["year_of_birth", "sex", "age"], axis=0)
         data = data.reset_index(drop=True)
         # Re-order the table columns.
-        diff_cols = ['diff_incidence', 'diff_prevalence']
-        cols = ['disease', 'year_of_birth'] + self.table_cols + diff_cols
+        diff_cols = ["diff_incidence", "diff_prevalence"]
+        cols = ["disease", "year_of_birth"] + self.table_cols + diff_cols
         data = data[cols]
         data.to_csv(self.output_file, index=False)
 
 
-class AdjustedPYandLE:
-    """
-    This class calculates the adjusted person-years and the adjusted
-    life-expectancy for each cohort at each year of the simulation.
+class TobaccoPrevalence:
+    """This class records the prevalence of tobacco use in the population.
+
+    Parameters
+    ----------
+    output_suffix
+        The suffix for the CSV file in which to record the
+        prevalence data.
+
     """
 
-    def __init__(self, output_file=None, unadjusted=True):
-        """
-        :param output_file: The name of the CSV file in which to record the
-            adjusted person-years and adjusted life-expectancy data.
-        :param unadjusted: Whether to also record unadjusted person-years and
-            life-expectancy data.
-        """
-        self.output_file = output_file
-        self.unadjusted = unadjusted
+    def __init__(self, output_suffix="tobacco"):
+        self.output_suffix = output_suffix
+
+    @property
+    def name(self):
+        return "tobacco_prevalence_observer"
 
     def setup(self, builder):
-        self.age_group_end = builder.configuration.population.max_age
-        self.time_span = builder.configuration.time
-        self.yld_rate = builder.value.get_value('yld_rate')
-        self.acm_rate = builder.value.get_value('mortality_rate')
-        view_cols = ['age', 'sex', 'population', 'bau_population']
-        # TODO: ugly hack, can't extract mortality rate when initialising
-        #       simulants unless the diseases have already been initialised.
-        extra_cols = ['CHD_S']
-        # extra_cols = []
-        req_cols = view_cols + extra_cols
-        builder.population.initializes_simulants(self.on_initialize,
-                                                 requires_columns=req_cols)
-        self.population_view = builder.population.get_view(view_cols)
+        self.config = builder.configuration
         self.clock = builder.time.clock()
-        builder.event.register_listener('collect_metrics', self.on_collect_metrics)
-        builder.event.register_listener('simulation_end', self.finalise_output)
-        self.idx_cols = ['age', 'sex', 'year']
+        self.bin_years = int(self.config["tobacco"]["delay"])
 
-    def create_table(self, min_age, min_year):
-        """
-        Create an empty data frame to hold all of the adjusted person-year and
-        adjusted life-expectancy values that will be produced during a
-        simulation.
-        """
-        ages = range(min_age, self.age_group_end + 1)
-        sexes = ['male', 'female']
-        years = range(min_year, self.time_span.end.year + 1)
-        # NOTE: columns must be in the same order as self.idx_cols.
-        rows = list(itertools.product(ages, sexes, years))
-        self.data = pd.DataFrame(rows, columns=self.idx_cols)
-        self.data.set_index(self.idx_cols)
-        self.data['PYadj'] = np.nan
-        self.data['PY'] = np.nan
-        self.data['population'] = np.nan
-        self.data['bau_PYadj'] = np.nan
-        self.data['bau_PY'] = np.nan
-        self.data['bau_population'] = np.nan
+        view_columns = ["age", "sex", "bau_population", "population"] + self.get_bin_names()
+        self.population_view = builder.population.get_view(view_columns)
 
-    def record_person_years(self, idx):
-        """
-        Record the un-adjusted and adjusted person-years for the BAU and the
-        intervention.
-        """
-        pop = self.population_view.get(idx)
+        self.tables = []
+        self.table_cols = [
+            "age",
+            "sex",
+            "year",
+            "bau_no",
+            "bau_yes",
+            "bau_previously",
+            "bau_population",
+            "int_no",
+            "int_yes",
+            "int_previously",
+            "int_population",
+        ]
+
+        builder.event.register_listener("collect_metrics", self.on_collect_metrics)
+        builder.event.register_listener("simulation_end", self.write_output)
+        self.output_file = output_file(builder.configuration, self.output_suffix)
+
+    def get_bin_names(self):
+        """Return the bin names for both the BAU and the intervention scenario.
+
+        These names take the following forms:
+
+        ``"name.no"``
+            The number of people who have never been exposed.
+        ``"name.yes"``
+            The number of people currently exposed.
+        ``"name.N"``
+            The number of people N years post-exposure.
+
+        The final bin is the number of people :math:`\ge N` years
+        post-exposure.
+
+        The intervention bin names take the form ``"name_intervention.X"``.
+
+        """
+        if self.bin_years == 0:
+            delay_bins = [str(0)]
+        else:
+            delay_bins = [str(s) for s in range(self.bin_years + 2)]
+        bins = ["no", "yes"] + delay_bins
+        bau_bins = ["{}.{}".format("tobacco", bin) for bin in bins]
+        int_bins = ["{}_intervention.{}".format("tobacco", bin) for bin in bins]
+        all_bins = bau_bins + int_bins
+        return all_bins
+
+    def on_collect_metrics(self, event):
+        pop = self.population_view.get(event.index)
         if len(pop.index) == 0:
             # No tracked population remains.
             return
 
-        pop['year'] = self.clock().year
+        bau_cols = [c for c in pop.columns.values if c.startswith("{}.".format("tobacco"))]
+        int_cols = [
+            c
+            for c in pop.columns.values
+            if c.startswith("{}_intervention.".format("tobacco"))
+        ]
+
+        bau_denom = pop.reindex(columns=bau_cols).sum(axis=1)
+        int_denom = pop.reindex(columns=int_cols).sum(axis=1)
+
+        # Normalise prevalence with respect to the total population.
+        pop["bau_no"] = pop["{}.no".format("tobacco")] / bau_denom
+        pop["bau_yes"] = pop["{}.yes".format("tobacco")] / bau_denom
+        pop["bau_previously"] = 1 - pop["bau_no"] - pop["bau_yes"]
+        pop["int_no"] = pop["{}_intervention.no".format("tobacco")] / int_denom
+        pop["int_yes"] = pop["{}_intervention.yes".format("tobacco")] / int_denom
+        pop["int_previously"] = 1 - pop["int_no"] - pop["int_yes"]
 
-        # Calculate (adjusted) person-years for the intervention.
-        int_pr_death = 1 - np.exp(- self.acm_rate(idx))
-        pop['PY'] = pop['population'] * (1 - 0.5 * int_pr_death)
-        pop['PYadj'] = pop['PY'] * (1 - self.yld_rate(idx))
-
-        # Calculate (adjusted) person-years for the BAU.
-        bau_pr_death = 1 - np.exp(- self.acm_rate.source(idx))
-        pop['bau_PY'] = pop['bau_population'] * (1 - 0.5 * bau_pr_death)
-        pop['bau_PYadj'] = pop['bau_PY'] * (1 - self.yld_rate.source(idx))
-
-        # Determine if any strata statistics need to be updated.
-        df = self.data.merge(pop, on=self.idx_cols, how='left',
-                             suffixes=('', '_new'))
-        if len(df.index) == 0:
-            # No strata to update.
-            return
-
-        # Determine which strata to update.
-        new_vals = df['PYadj_new'].notna()
-
-        # Update (adjusted) person-years and population denominators.
-        int_cols = ['PY', 'PYadj', 'population']
-        bau_cols = ['bau_{}'.format(c) for c in int_cols]
-        for col in int_cols + bau_cols:
-            new_col = '{}_new'.format(col)
-            self.data.loc[new_vals, col] = df.loc[new_vals, new_col]
+        pop = pop.rename(columns={"population": "int_population"})
 
-    def on_initialize(self, pop_data):
-        """
-        Calculate adjusted person-years and adjusted life-expectancy before
-        the first time-step.
-        """
-        idx = pop_data.index
-        pop = self.population_view.get(idx)
-        self.create_table(pop['age'].min(), self.clock().year)
-        self.record_person_years(idx)
+        pop["year"] = self.clock().year
+        self.tables.append(pop.reindex(columns=self.table_cols).reset_index(drop=True))
 
-    def on_collect_metrics(self, event):
-        """
-        Calculate adjusted person-years for the current year.
-        """
-        self.record_person_years(event.index)
-
-    def get_table(self):
-        """
-        Return a Pandas data frame that contains the adjusted person-years and
-        adjusted life-expectancy for each cohort at each year of the
-        simulation.
-        """
-        mask = self.data['PYadj'].notna()
-        return self.data.loc[mask].sort_index()
-
-    def to_csv(self, filename):
-        """
-        Save the adjusted person-years and the adjusted life-expectancy data
-        to a CSV file.
-        """
-        self.get_table().to_csv(filename, index=False)
-
-    def calculate_life_expectancy(self, py_col, le_col, denom_col):
-        # Group the person-years by cohort.
-        group_cols = ['year_of_birth', 'sex']
-        subset_cols = group_cols + [py_col]
-        grouped = self.data.loc[:, subset_cols].groupby(by=group_cols)[py_col]
-        # Calculate the reverse-cumulative sums of the adjusted person-years
-        # (i.e., the present and future person-years) by:
-        #   (a) reversing the adjusted person-years values in each cohort;
-        #   (b) calculating the cumulative sums in each cohort; and
-        #   (c) restoring the original order.
-        cumsum = grouped.apply(lambda x: pd.Series(x[::-1].cumsum()).iloc[::-1])
-        self.data[le_col] = cumsum / self.data[denom_col]
-
-    def finalise_output(self, event):
-        """
-        Calculate the adjusted life-expectancy for each cohort at each year of
-        the simulation, now that the simulation has finished and the adjusted
-        person-years for each cohort at each year have been calculated.
-
-        If an output file name was provided to the constructor, this method
-        will also save these data to a CSV file.
-        """
-        # Identify each generation by their year of birth.
-        self.data['year_of_birth'] = self.data['year'] - self.data['age']
+    def write_output(self, event):
+        data = pd.concat(self.tables, ignore_index=True)
+        data["year_of_birth"] = data["year"] - data["age"]
         # Sort the table by cohort (i.e., generation and sex), and then by
         # calendar year, so that results are output in the same order as in
         # the spreadsheet models.
-        self.data = self.data.sort_values(by=['year_of_birth', 'sex', 'age'],
-                                          axis=0)
-        self.data = self.data.reset_index(drop=True)
-        # Calculate (adjusted) life expectancy for BAU and the intervention.
-        self.calculate_life_expectancy('PY', 'LE', 'population')
-        self.calculate_life_expectancy('PYadj', 'LEadj', 'population')
-        self.calculate_life_expectancy('bau_PY', 'bau_LE', 'bau_population')
-        self.calculate_life_expectancy('bau_PYadj', 'bau_LEadj', 'bau_population')
-        # Calculate differences between the BAU and the intervention.
-        self.data['diff_LE'] = self.data['LE'] - self.data['bau_LE']
-        self.data['diff_PY'] = self.data['PY'] - self.data['bau_PY']
-        self.data['diff_LEadj'] = self.data['LEadj'] - self.data['bau_LEadj']
-        self.data['diff_PYadj'] = self.data['PYadj'] - self.data['bau_PYadj']
-        # Re-order the columns to better reflect how the spreadsheet model
-        # tables are arranged.
-        cols = ['year_of_birth', 'sex', 'age', 'year',
-                'population', 'bau_population',
-                'PYadj', 'LEadj', 'bau_PYadj', 'bau_LEadj',
-                'diff_LEadj', 'diff_PYadj']
-        if self.unadjusted:
-            cols.extend(['PY', 'LE', 'bau_PY', 'bau_LE', 'diff_PY', 'diff_LE'])
-        self.data = self.data[cols]
-        if self.output_file is not None:
-            self.to_csv(self.output_file)
+        data = data.sort_values(by=["year_of_birth", "sex", "age"], axis=0)
+        data = data.reset_index(drop=True)
+        # Re-order the table columns.
+        cols = ["year_of_birth"] + self.table_cols
+        data = data.reindex(columns=cols)
+        data.to_csv(self.output_file, index=False)
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/state.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/disease/state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,215 @@
-"""A toolbox for modeling diseases as state machines."""
-import pandas as pd
-import numpy as np
+"""
+==============
+Disease States
+==============
 
-from vivarium.framework.state_machine import State, Transient
-from vivarium.framework.values import list_combiner, joint_value_post_processor
+This module contains tools to manage standard disease states.
 
-from vivarium_public_health.disease import RateTransition, ProportionTransition
+"""
+from typing import Callable, Dict, List
+
+import numpy as np
+import pandas as pd
+from vivarium.framework.population import PopulationView, SimulantData
+from vivarium.framework.state_machine import State, Transient, Transition
+from vivarium.framework.values import list_combiner, union_post_processor
+
+from vivarium_public_health.disease.transition import (
+    ProportionTransition,
+    RateTransition,
+    TransitionString,
+)
+from vivarium_public_health.utilities import is_non_zero
 
 
 class BaseDiseaseState(State):
-    def __init__(self, cause, name_prefix=None, side_effect_function=None, cause_type="cause", **kwargs):
-        self.cause = cause
+    def __init__(
+        self, cause, name_prefix="", side_effect_function=None, cause_type="cause", **kwargs
+    ):
+        super().__init__(name_prefix + cause)  # becomes state_id
         self.cause_type = cause_type
-        cause_name = name_prefix + cause if name_prefix else cause
-        super().__init__(cause_name, **kwargs)
+        self.cause = cause
 
         self.side_effect_function = side_effect_function
+        if self.side_effect_function is not None:
+            self._sub_components.append(side_effect_function)
+
+        self.event_time_column = self.state_id + "_event_time"
+        self.event_count_column = self.state_id + "_event_count"
 
-        self.event_time_column = self.state_id + '_event_time'
-        self.event_count_column = self.state_id + '_event_count'
+    @property
+    def columns_created(self):
+        return [self.event_time_column, self.event_count_column]
 
+    # noinspection PyAttributeOutsideInit
     def setup(self, builder):
         """Performs this component's simulation setup.
 
         Parameters
         ----------
         builder : `engine.Builder`
             Interface to several simulation tools.
         """
         super().setup(builder)
-        if self.side_effect_function is not None:
-            builder.components.add_components([self.side_effect_function])
 
         self.clock = builder.time.clock()
 
-        columns = [self._model, 'alive']
-        columns += [self.event_time_column, self.event_count_column]
+        view_columns = self.columns_created + [self._model, "alive"]
+        self.population_view = builder.population.get_view(view_columns)
+        builder.population.initializes_simulants(
+            self.on_initialize_simulants,
+            creates_columns=self.columns_created,
+            requires_columns=[self._model],
+        )
+
+    def on_initialize_simulants(self, pop_data: SimulantData) -> None:
+        """Adds this state's columns to the simulation state table."""
+        for transition in self.transition_set:
+            if transition.start_active:
+                transition.set_active(pop_data.index)
 
-        self.population_view = builder.population.get_view(columns)
-        builder.population.initializes_simulants(self.load_population_columns,
-                                                 creates_columns=[self.event_time_column, self.event_count_column],
-                                                 requires_columns=[self._model])
+        pop_update = self.get_initial_event_times(pop_data)
+        self.population_view.update(pop_update)
 
-        builder.value.register_value_modifier('metrics', self.metrics)
+    def get_initial_event_times(self, pop_data: SimulantData) -> pd.DataFrame:
+        return pd.DataFrame(
+            {self.event_time_column: pd.NaT, self.event_count_column: 0}, index=pop_data.index
+        )
 
     def _transition_side_effect(self, index, event_time):
-        """Updates the simulation state and triggers any side-effects associated with this state.
+        """Updates the simulation state and triggers any side effects associated with this state.
 
         Parameters
         ----------
-        index : iterable of ints
+        index
             An iterable of integer labels for the simulants.
         event_time : pandas.Timestamp
             The time at which this transition occurs.
-        """
 
+        """
         pop = self.population_view.get(index)
         pop[self.event_time_column] = event_time
         pop[self.event_count_column] += 1
         self.population_view.update(pop)
 
         if self.side_effect_function is not None:
             self.side_effect_function(index, event_time)
 
-    def load_population_columns(self, pop_data):
-        """Adds this state's columns to the simulation state table.
+    ##################
+    # Public methods #
+    ##################
+
+    def get_transition_names(self) -> List[str]:
+        transitions = []
+        for trans in self.transition_set.transitions:
+            _, _, init_state, _, end_state = trans.name.split(".")
+            transitions.append(TransitionString(f"{init_state}_TO_{end_state}"))
+        return transitions
+
+    def add_transition(
+        self,
+        output: State,
+        source_data_type: str = None,
+        get_data_functions: Dict[str, Callable] = None,
+        **kwargs,
+    ) -> Transition:
+        """Builds a transition from this state to the given state.
 
         Parameters
         ----------
-        event : `vivarium.framework.population.PopulationEvent`
-            An event signaling the creation of new simulants.
-        """
+        output
+            The end state after the transition.
 
-        self.population_view.update(pd.DataFrame({self.event_time_column: pd.Series(pd.NaT, index=pop_data.index),
-                                                  self.event_count_column: pd.Series(0, index=pop_data.index)},
-                                                 index=pop_data.index))
+        source_data_type
+            the type of transition: either 'rate' or 'proportion'
 
-        for transition in self.transition_set:
-            if transition.start_active:
-                transition.set_active(pop_data.index)
+        get_data_functions
+            map from transition type to the function to pull that transition's data
 
-    def add_transition(self, output, source_data_type=None, get_data_functions=None, **kwargs):
-        transition_map = {'rate': RateTransition, 'proportion': ProportionTransition}
+        Returns
+        -------
+        vivarium.framework.state_machine.Transition
+            The created transition object.
 
-        if source_data_type is not None and source_data_type not in transition_map:
-            raise ValueError(f"Unrecognized data type {source_data_type}")
+        """
+        transition_map = {"rate": RateTransition, "proportion": ProportionTransition}
 
         if not source_data_type:
             return super().add_transition(output, **kwargs)
         elif source_data_type in transition_map:
             t = transition_map[source_data_type](self, output, get_data_functions, **kwargs)
             self.transition_set.append(t)
             return t
-
-    def metrics(self, index, metrics):
-        """Records data for simulation post-processing.
-
-        Parameters
-        ----------
-        index : iterable of ints
-            An iterable of integer labels for the simulants.
-        metrics : `pandas.DataFrame`
-            A table for recording simulation events of interest in post-processing.
-
-        Returns
-        -------
-        `pandas.DataFrame`
-            The metrics table updated to reflect new simulation state."""
-
-        population = self.population_view.get(index)
-        metrics[self.event_count_column] = population[self.event_count_column].sum()
-        return metrics
+        else:
+            raise ValueError(f"Unrecognized data type {source_data_type}")
 
 
 class SusceptibleState(BaseDiseaseState):
     def __init__(self, cause, *args, **kwargs):
-        super().__init__(cause, *args, name_prefix='susceptible_to_', **kwargs)
+        super().__init__(cause, *args, name_prefix="susceptible_to_", **kwargs)
 
-    def add_transition(self, output, source_data_type=None, get_data_functions=None, **kwargs):
-        if source_data_type == 'rate':
+    def add_transition(
+        self,
+        output: State,
+        source_data_type: str = None,
+        get_data_functions: Dict[str, Callable] = None,
+        **kwargs,
+    ) -> Transition:
+        if source_data_type == "rate":
             if get_data_functions is None:
                 get_data_functions = {
-                    'incidence_rate': lambda cause, builder: builder.data.load(f"{self.cause_type}.{cause}.incidence")
+                    "incidence_rate": lambda builder, cause: builder.data.load(
+                        f"{self.cause_type}.{cause}.incidence_rate"
+                    )
                 }
-            elif 'incidence_rate' not in get_data_functions:
-                raise ValueError('You must supply an incidence rate function.')
-        elif source_data_type == 'proportion':
-            if 'proportion' not in get_data_functions:
-                raise ValueError('You must supply a proportion function.')
+            elif "incidence_rate" not in get_data_functions:
+                raise ValueError("You must supply an incidence rate function.")
+        elif source_data_type == "proportion":
+            if "proportion" not in get_data_functions:
+                raise ValueError("You must supply a proportion function.")
 
         return super().add_transition(output, source_data_type, get_data_functions, **kwargs)
 
 
 class RecoveredState(BaseDiseaseState):
     def __init__(self, cause, *args, **kwargs):
-        super().__init__(cause, *args, name_prefix='recovered_from_', **kwargs)
+        super().__init__(cause, *args, name_prefix="recovered_from_", **kwargs)
 
-    def add_transition(self, output, source_data_type=None, get_data_functions=None, **kwargs):
-        if source_data_type == 'rate':
+    def add_transition(
+        self,
+        output: State,
+        source_data_type: str = None,
+        get_data_functions: Dict[str, Callable] = None,
+        **kwargs,
+    ) -> Transition:
+        if source_data_type == "rate":
             if get_data_functions is None:
                 get_data_functions = {
-                    'incidence_rate': lambda cause, builder: builder.data.load(f"{self.cause_type}.{cause}.incidence")
+                    "incidence_rate": lambda builder, cause: builder.data.load(
+                        f"{self.cause_type}.{cause}.incidence_rate"
+                    )
                 }
-            elif 'incidence_rate' not in get_data_functions:
-                raise ValueError('You must supply an incidence rate function.')
-        elif source_data_type == 'proportion':
-            if 'proportion' not in get_data_functions:
-                raise ValueError('You must supply a proportion function.')
+            elif "incidence_rate" not in get_data_functions:
+                raise ValueError("You must supply an incidence rate function.")
+        elif source_data_type == "proportion":
+            if "proportion" not in get_data_functions:
+                raise ValueError("You must supply a proportion function.")
 
         return super().add_transition(output, source_data_type, get_data_functions, **kwargs)
 
 
 class DiseaseState(BaseDiseaseState):
     """State representing a disease in a state machine model."""
+
     def __init__(self, cause, get_data_functions=None, cleanup_function=None, **kwargs):
         """
         Parameters
         ----------
-        state_id : str
+        cause : str
             The name of this state.
         disability_weight : pandas.DataFrame or float, optional
             The amount of disability associated with this state.
         prevalence_data : pandas.DataFrame, optional
             The baseline occurrence of this state in a population.
         dwell_time : pandas.DataFrame or pandas.Timedelta, optional
             The minimum time a simulant exists in this state.
@@ -169,213 +217,300 @@
             The name of a column to track the last time this state was entered.
         event_count_column : str, optional
             The name of a column to track the number of times this state was entered.
         side_effect_function : callable, optional
             A function to be called when this state is entered.
         """
         super().__init__(cause, **kwargs)
-        self._get_data_functions = get_data_functions if get_data_functions is not None else {}
+
+        self.excess_mortality_rate_pipeline_name = f"{self.state_id}.excess_mortality_rate"
+        self.excess_mortality_rate_paf_pipeline_name = (
+            f"{self.excess_mortality_rate_pipeline_name}.paf"
+        )
+
+        self._get_data_functions = (
+            get_data_functions if get_data_functions is not None else {}
+        )
         self.cleanup_function = cleanup_function
 
-        if (self.cause is None and
-                not set(self._get_data_functions.keys()).issuperset(['disability_weight', 'dwell_time', 'prevalence'])):
-            raise ValueError('If you do not provide a cause, you must supply'
-                             'custom data gathering functions for disability_weight, prevalence, and dwell_time.')
+        if self.cause is None and not set(self._get_data_functions.keys()).issuperset(
+            ["disability_weight", "dwell_time", "prevalence"]
+        ):
+            raise ValueError(
+                "If you do not provide a cause, you must supply"
+                "custom data gathering functions for disability_weight, prevalence, and dwell_time."
+            )
 
+    # noinspection PyAttributeOutsideInit
     def setup(self, builder):
         """Performs this component's simulation setup.
 
         Parameters
         ----------
         builder : `engine.Builder`
             Interface to several simulation tools.
         """
         super().setup(builder)
-        get_disability_weight_func = self._get_data_functions.get(
-            'disability_weight', lambda cause, builder: builder.data.load(
-                f"{self.cause_type}.{cause}.disability_weight"))
-        get_prevalence_func = self._get_data_functions.get(
-            'prevalence', lambda cause, builder: builder.data.load(f"{self.cause_type}.{cause}.prevalence"))
-        get_birth_prevalence_func = self._get_data_functions.get(
-            'birth_prevalence', lambda cause, builder: 0)
-        get_dwell_time_func = self._get_data_functions.get('dwell_time', lambda *args, **kwargs: pd.Timedelta(0))
-
-        self.prevalence_data = builder.lookup.build_table(get_prevalence_func(self.cause, builder))
-        self.birth_prevalence_data = builder.lookup.build_table(get_birth_prevalence_func(self.cause, builder),
-                                                                parameter_columns=(['year', 'year_start', 'year_end'],))
-        self._dwell_time = get_dwell_time_func(self.cause, builder)
-        self.randomness_prevalence = builder.randomness.get_stream(f'{self.state_id}_prevalent_cases')
-
-        disability_weight_data = get_disability_weight_func(self.cause, builder)
-        if isinstance(disability_weight_data, pd.DataFrame) and len(disability_weight_data) == 1:
-            disability_weight_data = disability_weight_data.value[0]  # sequela only have single value
-        self._disability_weight = builder.lookup.build_table(disability_weight_data)
-        self.disability_weight = builder.value.register_value_producer(f'{self._model}.disability_weight',
-                                                                       source=self.compute_disability_weight)
-        builder.value.register_value_modifier('disability_weight', modifier=self.disability_weight)
 
-        if isinstance(self._dwell_time, pd.DataFrame) or self._dwell_time.days > 0:
-            self.transition_set.allow_null_transition = True
+        prevalence_data = self.load_prevalence_data(builder)
+        self.prevalence = builder.lookup.build_table(
+            prevalence_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+
+        birth_prevalence_data = self.load_birth_prevalence_data(builder)
+        self.birth_prevalence = builder.lookup.build_table(
+            birth_prevalence_data, key_columns=["sex"], parameter_columns=["year"]
+        )
+
+        dwell_time_data = self.load_dwell_time_data(builder)
+        self.dwell_time = builder.value.register_value_producer(
+            f"{self.state_id}.dwell_time",
+            source=builder.lookup.build_table(
+                dwell_time_data, key_columns=["sex"], parameter_columns=["age", "year"]
+            ),
+            requires_columns=["age", "sex"],
+        )
+
+        disability_weight_data = self.load_disability_weight_data(builder)
+        self.has_disability = is_non_zero(disability_weight_data)
+        self.base_disability_weight = builder.lookup.build_table(
+            disability_weight_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.disability_weight = builder.value.register_value_producer(
+            f"{self.state_id}.disability_weight",
+            source=self.compute_disability_weight,
+            requires_columns=["age", "sex", "alive", self._model],
+        )
+        builder.value.register_value_modifier(
+            "disability_weight", modifier=self.disability_weight
+        )
+
+        excess_mortality_data = self.load_excess_mortality_rate_data(builder)
+        self.has_excess_mortality = is_non_zero(excess_mortality_data)
+        self.base_excess_mortality_rate = builder.lookup.build_table(
+            excess_mortality_data, key_columns=["sex"], parameter_columns=["age", "year"]
+        )
+        self.excess_mortality_rate = builder.value.register_rate_producer(
+            self.excess_mortality_rate_pipeline_name,
+            source=self.compute_excess_mortality_rate,
+            requires_columns=["age", "sex", "alive", self._model],
+            requires_values=[self.excess_mortality_rate_paf_pipeline_name],
+        )
+        paf = builder.lookup.build_table(0)
+        self.joint_paf = builder.value.register_value_producer(
+            self.excess_mortality_rate_paf_pipeline_name,
+            source=lambda idx: [paf(idx)],
+            preferred_combiner=list_combiner,
+            preferred_post_processor=union_post_processor,
+        )
+        builder.value.register_value_modifier(
+            "mortality_rate",
+            modifier=self.adjust_mortality_rate,
+            requires_values=[self.excess_mortality_rate_pipeline_name],
+        )
+
+        self.randomness_prevalence = builder.randomness.get_stream(
+            f"{self.state_id}_prevalent_cases"
+        )
+
+    def get_initial_event_times(self, pop_data: SimulantData) -> pd.DataFrame:
+        pop_update = super().get_initial_event_times(pop_data)
+
+        simulants_with_condition = self.population_view.subview([self._model]).get(
+            pop_data.index, query=f'{self._model}=="{self.state_id}"'
+        )
+        if not simulants_with_condition.empty:
+            infected_at = self._assign_event_time_for_prevalent_cases(
+                simulants_with_condition,
+                self.clock(),
+                self.randomness_prevalence.get_draw,
+                self.dwell_time,
+            )
+            pop_update.loc[infected_at.index, self.event_time_column] = infected_at
 
-        if isinstance(self._dwell_time, pd.Timedelta):
-            self._dwell_time = self._dwell_time.total_seconds() / (60*60*24)
+        return pop_update
 
-        self.dwell_time = builder.value.register_value_producer(f'{self.state_id}.dwell_time',
-                                                                source=builder.lookup.build_table(self._dwell_time))
+    def compute_disability_weight(self, index):
+        """Gets the disability weight associated with this state.
 
-    def load_population_columns(self, pop_data):
-        super().load_population_columns(pop_data)
-        simulants_with_condition = self.population_view.get(pop_data.index, query=f'{self._model}=="{self.state_id}"')
-        if not simulants_with_condition.empty:
-            infected_at = self._assign_event_time_for_prevalent_cases(simulants_with_condition, self.clock(),
-                                                                      self.randomness_prevalence.get_draw,
-                                                                      self.dwell_time)
-            infected_at.name = self.event_time_column
-            self.population_view.update(infected_at)
+        Parameters
+        ----------
+        index
+            An iterable of integer labels for the simulants.
+
+        Returns
+        -------
+        `pandas.Series`
+            An iterable of disability weights indexed by the provided `index`.
+        """
+        disability_weight = pd.Series(0, index=index)
+        with_condition = self.with_condition(index)
+        disability_weight.loc[with_condition] = self.base_disability_weight(with_condition)
+        return disability_weight
+
+    def compute_excess_mortality_rate(self, index):
+        excess_mortality_rate = pd.Series(0, index=index)
+        with_condition = self.with_condition(index)
+        base_excess_mort = self.base_excess_mortality_rate(with_condition)
+        joint_mediated_paf = self.joint_paf(with_condition)
+        excess_mortality_rate.loc[with_condition] = base_excess_mort * (
+            1 - joint_mediated_paf.values
+        )
+        return excess_mortality_rate
+
+    def adjust_mortality_rate(self, index, rates_df):
+        """Modifies the baseline mortality rate for a simulant if they are in this state.
+
+        Parameters
+        ----------
+        index
+            An iterable of integer labels for the simulants.
+        rates_df : `pandas.DataFrame`
+
+        """
+        rate = self.excess_mortality_rate(index, skip_post_processor=True)
+        rates_df[self.state_id] = rate
+        return rates_df
+
+    def with_condition(self, index):
+        pop = self.population_view.subview(["alive", self._model]).get(index)
+        with_condition = pop.loc[
+            (pop[self._model] == self.state_id) & (pop["alive"] == "alive")
+        ].index
+        return with_condition
 
     @staticmethod
-    def _assign_event_time_for_prevalent_cases(infected, current_time, randomness_func, dwell_time_func):
+    def _assign_event_time_for_prevalent_cases(
+        infected, current_time, randomness_func, dwell_time_func
+    ):
         dwell_time = dwell_time_func(infected.index)
         infected_at = dwell_time * randomness_func(infected.index)
-        infected_at = current_time - pd.to_timedelta(infected_at, unit='D')
+        infected_at = current_time - pd.to_timedelta(infected_at, unit="D")
         return infected_at
 
-    def add_transition(self, output, source_data_type=None, get_data_functions=None, **kwargs):
-        if source_data_type == 'rate':
+    def add_transition(
+        self,
+        output: State,
+        source_data_type: str = None,
+        get_data_functions: Dict[str, Callable] = None,
+        **kwargs,
+    ) -> Transition:
+        if source_data_type == "rate":
             if get_data_functions is None:
                 get_data_functions = {
-                    'remission_rate': lambda cause, builder: builder.data.load(f"{self.cause_type}.{cause}.remission")
+                    "remission_rate": lambda builder, cause: builder.data.load(
+                        f"{self.cause_type}.{cause}.remission_rate"
+                    )
                 }
-            elif 'remission_rate' not in get_data_functions:
-                raise ValueError('You must supply a remission rate function.')
-        elif source_data_type == 'proportion':
-            if 'proportion' not in get_data_functions:
-                raise ValueError('You must supply a proportion function.')
+            elif (
+                "remission_rate" not in get_data_functions
+                and "transition_rate" not in get_data_functions
+            ):
+                raise ValueError(
+                    "You must supply a transition rate or remission rate function."
+                )
+        elif source_data_type == "proportion":
+            if "proportion" not in get_data_functions:
+                raise ValueError("You must supply a proportion function.")
         return super().add_transition(output, source_data_type, get_data_functions, **kwargs)
 
-    def next_state(self, index, event_time, population_view):
+    def next_state(
+        self, index: pd.Index, event_time: pd.Timestamp, population_view: PopulationView
+    ):
         """Moves a population among different disease states.
 
         Parameters
         ----------
-        index : iterable of ints
+        index
             An iterable of integer labels for the simulants.
-        event_time : pandas.Timestamp
+        event_time:
             The time at which this transition occurs.
-        population_view : vivarium.framework.population.PopulationView
+        population_view:
             A view of the internal state of the simulation.
         """
         eligible_index = self._filter_for_transition_eligibility(index, event_time)
         return super().next_state(eligible_index, event_time, population_view)
 
     def _filter_for_transition_eligibility(self, index, event_time):
         """Filter out all simulants who haven't been in the state for the prescribed dwell time.
 
         Parameters
         ----------
-        index : iterable of ints
+        index
             An iterable of integer labels for the simulants.
 
         Returns
         -------
-        iterable of ints
+        pd.Index
             A filtered index of the simulants.
         """
         population = self.population_view.get(index, query='alive == "alive"')
         if np.any(self.dwell_time(index)) > 0:
-            state_exit_time = population[self.event_time_column] + pd.to_timedelta(self.dwell_time(index), unit='D')
+            state_exit_time = population[self.event_time_column] + pd.to_timedelta(
+                self.dwell_time(index), unit="D"
+            )
             return population.loc[state_exit_time <= event_time].index
         else:
             return index
 
     def _cleanup_effect(self, index, event_time):
         if self.cleanup_function is not None:
             self.cleanup_function(index, event_time)
 
-    def compute_disability_weight(self, index):
-        """Gets the disability weight associated with this state.
+    def load_prevalence_data(self, builder):
+        if "prevalence" in self._get_data_functions:
+            return self._get_data_functions["prevalence"](builder, self.cause)
+        else:
+            return builder.data.load(f"{self.cause_type}.{self.cause}.prevalence")
 
-        Parameters
-        ----------
-        index : iterable of ints
-            An iterable of integer labels for the simulants.
+    def load_birth_prevalence_data(self, builder):
+        if "birth_prevalence" in self._get_data_functions:
+            return self._get_data_functions["birth_prevalence"](builder, self.cause)
+        else:
+            return 0
 
-        Returns
-        -------
-        `pandas.Series`
-            An iterable of disability weights indexed by the provided `index`."""
-        population = self.population_view.get(index)
+    def load_dwell_time_data(self, builder):
+        if "dwell_time" in self._get_data_functions:
+            dwell_time = self._get_data_functions["dwell_time"](builder, self.cause)
+        else:
+            dwell_time = 0
+
+        if isinstance(dwell_time, pd.Timedelta):
+            dwell_time = dwell_time.total_seconds() / (60 * 60 * 24)
+        if (
+            isinstance(dwell_time, pd.DataFrame) and np.any(dwell_time.value != 0)
+        ) or dwell_time > 0:
+            self.transition_set.allow_null_transition = True
 
-        return self._disability_weight(population.index) * ((population[self._model] == self.state_id)
-                                                            & (population.alive == 'alive'))
+        return dwell_time
 
-    def name(self):
-        return '{}'.format(self.state_id)
+    def load_disability_weight_data(self, builder):
+        if "disability_weight" in self._get_data_functions:
+            disability_weight = self._get_data_functions["disability_weight"](
+                builder, self.cause
+            )
+        else:
+            disability_weight = builder.data.load(
+                f"{self.cause_type}.{self.cause}.disability_weight"
+            )
+
+        if isinstance(disability_weight, pd.DataFrame) and len(disability_weight) == 1:
+            disability_weight = disability_weight.value[0]  # sequela only have single value
+
+        return disability_weight
+
+    def load_excess_mortality_rate_data(self, builder):
+        only_morbid = builder.data.load(f"cause.{self._model}.restrictions")["yld_only"]
+        if "excess_mortality_rate" in self._get_data_functions:
+            return self._get_data_functions["excess_mortality_rate"](builder, self.cause)
+        elif only_morbid:
+            return 0
+        else:
+            return builder.data.load(f"{self.cause_type}.{self.cause}.excess_mortality_rate")
 
     def __repr__(self):
-        return 'DiseaseState({})'.format(self.state_id)
+        return "DiseaseState({})".format(self.state_id)
 
 
 class TransientDiseaseState(BaseDiseaseState, Transient):
-
     def __repr__(self):
-        return 'TransientDiseaseState(name={})'.format(self.state_id)
-
-
-class ExcessMortalityState(DiseaseState):
-    """State representing a disease with excess mortality in a state machine model.
-
-    Attributes
-    ----------
-    state_id : str
-        The name of this state.
-    excess_mortality_data : `pandas.DataFrame`
-        A table of excess mortality data associated with this state.
-    """
-    def __init__(self, cause, **kwargs):
-        super().__init__(cause, **kwargs)
-
-    def setup(self, builder):
-        """Performs this component's simulation setup.
-        Parameters
-        ----------
-        builder : `engine.Builder`
-            Interface to several simulation tools.
-        """
-        super().setup(builder)
-        get_excess_mortality_func = self._get_data_functions.get('excess_mortality', lambda cause, builder: builder.data.load(f"{self.cause_type}.{cause}.excess_mortality"))
-
-        self.base_excess_mortality = builder.lookup.build_table(get_excess_mortality_func(self.cause, builder))
-        self._mortality = builder.value.register_rate_producer(f'{self.state_id}.excess_mortality',
-                                                               source=self.effective_excess_mortality)
-        self.joint_paf = builder.value.register_value_producer(f'{self.state_id}.excess_mortality.paf',
-                                                               source=lambda idx: [builder.lookup.build_table(0)(idx)],
-                                                               preferred_combiner=list_combiner,
-                                                               preferred_post_processor=joint_value_post_processor)
-        builder.value.register_value_modifier('mortality_rate', modifier=self.mortality_rates)
-
-    def effective_excess_mortality(self, index):
-        base_excess_mort = self.base_excess_mortality(index)
-        joint_mediated_paf = self.joint_paf(index)
-        return pd.Series(base_excess_mort.values * (1 - joint_mediated_paf.values), index=index)
-
-    def mortality_rates(self, index, rates_df):
-        """Modifies the baseline mortality rate for a simulant if they are in this state.
-
-        Parameters
-        ----------
-        index : iterable of ints
-            An iterable of integer labels for the simulants.
-        rates_df : `pandas.DataFrame`
-
-        """
-        population = self.population_view.get(index)
-        rate = (self._mortality(population.index, skip_post_processor=True)
-                * (population[self._model] == self.state_id))
-        if isinstance(rates_df, pd.Series):
-            rates_df = pd.DataFrame({rates_df.name: rates_df, self.state_id: rate})
-        else:
-            rates_df[self.state_id] = rate
-        return rates_df
-
-    def __str__(self):
-        return 'ExcessMortalityState({})'.format(self.state_id)
+        return "TransientDiseaseState(name={})".format(self.state_id)
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/special_disease.py` & `vivarium_public_health-1.0.0/src/vivarium_public_health/risks/base_risk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,174 +1,196 @@
-import pandas as pd
-import re
-from operator import lt, gt
+"""
+===================
+Risk Exposure Model
+===================
+
+This module contains tools for modeling categorical and continuous risk
+exposure.
 
-from collections import namedtuple
+"""
+from typing import Dict, List
+
+import pandas as pd
+from vivarium.framework.engine import Builder
+from vivarium.framework.population import PopulationView, SimulantData
+from vivarium.framework.randomness import RandomnessStream
+from vivarium.framework.values import Pipeline
+
+from vivarium_public_health.risks.data_transformations import (
+    get_exposure_post_processor,
+)
+from vivarium_public_health.risks.distributions import SimulationDistribution
 from vivarium_public_health.utilities import EntityString
 
 
-class RiskAttributableDisease:
-    """Component to model a disease fully attributed by a risk.
-    
-    For some (risk, cause) pairs with population attributable fraction
-    equal to 1, the clinical definition of the with condition state 
-    corresponds to a particular exposure of a risk.
-
-    For example, a diagnosis of ``diabetes_mellitus`` occurs after 
-    repeated measurements of fasting plasma glucose above 7 mmol/L. 
-    Similarly, ``protein_energy_malnutrition`` corresponds to a weight 
-    for height ratio that is more than two standard deviations below
-    the WHO guideline median weight for height.  In the Global Burden
-    of Disease, this corresponds to a categorical exposure to 
-    ``child_wasting`` in either ``cat1`` or ``cat2``.
-    
-    The definition of the disease in terms of exposure should be provided
-    in the ``threshold`` configuration flag.  For risks with continuous
-    exposure models, the threshold should be provided as a single 
-    ``float`` or ``int`` with a proper sign between ">" and "<", implying
-    that disease is defined by the exposure level ">" than threshold level
-    or, "<" than threshold level, respectively.
-
-    For categorical risks, the threshold
-    should be provided as a list of categories.
-    
-    In addition to the threshold level, you may configure whether
-    there is any mortality associated with this disease with the 
-    ``mortality`` configuration flag.
-     
-    Finally, you may specify whether the someone should "recover" 
-    from the disease if their exposure level falls outside the 
-    provided threshold. 
-    
-    In our provided examples, a person would no longer be experiencing 
-    ``protein_energy_malnutrition`` if their exposure drift out (or
-    changes via an intervention) of the provided exposure categories. 
-    Having your ``fasting_plasma_glucose`` drop below a provided level
-    does not necessarily mean you're no longer diabetic however.
-
-    To add this component, you need to initialize it with full cause name
-    and full risk name, e.g.,
-
-    RiskAttributableDisease('cause.protein_energy_malnutrition',
-                            'risk_factor.child_wasting')
-
-    Configuration defaults should be given as, for the continuous risk factor,
-
-    diabetes_mellitus:
-        threshold : ">7"
-        mortality : True
-        recoverable : False
-
-    For the categorical risk factor,
-
-    protein_energy_malnutrition:
-        threshold : ['cat1', 'cat2'] # provide the categories to get PEM.
-        mortality : True
-        recoverable : True
+class Risk:
+    """A model for a risk factor defined by either a continuous or a categorical
+    value. For example,
+
+    #. high systolic blood pressure as a risk where the SBP is not dichotomized
+       into hypotension and normal but is treated as the actual SBP
+       measurement.
+    #. smoking as two categories: current smoker and non-smoker.
+
+    This component can source data either from builder.data or from parameters
+    supplied in the configuration. If data is derived from the configuration, it
+    must be an integer or float expressing the desired exposure level or a
+    covariate name that is intended to be used as a proxy. For example, for a
+    risk named "risk", the configuration could look like this:
+
+    .. code-block:: yaml
+
+       configuration:
+           risk:
+               exposure: 1.0
+
+    or
+
+    .. code-block:: yaml
+
+       configuration:
+           risk:
+               exposure: proxy_covariate
+
+    For polytomous risks, you can also provide an optional 'rebinned_exposed'
+    block in the configuration to indicate that the risk should be rebinned
+    into a dichotomous risk. That block should contain a list of the categories
+    that should be rebinned into a single exposed category in the resulting
+    dichotomous risk. For example, for a risk named "risk" with categories
+    cat1, cat2, cat3, and cat4 that you wished to rebin into a dichotomous risk
+    with an exposed category containing cat1 and cat2 and an unexposed category
+    containing cat3 and cat4, the configuration could look like this:
+
+    .. code-block:: yaml
+
+       configuration:
+           risk:
+              rebinned_exposed: ['cat1', 'cat2']
+
+    For alternative risk factors, you must provide a 'category_thresholds'
+    block in the in configuration to dictate the thresholds that should be
+    used to bin the continuous distributions. Note that this is mutually
+    exclusive with providing 'rebinned_exposed' categories. For a risk named
+    "risk", the configuration could look like:
+
+    .. code-block:: yaml
+
+       configuration:
+           risk:
+               category_thresholds: [7, 8, 9]
+
     """
 
     configuration_defaults = {
-        'risk_attributable_disease': {
-            'threshold': None,
-            'mortality': True,
-            'recoverable': True
+        "risk": {
+            "exposure": "data",
+            "rebinned_exposed": [],
+            "category_thresholds": [],
         }
     }
 
-    def __init__(self, cause, risk):
-        self.cause = EntityString(cause)
+    def __init__(self, risk: str):
+        """
+        Parameters
+        ----------
+        risk :
+            the type and name of a risk, specified as "type.name". Type is singular.
+        """
         self.risk = EntityString(risk)
-        self.configuration_defaults = {
-            self.cause.name: RiskAttributableDisease.configuration_defaults['risk_attributable_disease']
-        }
-
-    def setup(self, builder):
-        self.recoverable = builder.configuration[self.cause.name].recoverable
-
-        if builder.configuration[self.cause.name].mortality:
-            csmr_data = builder.data.load(f'cause.{self.cause.name}.cause_specific_mortality')
-            builder.value.register_value_modifier('csmr_data', lambda: csmr_data)
-            excess_mortality_data = builder.data.load(f'{self.cause}.excess_mortality')
-            builder.value.register_value_modifier('mortality_rate', self.mortality_rates)
-            self._mortality = builder.value.register_value_producer(
-                f'{self.cause}.excess_mortality', source=builder.lookup.build_table(excess_mortality_data)
+        self.configuration_defaults = self._get_configuration_defaults()
+        self.exposure_distribution = self._get_exposure_distribution()
+        self._sub_components = [self.exposure_distribution]
+
+        self._randomness_stream_name = f"initial_{self.risk.name}_propensity"
+        self.propensity_column_name = f"{self.risk.name}_propensity"
+        self.propensity_pipeline_name = f"{self.risk.name}.propensity"
+        self.exposure_pipeline_name = f"{self.risk.name}.exposure"
+
+    def __repr__(self) -> str:
+        return f"Risk({self.risk})"
+
+    ##########################
+    # Initialization methods #
+    ##########################
+
+    def _get_configuration_defaults(self) -> Dict[str, Dict]:
+        return {self.risk.name: Risk.configuration_defaults["risk"]}
+
+    def _get_exposure_distribution(self) -> SimulationDistribution:
+        return SimulationDistribution(self.risk)
+
+    ##############
+    # Properties #
+    ##############
+
+    @property
+    def name(self) -> str:
+        return f"risk.{self.risk}"
+
+    @property
+    def sub_components(self) -> List:
+        return self._sub_components
+
+    #################
+    # Setup methods #
+    #################
+
+    # noinspection PyAttributeOutsideInit
+    def setup(self, builder: Builder) -> None:
+        self.randomness = self._get_randomness_stream(builder)
+        self.propensity = self._get_propensity_pipeline(builder)
+        self.exposure = self._get_exposure_pipeline(builder)
+        self.population_view = self._get_population_view(builder)
+
+        self._register_simulant_initializer(builder)
+
+    def _get_randomness_stream(self, builder) -> RandomnessStream:
+        return builder.randomness.get_stream(self._randomness_stream_name)
+
+    def _get_propensity_pipeline(self, builder: Builder) -> Pipeline:
+        return builder.value.register_value_producer(
+            self.propensity_pipeline_name,
+            source=lambda index: (
+                self.population_view.subview([self.propensity_column_name])
+                .get(index)
+                .squeeze(axis=1)
+            ),
+            requires_columns=[self.propensity_column_name],
+        )
+
+    def _get_exposure_pipeline(self, builder: Builder) -> Pipeline:
+        return builder.value.register_value_producer(
+            self.exposure_pipeline_name,
+            source=self._get_current_exposure,
+            requires_columns=["age", "sex"],
+            requires_values=[self.propensity_pipeline_name],
+            preferred_post_processor=get_exposure_post_processor(builder, self.risk),
+        )
+
+    def _get_population_view(self, builder: Builder) -> PopulationView:
+        return builder.population.get_view([self.propensity_column_name])
+
+    def _register_simulant_initializer(self, builder: Builder) -> None:
+        builder.population.initializes_simulants(
+            self.on_initialize_simulants,
+            creates_columns=[self.propensity_column_name],
+            requires_streams=[self._randomness_stream_name],
+        )
+
+    ########################
+    # Event-driven methods #
+    ########################
+
+    def on_initialize_simulants(self, pop_data: SimulantData) -> None:
+        self.population_view.update(
+            pd.Series(
+                self.randomness.get_draw(pop_data.index), name=self.propensity_column_name
             )
+        )
 
-        disability_weight = builder.data.load(f'{self.cause}.disability_weight')
-        self._disability_weight = builder.lookup.build_table(disability_weight)
-        self.disability_weight = builder.value.register_value_producer(f'{self.cause}.disability_weight',
-                                                                       source=self.compute_disability_weight)
-        builder.value.register_value_modifier('disability_weight', modifier=self.disability_weight)
-
-        distribution = builder.data.load(f'{self.risk}.distribution')
-        exposure_pipeline = builder.value.get_value(f'{self.risk.name}.exposure')
-        threshold = builder.configuration[self.cause.name].threshold
-
-        self.filter_by_exposure = self.get_exposure_filter(distribution, exposure_pipeline, threshold)
-        self.population_view = builder.population.get_view([self.cause.name, 'alive'])
-
-        builder.event.register_listener('time_step', self.on_time_step)
-        builder.population.initializes_simulants(self.on_initialize_simulants)
-
-    def on_initialize_simulants(self, pop_data):
-        new_pop = pd.Series(f'susceptible_to_{self.cause.name}', index=pop_data.index, name=self.cause.name)
-        sick = self.filter_by_exposure(pop_data.index)
-        new_pop[sick] = self.cause.name
-        self.population_view.update(new_pop)
-
-    def on_time_step(self, event):
-        pop = self.population_view.get(event.index, query='alive == "alive"')
-        sick = self.filter_by_exposure(pop.index)
-        #  if this is recoverable, anyone who gets lower exposure in the event goes back in to susceptible status.
-        if self.recoverable:
-            pop.loc[~sick, self.cause.name] = f'susceptible_to_{self.cause.name}'
-        pop.loc[sick, self.cause.name] = self.cause.name
-        self.population_view.update(pop)
-
-    def get_exposure_filter(self, distribution, exposure_pipeline, threshold):
-
-        if distribution in ['dichotomous', 'ordered_polytomous', 'unordered_polytomous']:
-
-            def categorical_filter(index):
-                exposure = exposure_pipeline(index)
-                return exposure.isin(threshold)
-            filter_function = categorical_filter
-
-        else:  # continuous
-            Threshold = namedtuple('Threshold', ['operator', 'value'])
-            threshold_val = re.findall("[-+]?\d*\.?\d+", threshold)
-
-            if len(threshold_val) != 1:
-                raise ValueError(f'Your {threshold} is an incorrect threshold format. It should include "<" or ">" along'
-                                 f' with an integer or float number. Your threshold does not include a number or more '
-                                 'than one number.')
-
-            allowed_operator = {'<', '>'}
-            threshold_op = [s for s in threshold.split(threshold_val[0]) if s]
-            #  if threshold_op has more than 1 operators or 0 operator
-            if len(threshold_op) != 1 or not allowed_operator.intersection(threshold_op):
-                raise ValueError(f'Your {threshold} is an incorrect threshold format. It should include "<" or ">" along'
-                                 f' with an integer or float number.')
-
-            op = gt if threshold_op[0] == ">" else lt
-            threshold = Threshold(op, float(threshold_val[0]))
-
-            def continuous_filter(index):
-                exposure = exposure_pipeline(index)
-                return threshold.operator(exposure, threshold.value)
-            filter_function = continuous_filter
-
-        return filter_function
-
-    def mortality_rates(self, index, rates_df):
-        population = self.population_view.get(index)
-        rate = (self._mortality(population.index, skip_post_processor=True)
-                * (population[self.cause.name] == self.cause.name))
-        if isinstance(rates_df, pd.Series):
-            rates_df = pd.DataFrame({rates_df.name: rates_df, self.cause.name: rate})
-        else:
-            rates_df[self.cause.name] = rate
-        return rates_df
-
-    def compute_disability_weight(self, index):
-        population = self.population_view.get(index, query=f'alive=="alive" and {self.cause.name}=="{self.cause.name}"')
-        return self._disability_weight(population.index)
+    ##################################
+    # Pipeline sources and modifiers #
+    ##################################
+
+    def _get_current_exposure(self, index: pd.Index) -> pd.Series:
+        propensity = self.propensity(index)
+        return pd.Series(self.exposure_distribution.ppf(propensity), index=index)
```

### Comparing `vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/PKG-INFO` & `vivarium_public_health-1.0.0/src/vivarium_public_health.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 Metadata-Version: 2.1
 Name: vivarium-public-health
-Version: 0.9.9
+Version: 1.0.0
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
-Author: The vivarium_public_health developers
+Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: GNU GPLv3
-Description: Vivarium Public Health
-        ======================
-        
-        .. image:: https://badge.fury.io/py/vivarium-public-health.svg
-            :target: https://badge.fury.io/py/vivarium-public-health
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=develop
-            :target: https://travis-ci.org/ihmeuw/vivarium_public_health
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium_public_health/badge/?version=latest
-            :target: https://vivarium_public_health.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        .. image:: https://zenodo.org/badge/141212278.svg
-           :target: https://zenodo.org/badge/latestdoi/141212278
-        
-        This library contains several components for for modelling diseases and their interventions.
-        
-        You can install ``vivarium_public_health`` from PyPI with pip:
-        
-          ``> pip install vivarium_public_health``
-        
-        or build it from source with
-        
-          ``> git clone https://github.com/ihmeuw/vivarium_public_health.git``
-        
-          ``> cd vivarium_public_health``
-        
-          ``> python setup.py install``
-        
-        Documentation
-        ======================
-        You can view documentation at https://vivarium_public_health.readthedocs.io/en/latest/
-        
-Platform: UNKNOWN
+License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: dev
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+Vivarium Public Health
+======================
+
+.. image:: https://badge.fury.io/py/vivarium-public-health.svg
+    :target: https://badge.fury.io/py/vivarium-public-health
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_public_health.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/vivarium_public_health
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium_public_health/badge/?version=latest
+    :target: https://vivarium_public_health.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+.. image:: https://zenodo.org/badge/141212278.svg
+   :target: https://zenodo.org/badge/latestdoi/141212278
+
+This library contains several components for for modelling diseases and their interventions.
+
+You can install ``vivarium_public_health`` from PyPI with pip:
+
+  ``> pip install vivarium_public_health``
+
+or build it from source with
+
+  ``> git clone https://github.com/ihmeuw/vivarium_public_health.git``
+
+  ``> cd vivarium_public_health``
+
+  ``> python setup.py install``
+
+Documentation
+======================
+You can view documentation at https://vivarium_public_health.readthedocs.io/en/latest/
```

### Comparing `vivarium_public_health-0.9.9/CONTRIBUTING.rst` & `vivarium_public_health-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

