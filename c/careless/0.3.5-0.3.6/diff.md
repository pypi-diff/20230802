# Comparing `tmp/careless-0.3.5.tar.gz` & `tmp/careless-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.5.tar", last modified: Mon Jul 24 01:00:40 2023, max compression
+gzip compressed data, was "careless-0.3.6.tar", last modified: Wed Aug  2 19:08:11 2023, max compression
```

## Comparing `careless-0.3.5.tar` & `careless-0.3.6.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 01:00:26.000000 careless-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 01:00:26.000000 careless-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 01:00:40.425135 careless-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-07-24 01:00:26.000000 careless-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 01:00:26.000000 careless-0.3.5/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 01:00:26.000000 careless-0.3.5/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-24 01:00:26.000000 careless-0.3.5/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-24 01:00:26.000000 careless-0.3.5/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-24 01:00:26.000000 careless-0.3.5/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/prior_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-24 01:00:26.000000 careless-0.3.5/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-24 01:00:26.000000 careless-0.3.5/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 01:00:40.425135 careless-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 01:00:26.000000 careless-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-24 01:00:26.000000 careless-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-24 01:00:26.000000 careless-0.3.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 19:08:00.000000 careless-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 19:08:00.000000 careless-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 19:08:11.852491 careless-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-08-02 19:08:00.000000 careless-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 19:08:00.000000 careless-0.3.6/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 19:08:00.000000 careless-0.3.6/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-02 19:08:00.000000 careless-0.3.6/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 19:08:00.000000 careless-0.3.6/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-08-02 19:08:00.000000 careless-0.3.6/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-02 19:08:00.000000 careless-0.3.6/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-08-02 19:08:00.000000 careless-0.3.6/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-08-02 19:08:00.000000 careless-0.3.6/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-02 19:08:00.000000 careless-0.3.6/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-02 19:08:00.000000 careless-0.3.6/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-08-02 19:08:00.000000 careless-0.3.6/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-02 19:08:00.000000 careless-0.3.6/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-02 19:08:00.000000 careless-0.3.6/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.848491 careless-0.3.6/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 19:08:11.000000 careless-0.3.6/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-08-02 19:08:00.000000 careless-0.3.6/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-08-02 19:08:00.000000 careless-0.3.6/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-02 19:08:11.852491 careless-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-02 19:08:00.000000 careless-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:11.852491 careless-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:08:00.000000 careless-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-02 19:08:00.000000 careless-0.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-08-02 19:08:00.000000 careless-0.3.6/tests/test_cli.py
```

### Comparing `careless-0.3.5/LICENSE` & `careless-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/PKG-INFO` & `careless-0.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.5
+Version: 0.3.6
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.5/README.md` & `careless-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/common.py` & `careless-0.3.6/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/crossvalidation.py` & `careless-0.3.6/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/filtration.py` & `careless-0.3.6/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/interpretation.py` & `careless-0.3.6/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/optimizer.py` & `careless-0.3.6/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/poly.py` & `careless-0.3.6/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/positional_encoding.py` & `careless-0.3.6/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/prior.py` & `careless-0.3.6/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/required.py` & `careless-0.3.6/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/scaling.py` & `careless-0.3.6/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/args/tf_options.py` & `careless-0.3.6/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/callbacks/progress_bar.py` & `careless-0.3.6/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/careless.py` & `careless-0.3.6/careless/careless.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/io/asu.py` & `careless-0.3.6/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/io/formatter.py` & `careless-0.3.6/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/io/manager.py` & `careless-0.3.6/careless/io/manager.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/io/xds.py` & `careless-0.3.6/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/base.py` & `careless-0.3.6/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/likelihoods/laue.py` & `careless-0.3.6/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/likelihoods/mono.py` & `careless-0.3.6/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.6/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/merging/variational.py` & `careless-0.3.6/careless/models/merging/variational.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from careless.models.base import BaseModel
 from careless.utils.shame import sanitize_tensor
 from careless.models.merging.surrogate_posteriors import TruncatedNormal
