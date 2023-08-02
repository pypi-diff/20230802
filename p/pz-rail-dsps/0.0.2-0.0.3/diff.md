# Comparing `tmp/pz_rail_dsps-0.0.2.tar.gz` & `tmp/pz_rail_dsps-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_dsps-0.0.2.tar", last modified: Tue Jun 13 18:44:32 2023, max compression
+gzip compressed data, was "pz_rail_dsps-0.0.3.tar", last modified: Wed Aug  2 16:11:37 2023, max compression
```

## Comparing `pz_rail_dsps-0.0.2.tar` & `pz_rail_dsps-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_photometry_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_sed_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/galaxy_population_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/src/rail/dsps/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/dsps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 18:44:31.000000 pz_rail_dsps-0.0.2/src/rail/dsps/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/tests/dsps/
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/tests/dsps/test_dsps_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.345389 pz_rail_dsps-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.337389 pz_rail_dsps-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.337389 pz_rail_dsps-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-02 16:11:37.345389 pz_rail_dsps-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.337389 pz_rail_dsps-0.0.3/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:11:37.345389 pz_rail_dsps-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.337389 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.337389 pz_rail_dsps-0.0.3/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/creation/engines/dsps_photometry_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24505 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/creation/engines/dsps_sed_modeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.341389 pz_rail_dsps-0.0.3/src/rail/dsps/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/dsps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-02 16:11:37.000000 pz_rail_dsps-0.0.3/src/rail/dsps/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.341389 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.341389 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.341389 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.333389 pz_rail_dsps-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:11:37.345389 pz_rail_dsps-0.0.3/tests/dsps/
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-02 16:11:20.000000 pz_rail_dsps-0.0.3/tests/dsps/test_dsps_interface.py
```

### Comparing `pz_rail_dsps-0.0.2/.github/pull_request_template.md` & `pz_rail_dsps-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/.github/workflows/linting.yml` & `pz_rail_dsps-0.0.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/.github/workflows/publish-to-pypi.yml` & `pz_rail_dsps-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/.github/workflows/smoke-test.yml` & `pz_rail_dsps-0.0.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/.github/workflows/testing-and-coverage.yml` & `pz_rail_dsps-0.0.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/.gitignore` & `pz_rail_dsps-0.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 _version.py
+.DS_Store
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `pz_rail_dsps-0.0.2/.pre-commit-config.yaml` & `pz_rail_dsps-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/LICENSE` & `pz_rail_dsps-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/pyproject.toml` & `pz_rail_dsps-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/SOURCES.txt` & `pz_rail_dsps-0.0.3/src/pz_rail_dsps.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+environment.yml
 pyproject.toml
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
+examples/creation_examples/dsps_sed_demo.ipynb
 src/pz_rail_dsps.egg-info/PKG-INFO
 src/pz_rail_dsps.egg-info/SOURCES.txt
 src/pz_rail_dsps.egg-info/dependency_links.txt
 src/pz_rail_dsps.egg-info/requires.txt
 src/pz_rail_dsps.egg-info/top_level.txt
 src/rail/creation/engines/dsps_photometry_creator.py
 src/rail/creation/engines/dsps_sed_modeler.py
-src/rail/creation/engines/galaxy_population_components.py
 src/rail/dsps/__init__.py
 src/rail/dsps/_version.py
+src/rail/examples_data/creation_data/data/.DS_Store
+src/rail/examples_data/creation_data/data/dsps_default_data/.DS_Store
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5
```

### Comparing `pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_photometry_creator.py` & `pz_rail_dsps-0.0.3/src/rail/creation/engines/dsps_photometry_creator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from rail.core.utils import RAILDIR
+from rail.core.utils import find_rail_file
 from rail.creation.engine import Creator
 from rail.core.stage import RailStage
 from rail.core.data import Hdf5Handle
 from ceci.config import StageParameter as Param
 import numpy as np
 from jax import vmap
 from jax import jit as jjit
@@ -12,24 +12,29 @@
 from dsps import load_ssp_templates
 from dsps import load_transmission_curve
 from dsps.cosmology import DEFAULT_COSMOLOGY
 
 
 class DSPSPhotometryCreator(Creator):
     """
-    Derived class of Creator that generate synthetic photometric data from one or more SED models
-    generated with the DSPSSingleSedModeler and DSPSPopulationSedModeler classes.
-    The user is required to provide files in .npy format for the code to run. Details of what each file should
-    contain are explicited in config_options.
-    It accepts as input ModelHandles stored in pickle files and as output a Fits table containing magnitudes.
+    Derived class of Creator that generate synthetic absolute and apparent magnitudes from one or more SED models
+    generated with the DSPSSingleSedModeler or DSPSPopulationSedModeler classes.
+    It accepts as input Hdf5Handles containing the rest-frame SEDs in units of Lsun/Hz and outputs an Hdf5Handle
+    containing sequential indices, absolute and apparent magnitudes for each galaxy.
+    Photometric quantities are computed for the filters defined in the configuration file.
+
+    Notes
+    -----
+    jax serially execute the computations on CPU on single core, for CPU parallelization you need MPI.
+    If GPU is used, jax natively and automatically parallelize the execution.
 
     """
 
     name = "DSPSPhotometryCreator"
