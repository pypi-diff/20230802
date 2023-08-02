# Comparing `tmp/astroemperor-0.8.4.tar.gz` & `tmp/astroemperor-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroemperor-0.8.4.tar", last modified: Wed Aug  2 04:38:28 2023, max compression
+gzip compressed data, was "astroemperor-0.8.5.tar", last modified: Wed Aug  2 04:42:34 2023, max compression
```

## Comparing `astroemperor-0.8.4.tar` & `astroemperor-0.8.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.4/LICENSE
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.4/MANIFEST.in
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:38:28.000076 astroemperor-0.8.4/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11180 2023-08-02 04:09:57.000000 astroemperor-0.8.4/README.md
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.4/pyproject.toml
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       38 2023-08-02 04:38:28.000076 astroemperor-0.8.4/setup.cfg
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1103 2023-08-02 04:37:11.000000 astroemperor-0.8.4/setup.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:27.996076 astroemperor-0.8.4/src/
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:27.996076 astroemperor-0.8.4/src/astroemperor/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    63684 2023-08-02 04:37:28.000000 astroemperor-0.8.4/src/astroemperor/__init__.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    14002 2023-08-02 04:37:48.000000 astroemperor-0.8.4/src/astroemperor/block.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    19349 2023-08-02 04:37:55.000000 astroemperor-0.8.4/src/astroemperor/block_repo.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    32195 2023-08-02 04:37:41.000000 astroemperor-0.8.4/src/astroemperor/canvas.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     6506 2023-08-02 04:37:59.000000 astroemperor-0.8.4/src/astroemperor/model_repo.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:27.996076 astroemperor-0.8.4/src/astroemperor/support/
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/src/astroemperor/support/PAE/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.4/src/astroemperor/support/PAE/00.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.4/src/astroemperor/support/PAE/01.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.4/src/astroemperor/support/PAE/02.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.4/src/astroemperor/support/PAE/03.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.4/src/astroemperor/support/__init__.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.4/src/astroemperor/support/endit.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.4/src/astroemperor/support/endit_dyn.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      106 2023-08-02 04:35:44.000000 astroemperor-0.8.4/src/astroemperor/support/init.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      106 2023-08-02 04:35:46.000000 astroemperor-0.8.4/src/astroemperor/support/init_dyn.scr
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/src/astroemperor/support/likelihoods/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.4/src/astroemperor/support/likelihoods/00.like
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/src/astroemperor/support/models/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.4/src/astroemperor/support/models/acc.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.4/src/astroemperor/support/models/empty.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      235 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins00.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      920 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins01 (copy).model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      933 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins01.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1450 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins02.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      747 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins03 (copy).model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      876 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/models/ins03.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.4/src/astroemperor/support/models/kep00.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.4/src/astroemperor/support/models/kep01.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.4/src/astroemperor/support/models/kep02.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.4/src/astroemperor/support/models/kep03.model
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/src/astroemperor/support/pools/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.4/src/astroemperor/support/pools/00.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      160 2023-08-02 03:12:03.000000 astroemperor-0.8.4/src/astroemperor/support/pools/01.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.4/src/astroemperor/support/pools/02.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.4/src/astroemperor/support/pools/03.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.4/src/astroemperor/support/pools/04.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.4/src/astroemperor/support/pools/05.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.4/src/astroemperor/support/pools/06.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.4/src/astroemperor/support/pools/07.pool
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:28.000076 astroemperor-0.8.4/src/astroemperor/support/priors/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.4/src/astroemperor/support/priors/Fixed.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.4/src/astroemperor/support/priors/GaussianMixture.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.4/src/astroemperor/support/priors/Hill.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.4/src/astroemperor/support/priors/Jeffreys.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.4/src/astroemperor/support/priors/Normal.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.4/src/astroemperor/support/priors/Uniform.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2941 2023-08-02 04:38:03.000000 astroemperor-0.8.4/src/astroemperor/unmodel_repo.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    16554 2023-08-02 04:37:38.000000 astroemperor-0.8.4/src/astroemperor/utils.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:38:27.996076 astroemperor-0.8.4/src/astroemperor.egg-info/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:38:27.000000 astroemperor-0.8.4/src/astroemperor.egg-info/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1958 2023-08-02 04:38:27.000000 astroemperor-0.8.4/src/astroemperor.egg-info/SOURCES.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        1 2023-08-02 04:38:27.000000 astroemperor-0.8.4/src/astroemperor.egg-info/dependency_links.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      123 2023-08-02 04:38:27.000000 astroemperor-0.8.4/src/astroemperor.egg-info/requires.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       13 2023-08-02 04:38:27.000000 astroemperor-0.8.4/src/astroemperor.egg-info/top_level.txt
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.5/LICENSE
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.5/MANIFEST.in
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:42:34.838441 astroemperor-0.8.5/PKG-INFO
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11180 2023-08-02 04:09:57.000000 astroemperor-0.8.5/README.md
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.5/pyproject.toml
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       38 2023-08-02 04:42:34.838441 astroemperor-0.8.5/setup.cfg
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1103 2023-08-02 04:41:22.000000 astroemperor-0.8.5/setup.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.834441 astroemperor-0.8.5/src/
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.834441 astroemperor-0.8.5/src/astroemperor/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    63684 2023-08-02 04:41:43.000000 astroemperor-0.8.5/src/astroemperor/__init__.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    14002 2023-08-02 04:37:48.000000 astroemperor-0.8.5/src/astroemperor/block.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    19349 2023-08-02 04:37:55.000000 astroemperor-0.8.5/src/astroemperor/block_repo.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    32195 2023-08-02 04:37:41.000000 astroemperor-0.8.5/src/astroemperor/canvas.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     6506 2023-08-02 04:37:59.000000 astroemperor-0.8.5/src/astroemperor/model_repo.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/PAE/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.5/src/astroemperor/support/PAE/00.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.5/src/astroemperor/support/PAE/01.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.5/src/astroemperor/support/PAE/02.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.5/src/astroemperor/support/PAE/03.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.5/src/astroemperor/support/__init__.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.5/src/astroemperor/support/endit.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.5/src/astroemperor/support/endit_dyn.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      118 2023-08-02 04:41:02.000000 astroemperor-0.8.5/src/astroemperor/support/init.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      118 2023-08-02 04:41:04.000000 astroemperor-0.8.5/src/astroemperor/support/init_dyn.scr
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/likelihoods/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.5/src/astroemperor/support/likelihoods/00.like
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/models/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.5/src/astroemperor/support/models/acc.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.5/src/astroemperor/support/models/empty.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      235 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins00.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      920 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins01 (copy).model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      933 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins01.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1450 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins02.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      747 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins03 (copy).model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      876 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/models/ins03.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.5/src/astroemperor/support/models/kep00.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.5/src/astroemperor/support/models/kep01.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.5/src/astroemperor/support/models/kep02.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.5/src/astroemperor/support/models/kep03.model
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/pools/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.5/src/astroemperor/support/pools/00.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      160 2023-08-02 03:12:03.000000 astroemperor-0.8.5/src/astroemperor/support/pools/01.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.5/src/astroemperor/support/pools/02.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.5/src/astroemperor/support/pools/03.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.5/src/astroemperor/support/pools/04.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.5/src/astroemperor/support/pools/05.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.5/src/astroemperor/support/pools/06.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.5/src/astroemperor/support/pools/07.pool
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor/support/priors/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.5/src/astroemperor/support/priors/Fixed.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.5/src/astroemperor/support/priors/GaussianMixture.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.5/src/astroemperor/support/priors/Hill.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.5/src/astroemperor/support/priors/Jeffreys.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.5/src/astroemperor/support/priors/Normal.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.5/src/astroemperor/support/priors/Uniform.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2941 2023-08-02 04:38:03.000000 astroemperor-0.8.5/src/astroemperor/unmodel_repo.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    16554 2023-08-02 04:37:38.000000 astroemperor-0.8.5/src/astroemperor/utils.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:42:34.838441 astroemperor-0.8.5/src/astroemperor.egg-info/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:42:34.000000 astroemperor-0.8.5/src/astroemperor.egg-info/PKG-INFO
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1958 2023-08-02 04:42:34.000000 astroemperor-0.8.5/src/astroemperor.egg-info/SOURCES.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        1 2023-08-02 04:42:34.000000 astroemperor-0.8.5/src/astroemperor.egg-info/dependency_links.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      123 2023-08-02 04:42:34.000000 astroemperor-0.8.5/src/astroemperor.egg-info/requires.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       13 2023-08-02 04:42:34.000000 astroemperor-0.8.5/src/astroemperor.egg-info/top_level.txt
```

### Comparing `astroemperor-0.8.4/LICENSE` & `astroemperor-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/PKG-INFO` & `astroemperor-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.4
+Version: 0.8.5
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.4/README.md` & `astroemperor-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/setup.py` & `astroemperor-0.8.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="astroemperor",
-    version="0.8.4",
+    version="0.8.5",
     author="ReddTea",
     author_email="redd@tea.com",
     description="PTMCMC sampler for exoplanet search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/pypa/sampleproject",
     classifiers=[
```

### Comparing `astroemperor-0.8.4/src/astroemperor/__init__.py` & `astroemperor-0.8.5/src/astroemperor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.4
+# version 0.8.5
 # date 1 aug 2023
 
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 __name__ = 'astroemperor'
 __all__ = ['support']
 
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
```

### Comparing `astroemperor-0.8.4/src/astroemperor/block.py` & `astroemperor-0.8.5/src/astroemperor/block.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/block_repo.py` & `astroemperor-0.8.5/src/astroemperor/block_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/canvas.py` & `astroemperor-0.8.5/src/astroemperor/canvas.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/model_repo.py` & `astroemperor-0.8.5/src/astroemperor/model_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/endit.scr` & `astroemperor-0.8.5/src/astroemperor/support/endit.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/endit_dyn.scr` & `astroemperor-0.8.5/src/astroemperor/support/endit_dyn.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/ins01 (copy).model` & `astroemperor-0.8.5/src/astroemperor/support/models/ins01 (copy).model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/ins01.model` & `astroemperor-0.8.5/src/astroemperor/support/models/ins01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/ins02.model` & `astroemperor-0.8.5/src/astroemperor/support/models/ins02.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/ins03 (copy).model` & `astroemperor-0.8.5/src/astroemperor/support/models/ins03 (copy).model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/ins03.model` & `astroemperor-0.8.5/src/astroemperor/support/models/ins03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/kep01.model` & `astroemperor-0.8.5/src/astroemperor/support/models/kep01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/models/kep03.model` & `astroemperor-0.8.5/src/astroemperor/support/models/kep03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/support/priors/Hill.prior` & `astroemperor-0.8.5/src/astroemperor/support/priors/Hill.prior`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/unmodel_repo.py` & `astroemperor-0.8.5/src/astroemperor/unmodel_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor/utils.py` & `astroemperor-0.8.5/src/astroemperor/utils.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.4/src/astroemperor.egg-info/PKG-INFO` & `astroemperor-0.8.5/src/astroemperor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.4
+Version: 0.8.5
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.4/src/astroemperor.egg-info/SOURCES.txt` & `astroemperor-0.8.5/src/astroemperor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

