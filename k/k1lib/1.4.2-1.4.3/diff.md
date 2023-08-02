# Comparing `tmp/k1lib-1.4.2.tar.gz` & `tmp/k1lib-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k1lib-1.4.2.tar", last modified: Fri Jun 30 11:19:41 2023, max compression
+gzip compressed data, was "k1lib-1.4.3.tar", last modified: Wed Aug  2 03:58:02 2023, max compression
```

## Comparing `k1lib-1.4.2.tar` & `k1lib-1.4.3.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.313048 k1lib-1.4.2/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-06-30 11:16:28.000000 k1lib-1.4.2/LICENSE
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3427 2023-06-30 11:19:41.313048 k1lib-1.4.2/PKG-INFO
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.2/k1lib/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_baseClasses.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25511 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_basics.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_context.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/_hidden/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.2/k1lib/_hidden/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.2/k1lib/_hidden/hiddenFile.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_higher.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_k1a.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_learner.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/_mo/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.2/k1lib/_mo/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_mo/atom.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_mo/parseM.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_mo/substance.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_mo/system.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_monkey.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/_perlin.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/callbacks/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.2/k1lib/callbacks/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/callbacks.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/confusionMatrix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/core.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/hookModule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/hookParam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/landscape.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/limits.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/callbacks/lossFunctions/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.2/k1lib/callbacks/lossFunctions/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/lossFunctions/accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/lossFunctions/shorts.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/loss_accuracy.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/paramFinder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/profiler.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib/callbacks/profilers/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.2/k1lib/callbacks/profilers/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/profilers/computation.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/profilers/io.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/profilers/memory.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/profilers/time.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/progress.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/recorder.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/callbacks/shorts.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.313048 k1lib-1.4.2/k1lib/cli/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      926 2023-06-19 08:21:11.000000 k1lib-1.4.2/k1lib/cli/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/_applyCl.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/bio.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/cif.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    34729 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/conv.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    47519 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/filt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-06-30 11:09:58.000000 k1lib-1.4.2/k1lib/cli/gb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/grep.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35262 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/init.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    56332 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/inp.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1127 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/kcsv.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/kxml.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/mgi.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   102579 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/modifier.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/mol.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/nb.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/optimizations.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18482 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/output.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/sam.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    68110 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/structural.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/trace.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/typehint.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49329 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/cli/utils.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/eqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/fmt.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/graphEqn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5174 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/imports.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.313048 k1lib-1.4.2/k1lib/k1ui/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.2/k1lib/k1ui/256.model.state_dict.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.2/k1lib/k1ui/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/k1ui/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.2/k1lib/k1ui/mouseKey.pth
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/knn.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6449 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/p5.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/schedule.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/selector.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.313048 k1lib-1.4.2/k1lib/serve/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.2/k1lib/serve/__init__.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.2/k1lib/serve/main.html
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/serve/main.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.2/k1lib/serve/suffix-dash.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.2/k1lib/serve/suffix.py
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    27360 2023-06-30 11:09:59.000000 k1lib-1.4.2/k1lib/viz.py
-drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-06-30 11:19:41.309048 k1lib-1.4.2/k1lib.egg-info/
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3427 2023-06-30 11:19:41.000000 k1lib-1.4.2/k1lib.egg-info/PKG-INFO
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1975 2023-06-30 11:19:41.000000 k1lib-1.4.2/k1lib.egg-info/SOURCES.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-06-30 11:19:41.000000 k1lib-1.4.2/k1lib.egg-info/dependency_links.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-06-30 11:19:41.000000 k1lib-1.4.2/k1lib.egg-info/requires.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-06-30 11:19:41.000000 k1lib-1.4.2/k1lib.egg-info/top_level.txt
--rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-06-30 11:19:41.313048 k1lib-1.4.2/setup.cfg
--rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1162 2023-06-30 11:15:59.000000 k1lib-1.4.2/setup.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.031537 k1lib-1.4.3/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1049 2023-08-02 00:51:20.000000 k1lib-1.4.3/LICENSE
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3427 2023-08-02 03:58:02.031537 k1lib-1.4.3/PKG-INFO
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.023537 k1lib-1.4.3/k1lib/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     1441 2023-05-26 17:16:37.000000 k1lib-1.4.3/k1lib/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    83638 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_baseClasses.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    25641 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_basics.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8208 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_context.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib/_hidden/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        0 2021-08-11 18:19:53.000000 k1lib-1.4.3/k1lib/_hidden/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       79 2021-08-11 18:19:53.000000 k1lib-1.4.3/k1lib/_hidden/hiddenFile.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4314 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_higher.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3085 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_k1a.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20567 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_learner.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib/_mo/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      615 2021-10-24 23:32:21.000000 k1lib-1.4.3/k1lib/_mo/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    24015 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_mo/atom.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18173 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_mo/parseM.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5631 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_mo/substance.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15454 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_mo/system.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    36997 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_monkey.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5575 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/_perlin.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib/callbacks/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      378 2021-10-30 05:51:17.000000 k1lib-1.4.3/k1lib/callbacks/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31963 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/callbacks.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5455 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/confusionMatrix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2245 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/core.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    19517 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/hookModule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7488 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/hookParam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5728 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/landscape.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14525 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/limits.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib/callbacks/lossFunctions/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       30 2021-10-27 12:39:02.000000 k1lib-1.4.3/k1lib/callbacks/lossFunctions/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3695 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/lossFunctions/accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5968 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/lossFunctions/shorts.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10038 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/loss_accuracy.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6002 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/paramFinder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5311 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/profiler.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib/callbacks/profilers/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       45 2021-08-11 18:19:53.000000 k1lib-1.4.3/k1lib/callbacks/profilers/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     9311 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/profilers/computation.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4069 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/profilers/io.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7368 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/profilers/memory.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6971 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/profilers/time.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4242 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/progress.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4370 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/recorder.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8363 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/callbacks/shorts.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.031537 k1lib-1.4.3/k1lib/cli/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      975 2023-07-13 16:14:07.000000 k1lib-1.4.3/k1lib/cli/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31282 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/_applyCl.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    13909 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/bio.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5162 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/cif.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    39336 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/conv.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    50607 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/filt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     8480 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/gb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12136 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/grep.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    35488 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/init.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    69938 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/inp.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14704 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/ktree.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     7467 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/kxml.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15993 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/lsext.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2977 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/mgi.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    18005 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/models.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   125028 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/modifier.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      735 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/mol.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5822 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/nb.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     6311 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/optimizations.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20026 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/output.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3042 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/sam.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    72596 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/structural.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15949 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/trace.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    41733 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/typehint.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    49466 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/cli/utils.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    21263 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/eqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    12310 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/fmt.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    10890 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/graphEqn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     5180 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/imports.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.031537 k1lib-1.4.3/k1lib/k1ui/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)  2453826 2023-01-19 22:50:00.000000 k1lib-1.4.3/k1lib/k1ui/256.model.state_dict.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2023-01-19 22:00:40.000000 k1lib-1.4.3/k1lib/k1ui/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    88758 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/k1ui/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)   304735 2023-01-17 19:16:23.000000 k1lib-1.4.3/k1lib/k1ui/mouseKey.pth
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     4919 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/knn.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    31314 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/p5.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    14079 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/schedule.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    29996 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/selector.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.031537 k1lib-1.4.3/k1lib/serve/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       20 2022-09-16 01:12:41.000000 k1lib-1.4.3/k1lib/serve/__init__.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    20544 2023-03-19 11:14:40.000000 k1lib-1.4.3/k1lib/serve/main.html
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    15412 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/serve/main.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      153 2023-05-05 16:00:40.000000 k1lib-1.4.3/k1lib/serve/suffix-dash.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      642 2023-02-13 19:00:39.000000 k1lib-1.4.3/k1lib/serve/suffix.py
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)    28374 2023-08-02 03:41:46.000000 k1lib-1.4.3/k1lib/viz.py
+drwxrwxr-x   0 kelvin    (1000) kelvin    (1000)        0 2023-08-02 03:58:02.027537 k1lib-1.4.3/k1lib.egg-info/
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     3427 2023-08-02 03:58:01.000000 k1lib-1.4.3/k1lib.egg-info/PKG-INFO
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)     2015 2023-08-02 03:58:01.000000 k1lib-1.4.3/k1lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        1 2023-08-02 03:58:01.000000 k1lib-1.4.3/k1lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)      145 2023-08-02 03:58:01.000000 k1lib-1.4.3/k1lib.egg-info/requires.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)        6 2023-08-02 03:58:01.000000 k1lib-1.4.3/k1lib.egg-info/top_level.txt
+-rw-rw-r--   0 kelvin    (1000) kelvin    (1000)       38 2023-08-02 03:58:02.031537 k1lib-1.4.3/setup.cfg
+-rwxrwxr-x   0 kelvin    (1000) kelvin    (1000)     1162 2023-08-02 03:57:36.000000 k1lib-1.4.3/setup.py
```

### Comparing `k1lib-1.4.2/LICENSE` & `k1lib-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/PKG-INFO` & `k1lib-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.2
+Version: 1.4.3
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.2/k1lib/__init__.py` & `k1lib-1.4.3/k1lib/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_baseClasses.py` & `k1lib-1.4.3/k1lib/_baseClasses.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_basics.py` & `k1lib-1.4.3/k1lib/_basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,22 +106,16 @@
             while True:                                                          # cron
                 a = datetime.datetime.now()                                      # cron
                 now = {"year": a.year, "month": a.month, "day": a.day, "weekday": a.weekday(), "hour": a.hour, "minute": a.minute, "second": a.second} # cron
                 this = f(*[now[e] for e in args])                                # cron
                 if not last and this: func()                                     # cron
                 last = this; time.sleep(0.5)                                     # cron
         threading.Thread(target=startLoop).start()                               # cron
+        return func                                                              # cron
     return inner                                                                 # cron
-def cron(f):                                                                     # cron
-    """Sets up a cron job in another thread, activating whenever ``f`` goes from False to True.
-Example::
-
-
-"""                                                                              # cron
-    pass                                                                         # cron
 class wrapMod:                                                                   # wrapMod
     def __init__(self, m, moduleName=None):                                      # wrapMod
         """Wraps around a module, and only suggest symbols in __all__ list
 defined inside the module. Example::
 
     from . import randomModule
     randomModule = wrapMod(randomModule)
@@ -285,30 +279,36 @@
 - Alternatively, set the environment variable `k1lib_pushNotificationKey` instead
 - Run the function as usual"""                                                   # pushNotification
     import requests                                                              # pushNotification
     key = k1lib.settings.pushNotificationKey                                     # pushNotification
     requests.get("http://xdroid.net/api/message?" + urllib.parse.urlencode({'k': key, 't': title, 'c': content, 'u': url})) # pushNotification
     print("Pushed!")                                                             # pushNotification
 class Dependency:                                                                # Dependency
-    def __init__(self, s): self.s = s                                            # Dependency
-    def __getattr__(self, attr): raise Exception(f"Python package `{self.s}` not found. Please install it") # Dependency
-def dep(s):                                                                      # dep
+    def __init__(self, s, alt:str=None, url:str=None): self.s = s; self.alt = alt; self.url = url # Dependency
+    def __getattr__(self, attr):                                                 # Dependency
+        after = f"More information is available on {self.url}" if self.url else f"" # Dependency
+        raise Exception(f"Python package `{self.alt or self.s}` not found. Please install it. {after}") # Dependency
+def dep(s, alt:str=None, url:str=None):                                          # dep
     """Imports a potentially unavailable package
 Example::
 
     graphviz = k1.dep("graphviz")
 
     # executes as normal, if graphviz is available, else throws an error
     g = graphviz.Digraph()
 
 I don't imagine this would be useful for everyday use though.
 This is mainly for writing this library, so that it can use
-optional dependencies."""                                                        # dep
+optional dependencies.
+
+:param s: name of the package. Can be nested, like `matplotlib.pyplot`
+:param alt: (optional) name of the package to display in error message if package is not found
+:param url: (optional) url of the package's website, so that they know where to get official docs""" # dep
     try: return importlib.import_module(s)                                       # dep
-    except: return Dependency(s)                                                 # dep
+    except: return Dependency(s, alt, url)                                       # dep
 tickCheckpoints = np.array([1, 2, 2.5, 5, 10])/10                                # dep
 def ticks(x:float, y:float, rounding:int=6):                                     # ticks
     """Get tick locations in a plot that look reasonable.
 Example::
 
     ticks(-5, 40)     # returns [-10.0, -5.0, 0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 45.0]
     ticks(0.05, 0.07) # returns [0.05, 0.0525, 0.055, 0.0575, 0.06, 0.0625, 0.065, 0.0675, 0.07, 0.0725]
```

### Comparing `k1lib-1.4.2/k1lib/_context.py` & `k1lib-1.4.3/k1lib/_context.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_higher.py` & `k1lib-1.4.3/k1lib/_higher.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_k1a.py` & `k1lib-1.4.3/k1lib/_k1a.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_learner.py` & `k1lib-1.4.3/k1lib/_learner.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_mo/__init__.py` & `k1lib-1.4.3/k1lib/_mo/__init__.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_mo/atom.py` & `k1lib-1.4.3/k1lib/_mo/atom.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_mo/parseM.py` & `k1lib-1.4.3/k1lib/_mo/parseM.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_mo/substance.py` & `k1lib-1.4.3/k1lib/_mo/substance.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_mo/system.py` & `k1lib-1.4.3/k1lib/_mo/system.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_monkey.py` & `k1lib-1.4.3/k1lib/_monkey.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/_perlin.py` & `k1lib-1.4.3/k1lib/_perlin.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/callbacks.py` & `k1lib-1.4.3/k1lib/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/confusionMatrix.py` & `k1lib-1.4.3/k1lib/callbacks/confusionMatrix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/core.py` & `k1lib-1.4.3/k1lib/callbacks/core.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/hookModule.py` & `k1lib-1.4.3/k1lib/callbacks/hookModule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/hookParam.py` & `k1lib-1.4.3/k1lib/callbacks/hookParam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/landscape.py` & `k1lib-1.4.3/k1lib/callbacks/landscape.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/limits.py` & `k1lib-1.4.3/k1lib/callbacks/limits.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/lossFunctions/accuracy.py` & `k1lib-1.4.3/k1lib/callbacks/lossFunctions/accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/lossFunctions/shorts.py` & `k1lib-1.4.3/k1lib/callbacks/lossFunctions/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/loss_accuracy.py` & `k1lib-1.4.3/k1lib/callbacks/loss_accuracy.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/paramFinder.py` & `k1lib-1.4.3/k1lib/callbacks/paramFinder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/profiler.py` & `k1lib-1.4.3/k1lib/callbacks/profiler.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/profilers/computation.py` & `k1lib-1.4.3/k1lib/callbacks/profilers/computation.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/profilers/io.py` & `k1lib-1.4.3/k1lib/callbacks/profilers/io.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/profilers/memory.py` & `k1lib-1.4.3/k1lib/callbacks/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/profilers/time.py` & `k1lib-1.4.3/k1lib/callbacks/profilers/time.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/progress.py` & `k1lib-1.4.3/k1lib/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/recorder.py` & `k1lib-1.4.3/k1lib/callbacks/recorder.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/callbacks/shorts.py` & `k1lib-1.4.3/k1lib/callbacks/shorts.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/__init__.py` & `k1lib-1.4.3/k1lib/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from .grep import *
 from .inp import *
 from .modifier import *
 from .output import *
 from .structural import *
 from .conv import *
 from .utils import *
+from .models import *
+from .lsext import *
 
 # bio/chem specific
 from .bio import *
 from .mol import *
 from . import mgi;  mgi  = _wrapMod(mgi)
 from . import cif;  #cif  = _wrapMod(cif)
 
 # file formats
-from . import kxml; kxml = _wrapMod(kxml)
-from . import kcsv; #kcsv = _wrapMod(kcsv)
-from . import sam;  sam  = _wrapMod(sam)
-from . import gb;   gb   = _wrapMod(gb)
-from . import nb;   nb   = _wrapMod(nb)
+from . import ktree; ktree = _wrapMod(ktree)
+from . import kxml;  kxml = _wrapMod(kxml)
+from . import sam;   sam  = _wrapMod(sam)
+from . import gb;    gb   = _wrapMod(gb)
+from . import nb;    nb   = _wrapMod(nb)
 
 from .optimizations import *
 from .trace import * # has to be last, to wait for others to load up
```

### Comparing `k1lib-1.4.2/k1lib/cli/_applyCl.py` & `k1lib-1.4.3/k1lib/cli/_applyCl.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/bio.py` & `k1lib-1.4.3/k1lib/cli/bio.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/cif.py` & `k1lib-1.4.3/k1lib/cli/cif.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/conv.py` & `k1lib-1.4.3/k1lib/cli/conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 strings, types, ...), then most likely it will convert iterator to iterator, as you
 can always use the function directly if you only want to apply it on 1 object.
 
 If it sounds complicated (convert to PIL image, tensor, ...) then most likely it will
 convert object to object. Lastly, there are some that just feels right to input
 an iterator and output a single object (like getting max, min, std, mean values)."""
 __all__ = ["toTensor", "toRange", "toList",
-           "toSum", "toProd", "toAvg", "toMean", "toMax", "toMin", "toPIL", "toImg",
+           "toSum", "toProd", "toAvg", "toMean", "toStd", "toMax", "toMin", "toPIL", "toImg",
            "toRgb", "toRgba", "toGray", "toDict",
-           "toFloat", "toInt", "toBytes", "toHtml", "toAscii", "toHash"]
+           "toFloat", "toInt", "toBytes", "toHtml", "toAscii", "toHash", "toCsv"]
 import re, k1lib, math, os, numpy as np, io, base64, unicodedata
 from k1lib.cli.init import BaseCli, T, yieldT; import k1lib.cli as cli
 from k1lib.cli.typehint import *; import matplotlib as mpl; import matplotlib.pyplot as plt
 from collections import deque, defaultdict; from typing import Iterator, Any, List, Set, Tuple, Dict, Callable, Union
 settings = k1lib.settings.cli
 try: import PIL; hasPIL = True
 except: hasPIL = False