-    default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data', 'dsps_default_data')
+    default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data', 'dsps_default_data'))
     config_options = RailStage.config_options.copy()
     config_options.update(redshift_key=Param(str, 'redshifts', msg='Redshift keyword name of the hdf5 dataset '
                                                                    'containing rest-frame SEDs'),
                           restframe_sed_key=Param(str, 'restframe_seds', msg='Rest-frame SED keyword name of the '
                                                                              'hdf5 dataset containing rest-frame SEDs'),
                           absolute_mags_key=Param(str, 'rest_frame_absolute_mags', msg='Absolute magnitudes keyword'
                                                                                        ' name of the output hdf5 '
@@ -39,34 +44,40 @@
                           filter_folder=Param(str, os.path.join(default_files_folder, 'filters'),
                                               msg='Folder containing filter transmissions'),
                           instrument_name=Param(str, 'lsst', msg='Instrument name as prefix to filter transmission'
                                                                  ' files'),
                           wavebands=Param(str, 'u,g,r,i,z,y', msg='Comma-separated list of wavebands'),
                           ssp_templates_file=Param(str, os.path.join(default_files_folder,
                                                                      'ssp_data_fsps_v3.2_lgmet_age.h5'),
-                                                   msg='hdf5 file storing the SSP libraries used to create SEDs'))
+                                                   msg='hdf5 file storing the SSP libraries used to create SEDs'),
+                          default_cosmology = Param(bool, True, msg='True to use default DSPS cosmology. If False,'
+                                                                    'Om0, w0, wa, h need to be supplied in the '
+                                                                    'sample function'))
 
     inputs = [("model", Hdf5Handle)]
     outputs = [("output", Hdf5Handle)]
 
     def __init__(self, args, comm=None):
         """
-        Initialize class.
+        Initialize DSPSPhotometryCreator class. If the SSP templates are not provided by the user, they are automatically
+        downloaded from the public NERSC directory. These default templates are created with default FSPS values,
+        with gas emission at fixed gas solar metallicity value.
         The _b and _c tuples for jax are composed of None or 0, depending on whether you don't or do want the
         array axis to map over for all arguments.
+
         Parameters
         ----------
         args:
         comm:
         """
         RailStage.__init__(self, args, comm=comm)
 
         if not os.path.isfile(self.config.ssp_templates_file):
-            default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data',
-                                                'dsps_default_data')
+            default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data',
+                                                  'dsps_default_data'))
             os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/ssp_data_fsps_v3.2_lgmet_age.h5 '
                       '--output-dir {}'.format(default_files_folder))
 
         if not os.path.isdir(self.config.filter_folder):
             raise OSError("File {self.config.filter_folder} not found")
 
         self.wavebands = self.config.wavebands.split(',')
@@ -79,59 +90,87 @@
         self.filter_transmissions = np.array([load_transmission_curve(fn=os.path.join(self.config.filter_folder,
                                                                                       '{}_{}_transmission.h5'
                                                                                       .format(self.config.
                                                                                               instrument_name,
                                                                                               waveband))).transmission
                                              for waveband in self.wavebands], dtype=object)
 
-    def sample(self, seed: int = None, **kwargs):
+    def sample(self, seed: int = None,
+               input_data=os.path.join(default_files_folder, 'model_DSPSPopulationSedModeler.hdf5'),
+               Om0=DEFAULT_COSMOLOGY.Om0, w0=DEFAULT_COSMOLOGY.w0, wa=DEFAULT_COSMOLOGY.wa,
+               h=DEFAULT_COSMOLOGY.h, **kwargs):
         r"""
-        Creates observed and absolute magnitudes for population of galaxies and stores them into Fits table.
-
-        This is a method for running in interactive mode.
-        In pipeline mode, the subclass `run` method will be called by itself.
+        Creates observed and absolute magnitudes for the population of galaxy rest-frame SEDs and stores them into
+        an Hdf5Handle.
 
         Parameters
         ----------
         seed: int
             The random seed to control sampling
+        input_data: str
+            Filepath to the hdf5 table containing the galaxy rest-frame SEDs.
+        Om0: float
+            Omega matter: density of non-relativistic matter in units of the critical density at z=0.
+        w0: float
+            Dark energy equation of state at z=0 (a=1). This is pressure/density for dark energy in units where c=1.
+        wa: float
+            Negative derivative of the dark energy equation of state with respect to the scale factor.
+            A cosmological constant has w0=-1.0 and wa=0.0.
+        h: float
+            dimensionless Hubble constant at z=0.
 
         Returns
         -------
-        output: astropy.table.Table
-            Fits table storing galaxy magnitudes.
+        output: Hdf5Handle
+            Hdf5Handle storing the absolute and apparent magnitudes.
 
         Notes
         -----
-        This method puts  `seed` into the stage configuration
-        data, which makes them available to other methods.
-        It then calls the `run` method.
-        Finally, the `FitsHandle` associated to the `output` tag is returned.
+        This method puts  `seed` into the stage configuration data, which makes them available to other methods.
+        It then calls the `run` method. Finally, the `Hdf5Handle` associated to the `output` tag is returned.
 
         """