+from tensorflow.python.keras.engine import data_adapter
 from tqdm.autonotebook import tqdm
 import tensorflow_probability as tfp
 import tensorflow as tf
 from tensorflow import keras as tfk
 import numpy as np
 
 
@@ -178,23 +179,66 @@
 
         #Do some keras-y stuff
         self.add_loss(-ll)
         self.add_metric(-ll, name="NLL")
 
         return ipred
 
-    def train_model(self, data, steps, message=None, format_string="{:0.2e}", validation_data=None, validation_frequency=10, progress=True):
+    def train_step_with_gradient_norm(self, data):
+        """
+        Conduct a training step with `data`. This method is the same as tfk.Model.train_step except that it
+        tracks the norm of the gradients as well. 
+        """
+        data = data_adapter.expand_1d(data)
+        x, y, sample_weight = data_adapter.unpack_x_y_sample_weight(data)
+        # Run forward pass.
+        with tf.GradientTape() as tape:
+            y_pred = self(x, training=True)
+            loss = self.compiled_loss(y, y_pred, sample_weight, regularization_losses=self.losses)
+
+        # Run backwards pass.
+        grads = tape.gradient(loss, self.trainable_variables)
+
+        # Compute the L2 norm of the gradients
+        grad_norm = tf.linalg.global_norm(grads)
+
+        # Only apply gradients if they are valid
+        if tf.math.is_finite(grad_norm):
+            self.optimizer.apply_gradients(zip(grads, self.trainable_variables))
+
+        self.compiled_metrics.update_state(y, y_pred, sample_weight)
+        # Collect metrics to return
+        return_metrics = {
+            "Grad Norm" : grad_norm,
+        }
+        for metric in self.metrics:
+            result = metric.result()
+            if isinstance(result, dict):
+                return_metrics.update(result)
+            else:
+                return_metrics[metric.name] = result
+
+        return return_metrics
+
+    def train_model(self, data, steps, message=None, format_string="{:0.2e}", validation_data=None, validation_frequency=10, progress=True, use_custom_train_step=True):
         """
         Alternative to the keras backed VariationalMergingModel.fit method. This method is much faster at the moment but less flexible.
         """
-        def train_step(model_and_data):
-            model, data = model_and_data
-            model.reset_metrics()
-            history = model.train_step((data,))
-            return history
+        if use_custom_train_step:
+            def train_step(model_and_data):
+                model, data = model_and_data
+                model.reset_metrics()
+                history = model.train_step_with_gradient_norm((data,))
+                return history
+        else:
+            def train_step(model_and_data):
+                model, data = model_and_data
+                model.reset_metrics()
+                history = model.train_step((data,))
+                return history
 
         if not self._run_eagerly:
             train_step = tf.function(train_step, reduce_retracing=True)
 
         if validation_data is not None:
             val_scale = len(data[0]) / len(validation_data[0])
 
@@ -214,9 +258,13 @@
                 v = float(v)
                 pf[k] = format_string.format(v)
                 if k not in history:
                     history[k] = []
                 history[k].append(v)
 
             bar.set_postfix(pf)
+            if use_custom_train_step:
+                if not tf.math.is_finite(_history['Grad Norm']):
+                    print("Encountered numerical issues, terminating optimization early!")
+                    break
         return history
```

### Comparing `careless-0.3.5/careless/models/priors/empirical.py` & `careless-0.3.6/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/priors/wilson.py` & `careless-0.3.6/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/scaling/image.py` & `careless-0.3.6/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/models/scaling/nn.py` & `careless-0.3.6/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/parser.py` & `careless-0.3.6/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/stats/ccanom.py` & `careless-0.3.6/careless/stats/ccpred.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,134 @@
 """
-Compute CCanom from careless output.
+Compute CCpred from careless output.
+
 """
 import argparse
