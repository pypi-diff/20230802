# Comparing `tmp/reaxpro-wrappers-1.2.0.tar.gz` & `tmp/reaxpro-wrappers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.2.0.tar", last modified: Thu Jul 27 10:26:28 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.3.0.tar", last modified: Wed Aug  2 12:12:45 2023, max compression
```

## Comparing `reaxpro-wrappers-1.2.0.tar` & `reaxpro-wrappers-1.3.0.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/energy_landscape.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49183 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    77122 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-27 10:26:28.403791 reaxpro-wrappers-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.520789 reaxpro-wrappers-1.3.0/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.520789 reaxpro-wrappers-1.3.0/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/co_pt111_meso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/energy_landscape.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/ams/pesexploration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.524789 reaxpro-wrappers-1.3.0/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/multiscale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/multiscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/multiscale/co_pt111_meso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49172 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75884 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.528789 reaxpro-wrappers-1.3.0/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 12:12:45.000000 reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:12:45.532789 reaxpro-wrappers-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-02 12:12:27.000000 reaxpro-wrappers-1.3.0/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.2.0/LICENSE` & `reaxpro-wrappers-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/PKG-INFO` & `reaxpro-wrappers-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.2.0
+Version: 1.3.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.2.0/README.md` & `reaxpro-wrappers-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.3.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.3.0/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.3.0/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.3.0/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.3.0/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/models/settings/general.py` & `reaxpro-wrappers-1.3.0/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/models/utils/general.py` & `reaxpro-wrappers-1.3.0/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.3.0/osp/models/zacros/co_pyzacros.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from pathlib import Path
 import tempfile
 from typing import TYPE_CHECKING, List, Union, Optional
 from uuid import UUID
 import warnings
 
-from arcp import arcp_random, arcp_name
+from arcp import arcp_random
 from pydantic import AnyUrl, BaseModel, Field, root_validator, confloat, conlist, conint
 from pydantic.dataclasses import dataclass
 from urllib.parse import quote, urlencode
 
 
 from osp.core.cuds import Cuds
 from osp.core.namespaces import emmo, crystallography
```

### Comparing `reaxpro-wrappers-1.2.0/osp/tools/io_functions.py` & `reaxpro-wrappers-1.3.0/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.3.0/osp/tools/mapping_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from scm.plams import Settings as PlamsSettings
 from scm.plams import Molecule as PlamsMolecule
 from scm.plams import Atom as PlamsAtom
 from arcp import arcp_random
 from osp.tools.io_functions import raise_error, raise_warning
 from osp.tools.io_functions import read_mechanism, read_cluster_expansion, read_molecule
 from osp.tools.set_functions import AMS_default_setting
+from osp.models.utils.general import get_upload
 from osp.core.utils import simple_search as search
 from osp.core.ontology.oclass import OntologyClass
 from osp.core.cuds import Cuds
 from osp.core.namespaces import emmo, crystallography, cuba
 from osp.core.utils import pretty_print
 from typing import List
-
+from uuid import UUID
 
 def map_function(self, root_cuds_object: Cuds, engine=None) -> tuple:
     """
     Map a Calculations CUDS object to a engine-understandable input.
 
     :param root_cuds_object: Calculation CUDS object.
 
@@ -39,27 +40,15 @@
         search_landscape = \
             search.find_cuds_objects_by_oclass(emmo.EnergyLandscape, root_cuds_object, emmo.hasPart)
 
         if search_landscape:
             plams_molecule = map_PLAMSLandscape(search_landscape[0])
 
         else:
-            search_molecule = \
-                search.find_cuds_objects_by_oclass(emmo.MolecularGeometry, root_cuds_object, emmo.hasPart)
-
-            if len(search_molecule) > 1:
-                raise_error(file=os.path.basename(__file__),
-                            function=map_function.__name__,
-                            type='ValueError',
-                            message='More than one emmo.MolecularGeometry defined in the Wrapper object.')
-            elif not search_molecule:
-                raise_error(file=os.path.basename(__file__), function=map_molecule.__name__,
-                            type='ValueError', message='Molecule CUDS object missed in the wrapper.')
-            else:
-                plams_molecule = map_PLAMSMolecule(search_molecule[0])
+            plams_molecule = map_PLAMSMolecule(root_cuds_object)
 
         plams_settings = map_PLAMSSettings(root_cuds_object)
 
         return (plams_molecule, plams_settings)
 
     elif engine == "Zacros":
 
@@ -269,23 +258,35 @@
      "atom_coordinates":
                     [[coordinate_x_1, coordinate_y_1, coordinate_z_1, (region)],
                     [coordinate_x_2, coordinate_y_2, coordinate_z_2, (region)],
                      ...
                     [coordinate_x_2, coordinate_y_n, coordinate_z_n, (region)]]
     }
 
-    :param root_cuds_object: CUDS MolecularGeometry to be checked.
+    :param root_cuds_object: CUDS root_cuds_object to be checked.
 
     :return str: If a Molecule object is present, return dictionary with
                  atom labels and positions. Otherwise, raise an error.
     """