+        if self.config.default_cosmology:
+            self.config.Om0 = DEFAULT_COSMOLOGY.Om0
+            self.config.w0 = DEFAULT_COSMOLOGY.w0
+            self.config.wa = DEFAULT_COSMOLOGY.wa
+            self.config.h = DEFAULT_COSMOLOGY.h
+        else:
+            self.config.Om0 = Om0
+            self.config.w0 = w0
+            self.config.wa = wa
+            self.config.h = h
         self.config["seed"] = seed
         self.config.update(**kwargs)
+        self.set_data('model', input_data)
         self.run()
         self.finalize()
         output = self.get_handle("output")
         return output
 
     def _compute_rest_frame_absolute_magnitudes(self, ssp_data, rest_frame_seds, filter_wavelengths,
                                                 filter_transmissions):
         """
+        Computes the absolute magnitudes of the input rest-frame SEDs using the DSPS _calc_rest_mag_vmap function.
 
         Parameters
         ----------
         ssp_data
+            SSP templates created with FSPS
         rest_frame_seds
+            Rest-frame SEDs in units of Lsun/Hz generated using DSPS v3.* (Hearin+21).
         filter_wavelengths
+            Array of wavelengths for each filter band.
         filter_transmissions
+            Array of transmissions for each filter band.
 
         Returns
         -------
+        restframe_abs_mags
+            Array of absolute magnitudes with size (n_galaxies, n_filter_bands)
 
         """
         # consider the whole chunk
 
         self._b = [None, 0, 0, 0]
         self._calc_rest_mag_vmap = jjit(vmap(calc_rest_mag, in_axes=self._b))
         restframe_abs_mags = np.zeros((len(rest_frame_seds), len(self.wavebands)))
@@ -145,50 +184,59 @@
             restframe_abs_mags[:, j] = self._calc_rest_mag_vmap(*args_abs_mags)
 
         return restframe_abs_mags
 
     def _compute_apparent_magnitudes(self, ssp_data, rest_frame_seds, redshifts, filter_wavelengths,
                                      filter_transmissions):
         """
+        Computes the apparent magnitudes of the input rest-frame SEDs using the DSPS _calc_app_mag_vmap function for
+        a user-defined cosmology.
 
         Parameters
         ----------
         ssp_data
+            SSP templates created with FSPS
         rest_frame_seds
+            Rest-frame SEDs in units of Lsun/Hz generated using DSPS v3.* (Hearin+21).
         redshifts
+            Array of redshifts for each galaxy
         filter_wavelengths
+            Array of wavelengths for each filter band.
         filter_transmissions
+            Array of transmissions for each filter band.
 
         Returns
         -------
+        apparent_mags
+            Array of apparent magnitudes with size (n_galaxies, n_filter_bands)
 
         """
         # consider the whole chunk
 
         self._c = [None, 0, 0, 0, 0, None, None, None, None]
         self._calc_app_mag_vmap = jjit(vmap(calc_obs_mag, in_axes=self._c))
 
         apparent_mags = np.zeros((len(rest_frame_seds), len(self.wavebands)))
         for j in range(len(self.wavebands)):
 
             args_app_mags = (ssp_data.ssp_wave, rest_frame_seds, np.array(list(filter_wavelengths[:, j]),
                                                                           dtype='float'),
                              np.array(list(filter_transmissions[:, j]), dtype='float'), redshifts,
-                             *DEFAULT_COSMOLOGY)
+                             self.config.Om0, self.config.w0, self.config.wa, self.config.h)
 
             apparent_mags[:, j] = self._calc_app_mag_vmap(*args_app_mags)
 
         return apparent_mags
 
     def run(self):
         """
         This function computes rest-frame absolute magnitudes in the provided wavebands for all the galaxies
         in the population by calling `_calc_rest_mag_vmap` from DSPS. It does the same for the observed
         magnitudes in the AB system by calling `_calc_obs_mag_vmap` from DSPS.
-        It then stores both kind of magnitudes and the galaxy indices into an astropy.table.Table.
+        It then stores both kind of magnitudes and the galaxy indices into an Hdf5Handle.
 
         Returns
         -------
 
         """
 
         self.model = self.get_data('model')