-import matplotlib.pyplot as plt
+import numpy as np
 import reciprocalspaceship as rs
+import gemmi
+
+import matplotlib.pyplot as plt
 import seaborn as sns
 
 
 from careless.stats.parser import BaseParser
 class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtz",
             nargs="+",
-            help="MTZs containing crossvalidation data from careless",
+            help="MTZ(s) containing prediction data from careless",
         )
 
         # Optional arguments
         self.add_argument(
             "-m",
             "--method",
-            default="spearman",
-            choices=["spearman", "pearson"],
-            help="Method for computing correlation coefficient (spearman or pearson)",
+            default="pearson",
+            choices=["pearson", "spearman"],
+            help="Method for computing correlation coefficient (spearman or pearson). "
+            "The Pearson CC uses maximum-likelihood weights. Pearson is the default.",
         )
 
         self.add_argument(
             "-b",
             "--bins",
             default=10,
             type=int,
             help="Number of resolution bins to use, the default is 10.",
         )
 
+        self.add_argument(
+            '--overall',
+            action="store_true",
+            help="Pool all prediction mtz files into a single calculation rather than treating each file individually.",
+        )
 
+def weighted_pearson_ccfunc(df, iobs='Iobs', ipred='Ipred', sigiobs='SigIobs'):
+    x = df[iobs].to_numpy('float32')
+    y = df[ipred].to_numpy('float32')
+    w = np.reciprocal(np.square(df[sigiobs])).to_numpy('float32')
+    return rs.utils.weighted_pearsonr(x, y, w)
 
+def spearman_ccfunc(df, iobs='Iobs', ipred='Ipred'):
+    return df[[iobs, ipred]].corr(method='spearman')[iobs][ipred]
 
+def run_analysis(args):
+    labels = None
 
-def make_halves_ccanom(mtz, bins=10):
-    """Construct half-datasets for computing CCanom"""
-
-    half1 = mtz.loc[mtz.half == 0].copy()
-    half2 = mtz.loc[mtz.half == 1].copy()
-
-    half1["DF"] = half1["F(+)"] - half1["F(-)"]
-    half2["DF"] = half2["F(+)"] - half2["F(-)"]
-
-    temp = half1[["DF", "repeat"]].merge(
-        half2[["DF", "repeat"]], on=["H", "K", "L", "repeat"], suffixes=("1", "2")
-    )
-    temp, labels = temp.assign_resolution_bins(bins)
-
-    return temp, labels
-
-
-def analyze_ccanom_mtz(mtzpath, bins=10, return_labels=True, method="spearman"):
-    """Compute CCanom from 2-fold cross-validation"""
-
-    mtz = rs.read_mtz(mtzpath)
-
-    # Error handling -- make sure MTZ file is appropriate
-    if "half" not in mtz.columns:
-        raise ValueError("Please provide MTZs from careless crossvalidation")
-
-    if "F(+)" not in mtz.columns:
-        raise ValueError("Please provide MTZs merged with `--anomalous` in careless")
+    overall = False
 
-    mtz = mtz.acentrics
-    mtz = mtz.loc[(mtz["N(+)"] > 0) & (mtz["N(-)"] > 0)]
-    m, labels = make_halves_ccanom(mtz, bins=bins)
+    ds = []
+    for m in args.mtz:
+        _ds = rs.read_mtz(m)
+        #non-isomorphism could lead to different resolution for each mtz
+        #need to calculate dHKL before concatenating 
+        _ds.compute_dHKL(inplace=True)
+        _ds['file'] = m
+        _ds['Spacegroup'] = _ds.spacegroup.xhm()
+        ds.append(_ds)
+    ds = rs.concat(ds, check_isomorphous=False)
+    bins,edges = rs.utils.bin_by_percentile(ds.dHKL, args.bins, ascending=False)
+    ds['bin'] = bins
+    labels = [
+        f"{e1:0.2f} - {e2:0.2f}"
+        for e1, e2 in zip(edges[:-1], edges[1:])
+    ]
 