@@ -147,15 +147,49 @@
     def __ror__(self, it:Iterator[float]):                                       # toAvg
         if isinstance(it, settings.arrayTypes): return it.mean()                 # toAvg
         s = 0; i = -1                                                            # toAvg
         for i, v in enumerate(it): s += v                                        # toAvg
         i += 1                                                                   # toAvg
         if not k1lib.settings.cli.strict and i == 0: return float("nan")         # toAvg
         return s / i                                                             # toAvg
-toMean = toAvg                                                                   # toAvg
+if hasTorch:                                                                     # toAvg
+    torchVer = int(torch.__version__.split(".")[0])                              # toAvg
+    if torchVer >= 2:                                                            # toAvg
+        def torchStd(it, ddof, dim=None): return torch.std(it, dim, correction=ddof) # toAvg
+    else:                                                                        # toAvg
+        def torchStd(it, ddof, dim=None):                                        # toAvg
+            if ddof == 0: return torch.std(it, dim, unbiased=False)              # toAvg
+            if ddof == 1: return torch.std(it, dim, unbiased=True)               # toAvg
+            raise Exception(f"Please install PyTorch 2, as version 1 don't support correction factor of {ddof}") # toAvg
+else:                                                                            # toAvg
+    def torchStd(it, ddof): raise Exception("PyTorch not installed")             # toAvg
+class toStd(BaseCli):                                                            # toStd
+    def __init__(self, ddof:int=0):                                              # toStd
+        """Calculates standard deviation of list of numbers. Can pipe in :class:`torch.Tensor`
+or :class:`numpy.ndarray` to be faster. Example::
+
+    # returns 2.8722813232690143
+    range(10) | toStd()
+    # returns nan
+    [] | toStd()
+
+:param ddof: "delta degree of freedom". The divisor used in calculations is ``N - ddof``""" # toStd
+        self.ddof = ddof                                                         # toStd
+    def _all_array_opt(self, it, level):                                         # toStd
+        n = len(it.shape); ddof = self.ddof; dim = tuple(range(level, n))        # toStd
+        if isinstance(it, np.ndarray): return np.std(it, ddof=ddof, axis=dim)    # toStd
+        elif hasTorch and isinstance(it, torch.Tensor): return torchStd(it, ddof, dim) # toStd
+        return NotImplemented                                                    # toStd
+    def __ror__(self, it):                                                       # toStd
+        ddof = self.ddof                                                         # toStd
+        if isinstance(it, settings.arrayTypes):                                  # toStd
+            if isinstance(it, np.ndarray): return np.std(it, ddof=ddof)          # toStd
+            elif hasTorch and isinstance(it, torch.Tensor): return torchStd(it, ddof) # toStd
+        return np.std(np.array(list(it)))                                        # toStd
+toMean = toAvg                                                                   # toStd
 class toMax(BaseCli):                                                            # toMax
     def __init__(self):                                                          # toMax
         """Calculates the max of a bunch of numbers. Can pipe in :class:`torch.Tensor` or :class:`numpy.ndarray`.
 Example::
 
     # returns 6
     [2, 5, 6, 1, 2] | toMax()"""                                                 # toMax
@@ -429,27 +463,42 @@
 Example::
 
     # converts string to bytes
     "abc" | toBytes()
     # converts image to base64 bytes
     torch.randn(200, 100) | toImg() | toBytes()
 
+
+.. admonition:: Custom datatype
+
+    It is possible to build objects that can interoperate with this cli,
+    like this::
+
+        class custom1:
+            def __init__(self, config=None): ...
+            def _toBytes(self): return b"abc"
+
+        custom1() | toBytes() # returns b"abc"
+
+    When called upon, :class:`toBytes` will detect that the input has the ``_toBytes``
+    method, which will prompt it to execute that method of the complex object. Of
+    course, this means that you can return anything, not necessarily bytes, but to
+    maintain intuitiveness, you should return either bytes or iterator of bytes
+
 :param imgType: if input is an image then this is the image type. Can
     change to "PNG" or sth like that"""                                          # toBytes
         self.imgType = imgType                                                   # toBytes
     def __ror__(self, it):                                                       # toBytes
         if isinstance(it, str): return it.encode()                               # toBytes
         if hasPIL:                                                               # toBytes
             if isinstance(it, PIL.Image.Image):                                  # toBytes
-                it = it | toRgb()                                                # toBytes
-                buffered = io.BytesIO()                                          # toBytes
-                it.save(buffered, format=self.imgType)                           # toBytes
-                return buffered.getvalue()                                       # toBytes
-        import dill                                                              # toBytes
-        return dill.dumps(it)                                                    # toBytes
+                it = it | toRgb(); buffered = io.BytesIO()                       # toBytes
+                it.save(buffered, format=self.imgType); return buffered.getvalue() # toBytes
+        if hasattr(it, "_toBytes"): return it._toBytes()                         # toBytes
+        import dill; return dill.dumps(it)                                       # toBytes
 class toHtml(BaseCli):                                                           # toHtml
     def __init__(self):                                                          # toHtml
         """Converts several object types to bytes.
 Example::
 
     # converts PIL image to html <img> tag
     torch.randn(200, 100) | toImg() | toHtml()
@@ -501,7 +550,28 @@
     "abc" | toHash() # returns 'gASVJAAAAAAAAABDILp4Fr+PAc/qQUFA3l2uIiOwA2Gjlhd6nLQQ/2HyABWtlC4='
 
 Why not just use the builtin function ``hash("abc")``? Because it generates different
 hashes for different interpreter sessions, and that breaks many of my applications that
 need the hash value to stay constant forever."""                                 # toHash
     def hashF(msg:str) -> str: m = hashlib.sha256(); m.update(f"{msg}".encode()); return k1lib.encode(m.digest()) # toHash
     return cli.aS(hashF)                                                         # toHash
+import csv; pd = k1lib.dep("pandas")                                             # toHash
+class toCsv(BaseCli):                                                            # toCsv
+    def __init__(self, allSheets=False):                                         # toCsv
+        """Converts a csv file name into a table.
+Example::
+
+    "abc.csv"  | toCsv()     # returns table of values
+    "def.xlsx" | toCsv()     # returns table of values in the first sheet
+    "def.xlsx" | toCsv(True) # returns List[Sheet name (str), table of values]
+
+:param allSheets: if input is an Excel sheet, whether to read in all sheets or
+    just the first sheet. No effect if input is a normal csv file"""             # toCsv
+        self.allSheets = allSheets                                               # toCsv
+    def __ror__(self, fn:str):                                                   # toCsv
+        fn = os.path.expanduser(fn)                                              # toCsv
+        if fn.endswith(".xls") or fn.endswith(".xlsx"):                          # toCsv
+            if self.allSheets: return [[k, v.values] for k,v in pd.read_excel(fn, sheet_name=None).items()] # toCsv
+            else: return pd.read_excel(fn).values                                # toCsv
+        def gen():                                                               # toCsv
+            with open(fn) as f: yield from csv.reader(f)                         # toCsv
+        return gen()                                                             # toCsv
```

### Comparing `k1lib-1.4.2/k1lib/cli/filt.py` & `k1lib-1.4.3/k1lib/cli/filt.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,27 @@
     # returns [[2, 'a'], [6, 'c']], grabbing all the even elements in the 1st column
     [[2, "a"], [3, "b"], [5, "a"], [6, "c"]] | filt(lambda x: x%2 == 0, 0) | deref()
     # throws error, because strings can't mod divide
     [1, 2, "b", 8] | filt(lambda x: x % 2 == 0) | deref()
     # returns [2, 8]
     [1, 2, "b", 8] | filt(lambda x: x % 2 == 0, catchErrors=True) | deref()
 
-You can also pass in :class:`~k1lib.cli.modifier.op`, for extra intuitiveness::
+You can also pass in :class:`~k1lib.cli.modifier.op` or string, for extra intuitiveness and quickness::
 
     # returns [2, 6]
     [2, 3, 5, 6] | filt(op() % 2 == 0) | deref()
     # returns ['abc', 'a12']
     ["abc", "def", "a12"] | filt(op().startswith("a")) | deref()
     # returns [3, 4, 5, 6, 7, 8, 9]
     range(100) | filt(3 <= op() < 10) | deref()
+    # returns [3, 4, 5, 6, 7, 8, 9]
+    range(100) | filt("3 <= x < 10") | deref()
 
-If you pass in :class:`numpy.ndarray` or :class:`torch.Tensor`, then it will
+See :class:`~k1lib.cli.modifier.aS` for more details on string mode. If you
+pass in :class:`numpy.ndarray` or :class:`torch.Tensor`, then it will
 automatically use the C-accelerated versions if possible, like this::
 
     # returns np.array([2, 3, 4]), instead of iter([2, 3, 4])
     np.array([1, 2, 3, 4]) | filt(lambda x: x>=2) | deref()
     # returns [2, 3, 4], instead of np.array([2, 3, 4]), because `math.exp` can't operate on numpy arrays
     np.array([1, 2, 3, 4]) | filt(lambda x: math.exp(x) >= 3) | deref()
 
@@ -312,38 +315,47 @@
 
 ... you can use the shorthand :class:`~k1lib.cli.utils.rItem` instead::
 
     iter(range(10)) | rItem(3) # returns 3
 
 :param rows: ints for the row indices"""                                         # rows
         if len(rows) == 1 and isinstance(rows[0], slice):                        # rows
-            self.slice = rows[0]; self.idxMode = False                           # rows
-        else: self.rows = rows; self.sortedRows = sorted(rows); self.idxMode = True # rows
+            self.slice = rows[0]; self.rows = None; self.idxMode = False         # rows
+        else: self.slice = None; self.rows = rows; self.sortedRows = sorted(rows); self.idxMode = True # rows
         self.inverted = False                                                    # rows
     def __getitem__(self, _slice):                                               # rows
         start, stop, step = _slice.start, _slice.stop, _slice.step               # rows
         if step == None or step == 1:                                            # rows
             if start == None and stop == None: return cli.iden()                 # rows
             if start == None: return head(stop)                                  # rows
             if stop == None: return ~head(start)                                 # rows
         elif step == 0: return cli.ignore()                                      # rows
         answer = rows(_slice); answer.inverted = self.inverted; return answer    # rows
+    def _all_array_opt(self, it, level:int):                                     # rows
+        a = np.array(self.rows) if self.rows else self.slice; s = [slice(None, None, None)]*level # rows
+        if self.inverted: mask = np.ones(it.shape[level], dtype=bool); mask[a] = False; return it[(*s, mask)] # rows
+        return it[(*s, a)]                                                       # rows
     def __invert__(self): self.inverted = not self.inverted; return self         # rows
     def __ror__(self, it:Iterator[str]):                                         # rows
-        if not self.inverted:                                                    # rows
-            if self.idxMode:                                                     # rows
-                it = list(it) if self.sortedRows[0] < 0 else lazyList(it)        # rows
-                for idx in self.rows: yield it[idx]                              # rows
-            else: yield from list(it)[self.slice]                                # rows
-        else:                                                                    # rows
-            it = list(it); n = len(it)                                           # rows
-            if self.idxMode:                                                     # rows
-                idxs = set((e if e >= 0 else n+e) for e in self.rows)            # rows
-            else: idxs = set(range(n)[self.slice])                               # rows
-            yield from (e for i, e in enumerate(it) if i not in idxs)            # rows
+        idxMode = self.idxMode; inverted = self.inverted; sl = self.slice; rw = self.rows # rows
+        def gen(it):                                                             # rows
+            if not inverted:                                                     # rows
+                if idxMode:                                                      # rows
+                    if len(self.sortedRows) == 0: return                         # rows
+                    it = list(it) if self.sortedRows[0] < 0 else lazyList(it)    # rows
+                    for idx in rw: yield it[idx]                                 # rows
+                else: yield from list(it)[sl]                                    # rows
+            else:                                                                # rows
+                it = list(it); n = len(it); idxs = set((e if e >= 0 else n+e) for e in rw) if idxMode else set(range(n)[sl]) # rows
+                yield from (e for i, e in enumerate(it) if i not in idxs)        # rows
+        if isinstance(it, settings.arrayTypes):                                  # rows
+            a = np.array(rw) if rw else sl                                       # rows
+            if inverted: mask = np.ones(len(it), dtype=bool); mask[a] = False; return it[mask] # rows
+            else: return it[a]                                                   # rows
+        return gen(it)                                                           # rows
 class cut(BaseCli):                                                              # cut
     def __init__(self, *columns:List[int]):                                      # cut
         """Cuts out specific columns, sliceable. Examples::
 
     ["0123456789", "abcdefghij"] | cut(5, 8) | deref() # returns [['5', '8'], ['f', 'i']]
     ["0123456789", "abcdefghij"] | cut(8, 5) | deref() # returns [['8', '5'], ['i', 'f']], demonstrating permutation-safe
     ["0123456789"] | cut(5, 8) | deref() # returns [['5', '8']]
@@ -400,16 +412,20 @@
     But when applied to the second row, it now carries the meaning ~4, instead of ~(-3).
 
     Why don't I just fix these edge cases? Because the run time for it would be completely unacceptable,
     as we'd have to figure out what's the columns to include in the result for every row. This could
     easily be O(n^3). Of course, with more time optimizing, this could be solved, but this is the only
     extreme edge case and I don't feel like putting in the effort to optimize it.""" # cut
         super().__init__()                                                       # cut
-        if len(columns) == 1 and isinstance(columns[0], slice): columns = columns[0] # cut
+        if len(columns) == 1 and isinstance(columns[0], slice): columns = columns[0] # columns is either a slice object, or a list of ints # cut
         self.columns = columns; self.inverted = False # columns: list[int] | slice # cut
+    def _all_array_opt(self, it, level):                                         # cut
+        c = self.columns; r = rows(c) if isinstance(c, slice) else rows(*c)      # cut
+        if self.inverted: r = ~r                                                 # cut
+        it = it | r.all(level+1); return (it | cli.item().all(level+1)) if not isinstance(c, slice) and len(c) == 1 else it # cut
     def __ror__(self, it):                                                       # cut
         columns = self.columns; inverted = self.inverted                         # cut
         isArray = isinstance(it, settings.arrayTypes)#; isArray = False          # cut
         if isArray: nCols = len(it[0]); prs = rs = range(nCols) # range(nColumns). "prs" for padded rs # cut
         else: # carefully peaking first row and get the number of columns        # cut
             it = iter(it); sentinel = object(); row = next(it, sentinel)         # cut
             if row is sentinel: return []                                        # cut
@@ -421,26 +437,35 @@
         columns = [e if e >= 0 else nCols + e for e in columns] # clear negative indicies # cut
         if self.inverted: columns = list(set(e for e in prs if e not in columns)) # cut
         if len(columns) == 1: c = columns[0]; return it[:,c] if isArray else (r[c] for r in (list(row) for row in it) if len(r) > c) # cut
         else: return it[:,columns] if isArray else ([row[c] for c in columns if c < len(row)] for row in (list(row) for row in it)) # cut
     def __getitem__(self, idx): answer = cut(idx); answer.inverted = self.inverted; return answer # cut
     def __invert__(self): self.inverted = not self.inverted; return self         # cut
 class intersection(BaseCli):                                                     # intersection
-    def __init__(self, column=None):                                             # intersection
+    def __init__(self, column=None, full=False):                                 # intersection
         """Returns the intersection of multiple streams.
 Example::
 
     # returns set([2, 4, 5])
     [[1, 2, 3, 4, 5], [7, 2, 4, 6, 5]] | intersection()
     # returns ['2g', '4h', '5j']
     [["1a", "2b", "3c", "4d", "5e"], ["7f", "2g", "4h", "6i", "5j"]] | intersection(0) | deref()
 
+If you want the full distribution, meaning the intersection, as well
+as what's left of each stream, you can do something like this::
+
+    # returns [{2, 4, 5}, [1, 3], [7, 6]]
+    [[1, 2, 3, 4, 5], [7, 2, 4, 6, 5]] | intersection(full=True) | deref()
+
 :param column: what column to apply the intersection
-    on. Defaulted to None"""                                                     # intersection
+    on. Defaulted to None
+:param full: if specified, return the full distribution, instead of the intersection alone""" # intersection
         super().__init__(); self.column = column                                 # intersection
+        self.full = full                                                         # intersection
+        self.f = intersection(column, False) if full else None                   # intersection
     def _typehint(self, inp):                                                    # intersection
         if self.column is None:                                                  # intersection
             if isinstance(inp, tArrayTypes): return tSet(inp.child)              # intersection
             if isinstance(inp, tListIterSet):                                    # intersection
                 if isinstance(inp.child, tListIterSet):                          # intersection
                     return tSet(inp.child.child)                                 # intersection
                 return tSet(tAny())                                              # intersection
@@ -449,15 +474,20 @@
                 for e in inp.children:                                           # intersection
                     if not isinstance(e, tListIterSet): return tSet(tAny())      # intersection
                     if e.child != a.child: return tSet(tAny())                   # intersection
                 return tSet(a.child)                                             # intersection
             return tSet(tAny());                                                 # intersection
         else: return tAny()                                                      # intersection
     def __ror__(self, its:Iterator[Iterator[Any]]) -> Set[Any]:                  # intersection
-        c = self.column                                                          # intersection
+        c = self.column; full = self.full; f = self.f                            # intersection
+        if full:                                                                 # intersection
+            if c is None:                                                        # intersection
+                its = its | cli.deref(2); inter = its | f                        # intersection
+                return [inter, *((e for e in it if e not in inter) for it in its)] # intersection
+            else: raise Exception("intersection(int, True) mode not supported yet, as it's a little ambiguous what's the use case is, and there're many styles of functionality that this can take on") # intersection
         if c is None:                                                            # intersection
             answer = None                                                        # intersection
             for it in its:                                                       # intersection
                 if answer is None: answer = set(it); continue                    # intersection
                 answer = answer.intersection(it)                                 # intersection
             return set() if answer is None else answer                           # intersection
         else:                                                                    # intersection
@@ -499,24 +529,28 @@
 :param column: the column to detect unique elements. Can be
     None, which will behave like converting the input iterator
     into a set, but this cli will maintain the order"""                          # unique
         super().__init__(); self.column = column                                 # unique
     def __ror__(self, it):                                                       # unique
         c = self.column                                                          # unique
         if c is None:                                                            # unique