```

### Comparing `pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_sed_modeler.py` & `pz_rail_dsps-0.0.3/src/rail/creation/engines/dsps_sed_modeler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 import os
 from rail.creation.engine import Modeler
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.core.utils import find_rail_file
 from rail.core.data import Hdf5Handle
 from ceci.config import StageParameter as Param
 import numpy as np
 from jax import vmap
 from jax import jit as jjit
 from dsps.cosmology import age_at_z, DEFAULT_COSMOLOGY
 from dsps import load_ssp_templates
 from dsps import calc_rest_sed_sfh_table_lognormal_mdf
 from dsps import calc_rest_sed_sfh_table_met_table
 
 
 class DSPSSingleSedModeler(Modeler):
     r"""
-    Derived class of Modeler for creating a single galaxy rest-frame SED model using DSPS (Hearin+21).
+    Derived class of Modeler for creating a single galaxy rest-frame SED model using DSPS v3.* (Hearin+21).
     SPS calculations are based on a set of template SEDs of simple stellar populations (SSPs).
     Supplying such templates is outside the planned scope of the DSPS package, and so they
     will need to be retrieved from some other library. For example, the FSPS library supplies
     such templates in a convenient form.
 
+    The input galaxy properties, such as star-formation histories and metallicities, need to be supplied via an
+    hdf5 table.
+
     Notes
     -----
     The user-provided metallicity grid should be consistently defined with the metallicity of the templates SEDs.
     Users should be cautious in the use of the cosmic time grid. The time resolution strongly depends on the
     user scientific aim.
 
     """
 
     name = "DSPSSingleSedModeler"
-    default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data', 'dsps_default_data')
+    default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data', 'dsps_default_data'))
     config_options = RailStage.config_options.copy()
     config_options.update(ssp_templates_file=Param(str, os.path.join(default_files_folder,
                                                                      'ssp_data_fsps_v3.2_lgmet_age.h5'),
                                                    msg='hdf5 file storing the SSP libraries used to create SEDs'),
                           redshift_key=Param(str, 'redshifts',
-                                             msg='Redshift keyword name of the hdf5 dataset containing input galaxy '
-                                                 'properties'),
+                                             msg='Redshift keyword name of the hdf5 dataset'),
                           cosmic_time_grid_key=Param(str, 'cosmic_time_grid',
-                                                     msg='Cosmic time grid keyword name of the hdf5 dataset containing '
-                                                         'input galaxy properties, this is the grid over '
-                                                         'which the stellar mass build-up takes place in units of Gyr'),
+                                                     msg='Cosmic time grid keyword name of the hdf5 dataset, '
+                                                         'this is the grid of Universe age over which the stellar mass'
+                                                         ' build-up takes place in units of Gyr'),
                           star_formation_history_key=Param(str, 'star_formation_history',
                                                            msg='Star-formation history keyword name of the hdf5 '
-                                                               'dataset containing input galaxy properties, this is '
-                                                               'the star-formation history of the galaxy in units of '
-                                                               'Msun/yr'),
+                                                               'dataset, this is the star-formation history of the '
+                                                               'galaxy in units of Msun/yr'),
                           stellar_metallicity_key=Param(str, 'stellar_metallicity',
-                                                        msg='Stellar metallicity keyword name of the hdf5 dataset '
-                                                            'containing input galaxy properties, this is the stellar'
-                                                            ' metallicity in units of log10(Z/Zsun)'),
+                                                        msg='Stellar metallicity keyword name of the hdf5 dataset, '
+                                                            'this is the stellar metallicity in units of log10(Z)'),
                           stellar_metallicity_scatter_key=Param(str, 'stellar_metallicity_scatter',
                                                                 msg='Stellar metallicity scatter keyword name of the '
-                                                                    'hdf5 dataset containing input galaxy properties, '
-                                                                    'this is lognormal scatter in the metallicity '
-                                                                    'distribution function'),
-                          restframe_sed_key=Param(str, 'restframe_seds', msg='Rest-frame SED keyword name of the '
-                                                                             'output hdf5 dataset'))
+                                                                    'hdf5 dataset, this is lognormal scatter in the'
+                                                                    ' metallicity distribution function'),
+                          restframe_sed_key=Param(str, 'restframe_sed', msg='Rest-frame SED keyword name of the '
+                                                                            'output hdf5 dataset'),
+                          default_cosmology=Param(bool, True, msg='True to use default DSPS cosmology. If False,'
+                                                                  'Om0, w0, wa, h need to be supplied in the '
+                                                                  'fit_model function'))
 
     inputs = [("input", Hdf5Handle)]
     outputs = [("model", Hdf5Handle)]
 
     def __init__(self, args, comm=None):
         """
-        Initialize Modeler
+        Initialize SedModeler class. If the SSP templates are not provided by the user, they are automatically
+        downloaded from the public NERSC directory. These default templates are created with default FSPS values,
+        with gas emission at fixed gas solar metallicity value.
 
         Parameters
         ----------
         args:
         comm:
 
         """
         RailStage.__init__(self, args, comm=comm)
 
         if not os.path.isfile(self.config.ssp_templates_file):