-    grouper = m.groupby(["bin", "repeat"])[["DF1", "DF2"]]
-    result = (
-        grouper.corr(method=method).unstack()[("DF1", "DF2")].to_frame().reset_index()
-    )
+    if args.overall:
+        grouper = ds.groupby(["bin", "test"])
+    else:
+        grouper = ds.groupby(["file", "bin", "test"])
 
-    if return_labels:
-        return result, labels
+    if args.method.lower() == "spearman":
+        ccfunc = spearman_ccfunc
+    elif args.method.lower() == "pearson":
+        ccfunc = weighted_pearson_ccfunc
+
+    result = grouper.apply(ccfunc).reset_index(name='CCpred')
+    result['Resolution Range (Å)'] = np.array(labels)[result.bin]
+    result['Spacegroup'] = grouper['Spacegroup'].apply('first').to_numpy()
+    if not args.overall:
+        result['file'] = grouper['file'].apply('first').to_numpy()
+        result = result[['file', 'Resolution Range (Å)', 'bin', 'test', 'Spacegroup', 'CCpred']]
     else:
-        return result
+        result = result[['Resolution Range (Å)', 'bin', 'test', 'Spacegroup', 'CCpred']]
 
+    result['bin'] = result['bin'].to_numpy('int32')
+    result['test'] = np.array(['Train', 'Test'])[result['test']]
 
-def run_analysis(args):
-    results = []
-    labels = None
-    for m in args.mtz:
-        result = analyze_ccanom_mtz(m, method=args.method, bins=args.bins)
-        if result is None:
-            continue
-        else:
-            result[0]["filename"] = m
-            results.append(result[0])
-            labels = result[1]
-
-    results = rs.concat(results, check_isomorphous=False)
-    results = results.reset_index(drop=True)
-    results["CCanom"] = results[("DF1", "DF2")]
-    results.drop(columns=[("DF1", "DF2")], inplace=True)
+    if args.output is not None:
+        result.to_csv(args.output)
+    else:
+        print(result.to_string())
 
-    for k in ('bin', 'repeat'):
-        results[k] = results[k].to_numpy('int32')
+    plot_kwargs = {
+        'data' : result,
+        'x' : 'bin',
+        'y' : 'CCpred',
+        'style' : 'test',
+    }
 
-    if args.output is not None:
-        results.to_csv(args.output)
+    if args.overall:
+        plot_kwargs['color'] = 'k'
     else:
-        print(results.to_string())
+        plot_kwargs['hue'] = 'file'
+        plot_kwargs['palette'] = "Dark2"
+
+    sns.lineplot(**plot_kwargs)
 
