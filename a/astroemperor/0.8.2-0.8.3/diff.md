# Comparing `tmp/astroemperor-0.8.2.tar.gz` & `tmp/astroemperor-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroemperor-0.8.2.tar", last modified: Tue Apr 11 17:35:14 2023, max compression
+gzip compressed data, was "astroemperor-0.8.3.tar", last modified: Wed Aug  2 04:25:09 2023, max compression
```

## Comparing `astroemperor-0.8.2.tar` & `astroemperor-0.8.3.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.053519 astroemperor-0.8.2/
--rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.2/LICENSE
--rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.2/MANIFEST.in
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:35:14.053288 astroemperor-0.8.2/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.2/README.md
--rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.2/pyproject.toml
--rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:35:14.053586 astroemperor-0.8.2/setup.cfg
--rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:34:51.000000 astroemperor-0.8.2/setup.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.030222 astroemperor-0.8.2/src/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.036985 astroemperor-0.8.2/src/astroemperor/
--rw-r--r--   0 reddtea    (501) staff       (20)    63078 2023-04-11 17:34:57.000000 astroemperor-0.8.2/src/astroemperor/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)    13842 2023-04-11 17:25:49.000000 astroemperor-0.8.2/src/astroemperor/block.py
--rw-r--r--   0 reddtea    (501) staff       (20)    20634 2023-04-11 17:25:45.000000 astroemperor-0.8.2/src/astroemperor/block_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    29661 2023-04-11 17:34:26.000000 astroemperor-0.8.2/src/astroemperor/canvas.py
--rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.2/src/astroemperor/model_repo.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.040741 astroemperor-0.8.2/src/astroemperor/support/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.042892 astroemperor-0.8.2/src/astroemperor/support/PAE/
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/00.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/01.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/02.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/03.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.2/src/astroemperor/support/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.2/src/astroemperor/support/endit.scr
--rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.2/src/astroemperor/support/endit_dyn.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:10.000000 astroemperor-0.8.2/src/astroemperor/support/init.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:09.000000 astroemperor-0.8.2/src/astroemperor/support/init_dyn.scr
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.043366 astroemperor-0.8.2/src/astroemperor/support/likelihoods/
--rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.2/src/astroemperor/support/likelihoods/00.like
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.047144 astroemperor-0.8.2/src/astroemperor/support/models/
--rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.2/src/astroemperor/support/models/acc.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.2/src/astroemperor/support/models/empty.model
--rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep03.model
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.050865 astroemperor-0.8.2/src/astroemperor/support/pools/
--rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.2/src/astroemperor/support/pools/00.pool
--rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.2/src/astroemperor/support/pools/01.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.2/src/astroemperor/support/pools/02.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.2/src/astroemperor/support/pools/03.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.2/src/astroemperor/support/pools/04.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.2/src/astroemperor/support/pools/05.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.2/src/astroemperor/support/pools/06.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.2/src/astroemperor/support/pools/07.pool
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.052950 astroemperor-0.8.2/src/astroemperor/support/priors/
--rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Fixed.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.2/src/astroemperor/support/priors/GaussianMixture.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Hill.prior
--rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Jeffreys.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Normal.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Uniform.prior
--rw-r--r--   0 reddtea    (501) staff       (20)     2942 2023-04-11 17:25:59.000000 astroemperor-0.8.2/src/astroemperor/unmodel_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    16308 2023-04-11 17:26:03.000000 astroemperor-0.8.2/src/astroemperor/utils.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.038373 astroemperor-0.8.2/src/astroemperor.egg-info/
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/SOURCES.txt
--rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/dependency_links.txt
--rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/requires.txt
--rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/top_level.txt
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.3/LICENSE
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.3/MANIFEST.in
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:25:09.904914 astroemperor-0.8.3/PKG-INFO
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11180 2023-08-02 04:09:57.000000 astroemperor-0.8.3/README.md
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.3/pyproject.toml
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       38 2023-08-02 04:25:09.904914 astroemperor-0.8.3/setup.cfg
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1103 2023-08-02 04:24:00.000000 astroemperor-0.8.3/setup.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.900914 astroemperor-0.8.3/src/
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.900914 astroemperor-0.8.3/src/astroemperor/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    63684 2023-08-02 04:24:05.000000 astroemperor-0.8.3/src/astroemperor/__init__.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    14002 2023-08-02 04:24:10.000000 astroemperor-0.8.3/src/astroemperor/block.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    19349 2023-08-02 04:24:09.000000 astroemperor-0.8.3/src/astroemperor/block_repo.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    32195 2023-08-02 04:24:12.000000 astroemperor-0.8.3/src/astroemperor/canvas.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     6506 2023-08-02 04:24:14.000000 astroemperor-0.8.3/src/astroemperor/model_repo.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.900914 astroemperor-0.8.3/src/astroemperor/support/
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/src/astroemperor/support/PAE/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.3/src/astroemperor/support/PAE/00.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.3/src/astroemperor/support/PAE/01.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.3/src/astroemperor/support/PAE/02.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.3/src/astroemperor/support/PAE/03.pae
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.3/src/astroemperor/support/__init__.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.3/src/astroemperor/support/endit.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.3/src/astroemperor/support/endit_dyn.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      105 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/init.scr
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      105 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/init_dyn.scr
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/src/astroemperor/support/likelihoods/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.3/src/astroemperor/support/likelihoods/00.like
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/src/astroemperor/support/models/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.3/src/astroemperor/support/models/acc.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.3/src/astroemperor/support/models/empty.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      235 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins00.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      920 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins01 (copy).model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      933 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins01.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1450 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins02.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      747 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins03 (copy).model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      876 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/models/ins03.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.3/src/astroemperor/support/models/kep00.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.3/src/astroemperor/support/models/kep01.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.3/src/astroemperor/support/models/kep02.model
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.3/src/astroemperor/support/models/kep03.model
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/src/astroemperor/support/pools/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.3/src/astroemperor/support/pools/00.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      160 2023-08-02 03:12:03.000000 astroemperor-0.8.3/src/astroemperor/support/pools/01.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.3/src/astroemperor/support/pools/02.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.3/src/astroemperor/support/pools/03.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.3/src/astroemperor/support/pools/04.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.3/src/astroemperor/support/pools/05.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.3/src/astroemperor/support/pools/06.pool
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.3/src/astroemperor/support/pools/07.pool
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.904914 astroemperor-0.8.3/src/astroemperor/support/priors/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.3/src/astroemperor/support/priors/Fixed.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.3/src/astroemperor/support/priors/GaussianMixture.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.3/src/astroemperor/support/priors/Hill.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.3/src/astroemperor/support/priors/Jeffreys.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.3/src/astroemperor/support/priors/Normal.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.3/src/astroemperor/support/priors/Uniform.prior
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2941 2023-08-02 04:24:15.000000 astroemperor-0.8.3/src/astroemperor/unmodel_repo.py
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    16554 2023-08-02 04:24:17.000000 astroemperor-0.8.3/src/astroemperor/utils.py
+drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-08-02 04:25:09.900914 astroemperor-0.8.3/src/astroemperor.egg-info/
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    11556 2023-08-02 04:25:09.000000 astroemperor-0.8.3/src/astroemperor.egg-info/PKG-INFO
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1958 2023-08-02 04:25:09.000000 astroemperor-0.8.3/src/astroemperor.egg-info/SOURCES.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        1 2023-08-02 04:25:09.000000 astroemperor-0.8.3/src/astroemperor.egg-info/dependency_links.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      123 2023-08-02 04:25:09.000000 astroemperor-0.8.3/src/astroemperor.egg-info/requires.txt
+-rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       13 2023-08-02 04:25:09.000000 astroemperor-0.8.3/src/astroemperor.egg-info/top_level.txt
```

### Comparing `astroemperor-0.8.2/LICENSE` & `astroemperor-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/setup.py` & `astroemperor-0.8.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="astroemperor",
-    version="0.8.2",
+    version="0.8.3",
     author="ReddTea",
     author_email="redd@tea.com",
     description="PTMCMC sampler for exoplanet search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/pypa/sampleproject",
     classifiers=[
```

### Comparing `astroemperor-0.8.2/src/astroemperor/__init__.py` & `astroemperor-0.8.3/src/astroemperor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 __name__ = 'astroemperor'
 __all__ = ['support']
+
+
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
 
 # sourcery skip: remove-redundant-if
 if True:
     import numpy as np
     import pandas as pd
-    
+
     import os
     import time
     import pickle
 
     import itertools
     import multiprocessing
     from importlib import reload
@@ -175,14 +177,15 @@
         self.ModelSelection = ModelSelectionObj('BIC')
         self.evidence = 0, 0
 
 
         self.save_all = False
         self.save_plots = False
         self.save_log = True
+        self.save_log_simple = True
         self.save_plots_fmt = 'png'
 
         # plots
         self.instrument_names = None
 
 
         self.plot_gaussian_mixtures = {'plot':True,
@@ -243,15 +246,15 @@
             import reddemcee
             self.engine__ = reddemcee
             self.general_dependencies.extend(['reddemcee', 'emcee', 'logging'])
 
             self.reddemcee_config['burnin'] = 'half'
             self.reddemcee_config['thinby'] = 1
             self.reddemcee_config['logger_level'] = 'CRITICAL'
-            
+
         else:
             raise Exception(self.logger('Failed to set engine properly. Try a string!', center=True, c='red'))
 
 
     def load_data(self, folder_name):
         self.starname = folder_name
         self.data_wrapper = DataWrapper(folder_name, read_loc=self.read_loc)
@@ -264,14 +267,22 @@
         self.my_data = self.data_wrapper.get_data__()
 
         self.my_data_reduc = self.my_data.values[:, 0:3].T
         if len(self.data_wrapper.RV_labels) > 0:
             self.nins__ = len(self.data_wrapper.RV_labels)
             self.switch_RV = True
 
+        self.cornums = self.data_wrapper.nsai
+        if self.switch_SA:
+            if np.sum(self.cornums) > 0:
+                pass
+        else:
+            self.my_data = self.my_data[['BJD', 'RV', 'eRV', 'Flag']]
+            self.cornums = [0 for j in self.cornums]
+
 
     def add_keplerian_block(self, parameterisation=0):
         self.kplanets__ += 1
         kb = mk_KeplerianBlock(self.my_data, parameterisation=parameterisation,
                                   number=self.kplanets__)
 
         prargs = [self.eccentricity_limits, self.eccentricity_prargs]
@@ -295,15 +306,16 @@
         msg = f'                              {msg}'
         self.logger(msg, center=True)
         self.logger('\n')
 
 
     def add_instrumental_blocks(self, moav=0, offset=True):
         for i in range(self.nins__):
-            ib = mk_InstrumentBlock(self.my_data, number=i+1, moav=moav)
+            ib = mk_InstrumentBlock(self.my_data, number=i+1, moav=moav, sa=self.cornums[i])
+            ib.cornum = self.cornums[i]
 
             jitter_args = [self.jitter_limits, self.jitter_prargs]
             SmartLimits(self.my_data, ib, *jitter_args)
 
             ib.ins_no = int(i+1)
             ib.slice = slice(self.kplanets__ * 5 + (i) * ib.ndim_,
                              self.kplanets__ * 5 + (i+1) * ib.ndim_)
@@ -469,15 +481,15 @@
                                          logp_args=[], logp_kwargs={},
                                          ntemps=ntemps, pool=None)
 
             #self.sampler = [None for _ in range(ntemps)]
             with open('sampler_pickle.pkl', 'rb') as sampler_metadata:
                 self.sampler_metadata_dict = pickle.load(sampler_metadata)
             os.system(f'mv sampler_pickle.pkl {self.saveplace}/restore/sampler_pickle.pkl')
-            
+
             for t in range(ntemps):
                 loc_t = '{}emperor_backend_{}.h5'.format(self.saveplace+'/restore/backends/', t)
                 self.sampler[t] = HDFBackend(loc_t)
 
         if self.engine__.__name__ == 'dynesty':
             # TRANSFORM TO PTFORMARGS
             # This is missing additional_parameters ! !
@@ -515,25 +527,25 @@
                 os.system(f'mv sampler_pickle.pkl {self.saveplace}/restore/sampler_pickle.pkl')
             else:
                 # SET SETUP
                 # SET SAMPLER
                 # RUN SAMPLER
                 pass
 
-        
+
     def run_auto(self, setup, k_start=0, k_end=10, parameterisation=1, moav=0, accel=0, progress=True):
         if self.debug_mode:
             #self.set_marker('begin autorun')
             self.debug_timer = time.time()
             print(f'run_auto : INIT run_auto | {time.time()-self.debug_timer}')
 
         self.auto_setup = setup
         if self.engine__.__name__ in ['emcee', 'dynesty', 'pymc3', 'reddemcee']:
 
-            if self.switch_RV and not self.switch_SA:
+            if self.switch_RV:
                 self.add_instrumental_blocks(moav=moav)
             if accel:
                 self.add_acceleration_block(accel=accel)
 
             while k_start <= k_end:
                 if not self.switch_first and k_start > 0 and self.switch_RV:
                     for _ in range(k_start):
@@ -772,18 +784,16 @@
 
                 np.savetxt(f'{self.saveplace}/restore/residuals.dat', np.array([self.my_data['BJD'].values,
                                                       residuals,
                                                       self.my_data['eRV'].values,
                                                       self.my_data['Flag'].values,
                                                       ]))
 
-                rss = np.sum(residuals**2)
-
                 self.dof = ndat - ndim
-                self.chi2 = rss / self.dof
+                self.chi2 = np.sum(residuals**2 / ferr2)
                 self.chi2_red = np.sum(residuals**2 / ferr2) / self.dof
                 self.RMSE = np.sqrt(np.sum(residuals ** 2) / len(residuals))
 
                 self.AIC = 2 * ndim - 2 * self.like_max
                 self.BIC = np.log(ndat) * ndim - 2 * self.like_max
 
                 tm = np.mean(raw_chain[0], axis=0)
@@ -1135,24 +1145,28 @@
                         if p.has_posterior:
                             self.plot_gaussian_mixtures['plot_name'] = f'{b.bnumber_} {p.GM_parameter.name}'
                             plot_GM_Estimator(p.GM_parameter,
                                             options=self.plot_gaussian_mixtures)
                 pbar.close()
 
         # PLOT Keplerian Model and uncertainties
-        if self.kplanets__ > 0:
+        if True:
             if self.plot_keplerian_model['plot']:
                 res_max = flatten(self.get_attr_param('value_max'))
                 self.logger('Plotting Keplerian Models', center=True, c='green')
                 if True:
                     plot_KeplerianModel(self.my_data, self.model,
                                         res_max,
                                         options = self.plot_keplerian_model)
                 else:
                     print('Model plot failed miserably :(\n')
+        if True:
+            if False:
+                plot_periodogram(self.my_data, options=self.plot_keplerian_model)
+
 
         # PLOT stuff with arviz, including corner!!
 
         if self.plot_trace['plot']:
             self.logger('Plotting Trace', center=True, c='green')
 
             plot_traces(self.sampler[self.plot_trace['temp']],
@@ -1160,14 +1174,19 @@
                                 self.model, saveloc=self.saveplace,
                                 trace_modes=self.plot_trace['modes'], fmt='png')
 
         # SAVE LOG
         if self.save_log:
             self.logger.saveto(self.saveplace)
 
+        if self.save_log_simple:
+            simple_log = [flatten(self.model.get_attr_param('name')),
+                          flatten(self.model.get_attr_param('value'))]
+            np.savetxt(f'{self.saveplace}/best_fit.dat', simple_log, fmt='%28s')
+
         # CLEAN A BIT
         os.system(f'mv {self.temp_script} {self.saveplace}/temp/{self.temp_script}')
 
 
     def get_attr_param(self, call, flat=False, asarray=False):
         ret = [b.get_attr(call) for b in self]
         if flat:
@@ -1250,19 +1269,19 @@
         self.script_pool_opt = get_support(f'pools/0{self.multiprocess_method}.pool')
 
         if self.engine__.__name__ == 'reddemcee':
             ntemps, nwalkers, nsteps = self.auto_setup
             #self.my_data.to_csv('{}/temp/temp_data.csv'.format(self.saveplace))
             if self.debug_mode:
                 print(f'write_script() : open(temp_script.py, w) | {time.time()-self.debug_timer}')
-            
+
             with open(self.temp_script, 'w') as f:
                 f.write(open(get_support('init.scr')).read())
                 if self.debug_mode:
-                    #marker = self.set_marker('begin writing script', ret=self.debug_mode)                
+                    #marker = self.set_marker('begin writing script', ret=self.debug_mode)
                     f.write(f'''
 print('temp_script.py   : INIT | {time.time()-self.debug_timer}')
 ''')
                 # DEPENDENCIES
                 for d in self.general_dependencies:
                     f.write(f'''
 import {d}
@@ -1276,14 +1295,15 @@
 '''.format(self.reddemcee_config['logger_level']))
                 # CONSTANTS
                 f.write(f'''
 nan = np.nan
 A_ = {self.model.A_}
 mod_fixed_ = {self.model.mod_fixed}
 gaussian_mixture_objects = dict()
+cornums = {self.cornums}
 
 ''')
 
                 # MODEL
                 f.write(open(self.model.write_model_(loc=self.saveplace)).read())
                 if self.debug_mode:
                     #marker = self.set_marker('end writing model', ret=self.debug_mode)
@@ -1402,15 +1422,15 @@
 
 
 ''')
 
                 # MULTIPROCESSING
                 if self.debug_mode:
                     print(f'write_script() : import multiprocessing pool | {time.time()-self.debug_timer}')
-                f.write(open(self.script_pool_opt).read())
+                f.write(open(self.script_pool_opt).read().format(self.cores__))
 
                 # SETUP CONSTS
                 f.write('''
 
 ntemps, nwalkers, nsteps = {0}, {1}, {2}
 setup = ntemps, nwalkers, nsteps
 ndim = {3}
@@ -1576,19 +1596,18 @@
 
                     f.write(open(get_support('endit_dyn.scr')).read().format(pool_bool, self.cores__, nested_args))
 
         # load just the model into emperor
         if self.debug_mode:
             print('write_script() : imports & reloads | {time.time()-self.debug_timer}')
 
-        try:
-            temp_script = reload(temp_script)    
-        except:
-            import temp_script
-        
+        import temp_script
+        temp_script = reload(temp_script)
+
+
         self.temp_model_func = temp_script.my_model
         self.temp_like_func = temp_script.my_likelihood
         self.temp_prior_func = temp_script.my_prior
 
         if self.debug_mode:
             print('write_script() : END | {time.time()-self.debug_timer}')
 
@@ -1599,15 +1618,15 @@
             print(marker)
         if ret:
             return marker
         return ''
 
 
     def load_run(self):
-        
+
         pass
 
 
     def __getitem__(self, n):
         return self.blocks__[n]
```

### Comparing `astroemperor-0.8.2/src/astroemperor/block.py` & `astroemperor-0.8.3/src/astroemperor/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -342,14 +342,19 @@
                     j += 1
                 else:
                     p.cpointer = None
 
             tdims += b.ndim_
             ntdims += (len(b)-b.ndim_)
 
+        # updates nsai
+        self.cornums = []
+        for b in self:
+            if b.type_ == 'Instrumental':
+                self.cornums.append(b.cornum)
 
     def get_attr_param(self, call):
         return [b.get_attr(call) for b in self]
 
 
     def get_attr_block(self, call):
         return [getattr(b, call) for b in self]
@@ -463,8 +468,8 @@
     def GaussianMixture(x, limits, args):
         #  = my_bgm.bgm_estimator[0]
         if limits[0] <= x <= limits[1]:
             return 0
         else:
             return -np.inf
 
-#
+#
```

### Comparing `astroemperor-0.8.2/src/astroemperor/block_repo.py` & `astroemperor-0.8.3/src/astroemperor/block_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -111,19 +111,25 @@
         pnames = [pnam+' %i' % number for pnam in pnames]
     if moav > 0:
         for j in range(moav):
             if number:
                 pnames.append(f'MACoefficient {number} Order {j + 1}')
                 pnames.append(f'MATimescale {number} Order {j+1}')
 
+                punits.append(r'($\frac{m}{s}$)')
                 punits.append('(Days)')
             else:
                 pnames.extend((f'MACoefficient Order {j + 1}', f'MATimescale Order {j + 1}'))
+                punits.extend((r'($\frac{m}{s}$)', '(Days)'))
         math_display = f'{math_display} + 𝛴ᵢ𝛴ₘ 𝛷ₘ⋅exp((t₍ᵢ₋ₘ₎-tᵢ)/𝜏ₘ)⋅𝜀(t₍ᵢ₋ₘ₎)'
 
+    if sa != 0:
+        for si in range(sa):
+            pnames.append(f'Staract {number} {si}')
+            punits.append('')
     bdim = len(pnames)
 
     pvalues = [-np.inf for _ in range(bdim)]
     ppriors = ['Uniform' for _ in range(bdim)]
     plimits = [[None, None] for _ in range(bdim)]
 
     ptypes = [None for _ in range(bdim)]
@@ -157,19 +163,25 @@
                              my_data.values[:, 0], my_data.values[:, 1]])
         b_script = 'ins01.model'
         if sa:
             insmod = Instrument_Moav_SA_Model
             b_mod = ModelWrapper(insmod, [number, my_data.values[:, 3], moav,
                                  my_data.values[:, 0], my_data.values[:, 4:],
                                  my_data.shape[1]-4])