-            default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data',
-                                                'dsps_default_data')
+            default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data',
+                                                  'dsps_default_data'))
             os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/ssp_data_fsps_v3.2_lgmet_age.h5 '
                       '--output-dir {}'.format(default_files_folder))
 
     def _get_rest_frame_seds(self, ssp_data, redshifts, cosmic_time_grids, star_formation_histories,
                              stellar_metallicities, stellar_metallicities_scatter):
         """
         Computes the rest-frame SED with DSPS based on user-supplied input galaxy population properties.
@@ -94,30 +98,41 @@
             SSP weights of the distribution of stellar metallicity
         age_weightsndarray of shape (n_ages, )
             SSP weights of the distribution of stellar age
 
         Parameters
         ----------
         ssp_data
+            SSP templates created with FSPS
         redshifts
+            Array of redshifts for each galaxy
         cosmic_time_grids
+            Array of ages of the universe in Gyr at which the input galaxy SFH and metallicity have been tabulated
         star_formation_histories
+            Star formation history in Msun/yr evaluated at the input cosmic_time_grids
         stellar_metallicities
+            If a scalar value, log10(Z) of the galaxy at the time of observation, else Metallicity history evaluated
+            at the input cosmic_time_grids
         stellar_metallicities_scatter
+            Lognormal scatter in metallicity
 
         Returns
         -------
-
+        restframe_seds
+            Array of rest-frame SEDs generated with DSPS for each input galaxy.
         """
 
         restframe_seds = {}
 
         for i in self.split_tasks_by_rank(range(len(redshifts))):
-            t_obs = age_at_z(redshifts[i], *DEFAULT_COSMOLOGY)  # age of the universe in Gyr at z_obs
-            t_obs = t_obs[0]
+            t_obs = age_at_z(redshifts[i], self.config.Om0, self.config.w0, self.config.wa, self.config.h)
+            if t_obs[0] > cosmic_time_grids[i][-1]:
+                t_obs = cosmic_time_grids[i][-1]
+            else:
+                t_obs = t_obs[0]
 
             if np.isscalar(stellar_metallicities[i]):
                 restframe_sed = calc_rest_sed_sfh_table_lognormal_mdf(cosmic_time_grids[i], star_formation_histories[i],
                                                                       stellar_metallicities[i],
                                                                       stellar_metallicities_scatter[i],
                                                                       ssp_data.ssp_lgmet, ssp_data.ssp_lg_age_gyr,
                                                                       ssp_data.ssp_flux, t_obs)
@@ -139,35 +154,67 @@
 
             restframe_seds = {k: v for a in restframe_seds for k, v in a.items()}
 
         restframe_seds = np.array([restframe_seds[i] for i in range(len(redshifts))])
 
         return restframe_seds
 
-    def fit_model(self):
+    def fit_model(self, input_data=os.path.join(default_files_folder, 'input_galaxy_properties_dsps.hdf5'),
+                  Om0=DEFAULT_COSMOLOGY.Om0, w0=DEFAULT_COSMOLOGY.w0, wa=DEFAULT_COSMOLOGY.wa,
+                  h=DEFAULT_COSMOLOGY.h):
         """
-        Produce a creation model from which photometry can be generated
+        This function generates the rest-frame SEDs and stores them into the Hdf5Handle.
 
         Parameters
         ----------
-        [The parameters depend entirely on the modeling approach!]
+        input_data: str
+            Filepath to the hdf5 table containing galaxy properties.
+        Om0: float
+            Omega matter: density of non-relativistic matter in units of the critical density at z=0.
+        w0: float
+            Dark energy equation of state at z=0 (a=1). This is pressure/density for dark energy in units where c=1.
+        wa: float
+            Negative derivative of the dark energy equation of state with respect to the scale factor.
+            A cosmological constant has w0=-1.0 and wa=0.0.
+        h: float
+            dimensionless Hubble constant at z=0.
 
         Returns
         -------
-        model: ModelHandle
-            ModelHandle storing the rest-frame SED model
+        model: Hdf5Handle
+            Hdf5Handle storing the rest-frame SED model
         """
