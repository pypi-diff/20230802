# Comparing `tmp/openedx-learning-0.1.0.tar.gz` & `tmp/openedx-learning-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-learning-0.1.0.tar", last modified: Wed Jul 26 04:14:03 2023, max compression
+gzip compressed data, was "openedx-learning-0.1.1.tar", last modified: Wed Aug  2 00:17:56 2023, max compression
```

## Comparing `openedx-learning-0.1.0.tar` & `openedx-learning-0.1.1.tar`

### file list

```diff
@@ -1,84 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10096 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.223893 openedx-learning-0.1.0/openedx_learning/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.223893 openedx-learning-0.1.0/openedx_learning/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.227893 openedx-learning-0.1.0/openedx_learning/contrib/media_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/contrib/media_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/contrib/media_server/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/contrib/media_server/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/contrib/media_server/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.227893 openedx-learning-0.1.0/openedx_learning/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.227893 openedx-learning-0.1.0/openedx_learning/core/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.227893 openedx-learning-0.1.0/openedx_learning/core/components/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10269 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/components/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.231893 openedx-learning-0.1.0/openedx_learning/core/contents/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.231893 openedx-learning-0.1.0/openedx_learning/core/contents/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/contents/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.231893 openedx-learning-0.1.0/openedx_learning/core/publishing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5784 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.231893 openedx-learning-0.1.0/openedx_learning/core/publishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     9060 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/model_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    17344 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/core/publishing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_learning/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/lib/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/lib/collations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6334 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/lib/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_learning/rest_api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_learning/rest_api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_learning/rest_api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.223893 openedx-learning-0.1.0/openedx_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10096 2023-07-26 04:14:02.000000 openedx-learning-0.1.0/openedx_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2460 2023-07-26 04:14:03.000000 openedx-learning-0.1.0/openedx_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 04:14:02.000000 openedx-learning-0.1.0/openedx_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 04:14:02.000000 openedx-learning-0.1.0/openedx_learning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-26 04:14:02.000000 openedx-learning-0.1.0/openedx_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-26 04:14:02.000000 openedx-learning-0.1.0/openedx_learning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_tagging/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.219892 openedx-learning-0.1.0/openedx_tagging/core/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_tagging/core/tagging/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     8556 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21475 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/openedx_tagging/core/tagging/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-26 04:14:03.235893 openedx-learning-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2830 2023-07-26 04:13:56.000000 openedx-learning-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10096 2023-08-02 00:17:56.851431 openedx-learning-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/contrib/media_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/contrib/media_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/contrib/media_server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/contrib/media_server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/contrib/media_server/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/core/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/core/components/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10269 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/components/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning/core/contents/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/core/contents/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/contents/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/core/publishing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5784 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/core/publishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     9060 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/model_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17344 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/core/publishing/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/lib/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/lib/collations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6334 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/lib/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_learning/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_learning/rest_api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.839431 openedx-learning-0.1.1/openedx_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10096 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3311 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-02 00:17:56.000000 openedx-learning-0.1.1/openedx_learning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.843431 openedx-learning-0.1.1/openedx_tagging/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.835431 openedx-learning-0.1.1/openedx_tagging/core/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)    22225 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/fixtures/language_taxonomy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.835431 openedx-learning-0.1.1/openedx_tagging/core/tagging/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/management/commands/build_language_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     8556 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22815 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8422 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/models/system_defined.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5757 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rest_api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/rules.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/openedx_tagging/core/tagging/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 00:17:56.847431 openedx-learning-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-08-02 00:17:56.851431 openedx-learning-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2830 2023-08-02 00:17:49.000000 openedx-learning-0.1.1/setup.py
```

### Comparing `openedx-learning-0.1.0/CHANGELOG.rst` & `openedx-learning-0.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/LICENSE.txt` & `openedx-learning-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/PKG-INFO` & `openedx-learning-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openedx-learning
-Version: 0.1.0
+Version: 0.1.1
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Description: openedx-learning
         =============================
