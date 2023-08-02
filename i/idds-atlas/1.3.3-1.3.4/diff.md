# Comparing `tmp/idds-atlas-1.3.3.tar.gz` & `tmp/idds-atlas-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-atlas-1.3.3.tar", last modified: Fri Jul 21 07:10:57 2023, max compression
+gzip compressed data, was "idds-atlas-1.3.4.tar", last modified: Wed Aug  2 09:00:10 2023, max compression
```

## Comparing `idds-atlas-1.3.3.tar` & `idds-atlas-1.3.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.404868 idds-atlas-1.3.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.404868 idds-atlas-1.3.3/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/notifier/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/activelearning_condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/activelearning_condor_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/condor_submitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2495 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/stagein_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/processing/stagein_submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/rucio/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/collection_lister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/collection_metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/contents_lister.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/contents_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/transformer/activelearning_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/transformer/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/transformer/hyperparameteropt_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/transformer/stagein_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:10:52.000000 idds-atlas-1.3.3/lib/idds/atlas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.408867 idds-atlas-1.3.3/lib/idds/atlas/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasactuatorwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlascondorwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasdagwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlashpowork.py
--rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlaslocalpandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasstageinwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasactuatorwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlascondorwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasdagwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    35429 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlashpowork.py
--rw-r--r--   0 runner    (1001) docker     (123)    21763 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlaslocalpandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasstageinwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/lib/idds_atlas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 07:10:57.000000 idds-atlas-1.3.3/lib/idds_atlas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-21 07:10:57.000000 idds-atlas-1.3.3/lib/idds_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:10:57.000000 idds-atlas-1.3.3/lib/idds_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 07:10:57.000000 idds-atlas-1.3.3/lib/idds_atlas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 07:10:57.000000 idds-atlas-1.3.3/lib/idds_atlas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-21 07:10:42.000000 idds-atlas-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.404868 idds-atlas-1.3.3/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:57.412867 idds-atlas-1.3.3/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-21 07:10:52.000000 idds-atlas-1.3.3/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/lib/idds/atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/lib/idds/atlas/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/notifier/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/lib/idds/atlas/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/activelearning_condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/activelearning_condor_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/condor_submitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2495 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/stagein_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/processing/stagein_submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/lib/idds/atlas/rucio/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/collection_lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/collection_metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/contents_lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/contents_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/lib/idds/atlas/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/transformer/activelearning_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/transformer/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/transformer/hyperparameteropt_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/transformer/stagein_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:00:05.000000 idds-atlas-1.3.4/lib/idds/atlas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/lib/idds/atlas/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasactuatorwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlascondorwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasdagwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlashpowork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlaslocalpandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasstageinwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasactuatorwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlascondorwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasdagwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35429 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlashpowork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21763 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlaslocalpandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasstageinwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/lib/idds_atlas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 09:00:10.000000 idds-atlas-1.3.4/lib/idds_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-02 09:00:10.000000 idds-atlas-1.3.4/lib/idds_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:00:10.000000 idds-atlas-1.3.4/lib/idds_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 09:00:10.000000 idds-atlas-1.3.4/lib/idds_atlas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 09:00:10.000000 idds-atlas-1.3.4/lib/idds_atlas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-02 08:59:54.000000 idds-atlas-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.097497 idds-atlas-1.3.4/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:10.101498 idds-atlas-1.3.4/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-02 09:00:05.000000 idds-atlas-1.3.4/tools/env/environment.yml
```

### Comparing `idds-atlas-1.3.3/LICENSE.rst` & `idds-atlas-1.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/PKG-INFO` & `idds-atlas-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-atlas
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/notifier/messaging.py` & `idds-atlas-1.3.4/lib/idds/atlas/notifier/messaging.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/activelearning_condor_poller.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/activelearning_condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/activelearning_condor_submitter.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/activelearning_condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/base_plugin.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/condor_poller.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/condor_submitter.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_bayesian.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_bayesian.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_condor_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_condor_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/hyperparameteropt_nevergrad.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/stagein_poller.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/stagein_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/processing/stagein_submitter.py` & `idds-atlas-1.3.4/lib/idds/atlas/processing/stagein_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/base_plugin.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/collection_lister.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/collection_lister.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/collection_metadata_reader.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/collection_metadata_reader.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/contents_lister.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/contents_lister.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/contents_register.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/contents_register.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_creator.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_creator.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_poller.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_poller.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/rucio/rule_submitter.py` & `idds-atlas-1.3.4/lib/idds/atlas/rucio/rule_submitter.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/transformer/activelearning_transformer.py` & `idds-atlas-1.3.4/lib/idds/atlas/transformer/activelearning_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/transformer/base_plugin.py` & `idds-atlas-1.3.4/lib/idds/atlas/transformer/base_plugin.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/transformer/hyperparameteropt_transformer.py` & `idds-atlas-1.3.4/lib/idds/atlas/transformer/hyperparameteropt_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/transformer/stagein_transformer.py` & `idds-atlas-1.3.4/lib/idds/atlas/transformer/stagein_transformer.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasactuatorwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasactuatorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlascondorwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlascondorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasdagwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasdagwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlashpowork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlashpowork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlaslocalpandawork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlaslocalpandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlaspandawork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflow/atlasstageinwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflow/atlasstageinwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasactuatorwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasactuatorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlascondorwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlascondorwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasdagwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasdagwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlashpowork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlashpowork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlaslocalpandawork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlaslocalpandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlaspandawork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds/atlas/workflowv2/atlasstageinwork.py` & `idds-atlas-1.3.4/lib/idds/atlas/workflowv2/atlasstageinwork.py`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/lib/idds_atlas.egg-info/PKG-INFO` & `idds-atlas-1.3.4/lib/idds_atlas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-atlas
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-atlas-1.3.3/lib/idds_atlas.egg-info/SOURCES.txt` & `idds-atlas-1.3.4/lib/idds_atlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-atlas-1.3.3/setup.py` & `idds-atlas-1.3.4/setup.py`

 * *Files identical despite different names*