-            terms = set()                                                        # unique
-            for e in it:                                                         # unique
-                if e not in terms: yield e                                       # unique
-                terms.add(e)                                                     # unique
+            if isinstance(it, settings.arrayTypes): bm = np if isinstance(it, np.ndarray) else (torch if hasTorch and isinstance(it, torch.Tensor) else None); return bm.unique(it) # unique
+            def gen():                                                           # unique
+                terms = set()                                                    # unique
+                for e in it:                                                     # unique
+                    if e not in terms: yield e                                   # unique
+                    terms.add(e)                                                 # unique
         else:                                                                    # unique
-            terms = set()                                                        # unique
-            for row in it:                                                       # unique
-                row = list(row); e = row[c]                                      # unique
-                if e not in terms: yield row                                     # unique
-                terms.add(e)                                                     # unique
+            def gen():                                                           # unique
+                terms = set()                                                    # unique
+                for row in it:                                                   # unique
+                    row = list(row); e = row[c]                                  # unique
+                    if e not in terms: yield row                                 # unique
+                    terms.add(e)                                                 # unique
+        return gen()                                                             # unique
 class breakIf(BaseCli):                                                          # breakIf
     def __init__(self, f):                                                       # breakIf
         """Breaks the input iterator if a condition is met.
 Example::
 
     # returns [0, 1, 2, 3, 4, 5]
     [*range(10), 2, 3] | breakIf(lambda x: x > 5) | deref()"""                   # breakIf
```

### Comparing `k1lib-1.4.2/k1lib/cli/gb.py` & `k1lib-1.4.3/k1lib/cli/gb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/grep.py` & `k1lib-1.4.3/k1lib/cli/grep.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/init.py` & `k1lib-1.4.3/k1lib/cli/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 - Replace with last recorded ``4 in op()``, if ``f`` is :data:`True`, because Python does
   not allow returning complex objects from __contains__ method
 - Solidifies every :class:`~k1lib.cli.modifier.op`.
 
 :param capture: whether to capture all clis to the right of it and make it accessible under capturedClis and capturedSerial properties""" # BaseCli
         if isinstance(fs, tuple): raise AttributeError("`fs` should not be a tuple. Use a list instead, so that new functions can be returned") # BaseCli
         _k1_init_l = []                                                          # BaseCli
-        for _k1_init_f in fs: cli.op.solidify(_k1_init_f); _k1_init_l.append(_k1_init_f) # BaseCli
+        for _k1_init_f in fs: cli.op.solidify(_k1_init_f); _k1_init_l.append(_k1_init_f) # this is supposed to turn the exotic function into a normal function and leave normal functions alone. Purposefully don't do heavy optimizations here, cause we might want to poke around and change its internal representation # BaseCli
         fs.clear(); fs.extend(_k1_init_l);                                       # BaseCli
         self.capture = capture; self._capturedClis = []; self._capturedSerial = None # BaseCli
     @property                                                                    # BaseCli
     def capturedClis(self):                                                      # BaseCli
         if isinstance(self._capturedClis, list):                                 # BaseCli
             ans = []                                                             # BaseCli
             for e in self._capturedClis: ans.append(cli.op.solidify(e))          # BaseCli
```

### Comparing `k1lib-1.4.2/k1lib/cli/inp.py` & `k1lib-1.4.3/k1lib/cli/inp.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,69 +105,123 @@
             try: return requests.head(self.url, timeout=self.timeout).headers.items() | cli.apply(cli.op().lower(), 0) | cli.toDict() | cli.op()["content-length"].ab_int() # RemoteFile
             except Exception as e:                                               # RemoteFile
                 if i >= self.retries: raise Exception(f"Can't get size of remote file: {e}") # RemoteFile
     def __len__(self):                                                           # RemoteFile
         if self.size is None: self.size = self._getSize()                        # RemoteFile
         return self.size                                                         # RemoteFile
     def __repr__(self): return f"<RemoteFile url={self.url} size={k1lib.fmt.size(len(self))}>" # RemoteFile
-@contextmanager                                                                  # RemoteFile
+import zipfile, inspect                                                          # RemoteFile
+class ZipWrapper:                                                                # ZipWrapper
+    def __init__(self, a, zfn): self.a = a; self.zfn = zfn                       # ZipWrapper
+    def __repr__(self):                                                          # ZipWrapper
+        a = self.a; s = f" ({round(a.compress_size/a.file_size*100)}%)" if a.file_size > 0 else "" # ZipWrapper
+        return f"<Zip subfile name='{a.filename}' {k1lib.fmt.size(a.file_size)} -> {k1lib.fmt.size(a.compress_size)}{s}>" # ZipWrapper
+    @property                                                                    # ZipWrapper
+    def size(self): return a.file_size                                           # ZipWrapper
+    @property                                                                    # ZipWrapper
+    def compressedSize(self): return a.compress_size                             # ZipWrapper
+    def _catHandle(self):                                                        # ZipWrapper
+        with zipfile.ZipFile(self.zfn) as zipf:                                  # ZipWrapper
+            with zipf.open(self.a.filename) as subfile:                          # ZipWrapper
+                yield subfile                                                    # ZipWrapper
+@contextmanager                                                                  # ZipWrapper
 def openFile(fn, text, noPartialConfirm=False): # can be actual file or url      # openFile
-    if not isinstance(fn, str): yield fn; return # file handle case, just return itself # openFile
+    if not isinstance(fn, str):                                                  # openFile
+        if hasattr(fn, "_catHandle"): yield from fn._catHandle(); return # custom datatype case # openFile
+        else: yield fn; return # file handle case, just return itself            # openFile
     if os.path.exists(fn):                                                       # openFile
         if text:                                                                 # openFile
             with open(fn, "r", settings.cat.chunkSize) as f: yield f             # openFile
         else:                                                                    # openFile
             with open(fn, "rb", settings.cat.chunkSize) as f: yield f            # openFile
     elif validators.url(fn) is True:                                             # openFile
         yield RemoteFile(fn, False, noPartialConfirm=noPartialConfirm)           # openFile
     else: raise FileNotFoundError(f"The file {fn} doesn't seem to exist and/or it's not a valid url") # openFile
 def _catGenText(fn, sB, eB): # fn for "file name"                                # _catGenText
     try:                                                                         # _catGenText
         if sB == 0 and eB == -1: # fast path without bounds (90-160 MB/s expected) # _catGenText
             with openFile(fn, True) as f:                                        # _catGenText
-                while True:                                                      # _catGenText
-                    line = f.readline()                                          # _catGenText
-                    if line == "": return                                        # _catGenText
-                    yield line[:-1] if line[-1] == "\n" else line                # _catGenText
+                line = f.readline()                                              # _catGenText
+                if isinstance(line, str): # why put the if outside the loop? Speed reasons. Also, isn't .readline() supposed to return a string? Well, cause we're supporting random file handles from custom datatypes, some asshole file handles might return bytes instead # _catGenText
+                    while True:                                                  # _catGenText
+                        if line == "": return                                    # _catGenText
+                        yield line[:-1] if line[-1] == "\n" else line            # _catGenText
+                        line = f.readline()                                      # _catGenText
+                else:                                                            # _catGenText
+                    while True:                                                  # _catGenText
+                        line = line.decode()                                     # _catGenText
+                        if line == "": return                                    # _catGenText
+                        yield line[:-1] if line[-1] == "\n" else line            # _catGenText
+                        line = f.readline()                                      # _catGenText
         else: # slow path with bounds (15 MB/s expected). Update: much faster now, expect only 40% slower than the path above # _catGenText
             sB = wrap(fn, sB); eB = wrap(fn, eB)                                 # _catGenText
             with openFile(fn, True) as f:                                        # _catGenText
                 f.seek(sB); b = sB # current byte                                # _catGenText
-                while True:                                                      # _catGenText
-                    line = f.readline(); b += len(line)                          # _catGenText
-                    if line == "": return                                        # _catGenText
-                    if b > eB: yield line[:len(line)-(b-eB)]; return             # _catGenText
-                    yield line[:-1] if line[-1] == "\n" else line                # _catGenText
+                line = f.readline()                                              # _catGenText
+                if isinstance(line, str):                                        # _catGenText
+                    while True:                                                  # _catGenText
+                        b += len(line)                                           # _catGenText
+                        if len(line) == 0: return                                # _catGenText
+                        if b > eB: yield line[:len(line)-(b-eB)]; return         # _catGenText
+                        yield line[:-1] if line[-1] == "\n" else line            # _catGenText
+                        line = f.readline()                                      # _catGenText
+                else:                                                            # _catGenText
+                    while True:                                                  # _catGenText
+                        line = line.decode()                                     # _catGenText
+                        b += len(line)                                           # _catGenText
+                        if len(line) == 0: return                                # _catGenText
+                        if b > eB: yield line[:len(line)-(b-eB)]; return         # _catGenText
+                        yield line[:-1] if line[-1] == "\n" else line            # _catGenText
+                        line = f.readline()                                      # _catGenText
     except FileNotFoundError: pass                                               # _catGenText
 def _catGenBin(fn, sB, eB):                                                      # _catGenBin
     chunkSize = settings.cat.chunkSize; sB = wrap(fn, sB); eB = wrap(fn, eB); nB = eB - sB # number of bytes to read total # _catGenBin
     with openFile(fn, False) as f:                                               # _catGenBin
         f.seek(sB); nChunks = math.ceil(nB / chunkSize); lastChunkSize = nB - chunkSize*(nChunks-1) # _catGenBin
         # had to do this because RemoteFile is actually not thread-safe          # _catGenBin
         # applyF = (lambda f_: cli.apply(f_)) if isinstance(f, RemoteFile) else (lambda f_: cli.applyTh(f_, prefetch=10)) # _catGenBin
         applyF = (lambda f_: cli.apply(f_)) # actually, normal reads are not thread-safe either. Stupid me # _catGenBin
         yield from range(nChunks) | applyF(lambda i: f.read(chunkSize) if i < nChunks-1 else f.read(chunkSize)[:lastChunkSize]) # _catGenBin
 def fileLength(fn):                                                              # fileLength
     with openFile(fn, False) as f: return f.seek(0, os.SEEK_END)                 # fileLength
 def wrap(fn, b): return b if b >= 0 else b + fileLength(fn) + 1                  # wrap
 class _cat(BaseCli):                                                             # _cat
-    def __init__(self, text, chunks, sB, eB): self.text = text; self.chunks = chunks; self.sB = sB; self.eB = eB # _cat
+    def __init__(self, text, chunks, sB, eB):                                    # _cat
+        super().__init__(capture=True)                                           # _cat
+        self.text = text; self.chunks = chunks; self.sB = sB; self.eB = eB       # _cat
     def _typehint(self, ignored=None):                                           # _cat
         if self.text: return tIter(str) if self.chunks else tList(str)           # _cat
         else: return tIter(bytes) if self.chunks else bytes                      # _cat
     def __ror__(self, fn:Union[str, "fileHandle"]) -> Union[Iterator[str], bytes]: # _cat
-        text = self.text; chunks = self.chunks; sB = self.sB; eB = self.eB; fn = os.path.expanduser(fn) if isinstance(fn, str) else fn # _cat
+        ser = self.capturedSerial; text = self.text; chunks = self.chunks; sB = self.sB; eB = self.eB # _cat
+        if not isinstance(fn, str) and hasattr(fn, "_cat"): # custom datatype, _cat method defined, so it will take control of things # _cat
+            kwargs = {"text": text, "chunks": chunks, "sB": sB, "eB": eB}        # _cat
+            kwdiff = [a for a, b in [["text",text!=True], ["chunks",chunks!=True if text else chunks!=False], ["sB",sB!=0], ["eB",eB!=-1]] if b] # _cat
+            args = inspect.getfullargspec(fn._cat).args[1:]; n = len(args)       # _cat
+            s = set(["ser", "kwargs"]); weirdArgs = [a for a in args if a not in s] # _cat
+            if len(weirdArgs) > 0: raise Exception(f"Custom datatype `{type(fn)}` has ._cat() method, which expects only `ser` and `kwargs` arguments, but detected these arguments instead: {weirdArgs}. Please fix `{type(fn)}`") # _cat
+            def guard():                                                         # _cat
+                if kwdiff: raise Exception(f"Custom datatype `{type(fn)}` does not support custom cat() arguments like {kwdiff}") # _cat
+            if n == 0: guard(); return fn._cat() | ser                           # _cat
+            elif n == 1:                                                         # _cat
+                if args[0] == "ser": guard(); return fn._cat(ser)                # _cat
+                if args[0] == "kwargs": return fn._cat(kwargs) | ser             # _cat
+            elif n == 2:                                                         # _cat
+                if args[0] == "ser": return fn._cat(ser, kwargs)                 # _cat
+                else: return fn._cat(kwargs, ser)                                # _cat
+            else: raise Exception("Unreachable")                                 # _cat
+        fn = os.path.expanduser(fn) if isinstance(fn, str) else fn               # _cat
         if text and chunks and k1lib._settings.packages.k1a and isinstance(fn, str) and os.path.exists(fn): # _cat
-            return k1lib._k1a.k1a.StrIterCat(fn, sB, eB) # accelerated C version # _cat
-        if chunks: return _catGenText(fn, sB, eB) if text else _catGenBin(fn, sB, eB) # _cat
+            return k1lib._k1a.k1a.StrIterCat(fn, sB, eB) | ser # accelerated C version # _cat
+        if chunks: return _catGenText(fn, sB, eB) if text else _catGenBin(fn, sB, eB) | ser # _cat
         sB = wrap(fn, sB); eB = wrap(fn, eB)                                     # _cat
         if text:                                                                 # _cat
-            with openFile(fn, True) as f: f.seek(sB); return f.read(eB-sB).splitlines() # _cat
+            with openFile(fn, True) as f: f.seek(sB); return f.read(eB-sB).splitlines() | ser # _cat
         else:                                                                    # _cat
-            with openFile(fn, False) as f: f.seek(sB); return f.read(eB-sB)      # _cat
+            with openFile(fn, False) as f: f.seek(sB); return f.read(eB-sB) | ser # _cat
 class Profile(BaseCli):                                                          # Profile
     def __init__(self, text): self.data = []; self.text = text                   # Profile
     def __ror__(self, it):                                                       # Profile
         fmt = k1lib.fmt; chars = 0; beginTime = time.time()                      # Profile
         if self.text:                                                            # Profile
             a, b, c, d, f = k1lib.ConstantPad.multi(5); every = settings.cat.every.text # Profile
             for lines, e in enumerate(it):                                       # Profile
@@ -225,24 +279,124 @@
 threads/processes, then you can use this cli in conjunction with :class:`splitSeek`.
 
 If you are dumping multiple pickled objects into a single file, you can read all
 of them using :meth:`cat.pickle`.
 
 This cli has lots of settings at :data:`~k1lib.settings`.cli.cat
 
+See also: :meth:`ls`
+
+.. admonition:: Custom datatype
+
+    It is possible to build objects that can interoperate with this cli,
+    like this::
+
+        class custom1:
+            def __init__(self, config=None): ...
+            def _cat(self): return ["abc", "def"]
+
+        custom1() |  cat()           # returns ["abc", "def"]
+        custom1() |  cat() | item()  # returns "abc"
+        custom1() | (cat() | item()) # returns "abc"
+
+    When called upon, :meth:`cat` will see that the input is not a simple string, which
+    will prompt it to look for ``_cat()`` method of the complex object and execute it.
+    By default, if the user specifies any non-default arguments like ``text=False``,
+    it will errors out because :meth:`cat` does not know how to handle it. Here's how
+    to do it right::
+
+        class custom2:
+            def __init__(self, config=None): ...
+            def _cat(self, kwargs): # default kwargs if user doesn't specify anything else is `{"text": True, "chunks": None, "sB": 0, "eB": -1}`
+                if kwargs["text"]: return ["abc", "def"]
+                else: return [b"abc", b"def"]
+
+        custom2() |  cat()                     # returns ["abc", "def"]
+        custom2() |  cat()           | item()  # returns "abc"
+        custom2() | (cat()           | item()) # returns "abc"
+        custom2() |  cat(text=False)           # returns [b"abc", b"def"]
+        custom2() |  cat(text=False) | item()  # returns b"abc"
+
+    Here, you're saying that your function can handle non-standard arguments, so
+    :meth:`cat` will give you all the args. You may support only some arguments
+    and completely ignore others, it's all up to you. Might still be worth it to
+    throw some errors warning users of arguments your custom datatype does not support.
+
+    You can also capture future clis like this::
+
+        class custom3:
+            def __init__(self, config=None): ...
+            def _cat(self, ser):            # "ser" stands for "serial"
+                if len(ser.clis) == 1 and isinstance(ser.clis[0], item):
+                    return "123"            # fancy optimization
+                return ["abc", "def"] | ser # default "slow" base case
+
+        custom3() |  cat()           # returns ["abc", "def"]
+        custom3() |  cat() | item()  # returns "abc", because cat() did not capture any clis
+        custom3() | (cat() | item()) # returns "123", which might be desireable, up to you
+
+    This feature is pretty advanced actually, in that you can actually do different
+    things based on future processing tasks. Let's say that the captured cli looks like
+    ``cut(3) | batched(10) | rItem(3)``. This essentially means "give me elements 30
+    through 39 from the 4th column". With this information, you can query your custom
+    database for exactly those elements only, while fetching nothing else, which would be
+    great for performance.
+
+    You can also outright lie to the user like in the example, where if :class:`~k1lib.cli.utils.item`
+    is detected, it will return a completely different version ("123") while it should return
+    "abc" instead. The possibilities are endless. As you can probably feel, it's super hard to
+    actually utilize this in the right way without breaking something, as you are completely
+    responsible for the captured clis. Let's see another example::
+
+        class custom4:
+            def __init__(self, config=None): ...
+            def _cat(self, ser):
+                return ["abc", "def"]
+
+        custom4() |  cat()           # returns ["abc", "def"]
+        custom4() |  cat() | item()  # returns "abc"
+        custom4() | (cat() | item()) # returns ["abc", "def"]
+
+    Same story as ``custom3``, demonstrating that if you declare that you want to see and
+    manipulate ``ser``, you'll be completely responsible for it, and if you don't handle it
+    correctly, it will create horrible bugs. You can, of course, have access to ``ser`` and
+    ``kwargs`` at the same time::
+
+        class custom5:
+            def __init__(self, config=None): ...
+            def _cat(self, ser, kwargs): return ["abc", "def"] | ser
+
+    If your custom datatype feels like a block device, and you don't want to rewrite all
+    the functionalities in :meth:`cat`, you can implement the method ``_catHandle`` that
+    yields the custom file handle instead::
+
+        class custom6:
+            def __init__(self, config=None): ...
+            def _catHandle(self): yield io.BytesIO(b"abc\\ndef\\n123")
+        class custom7:
+            def __init__(self, config=None): ...
+            def _catHandle(self): yield io.StringIO("abc\\ndef\\n123")
+
+        custom6() | cat(text=False) # returns b'abc\\ndef\\n123'
+        custom7() | cat() | deref() # returns ['abc', 'def', '123']
+
+    Remember that you have to yield instead of returning the file handle. This is so that
+    you can use ``with`` statements, and if you return the file handle, the file might be
+    closed by the time :meth:`cat` decides to use it.
+
 :param fileName: if None, then return a :class:`~k1lib.cli.init.BaseCli`
     that accepts a file name and outputs Iterator[str]
 :param text: if True, read text file, else read binary file
 :param chunks: if True then reads the file chunk by chunk, else reads the
     entire file. Defaults to True in text mode and False in binary mode
 :param profile: whether to profile the file reading rate or not. Can adjust
     printing frequency using `settings.cli.cat.every`
 :param sB: "start byte". Specify this if you want to start reading from this byte
 :param eB: "end byte", exclusive. Default -1 means end of file"""                # cat