-    molecule_data = {}
 
+    search_molecule = \
+        search.find_cuds_objects_by_oclass(emmo.MolecularGeometry, root_cuds_object, emmo.hasPart)
+
+    if len(search_molecule) > 1:
+        raise_error(file=os.path.basename(__file__),
+                    function=map_function.__name__,
+                    type='ValueError',
+                    message='More than one emmo.MolecularGeometry defined in the Wrapper object.')
+    elif not search_molecule:
+        raise_error(file=os.path.basename(__file__), function=map_molecule.__name__,
+                    type='ValueError', message='Molecule CUDS object missed in the wrapper.')
+
+    molecule_data = {}
     # Looking for atoms:
-    first = root_cuds_object.get(rel=emmo.hasSpatialFirst)
+    first = search_molecule.pop().get(rel=emmo.hasSpatialFirst)
     if len(first) > 1:
         raise_error(file=os.path.basename(__file__),
                     function=map_molecule.__name__,
                     type='ValueError',
                     message='More than one first spatial atom found in molecule.')
     elif len(first) == 0:
         raise_error(file=os.path.basename(__file__),
@@ -1517,37 +1518,32 @@
 
 def map_energies(root_cuds_object: Cuds) -> list:
     """
     Gather a list of three TotalElectronicEnergy values from a cuba.Wrapper
     object.
     """
 
+    calculations = []
     electronic_energies = []
     electronic_energy_values = []
     search_simulation = \
         search.find_cuds_object(criterion=lambda x: x.is_a(oclass=emmo.Simulation),
                                 root=root_cuds_object, rel=emmo.hasPart,
                                 find_all=True, max_depth=1)
 
     if not len(search_simulation):
         return
-
-    first_calculation = search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalFirst,
-                                                  root=search_simulation[0],
-                                                  consider_rel=emmo.EMMORelation)
-
-    next_calculation = search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalNext,
-                                                 root=search_simulation[0],
-                                                 consider_rel=emmo.hasTemporalNext)
-
-    last_calculation = search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalLast,
-                                                 root=search_simulation[0],
-                                                 consider_rel=emmo.hasTemporalLast)
-    calculations = \
-        first_calculation + next_calculation + last_calculation
+    
+    # First
+    next_calc = search_simulation[0].get(rel=emmo.hasSpatialFirst)
+
+    while next_calc:
+        current = next_calc.pop()
+        calculations.append(current)
+        next_calc = current.get(rel=emmo.hasSpatialNext)
 
     for calculation in calculations:
 
         electronic_energy = \
             search.find_cuds_objects_by_oclass(oclass=emmo.TotalElectronicEnergy,
                                                root=calculation, rel=emmo.hasOutput)
         electronic_energies += electronic_energy
@@ -1623,50 +1619,43 @@
             elif map_calculation_type(root_cuds_object) == "BindingSites":
 
                 # Attach UnitCell() with file path to Wrapper object as Output:
                 loader_bs = pz.RKFLoader(engine.children[0].results)
                 loader_bs.replace_site_types(['A', 'B', 'C'], ['fcc', 'br', 'hcp'])
                 loader_bs.lattice.set_repeat_cell((10, 10))
                 loader_bs.lattice.plot()