-    sns.lineplot(
-        data=results, x="bin", y="CCanom", hue="filename", palette="Dark2"
-    )
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
-    plt.ylabel(r"$\mathrm{CC_{anom}}$ " + f"({args.method})")
+    plt.ylabel(r"$\mathrm{CC_{pred}}$ " + f"({args.method})")
+    plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
 
     if args.image is not None:
         plt.savefig(args.image)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `careless-0.3.5/careless/stats/cchalf.py` & `careless-0.3.6/careless/stats/rsplit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Compute CChalf from careless output.
 """
 import argparse
+import numpy as np
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
+from scipy.optimize import minimize
 
 
 from careless.stats.parser import BaseParser
 class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
             description=__doc__
@@ -18,101 +20,104 @@
         self.add_argument(
             "mtz",
             nargs="+",
             help="MTZs containing crossvalidation data from careless",
         )
 
         self.add_argument(
-            "-m",
-            "--method",
-            default="spearman",
-            choices=["spearman", "pearson"],
-            help=("Method for computing correlation coefficient (spearman or pearson)"),
-        )
-
-        self.add_argument(
             "-b",
             "--bins",
             default=10,
             type=int,
             help=("Number of resolution bins to use, the default is 10."),
         )
 
-def make_halves_cchalf(mtz, bins=10):
-    """Construct half-datasets for computing CChalf"""
+        self.add_argument(
+            "--overall",
+            action="store_true",
+            help="Pool all prediction mtz files into a single calculation rather than treating each file individually.",
+        )
+
+def rsplit(dataset):
+    x,y = dataset.F1.to_numpy(),dataset.F2.to_numpy()
+    def rfunc(k):
+        return np.sum(np.abs(x - k * y)) / np.sum(x + k * y)
+
+    p = minimize(rfunc, 1.)
+    return np.sqrt(2) * p.fun 
+
+def make_halves_rsplit(mtz, bins=10):
+    """Construct half-datasets for computing Rsplit"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
 
     # Support anomalous
     if "F(+)" in half1.columns:
         half1 = half1.stack_anomalous()
         half2 = half2.stack_anomalous()
 
-    temp = half1[["F", "repeat"]].merge(
-        half2[["F", "repeat"]], on=["H", "K", "L", "repeat"], suffixes=("1", "2")
-    )
-    temp, labels = temp.assign_resolution_bins(bins)
-
-    return temp, labels
-
-
-def analyze_cchalf_mtz(mtzpath, bins=10, return_labels=True, method="spearman"):
-    """Compute CChalf from 2-fold cross-validation"""
-
-    mtz = rs.read_mtz(mtzpath)
-
-    # Error handling -- make sure MTZ file is appropriate
-    if "half" not in mtz.columns:
-        raise ValueError("Please provide MTZs from careless crossvalidation")
-
-    m, labels = make_halves_cchalf(mtz, bins)
-
-    grouper = m.groupby(["bin", "repeat"])[["F1", "F2"]]
-    result = (
-        grouper.corr(method=method).unstack()[("F1", "F2")].to_frame().reset_index()
-    )
-
-    if return_labels:
-        return result, labels
-    else:
-        return result
-
+    out = half1[["F", "SigF", "repeat"]].merge(
+        half2[["F", "SigF", "repeat"]], on=["H", "K", "L", "repeat"], suffixes=("1", "2")
+    ).dropna()
+    return out
 
 def run_analysis(args):
-    results = []
-    labels = None
+    ds = []
     for m in args.mtz:
-        result = analyze_cchalf_mtz(m, bins=args.bins, method=args.method)
-        if result is None:
-            continue
-        else:
-            result[0]["filename"] = m
-            results.append(result[0])
-            labels = result[1]
-
-    results = rs.concat(results, check_isomorphous=False)
-    results = results.reset_index(drop=True)
-    results["CChalf"] = results[("F1", "F2")]
-    results.drop(columns=[("F1", "F2")], inplace=True)
+        _ds = rs.read_mtz(m)
+        #non-isomorphism could lead to different resolution for each mtz
+        #need to calculate dHKL before concatenating 
+        _ds = make_halves_rsplit(_ds)
+        _ds.compute_dHKL(inplace=True)
+        _ds['file'] = m
+        _ds['Spacegroup'] = _ds.spacegroup.xhm()
+        ds.append(_ds)
+    ds = rs.concat(ds, check_isomorphous=False)
+    bins,edges = rs.utils.bin_by_percentile(ds.dHKL, args.bins, ascending=False)
+    ds['bin'] = bins
+    labels = [
+        f"{e1:0.2f} - {e2:0.2f}"
+        for e1, e2 in zip(edges[:-1], edges[1:])
+    ]
 
+    if args.overall:
+        grouper = ds.groupby(["bin", "repeat"])
+    else:
+        grouper = ds.groupby(["file", "bin", "repeat"])
+    result = grouper.apply(rsplit).reset_index(name='Rsplit')
+    result['Resolution Range (Å)'] = np.array(labels)[result.bin]
+    result['Spacegroup'] = grouper['Spacegroup'].apply('first').to_numpy()
+    if not args.overall:
+        result['file'] = grouper['file'].apply('first').to_numpy()
+        result = result[['file', 'repeat', 'Resolution Range (Å)', 'bin', 'Spacegroup', 'Rsplit']]
+    else:
+        result = result[['repeat', 'Resolution Range (Å)', 'bin', 'Spacegroup', 'Rsplit']]
 
-    for k in ('bin', 'repeat'):
-        results[k] = results[k].to_numpy('int32')
 
     if args.output is not None:
-        results.to_csv(args.output)
+        result.to_csv(args.output)
     else:
-        print(results.to_string())
+        print(result.to_string())
     
-    sns.lineplot(
-        data=results, x="bin", y="CChalf", hue="filename", palette="viridis"
-    )
+    plot_kwargs = {
+        'data' : result,
+        'x' : 'bin',
+        'y' : 'Rsplit',
+    }
+
+    if args.overall:
+        plot_kwargs['color'] = 'k'
+    else:
+        plot_kwargs['hue'] = 'file'
+        plot_kwargs['palette'] = "Dark2"
+
+    sns.lineplot(**plot_kwargs)
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
-    plt.ylabel(r"$\mathrm{CC_{1/2}}$ " + f"({args.method})")
+    plt.ylabel(r"$R_{\mathrm{split}}$")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
 
     if args.image is not None:
         plt.savefig(args.image)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `careless-0.3.5/careless/stats/ccpred.py` & `careless-0.3.6/careless/stats/cchalf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,144 +1,148 @@
 """
-Compute CCpred from careless output.
-
+Compute CChalf from careless output.
 """
 import argparse
 import numpy as np