-    if chunks is None: chunks = True if text else False                          # cat
+    if chunks is None: chunks = True if text else False # dev note: if default arguments are changed, please also change _cat()'s implementation for custom datatypes # cat
     if profile and not chunks: warnings.warn(f"Can't profile reading rate when you're trying to read everything at once"); profile = False # cat
     f = _cat(text, chunks, sB, eB)                                               # cat
     if profile: f = f | Profile(text)                                            # cat
     return f if fileName is None else fileName | f                               # cat
 def _catPickle(fileName=None, pickleModule=dill):                                # _catPickle
     """Reads a file as a series of pickled objects.
 Example::
@@ -463,22 +617,56 @@
 Example::
 
     # returns List[str]
     ls("/home")
     # same as above
     "/home" | ls()
     # only outputs files, not folders
-    ls("/home") | filt(os.path.isfile)"""                                        # ls
+    ls("/home") | filt(os.path.isfile)
+
+This can handle things that are not plain folders. For example,
+it can handle zip file whereby it will list out all the files contained
+within a particular .zip::
+
+    ls("abc.zip")
+
+Then, you can use :meth:`cat` as usual, like this::
+
+    ls("abc.zip") | item() | cat()
+
+Pretty nice!
+
+.. admonition:: Custom datatype
+
+    It is possible to build objects that can interoperate with this cli,
+    like this::
+
+        class sql:
+            def __init__(self): ...
+            def _ls(self): return ["something", "here"]
+
+    ls() will identify that what's inputted is not a string, and will try
+    to execute the object's "_ls()" method, so you can just simply implement
+    it in your classes
+"""                                                                              # ls
     if folder is None: return _ls()                                              # ls
     else: return folder | _ls()                                                  # ls
 class _ls(BaseCli):                                                              # _ls
     def _typehint(self, ignored=None): return tList(str)                         # _ls
     def __ror__(self, path:str):                                                 # _ls
-        path = os.path.expanduser(path.rstrip(os.sep))                           # _ls
-        return [f"{path}{os.sep}{e}" for e in os.listdir(path)]                  # _ls
+        if isinstance(path, str):                                                # _ls
+            path = os.path.expanduser(path.rstrip(os.sep))                       # _ls
+            if os.path.exists(path):                                             # _ls
+                if os.path.isfile(path):                                         # _ls
+                    if cat(path, False, eB=2) == b"PK": # list subfiles in a zip file # _ls
+                        return [ZipWrapper(e, path) for e in zipfile.ZipFile(path).infolist()] # _ls
+                    else: raise Exception(f"{path} is a file, not a folder, so can't list child directories") # _ls
+                else: return [f"{path}{os.sep}{e}" for e in os.listdir(path)]    # _ls
+            else: return []                                                      # _ls
+        else: return path._ls()                                                  # _ls
 k1lib.settings.cli.add("quiet", False, "whether to mute extra outputs from clis or not") # _ls
 newline = b'\n'[0]                                                               # _ls
 class lazySt:                                                                    # lazySt
     def __init__(self, st, text:bool):                                           # lazySt
         """Converts byte stream into lazy text/byte stream, with nice __repr__.""" # lazySt
         self.st = st; self.text = text;                                          # lazySt
     def __iter__(self):                                                          # lazySt
@@ -635,15 +823,14 @@
     base = base.rstrip("/\\")                                                    # urlPath
     def inner(url):                                                              # urlPath
         p = urllib.parse.urlparse(url)                                           # urlPath
         a = (p.netloc.replace(".", "_") + os.sep) if host else ""                # urlPath
         return f"{base}{os.sep}{a}{p.path.strip('/')}".replace("//", "/")        # urlPath
     return cli.aS(inner)                                                         # urlPath
 import bz2, gzip, zlib                                                           # urlPath
-puremagic = k1lib.dep("puremagic")                                               # urlPath
 class kzip(BaseCli):                                                             # kzip
     def __init__(self, fmt="gz"):                                                # kzip
         """Incrementally compresses a stream of data using gzip or bzip2.
 Example::
 
     data = range(100) | apply(lambda x: str(x).encode()) | deref() # list of bytes
     data | kzip() | deref() # returns list of bytes
@@ -681,75 +868,102 @@
             try:                                                                 # kzip
                 res = o.flush()                                                  # kzip
                 if res: yield res                                                # kzip
             except: pass                                                         # kzip
         if isinstance(it, str): it = it.encode()                                 # kzip
         if isinstance(it, bytes): return [o.compress(it), o.flush()] | cli.filt("x") | cli.aS(b"".join) # kzip
         else: return gen()                                                       # kzip
-class decompressobj:                                                             # decompressobj
+class decompressobj: # .gz or .bz2 file                                          # decompressobj
     """
 Why not just use zlib.decompressobj() directly? I encountered a strange bug when trying
 to decompress CommonCrawl's gzip files, posted on Stack Overflow and got help from none
 other than Mark Adler, creator of gzip and zlib. That guy's super active on Stack Overflow.
 Anyway, this code here is a modified version of his code. Here's the discussion:
 https://stackoverflow.com/questions/76452480/pythons-zlib-doesnt-work-on-commoncrawl-file
 """                                                                              # decompressobj
     def __init__(self, gz=True): self.gz = gz                                    # decompressobj
     def __ror__(self, it):                                                       # decompressobj
         gz = self.gz; data = left = b''; o = zlib.decompressobj(zlib.MAX_WBITS|32) if gz else bz2.BZ2Decompressor() # decompressobj
         for got in it:                                                           # decompressobj
             yield o.decompress(left + got); left = b''                           # decompressobj
             if o.eof: left = o.unused_data; o = zlib.decompressobj(zlib.MAX_WBITS|32) if gz else bz2.BZ2Decompressor() # decompressobj
             if len(got) == 0 and len(left) == 0: break                           # decompressobj
+stream_unzip = k1lib.dep("stream_unzip")                                         # decompressobj
+class decompressobjZip: # .zip files                                             # decompressobjZip
+    def __ror__(self, it):                                                       # decompressobjZip
+        for a, b, c in stream_unzip.stream_unzip(it): yield from c; return       # decompressobjZip
 class kunzip(BaseCli):                                                           # kunzip
     def __init__(self, text=False):                                              # kunzip
         """Incrementally decompress a stream of data using gzip or bzip2.
 Example::
 
     # returns an iterator of bytes. cat() command can shorten to cat("someFile.gz", False, True)
-    cat("someFile.gz", text=False, chunks=True) | kunzip()
+    cat("someFile.gz", text=False, chunks=True) | unzip()
     # incrementally fetches remote file, then incrementally unzips it
-    cat("https://example.com/someFile.gz", False, True) | kunzip()
+    cat("https://example.com/someFile.gz", False, True) | unzip()
 
     data = range(100) | apply(lambda x: str(x).encode()) | deref() # list of bytes
-    data | kzip() | kunzip() | deref() # returns original data in list of bytes. May split the bytes at different positions though
+    data | kzip() | unzip() | deref() # returns original data in list of bytes. May split the bytes at different positions though
 
 How does it know which algorithm to pick to decompress? It looks at the
 first few bytes of the file for its magic number. Also, if you're expecting
 a text file after decompression, you can do this to get the lines directly::
 
     # returns iterator of strings
-    cat("https://example.com/someFile.gz", False, True) | kunzip(True)
+    cat("https://example.com/someFile.gz", False, True) | unzip(True)
 
 One more thing. If you're planning to use this to download whole files, you might
 want to tune the chunk size in :data:`~k1lib.settings`.cli.cat.chunkSize as
 it might speed things up considerably to raise it. Or may be you should just
 use wget instead =))
 
 More examples of the different styles to use this cli::
 
-    ["abc"] | kzip() | kunzip(True) | deref() # returns ["abc"]
-    "abc"   | kzip() | kunzip(True)           # returns  "abc"
-    "abc"   | kzip() | kunzip()               # returns b"abc"
+    ["abc"] | kzip() | unzip(True) | deref() # returns ["abc"]
+     "abc"  | kzip() | unzip(True)           # returns  "abc"
+     "abc"  | kzip() | unzip()               # returns b"abc"
+
+See also: :class:`kzip`.
+
+.. admonition:: Reading files directly
+
+    The original purpose of this cli is to incrementally decompress a byte stream.
+    But a lot of time, that byte stream is coming from a file, and typing out
+    ``cat(fn, False, True)`` to generate a byte stream to feed into this cli is
+    tedious, so instead, you can pipe in the file name and this will just unzips
+    it and return the string/byte stream to you::
+
+        "abc.gz"  | unzip() # returns string iterator
+        "abc.bz2" | unzip() # same
+        "abc.zip" | unzip() # returns string iterator from the first subfile only. All subsequent subfiles are ignored
+
+.. admonition:: .zip files
+
+    This can also work with subfiles within .zip files, like this::
 
-See also: :class:`kzip`. There's also an alias to this cli: :class:`unzip`
+        "abc.zip" | unzip()                   # unzips the first subfile
+        "abc.zip" | ls()                      # lists out all subfiles
+        "abc.zip" | ls() | rItem(2) | unzip() # unzips the 3rd subfile
 
 :param text: whether to yield string lines or bytes"""                           # kunzip
         self.text = text                                                         # kunzip
     def __ror__(self, it):                                                       # kunzip
-        def gen(it):                                                             # kunzip
-            it = iter(it); e = next(it); magic = puremagic.from_string(e).split(".")[-1] # kunzip
-            if magic == "gz": o = decompressobj(True)                            # kunzip
-            elif magic == "bz2": o = decompressobj(False)                        # kunzip
+        def gen(it): # generates a stream of bytes                               # kunzip
+            it = iter(it); e = next(it)                                          # kunzip
+            if e[:2] == b"\x1f\x8b": o = decompressobj(True) # .gz               # kunzip
+            elif e[:3] == b"BZh": o = decompressobj(False)    # .bz2             # kunzip
+            elif e[:2] == b"PK": o = decompressobjZip()      # .zip              # kunzip
             else: raise Exception("Can't infer the file type (whether gz or bz2) of this file") # kunzip
             yield from [[e], it] | cli.joinStreams() | o                         # kunzip
         single = False                                                           # kunzip
+        if isinstance(it, str): return cat(it, False, True) | kunzip(self.text) # special case for reading file names directly # kunzip
+        if isinstance(it, ZipWrapper): return it | cat(text=self.text, chunks=True) # special case for .zip subfile # kunzip
         if isinstance(it, bytes): single = True; it = [it]                       # kunzip
         if self.text:                                                            # kunzip
-            def gen2(it):                                                        # kunzip
+            def gen2(it): # generates a stream of strings                        # kunzip
                 last = b"" # last split is probably not the right line boundary, so gotta do this # kunzip
                 for e in gen(it):                                                # kunzip
                     e = last + e; splits = e.split(b"\n")                        # kunzip
                     for line in splits[:-1]: yield line.decode()                 # kunzip
                     last = splits[-1]                                            # kunzip
                 yield last.decode()                                              # kunzip
             res = gen2(it)                                                       # kunzip
```

### Comparing `k1lib-1.4.2/k1lib/cli/kxml.py` & `k1lib-1.4.3/k1lib/cli/kxml.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/mgi.py` & `k1lib-1.4.3/k1lib/cli/mgi.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/modifier.py` & `k1lib-1.4.3/k1lib/cli/modifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __all__ = ["applyS", "aS", "apply", "map_", "applyMp", "parallel", "applyCl",
            "applyTh", "applySerial",
            "sort", "sortF", "consume", "randomize", "stagger", "op",
            "integrate"]
 from typing import Callable, Iterator, Any, Union, List, Tuple
 from k1lib.cli.init import patchDefaultDelim, BaseCli, fastF
 import k1lib.cli as cli, numpy as np, threading, gc; import k1lib
-from collections import deque
+from collections import deque, defaultdict
 from functools import partial, update_wrapper, lru_cache
 from k1lib.cli.typehint import *
 import dill, pickle, k1lib, warnings, atexit, signal, time, os, random, sys
 try: import torch; import torch.multiprocessing as mp; hasTorch = True
 except: import multiprocessing as mp; hasTorch = False
 ray = k1lib.dep("ray")
 settings = k1lib.settings.cli
@@ -80,14 +80,27 @@
         return x*y + a
     # returns 10
     [2, 3] | ~aS(f)
     # returns 11
     [2, 3] | ~aS(f, a=5)"""                                                      # applyS
         f = self.f; a = self.args; kw = self.kwargs; return applyS(lambda x: f(*x, *a, **kw)); # applyS
 aS = applyS                                                                      # applyS
+def _allOpt_gen(a, ir:List[int], n:int): # a is a complex, deref-ed structure    # _allOpt_gen
+    if n == 0: return                                                            # _allOpt_gen
+    ir.append(len(a))                                                            # _allOpt_gen
+    for e in a: _allOpt_gen(e, ir, n-1)                                          # _allOpt_gen
+def _allOpt_genIr(a, n=None) -> "(derefed structure, flattened structure, ir, depth)": # a is a complex, not yet deref-ed structure # _allOpt_genIr
+    a = (a | cli.deref()) if n is None else (a | cli.deref(n)); ir = []; n = n or (a | cli.shape() | cli.shape(0)) # _allOpt_genIr
+    _allOpt_gen(a, ir, n); return a, list(a | cli.joinStreams(n-1)), ir, n       # _allOpt_genIr
+def _allOpt_recover(b:Iterator["data_structure"], ir:Iterator[int], n): # assumes b and ir are iterators # _allOpt_recover
+    ans = []; l = next(ir)                                                       # _allOpt_recover
+    for i in range(l):                                                           # _allOpt_recover
+        if n-1 > 0: ans.append(_allOpt_recover(b, ir, n-1))                      # _allOpt_recover
+        else: ans.append(next(b)); #print("  "*(4-n) + f"appended: {ans}");      # _allOpt_recover
+    return ans                                                                   # _allOpt_recover
 class apply(BaseCli):                                                            # apply
     def __init__(self, f:Callable[[Any], Any], column:Union[int, List[int]]=None, cache:int=0, **kwargs): # apply
         """Applies a function f to every element in the incoming list/iterator.
 Example::
 
     # returns [0, 1, 4, 9, 16]
     range(5) | apply(lambda x: x**2) | deref()
@@ -119,66 +132,92 @@
     # returns [15, 17, 19, 21, 23]
     [range(5), range(10, 15)] | transpose() | ~apply(f, z=5) | deref()
 
 If "apply" is too hard to remember, this cli also has an alias :class:`map_`
 that kinda mimics Python's ``map()``. Also slight reminder that you can't pass
 in extra positional args like in :class:`aS`, just extra keyword arguments.
 
