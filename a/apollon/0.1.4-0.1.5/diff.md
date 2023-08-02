# Comparing `tmp/apollon-0.1.4.tar.gz` & `tmp/apollon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollon-0.1.4.tar", last modified: Sun Jul 30 09:34:33 2023, max compression
+gzip compressed data, was "apollon-0.1.5.tar", last modified: Wed Aug  2 09:01:53 2023, max compression
```

## Comparing `apollon-0.1.4.tar` & `apollon-0.1.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.769096 apollon-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-30 09:34:16.000000 apollon-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-30 09:34:16.000000 apollon-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-30 09:34:16.000000 apollon-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-30 09:34:33.769096 apollon-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-30 09:34:16.000000 apollon-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-30 09:34:16.000000 apollon-0.1.4/include/cdim.h
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-30 09:34:16.000000 apollon-0.1.4/include/correlogram.h
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 09:34:16.000000 apollon-0.1.4/include/distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-30 09:34:16.000000 apollon-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 09:34:33.769096 apollon-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-30 09:34:16.000000 apollon-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/src/apollon/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/aplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/fractal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/io/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/onsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/_features_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/cdim.c
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/correlogram.c
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/critical_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/som/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/_distance_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/distance.c
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/som.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/topologies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.769096 apollon-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_onsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.898969 apollon-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 09:01:40.000000 apollon-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 09:01:40.000000 apollon-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 09:01:40.000000 apollon-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-02 09:01:53.898969 apollon-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 09:01:40.000000 apollon-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.890969 apollon-0.1.5/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 09:01:40.000000 apollon-0.1.5/include/cdim.h
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-02 09:01:40.000000 apollon-0.1.5/include/correlogram.h
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 09:01:40.000000 apollon-0.1.5/include/distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-02 09:01:40.000000 apollon-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:01:53.898969 apollon-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 09:01:40.000000 apollon-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.890969 apollon-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.890969 apollon-0.1.5/src/apollon/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/aplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/fractal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/src/apollon/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/hmm/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/hmm/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/src/apollon/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/onsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/src/apollon/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/_features_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/cdim.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/correlogram.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/critical_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/signal/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/src/apollon/som/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/_distance_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/distance.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/som.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/topologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/som/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-02 09:01:40.000000 apollon-0.1.5/src/apollon/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/src/apollon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-02 09:01:53.000000 apollon-0.1.5/src/apollon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-02 09:01:53.000000 apollon-0.1.5/src/apollon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:01:53.000000 apollon-0.1.5/src/apollon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 09:01:53.000000 apollon-0.1.5/src/apollon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:01:53.000000 apollon-0.1.5/src/apollon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:01:53.894969 apollon-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_onsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 09:01:40.000000 apollon-0.1.5/tests/test_tools.py
```

### Comparing `apollon-0.1.4/CONTRIBUTING.md` & `apollon-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/LICENSE.txt` & `apollon-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/PKG-INFO` & `apollon-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Feature extraction frame work for content-based music analysis
 Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Michael Blaß 
         All rights reserved.
         