-import reciprocalspaceship as rs
-import gemmi
-
 import matplotlib.pyplot as plt
+import reciprocalspaceship as rs
 import seaborn as sns
 
 
 from careless.stats.parser import BaseParser
 class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
-            "mtzs",
+            "mtz",
             nargs="+",
-            help="MTZs containing prediction data from careless",
+            help="MTZs containing crossvalidation data from careless",
         )
 
-        # Optional arguments
         self.add_argument(
             "-m",
             "--method",
-            default="spearman",
+            default="pearson",
             choices=["spearman", "pearson"],
-            help="Method for computing correlation coefficient (spearman or pearson)",
+            help="Method for computing correlation coefficient (spearman or pearson). "
+            "The Pearson CC uses maximum-likelihood weights. Pearson is the default.",
         )
 
         self.add_argument(
             "-b",
             "--bins",
             default=10,
             type=int,
-            help="Number of resolution bins to use, the default is 10.",
+            help=("Number of resolution bins to use, the default is 10."),
         )
 
         self.add_argument(
-            '--overall',
+            "--overall",
             action="store_true",
             help="Pool all prediction mtz files into a single calculation rather than treating each file individually.",
         )
 
 
-def compute_ccpred(
-    dataset, overall=False, bins=10, return_labels=True, method="spearman"
-):
-    """Compute CCpred from cross-validation"""
-
-    if overall:
-        labels = ['Overall']
-        dataset['bin'] = -1
-        grouper = dataset.groupby(["test"])[["Iobs", "Ipred"]]
-    else:
-        dataset, labels = dataset.assign_resolution_bins(bins)
-        grouper = dataset.groupby(["bin", "test"])[["Iobs", "Ipred"]]
-
-    result = (
-        grouper.corr(method=method)
-        .unstack()[("Iobs", "Ipred")]
-        .to_frame()
-        .reset_index()
-    )
-
-    result["spacegroup"] = dataset.spacegroup.xhm()
-
-    return result, labels
 