+See also: :class:`aS`, :class:`~k1lib.cli.filt.filt`
+
 :param column: if not None, then applies the function to that column or columns only
 :param cache: if specified, then caches this much number of values
 :param kwargs: extra keyword arguments to pass in the function"""                # apply
         super().__init__(fs=[f]); self.f = f; self.kwargs = kwargs # f is the original operator, _fC is # apply
-        if column:                                                               # apply
+        if column: # quick type checks                                           # apply
             ex = Exception(f"Applying a function on a negative-indexed column ({column}) is not supported") # apply
             if isinstance(column, int):                                          # apply
                 if column < 0: raise ex                                          # apply
             else:                                                                # apply
                 column = list(column)                                            # apply
                 if len([c for c in column if c < 0]): raise ex                   # apply
         self.column = column; self.cache = cache; self._fC = fastF(f)            # apply
         if cache > 0: self._fC = lru_cache(cache)(self._fC)                      # apply
-        self.normal = self.column is None and self.cache == 0 # cached value to say that this apply is just being used as a wrapper, nothing out of the ordinary # apply
-        self.__arrayTypeF = None # None for not formulated yet, 0 for cannot formulate a faster operation # apply
+        self.normal = self.column is None and self.cache == 0 and len(kwargs) == 0 # cached value to say that this apply is just being used as a wrapper, nothing out of the ordinary, like custom columns, cache or custom kwargs # apply
+        if self.normal: # just propagating information upward, to save runtime graph analysis time # apply
+            try: self._propagatedF = f._propagatedF; self._applyDepth = f._applyDepth + 1 # assuming f is another apply() # apply
+            except: self._propagatedF = f; self._applyDepth = 1                  # apply
+        else: self._propagatedF = None; self._applyDepth = 1 # might have to rethink if this depth should be 1 or not # apply
+        # optimization 1: BaseCli._all_array_opt(), aimed at accelerating array types # apply
+        self.__arrayTypeF = None # None for not formulated yet, 0 for cannot formulate a faster operation, else the cached, accelerated function (that might not work) # apply
+        # optimization 2: BaseCli._all_opt(), aimed at accelerating language models # apply
+        self.__allOptF = None # None for not formulated yet, 0 for cannot formulate a faster operation, else the cached, accelerated function (that will guaranteed to work) # apply
     @property                                                                    # apply
-    def _arrayTypeF(self): # returns None or the function                        # apply
+    def _arrayTypeF(self): # optimization 1: returns None or the function (that might not work) # apply
         if self.__arrayTypeF == 0: return None                                   # apply
         if self.__arrayTypeF is None:                                            # apply
             arrs = []; last = self # figure out the depth                        # apply
             while isinstance(last, apply) and last.normal: arrs.append(last); last = last.f # apply
             depth = len(arrs)                                                    # apply
             if depth == 0: self.__arrayTypeF = 0; return None                    # apply
-            if isinstance(last, cli.serial): self.__arrayTypeF = cli.serial(*[(e if isinstance(e, BaseCli) else aS(e)).all(depth) for e in last.clis]); return self.__arrayTypeF # breaks up the serial # apply
-            else: self.__arrayTypeF = aS(lambda it: last._all_array_opt(it, depth)); return self.__arrayTypeF # actually call accelerate function on each individual operation # apply
+            if isinstance(last, cli.serial): # breaks up the serial: (A | B.all(2)).all(3) -> A.all(3) | B.all(5) # apply
+                self.__arrayTypeF = cli.serial(*[(e if isinstance(e, BaseCli) else aS(e)).all(depth) for e in last.clis]); return self.__arrayTypeF # apply
+            else: # it | A.all(3) -> A._all_array_opt(it, 3). This function might return NotImplemented, which means it can't figure out how to utilize the speed up # apply
+                self.__arrayTypeF = aS(lambda it: last._all_array_opt(it, depth)); return self.__arrayTypeF # apply
         return self.__arrayTypeF                                                 # apply
+    @property                                                                    # apply
+    def _allOptF(self): # optimization 2: returns None or the function (that has to work all the time!) # apply
+        if self.__allOptF == 0: return None                                      # apply
+        if self._propagatedF is None or not hasattr(self._propagatedF, "_all_opt"): self.__allOptF = 0; return None # apply
+        f = self._propagatedF._all_opt                                           # apply
+        def inner(it): # has to regenerate the IR on each pass through. Slow (O(30*n) or so), but the function this is supposed to run (LLMs), are even slower, so this is fine for now # apply
+            a, af, ir, n = _allOpt_genIr(it, self._applyDepth) # af = a flat     # apply
+            return _allOpt_recover(iter(f(af)), iter(ir), n)                     # apply
+        return inner                                                             # apply
     def _typehint(self, inp):                                                    # apply
         if self.column is None:                                                  # apply
             if isinstance(inp, tListIterSet):                                    # apply
                 try: return tIter(self.f._typehint(inp.child))                   # apply
                 except: return tIter(tAny())                                     # apply
         return super()._typehint(inp)                                            # apply
     def _copy(self): return apply(self.f, self.column, self.cache, **self.kwargs) # ~apply() case handled automatically # apply
     def __ror__(self, it:Iterator[str]):                                         # apply
         c = self.column; f = self._fC; kwargs = self.kwargs                      # apply
         if c is None:                                                            # apply
-            if self.normal and isinstance(it, settings.arrayTypes):              # apply
-                af = self._arrayTypeF # this whole section is for unwrapping (A.all(2) | B).all(3) into A.all(5) | B.all(3), and each A and B will have their own _all_array_opt() functions that can handle array types insanely fast # apply
-                if af is not None: # there're lots of code here, but it doesn't impact perf cause it's done once for each array object # apply
-                    try:                                                         # apply
-                        ans = af(it)                                             # apply
-                        if ans is not NotImplemented: return ans                 # apply
-                    except Exception as e: self.__arrayTypeF = 0                 # apply
+            if self.normal:                                                      # apply
+                if isinstance(it, settings.arrayTypes): # optimization 1         # apply
+                    af = self._arrayTypeF                                        # apply
+                    if af is not None: # there're lots of code here, but it doesn't impact perf cause it's done once for each array object # apply
+                        try:                                                     # apply
+                            ans = af(it)                                         # apply
+                            if ans is not NotImplemented: return ans             # apply
+                        except Exception as e: pass                              # apply
+                        self.__arrayTypeF = 0 # tried to use the accelerated version, but failed, so won't ever try the accelerated version again # apply
+                elif self._allOptF is not None: return self._allOptF(it) # optimization 2, for LLMs # apply
             return (f(line, **kwargs) for line in it)                            # apply
         elif isinstance(c, int):                                                 # apply
             def gen(it):                                                         # apply
-                for row in it: row = list(row); row[c] = f(row[c]); yield row    # apply
+                for row in it: row = list(row); row[c] = f(row[c], **kwargs); yield row # apply
             return gen(it) # return ([(e if i != c else f(e, **kwargs)) for i, e in enumerate(row)] for row in it) # old version # apply
-        else:                                                                    # apply
-            ops = []                                                             # apply
-            for c_ in c: a = self._copy(); a.column = c_; ops.append(a)          # apply
-            return it | cli.serial(*ops)                                         # apply
+        else: # List[int]                                                        # apply
+            def gen(it):                                                         # apply
+                for row in it:                                                   # apply
+                    row = list(row)                                              # apply
+                    for c_ in c: row[c_] = f(row[c_], **kwargs)                  # apply
+                    yield row                                                    # apply
+            return gen(it)                                                       # apply
     def __invert__(self):                                                        # apply
         """Same mechanism as in :class:`applyS`, it expands the
 arguments out. Just for convenience really. Example::
 
     # returns [10, 12, 14, 16, 18]
     [range(5), range(10, 15)] | transpose() | ~apply(lambda x, y: x+y) | deref()""" # apply
         return apply(lambda x: self.f(*x, **self.kwargs), self.column, self.cache) # apply
@@ -392,21 +431,22 @@
             self.p.terminate();                                                  # applyMp
             if self.p in applyMp._pools: applyMp._pools.remove(self.p)           # applyMp
 # apparently, this doesn't do anything, at least in jupyter environment          # applyMp
 atexit.register(lambda: applyMp.clearPools())                                    # applyMp
 parallel = applyMp                                                               # applyMp
 s = k1lib.Settings(); settings.add("applyCl", s, "modifier.applyCl() settings")  # applyMp
 s.add("sudoTimeout", 300, "seconds before deleting the stored password for sudo commands") # applyMp
-_password = k1lib.Wrapper(None)                                                  # applyMp
+s.add("cpuLimit", None, "if specified (int), will not schedule more jobs if the current number of assigned cpus exceeds this") # applyMp
+_password = k1lib.Wrapper(None); _cpuUsed = k1lib.Wrapper(0)                     # applyMp
 def removePw():                                                                  # removePw
     while True: time.sleep(settings.applyCl.sudoTimeout); _password.value = None # removePw
 t = threading.Thread(target=removePw, daemon=True).start()                       # removePw
 _nodeIdsCache = k1lib.Wrapper([])                                                # removePw
-def specificNode(obj, nodeId:str):                                               # specificNode
-    return obj.options(scheduling_strategy=ray.util.scheduling_strategies.NodeAffinitySchedulingStrategy(node_id=nodeId, soft=False)) # specificNode
+def specificNode(f, nodeId:str): # modify a function so that it will only run on a specific node only # specificNode
+    return f.options(scheduling_strategy=ray.util.scheduling_strategies.NodeAffinitySchedulingStrategy(node_id=nodeId, soft=False)) # specificNode
 def exportSe(se):                                                                # exportSe
     if not isinstance(se, k1lib.Settings): return se                             # exportSe
     return {k:exportSe(v) for k,v in se.__dict__.items() if not k.startswith("_")} # exportSe
 def movePropsSe(obj, se):                                                        # movePropsSe
     d = se.__dict__; keys = [e for e in d.keys() if not e.startswith("_")]       # movePropsSe
     for key in keys:                                                             # movePropsSe
         if key not in obj: continue                                              # movePropsSe
@@ -425,14 +465,40 @@
     # returns [5, 6, 9]
     range(3) | applyCl(lambda x, bias: x**2+bias, bias=5) | deref()
 
     # returns [[1, 2, 3], [1, 2, 3]], demonstrating outside vars work
     someList = [1, 2, 3]
     ["abc", "de"] | applyCl(lambda s: someList) | deref()
 
+    nIds = applyCl.nodeIds()
+    # returns [[<nodeId1>, 0], [<nodeId2>, 1], ...], demonstrating preserve mode
+    [nIds, range(10)] | transpose() | applyCl(lambda x: x**2, pre=True) | deref()
+
+    # executes the function, but stores the result on remote nodes, instead of copying result to this node
+    a = range(5) | applyCl(lambda x: x**2, resolve=False) | deref()
+    # returns [0, 1, 4, 9, 16]
+    a | applyCl(lambda x: x) | deref()
+
+Summary of all mode of operations::
+
+    # Data types:
+    # - 1:   literal value, just a normal Python object
+    # - or1: ray.ObjectRef object - Ray's reference to a remote object living somewhere
+    # - h1:  Handle        object - k1lib's reference to a remote object, obtained if `resolve` is set to False. Use `h.get()` to
+    # - n1:  node id, string
+
+    [1/or1/h1, 2/or2/h2] | applyCl(...)                                              # returns [1, 2, 3]. "1/or1/h1" means that the input can be a list of literals, ObjectRef, or Handle
+    [1/or1/h1, 2/or2/h2] | applyCl(..., resolve=False)                               # returns [h1, h2, h3]
+    [[n1/h1,   1/or1/h3], [n2/h2, 2/or2/h4]] | applyCl(..., pre=True)                # returns [[n1/h1, 1],  [n2/h2, 2]], executed on n1/h1, h3 is copied over
+    [[n1/h1,   1/or1/h3], [n2/h2, 2/or2/h4]] | applyCl(..., pre=True, resolve=False) # returns [[n1/h1, h3], [n2/h2, h4]]
+
+    [n1, n2] | applyCl.aS(lambda: ...)                # returns [[n1, 1],  [n2, 2]]
+    None     | applyCl.aS(lambda: ...)                # returns [[n1, 1],  [n2, 2], ...], executes once on all nodes
+    [n1, n2] | applyCl.aS(lambda: ..., resolve=False) # returns [[n1, h1], [n2, h2]]
+
 Internally, this uses the library Ray (https://www.ray.io) to do the heavy
 lifting. So, :class:`applyCl` can be thought of as a thin wrapper around that
 library, but still has the same consistent interface as :class:`apply` and
 :class:`applyMp`. From all of my tests so far, it seems that :class:`applyCl`
 works quite well and is quite robust, so if you have access to a cluster, use
 it over :class:`applyMp`.
 
@@ -449,14 +515,46 @@
 on 1 or multiple nodes, so check out the docs over there to be aware of them,
 as those translates well to here.
 
 There're more extensive documentation on these notebooks: `27-multi-node <https://mlexps.com/other/27-multi-node/>`_,
 `30-applyCl-benchmarks <https://mlexps.com/other/30-applyCl-benchmarks/>`_, if you want to kinda get the feel of this
 tool more.
 
+.. admonition:: Time sharing the cluster
+
+    Let's say that the cluster is located in a company, and that multiple users want to
+    access it, then you might have to think about it a little more. Say the cluster has
+    60 cores, and someone has launched a long-running job: 2160 tasks, 10 minutes/task,
+    1 core/task, totalling 6 hours. If you want to launch another job that has 20 tasks,
+    requiring 10 cores, 1 second/task, totalling 2 seconds on an idle cluster.
+
+    All modern schedulers (Ray, Slurm, Spark, etc) can't schedule your 20 tasks immediately.
+    It has to wait for some running tasks to finish to schedule your task. This means you
+    have to wait on average for 5-10 minutes before all of your tasks finish. This might be
+    fine if you've used Slurm a lot, but extremely not okay for me and my patience. The whole
+    point of a cluster is to get results immediately, within a few seconds. So here's a
+    workaround::
+
+        # long running task, on notebook 1
+        from k1lib.imports import *
+        settings.cli.applyCl.cpuLimit = 40
+        range(2160) | applyCl(lambda x: time.sleep(10*60)) | ignore() # long running task
+
+        # short running task, on notebook 2
+        from k1lib.imports import *
+        range(20) | applyCl(lambda x: time.sleep(1)) | ignore() # short running task, should finishes almost immediately
+
+    Essentially, there's that setting that you can adjust. Like with Ray's ``num_cpus``,
+    this is merely a suggestion to my library to not schedule jobs past that cpu limit,
+    but you can circumvent it in some strange edge cases that I'm too lazy to implement.
+    Likewise, when you schedule a Ray task, you can specify that it will only take 1 cpu,
+    but you can end up forking it into 5 different processes, which can cause congestion
+    and memory thrashing. If Ray doesn't do it right (possibly impossible to do so anyway)
+    then do I really have to?
+
 .. admonition:: Advanced use case
 
     Not really advanced, but just a bit difficult to understand/follow. Let's say
     that you want to scan through the home directory of all nodes, grab all files,
     read them, and get the number of bytes they have. You can do something like this::
 
         a = None | applyCl.aS(lambda: None | cmd("ls ~") | filt(os.path.isfile) | deref()) | deref()
@@ -572,61 +670,87 @@
     through node ids as the first column to shedule jobs on those specific nodes only
 :param num_cpus: how many cpu does each task take?
 :param memory: how much memory to give to the task in bytes?
 :param resolve: whether to resolve the outputs or not. Set this to False to not move
     memory to the requesting node and cache the big data structure on the remote node
 :param kwargs: extra arguments to be passed to the function. ``args`` not
     included as there're a couple of options you can pass for this cli."""       # applyCl
-        super().__init__(fs=[f]); _fC = fastF(f); self.ogF = f; self.pre = pre   # applyCl
-        isCythonFunc = "cython" in f.__module__                                  # applyCl
-        if isCythonFunc: applyCl.installSo(sys.modules[f.__module__].__file__)   # applyCl
+        super().__init__(fs=[f]); _fC = fastF(f); self.ogF = f; self.pre = pre; self.num_cpus = num_cpus # applyCl
+        try: # f might be a string, so can't do f.__module__                     # applyCl
+            isCythonFunc = "cython" in f.__module__                              # applyCl
+            if isCythonFunc: applyCl.installSo(sys.modules[f.__module__].__file__) # applyCl
+        except: isCythonFunc = False                                             # applyCl
         self.rss = rss = {rss: 1} if isinstance(rss, str) else rss               # applyCl
         cwd = os.getcwd(); se = exportSe(k1lib.settings)                         # applyCl
-        def remoteF(e):                                                          # applyCl
+        def remoteF(s, e): # function that will be executed on remote node. Have to setup environment a little bit before executing # applyCl
+            # e: the real element. s is just e's storage context, in case e is a Handle. Else s is not used and can be None. Why? Because Actors can't be # applyCl
+            # serialized directly with cloudpickle, but it can be passed as function parameters, which Ray will do some special sauce serialization # applyCl
             import k1lib; movePropsSe(se, k1lib.settings) # do this to sync current settings with the remote worker nodes # applyCl
             if k1lib.settings.startup.or_patch.numpy: k1lib.cli.init.patchNumpy() # applyCl
             if k1lib.settings.startup.or_patch.dict: k1lib.cli.init.patchDict()  # applyCl
             if k1lib.settings.startup.or_patch.pandas: k1lib.cli.init.patchPandas() # applyCl
             import os; os.makedirs(cwd, exist_ok = True); os.chdir(cwd)          # applyCl
+            if isinstance(e, Handle): e.setStorage(s); e = e.get()               # applyCl
             return _fC(e, **kwargs)                                              # applyCl
-        self.remoteF = remoteF; self.f = ray.remote(resources=rss, num_cpus=num_cpus, **({"memory": memory} if memory else {}))(remoteF) # applyCl
-        self.prefetch = prefetch or int(1e9)                                     # applyCl
-        self.timeout = timeout; self.bs = bs                                     # applyCl
+        # self.remoteF = remoteF; f = ray.remote(resources=rss, num_cpus=num_cpus, **({"memory": memory} if memory else {}))(remoteF) # applyCl
+        rssKw = {"resources": rss, "num_cpus": num_cpus, **({"memory": memory} if memory else {})}#; rssKw = None # applyCl
+        self.prefetch = prefetch or int(1e8); self.timeout = timeout; self.bs = bs # applyCl
         self._copyCtx = lambda: [f, [prefetch, timeout, bs, rss, pre, num_cpus, memory, resolve], kwargs] # applyCl