+        if self.config.default_cosmology:
+            self.config.Om0 = DEFAULT_COSMOLOGY.Om0
+            self.config.w0 = DEFAULT_COSMOLOGY.w0
+            self.config.wa = DEFAULT_COSMOLOGY.wa
+            self.config.h = DEFAULT_COSMOLOGY.h
+        else:
+            self.config.Om0 = Om0
+            self.config.w0 = w0
+            self.config.wa = wa
+            self.config.h = h
+        self.set_data('input', input_data)
         self.run()
         self.finalize()
         model = self.get_handle("model")
         return model
 
     def run(self):
         """
         Run method. It Calls `_get_rest_frame_seds` from DSPS to create a galaxy rest-frame SED.
+        The load_ssp_templates function loads the SSP templates created with FSPS. The resulting NamedTuple has
+        4 entries:
+        ssp_lgmetndarray of shape (n_met, )
+            Array of log10(Z) of the SSP templates where dimensionless Z is the mass fraction of elements heavier than He
+        ssp_lg_age_gyrndarray of shape (n_ages, )
+            Array of log10(age/Gyr) of the SSP templates
+        ssp_wave : ndarray of shape (n_wave, )
+        ssp_fluxndarray of shape (n_met, n_ages, n_wave)
+            SED of the SSP in units of Lsun/Hz/Msun
 
         Notes
         -----
         The initial stellar mass of the galaxy is 0.
         The definition of the stellar mass table as cumulative sum refers to the total stellar mass formed.
         DSPS conveniently provides IMF-dependent fitting functions to compute the surviving mass
         (see surviving_mstar.py).
@@ -194,162 +241,212 @@
             rest_frame_sed_models = {self.config.restframe_sed_key: restframe_seds,
                                      self.config.redshift_key: redshifts}
             self.add_data('model', rest_frame_sed_models)
 
 
 class DSPSPopulationSedModeler(Modeler):
     r"""
-    Derived class of Modeler for creating a galaxy population rest-frame SED models using DSPS (Hearin+21).
+    Derived class of Modeler for creating a population of galaxy rest-frame SED models using DSPS v3.* (Hearin+21).
     SPS calculations are based on a set of template SEDs of simple stellar populations (SSPs).
     Supplying such templates is outside the planned scope of the DSPS package, and so they
     will need to be retrieved from some other library. For example, the FSPS library supplies
     such templates in a convenient form.
 
+    The input galaxy properties, such as star-formation histories and metallicities, need to be supplied via an
+    hdf5 table.
+
     Notes
     -----
     The user-provided metallicity grid should be consistently defined with the metallicity of the templates SEDs.
     Users should be cautious in the use of the cosmic time grid. The time resolution strongly depends on the
     user scientific aim.
     jax serially execute the computations on CPU on single core, for CPU parallelization you need MPI.
     If GPU is used, jax natively and automatically parallelize the execution.
     """
 
     name = "DSPSPopulationSedModeler"
-    default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data', 'dsps_default_data')
+    default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data', 'dsps_default_data'))
     config_options = RailStage.config_options.copy()
     config_options.update(ssp_templates_file=Param(str, os.path.join(default_files_folder,
                                                                      'ssp_data_fsps_v3.2_lgmet_age.h5'),
                                                    msg='hdf5 file storing the SSP libraries used to create SEDs'),
                           redshift_key=Param(str, 'redshift',
-                                             msg='Redshift keyword name of the hdf5 dataset containing input galaxy '
-                                                 'properties'),
+                                             msg='Redshift keyword name of the hdf5 dataset'),
                           cosmic_time_grid_key=Param(str, 'cosmic_time_grid',
-                                                     msg='Cosmic time grid keyword name of the hdf5 dataset containing '
-                                                         'input galaxy properties, this is the grid over '
-                                                         'which the stellar mass build-up takes place in units of Gyr'),
+                                                     msg='Cosmic time grid keyword name of the hdf5 dataset, '
+                                                         'this is the grid of Universe age over which the stellar mass'
+                                                         ' build-up takes place in units of Gyr'),
                           star_formation_history_key=Param(str, 'star_formation_history',
                                                            msg='Star-formation history keyword name of the hdf5 '
-                                                               'dataset containing input galaxy properties, this is '
-                                                               'the star-formation history of the galaxy in units of '
-                                                               'Msun/yr'),
+                                                               'dataset, this is the star-formation history of the'
+                                                               ' galaxy in units of Msun/yr'),
                           stellar_metallicity_key=Param(str, 'stellar_metallicity',
-                                                        msg='Stellar metallicity keyword name of the hdf5 dataset '
-                                                            'containing input galaxy properties, this is the stellar'
-                                                            ' metallicity in units of log10(Z/Zsun)'),
+                                                        msg='Stellar metallicity keyword name of the hdf5 dataset, '
+                                                            'this is the stellar metallicity in units of log10(Z)'),
                           stellar_metallicity_scatter_key=Param(str, 'stellar_metallicity_scatter',
                                                                 msg='Stellar metallicity scatter keyword name of the '
-                                                                    'hdf5 dataset containing input galaxy properties, '
-                                                                    'this is lognormal scatter in the metallicity '
-                                                                    'distribution function'),
+                                                                    'hdf5 dataset, this is lognormal scatter in the '
+                                                                    'metallicity distribution function'),
                           restframe_sed_key=Param(str, 'restframe_seds', msg='Rest-frame SED keyword name of the '
-                                                                             'output hdf5 dataset'))
+                                                                             'output hdf5 dataset'),
+                          default_cosmology = Param(bool, True, msg='True to use default DSPS cosmology. If False,'
+                                                                    'Om0, w0, wa, h need to be supplied in the '
+                                                                    'fit_model function'))
 
     inputs = [("input", Hdf5Handle)]
     outputs = [("model", Hdf5Handle)]
 
     def __init__(self, args, comm=None):
         r"""