-            b_script = None
+            b_script = 'ins02.model'
     else:
         insmod = Instrument_Model
         b_mod = ModelWrapper(insmod, [number, my_data.values[:, 3]])
         b_script = 'ins00.model'
+        if sa:
+            ###
+            insmod = Instrument_Model_SA
+            b_mod = ModelWrapper(insmod, [number, my_data.values[:, 3]])
+            b_script = 'ins03.model'
+            pass
 
     b_name = f'InstrumentalBlock {number}'
 
     return Parameter_Block(my_params, block_model=b_mod,
                            block_name=b_name, block_type='Instrumental',
                            model_script=b_script,
                            is_iterative=False,
@@ -362,15 +374,15 @@
             '''
             b.add_additional_priors([['Eccentricity', norm, ecc_limits, ecc_prargs],
                                    ['Longitude', uni, [0, 2*np.pi], []],
                                    ])
             '''
         if d['starmass']:
             sma_minmass_add_additional(b, uni)
-        
+
             if d['dynamics']:
                 if not d['dynamics_already_included'] and d['kplan'] > 1:
                     d0 = {'name': 'Hill',
                         'display_name': 'Dynamical Criteria',
                         'prior': 'Hill',
                         'limits':[None, None],
                         'prargs':[d['kplan'], d['starmass']],
@@ -399,67 +411,30 @@
 
         lims = [[-jit_limiter, jit_limiter], [1e-5, jit_limiter]]
         priors = [uni, norm]
         prargs = [None, jit_prargs]
 
         if b.moav > 0:
             for _ in range(b.moav):
-                lims.extend(([0.5, 1], [15, 25]))
-                priors.extend((uni, uni))
-                prargs.extend((None, None))
-        '''
-            elif b.type_ == 'AdditionalPriors':
-                my_params = []
+                lims.append([0.0, 0.3])
+                lims.append([5, 25])
+
+                priors.append(uni)
+                priors.append(uni)
+
+                prargs.append(None)
+                prargs.append(None)
+
+        if b.cornum > 0:
+            for _ in range(b.cornum):
+                lims.append([-1., 1.])
+                priors.append(uni)
+                prargs.append(None)
+
 
-                pnames = []
-                punits = []
-                pvalues = []
-                ppriors = []
-                plimits = []
-
-                ptypes = []
-                prargs = []
-                ptformargs = []
-                pfixed = []
-                psigma = []
-                if False:
-                    # All CVs go here!!!
-                    sig_limiter = my_data['RV'].std(ddof=0)
-                    per_limiter = my_data['BJD'].max() - my_data['BJD'].min()
-                    amp_limiter = sig_limiter * np.sqrt(3)
-                    angle_limits = [0, 2*np.pi]
-
-                    ecc_limits, ecc_prargs = d['prargs']
-                if True:
-                    #Hill goes here
-                    if d['dynamics']:
-                        if d['kplan'] > 1:
-                            prarg = [d['kplan'], d['starmass']]
-
-                            pnames.append('Hill')
-                            ppriors.append('Hill')
-                            pvalues.append(None)
-                            plimits.append([None, None])
-                            punits.append(None)
-                            prargs.append(prarg)
-                            ptypes.append(None)
-                            ptformargs.append(None)
-                            pfixed.append(None)
-                            psigma.append(None)
-
-                bdim = len(pnames)
-                for i in range(bdim):
-                    d0 = {'name':pnames[i], 'prior':ppriors[i], 'value':pvalues[i],
-                              'limits':plimits[i], 'unit':punits[i], 'prargs':prargs[i],
-                              'type':ptypes[i], 'ptformargs':ptformargs[i], 'fixed':pfixed[i],
-                              'sigma':psigma[i]}
-                    my_params.append(Parameter(d0))
-                b.list_ = np.array(my_params)
-                return
-            '''
     elif b.type_ != 'Acceleration':
         print(f'type_ {b.type_} not recognised. \nSmartLimits failed')
 
     b.set_attr('limits', lims, silent=True)
     b.set_attr('prior', priors, silent=True)
     b.set_attr('prargs', prargs, silent=True)
 
@@ -523,8 +498,8 @@
 # ~𝓤()
 # ~𝓝()
 # ~𝓖()
 # ~ 𝓙()
 
 # ✅ ✔ ✓
 # ◯
-# ❎ ❌ ✘ ✗ ☒
+# ❎ ❌ ✘ ✗ ☒
```

### Comparing `astroemperor-0.8.2/src/astroemperor/canvas.py` & `astroemperor-0.8.3/src/astroemperor/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # type: ignore
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 # sourcery skip
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
@@ -26,15 +26,15 @@
 from tqdm import tqdm
 
 from reddcolors import Palette
 
 from .model_repo import *
 from .unmodel_repo import *
 from .block import ReddModel
-from .utils import fold_dataframe, nullify_output, flatten, get_support
+from .utils import fold_dataframe, nullify_output, flatten, get_support, getExtremePoints
 
 
 rc = Palette()
 
 
 def plot_GM_Estimator(estimator, options=None):
     # sourcery skip: use-fstring-for-formatting
@@ -312,15 +312,15 @@
         switch_uncertain = options['uncertain']
         switch_errors = options['errors']
         logger_level = options['logger_level']
         gC = options['gC']
 
         axhline_kwargs = {'color':'gray', 'linewidth':2}
         errorbar_kwargs = {'marker':'o', 'ls':''}
-       
+
         posterior_method = 'GM'
         #c = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
         c = ['C0', 'C1', 'C2', 'C4', 'C6', 'C7', 'C8', 'C9']
         colors = np.array([c,c,c,c,c]).flatten()
 
         temp_file_names = []
         temp_mod_names = []
@@ -346,32 +346,34 @@
         with open(temp_script, 'w') as f:
             f.write(open(get_support('init.scr')).read())
             # DEPENDENCIES
             f.write('''
 import kepler
 ''')
             # CONSTANTS
-            f.write('''
+            f.write(f'''
 nan = np.nan
 A_ = []
 mod_fixed_ = []
 gaussian_mixture_objects = dict()
+
+cornums = {my_model.cornums}
 ''')
 
             f.write(open(x.write_model_(loc=saveloc, tail=tail_x)).read())
 
     if True:
         ## COL
         D = deepcopy(my_data)
         ajuste = res
         OGM = my_model
 
         # Block selection
-        DB_A = [b for b in OGM if b.display_on_data_==True]
-        NDB_A = [b for b in OGM if b.display_on_data_==False]
+        DB_A = [b for b in OGM if b.display_on_data_==True]  # Keplerians
+        NDB_A = [b for b in OGM if b.display_on_data_==False]  # Instrumental
 
         pbar_tot = 1 + len(DB_A)
 
         pbar = tqdm(total=pbar_tot)
         # data for continuous
         x_c = np.linspace(D['BJD'].min(), D['BJD'].max(), 5000)
         DC = pd.DataFrame({'BJD':x_c, 'RV':np.zeros_like(x_c), 'eRV':np.zeros_like(x_c)})
@@ -388,24 +390,26 @@
         ndm, ndferr = NDM_A_mod(ajuste)
 
         # data gets cleaned from no display
         D['RV'] -= ndm.values
         D['eRV'] = np.sqrt(D['eRV'].values**2 + ndferr.values)
 
         # get the residuals
+        D['residuals'] = D['RV'].values
+        if DB_A:
+            create_mod(D, DB_A, '_DM_A', 1)
 
-        create_mod(D, DB_A, '_DM_A', 1)
+            import temp_mod_01
+            DM_A_mod = reload(temp_mod_01).my_model
 
-        import temp_mod_01
-        DM_A_mod = reload(temp_mod_01).my_model
 
-        D['residuals'] = D['RV'].values - DM_A_mod(ajuste)[0]
+            D['residuals'] -= DM_A_mod(ajuste)[0]
 
-        # Here we are done. We have 3 different datasets
-        # display, og-no_display, continuous
+            # Here we are done. We have 3 different datasets
+            # display, og-no_display, continuous
 
     # FULL MODEL
     # this requires a subgrid, for plotting the residuals
 
     if True:
         if True:
             fig = pl.figure(figsize=(10, 8))
@@ -440,16 +444,17 @@
                                 c=colors[b_ins.number_-1],
                                 **errorbar_kwargs)
                     else:
                         ax.plot(D[mask]['BJD'], D[mask]['RV'],
                                 colors[b_ins.number_-1]+'o', label=b_ins.instrument_label)
 
                         axr.plot(D[mask]['BJD'], D[mask]['residuals'], colors[b_ins.number_-1]+'o')
+
         # We set unmodels for uncertainties
-        if True:
+        if len(DB_A):
             for b in DB_A:
                 if b.parameterisation == 0:
                     #kepmod = Keplerian_Model
                     unkepmod = unKeplerian_Model
                     un_model_name = "unKeplerian_Model"
                     chaos_names = ['Period', 'Amplitude', 'Phase', 'Eccentricity', 'Longitude_Periastron']
                 if b.parameterisation == 1:
@@ -465,25 +470,26 @@
                 if b.parameterisation == 3:
                     #kepmod = Keplerian_Model_3
                     unkepmod = unKeplerian_Model_3
                     un_model_name = "unKeplerian_Model_3"
                     chaos_names = ['Period', 'Amplitude', 'Time_Periastron', 'Ecc_sin', 'Ecc_cos']
 
         # Now we plot our line
-        DB_AC = deepcopy(DB_A)
+        if len(DB_A):
+            DB_AC = deepcopy(DB_A)
 
-        create_mod(DC, DB_AC, '_DM_AC', 2)
+            create_mod(DC, DB_AC, '_DM_AC', 2)
 
-        import temp_mod_02
-        DM_AC_mod = reload(temp_mod_02).my_model
+            import temp_mod_02
+            DM_AC_mod = reload(temp_mod_02).my_model
 
 
-        DC['RV'] = DM_AC_mod(ajuste)[0]
+            DC['RV'] = DM_AC_mod(ajuste)[0]
 
-        ax.plot(DC['BJD'], DC['RV'], color=rc.fg, ls='--')
+            ax.plot(DC['BJD'], DC['RV'], color=rc.fg, ls='--')
 
         if True and switch_histogram:
             nbins = 5
             while nbins < len(D):
                 counts, bins = np.histogram(D['RV'], bins=nbins)
                 if (counts==0).any():
                     break
@@ -579,15 +585,15 @@
 
             D_PF = fold_dataframe(D_PF, per=per)
 
             ## plot data per instrument
             for b_ins in NDB_A:
                 if b_ins.type_ == 'Instrumental':
                     mask = D_PF['Flag']==b_ins.number_
-                    
+
                     if switch_errors:
                         ax.errorbar(D_PF[mask]['BJD'], D_PF[mask]['RV_D'], yerr=D_PF[mask]['eRV'],
                                     c=colors[b_ins.number_-1], label=b_ins.instrument_label,
                                     **errorbar_kwargs)
 
                         axr.errorbar(D_PF[mask]['BJD'], D_PF[mask]['residuals'], yerr=D_PF[mask]['eRV'],
                                 c=colors[b_ins.number_-1],
@@ -768,15 +774,91 @@
                 os.system('mv {0} {1}{2}'.format(file, temp_file_folder, file.split('/')[-1]))
             except Warning:
                 print('Couldnt auto-delete temp files')
 
     return chaos_thetas
 
 
+def plot_periodogram(my_data, options, tail_name=''):
+    from scipy.signal import lombscargle
+    if options is None:
+        options = {}
 
+    saveplace = options['saveloc'] + '/plots/'
+    plot_fmt = options['format']
+    x = my_data['BJD']
+    y = my_data['RV']
+    yerr = my_data['eRV']
+
+    # other params
+    Nfreq = 10000
+    periods = np.linspace(x.min(), x.max(), Nfreq)
+    ang_freqs = 2 * np.pi / periods
+
+    maxpoints = 5
+    ide = np.arange(maxpoints)+1
+
+    TITLE = 'Periodogram'
+    xaxis_label = 'Period (days)'
+    yaxis_label = 'Lomb-Scargle Power'
+    title_fontsize = 'large'
+    label_fontsize = 'medium'
+    line_style = '-'
+    line_color = rc.fg
+    hsize, vsize = 10, 8
+    dpi = 80
+    xlog = True
+    ylog = False
+
+    scatter_marker_style = 'o'
+    scatter_size = 40
+    scatter_color = '#FF0000'
+    scatter_alpha = 1
+
+    method = 0
+    t = np.ascontiguousarray(x.values)
+    mag = np.ascontiguousarray(y.values)
+    dmag = np.ascontiguousarray(yerr.values)
+
+    if method == 0:
+        power = lombscargle(t, mag - np.mean(mag), ang_freqs)
+        N = len(t)
+        power *= 2 / (N * np.std(mag) ** 2)
+
+    # Plot
+    fig, ax = pl.subplots(figsize=(hsize, vsize), dpi=dpi)
+    pl.title(TITLE, fontsize=title_fontsize)
+
+    idx = getExtremePoints(power, typeOfExtreme='max', maxPoints=maxpoints)
+
+    pl.plot(periods, power, ls=line_style, c=line_color)
+    # fap line
+
+    #ax.annotate('0.1% significance level', (3, 0.13))
+    #pl.plot(periods, np.ones_like(periods)*0.12, ls='--', c=line_color, alpha=0.5)
+
+    pl.scatter(periods[idx], power[idx],
+                marker=scatter_marker_style,
+                s=scatter_size, c=scatter_color,
+                alpha=scatter_alpha)
+
+    for i in idx:
+        ax.annotate(f' Max = {np.round(periods[i], 2)}', (periods[i]+10, power[i]))
+
+        ax.set_title(TITLE, fontsize=title_fontsize)
+        ax.set_xlabel(xaxis_label, fontsize=label_fontsize)
+        ax.set_ylabel(yaxis_label, fontsize=label_fontsize)
+
+        if xlog:
+            ax.set_xscale('log')
+        if ylog:
+            ax.set_yscale('log')
+
+    tabable = np.array([periods[idx][::-1], power[idx][::-1]])
+    taball = np.vstack([ide, tabable])
+    headers = ['Rank', 'Period', 'Power']
 
+    ax.table(cellText=taball.T, colLabels=headers, loc='top right')
 
-
-
-
+    pl.savefig(f'{saveplace}periodogram{tail_name}.{plot_fmt}')
 
 # blue verde rojo purp naran cyan brown blue green
```

### Comparing `astroemperor-0.8.2/src/astroemperor/model_repo.py` & `astroemperor-0.8.3/src/astroemperor/model_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -198,14 +198,39 @@
                     residuals[my_mask][i] -= MA
 
     new_err = my_mask * theta[1] ** 2
 
     return mod, new_err
 
 
+def Instrument_Model_SA(theta, *args, **kwargs):
+    # time and residuals should exclusively be the ones for this instrument
+    ins_no = args[0]
+    flags = args[1]
+    maorder = args[2]
+    time = args[3]
+
+    staracts = args[4]
+    cornum = args[5]
+
+    #print('in model 2', offset*[flags == ins_no])
+
+    my_mask = (flags == ins_no)
+    mod = theta[0] * my_mask  # OFFSET
+    #residuals = rv - mod
+
+    if cornum:
+        for j in range(cornum):
+            mod[my_mask] += theta[2 * (maorder + 1) + j] * staracts[j]
+
+    new_err = my_mask * theta[1] ** 2
+
+    return mod, new_err
+
+
 def Acceleration_Model(theta, *args, **kwargs):
     time = args[0]
     mod = np.polyval(np.concatenate([theta, [0]]), time-time[0])
 
     return mod, 0
```

### Comparing `astroemperor-0.8.2/src/astroemperor/support/endit.scr` & `astroemperor-0.8.3/src/astroemperor/support/endit.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/src/astroemperor/support/endit_dyn.scr` & `astroemperor-0.8.3/src/astroemperor/support/endit_dyn.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/src/astroemperor/support/models/ins01.model` & `astroemperor-0.8.3/src/astroemperor/support/models/ins01.model`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+    # Instrumental Part, ins01.model
+
     residuals = my_data['RV'] - model0
 
     my_mask = (my_data['Flag'] == {0})
 
     mod = theta[{1}][0] * my_mask  # OFFSET
 
+    # Moav Part
     if {2} > 0:
         theta_ma = theta[{1}][2:]
-        t_ = my_data['BJD'][my_mask]
+        t_ = my_data['BJD'][my_mask].values
+        res_ = residuals[my_mask].values
+        mod_ = mod[my_mask].values
         for i in range(len(t_)):
             for c in range({2}):
                 if i > c:
                     dt = abs(t_[i] - t_[i - 1 - c])
                     macoef = theta_ma[2 * c]
                     matime = theta_ma[2 * c + 1]
-                    MA = macoef * np.exp(-dt / matime) * residuals[my_mask][i - 1 - c]
-                    mod[my_mask][i] += MA
-                    residuals[my_mask][i] -= MA
-
+                    MA = macoef * np.exp(-dt / matime) * res_[i - 1 - c]
+                    mod_[i] += MA
+                    res_[i] -= MA
+        mod[my_mask] = mod_
+        residuals[my_mask] = res_
 
     new_err = my_mask * theta[{1}][1] ** 2
 
     model0 += mod
     err20 += new_err
+
+    # End Instrumental Part
```

### Comparing `astroemperor-0.8.2/src/astroemperor/support/models/kep01.model` & `astroemperor-0.8.3/src/astroemperor/support/models/kep01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/src/astroemperor/support/models/kep03.model` & `astroemperor-0.8.3/src/astroemperor/support/models/kep03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/src/astroemperor/support/priors/Hill.prior` & `astroemperor-0.8.3/src/astroemperor/support/priors/Hill.prior`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.2/src/astroemperor/unmodel_repo.py` & `astroemperor-0.8.3/src/astroemperor/unmodel_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
```

### Comparing `astroemperor-0.8.2/src/astroemperor/utils.py` & `astroemperor-0.8.3/src/astroemperor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8.1
-# date 11 apr 2023
+# version 0.8.3
+# date 1 aug 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -45,20 +45,20 @@
     @dr.setter
     def dr(self, val):
         self._dr = val
 
     @property
     def loc(self):
         return self._loc
-    
+
     @loc.setter
     def loc(self, val: str):
         self._loc = val
 
-    
+
     def aim(self, target):
         if type(target) == str:
             self._target_folder = target
             self._dr = f'{self._loc}datalogs/{self._target_folder}/'
             self._target_list = os.listdir(self._dr)
 
         if type(target) == tuple:
@@ -74,15 +74,15 @@
             self._dr = f'{self._loc}datalogs/'
             self._nuclear = True
             self._target_list = os.listdir(self._dr)
 
         for x in self._target_list:
             if x[0] == '.':
                 self._target_list.remove(x)
-                
+
 
     def nuke(self):
         if not self.IamSure:
             print('You are about to delete the following directories:\n')
             for tg in self._target_list:
                 print(f'    - {self._dr}{tg}\n')
             print('if you are really sure, set nuker.IamSure = True')
@@ -234,15 +234,15 @@
     if (len(data) - 1) in idx:
         idx = np.delete(idx, len(data)-1)
 
     idx = idx[np.argsort(data[idx])]
     # If we have maxpoints we want to make sure the timeseries has a cutpoint
     # in each segment, not all on a small interval
     if maxPoints is not None:
-        idx = idx[:maxPoints]
+        idx = idx[-maxPoints:]
         if len(idx) < maxPoints:
             return (np.arange(maxPoints) + 1) * (len(data)//(maxPoints + 1))
 
     return idx
 
 
 def plot_extreme(data, n=10):
@@ -520,24 +520,30 @@
         self.RV_labels.append(filename)
 
         names = ['BJD', 'RV', 'eRV']
 
         # identify and name SAI
         nsa = ncol - 3
         if nsa > 0:
-            names.extend(f'Staract {j}' for j in range(nsa))
+            names.extend(f'Staract {len(self.ndata)} {j}' for j in range(nsa))
         self.nsai.append(nsa)
 
         df = pd.DataFrame(data, columns=names)
 
         # substract RV
         if abs(df.mean()['RV']) > 1e-6:
             df['RV'] -= df.mean()['RV']
+
+        for nam in names:
+            if nam[:3] == 'Sta':
+                if abs(df.mean()[nam]) > 1e-6:
+                    df[nam] -= df.mean()[nam]
+                    df[nam] = df[nam] / (df.max()[nam] - df.min()[nam])
         # create another column containing flags for the instrument
-        df['Flag'] = np.ones(ndat, int) * len(self.ndata)
+        df.insert(loc=3, column='Flag', value=np.ones(ndat, int) * len(self.ndata))
         self.data.append(df)
 
         return 'Reading data from {0}'.format(filename)
 
 
     def add_all__(self):
         my_files = list(np.sort(os.listdir(self.RV_PATH)))
@@ -574,8 +580,8 @@
         self.fargs = fargs
         self.fkwargs = fkwargs
 
     def __call__(self, x):
         return self.func(x, *self.fargs, **self.fkwargs)
 
 
-#
+#
```

### Comparing `astroemperor-0.8.2/src/astroemperor.egg-info/SOURCES.txt` & `astroemperor-0.8.3/src/astroemperor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 src/astroemperor/support/PAE/01.pae
 src/astroemperor/support/PAE/02.pae
 src/astroemperor/support/PAE/03.pae
 src/astroemperor/support/likelihoods/00.like
 src/astroemperor/support/models/acc.model
 src/astroemperor/support/models/empty.model
 src/astroemperor/support/models/ins00.model
+src/astroemperor/support/models/ins01 (copy).model
 src/astroemperor/support/models/ins01.model
 src/astroemperor/support/models/ins02.model
+src/astroemperor/support/models/ins03 (copy).model
+src/astroemperor/support/models/ins03.model
 src/astroemperor/support/models/kep00.model
 src/astroemperor/support/models/kep01.model
 src/astroemperor/support/models/kep02.model
 src/astroemperor/support/models/kep03.model
 src/astroemperor/support/pools/00.pool
 src/astroemperor/support/pools/01.pool
 src/astroemperor/support/pools/02.pool
```