-        def preprocessF(f, e): # return future (if pre=False), or [nodeId, future] (if pre=True) # applyCl
-            if pre: nodeId, e = e; return [nodeId, specificNode(f, nodeId).remote(e)] # applyCl
-            else: return f.remote(e)                                             # applyCl
+        nodeId = applyCl.nodeId(); rssF = ray.remote(**rssKw)(remoteF) # f that has constraints injected into it # applyCl
+        def preprocessF(e): # return Handle (if pre=False), or [nodeId, Handle] (if pre=True). f is remoteF, core element can be a Handle, real object, or ObjectRef # applyCl
+            if resolve: # storage location managed by ray, returns or2/h2 or [nId/h1, or2/h2] # applyCl
+                if pre:                                                          # applyCl
+                    a, b = e; s = extractStorage(b)                              # applyCl
+                    if isinstance(a, Handle): h = a.deposit(b); return [a, h.executeAsync(remoteF, s, rssKw)] # applyCl
+                    else: return [a, specificNode(rssF, a).remote(s, b)]         # applyCl
+                else:                                                            # applyCl
+                    if isinstance(e, Handle): return e.executeAsync(remoteF, e.storage, rssKw) # applyCl
+                    else: return rssF.remote(None, e)                            # applyCl
+            else: # storage location explicitly managed by me, returns h2 or [nId/h1, h2] # applyCl
+                storageWarmup()                                                  # applyCl
+                if pre:                                                          # applyCl
+                    a, b = e; s = extractStorage(b)                              # applyCl
+                    if isinstance(a, Handle): # [h1, 2/or2/h2]                   # applyCl
+                        h = a.deposit(b) # first deposits b into a's storage context to get handle. h and a have the same storage context # applyCl
+                        return [a, h.executeAsync(remoteF, h.storage, rssKw)] # then executes it in h's storage context # applyCl
+                    else: # [nId, 2/or2/h2]                                      # applyCl
+                        if isinstance(b, Handle) and b.nodeId == nodeId: return [a, b.executeAsync(remoteF, s, rssKw)] # [nId, h2], if h2 is on nId, then use h2's storage context # applyCl
+                        h = Handle.create(b, a); return [a, h.executeAsync(remoteF, h.storage, rssKw)] # create storage context on `a`, deposits b on it, then execute # applyCl
+                else: # 1/or1/h1                                                 # applyCl
+                    s = extractStorage(e)                                        # applyCl
+                    if isinstance(e, Handle): return e.executeAsync(remoteF, s, rssKw) # has storage context already, execute on it directly # applyCl
+                    else: return Handle.create(e).executeAsync(remoteF, s, rssKw) # create storage context, deposit e on it, then execute # applyCl
         @ray.remote                                                              # applyCl
         def resolveFRemote(o): return 1                                          # applyCl
         def resolveF(e):                                                         # applyCl
             if resolve:                                                          # applyCl
-                if pre: return [e[0], ray.get(e[1], timeout=timeout)]            # applyCl
-                else: return ray.get(e, timeout=timeout)                         # applyCl
-            else: # don't resolve to this node, but still block execution until that object is resolvable # applyCl
-                f = specificNode(resolveFRemote, e[0]) if pre else resolveFRemote # if node ids are available (pre=True), then resolves to that specific node only, else do generic resolve # applyCl
-                ray.get(f.remote(e[1] if pre else e), timeout=timeout); return e # applyCl
-        self.preprocessF = preprocessF; self.resolveF = resolveF                 # applyCl
+                if pre: a, b = e; return [a, b.block().get() if isinstance(b, Handle) else ray.get(b)] # applyCl
+                else: return e.block().get() if isinstance(e, Handle) else ray.get(e) # applyCl
+            else: return [e[0], e[1].block()] if pre else e.block() # don't resolve to this node, but still block execution until that object is resolvable # applyCl
+        self.preprocessF = preprocessF; self.resolveF = resolveF; applyCl.preprocessF = preprocessF; applyCl.resolveF = resolveF # references for lprun so that I can benchmark these 2 functions # applyCl
     @staticmethod                                                                # applyCl
     def installSo(fn:str, force:bool=False):                                     # applyCl
         """Installs dynamic library (.so file) to all nodes.
 
 :param fn: file name of the shared library
 :param force: force reinstall even if the library is already on the remote node""" # applyCl
         basename = os.path.basename(fn)                                          # applyCl
         if not force and basename in _applyCl_soCache: return                    # applyCl
         print("Installing dynamic library to all nodes... ", end=""); _applyCl_soCache.add(basename); contents = cli.cat(fn, False) # applyCl
         None | applyCl.aS(lambda: contents | cli.file(basename)) | cli.ignore(); print("Done") # applyCl
     def __ror__(self, it):                                                       # applyCl
-        f = self.f; timeout = self.timeout; bs = self.bs; ogF = self.ogF; preprocessF = self.preprocessF; resolveF = self.resolveF # applyCl
+        timeout = self.timeout; bs = self.bs; ogF = self.ogF; preprocessF = self.preprocessF; resolveF = self.resolveF # applyCl
         if bs > 1: return it | cli.batched(bs, True) | applyCl(lambda x: x | apply(ogF) | cli.aS(list), self.prefetch, timeout) | cli.joinStreams() # applyCl
         def gen(it):                                                             # applyCl