-        Initialize Modeler.
+        Initialize SedModeler class. If the SSP templates are not provided by the user, they are automatically
+        downloaded from the public NERSC directory. These default templates are created with default FSPS values,
+        with gas emission at fixed gas solar metallicity value.
         The _a tuple for jax is composed of None or 0, depending on whether you don't or do want the
         array axis to map over for all arguments.
 
         Parameters
         ----------
         args:
         comm:
         """
 
         RailStage.__init__(self, args, comm=comm)
 
         if not os.path.isfile(self.config.ssp_templates_file):
-            default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data',
-                                                'dsps_default_data')
+            default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data',
+                                                  'dsps_default_data'))
             os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/ssp_data_fsps_v3.2_lgmet_age.h5 '
                       '--output-dir {}'.format(default_files_folder))
 
     def _get_rest_frame_seds(self, ssp_data, redshifts, cosmic_time_grids, star_formation_histories,
                              stellar_metallicities, stellar_metallicities_scatter):
         """
-        Computes the rest-frame SEDs with DSPS vmap based on user-supplied input galaxy population properties.
+        Computes the rest-frame SED with DSPS based on user-supplied input galaxy population properties.
+        The functions calc_rest_sed_sfh_table_lognormal_mdf and calc_rest_sed_sfh_table_met_table
+        return a RestSED object composed of
+        rest_sedndarray of shape (n_wave, )
+            Restframe SED of the galaxy in units of Lsun/Hz
+        weightsndarray of shape (n_met, n_ages, 1)
+            SSP weights of the joint distribution of stellar age and metallicity
+        lgmet_weightsndarray of shape (n_met, )
+            SSP weights of the distribution of stellar metallicity
+        age_weightsndarray of shape (n_ages, )
+            SSP weights of the distribution of stellar age
 
         Parameters
         ----------
         ssp_data
+            SSP templates created with FSPS
         redshifts
+            Array of redshifts for each galaxy
         cosmic_time_grids
+            Array of ages of the universe in Gyr at which the input galaxy SFH and metallicity have been tabulated
         star_formation_histories
+            Star formation history in Msun/yr evaluated at the input cosmic_time_grids
         stellar_metallicities
+            If a scalar value, log10(Z) of the galaxy at the time of observation, else Metallicity history evaluated
+            at the input cosmic_time_grids
         stellar_metallicities_scatter
+            Lognormal scatter in metallicity
 
         Returns
         -------
-
+        restframe_seds_galpop.rest_sed
+            Array of rest-frame SEDs generated with DSPS for each input galaxy.
         """
 
         # consider the whole chunk
         self._a = (0, 0, 0, 0, None, None, None, 0)
 
         if np.isscalar(stellar_metallicities[0]):
             self._calc_sed_vmap = jjit(vmap(calc_rest_sed_sfh_table_lognormal_mdf, in_axes=self._a))
         elif len(stellar_metallicities[0]) > 1:
             self._calc_sed_vmap = jjit(vmap(calc_rest_sed_sfh_table_met_table, in_axes=self._a))
         else:
             raise ValueError
 
         self._b = (0, None, None, None, None)
         self._calc_age_at_z_vmap = jjit(vmap(age_at_z, in_axes=self._b))
-        args_pop_z = (redshifts, *DEFAULT_COSMOLOGY)
+        args_pop_z = (redshifts, self.config.Om0, self.config.w0, self.config.wa, self.config.h)
         t_obs = self._calc_age_at_z_vmap(*args_pop_z)[:, 0]
 
         args_pop = (cosmic_time_grids, star_formation_histories, stellar_metallicities,
                     stellar_metallicities_scatter, ssp_data.ssp_lgmet, ssp_data.ssp_lg_age_gyr, ssp_data.ssp_flux,
                     t_obs)
 
         restframe_seds_galpop = self._calc_sed_vmap(*args_pop)
 
         return restframe_seds_galpop.rest_sed
 
-    def fit_model(self):
+    def fit_model(self, input_data=os.path.join(default_files_folder, 'input_galaxy_properties_dsps.hdf5'),
+                  Om0=DEFAULT_COSMOLOGY.Om0, w0=DEFAULT_COSMOLOGY.w0, wa=DEFAULT_COSMOLOGY.wa,
+                  h=DEFAULT_COSMOLOGY.h):
         """