```

### Comparing `openedx-learning-0.1.0/README.rst` & `openedx-learning-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/contrib/media_server/apps.py` & `openedx-learning-0.1.1/openedx_learning/contrib/media_server/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/contrib/media_server/views.py` & `openedx-learning-0.1.1/openedx_learning/contrib/media_server/views.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/components/admin.py` & `openedx-learning-0.1.1/openedx_learning/core/components/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/components/api.py` & `openedx-learning-0.1.1/openedx_learning/core/components/api.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/components/apps.py` & `openedx-learning-0.1.1/openedx_learning/core/components/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/components/migrations/0001_initial.py` & `openedx-learning-0.1.1/openedx_learning/core/components/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/components/models.py` & `openedx-learning-0.1.1/openedx_learning/core/components/models.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/contents/admin.py` & `openedx-learning-0.1.1/openedx_learning/core/contents/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/contents/api.py` & `openedx-learning-0.1.1/openedx_learning/core/contents/api.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/contents/migrations/0001_initial.py` & `openedx-learning-0.1.1/openedx_learning/core/contents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/contents/models.py` & `openedx-learning-0.1.1/openedx_learning/core/contents/models.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/publishing/admin.py` & `openedx-learning-0.1.1/openedx_learning/core/publishing/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/publishing/api.py` & `openedx-learning-0.1.1/openedx_learning/core/publishing/api.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/publishing/migrations/0001_initial.py` & `openedx-learning-0.1.1/openedx_learning/core/publishing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/publishing/model_mixins.py` & `openedx-learning-0.1.1/openedx_learning/core/publishing/model_mixins.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/core/publishing/models.py` & `openedx-learning-0.1.1/openedx_learning/core/publishing/models.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/lib/admin_utils.py` & `openedx-learning-0.1.1/openedx_learning/lib/admin_utils.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/lib/collations.py` & `openedx-learning-0.1.1/openedx_learning/lib/collations.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/lib/fields.py` & `openedx-learning-0.1.1/openedx_learning/lib/fields.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning/rest_api/v1/components.py` & `openedx-learning-0.1.1/openedx_learning/rest_api/v1/components.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_learning.egg-info/PKG-INFO` & `openedx-learning-0.1.1/openedx_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openedx-learning
-Version: 0.1.0
+Version: 0.1.1
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Description: openedx-learning
         =============================
```

### Comparing `openedx-learning-0.1.0/openedx_learning.egg-info/SOURCES.txt` & `openedx-learning-0.1.1/openedx_learning.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -51,13 +51,28 @@
 openedx_learning/rest_api/v1/components.py
 openedx_learning/rest_api/v1/urls.py
 openedx_tagging/__init__.py
 openedx_tagging/core/tagging/__init__.py
 openedx_tagging/core/tagging/admin.py
 openedx_tagging/core/tagging/api.py
 openedx_tagging/core/tagging/apps.py
-openedx_tagging/core/tagging/models.py
 openedx_tagging/core/tagging/rules.py
+openedx_tagging/core/tagging/urls.py
+openedx_tagging/core/tagging/fixtures/language_taxonomy.yaml
+openedx_tagging/core/tagging/management/commands/__init__.py
+openedx_tagging/core/tagging/management/commands/build_language_fixture.py
 openedx_tagging/core/tagging/migrations/0001_initial.py
 openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
+openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
+openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
+openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
 openedx_tagging/core/tagging/migrations/__init__.py
+openedx_tagging/core/tagging/models/__init__.py
+openedx_tagging/core/tagging/models/base.py
+openedx_tagging/core/tagging/models/system_defined.py
+openedx_tagging/core/tagging/rest_api/urls.py
+openedx_tagging/core/tagging/rest_api/v1/__init__.py
+openedx_tagging/core/tagging/rest_api/v1/permissions.py
+openedx_tagging/core/tagging/rest_api/v1/serializers.py
+openedx_tagging/core/tagging/rest_api/v1/urls.py
+openedx_tagging/core/tagging/rest_api/v1/views.py
 requirements/base.in