-            futures = deque(); it = iter(it)                                     # applyCl
-            for i, e in zip(range(self.prefetch), it): futures.append(preprocessF(f, e)) # applyCl
-            for e in it: yield resolveF(futures.popleft()); futures.append(preprocessF(f, e)) # applyCl
-            for e in futures: yield resolveF(e)                                  # applyCl
+            futures = deque(); it = iter(it); n = self.num_cpus; limit = settings.applyCl.cpuLimit or int(1e9) # applyCl
+            for i, e in zip(range(min(self.prefetch, (limit-_cpuUsed.value)//n)), it): # try to anticipate how much resources can be consumed ahead of time and only schedule that much, to prevent deadlocks when multiple applyCl() is called, but their parent process has not consumed the yield statement, so the cpu count doesn't get decremented # applyCl
+                while _cpuUsed.value + n > limit: time.sleep(0.1) # this is a very rudimentary lock. Doesn't have to be accurate though, and Python's GIL ensure atomic-ness # applyCl
+                futures.append(preprocessF(e)); _cpuUsed.value += n              # applyCl
+            for e in it: yield resolveF(futures.popleft()); futures.append(preprocessF(e)) # free and allocate cpu slot immediately, so no while loop necessary # applyCl
+            for e in futures: res = resolveF(e); _cpuUsed.value -= n; yield res  # applyCl
         return gen(it)                                                           # applyCl
     def __invert__(self):                                                        # applyCl
         """Expands the arguments out, just like :class:`apply`.
 Example::
 
     # returns [20, 20, 18, 14, 8, 0, -10, -22, -36, -52]
     [range(10), range(20, 30)] | transpose() | ~applyCl(lambda x, y: y-x**2) | deref()""" # applyCl
@@ -641,14 +765,15 @@
 If you want to get nodes' metadata, then just use ray's builtin function ``ray.nodes()``
 
 :param includeSelf: whether to include node id of the current process or not"""  # applyCl
         res = ray.nodes() | cli.filt(lambda x: x["Alive"]) | apply(lambda x: x["NodeID"]) | aS(list) # applyCl
         if includeSelf: return res                                               # applyCl
         res.remove(applyCl.nodeId()); return res                                 # applyCl
     @staticmethod                                                                # applyCl
+    @lru_cache                                                                   # applyCl
     def nodeId() -> str:                                                         # applyCl
         """Returns current node id"""                                            # applyCl
         return ray.runtime_context.get_runtime_context().get_node_id()           # applyCl
     @staticmethod                                                                # applyCl
     def meta() -> object:                                                        # applyCl
         """Grabs the metadata object for the current node"""                     # applyCl
         return ray.nodes() | cli.filt(lambda x: x["NodeID"] == applyCl.nodeId()) | cli.item() # applyCl
@@ -707,14 +832,34 @@
         global _password; import getpass                                         # applyCl
         if sudo:                                                                 # applyCl
             if _password() is None:                                              # applyCl
                 print("Enter password:"); _password.value = getpass.getpass(prompt="") # applyCl
             return   nodeIds | applyCl.aS(lambda: _password() | cli.cmd(f"sudo -S {s}") | cli.deref(), **kwargs) | cli.deref() # applyCl
         else: return nodeIds | applyCl.aS(lambda: None        | cli.cmd(s)              | cli.deref(), **kwargs) | cli.deref() # applyCl
     @staticmethod                                                                # applyCl
+    def lookup():                                                                # applyCl
+        """Tries to lookup a particular file to see on which node it's at.
+Example::
+
+    # returns [[nodeId, "something.txt"], [nodeId, "abc.jpg"]]
+    ["something.txt", "abc.jpg"] | applyCl.lookup()
+    # returns [nodeId, "something.txt"]
+    "something.txt" | applyCl.lookup()
+
+Files that don't exist won't be included in the result, and files that
+exist on multiple nodes will be returned multiple times. The output format
+is such that I can pipe it into applyCl(..., pre=True) and have it execute
+some function that I want. This is pretty much just a convenience function."""   # applyCl
+        def inner(fns):                                                          # applyCl
+            fns = fns | cli.deref(); single = isinstance(fns, str)               # applyCl
+            if single: fns = [fns]                                               # applyCl
+            ans = None | applyCl.aS(lambda: fns | cli.iden() & (apply(os.path.expanduser) | apply(os.path.exists)) | cli.transpose() | cli.filt("x", 1) | cli.cut(0) | cli.deref()) | cli.ungroup() | cli.deref() # applyCl
+            return ans[0] if single else ans                                     # applyCl
+        return cli.aS(inner)                                                     # applyCl
+    @staticmethod                                                                # applyCl
     def replicateFile(fn:str, nodeIds=None):                                     # applyCl
         """Replicates a specific file in the current node to all the other nodes.
 Example::
 
     applyCl.replicateFile("~/cron.log")
 
 Internally, this will read chunks of 100kB of the specified file and dump it
@@ -1092,15 +1237,91 @@
         if folder is None: return getFolderSize                                  # applyCl
         return folder | getFolderSize                                            # applyCl
     @staticmethod                                                                # applyCl
     def getFilesInFolder(folder:str=None):                                       # applyCl
         from k1lib.cli._applyCl import getFilesInFolder                          # applyCl
         if folder is None: return getFilesInFolder                               # applyCl
         return folder | getFilesInFolder                                         # applyCl
-thEmptySentinel = object()                                                       # applyCl
+@ray.remote(num_cpus=0)                                                          # applyCl
+class Storage: # a wrapper for specific objects, kinda like ObjectRef, but it's an ObjectRef in my control. Should not be serialized to every other place # Storage
+    def __init__(self, v=None):                                                  # Storage
+        self.nodeId = applyCl.nodeId(); self.d = {}; self.refs = defaultdict(lambda: 0) # Storage
+        self.autoInc = k1lib.AutoIncrement(prefix="_d"); self.deposit(v)         # Storage
+        self.idx = f"{self.nodeId}_" + f"{random.random()}"[:10] + f"_{time.time()}" # Storage
+    def getIdx(self): return self.idx                                            # Storage
+    def getMeta(self): return [self.nodeId, self.idx]                            # Storage
+    def lookup(self, idx:str): return self.d[idx]                                # Storage
+    def remove(self, idx:str): del self.d[idx]                                   # Storage
+    def keys(self): return list(self.d.keys())                                   # Storage
+    def incref(self, idx:str): self.refs[idx] += 1#; return self                 # Storage
+    def decref(self, idx:str):                                                   # Storage
+        self.refs[idx] -= 1                                                      # Storage
+        if self.refs[idx] == 0: self.remove(idx)                                 # Storage
+        # return self                                                            # Storage
+    def deposit(self, v:"1/or1/h1", s:"Storage"=None) -> "idx:str": # injecting s into v if v is a Handle # Storage
+        if isinstance(v, Handle): v.setStorage(s); v = v.get()                   # Storage
+        if isinstance(v, ray.ObjectRef): v = ray.get(v)                          # Storage
+        idx = self.autoInc(); self.d[idx] = v; self.incref(idx); return idx      # Storage
+    def execute(self, f, s:"Storage", idx:str) -> "idx:str": return self.deposit(f(s, self.d[idx])) # executing "pure" f with some argument taken from the storage # Storage
+    def __getstate__(self): raise Exception("Can't be serialized!")              # Storage
+_storages = {} # nodeId -> {idx: int, ss: [Storage]}, idx for current index to yield the storage # Storage
+_cpuCounts = {} # nodeId -> int                                                  # Storage
+_nodeIdsGen = None                                                               # Storage
+def getStorage(nodeId:str=None):                                                 # getStorage
+    """Handles creating storage contexts. This is created mainly because it's
+costly to actually instantiate a new actor (1-2 second/actor!), so this will
+spawn new storage contexts till the cpu count of each node is reached. From
+then on, it will keep reusing old storage contexts"""                            # getStorage
+    global _nodeIdsGen; _nodeIdsGen = _nodeIdsGen or applyCl.balancedNodeIds()   # getStorage
+    nodeId = nodeId or next(_nodeIdsGen)                                         # getStorage
+    if nodeId not in _storages or nodeId not in _cpuCounts:                      # getStorage
+        _storages[nodeId] = {"idx": 0, "ss": []}                                 # getStorage
+        _cpuCounts[nodeId] = nodeId | applyCl.aS(lambda: os.cpu_count())         # getStorage
+    if len(_storages[nodeId]["ss"]) < _cpuCounts[nodeId]: # add new storage context # getStorage
+        _storages[nodeId]["ss"].append(specificNode(Storage, nodeId).remote())   # getStorage
+    idx = _storages[nodeId]["idx"]; res = _storages[nodeId]["ss"][idx]           # getStorage
+    _storages[nodeId]["idx"] = (idx+1)%_cpuCounts[nodeId]; return res            # getStorage
+def extractStorage(x): return x.storage if isinstance(x, Handle) else None       # extractStorage
+class Handle: # specific object in storage, pretty much ObjectRef that I'm in control of. Can be serialized to every other place # Handle
+    def __init__(self, storage, idx:str=None, _or=None):                         # Handle
+        self.storage = storage; self.idx = idx; self._or = _or                   # Handle
+        self.nodeId, self.storageId = ray.get(storage.getMeta.remote()); self.weakref = False # whether this Handle should decrement reference count of storage element or not # Handle
+    @staticmethod                                                                # Handle
+    def create(v, nodeId:str=None) -> "Handle": # creates new storage and put value into it # Handle
+        s = getStorage(nodeId); return Handle(s, ray.get(s.deposit.remote(v, extractStorage(v)))) # Handle
+    def deposit(self, v) -> "Handle": # put new value into this handle's Storage # Handle
+        return Handle(self.storage, ray.get(self.storage.deposit.remote(v, extractStorage(v)))) # Handle
+    def execute(self, f, s:"Storage"=None, kwargs=None) -> "Handle": # f is a normal function. Blocks until finished executing # Handle
+        if kwargs:                                                               # Handle
+            @ray.remote(**kwargs)                                                # Handle
+            def inner(sto, s): return sto.execute.remote(f, s, self.idx)         # Handle
+            return Handle(self.storage, ray.get(ray.get(inner.remote(self.storage, s)))) # Handle
+        else: return Handle(self.storage, ray.get(self.storage.execute.remote(f, s, self.idx))) # Handle
+    def block(self) -> "Handle": # block execution and finalize Handle's state   # Handle
+        if self._or: self.idx = ray.get(self._or)                                # Handle
+        return self                                                              # Handle
+    def executeAsync(self, f, s:"Storage"=None, kwargs=None) -> "Handle": # f is a normal function. Returns immediately, finalize it by calling .block() # Handle
+        if kwargs:                                                               # Handle
+            @ray.remote(**kwargs)                                                # Handle
+            def inner(sto, s): return sto.execute.remote(f, s, self.idx)         # Handle
+            return Handle(self.storage, _or=ray.get(inner.remote(self.storage, s))) # Handle
+        else: return Handle(self.storage, _or=self.storage.execute.remote(f, s, self.idx)) # Handle
+    def get(self, s=None): return ray.get(self.storage.lookup.remote(self.idx))  # Handle
+    def setStorage(self, s):                                                     # Handle
+        if s: self.storage = s; self.storage.incref.remote(self.idx); self.weakref = False # Handle
+    def __repr__(self): return f"<Handle idx={self.idx} storage={self.storageId}>" # Handle
+    def __getstate__(self): d = dict(self.__dict__); d["storage"] = None; return d # Handle
+    def __setstate__(self, d): self.__dict__.update(d); self.weakref = True # reconstructed Handles don't decrement reference count of variable, because Actors can't be serialized # Handle
+    def __del__(self):                                                           # Handle
+        # print(f"storage: {self.storage}, nodeId: {self.nodeId}")               # Handle
+        if not self.weakref: self.storage.decref.remote(self.idx)                # Handle
+@lru_cache                                                                       # Handle
+def storageWarmup(): print("Warming up distributed storage..."); None | applyCl.aS(lambda: os.cpu_count()) | ~apply(lambda x,y: [x]*y) | cli.joinSt() | apply(getStorage) | cli.ignore(); print("Finished warming up") # storageWarmup
+def storageSize(): return _storages.values() | cli.op()["ss"].all() | cli.joinSt() | apply(lambda s: ray.get(s.keys.remote())) | cli.joinSt() | cli.shape(0) # storageSize
+thEmptySentinel = object()                                                       # storageSize
 class applyTh(BaseCli):                                                          # applyTh
     def __init__(self, f, prefetch:int=None, timeout:float=5, bs:int=1, **kwargs): # applyTh
         """Kinda like the same as :class:`applyMp`, but executes ``f`` on multiple
 threads, instead of on multiple processes. Advantages:
 
 - Relatively low overhead for thread creation
 - Fast, if ``f`` is io-bound
@@ -1181,66 +1402,92 @@
         if self.unpack:                                                          # applySerial
             while True: yield it; it = f(*it, *self.args, **self.kwargs)         # applySerial
         else:                                                                    # applySerial
             while True: yield it; it = f(it, *self.args, **self.kwargs)          # applySerial
     def __invert__(self):                                                        # applySerial
         ans = applySerial(self.f, *self.args, **self.kwargs)                     # applySerial
         ans.unpack = True; return ans                                            # applySerial
+def argsort(it, key=None, reverse=False):                                        # argsort
+    if isinstance(it, settings.arrayTypes): return np.argsort(it) # this mode ignores key and reverse! # argsort
+    if key: return sorted(range(len(it)), key=lambda i: key(it[i]), reverse=reverse) # argsort
+    else: return sorted(range(len(it)), key=it.__getitem__, reverse=reverse)     # argsort
 class sort(BaseCli):                                                             # sort
-    def __init__(self, column:int=0, numeric=True, reverse=False):               # sort
+    def __init__(self, column:int=0, numeric=True, reverse=False, unsort=False): # sort
         """Sorts all lines based on a specific `column`.
 Example::
 
     # returns [[5, 'a'], [1, 'b']]
     [[1, "b"], [5, "a"]] | ~sort(0) | deref()
     # returns [[2, 3]]
     [[1, "b"], [5, "a"], [2, 3]] | ~sort(1) | deref()
     # errors out, as you can't really compare str with int
     [[1, "b"], [2, 3], [5, "a"]] | sort(1, False) | deref()
     # returns [-1, 2, 3, 5, 8]
     [2, 5, 3, -1, 8] | sort(None) | deref()
 
+.. admonition:: unsort
+
+    This is how it works::
+
+        a = np.array([1, 5, 9, 2, 6, 3, 7, 4, 8])
+        # returns np.array([1, 5, 9, 2, 6, 3, 7, 4, 8])
+        a | sort(None, unsort=True)
+        # returns np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]), normal sort
+        a | sort(None)
+        # returns np.array([-3.5,  0.5,  4.5, -2.5,  1.5, -1.5,  2.5, -0.5,  3.5]), sorts, do transformation, then unsort
+        a | (sort(None, unsort=True) | aS(lambda x: x - x[-1]/2))
+        # returns np.array([12.25,  0.25, 20.25,  6.25,  2.25,  2.25,  6.25,  0.25, 12.25])
+        a | (sort(None, unsort=True) | aS(lambda x: (x - x[-1]/2)**2))
+
+    How this works is that it will sort everything as usual, then it'll execute the captured
+    transformation and then it will unsort everything. This is for scenarios when an operation
+    needs to operate on sorted data, but you still want to keep the original ordering for some
+    reason.
+
 :param column: if None, sort rows based on themselves and not an element
 :param numeric: whether to convert column to float
 :param reverse: False for smaller to bigger, True for bigger to smaller. Use
-    :meth:`__invert__` to quickly reverse the order instead of using this param""" # sort
-        self.column = column; self.reverse = reverse; self.numeric = numeric     # sort
-        self.filterF = (lambda x: float(x)) if numeric else (lambda x: x)        # sort
+    :meth:`__invert__` to quickly reverse the order instead of using this param
+:param unsort: whether to sort and then unsort the input or not"""               # sort
+        super().__init__(capture=True)                                           # sort
+        self.column = column; self.reverse = reverse; self.numeric = numeric; self.unsort = unsort # sort
+        self.filterF = (lambda x: float(x)) if numeric else (lambda x: str(x))   # sort
     def _all_array_opt(self, it, level):                                         # sort
-        c = self.column; reverse = self.reverse; p = [slice(None, None, None)]*level; p1 = (*p, slice(None, None, None)) # sort
+        if self.unsort: return NotImplemented # too complex to think about right now # sort
+        c = self.column; reverse = self.reverse; p = [slice(None, None, None)]*level; p1 = (*p, slice(None, None, None)); ser = self.capturedSerial # sort
         if c is None and len(it.shape)-level != 1: raise Exception(f"Expected sort(None) to take in 1-d array, but the array has shape {it.shape[level:]}") # sort
         if c is not None and len(it.shape)-level != 2: raise Exception(f"Expected sort(None) to take in 2-d array, but the array has shape {it.shape[level:]}") # sort
         bm = np if isinstance(it, np.ndarray) else (torch if (hasTorch and isinstance(it, torch.Tensor)) else None) # sort
         if bm is not None:                                                       # sort
             try:                                                                 # sort
-                if c is None: b = bm.argsort(it);   b = bm.flip(b, (level,)) if reverse else b; return bm.gather(it, level, b) # sort
-                else: b = bm.argsort(it[(*p1, c)]); b = bm.flip(b, (level,)) if reverse else b; return bm.gather(it, level, b[(*p1, None)].expand(it.shape)) # sort
-            except Exception as e:                                               # sort
-                print(e)                                                         # sort
+                if c is None: b = bm.argsort(it);   b = bm.flip(b, (level,)) if reverse else b; return bm.gather(it, level, b) | ser.all(level) # sort
+                else: b = bm.argsort(it[(*p1, c)]); b = bm.flip(b, (level,)) if reverse else b; return bm.gather(it, level, b[(*p1, None)].expand(it.shape)) | ser.all(level) # sort
+            except Exception as e: print(e)                                      # sort
         return NotImplemented                                                    # sort
     def __ror__(self, it:Iterator[str]):                                         # sort
-        c = self.column; reverse = self.reverse; bm = None                       # sort
+        c = self.column; reverse = self.reverse; bm = None; ser = self.capturedSerial # sort
         if isinstance(it, settings.arrayTypes):                                  # sort
             if c is None and len(it.shape) != 1: raise Exception(f"Expected sort(None) to take in a 1-d array, but the array has shape {it.shape}") # sort
             if c is not None and len(it.shape) != 2: raise Exception(f"Expected sort(col) to take in a 2-d array, but the array has shape {it.shape}") # sort
             bm = np if isinstance(it, np.ndarray) else (torch if (hasTorch and isinstance(it, torch.Tensor)) else None) # sort
             if bm:                                                               # sort
-                if c is None: ans = it[bm.argsort(it)]; return bm.flip(ans, (0,)) if reverse else ans # sort
-                else: ans = it[bm.argsort(it[:,c])]; return bm.flip(ans, (0,)) if reverse else ans # sort
-        if c is None:                                                            # sort
-            return it | cli.wrapList() | cli.transpose() | sort(0, self.numeric, self.reverse) | cli.op()[0].all() # sort
+                arg = bm.argsort(it) if c is None else bm.argsort(it[:,c]); arg = bm.flip(arg, (0,)) if reverse else arg # sort
+                return it[arg] | ser | (cli.rows(*argsort(arg)) if self.unsort else cli.iden()) # sort
         f = self.filterF                                                         # sort
-        rows = (it | cli.isNumeric(c) if self.numeric else it) | cli.apply(list) # sort
+        rows = list(it) if c is None else list((it | cli.isNumeric(c) if self.numeric else it) | cli.apply(list)) # sort
         def sortF(row):                                                          # sort
             if len(row) > c: return f(row[c])                                    # sort
             return float("inf")                                                  # sort
-        return sorted(rows, key=sortF, reverse=self.reverse)                     # sort
+        if self.unsort:                                                          # sort
+            arg = argsort(rows, f if c is None else sortF, self.reverse)         # sort
+            return rows | cli.rows(*arg) | ser | cli.rows(*argsort(arg))         # sort
+        return sorted(rows, key=f if c is None else sortF, reverse=self.reverse) | ser # sort
     def __invert__(self):                                                        # sort
         """Creates a clone that has the opposite sort order"""                   # sort
-        return sort(self.column, self.numeric, not self.reverse)                 # sort
+        return sort(self.column, self.numeric, not self.reverse, self.unsort)    # sort
 class sortF(BaseCli):                                                            # sortF
     def __init__(self, f:Callable[[Any], float], column:int=None, reverse=False): # sortF
         """Sorts rows using a function.
 Example::
 
     # returns ['a', 'aa', 'aaa', 'aaaa', 'aaaaa']
     ["a", "aaa", "aaaaa", "aa", "aaaa"] | sortF(lambda r: len(r)) | deref()
```

### Comparing `k1lib-1.4.2/k1lib/cli/mol.py` & `k1lib-1.4.3/k1lib/cli/mol.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/nb.py` & `k1lib-1.4.3/k1lib/cli/nb.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/optimizations.py` & `k1lib-1.4.3/k1lib/cli/optimizations.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/output.py` & `k1lib-1.4.3/k1lib/cli/output.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,32 +180,58 @@
         else: return self.__ror__(it)                                            # file
     @property                                                                    # file
     def name(self):                                                              # file
         """File name of this :class:`file`"""                                    # file
         return self.fileName                                                     # file
 class pretty(BaseCli):                                                           # pretty
     def __init__(self, delim=""):                                                # pretty
-        """Pretty prints a table. Not really used directly.
+        """Pretty-formats a table, or a list of tables.
 Example::
 
     # These 2 statements are pretty much the same
-    [range(10), range(10)] | head(5) | pretty() > stdout()
-    [range(10), range(10)] | display()"""                                        # pretty
-        self.delim = delim                                                       # pretty
+    [range(10), range(10, 20)] | head(5) | pretty() > stdout()
+    [range(10), range(10, 20)] | display()
+
+They both print::
+
+    0    1    2    3    4    5    6    7    8    9
+    10   11   12   13   14   15   16   17   18   19
+
+This can also pretty-formats multiple tables::
+
+    [[range(10), range(10, 20)], [["abc", "defff"], ["1", "1234567"]]] | ~pretty() | joinStreams() | stdout()
+
+This will print::
+
+    0     1         2    3    4    5    6    7    8    9
+    10    11        12   13   14   15   16   17   18   19
+    abc   defff
+    1     1234567
+
+:param delim: delimiter between elements within a row. You might want
+    to set it to "|" to create an artificial border or sth
+"""                                                                              # pretty
+        self.delim = delim; self.inverted = False                                # pretty
     def _typehint(self, inp): return tIter(str)                                  # pretty
     def __ror__(self, it) -> Iterator[str]:                                      # pretty
-        table = []; widths = defaultdict(lambda: 0)                              # pretty
-        for row in it:                                                           # pretty
-            _row = []                                                            # pretty
-            for i, e in enumerate(row):                                          # pretty
-                e = f"{e}"; _row.append(e)                                       # pretty
-                widths[i] = max(len(e), widths[i])                               # pretty
-            table.append(_row)                                                   # pretty
-        for row in table:                                                        # pretty
-            yield self.delim.join(e.rstrip(" ").ljust(w+3) for w, e in zip(widths.values(), row)) # pretty
+        inv = self.inverted; delim = self.delim                                  # pretty
+        if inv: tables = [[list(i1) for i1 in i2] for i2 in it]                  # pretty
+        else: tables = [[list(i1) for i1 in it]]                                 # pretty
+        widths = defaultdict(lambda: 0)                                          # pretty
+        for table in tables:                                                     # pretty
+            for row in table:                                                    # pretty
+                for i, e in enumerate(row):                                      # pretty
+                    e = f"{e}"; row[i] = e                                       # pretty
+                    widths[i] = max(len(e), widths[i])                           # pretty
+        def gen(table):                                                          # pretty
+            for row in table:                                                    # pretty
+                yield delim.join(e.rstrip(" ").ljust(w+3) for w, e in zip(widths.values(), row)) # pretty
+        if inv: return tables | cli.apply(gen)                                   # pretty
+        else: return gen(tables[0])                                              # pretty
+    def __invert__(self): self.inverted = not self.inverted; return self         # pretty
 def display(lines:int=10):                                                       # display
     """Convenience method for displaying a table.
 Pretty much equivalent to ``head() | pretty() | stdout()``.
 
 See also: :class:`pretty`"""                                                     # display
     f = pretty() | stdout()                                                      # display
     if lines is None: return f                                                   # display
@@ -241,14 +267,20 @@
     [[torch.randn(10, 20), "img 1"], [torch.randn(20, 10), "img 2"]] | plotImgs()
 
 If you have multiple rows with different number of images, you can
 plot that with this too, just set ``table=True`` like this::
 
     [[torch.randn(10, 20), torch.randn(20, 10)], [torch.randn(10, 20)]] | plotImgs(table=True)
 
+There's another cli that kinda does what this does: :class:`~k1lib.cli.utils.sketch`. You have
+more control over there, and it does roughly what this cli does, but the typical usage is
+different. This is more for plotting static, throwaway list of 2d arrays, like training set
+images, where as :class:`~k1lib.cli.utils.sketch` is more about plotting results of detailed
+analyses.
+
 :param col: number of columns in the table. If explicitly None, it will turn
     into the number of images fed. Not available if ``table=True``
 :param aspect: aspect ratio of each images, or ratio between width and height
 :param fac: figsize factor. The higher, the more resolution
 :param axis: whether to display the axis or not
 :param table: whether to plot using table mode
 :param im: if True, returns an image"""                                          # plotImgs
```

### Comparing `k1lib-1.4.2/k1lib/cli/sam.py` & `k1lib-1.4.3/k1lib/cli/sam.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/structural.py` & `k1lib-1.4.3/k1lib/cli/structural.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import defaultdict, Counter, deque
 from k1lib.cli.init import patchDefaultDelim, BaseCli, oneToMany, fastF, yieldT
 import k1lib.cli as cli; from k1lib.cli.typehint import *
 import itertools, numpy as np, k1lib, math; import matplotlib.pyplot as plt
 try: import torch; hasTorch = True
 except: torch = k1lib.Object().withAutoDeclare(lambda: type("RandomClass", (object, ), {})); hasTorch = True
 __all__ = ["transpose", "T", "reshape", "insert", "splitW", "splitC",
-           "joinStreams", "flatten", "joinStreamsRandom", "activeSamples",
+           "joinStreams", "joinSt", "joinStreamsRandom", "activeSamples",
            "table", "batched", "window", "groupBy", "ungroup",
            "insertColumn", "insertIdColumn",
            "expandE", "unsqueeze",
            "count", "hist", "permute", "AA_", "peek", "peekF",
            "repeat", "repeatF", "repeatFrom", "oneHot"]
 settings = k1lib.settings.cli
 class transpose(BaseCli):                                                        # transpose
@@ -248,31 +248,32 @@
     # returns array with shape (6, 4)
     np.random.randn(2, 3, 4) | joinStreams()
 
 Sometimes, you may want to impose some dimensional structure after joining all streams
 together, which :class:`reshape` does.
 
 If "joinStreams" is too unintuitive to remember, there's also an alias called
-:class:`flatten`.
+:class:`joinSt`.
 
 :param dims: how many ``joinStreams()`` do you want to do consecutively?"""      # joinStreams
-        if dims < 1: raise AttributeError(f"`dims` ({dims}) can't be less than 1, as it doesn't make any sense!") # joinStreams
-        self.multi = cli.serial(*(joinStreams() for d in range(dims))) if dims > 1 else None # joinStreams
+        if dims < 0: raise AttributeError(f"`dims` ({dims}) can't be less than 0, as it doesn't make any sense!") # joinStreams
+        self.dims = dims; self.multi = cli.serial(*(joinStreams() for d in range(dims))) if dims > 1 else None # joinStreams
+    def _all_array_opt(self, it, level:int): sh = it | cli.shape(); return it.reshape([*sh[:level], sh[level:level+self.dims+1] | cli.toProd(), *sh[level+self.dims+1:]]) # joinStreams
     def __ror__(self, streams:Iterator[Iterator[Any]]) -> Iterator[Any]:         # joinStreams
+        if isinstance(streams, settings.arrayTypes): return self._all_array_opt(streams, 0) # joinStreams
         if self.multi != None:                                                   # joinStreams
             return streams | self.multi                                          # joinStreams
             def gen(): yield from streams | self.multi                           # joinStreams
             return gen()                                                         # joinStreams
-        else:                                                                    # joinStreams
-            if isinstance(streams, settings.arrayTypes): return streams.reshape(-1, *streams.shape[2:]) # joinStreams
-            else:                                                                # joinStreams
-                def gen():                                                       # joinStreams
-                    for stream in streams: yield from stream                     # joinStreams
-                return gen()                                                     # joinStreams
-flatten = joinStreams                                                            # joinStreams
+        elif self.dims == 1:                                                     # joinStreams
+            def gen():                                                           # joinStreams
+                for stream in streams: yield from stream                         # joinStreams
+            return gen()                                                         # joinStreams
+        else: return streams                                                     # joinStreams
+joinSt = joinStreams                                                             # joinStreams
 def probScale(ps, t): # t from 0 -> 1, for typical usage                         # probScale
     l = np.log(ps); avg = l.mean()                                               # probScale
     a = (l-avg)*t+avg; a -= a.max()                                              # probScale
     ans = np.exp(a); return ans/ans.sum()                                        # probScale
 import random                                                                    # probScale
 def rand(n, ps=None):                                                            # rand
     if ps is None:                                                               # rand
@@ -899,67 +900,108 @@
     it() | peekF(headOut()) | deref()"""                                         # peekF
         super().__init__(fs=[f]); self.f = f                                     # peekF
     def __ror__(self, it:Iterator[Any]) -> Iterator[Any]:                        # peekF
         it = iter(it); sentinel = object(); row = next(it, sentinel)             # peekF
         if row == sentinel: return []                                            # peekF
         def gen(): yield row; yield from it                                      # peekF
         self.f(row); return gen()                                                # peekF
+settings.add("repeat", k1lib.Settings().add("infBs", 100, "if dealing with infinite lists, how many elements at a time should be processed?"), "settings related to repeat() and repeatFrom()") # peekF
 class repeat(BaseCli):                                                           # repeat
     def __init__(self, limit:int=None):                                          # repeat
         """Yields a specified amount of the passed in object. If you intend
 to pass in an iterator, then make a list out of it first, as second copy of
 iterator probably won't work as you will have used it the first time. Example::
 
     # returns [[1, 2, 3], [1, 2, 3], [1, 2, 3]]
-    [1, 2, 3] | repeat(3) | toList()
+    [1, 2, 3] | repeat(3) | deref()
+
+If ``limit`` is not specified, then this will repeat indefinitely, which may or may
+not cause a problem downstream. It could be that some downstream operators want to
+get the full view of all elements in the input iterator, but because it's an infinite
+iterator, it will never complete executing and get the full view that it wants::
+
+    [1, 2] |  repeat() | deref()  | headOut() # will hang indefinitely, fill RAM up and crash after a while
+    [1, 2] | (repeat() | deref()) | headOut() # will not hang, and actually print out the first 10 lines, each line is "[1, 2]"
+
+The solution is to just make a group that starts with ``repeat()``. Then ``repeat()``
+can capture all downstream operations, and actually batch up the infinite iterator,
+pass each batch into the downstream operations, and merge the results together. The
+batch size can be controlled by ``settings.cli.repeat.infBs = 200`` if you need it
+for some reason.
+
+See also: :meth:`repeatF`
 
 :param repeat: if None, then repeats indefinitely"""                             # repeat
-        super().__init__(); self.limit = limit                                   # repeat
+        super().__init__(capture=True); self.limit = limit                       # repeat
     def _typehint(self, inp): return tIter(inp)                                  # repeat
+    def _all_array_opt(self, it, level):                                         # repeat
+        if self.limit is None or self.limit == float("inf"): return NotImplemented # repeat
+        sh = it | cli.shape(); s = slice(None, None, None)                       # repeat
+        it = it[(*[s]*level, None)]; newSh = [*sh[:level], self.limit, *sh[level:]] # repeat
+        if isinstance(it, np.ndarray): return np.broadcast_to(it, newSh) | self.capturedSerial.all(level) # repeat
+        elif hasTorch and isinstance(it, torch.Tensor): return it.expand(newSh) | self.capturedSerial.all(level) # repeat
+        return NotImplemented                                                    # repeat
     def __ror__(self, o:Any) -> Iterator[Any]:                                   # repeat
-        limit = self.limit if self.limit != None else k1lib.settings.cli.inf     # repeat
-        for i in itertools.count():                                              # repeat
-            if i >= limit: break                                                 # repeat
-            yield o                                                              # repeat
-def repeatF(f, limit:int=None, **kwargs):                                        # repeatF
+        limit = self.limit if self.limit != None else k1lib.settings.cli.inf; ser = self.capturedSerial # repeat
+        def gen():                                                               # repeat
+            for i in itertools.count():                                          # repeat
+                if i >= limit: break                                             # repeat
+                yield o                                                          # repeat
+        if limit < float("inf"): return self._all_array_opt(o, 0) if isinstance(o, settings.arrayTypes) else (gen() | ser) # repeat
+        return (gen() | ser) if len(self.capturedClis) == 0 else gen() | cli.batched(settings.repeat.infBs) | cli.apply(ser) | cli.joinStreams() # repeat
+class _repeatF(BaseCli):                                                         # _repeatF
+    def __init__(self, limit, kwargs): super().__init__(capture=True); self.limit = limit; self.kwargs = kwargs # _repeatF
+    def __ror__(self, f):                                                        # _repeatF
+        f = fastF(f); limit = self.limit; kwargs = self.kwargs; ser = self.capturedSerial # _repeatF
+        limit = limit if limit != None else k1lib.settings.cli.inf               # _repeatF
+        def gen():                                                               # _repeatF
+            if len(kwargs) == 0:                                                 # _repeatF
+                for i in itertools.count():                                      # _repeatF
+                    if i >= limit: break                                         # _repeatF
+                    yield f()                                                    # _repeatF
+            else:                                                                # _repeatF
+                for i in itertools.count():                                      # _repeatF
+                    if i >= limit: break                                         # _repeatF
+                    yield f(**kwargs)                                            # _repeatF
+        if limit < float("inf"): return gen() | ser                              # _repeatF
+        return (gen() | ser) if len(self.capturedClis) == 0 else gen() | cli.batched(settings.repeat.infBs) | cli.apply(ser) | cli.joinStreams() # _repeatF
+def repeatF(f=None, limit:int=None, **kwargs):                                   # repeatF
     """Yields a specified amount generated by a specified function.
 Example::
 
-    # returns [4, 4, 4]
-    repeatF(lambda: 4, 3) | toList()
-    # returns 10
-    repeatF(lambda: 4) | head() | shape(0)
+    repeatF(lambda: 4, 3) | deref()          # returns [4, 4, 4]
+    (lambda: 4) | repeatF(limit=3) | deref() # returns [4, 4, 4]
+    repeatF(lambda: 4) | head() | shape(0)   # returns 10
 
     f = lambda a: a+2
-    # returns [8, 8, 8]
-    repeatF(f, 3, a=6) | toList()
+    repeatF(f, 3, a=6) | deref()        # returns [8, 8, 8]
+    f | repeatF(limit=3, a=6) | deref() # returns [8, 8, 8]
 
+See :class:`repeat` for a discussion on how to deal with infinite iterators.
+If you want to do something like that, then you have to pipe in f instead of
+specifying f in the params directly.
+
+:param f: function to repeat. If None, then you can pipe the function in
 :param limit: if None, then repeats indefinitely
 :param kwargs: extra keyword arguments that you can pass into the function
 
 See also: :class:`repeatFrom`"""                                                 # repeatF
-    f = fastF(f); limit = limit if limit != None else k1lib.settings.cli.inf     # repeatF
-    if len(kwargs) == 0:                                                         # repeatF
-        for i in itertools.count():                                              # repeatF
-            if i >= limit: break                                                 # repeatF
-            yield f()                                                            # repeatF
-    else:                                                                        # repeatF
-        for i in itertools.count():                                              # repeatF
-            if i >= limit: break                                                 # repeatF
-            yield f(**kwargs)                                                    # repeatF
+    return _repeatF(limit, kwargs) if f is None else f | _repeatF(limit, kwargs) # repeatF
 class repeatFrom(BaseCli):                                                       # repeatFrom
     def __init__(self, limit:int=None):                                          # repeatFrom
         """Yields from a list. If runs out of elements, then do it again for
 ``limit`` times. Example::
 
     # returns [1, 2, 3, 1, 2]
     [1, 2, 3] | repeatFrom() | head(5) | deref()
     # returns [1, 2, 3, 1, 2, 3]
     [1, 2, 3] | repeatFrom(2) | deref()
 
+See :class:`repeat` for a discussion on how to deal with infinite iterators
+
 .. note::
 
     For advanced users who wants to modify the resulting stream mid-way, read this section
 
     Because this reuses elements inside the input iterator, it's necessary
     that the input feels like a list and not an iterator. So in order to make
     this work::
@@ -991,33 +1033,39 @@
 
     This is because internally, :class:`repeatFrom` turns the iterator into a
     list, and continues yielding from that list, and thus won't use the updated
     values. To do it, you have to make the input feels like a list (can get length)::
 
         l = [1, 2, 3]
         def h():
-            for i, e in enumerate(l | repeatFrom(2)):
+            for i, e in enumerate(l | repeatFrom(2)): # ---------------- changed section
                 if i == 3: l.append(5)
                 yield e
         h() | deref() # returns [1, 2, 3, 1, 2, 3, 5]
 
 :param limit: if None, then repeats indefinitely"""                              # repeatFrom
-        super().__init__(); self.limit = limit                                   # repeatFrom
+        super().__init__(capture=True); self.limit = limit                       # repeatFrom
     def _typehint(self, inp):                                                    # repeatFrom
         i = tAny()                                                               # repeatFrom
         if isinstance(inp, tListIterSet): i = inp.child                          # repeatFrom
         if isinstance(inp, tArrayTypes): i = inp                                 # repeatFrom
         return tIter(i)                                                          # repeatFrom
+    def _all_array_opt(self, it, level:int):                                     # repeatFrom
+        if self.limit is None or self.limit == float("inf"): return NotImplemented # repeatFrom
+        return it | (repeat(self.limit) | joinStreams()).all(level) | self.capturedSerial.all(level) # repeatFrom
     def __ror__(self, it:Iterator[Any]) -> Iterator[Any]:                        # repeatFrom
-        try: len(it)                                                             # repeatFrom
-        except: it = list(it)                                                    # repeatFrom
-        limit = self.limit or k1lib.settings.cli.inf                             # repeatFrom
-        for i in itertools.count():                                              # repeatFrom
-            if i >= limit: break                                                 # repeatFrom
-            yield from it                                                        # repeatFrom
+        limit = self.limit or k1lib.settings.cli.inf; ser = self.capturedSerial  # repeatFrom
+        def gen(it):                                                             # repeatFrom
+            try: len(it)                                                         # repeatFrom
+            except: it = list(it)                                                # repeatFrom
+            for i in itertools.count():                                          # repeatFrom
+                if i >= limit: break                                             # repeatFrom
+                yield from it                                                    # repeatFrom
+        if limit < float("inf"): return self._all_array_opt(it, 0) if isinstance(it, settings.arrayTypes) else (gen(it) | ser) # repeatFrom
+        return (gen(it) | ser) if len(self.capturedClis) == 0 else gen(it) | cli.batched(settings.repeat.infBs) | cli.apply(ser) | cli.joinStreams() # repeatFrom
 def oneHotRow(i, n): ans = [0]*n; ans[i] = 1; return ans                         # oneHotRow
 class oneHot(BaseCli):                                                           # oneHot
     _groups = {}                                                                 # oneHot
     def __init__(self, col, n:int=0, group:str=None, sep:bool=False):            # oneHot
         """One-hot encode some column in a table.
 Example::
```

### Comparing `k1lib-1.4.2/k1lib/cli/trace.py` & `k1lib-1.4.3/k1lib/cli/trace.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/typehint.py` & `k1lib-1.4.3/k1lib/cli/typehint.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/cli/utils.py` & `k1lib-1.4.3/k1lib/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     [2, 3] | apply(lambda x: print(x))
     # will prints "2\n3"
     [2, 3] | apply(lambda x: print(x)) | ignore()"""                             # ignore
         super().__init__()                                                       # ignore
     def _all_array_opt(self, it, level): return it                               # ignore
     def _typehint(self, inp): return type(None)                                  # ignore
     def __ror__(self, it:Iterator[Any]):                                         # ignore
+        if isinstance(it, settings.arrayTypes): return                           # ignore
         for _ in it: pass                                                        # ignore
 class rateLimit(BaseCli):                                                        # rateLimit
     def __init__(self, f, delay=0.1):                                            # rateLimit
         """Limits the execution flow rate upon a condition.
 Example::
 
     s = 0; semaphore = 0
@@ -595,14 +596,16 @@
 
 .. image:: ../images/probScale.png
 
 Is it worth the extra confusion? Afterall, it just saves you 2-3 lines of
 code. To me, it is worth it, because you can quickly change styles (add
 a grid, make y axis log)
 
+See also: :class:`~k1lib.cli.output.plotImgs`
+
 :param transforms: transform functions to be run when drawing every plot. ``plt`` (aka ``matplotlib.pyplot``) will be passed in
 :param titles: if specified, use these titles for each plot. Kinda hacky I have to admit
 :param im: if True, returns a PIL image and closes the sketch, else return nothing but still have the sketch open
 :param ncols: if specified, will sketch with this number of columns"""           # sketch
         super().__init__(capture=True); self.titles = titles; self.im = im       # sketch
         self.transforms = [cli.fastF(t) for t in transforms]; self.ncols = ncols # sketch
     def __ror__(self, it):                                                       # sketch
```

### Comparing `k1lib-1.4.2/k1lib/eqn.py` & `k1lib-1.4.3/k1lib/eqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/fmt.py` & `k1lib-1.4.3/k1lib/fmt.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/graphEqn.py` & `k1lib-1.4.3/k1lib/graphEqn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/imports.py` & `k1lib-1.4.3/k1lib/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     import torch; from torch import nn, optim
     import torch.nn.functional as F, torch.utils.data as data
 except: pass
 import matplotlib.pyplot as plt, matplotlib as mpl
 import numpy as np, dill as pickle, multiprocessing as mp, concurrent.futures as futures, threading
 import math, os, time, sys, random, logging, traceback, re, typing, glob, warnings, asyncio
-import dill, json, inspect, xml, base64, io
+import dill, json, inspect, xml, base64, io, html
 import functools; from functools import partial, lru_cache
 import contextlib; from contextlib import contextmanager
 from collections import deque, defaultdict
 from typing import List, Tuple, Callable, Union, Iterator, Set, Dict, Any
 import k1lib; from k1lib import schedule, graphEqn, mo, knn, fmt, selector,\
 viz, Cbs, settings, cli, _k1a, serve, p5, k1ui
 from k1lib.cli import *; k1 = k1lib; k1a = _k1a
```

### Comparing `k1lib-1.4.2/k1lib/k1ui/256.model.state_dict.pth` & `k1lib-1.4.3/k1lib/k1ui/256.model.state_dict.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/k1ui/main.py` & `k1lib-1.4.3/k1lib/k1ui/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/k1ui/mouseKey.pth` & `k1lib-1.4.3/k1lib/k1ui/mouseKey.pth`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/knn.py` & `k1lib-1.4.3/k1lib/knn.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/schedule.py` & `k1lib-1.4.3/k1lib/schedule.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/selector.py` & `k1lib-1.4.3/k1lib/selector.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/serve/main.html` & `k1lib-1.4.3/k1lib/serve/main.html`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/serve/main.py` & `k1lib-1.4.3/k1lib/serve/main.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/serve/suffix.py` & `k1lib-1.4.3/k1lib/serve/suffix.py`

 * *Files identical despite different names*

### Comparing `k1lib-1.4.2/k1lib/viz.py` & `k1lib-1.4.3/k1lib/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 try: import torch; import torch.nn as nn; hasTorch = True
 except:
     torch = k1lib.Object().withAutoDeclare(lambda: type("RandomClass", (object, ), {}))
     nn = k1lib.Object().withAutoDeclare(lambda: type("RandomClass", (object, ), {})); hasTorch = False
 try: import PIL; hasPIL = True
 except: hasPIL = False
 __all__ = ["SliceablePlot", "plotSegments", "Carousel", "Toggle", "ToggleImage",
-           "Scroll", "confusionMatrix", "FAnim", "mask"]
+           "Scroll", "confusionMatrix", "FAnim", "mask", "PDF"]
 class _PlotDecorator:                                                            # _PlotDecorator
     """The idea with decorators is that you can do something like this::
 
     sp = k1lib.viz.SliceablePlot()
     sp.yscale("log") # will format every plot as if ``plt.yscale("log")`` has been called
 
 This class is not expected to be used by end users though."""                    # _PlotDecorator
@@ -453,7 +453,27 @@
 
 :param img: the image, expected to have dimension of (3, h, w)
 :param act: the activation, expected to have dimension of (x, y), and with
     elements from 0 to 1."""                                                     # mask
     *_, h, w = img.shape                                                         # mask
     mask = act[None,] | nn.AdaptiveAvgPool2d([h//16, w//16]) | nn.AdaptiveAvgPool2d([h//8, w//8]) | nn.AdaptiveAvgPool2d([h, w]) # mask
     return mask * img | op().permute(1, 2, 0)                                    # mask
+class PDF(object):                                                               # PDF
+    def __init__(self, pdf:str=None, size=(700,500)):                            # PDF
+        """Displays pdf in the notebook.
+Example::
+
+    viz.PDF("a.pdf")
+    "a.pdf" | viz.PDF()
+
+    viz.PDF("a.pdf", (700, 500))
+    "a.pdf" | viz.PDF(size=(700, 500))
+
+If you're exporting this notebook as html, then you have to make sure
+you place the generated html file in the correct directory so that it
+can reference those pdf files.
+
+:param pdf: relative path to pdf file"""                                         # PDF
+        self.pdf = pdf; self.size = size                                         # PDF
+    def __ror__(self, pdf): self.pdf = pdf; return self                          # PDF
+    def _repr_html_(self): return '<iframe src={0} width={1[0]} height={1[1]}></iframe>'.format(self.pdf, self.size) # PDF
+    def _repr_latex_(self): return r'\includegraphics[width=1.0\textwidth]{{{0}}}'.format(self.pdf) # PDF
```

### Comparing `k1lib-1.4.2/k1lib.egg-info/PKG-INFO` & `k1lib-1.4.3/k1lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1lib
-Version: 1.4.2
+Version: 1.4.3
 Summary: Some nice ML overhaul
 Home-page: https://k1lib.com
 Author: Quang Ho
 Author-email: 157239q@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `k1lib-1.4.2/k1lib.egg-info/SOURCES.txt` & `k1lib-1.4.3/k1lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,19 @@
 k1lib/cli/cif.py
 k1lib/cli/conv.py
 k1lib/cli/filt.py
 k1lib/cli/gb.py
 k1lib/cli/grep.py
 k1lib/cli/init.py
 k1lib/cli/inp.py
-k1lib/cli/kcsv.py
+k1lib/cli/ktree.py
 k1lib/cli/kxml.py
+k1lib/cli/lsext.py
 k1lib/cli/mgi.py
+k1lib/cli/models.py
 k1lib/cli/modifier.py
 k1lib/cli/mol.py
 k1lib/cli/nb.py
 k1lib/cli/optimizations.py
 k1lib/cli/output.py
 k1lib/cli/sam.py
 k1lib/cli/structural.py
```

### Comparing `k1lib-1.4.2/setup.py` & `k1lib-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     packages=["k1lib", "k1lib._hidden",
               "k1lib.cli",
               "k1lib.callbacks", "k1lib.callbacks.profilers",
               "k1lib.callbacks.lossFunctions",
               "k1lib._mo", "k1lib.serve", "k1lib.k1ui"],
     data_files=[('k1lib/serve', ['k1lib/serve/main.html']),
                 ('k1lib/k1ui', ['k1lib/k1ui/mouseKey.pth', 'k1lib/k1ui/256.model.state_dict.pth'])],
-    version="1.4.2",
+    version="1.4.3",
     python_requires='>=3.7',
     install_requires=["numpy>=1.14", "matplotlib>=2.0", "dill", "forbiddenfruit", "wurlitzer", "validators"],
     extras_require={"all": deps},
     description="Some nice ML overhaul",
     url="https://k1lib.com",
     author="Quang Ho",
     author_email="157239q@gmail.com",
```