-                lattice_file = open("lattice_input.dat", "a")
-                lattice_file.write(str(loader_bs.lattice))
-                iri = arcp_random("./lattice_input.dat")
-                lattice_output = crystallography.UnitCell(iri=iri)
+                
+                file = os.path.join(engine.path, "lattice_input.dat")
+                with open(file, "w+") as lattice_file:
+                    lattice_file.write(str(loader_bs.lattice))
+                uuid = get_upload(file)
+                lattice_output = crystallography.UnitCell(uid=UUID(uuid))
                 search_calculation[0].add(lattice_output, rel=emmo.hasOutput)
 
             elif map_calculation_type(root_cuds_object) == "LandscapeRefinement":
                 add_AMSLandscape_to_object(engine.children[0], search_calculation[0])
 
             # TODO elif map_calculation_type(root_cuds_object) == "XXXX":
 
         else:
             if (map_calculation_type(root_cuds_object) == "WavefunctionOptimization") \
                or (map_calculation_type(root_cuds_object) == "GeometryOptimization"):
 
                 # First
-                first_calculation = search.find_relationships(
-                    find_rel=emmo.INVERSE_OF_hasTemporalFirst, root=search_simulation[0],
-                    consider_rel=emmo.EMMORelation)
-                add_AMSenergy_to_object(engine.children[0], first_calculation[0])
-
-                # Next
-                next_calculation = \
-                    search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalNext,
-                                              root=search_simulation[0],
-                                              consider_rel=emmo.hasTemporalNext)
-                add_AMSenergy_to_object(engine.children[1], next_calculation[0])
-
-                # Last
-                last_calculation = \
-                    search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalLast,
-                                              root=search_simulation[0],
-                                              consider_rel=emmo.hasTemporalLast)
-                add_AMSenergy_to_object(engine.children[2], last_calculation[0])
+                next_calc = search_simulation[0].get(rel=emmo.hasSpatialFirst)
+                i = 0
+
+                while next_calc:
+                    
+                    current = next_calc.pop()
+                    add_AMSenergy_to_object(engine.children[i], current)
+                    i += 1
+                    next_calc = current.get(rel=emmo.hasSpatialNext)
 
-            tarball = map_tarball(engine, last_calculation[0])
+            tarball = map_tarball(engine, current)
 
     elif isinstance(engine, pz.ZacrosJob):
         search_calculation = search.find_cuds_objects_by_oclass(
                                    emmo.MesoscopicCalculation, root_cuds_object,
                                    rel=cuba.relationship)
         tarball = map_tarball(engine, search_calculation[0])
```

### Comparing `reaxpro-wrappers-1.2.0/osp/tools/set_functions.py` & `reaxpro-wrappers-1.3.0/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.3.0/osp/wrappers/simams/simams_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.3.0/osp/wrappers/simzacros/simzacros_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.2.0
+Version: 1.3.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.3.0/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 README.md
 setup.cfg
 setup.py
 osp/__init__.py
 osp/dictionaries/__init__.py
 osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
 osp/dictionaries/ams/__init__.py
+osp/dictionaries/ams/co_pt111_meso.json
 osp/dictionaries/ams/energy_landscape.json
+osp/dictionaries/ams/pesexploration.json
 osp/dictionaries/defaults/__init__.py
 osp/dictionaries/defaults/defaults_AMS.yaml
 osp/dictionaries/energies/gas_energies.yaml
+osp/dictionaries/example_data/CO_ads+Pt111.xyz
 osp/dictionaries/example_data/__init__.py
 osp/dictionaries/example_data/lattice_input.dat
 osp/dictionaries/example_data/state1.xyz
 osp/dictionaries/example_data/state2.xyz
 osp/dictionaries/example_data/state3.xyz
 osp/dictionaries/example_data/state4.xyz
 osp/dictionaries/example_data/state5.xyz
 osp/models/__init__.py
 osp/models/ams/__init__.py
 osp/models/ams/energy_landscape_refinement.py
+osp/models/multiscale/__init__.py
+osp/models/multiscale/co_pt111_meso.py
 osp/models/settings/__init__.py
 osp/models/settings/general.py
 osp/models/utils/__init__.py
 osp/models/utils/general.py
 osp/models/zacros/__init__.py
 osp/models/zacros/co_pyzacros.py
 osp/tools/__init__.py
```

### Comparing `reaxpro-wrappers-1.2.0/setup.cfg` & `reaxpro-wrappers-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.2.0
+version = v1.3.0
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.2.0/setup.py` & `reaxpro-wrappers-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.3.0/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/tests/test_examples.py` & `reaxpro-wrappers-1.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.3.0/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.2.0/tests/test_tools.py` & `reaxpro-wrappers-1.3.0/tests/test_tools.py`

 * *Files identical despite different names*