```

### Comparing `openedx-learning-0.1.0/openedx_tagging/core/tagging/api.py` & `openedx-learning-0.1.1/openedx_tagging/core/tagging/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,16 +102,17 @@
     Generates a list of object tags for a given object.
 
     Pass taxonomy to limit the returned object_tags to a specific taxonomy.
 
     Pass valid_only=False when displaying tags to content authors, so they can see invalid tags too.
     Invalid tags will (probably) be hidden from learners.
     """
+    ObjectTagClass = taxonomy.object_tag_class if taxonomy else ObjectTag
     tags = (
-        ObjectTag.objects.filter(
+        ObjectTagClass.objects.filter(
             object_id=object_id,
         )
         .select_related("tag", "taxonomy")
         .order_by("id")
     )
     if taxonomy:
         tags = tags.filter(taxonomy=taxonomy)
```

### Comparing `openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/0001_initial.py` & `openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py` & `openedx-learning-0.1.1/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py`

 * *Files identical despite different names*

### Comparing `openedx-learning-0.1.0/openedx_tagging/core/tagging/models.py` & `openedx-learning-0.1.1/openedx_tagging/core/tagging/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-""" Tagging app data models """
+""" Tagging app base data models """
 import logging
 from typing import List, Type, Union
 
 from django.db import models
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
-from openedx_learning.lib.fields import MultiCollationTextField, case_insensitive_char_field
+from openedx_learning.lib.fields import (
+    MultiCollationTextField,
+    case_insensitive_char_field,
+)
 
 log = logging.getLogger(__name__)
 
 
 # Maximum depth allowed for a hierarchical taxonomy's tree of tags.
 TAXONOMY_MAX_DEPTH = 3
 
@@ -62,14 +65,18 @@
     )
 
     class Meta:
         indexes = [
             models.Index(fields=["taxonomy", "value"]),
             models.Index(fields=["taxonomy", "external_id"]),
         ]
+        unique_together = [
+            ["taxonomy", "external_id"],
+            ["taxonomy", "value"],
+        ]
 
     def __repr__(self):
         """
         Developer-facing representation of a Tag.
         """
         return str(self)
 
@@ -136,22 +143,14 @@
     )
     allow_free_text = models.BooleanField(
         default=False,
         help_text=_(
             "Indicates that tags in this taxonomy need not be predefined; authors may enter their own tag values."
         ),
     )
-    system_defined = models.BooleanField(
-        default=False,
-        editable=False,
-        help_text=_(
-            "Indicates that tags and metadata for this taxonomy are maintained by the system;"
-            " taxonomy admins will not be permitted to modify them.",
-        ),
-    )
     visible_to_authors = models.BooleanField(
         default=True,
         editable=False,
         help_text=_(
             "Indicates whether this taxonomy should be visible to object authors."
         ),
     )
@@ -173,27 +172,52 @@
         """
         return str(self)
 
     def __str__(self):
         """
         User-facing string representation of a Taxonomy.
         """
+        try:
+            if self._taxonomy_class:
+                return f"<{self.taxonomy_class.__name__}> ({self.id}) {self.name}"
+        except ImportError:
+            # Log error and continue
+            log.exception(
+                f"Unable to import taxonomy_class for {self.id}: {self._taxonomy_class}"
+            )
         return f"<{self.__class__.__name__}> ({self.id}) {self.name}"
 
     @property
+    def object_tag_class(self) -> Type:
+        """
+        Returns the ObjectTag subclass associated with this taxonomy, which is ObjectTag by default.
+
+        Taxonomy subclasses may override this method to use different subclasses of ObjectTag.
+        """
+        return ObjectTag
+
+    @property
     def taxonomy_class(self) -> Type:
         """
         Returns the Taxonomy subclass associated with this instance, or None if none supplied.
 
         May raise ImportError if a custom taxonomy_class cannot be imported.
         """
         if self._taxonomy_class:
             return import_string(self._taxonomy_class)
         return None
 
+    @property
+    def system_defined(self) -> bool:
+        """
+        Indicates that tags and metadata for this taxonomy are maintained by the system;
+        taxonomy admins will not be permitted to modify them.
+        """
+        return False
+
     @taxonomy_class.setter
     def taxonomy_class(self, taxonomy_class: Union[Type, None]):
         """
         Assigns the given taxonomy_class's module path.class to the field.
 
         Must be a subclass of Taxonomy, or raises a ValueError.
         """
@@ -235,34 +259,38 @@
         self.id = taxonomy.id
         self.name = taxonomy.name
         self.description = taxonomy.description
         self.enabled = taxonomy.enabled
         self.required = taxonomy.required
         self.allow_multiple = taxonomy.allow_multiple
         self.allow_free_text = taxonomy.allow_free_text
-        self.system_defined = taxonomy.system_defined
         self.visible_to_authors = taxonomy.visible_to_authors
         self._taxonomy_class = taxonomy._taxonomy_class
         return self
 