-        Produce a creation model from which photometry can be generated
+        This function generates the rest-frame SEDs and stores them into the Hdf5Handle.
 
         Parameters
         ----------
-        [The parameters depend entirely on the modeling approach!]
+        input_data: str
+            Filepath to the hdf5 table containing galaxy properties.
+        Om0: float
+            Omega matter: density of non-relativistic matter in units of the critical density at z=0.
+        w0: float
+            Dark energy equation of state at z=0 (a=1). This is pressure/density for dark energy in units where c=1.
+        wa: float
+            Negative derivative of the dark energy equation of state with respect to the scale factor.
+            A cosmological constant has w0=-1.0 and wa=0.0.
+        h: float
+            dimensionless Hubble constant at z=0.
 
         Returns
         -------
-        model: ModelHandle
-            ModelHandle storing the rest-frame SED models
+        model: Hdf5Handle
+            Hdf5Handle storing the rest-frame SED model
         """
-
+        if self.config.default_cosmology:
+            self.config.Om0 = DEFAULT_COSMOLOGY.Om0
+            self.config.w0 = DEFAULT_COSMOLOGY.w0
+            self.config.wa = DEFAULT_COSMOLOGY.wa
+            self.config.h = DEFAULT_COSMOLOGY.h
+        else:
+            self.config.Om0 = Om0
+            self.config.w0 = w0
+            self.config.wa = wa
+            self.config.h = h
+        self.set_data('input', input_data)
         self.run()
         self.finalize()
         model = self.get_handle("model")
         return model
 
     def run(self):
         """
-        Run method
-
-        Calls `_get_rest_frame_seds` from DSPS to create galaxy rest-frame SEDs for a galaxy population.
+        Run method. It Calls `_get_rest_frame_seds` from DSPS to create rest-frame SEDs for a population of galaxies.
+        The load_ssp_templates function loads the SSP templates created with FSPS. The resulting NamedTuple has
+        4 entries:
+        ssp_lgmetndarray of shape (n_met, )
+            Array of log10(Z) of the SSP templates where dimensionless Z is the mass fraction of elements heavier than He
+        ssp_lg_age_gyrndarray of shape (n_ages, )
+            Array of log10(age/Gyr) of the SSP templates
+        ssp_wave : ndarray of shape (n_wave, )
+        ssp_fluxndarray of shape (n_met, n_ages, n_wave)
+            SED of the SSP in units of Lsun/Hz/Msun
 
         Notes
         -----
+        The initial stellar mass of the galaxy is 0.
         The definition of the stellar mass table as cumulative sum refers to the total stellar mass formed.
         DSPS conveniently provides IMF-dependent fitting functions to compute the surviving mass
         (see surviving_mstar.py).
-        The units of the resulting rest-frame SEDs are solar luminosity per Hertz. The luminosity refers to that
+        The units of the resulting rest-frame SED is solar luminosity per Hertz. The luminosity refers to that
         emitted by the formed mass at the time of observation.
 
         Returns
         -------
-
         """
-
         input_galaxy_properties = self.get_data('input')
         ssp_data = load_ssp_templates(fn=self.config.ssp_templates_file)
 
         redshifts = input_galaxy_properties[self.config.redshift_key][()]
         cosmic_time_grids = input_galaxy_properties[self.config.cosmic_time_grid_key][()]
         star_formation_histories = input_galaxy_properties[self.config.star_formation_history_key][()]
         stellar_metallicities = input_galaxy_properties[self.config.stellar_metallicity_key][()]
```

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5` & `pz_rail_dsps-0.0.3/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.2/tests/dsps/test_dsps_interface.py` & `pz_rail_dsps-0.0.3/tests/dsps/test_dsps_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import subprocess
 
 import numpy as np
 import h5py
 import pytest
 
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.core.utils import find_rail_file
 from src.rail.creation.engines.dsps_photometry_creator import DSPSPhotometryCreator
 from src.rail.creation.engines.dsps_sed_modeler import DSPSPopulationSedModeler, DSPSSingleSedModeler
 
-default_files_folder = os.path.join(RAILDIR, 'rail', 'examples_data', 'creation_data', 'data', 'dsps_default_data')
+default_files_folder = find_rail_file(os.path.join('examples_data', 'creation_data', 'data', 'dsps_default_data'))
 
 
 def create_testdata(files_folder):
     """
 
     Parameters
     ----------
@@ -84,15 +84,14 @@
 
     Returns
     -------
 
     """
 
     trainFile = create_testdata(default_files_folder)
-
     DS = RailStage.data_store
     DS.__class__.allow_overwrite = True
 
     single_sed_model = DSPSSingleSedModeler.make_stage(name='DSPS_single_SED_model',
                                                        ssp_templates_file=
                                                        os.path.join(default_files_folder,
                                                                     'ssp_data_fsps_v3.2_lgmet_age.h5'),
```