@@ -29,48 +29,53 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Repository, http://github.com/ifsm/apollo
+Project-URL: Repository, http://github.com/ifsm/apollon
 Project-URL: Documentation, https://apollon.readthedocs.io
 Keywords: music,analysis,feature extraction
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+[![tests](https://github.com/ifsm/apollon/actions/workflows/tests.yml/badge.svg)](
+https://github.com/ifsm/apollon/actions/workflows/tests.yml)
+
 # Apollon
 Apollon is a Python framework for audio feature extraction and music similarity
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
 ### 1.1 Install from PyPI
 The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
-pip install apollon 
+pip install apollon
 ```
 
 We currently provide wheels for macOS and Windows; GNU/Linux users have to
 build apollon from source.
 
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.4/README.md` & `apollon-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+[![tests](https://github.com/ifsm/apollon/actions/workflows/tests.yml/badge.svg)](
+https://github.com/ifsm/apollon/actions/workflows/tests.yml)
+
 # Apollon
 Apollon is a Python framework for audio feature extraction and music similarity
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
 ### 1.1 Install from PyPI
 The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
-pip install apollon 
+pip install apollon
 ```
 
 We currently provide wheels for macOS and Windows; GNU/Linux users have to
 build apollon from source.
 
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.4/include/cdim.h` & `apollon-0.1.5/include/cdim.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/include/correlogram.h` & `apollon-0.1.5/include/correlogram.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/pyproject.toml` & `apollon-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [project]
 name = "apollon"
-version = "0.1.4"
+version = "0.1.5"
 description = "Feature extraction frame work for content-based music analysis"
 authors = [ {name="Michael Blaß", email="mblass@posteo.net"} ]
 license = { file="LICENSE.txt" }
 readme = "README.md"
 keywords = ["music", "analysis", "feature extraction"]
 classifiers = [
 	"License :: OSI Approved :: BSD License",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3 :: Only",
 	"Programming Language :: Python :: Implementation :: CPython",
 	"Topic :: Scientific/Engineering",
 	"Topic :: Multimedia :: Sound/Audio :: Analysis",
 	"Intended Audience :: Science/Research",
 	"Intended Audience :: Information Technology",
 	"License :: OSI Approved :: BSD License",
@@ -28,13 +30,13 @@
 	"matplotlib >= 2",
 	"pandas >= 0.20",
 	"soundfile >= 0.10.2",
 	"chainsaddiction >= 0.2.1",
 ]
 
 [project.urls]
-Repository = "http://github.com/ifsm/apollo"
+Repository = "http://github.com/ifsm/apollon"
 Documentation = "https://apollon.readthedocs.io"
 
 [build-system]
 requires = ["setuptools", "numpy"]
 build-backend = "setuptools.build_meta"
```

### Comparing `apollon-0.1.4/setup.py` & `apollon-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/_defaults.py` & `apollon-0.1.5/src/apollon/_defaults.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/aplot.py` & `apollon-0.1.5/src/apollon/aplot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/audio.py` & `apollon-0.1.5/src/apollon/audio.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/container.py` & `apollon-0.1.5/src/apollon/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/datasets.py` & `apollon-0.1.5/src/apollon/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/fractal.py` & `apollon-0.1.5/src/apollon/fractal.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/hmm/poisson.py` & `apollon-0.1.5/src/apollon/hmm/poisson.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/hmm/utilities.py` & `apollon-0.1.5/src/apollon/hmm/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/io/io.py` & `apollon-0.1.5/src/apollon/io/io.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/io/json.py` & `apollon-0.1.5/src/apollon/io/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
     schema_path = 'schema/' + schema_name + SCHEMA_EXT
     if pkg_resources.resource_exists('apollon', schema_path):
         schema = pkg_resources.resource_string('apollon', schema_path)
         schema = json.loads(schema)
         jsonschema.Draft7Validator.check_schema(schema)
         return schema
-    raise IOError(f'Schema ``{schema_path.name}`` not found.')
+    raise IOError(f'Schema ``{schema_path}`` not found.')
 
 
 def dump(obj: Any, path: PathType) -> None:
     """Write ``obj`` to JSON file.
 
     This function can handel numpy arrays.
```

### Comparing `apollon-0.1.4/src/apollon/onsets.py` & `apollon-0.1.5/src/apollon/onsets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/segment.py` & `apollon-0.1.5/src/apollon/segment.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/_features_module.c` & `apollon-0.1.5/src/apollon/signal/_features_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/cdim.c` & `apollon-0.1.5/src/apollon/signal/cdim.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/container.py` & `apollon-0.1.5/src/apollon/signal/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/correlogram.c` & `apollon-0.1.5/src/apollon/signal/correlogram.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/critical_bands.py` & `apollon-0.1.5/src/apollon/signal/critical_bands.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/features.py` & `apollon-0.1.5/src/apollon/signal/features.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 |  Licensed under the terms of the BSD-3-Clause license.
 |  Copyright (C) 2019 Michael Blaß
 |  mblass[at]posteo[dot]net
 """
 
 import numpy as _np
 from scipy.signal import hilbert as _hilbert
+from scipy.signal import correlate
 from typing import Optional
 
 import _features
 from . import tools as _sigtools
 from .. import segment as _segment
 from .. import tools
 from .. types import Array as _Array
@@ -393,18 +394,42 @@
     """
     cbrs = _cb.filter_bank(frqs) @ bins
     return _cb.total_loudness(cbrs)
 
 
 def roughness_helmholtz(d_frq: float, bins: _Array, frq_max: float,
                         total: bool = True) -> _Array:
+    """Estimate perceived audiotory roughness.
+
+    Args:
+        d_frq:      Spacing of FFT bins
+        bins:       Absolute values of FFT bins
+        frq_max:    Upper frequency threshold
+        total:      If ``True``, compute total roughness. Default ``True``.
+
+    Returns:
+        Auditory roughness as 2-D array.
+    """
     kernel = _roughnes_kernel(d_frq, frq_max)
     out = _np.empty((kernel.size, bins.shape[1]))
     for i, bin_slice in enumerate(bins.T):
-        out[:, i] = _np.correlate(bin_slice, kernel, mode='same')
+        bin_slice = bin_slice[:kernel.size]
+        bin_max = bin_slice.max()
+        if bin_max > 0:
+            bin_slice /= bin_max
+        bin_slice[bin_slice<0.1] = 0
+        rns = correlate(bin_slice, bin_slice)
+        rns = rns[rns.size//2:]
+        rns[0] = 0
+        rns_max = rns.max()
+        if rns_max > 0:
+            rns /= rns_max
+            out[:, i] = rns * kernel / sum(rns>0.2)
+        else:
+            out[:, i] = rns * kernel
 
     if total is True:
         out = out.sum(axis=0, keepdims=True)
     return out
 
 
 def sharpness(frqs: _Array, bins: _Array) -> _Array:
@@ -433,21 +458,21 @@
     """
     total_power = tools.fsum(bins, axis=0, keepdims=True)
     total_power[total_power == 0] = 1
     return bins / total_power
 
 
 def _roughnes_kernel(frq_res: float, frq_max: float) -> _Array:
-    """Comput the convolution kernel for roughness computation.
+    """Compute the weights of the convolution of roughness computation.
 
     Args:
-        frq_res:    Frequency resolution
+        frq_res:    Frequency resolution.
         frq_max:    Frequency bound.
 
     Returns:
         Weight for each frequency below ``frq_max``.
     """
-    frm = 33.5
+    frm = 33
     bin_idx = int(_np.round(frq_max/frq_res))
     norm = frm * _np.exp(-1)
-    base = _np.abs(_np.arange(-bin_idx, bin_idx+1)) * frq_res
+    base = _np.abs(_np.arange(bin_idx+1)) * frq_res
     return base / norm * _np.exp(-base/frm)
```

### Comparing `apollon-0.1.4/src/apollon/signal/filter.py` & `apollon-0.1.5/src/apollon/signal/filter.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/spectral.py` & `apollon-0.1.5/src/apollon/signal/spectral.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/signal/tools.py` & `apollon-0.1.5/src/apollon/signal/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/_distance_module.c` & `apollon-0.1.5/src/apollon/som/_distance_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/datasets.py` & `apollon-0.1.5/src/apollon/som/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/distance.c` & `apollon-0.1.5/src/apollon/som/distance.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/neighbors.py` & `apollon-0.1.5/src/apollon/som/neighbors.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/plot.py` & `apollon-0.1.5/src/apollon/som/plot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/som.py` & `apollon-0.1.5/src/apollon/som/som.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/topologies.py` & `apollon-0.1.5/src/apollon/som/topologies.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/som/utilities.py` & `apollon-0.1.5/src/apollon/som/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/tools.py` & `apollon-0.1.5/src/apollon/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon/types.py` & `apollon-0.1.5/src/apollon/types.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/src/apollon.egg-info/PKG-INFO` & `apollon-0.1.5/src/apollon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Feature extraction frame work for content-based music analysis
 Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Michael Blaß 
         All rights reserved.
         
@@ -29,48 +29,53 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Repository, http://github.com/ifsm/apollo
+Project-URL: Repository, http://github.com/ifsm/apollon
 Project-URL: Documentation, https://apollon.readthedocs.io
 Keywords: music,analysis,feature extraction
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+[![tests](https://github.com/ifsm/apollon/actions/workflows/tests.yml/badge.svg)](
+https://github.com/ifsm/apollon/actions/workflows/tests.yml)
+
 # Apollon
 Apollon is a Python framework for audio feature extraction and music similarity
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
 ### 1.1 Install from PyPI
 The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
-pip install apollon 
+pip install apollon
 ```
 
 We currently provide wheels for macOS and Windows; GNU/Linux users have to
 build apollon from source.
 
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.4/src/apollon.egg-info/SOURCES.txt` & `apollon-0.1.5/src/apollon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_audio.py` & `apollon-0.1.5/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_container.py` & `apollon-0.1.5/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_io.py` & `apollon-0.1.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_onsets.py` & `apollon-0.1.5/tests/test_onsets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_schema.py` & `apollon-0.1.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.4/tests/test_segment.py` & `apollon-0.1.5/tests/test_segment.py`

 * *Files identical despite different names*