-    def get_tags(self) -> List[Tag]:
+    def get_tags(self, tag_set: models.QuerySet = None) -> List[Tag]:
         """
         Returns a list of all Tags in the current taxonomy, from the root(s) down to TAXONOMY_MAX_DEPTH tags, in tree order.
 
+        Use `tag_set` to do an initial filtering of the tags.
+
         Annotates each returned Tag with its ``depth`` in the tree (starting at 0).
 
         Performance note: may perform as many as TAXONOMY_MAX_DEPTH select queries.
         """
         tags = []
         if self.allow_free_text:
             return tags
 
+        if tag_set is None:
+            tag_set = self.tag_set
+
         parents = None
         for depth in range(TAXONOMY_MAX_DEPTH):
-            filtered_tags = self.tag_set.prefetch_related("parent")
+            filtered_tags = tag_set.prefetch_related("parent")
             if parents is None:
                 filtered_tags = filtered_tags.filter(parent=None)
             else:
                 filtered_tags = filtered_tags.filter(parent__in=parents)
             next_parents = list(
                 filtered_tags.annotate(
                     annotated_field=models.Value(
@@ -362,40 +390,33 @@
             raise ValueError(_(f"Taxonomy ({self.id}) only allows one tag per object."))
 
         if self.required and len(tags) == 0:
             raise ValueError(
                 _(f"Taxonomy ({self.id}) requires at least one tag per object.")
             )
 
+        ObjectTagClass = self.object_tag_class
         current_tags = {
             tag.tag_ref: tag
-            for tag in ObjectTag.objects.filter(
+            for tag in ObjectTagClass.objects.filter(
                 taxonomy=self,
                 object_id=object_id,
             )
         }
         updated_tags = []
         for tag_ref in tags:
             if tag_ref in current_tags:
                 object_tag = current_tags.pop(tag_ref)
             else:
-                object_tag = ObjectTag(
+                object_tag = ObjectTagClass(
                     taxonomy=self,
                     object_id=object_id,
                 )
 
-            try:
-                object_tag.tag = self.tag_set.get(
-                    id=tag_ref,
-                )
-            except (ValueError, Tag.DoesNotExist):
-                # This might be ok, e.g. if self.allow_free_text.
-                # We'll validate below before saving.
-                object_tag.value = tag_ref
-
+            object_tag.tag_ref = tag_ref
             object_tag.resync()
             if not self.validate_object_tag(object_tag):
                 raise ValueError(
                     _(f"Invalid object tag for taxonomy ({self.id}): {tag_ref}")
                 )
             updated_tags.append(object_tag)
 
@@ -427,14 +448,15 @@
     Also, if an ObjectTag is associated with free-text Taxonomy, then the tag's value won't be stored as a standalone
     Tag in the database -- it'll be stored here.
     """
 
     id = models.BigAutoField(primary_key=True)
     object_id = case_insensitive_char_field(
         max_length=255,
+        db_index=True,
         editable=False,
         help_text=_("Identifier for the object being tagged"),
     )
     taxonomy = models.ForeignKey(
         Taxonomy,
         null=True,
         default=None,
@@ -468,14 +490,15 @@
             " becomes null (e.g. if the Tag is deleted)."
             " If the tag field is set, then tag.value takes precedence over this field."
         ),
     )
 
     class Meta:
         indexes = [
+            models.Index(fields=["taxonomy", "object_id"]),
             models.Index(fields=["taxonomy", "_value"]),
         ]
 
     def __repr__(self):
         """
         Developer-facing representation of an ObjectTag.
         """
@@ -527,14 +550,32 @@
         Returns this tag's reference string.
 
         If tag is set, then returns its id.
         Otherwise, returns the cached _value field.
         """
         return self.tag.id if self.tag_id else self._value
 
+    @tag_ref.setter
+    def tag_ref(self, tag_ref: str):
+        """
+        Sets the ObjectTag's Tag and/or value, depending on whether a valid Tag is found.
+
+        Subclasses may override this method to dynamically create Tags.
+        """
+        self.value = tag_ref
+
+        if self.taxonomy_id:
+            try:
+                self.tag = self.taxonomy.tag_set.get(pk=tag_ref)
+                self.value = self.tag.value
+            except (ValueError, Tag.DoesNotExist):
+                # This might be ok, e.g. if our taxonomy.allow_free_text, so we just pass through here.
+                # We rely on the caller to validate before saving.
+                pass
+
     def is_valid(self) -> bool:
         """
         Returns True if this ObjectTag represents a valid taxonomy tag.
 
         A valid ObjectTag must be linked to a Taxonomy, and be a valid tag in that taxonomy.
         """
         return self.taxonomy_id and self.taxonomy.validate_object_tag(self)
```

### Comparing `openedx-learning-0.1.0/openedx_tagging/core/tagging/rules.py` & `openedx-learning-0.1.1/openedx_tagging/core/tagging/rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,68 +12,67 @@
 # (Superusers can already do anything)
 is_taxonomy_admin = rules.is_staff
 
 
 @rules.predicate
 def can_view_taxonomy(user: User, taxonomy: Taxonomy = None) -> bool:
     """
-    Anyone can view an enabled taxonomy,
+    Anyone can view an enabled taxonomy or list all taxonomies,
     but only taxonomy admins can view a disabled taxonomy.
     """
-    return (taxonomy and taxonomy.enabled) or is_taxonomy_admin(user)
+    return not taxonomy or taxonomy.cast().enabled or is_taxonomy_admin(user)
 
 
 @rules.predicate
 def can_change_taxonomy(user: User, taxonomy: Taxonomy = None) -> bool:
     """
     Even taxonomy admins cannot change system taxonomies.
     """
     return is_taxonomy_admin(user) and (
-        not taxonomy or not taxonomy or (taxonomy and not taxonomy.system_defined)
+        not taxonomy or (taxonomy and not taxonomy.cast().system_defined)
     )
 
 
 @rules.predicate
-def can_change_taxonomy_tag(user: User, tag: Tag = None) -> bool:
+def can_change_tag(user: User, tag: Tag = None) -> bool:
     """
     Even taxonomy admins cannot add tags to system taxonomies (their tags are system-defined), or free-text taxonomies
     (these don't have predefined tags).
     """
+    taxonomy = tag.taxonomy.cast() if (tag and tag.taxonomy_id) else None
     return is_taxonomy_admin(user) and (
         not tag
-        or not tag.taxonomy
-        or (
-            tag.taxonomy
-            and not tag.taxonomy.allow_free_text
-            and not tag.taxonomy.system_defined
-        )
+        or not taxonomy
+        or (taxonomy and not taxonomy.allow_free_text and not taxonomy.system_defined)
     )
 
 
 @rules.predicate
 def can_change_object_tag(user: User, object_tag: ObjectTag = None) -> bool:
     """
     Taxonomy admins can create or modify object tags on enabled taxonomies.
     """
+    taxonomy = (
+        object_tag.taxonomy.cast() if (object_tag and object_tag.taxonomy_id) else None
+    )
+    object_tag = taxonomy.object_tag_class.cast(object_tag) if taxonomy else object_tag
     return is_taxonomy_admin(user) and (
-        not object_tag
-        or not object_tag.taxonomy
-        or (object_tag.taxonomy and object_tag.taxonomy.enabled)
+        not object_tag or not taxonomy or (taxonomy and taxonomy.enabled)
     )
 
 
 # Taxonomy
 rules.add_perm("oel_tagging.add_taxonomy", can_change_taxonomy)
 rules.add_perm("oel_tagging.change_taxonomy", can_change_taxonomy)
 rules.add_perm("oel_tagging.delete_taxonomy", can_change_taxonomy)
 rules.add_perm("oel_tagging.view_taxonomy", can_view_taxonomy)
 
 # Tag
-rules.add_perm("oel_tagging.add_tag", can_change_taxonomy_tag)
-rules.add_perm("oel_tagging.change_tag", can_change_taxonomy_tag)
+rules.add_perm("oel_tagging.add_tag", can_change_tag)
+rules.add_perm("oel_tagging.change_tag", can_change_tag)
 rules.add_perm("oel_tagging.delete_tag", is_taxonomy_admin)
 rules.add_perm("oel_tagging.view_tag", rules.always_allow)
 
 # ObjectTag
 rules.add_perm("oel_tagging.add_object_tag", can_change_object_tag)
 rules.add_perm("oel_tagging.change_object_tag", can_change_object_tag)
 rules.add_perm("oel_tagging.delete_object_tag", is_taxonomy_admin)
```

### Comparing `openedx-learning-0.1.0/setup.py` & `openedx-learning-0.1.1/setup.py`

 * *Files identical despite different names*