+def weighted_pearson_ccfunc(df):
+    x = df['F1'].to_numpy('float32')
+    y = df['F2'].to_numpy('float32')
+    w = np.reciprocal(
+        np.square(df['SigF1']) + np.square(df['SigF2'])
+    ).to_numpy('float32')
+    return rs.utils.weighted_pearsonr(x, y, w)
+
+def spearman_ccfunc(df):
+    return df[['F1', 'F2']].corr(method='spearman')['F1']['F2']
+
+def make_halves_cchalf(mtz, bins=10):
+    """Construct half-datasets for computing CChalf"""
+
+    half1 = mtz.loc[mtz.half == 0].copy()
+    half2 = mtz.loc[mtz.half == 1].copy()
+
+    # Support anomalous
+    if "F(+)" in half1.columns:
+        half1 = half1.stack_anomalous()
+        half2 = half2.stack_anomalous()
+
+    out = half1[["F", "SigF", "repeat"]].merge(
+        half2[["F", "SigF", "repeat"]], on=["H", "K", "L", "repeat"], suffixes=("1", "2")
+    ).dropna()
+    return out
 
 def run_analysis(args):
-    results = []
-    labels = None
-
-    overall = False
+    ds = []
+    for m in args.mtz:
+        _ds = rs.read_mtz(m)
+        #non-isomorphism could lead to different resolution for each mtz
+        #need to calculate dHKL before concatenating 
+        _ds = make_halves_cchalf(_ds)
+        _ds.compute_dHKL(inplace=True)
+        _ds['file'] = m
+        _ds['Spacegroup'] = _ds.spacegroup.xhm()
+        ds.append(_ds)
+    ds = rs.concat(ds, check_isomorphous=False)
+    bins,edges = rs.utils.bin_by_percentile(ds.dHKL, args.bins, ascending=False)
+    ds['bin'] = bins
+    labels = [
+        f"{e1:0.2f} - {e2:0.2f}"
+        for e1, e2 in zip(edges[:-1], edges[1:])
+    ]
 
     if args.overall:
-        ds = []
-        for m in args.mtzs:
-            ds.append(rs.read_mtz(m))
-        ds = rs.concat(ds)
-        results,labels = compute_ccpred(ds, overall=overall, bins=args.bins, method=args.method)
+        grouper = ds.groupby(["bin", "repeat"])
     else:
-        for m in args.mtzs:
-            ds = rs.read_mtz(m)
-            result,labels = compute_ccpred(ds, overall=overall, bins=args.bins, method=args.method)
-            result['file'] = m
-            if isinstance(result, tuple):
-                results.append(result)
-                labels = result
-            else:
-                results.append(result)
-        results = rs.concat(results, check_isomorphous=False)
-
-    results = results.reset_index(drop=True)
-    results["CCpred"] = results[("Iobs", "Ipred")]
-    results.drop(columns=[("Iobs", "Ipred")], inplace=True)
+        grouper = ds.groupby(["file", "bin", "repeat"])
+    if args.method.lower() == "spearman":
+        ccfunc = spearman_ccfunc
+    elif args.method.lower() == "pearson":
+        ccfunc = weighted_pearson_ccfunc
+    result = grouper.apply(ccfunc).reset_index(name='CChalf')
+    result['Resolution Range (Å)'] = np.array(labels)[result.bin]
+    result['Spacegroup'] = grouper['Spacegroup'].apply('first').to_numpy()
+    if not args.overall:
+        result['file'] = grouper['file'].apply('first').to_numpy()
+        result = result[['file', 'repeat', 'Resolution Range (Å)', 'bin', 'Spacegroup', 'CChalf']]
+    else:
+        result = result[['repeat', 'Resolution Range (Å)', 'bin', 'Spacegroup', 'CChalf']]
 
-    results['bin'] = results['bin'].to_numpy('int32')
-    results['test'] = np.array(['Train', 'Test'])[results['test']]
 
     if args.output is not None:
-        results.to_csv(args.output)
+        result.to_csv(args.output)
     else:
-        print(results.to_string())
-
+        print(result.to_string())
+    
     plot_kwargs = {
-        'data' : results,
+        'data' : result,
         'x' : 'bin',
-        'y' : 'CCpred',
-        'style' : 'test',
+        'y' : 'CChalf',
     }
 
-    if 'file' in results:
+    if args.overall:
+        plot_kwargs['color'] = 'k'
+    else:
         plot_kwargs['hue'] = 'file'
         plot_kwargs['palette'] = "Dark2"
-    else:
-        plot_kwargs['color'] = 'k'
 
     sns.lineplot(**plot_kwargs)
-
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
-    plt.ylabel(r"$\mathrm{CC_{pred}}$ " + f"({args.method})")
-    plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+    plt.ylabel(r"$\mathrm{CC_{1/2}}$ " + f"({args.method})")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
 
     if args.image is not None:
         plt.savefig(args.image)
 
     if args.show:
         plt.show()
 
+
 def main():
     parser = ArgumentParser().parse_args()
     run_analysis(parser)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `careless-0.3.5/careless/stats/completeness.py` & `careless-0.3.6/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/stats/parser.py` & `careless-0.3.6/careless/stats/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/stats/prior_b.py` & `careless-0.3.6/careless/stats/prior_b.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/stats/rescale.py` & `careless-0.3.6/careless/stats/rescale.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/utils/distributions.py` & `careless-0.3.6/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/utils/laue.py` & `careless-0.3.6/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless/utils/positional_encoding.py` & `careless-0.3.6/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/careless.egg-info/PKG-INFO` & `careless-0.3.6/careless.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.5
+Version: 0.3.6
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.5/careless.egg-info/SOURCES.txt` & `careless-0.3.6/careless.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 careless/models/scaling/image.py
 careless/models/scaling/nn.py
 careless/stats/__init__.py
 careless/stats/ccanom.py
 careless/stats/cchalf.py
 careless/stats/ccpred.py
 careless/stats/completeness.py
+careless/stats/history.py
 careless/stats/parser.py
 careless/stats/prior_b.py
 careless/stats/rescale.py
 careless/stats/rsplit.py
 careless/utils/__init__.py
 careless/utils/device.py
 careless/utils/distributions.py
```

### Comparing `careless-0.3.5/scripts/make_difference_map` & `careless-0.3.6/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/scripts/stream2mtz` & `careless-0.3.6/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.5/setup.py` & `careless-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     ],
     entry_points={
         "console_scripts": [
             "careless=careless.careless:main",
             "careless.ccanom=careless.stats.ccanom:main",
             "careless.cchalf=careless.stats.cchalf:main",
             "careless.ccpred=careless.stats.ccpred:main",
+            "careless.plot_history=careless.stats.history:main",
             "careless.bfactor=careless.stats.prior_b:main",
             "careless.apply_bfactor=careless.stats.rescale:main",
             "careless.completeness=careless.stats.completeness:main",
             "careless.rsplit=careless.stats.rsplit:main",
             "careless.xds2mtz=careless.io.xds:main",
         ]
     },
```

### Comparing `careless-0.3.5/tests/conftest.py` & `careless-0.3.6/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 @pytest.fixture
 def xval_mtz():
     datapath = "data/output/pyp_xval_0.mtz"
     filename = abspath(join(dirname(__file__), datapath))
     return filename
 
 @pytest.fixture
+def history_csv():
+    datapath = "data/output/pyp_history.csv"
+    filename = abspath(join(dirname(__file__), datapath))
+    return filename
+
+@pytest.fixture
 def predictions_mtz():
     datapath = "data/output/pyp_predictions_0.mtz"
     filename = abspath(join(dirname(__file__), datapath))
     return filename
 
 @pytest.fixture
 def merged_mtz():
```

### Comparing `careless-0.3.5/tests/test_cli.py` & `careless-0.3.6/tests/test_cli.py`

 * *Files identical despite different names*

