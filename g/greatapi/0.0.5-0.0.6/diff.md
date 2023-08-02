# Comparing `tmp/greatapi-0.0.5.tar.gz` & `tmp/greatapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatapi-0.0.5.tar", last modified: Fri Jul 15 06:40:47 2022, max compression
+gzip compressed data, was "greatapi-0.0.6.tar", last modified: Wed Aug  2 17:00:08 2023, max compression
```

## Comparing `greatapi-0.0.5.tar` & `greatapi-0.0.6.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-15 06:40:31.000000 greatapi-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-07-15 06:40:47.135881 greatapi-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-07-15 06:40:31.000000 greatapi-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.127880 greatapi-0.0.5/greatapi/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/admin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/admin/static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6927 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/static/greatapi_readme.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/static/main.js
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/admin/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/admin/templates/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/authentication/login.html
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/admin/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6908 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/account.html
--rw-r--r--   0 runner    (1001) docker     (121)    12256 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/add_item.html
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/delete_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/group.html
--rw-r--r--   0 runner    (1001) docker     (121)    10805 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/history.html
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (121)    10073 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/items.html
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/dashboard/visualization.html
--rw-r--r--   0 runner    (1001) docker     (121)     9760 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (121)     8938 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/admin/templates/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/commands/runserver.py
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/commands/startapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/commands/startproject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi/conf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/conf/app_template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/__init__.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/admin.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/models.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/repository.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/router.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/app_template/schemas.py-tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/conf/project_template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/project_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/project_template/main.py-tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/conf/project_template/project_name/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/project_template/project_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/conf/project_template/project_name/settings.py-tpl
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/core/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/core/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/auth/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/auth/jwt_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/auth/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/auth/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/core/history/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/history/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/history/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/history/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/core/test_auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/test_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/test_auth/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/core/users/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/users/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/users/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/core/users/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/db/database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/db/models/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/db/models/default.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/db/models/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/multiplication.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.135881 greatapi-0.0.5/greatapi/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/cbv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/inferring_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/management.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-07-15 06:40:31.000000 greatapi-0.0.5/greatapi/utils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 06:40:47.131881 greatapi-0.0.5/greatapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-07-15 06:40:46.000000 greatapi-0.0.5/greatapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-07-15 06:40:47.000000 greatapi-0.0.5/greatapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 06:40:46.000000 greatapi-0.0.5/greatapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-15 06:40:46.000000 greatapi-0.0.5/greatapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-15 06:40:46.000000 greatapi-0.0.5/greatapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-15 06:40:46.000000 greatapi-0.0.5/greatapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-07-15 06:40:47.139881 greatapi-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-15 06:40:31.000000 greatapi-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 16:59:59.000000 greatapi-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-08-02 17:00:08.978250 greatapi-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-02 16:59:59.000000 greatapi-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/greatapi_readme.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi/admin/templates/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/authentication/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/admin/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/account.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/add_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/delete_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/dashboard/visualization.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/admin/templates/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/startapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/commands/startproject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/app_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/__init__.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/models.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/repository.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/router.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/app_template/schemas.py-tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/project_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/main.py-tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/conf/project_template/project_name/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/conf/project_template/project_name/settings.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/jwt_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/auth/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/history/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/test_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/test_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/test_auth/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/core/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/core/users/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.974250 greatapi-0.0.6/greatapi/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/greatapi/db/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/db/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.978250 greatapi-0.0.6/greatapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/cbv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/inferring_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-02 16:59:59.000000 greatapi-0.0.6/greatapi/utils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:00:08.970250 greatapi-0.0.6/greatapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 17:00:08.000000 greatapi-0.0.6/greatapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 17:00:08.978250 greatapi-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:59:59.000000 greatapi-0.0.6/setup.py
```

### Comparing `greatapi-0.0.5/LICENSE` & `greatapi-0.0.6/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Sahaj Raj Malla
+Copyright (c) 2023 Sahaj Raj Malla
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `greatapi-0.0.5/greatapi/admin/static/greatapi_readme.svg` & `greatapi-0.0.6/greatapi/admin/static/greatapi_readme.svg`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/admin/static/logo.svg` & `greatapi-0.0.6/greatapi/admin/static/logo.svg`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/admin/static/main.js` & `greatapi-0.0.6/greatapi/admin/static/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -71,13 +71,12 @@
 
 
 function onSelectAll() {
     var table = document.getElementById('item-table')
     var items = table.querySelectorAll('#checkbox')
 
     for (var i = 0; i < items.length; i++) {
-        console.log(items[i])
         items[i].checked = event.target.checked
     }
 
 
 }
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/authentication/login.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/delete_user.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
   <meta charset="UTF-8" />
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-
-  <title>{%block title%}{%endblock%}</title>
+  <title>Modal | GreatAPI</title>
   <link href="{{ url_for('static', path='/styles.css') }}" rel="stylesheet" />
   <link
     href="https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap"
     rel="stylesheet" />
   <script src="https://cdn.tailwindcss.com"></script>
   <script src="https://cdn.tailwindcss.com?plugins=forms,typography,aspect-ratio,line-clamp"></script>
+  <script href="{{ url_for('static', path='/main.js') }}"></script>
 </head>
 
-
 <body>
-  <section class="w-full h-screen flex justify-center items-center p-2">
-    <main class="max-w-md w-full flex flex-col gap-6">
-      <div class="flex justify-center items-center">
-        <img src="{{ url_for('static', path='/logo.svg') }}" alt="" class="w-52" />
-      </div>
-      <div class="bg-white px-3 sm:px-4 py-8 rounded-3xl">
-        <h2 class="text-xl text-center font-extrabold">Log In</h2>
-        <form action="" class="flex flex-col gap-4 mt-8">
-          <div>
-            <input type="text" name="Username" id="" placeholder="Username"
-              class="w-full h-12 px-4 tracking-wider font-medium text-shadeblack bg-shadegray rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300" />
-          </div>
-
-          <div class="relative select-none">
-            <input type="password" name="Password" id="user-password-login" placeholder="Password"
-              class="w-full h-12 px-4 pr-12 tracking-wider font-medium text-shadeblack bg-shadegray rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300" />
-            <span class="absolute inset-y-0 right-4 flex justify-center items-center cursor-pointer" id="eye" onclick="togglePassword('user-password-login')">
-              <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 stroke-shadeblack" viewBox="0 0 512 512">
-                <path
-                  d="M255.66 112c-77.94 0-157.89 45.11-220.83 135.33a16 16 0 00-.27 17.77C82.92 340.8 161.8 400 255.66 400c92.84 0 173.34-59.38 221.79-135.25a16.14 16.14 0 000-17.47C428.89 172.28 347.8 112 255.66 112z"
-                  fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="40" />
-                <circle cx="256" cy="256" r="80" fill="none" stroke-miterlimit="10" stroke-width="40" />
-              </svg>
-            </span>
-          </div>
-
-          <div class="mt-2">
-            <button type="button" class="w-full h-12 bg-primary text-white text-lg font-bold rounded-xl">
-              Log In
-            </button>
-          </div>
-        </form>
-      </div>
-      <div class="text-center">
-        <h6 class="text-shadeblack font-medium" id="date"></h6>
+  <section class="w-full h-screen fixed inset-0 bg-[#264073]/60 z-20 flex justify-center items-center p-2">
+    <main class="max-w-md xxl:max-w-lg w-full flex flex-col gap-6">
+      <div class="bg-white p-6 rounded-3xl">
+        <h3 class="text-lg text-blacktwo font-bold">Attention!</h3>
+        <h6 class="font-medium text-shadeblack mt-1">
+          You are about to delete your account please enter your password to
+          continue.
+        </h6>
+        <div class="relative mt-6">
+          <input type="password" name="Password" id="" placeholder="Password"
+            class="w-full h-12 px-4 pr-12 tracking-wider font-medium text-shadeblack bg-shadegray rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300" />
+          <span class="absolute inset-y-0 right-4 flex justify-center items-center cursor-pointer">
+            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 stroke-shadeblack" viewBox="0 0 512 512">
+              <path
+                d="M255.66 112c-77.94 0-157.89 45.11-220.83 135.33a16 16 0 00-.27 17.77C82.92 340.8 161.8 400 255.66 400c92.84 0 173.34-59.38 221.79-135.25a16.14 16.14 0 000-17.47C428.89 172.28 347.8 112 255.66 112z"
+                fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="40" />
+              <circle cx="256" cy="256" r="80" fill="none" stroke-miterlimit="10" stroke-width="40" />
+            </svg>
+          </span>
+        </div>
+        <div class="w-full flex justify-between items-center flex-wrap sm:flex-nowrap gap-4 mt-6">
+          <button type="button"
+            class="w-full p-3 bg-white text-lg text-shadeblack font-bold border-2 border-shadeblack flex justify-center items-center gap-2 rounded-lg tracking-wider">
+            Cancel
+          </button>
+
+          <button type="submit"
+            class="w-full p-3 bg-danger text-lg text-white font-bold border-2 border-danger flex justify-center items-center gap-2 rounded-lg tracking-wider">
+            Confirm
+          </button>
+        </div>
       </div>
     </main>
   </section>
 </body>
-<script>
-
-  let id = document.getElementById("date");
-  var date = new Date().getFullYear();
-
-  id.innerHTML = `© ${date}. <b>GreatAPI</b>`;
-</script>
-<script src="{{ url_for('static', path='/main.js') }}"></script>
 
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 
 
 
-***** Log In *****
-[Username            ]
+**** Attention! ****
+* You are about to delete your account please enter your password to continue.
+*
 [********************]
- Log In
+ Cancel   Confirm
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/add_item.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/add_item.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%extends 'base.html'%} {%block title%}Add Blog | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Add Blog | GreatAPI{%endblock%} {%block
 body%} {%include 'sidebar.html'%}
 
 <main class="w-full h-full rounded-2xl flex flex-col gap-2 xxl:gap-3">
   {%include 'navbar.html'%}
 
   <div class="w-full h-full overflow-y-scroll px-0.5">
     <div class="flex items-center gap-3 py-4 overflow-y-auto whitespace-nowrap">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{%extends 'base.html'%} {%block title%}Add Blog | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Add Blog | GreatAPI{%endblock%} {%block
 body%} {%include 'sidebar.html'%}  {%include 'navbar.html'%}
 Dashboard      Group      Blogs      Add_Blog
 ****** Add Blog ******
  Name  [name                ]
  Price  [Unknown INPUT type]
 
 ⁰  On offer
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/group.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/group.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%extends 'base.html'%} {%block title%}Group | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Group | GreatAPI{%endblock%} {%block
 body%} {%include 'sidebar.html'%}
 <!-- ends -->
 
 <main class="w-full h-full rounded-2xl flex flex-col gap-2 xxl:gap-3">
   {%include 'navbar.html'%}
 
   <div class="w-full h-full overflow-y-scroll px-0.5">
@@ -35,15 +35,15 @@
 
     <div class="w-full flex flex-wrap xl:flex-nowrap gap-2 gap-y-8 xxl:gap-4">
       <div class="w-full xl:w-2/3 h-full grid grid-cols-1 gap-3">
         <div class="block relative w-full h-fit">
           <input
             type="search"
             name="search"
-            id=""
+            id="searchInput"
             placeholder="Search contents.."
             class="w-full h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300"
           />
           <span
             class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer"
           >
             <svg
@@ -87,8 +87,30 @@
         </a>
         {%endfor%}
       </div>
     </div>
   </div>
 </main>
 
+<script>
+  document.addEventListener("DOMContentLoaded", function () {
+    const searchInput = document.getElementById("searchInput");
+    const groups = document.querySelectorAll(".w-full.bg-white.p-4"); // Modify this selector to target the elements that represent the groups.
+
+    searchInput.addEventListener("keypress", function (event) {
+      if (event.key === "Enter") {
+        const searchText = event.target.value.toLowerCase();
+        groups.forEach((group) => {
+          const groupName = group.querySelector(".font-bold.text-blacktwo")
+            .innerText.toLowerCase();
+          if (groupName.includes(searchText)) {
+            group.style.display = "block";
+          } else {
+            group.style.display = "none";
+          }
+        });
+      }
+    });
+  });
+</script>
+
 {%endblock%}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{%extends 'base.html'%} {%block title%}Group | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Group | GreatAPI{%endblock%} {%block
 body%} {%include 'sidebar.html'%}   {%include 'navbar.html'%}
 Dashboard      {{group_name}}
 [Unknown INPUT type]
 {%for item in items%}
 ****_{{item.name}}_****
 {%if_item.total_count_is_not_none_%}
 *_Total_articles:__{{item.total_count}}__*
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/history.html` & `greatapi-0.0.6/greatapi/admin/templates/navbar.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,245 +1,288 @@
-{%extends 'base.html'%} {%block title%}History | Great
-API{%endblock%} {%block body%} {%include 'sidebar.html'%}
-<!-- ends -->
-
-<main class="w-full h-full rounded-2xl flex flex-col gap-2 xxl:gap-3">
-  {%include 'navbar.html'%}
-
-  <div class="w-full h-full overflow-y-scroll">
-    <div class="flex items-center gap-3 py-4 overflow-y-auto whitespace-nowrap">
-      <a href="#" class="text-blacktwo text-sm font-medium">History</a>
-      <!-- <span class="text-blacktwo">
-              <svg
-                xmlns="http://www.w3.org/2000/svg"
-                class="w-5 h-5"
-                viewBox="0 0 20 20"
-                fill="currentColor"
-              >
-                <path
-                  fill-rule="evenodd"
-                  d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
-                  clip-rule="evenodd"
-                />
-              </svg>
-            </span>
-            <a href="#" class="text-primary text-sm font-medium">Overall</a> -->
+<div class="w-full flex justify-between items-center gap-4 pt-3 lg:p-0">
+  <div class="flex items-center gap-4">
+    <div
+      class="w-12 h-12 text-primary bg-white lg:hidden flex items-center justify-center rounded-lg cursor-pointer"
+      onclick="toggleMenu()"
+    >
+      <svg
+        xmlns="http://www.w3.org/2000/svg"
+        class="w-6 h-6"
+        viewBox="0 0 512 512"
+      >
+        <rect
+          x="48"
+          y="48"
+          width="176"
+          height="176"
+          rx="20"
+          ry="20"
+          fill="none"
+          stroke="currentColor"
+          stroke-linecap="round"
+          stroke-linejoin="round"
+          stroke-width="30"
+        />
+        <rect
+          x="288"
+          y="48"
+          width="176"
+          height="176"
+          rx="20"
+          ry="20"
+          fill="none"
+          stroke="currentColor"
+          stroke-linecap="round"
+          stroke-linejoin="round"
+          stroke-width="30"
+        />
+        <rect
+          x="48"
+          y="288"
+          width="176"
+          height="176"
+          rx="20"
+          ry="20"
+          fill="none"
+          stroke="currentColor"
+          stroke-linecap="round"
+          stroke-linejoin="round"
+          stroke-width="30"
+        />
+        <rect
+          x="288"
+          y="288"
+          width="176"
+          height="176"
+          rx="20"
+          ry="20"
+          fill="none"
+          stroke="currentColor"
+          stroke-linecap="round"
+          stroke-linejoin="round"
+          stroke-width="30"
+        />
+      </svg>
     </div>
-    <!-- ends -->
-    <div class="w-full flex flex-wrap xl:flex-nowrap gap-2 gap-y-8 xxl:gap-4">
-      <div class="w-full xl:w-2/3 h-full">
-        <div class="block relative w-full h-fit">
-          <input type="search" name="search" id="" placeholder="Search history.."
-            class="w-full h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300" />
-          <span class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer">
-            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 stroke-shadeblack" viewBox="0 0 512 512">
-              <path d="M221.09 64a157.09 157.09 0 10157.09 157.09A157.1 157.1 0 00221.09 64z" fill="none"
-                stroke-miterlimit="10" stroke-width="30" />
-              <path fill="none" stroke-linecap="round" stroke-miterlimit="10" stroke-width="30"
-                d="M338.29 338.29L448 448" />
-            </svg>
-          </span>
-        </div>
-
-        <div class="flex flex-col gap-3">
-          <div class="mt-8">
-            {%for item in history_items%}
-            <div class="flex items-start gap-4 bg-white p-4 rounded-lg my-2">
-              {%if item.category == 'edit'%}
-              <div
-                class="w-10 h-10 flex justify-center items-center rounded-lg bg-shadegray text-warning cursor-pointer">
-                <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                  <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
-                    stroke-width="32"
-                    d="M364.13 125.25L87 403l-23 45 44.99-23 277.76-277.13-22.62-22.62zM420.69 68.69l-22.62 22.62 22.62 22.63 22.62-22.63a16 16 0 000-22.62h0a16 16 0 00-22.62 0z" />
-                </svg>
-              </div>
-              <div>
-                <h4 class="text-blacktwo font-semibold">{{item.name}} Edited</h4>
-                <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                  {{item.created_date}}
-                </h6>
-              </div>
-              {%elif item.category == 'create'%}
-              <div
-                class="w-10 h-10 flex justify-center items-center rounded-lg text-success bg-shadegray cursor-pointer">
-                <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                  <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
-                    stroke-width="32" d="M416 128L192 384l-96-96" />
-                </svg>
-              </div>
-              <div>
-                <h4 class="text-blacktwo font-semibold">{{item.name}} Added</h4>
-                <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                  {{item.created_date}}
-                </h6>
-              </div>
-
-              {%else%}
-              <div
-              class="w-10 h-10 flex justify-center items-center rounded-lg text-danger bg-shadegray cursor-pointer">
-
-            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="red" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="3 6 5 6 21 6"></polyline><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"></path><line x1="10" y1="11" x2="10" y2="17"></line><line x1="14" y1="11" x2="14" y2="17"></line></svg>
+    <div class="hidden sm:block relative">
+      <!--
+      <input
+        type="search"
+        name="search"
+        id=""
+        placeholder="Search"
+        autocomplete="off"
+        class="w-96 h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300"
+      />
+      -->
+      <span
+        class="bg-white rounded inset-y-0 left-2 flex justify-center items-center cursor-pointer px-4 py-3"
+      >
+      <b>GreatAPI Administrator</b>
+        <!--<svg
+          xmlns="http://www.w3.org/2000/svg"
+          class="w-6 h-6 stroke-shadeblack"
+          viewBox="0 0 512 512"
+        >
+          <path
+            d="M221.09 64a157.09 157.09 0 10157.09 157.09A157.1 157.1 0 00221.09 64z"
+            fill="none"
+            stroke-miterlimit="10"
+            stroke-width="30"
+          />
+          <path
+            fill="none"
+            stroke-linecap="round"
+            stroke-miterlimit="10"
+            stroke-width="30"
+            d="M338.29 338.29L448 448"
+          />
+        </svg>
+      -->
+      </span>
+      <!-- search results -->
+      <!-- <div
+        class="w-full absolute bg-white mt-2 h-72 p-3 rounded-xl shadow-[0_10px_20px_rgb(0,0,0,0.03)]"
+      >
+        <div class="w-full h-full overflow-auto flex flex-col gap-2">
+          <a href="">
+            <div class="w-full p-2 bg-shadegray rounded-lg">
+              <h3 class="font-semibold text-blacktwo">Search result</h3>
+              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
             </div>
-            <div>
-              <h4 class="text-blacktwo font-semibold">{{item.name}} Deleted</h4>
-              <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                {{item.created_date}}
-              </h6>
+          </a>
+          <a href="">
+            <div class="w-full p-2 bg-shadegray rounded-lg">
+              <h3 class="font-semibold text-blacktwo">Search result</h3>
+              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
             </div>
-            {%endif%}
+          </a>
+          <a href="">
+            <div class="w-full p-2 bg-shadegray rounded-lg">
+              <h3 class="font-semibold text-blacktwo">Search result</h3>
+              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
             </div>
-
-            {%endfor%}
-          </div>
-
-          <!-- <div class="flex items-start gap-4 bg-white p-4 rounded-lg mt-12">
-            <div
-              class="w-10 h-10 flex justify-center items-center rounded-lg bg-shadegray text-warning cursor-pointer"
-            >
-              <svg
-                xmlns="http://www.w3.org/2000/svg"
-                class="w-5 h-5"
-                viewBox="0 0 512 512"
-              >
-                <path
-                  fill="none"
-                  stroke="currentColor"
-                  stroke-linecap="round"
-                  stroke-linejoin="round"
-                  stroke-width="32"
-                  d="M364.13 125.25L87 403l-23 45 44.99-23 277.76-277.13-22.62-22.62zM420.69 68.69l-22.62 22.62 22.62 22.63 22.62-22.63a16 16 0 000-22.62h0a16 16 0 00-22.62 0z"
-                />
-              </svg>
-            </div>
-            <div>
-              <h4 class="text-blacktwo font-semibold">Item Edited</h4>
-              <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                Feb 20, 2022
-              </h6>
+          </a>
+          <a href="">
+            <div class="w-full p-2 bg-shadegray rounded-lg">
+              <h3 class="font-semibold text-blacktwo">Search result</h3>
+              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
             </div>
-          </div>
-
-          <div class="flex items-start gap-4 bg-white p-4 rounded-lg">
-            <div
-              class="w-10 h-10 flex justify-center items-center rounded-lg text-success bg-shadegray cursor-pointer"
-            >
-              <svg
-                xmlns="http://www.w3.org/2000/svg"
-                class="w-5 h-5"
-                viewBox="0 0 512 512"
-              >
-                <path
-                  fill="none"
-                  stroke="currentColor"
-                  stroke-linecap="round"
-                  stroke-linejoin="round"
-                  stroke-width="32"
-                  d="M416 128L192 384l-96-96"
-                />
-              </svg>
-            </div>
-            <div>
-              <h4 class="text-blacktwo font-semibold">New Item Added</h4>
-              <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                Feb 20, 2022
-              </h6>
+          </a>
+          <a href="">
+            <div class="w-full p-2 bg-shadegray rounded-lg">
+              <h3 class="font-semibold text-blacktwo">Search result</h3>
+              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
             </div>
-          </div> -->
+          </a>
         </div>
+      </div> -->
+      <!-- end search results -->
+    </div>
+  </div>
+  <!-- nav ends -->
 
-        <div class="flex gap-2 mt-8 justify-between sm:justify-end">
-          <a href="#"
-            class="px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline cursor-not-allowed">
-            <div class="flex items-center -mx-1">
-              <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="48"
-                  d="M328 112L184 256l144 144" />
-              </svg>
-
-              <span class="mx-1">Prev</span>
+  <!-- ends -->
+  <div class="flex gap-4">
+    <div
+      class="w-12 h-12 flex justify-center items-center rounded-xl bg-white cursor-pointer"
+    >
+      <a href="/" target="_blank">
+        <svg
+          xmlns="http://www.w3.org/2000/svg"
+          class="w-6 h-6 stroke-primary"
+          viewBox="0 0 512 512"
+        >
+          <path
+            d="M384 224v184a40 40 0 01-40 40H104a40 40 0 01-40-40V168a40 40 0 0140-40h167.48M336 64h112v112M224 288L440 72"
+            fill="none"
+            stroke-linecap="round"
+            stroke-linejoin="round"
+            stroke-width="32"
+          />
+        </svg>
+      </a>
+    </div>
+    <!-- account settings -->
+    <div class="relative" id="account-settings">
+      <div
+        class="h-12 select-none flex justify-center items-center p-2 rounded-xl bg-white cursor-pointer"
+        onclick="togglePopup()"
+      >
+        <!-- <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 stroke-primary" viewBox="0 0 512 512">
+          <path
+            d="M262.29 192.31a64 64 0 1057.4 57.4 64.13 64.13 0 00-57.4-57.4zM416.39 256a154.34 154.34 0 01-1.53 20.79l45.21 35.46a10.81 10.81 0 012.45 13.75l-42.77 74a10.81 10.81 0 01-13.14 4.59l-44.9-18.08a16.11 16.11 0 00-15.17 1.75A164.48 164.48 0 01325 400.8a15.94 15.94 0 00-8.82 12.14l-6.73 47.89a11.08 11.08 0 01-10.68 9.17h-85.54a11.11 11.11 0 01-10.69-8.87l-6.72-47.82a16.07 16.07 0 00-9-12.22 155.3 155.3 0 01-21.46-12.57 16 16 0 00-15.11-1.71l-44.89 18.07a10.81 10.81 0 01-13.14-4.58l-42.77-74a10.8 10.8 0 012.45-13.75l38.21-30a16.05 16.05 0 006-14.08c-.36-4.17-.58-8.33-.58-12.5s.21-8.27.58-12.35a16 16 0 00-6.07-13.94l-38.19-30A10.81 10.81 0 0149.48 186l42.77-74a10.81 10.81 0 0113.14-4.59l44.9 18.08a16.11 16.11 0 0015.17-1.75A164.48 164.48 0 01187 111.2a15.94 15.94 0 008.82-12.14l6.73-47.89A11.08 11.08 0 01213.23 42h85.54a11.11 11.11 0 0110.69 8.87l6.72 47.82a16.07 16.07 0 009 12.22 155.3 155.3 0 0121.46 12.57 16 16 0 0015.11 1.71l44.89-18.07a10.81 10.81 0 0113.14 4.58l42.77 74a10.8 10.8 0 01-2.45 13.75l-38.21 30a16.05 16.05 0 00-6.05 14.08c.33 4.14.55 8.3.55 12.47z"
+            fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="32" />
+        </svg> -->Admin
+      </div>
+      <div
+        id="account-identifier"
+        class="w-44 xxl:w-48 bg-white absolute z-10 right-0 mt-2 rounded-xl p-2 xl:p-3 shadow-[0_10px_20px_rgb(0,0,0,0.03)]"
+        style="display: none"
+      >
+        <div class="flex flex-col gap-1 w-full text-center">
+          <a href="{{ '/admin/account' }}">
+            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg">
+              <h4 class="text-blacktwo font-semibold">Account</h4>
             </div>
           </a>
-
-          <a href="#"
-            class="hidden px-4 py-2 font-semibold text-primary hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
-            1
-          </a>
-
-          <a href="#"
-            class="hidden px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
-            2
-          </a>
-
-          <a href="#"
-            class="hidden px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
-            3
-          </a>
-
-          <a href="#"
-            class="hidden px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
-            4
+          <!--<a href="">
+            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg">
+              <h4 class="text-blacktwo font-semibold">Dark</h4>
+            </div>
           </a>
-
-          <a href="#"
-            class="px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
-            <div class="flex items-center -mx-1">
-              <span class="mx-1"> Next </span>
-
-              <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="48"
-                  d="M184 112l144 144-144 144" />
-              </svg>
+        -->
+          <a>
+            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg" onclick="performLogout()">
+              <h4 class="text-blacktwo font-semibold">Logout</h4>
             </div>
           </a>
         </div>
       </div>
-      <!-- ends -->
-      <div class="w-full xl:w-1/3 h-fit bg-white p-4 rounded-2xl flex flex-col gap-4">
-        <div class="flex justify-between items-center">
-          <h3 class="text-lg font-semibold text-blacktwo">Filter</h3>
-        </div>
 
-        <hr class="border-shadeblack/30" />
-
-        <div class="flex flex-col gap-3">
-          <div class="flex flex-col gap-2">
-            <h2 class="text-lg font-semibold text-blacktwo">Status</h2>
-            <ul class="flex flex-col gap-1">
-              <li>
-                <a href="/admin/history" class="text-primary font-medium">All</a>
-              </li>
-              <li>
-                <a href="{%if params %}{{params}}&draft=True{%else%}?Draft=True{%endif%}" class="text-shadeblack font-medium">Draft</a>
-              </li>
-              <li>
-                <a href="{%if params %}{{params}}&Published=True{%else%}?Published=True{%endif%}" class="text-shadeblack font-medium">Published</a>
-              </li>
-            </ul>
-          </div>
-          <div class="flex flex-col gap-2">
-            <h2 class="text-lg font-semibold text-blacktwo">Date</h2>
-            <ul class="flex flex-col gap-1">
-              <li>
-                <a href="" class="text-primary font-medium">Any Date</a>
-              </li>
-              <li>
-                <a href="" class="text-shadeblack font-medium">Today</a>
-              </li>
-              <li>
-                <a href="" class="text-shadeblack font-medium">This Week</a>
-              </li>
-              <li>
-                <a href="" class="text-shadeblack font-medium">This Month</a>
-              </li>
-              <li>
-                <a href="" class="text-shadeblack font-medium">This Year</a>
-              </li>
-            </ul>
-          </div>
+    </div>
+  </div>
+</div>
+<!-- nav ends -->
+<!--
+<div class="sm:hidden relative w-full">
+  <input
+    type="search"
+    name="search"
+    id=""
+    placeholder="Search"
+    autocomplete="off"
+    class="w-full h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none focus:ring-1 focus:ring-primary/70 duration-300"
+  />
+  <span
+    class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer"
+  >
+    <svg
+      xmlns="http://www.w3.org/2000/svg"
+      class="w-6 h-6 stroke-shadeblack"
+      viewBox="0 0 512 512"
+    >
+      <path
+        d="M221.09 64a157.09 157.09 0 10157.09 157.09A157.1 157.1 0 00221.09 64z"
+        fill="none"
+        stroke-miterlimit="10"
+        stroke-width="30"
+      />
+      <path
+        fill="none"
+        stroke-linecap="round"
+        stroke-miterlimit="10"
+        stroke-width="30"
+        d="M338.29 338.29L448 448"
+      />
+    </svg>
+  </span>
+  <div
+    class="hidden w-full absolute bg-white mt-2 h-72 p-3 rounded-xl shadow-xl"
+  >
+    <div class="w-full h-full overflow-auto flex flex-col gap-2">
+      <a href="">
+        <div class="w-full p-2 bg-shadegray rounded-lg">
+          <h3 class="font-semibold text-blacktwo">Search result</h3>
+          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
         </div>
-      </div>
+      </a>
+      <a href="">
+        <div class="w-full p-2 bg-shadegray rounded-lg">
+          <h3 class="font-semibold text-blacktwo">Search result</h3>
+          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
+        </div>
+      </a>
+      <a href="">
+        <div class="w-full p-2 bg-shadegray rounded-lg">
+          <h3 class="font-semibold text-blacktwo">Search result</h3>
+          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
+        </div>
+      </a>
+      <a href="">
+        <div class="w-full p-2 bg-shadegray rounded-lg">
+          <h3 class="font-semibold text-blacktwo">Search result</h3>
+          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
+        </div>
+      </a>
+      <a href="">
+        <div class="w-full p-2 bg-shadegray rounded-lg">
+          <h3 class="font-semibold text-blacktwo">Search result</h3>
+          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
+        </div>
+      </a>
     </div>
   </div>
-</main>
+</div>
+
+-->
+<!-- mobile search -->
 
-{%endblock%}
+<script>
+  function performLogout() {
+    // Remove the access_token from localStorage
+    localStorage.removeItem('access_token');
+
+    // Redirect to the login page or another appropriate page after logout.
+    window.location.href = '/admin/login';
+  }
+</script>
```

#### html2text {}

```diff
@@ -1,34 +1,10 @@
-{%extends 'base.html'%} {%block title%}History | Great API{%endblock%} {%block
-body%} {%include 'sidebar.html'%}   {%include 'navbar.html'%}
-History
-[Unknown INPUT type]
-{%for item in history_items%}
-{%if item.category == 'edit'%}
 
-*** {{item.name}} Edited ***
-* {{item.created_date}} *
-{%elif item.category == 'create'%}
+  GreatAPI Administrator
+
+__
+Admin
+***_Account_***
+
+*** Logout ***
+
 
-*** {{item.name}} Added ***
-* {{item.created_date}} *
-{%else%}
-*** {{item.name}} Deleted ***
-* {{item.created_date}} *
-{%endif%}
-{%endfor%}
-   Prev
- 1 2 3 4
- Next
-**** Filter ****
-===============================================================================
-***** Status *****
-    * All
-    * Draft
-    * Published
-***** Date *****
-    * Any Date
-    * Today
-    * This Week
-    * This Month
-    * This Year
- {%endblock%}
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/index.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-{%extends 'base.html'%} {%block title%}Great API{%endblock%}
+{%extends 'base.html'%} {%block title%}GreatAPI{%endblock%}
 {%block body%} {%include 'sidebar.html'%}
-<!-- ends -->
 
 <main class="w-full h-full rounded-2xl flex flex-col gap-2 xxl:gap-3">
   {%include 'navbar.html'%}
   <div class="w-full h-full overflow-y-scroll">
     <div class="flex items-center gap-3 py-4 overflow-y-auto whitespace-nowrap">
       <a href="{{ '/admin' }}" class="text-blacktwo text-sm font-medium">Dashboard</a>
-      <!-- <span class="text-blacktwo">
-              <svg
-                xmlns="http://www.w3.org/2000/svg"
-                class="w-5 h-5"
-                viewBox="0 0 20 20"
-                fill="currentColor"
-              >
-                <path
-                  fill-rule="evenodd"
-                  d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
-                  clip-rule="evenodd"
-                />
-              </svg>
-            </span>
-            <a href="#" class="text-primary text-sm font-medium">Overall</a> -->
     </div>
-    <!-- ends -->
     <div class="w-full flex flex-wrap xl:flex-nowrap gap-2 gap-y-8 xxl:gap-4">
       <div class="w-full xl:w-2/3 h-full grid grid-cols-1 xs:grid-cols-2 xxl:grid-cols-3 gap-3">
         {%for group in groups%}
         <a href="{{ '/admin/%s' % group.name }}">
           <div class="w-full bg-white p-4 flex justify-between rounded-2xl cursor-pointer">
             <div class="flex flex-col gap-3">
               <h3 class="font-bold text-blacktwo">{{group.name}}</h3>
@@ -38,57 +21,66 @@
             </div>
 
           </div>
         </a>
         {%endfor%}
       </div>
 
-      <div class="w-full xl:w-1/3 h-fit bg-white p-4 rounded-2xl flex flex-col gap-4">
+    <div class="w-full xl:w-1/3 h-fit bg-white p-4 rounded-2xl flex flex-col gap-4">
         <div class="flex justify-between items-center">
           <h3 class="text-lg font-semibold text-blacktwo">History</h3>
           <a href="{{ 'admin/history' }}">
             <h6 class="text-sm font-medium text-primary cursor-pointer">
               View All
             </h6>
           </a>
         </div>
 
+
         <hr class="border-shadeblack/30" />
 
-        <div class="flex flex-col gap-3">
+        <div class="flex flex-col gap-1">
           {%for item in history_items%}
-          <div class="flex items-start gap-4 my-1">
-            {%if item.type == 'edit'%}
-            <div class="w-10 h-10 flex justify-center items-center rounded-lg bg-shadegray text-warning cursor-pointer">
+          <div class="flex items-start gap-2 bg-white p-2 rounded-lg my-2">
+            {%if item.category == 'edit'%}
+            <div
+              class="flex justify-center items-center rounded-lg bg-shadegray text-warning cursor-pointer">
               <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="32"
+                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
+                  stroke-width="32"
                   d="M364.13 125.25L87 403l-23 45 44.99-23 277.76-277.13-22.62-22.62zM420.69 68.69l-22.62 22.62 22.62 22.63 22.62-22.63a16 16 0 000-22.62h0a16 16 0 00-22.62 0z" />
               </svg>
             </div>
             <div>
-              <h4 class="text-blacktwo font-semibold">Item Edited</h4>
-              <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                {{item.date}}
-              </h6>
+              <h4 class="text-blacktwo font-semibold">{{item.name}}</h4>
             </div>
-            {%else%}
-            <div class="w-10 h-10 flex justify-center items-center rounded-lg text-success bg-shadegray cursor-pointer">
+            {%elif item.category == 'create'%}
+            <div
+              class="flex justify-center items-center rounded-lg text-success bg-shadegray cursor-pointer">
               <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
-                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="32"
-                  d="M416 128L192 384l-96-96" />
+                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
+                  stroke-width="32" d="M416 128L192 384l-96-96" />
               </svg>
             </div>
             <div>
-              <h4 class="text-blacktwo font-semibold">New Item Added</h4>
-              <h6 class="text-xs xxl:text-sm font-medium text-shadeblack">
-                {{item.date}}
-              </h6>
+              <h4 class="text-blacktwo font-semibold">{{item.name}}</h4>
             </div>
-            {%endif%}
+
+            {%else%}
+            <div
+            class="flex justify-center items-center rounded-lg text-danger bg-shadegray cursor-pointer">
+
+          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="red" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="3 6 5 6 21 6"></polyline><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"></path><line x1="10" y1="11" x2="10" y2="17"></line><line x1="14" y1="11" x2="14" y2="17"></line></svg>
           </div>
+          <div>
+            <h4 class="text-blacktwo font-semibold">{{item.name}}</h4>
+          </div>
+          {%endif%}
+          </div>
+
           {%endfor%}
         </div>
       </div>
     </div>
   </div>
 </main>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-{%extends 'base.html'%} {%block title%}Great API{%endblock%} {%block body%}
-{%include 'sidebar.html'%}   {%include 'navbar.html'%}
+{%extends 'base.html'%} {%block title%}GreatAPI{%endblock%} {%block body%}
+{%include 'sidebar.html'%}  {%include 'navbar.html'%}
 Dashboard
 {%for group in groups%}
 ****_{{group.name}}_****
 *_Total_User:_{{group.total_count}}_*
  {%endfor%}
 **** History ****
 *_View_All_*
 ===============================================================================
 {%for item in history_items%}
-{%if item.type == 'edit'%}
+{%if item.category == 'edit'%}
 
-*** Item Edited ***
-* {{item.date}} *
-{%else%}
+*** {{item.name}} ***
+{%elif item.category == 'create'%}
 
-*** New Item Added ***
-* {{item.date}} *
+*** {{item.name}} ***
+{%else%}
+*** {{item.name}} ***
 {%endif%}
 {%endfor%}
  {%endblock%}
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/items.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/items.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%extends 'base.html'%} {%block title%}Blogs | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Blogs | GreatAPI{%endblock%} {%block
 body%}
   {%include 'sidebar.html'%}
   <!-- ends -->
 
   <main class="w-full h-full rounded-2xl flex flex-col gap-2 xxl:gap-3">
     {%include 'navbar.html'%}
 
@@ -58,15 +58,15 @@
         class="w-full flex flex-w rap xl:flex-nowrap gap-2 gap-y-8 xxl:gap-4"
       >
         <div class="w-full xl:w-2/3 h-full grid grid-cols-1 gap-3">
           <div class="block relative w-full h-fit">
             <input
               type="search"
               name="search"
-              id=""
+              id="item-search"
               placeholder="Search contents.."
               class="w-full h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300"
             />
             <span
               class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer"
             >
               <svg
@@ -87,15 +87,15 @@
                   stroke-width="30"
                   d="M338.29 338.29L448 448"
                 />
               </svg>
             </span>
           </div>
 
-          <div class="flex justify-between items-center gap-2 sm:gap-4">
+          <!--<div class="flex justify-between items-center gap-2 sm:gap-4">
             <button
               type="button"
               class="p-3 bg-white text-primary font-semibold flex items-center gap-2 rounded-lg"
             >
               <input
                 type="checkbox"
                 id="checkbox"
@@ -142,50 +142,53 @@
                     d="M24.2,12.193,23.8,24.3a3.988,3.988,0,0,1-4,3.857H12.2a3.988,3.988,0,0,1-4-3.853L7.8,12.193a1,1,0,0,1,2-.066l.4,12.11a2,2,0,0,0,2,1.923h7.6a2,2,0,0,0,2-1.927l.4-12.106a1,1,0,0,1,2,.066Zm1.323-4.029a1,1,0,0,1-1,1H7.478a1,1,0,0,1,0-2h3.1a1.276,1.276,0,0,0,1.273-1.148,2.991,2.991,0,0,1,2.984-2.694h2.33a2.991,2.991,0,0,1,2.984,2.694,1.276,1.276,0,0,0,1.273,1.148h3.1A1,1,0,0,1,25.522,8.164Zm-11.936-1h4.828a3.3,3.3,0,0,1-.255-.944,1,1,0,0,0-.994-.9h-2.33a1,1,0,0,0-.994.9A3.3,3.3,0,0,1,13.586,7.164Zm1.007,15.151V13.8a1,1,0,0,0-2,0v8.519a1,1,0,0,0,2,0Zm4.814,0V13.8a1,1,0,0,0-2,0v8.519a1,1,0,0,0,2,0Z"
                   />
                 </svg>
                 Remove
               </button>
             </div>
           </div>
+        -->
 
           <div class="overflow-auto rounded-xl">
             <table id="item-table" class="w-full bg-white">
               <thead>
                 <tr class="text-left">
-                  <th
+                  <!--<th
                     class="w-20 text-sm text-blacktwo font-bold py-5 px-4 whitespace-nowrap"
                   >
                     Select
                   </th>
+                -->
                   {%for title in titles%}
                   <th
                     class="text-sm text-blacktwo font-bold py-5 px-4 whitespace-nowrap"
                   >
                     {{title}}
                   </th>
                   {%endfor%}
                 </tr>
               </thead>
               <tbody>
                 {%for item in items%}
-                <tr>
-                  <td class="py-3 px-4 whitespace-nowrap">
+                <tr class="group-item">
+                  <!--<td class="py-3 px-4 whitespace-nowrap">
                     <input
                       type="checkbox"
                       id="checkbox"
                       class="w-6 h-6 rounded-md border-primary outline-none focus:ring-0 appearance-none checked:bg-primary"
                     />
                   </td>
+                  <-->
                   {%for content in item%}
                   <td
                     class="text-sm text-primary font-semibold py-3 px-4 cursor-pointer whitespace-nowrap"
                   >
-                    <a
+                    <!--<a
                       href="{{ '/admin/%s/%s/%s' % (group_name, group_item, item.id) }}"
-                    >
+                    >-->
                       {{content}}
                     </a>
                   </td>
                   {%endfor%}
                 </tr>
                 {%endfor%}
                 <!-- <td
@@ -196,16 +199,44 @@
                       class="w-5 h-5 rounded-md border-primary outline-none focus:ring-0 appearance-none checked:bg-primary"
                     />
                     Pin
                   </td> -->
               </tbody>
             </table>
           </div>
+          <div class="flex gap-2 mt-8 justify-between sm:justify-end">
+            <a onclick="prevPage()"
+              class="px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline cursor-not-allowed">
+              <div class="flex items-center -mx-1">
+                <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
+                  <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="48"
+                    d="M328 112L184 256l144 144" />
+                </svg>
+
+                <span class="mx-1">Prev</span>
+              </div>
+            </a>
+
+
+            <a onclick="nextPage()"
+              class="px-4 py-2 font-semibold text-blacktwo hover:text-white bg-white hover:bg-primary duration-300 rounded-md sm:inline">
+              <div class="flex items-center -mx-1">
+                <span class="mx-1"> Next </span>
+
+                <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 512 512">
+                  <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="48"
+                    d="M184 112l144 144-144 144" />
+                </svg>
+              </div>
+            </a>
+          </div>
+        </div>
         </div>
 
+        <!--
         <div
           class="w-full xl:w-1/3 h-fit bg-white p-4 rounded-2xl flex flex-col gap-4"
         >
           <div class="flex justify-between items-center">
             <h3 class="text-lg font-semibold text-blacktwo">Filter</h3>
           </div>
 
@@ -256,12 +287,43 @@
                 <li>
                   <a href="" class="text-shadeblack font-medium">This Year</a>
                 </li>
               </ul>
             </div>
           </div>
         </div>
-      </div>
+      </div>-->
     </div>
   </main>
+  <script>
+    let currentPage = parseInt(new URLSearchParams(window.location.search).get('page') || 1);
+    let name = new URLSearchParams(window.location.search).get('name') || "all_history";
+    const groupName = "{{ group_name|lower }}";
+    const groupItem = "{{ group_item|lower }}";
+
+    function nextPage() {
+      window.location.href = `/admin/${groupName}/${groupItem}?page=${currentPage + 1}&name=${name}`;
+
+    }
+
+
+    function prevPage() {
+      if (currentPage > 1) {
+        window.location.href = `/admin/${groupName}/${groupItem}?page=${currentPage - 1}&name=${name}`;
+      }
+    }
+
+
+    document.addEventListener("DOMContentLoaded", function () {
+      const searchInput = document.getElementById("item-search");
 
+      searchInput.addEventListener("keypress", function (event) {
+        if (event.key === "Enter") {
+          const searchText = event.target.value.toLowerCase();
+          name = searchText;
+          currentPage = 1;
+          window.location.href = `/admin/${groupName}/${groupItem}?page=${currentPage}&name=${name}`;
+        }
+      });
+    });
+  </script>
   {%endblock%}
```

#### html2text {}

```diff
@@ -1,21 +1,10 @@
-{%extends 'base.html'%} {%block title%}Blogs | Great API{%endblock%} {%block
+{%extends 'base.html'%} {%block title%}Blogs | GreatAPI{%endblock%} {%block
 body%} {%include 'sidebar.html'%}   {%include 'navbar.html'%}
 Dashboard      {{group_name}}      {{group_item}}
 [Unknown INPUT type]
- ⁰ Select All
-______Add_     Remove
-Select {{title}}
-⁰    {{content}}
-**** Filter ****
-===============================================================================
-***** Status *****
-    * All
-    * Draft
-    * Published
-***** Date *****
-    * Any Date
-    * Today
-    * This Week
-    * This Month
-    * This Year
+{{title}}
+ {{content}}
+   Prev
+
+ Next
  {%endblock%}
```

### Comparing `greatapi-0.0.5/greatapi/admin/templates/dashboard/visualization.html` & `greatapi-0.0.6/greatapi/admin/templates/dashboard/visualization.html`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/admin/templates/navbar.html` & `greatapi-0.0.6/greatapi/admin/templates/sidebar.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,273 +1,271 @@
-<div class="w-full flex justify-between items-center gap-4 pt-3 lg:p-0">
-  <div class="flex items-center gap-4">
+<main
+  id="menu-box"
+  class="absolute z-10 hidden lg:static lg:block h-full w-fit rounded-2xl bg-white p-3"
+>
+  <div class="flex-col justify-between gap-4  w-60 h-full flex">
     <div
-      class="w-12 h-12 text-primary bg-white lg:hidden flex items-center justify-center rounded-lg cursor-pointer"
       onclick="toggleMenu()"
+      class="absolute right-4 w-8 h-8 bg-primary/10 rounded-lg text-primary lg:hidden flex justify-center items-center"
     >
       <svg
         xmlns="http://www.w3.org/2000/svg"
-        class="w-6 h-6"
+        class="w-5 h-5"
         viewBox="0 0 512 512"
       >
-        <rect
-          x="48"
-          y="48"
-          width="176"
-          height="176"
-          rx="20"
-          ry="20"
+        <path
           fill="none"
           stroke="currentColor"
           stroke-linecap="round"
           stroke-linejoin="round"
-          stroke-width="30"
-        />
-        <rect
-          x="288"
-          y="48"
-          width="176"
-          height="176"
-          rx="20"
-          ry="20"
-          fill="none"
-          stroke="currentColor"
-          stroke-linecap="round"
-          stroke-linejoin="round"
-          stroke-width="30"
-        />
-        <rect
-          x="48"
-          y="288"
-          width="176"
-          height="176"
-          rx="20"
-          ry="20"
-          fill="none"
-          stroke="currentColor"
-          stroke-linecap="round"
-          stroke-linejoin="round"
-          stroke-width="30"
-        />
-        <rect
-          x="288"
-          y="288"
-          width="176"
-          height="176"
-          rx="20"
-          ry="20"
-          fill="none"
-          stroke="currentColor"
-          stroke-linecap="round"
-          stroke-linejoin="round"
-          stroke-width="30"
+          stroke-width="32"
+          d="M368 368L144 144M368 144L144 368"
         />
       </svg>
     </div>
-    <div class="hidden sm:block relative">
-      <input
-        type="search"
-        name="search"
-        id=""
-        placeholder="Search"
-        autocomplete="off"
-        class="w-96 h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none border-0 focus:ring-1 focus:ring-primary/70 duration-300"
-      />
-      <span
-        class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer"
-      >
-        <svg
-          xmlns="http://www.w3.org/2000/svg"
-          class="w-6 h-6 stroke-shadeblack"
-          viewBox="0 0 512 512"
-        >
-          <path
-            d="M221.09 64a157.09 157.09 0 10157.09 157.09A157.1 157.1 0 00221.09 64z"
-            fill="none"
-            stroke-miterlimit="10"
-            stroke-width="30"
-          />
-          <path
-            fill="none"
-            stroke-linecap="round"
-            stroke-miterlimit="10"
-            stroke-width="30"
-            d="M338.29 338.29L448 448"
+    <div class="flex flex-col gap-6">
+      <a href="/admin" class="mt-6">
+        <div class="flex justify-center items-center">
+          <img
+            src="{{ url_for('static', path='/logo.svg') }}"
+            alt=""
+            class="w-2/3"
           />
-        </svg>
-      </span>
-      <!-- search results -->
-      <!-- <div
-        class="w-full absolute bg-white mt-2 h-72 p-3 rounded-xl shadow-[0_10px_20px_rgb(0,0,0,0.03)]"
-      >
-        <div class="w-full h-full overflow-auto flex flex-col gap-2">
-          <a href="">
-            <div class="w-full p-2 bg-shadegray rounded-lg">
-              <h3 class="font-semibold text-blacktwo">Search result</h3>
-              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-            </div>
-          </a>
-          <a href="">
-            <div class="w-full p-2 bg-shadegray rounded-lg">
-              <h3 class="font-semibold text-blacktwo">Search result</h3>
-              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-            </div>
-          </a>
-          <a href="">
-            <div class="w-full p-2 bg-shadegray rounded-lg">
-              <h3 class="font-semibold text-blacktwo">Search result</h3>
-              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-            </div>
-          </a>
-          <a href="">
-            <div class="w-full p-2 bg-shadegray rounded-lg">
-              <h3 class="font-semibold text-blacktwo">Search result</h3>
-              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-            </div>
-          </a>
-          <a href="">
-            <div class="w-full p-2 bg-shadegray rounded-lg">
-              <h3 class="font-semibold text-blacktwo">Search result</h3>
-              <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-            </div>
-          </a>
         </div>
-      </div> -->
-      <!-- end search results -->
-    </div>
-  </div>
-  <!-- nav ends -->
-
-  <!-- ends -->
-  <div class="flex gap-4">
-    <div
-      class="w-12 h-12 flex justify-center items-center rounded-xl bg-white cursor-pointer"
-    >
-      <a href="/" target="_blank">
-        <svg
-          xmlns="http://www.w3.org/2000/svg"
-          class="w-6 h-6 stroke-primary"
-          viewBox="0 0 512 512"
-        >
-          <path
-            d="M384 224v184a40 40 0 01-40 40H104a40 40 0 01-40-40V168a40 40 0 0140-40h167.48M336 64h112v112M224 288L440 72"
-            fill="none"
-            stroke-linecap="round"
-            stroke-linejoin="round"
-            stroke-width="32"
-          />
-        </svg>
       </a>
-    </div>
-    <!-- account settings -->
-    <div class="relative" id="account-settings">
-      <div
-        class="h-12 select-none flex justify-center items-center p-2 rounded-xl bg-white cursor-pointer"
-        onclick="togglePopup()"
-      >
-        <!-- <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 stroke-primary" viewBox="0 0 512 512">
-          <path
-            d="M262.29 192.31a64 64 0 1057.4 57.4 64.13 64.13 0 00-57.4-57.4zM416.39 256a154.34 154.34 0 01-1.53 20.79l45.21 35.46a10.81 10.81 0 012.45 13.75l-42.77 74a10.81 10.81 0 01-13.14 4.59l-44.9-18.08a16.11 16.11 0 00-15.17 1.75A164.48 164.48 0 01325 400.8a15.94 15.94 0 00-8.82 12.14l-6.73 47.89a11.08 11.08 0 01-10.68 9.17h-85.54a11.11 11.11 0 01-10.69-8.87l-6.72-47.82a16.07 16.07 0 00-9-12.22 155.3 155.3 0 01-21.46-12.57 16 16 0 00-15.11-1.71l-44.89 18.07a10.81 10.81 0 01-13.14-4.58l-42.77-74a10.8 10.8 0 012.45-13.75l38.21-30a16.05 16.05 0 006-14.08c-.36-4.17-.58-8.33-.58-12.5s.21-8.27.58-12.35a16 16 0 00-6.07-13.94l-38.19-30A10.81 10.81 0 0149.48 186l42.77-74a10.81 10.81 0 0113.14-4.59l44.9 18.08a16.11 16.11 0 0015.17-1.75A164.48 164.48 0 01187 111.2a15.94 15.94 0 008.82-12.14l6.73-47.89A11.08 11.08 0 01213.23 42h85.54a11.11 11.11 0 0110.69 8.87l6.72 47.82a16.07 16.07 0 009 12.22 155.3 155.3 0 0121.46 12.57 16 16 0 0015.11 1.71l44.89-18.07a10.81 10.81 0 0113.14 4.58l42.77 74a10.8 10.8 0 01-2.45 13.75l-38.21 30a16.05 16.05 0 00-6.05 14.08c.33 4.14.55 8.3.55 12.47z"
-            fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="32" />
-        </svg> -->Admin
-      </div>
-      <div
-        id="account-identifier"
-        class="w-44 xxl:w-48 bg-white absolute z-10 right-0 mt-2 rounded-xl p-2 xl:p-3 shadow-[0_10px_20px_rgb(0,0,0,0.03)]"
-        style="display: none"
-      >
-        <div class="flex flex-col gap-1 w-full text-center">
-          <a href="{{ '/admin/account' }}">
-            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg">
-              <h4 class="text-blacktwo font-semibold">Account</h4>
-            </div>
-          </a>
-          <a href="">
-            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg">
-              <h4 class="text-blacktwo font-semibold">Dark</h4>
-            </div>
-          </a>
-          <a href="">
-            <div class="hover:bg-shadegray py-2 xxl:py-3 rounded-lg">
-              <h4 class="text-blacktwo font-semibold">Logout</h4>
-            </div>
-          </a>
-        </div>
-      </div>
-      <!-- account settings -->
+      <div class="w-full flex flex-col">
+        <a href="{{ '/admin' }}">
+          <div
+            class="flex items-center gap-5 {% if active == 'dashboard' %} bg-shadeblue stroke-primary text-primary {%else%} stroke-blacktwo text-blacktwo {%endif%} px-4 xxl:px-6 py-3 xxl:py-4 rounded-lg cursor-pointer"
+          >
+            <span>
+              <svg
+                xmlns="http://www.w3.org/2000/svg"
+                class="w-6 h-6"
+                viewBox="0 0 512 512"
+              >
+                <rect
+                  x="48"
+                  y="48"
+                  width="176"
+                  height="176"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <rect
+                  x="288"
+                  y="48"
+                  width="176"
+                  height="176"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <rect
+                  x="48"
+                  y="288"
+                  width="176"
+                  height="176"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <rect
+                  x="288"
+                  y="288"
+                  width="176"
+                  height="176"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+              </svg>
+            </span>
+            <h2 class="font-semibold tracking-widest">Dashboard</h2>
+          </div>
+        </a>
+        <!--<a href="{{ '/admin/visualization' }}">
+          <div
+            class="flex items-center gap-5 {% if active == 'visualization' %} bg-shadeblue stroke-primary text-primary {%else%} stroke-blacktwo text-blacktwo {%endif%} px-4 xxl:px-6 py-3 xxl:py-4 rounded-lg cursor-pointer"
+          >
+            <span>
+              <svg
+                xmlns="http://www.w3.org/2000/svg"
+                class="w-6 h-6"
+                viewBox="0 0 512 512"
+              >
+                <rect
+                  x="96"
+                  y="224"
+                  width="80"
+                  height="192"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <rect
+                  x="240"
+                  y="176"
+                  width="80"
+                  height="240"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <rect
+                  x="383.64"
+                  y="112"
+                  width="80"
+                  height="304"
+                  rx="20"
+                  ry="20"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+              </svg>
+            </span>
+            <h2 class="font-semibold tracking-widest">Visualization</h2>
+          </div>
+        </a>
+      -->
+        <a href="{{ '/admin/history?page=1' }}">
+          <div
+            class="flex items-center gap-5 {% if active == 'history' %} bg-shadeblue stroke-primary text-primary {%else%} stroke-blacktwo text-blacktwo {%endif%} px-4 xxl:px-6 py-3 xxl:py-4 rounded-lg cursor-pointer"
+          >
+            <span>
+              <svg
+                xmlns="http://www.w3.org/2000/svg"
+                class="w-6 h-6"
+                viewBox="0 0 512 512"
+              >
+                <rect
+                  x="96"
+                  y="48"
+                  width="320"
+                  height="416"
+                  rx="48"
+                  ry="48"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <path
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                  d="M176 128h160M176 208h160M176 288h80"
+                />
+              </svg>
+            </span>
+            <h2 class="font-semibold tracking-widest">History</h2>
+          </div>
+        </a>
 
-      <!-- account settings ends -->
+       <hr class="border-shadeblack/30 my-2" />
+       {%for group in sidebar_groups%} {%if group_name and group_item%}
+        <a href="{{ '/admin/%s/%s' % (group_name, group) }}">
+          <div
+            class="flex items-center gap-5 stroke-blacktwo text-blacktwo px-4 xxl:px-6 py-3 xxl:py-4 rounded-lg cursor-pointer"
+          >
+            <span>
+              <svg
+                xmlns="http://www.w3.org/2000/svg"
+                class="w-6 h-6"
+                viewBox="0 0 512 512"
+              >
+                <path
+                  d="M64 192v-72a40 40 0 0140-40h75.89a40 40 0 0122.19 6.72l27.84 18.56a40 40 0 0022.19 6.72H408a40 40 0 0140 40v40"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <path
+                  d="M479.9 226.55L463.68 392a40 40 0 01-39.93 40H88.25a40 40 0 01-39.93-40L32.1 226.55A32 32 0 0164 192h384.1a32 32 0 0131.8 34.55z"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+              </svg>
+            </span>
+            <h2 class="font-semibold tracking-widest">{{group}}</h2>
+          </div>
+        </a>
+        {%else%}
+        <a href="{{ '%s' % group }}">
+          <div
+            class="flex items-center gap-5 stroke-blacktwo text-blacktwo px-4 xxl:px-6 py-3 xxl:py-4 rounded-lg cursor-pointer"
+          >
+            <span>
+              <svg
+                xmlns="http://www.w3.org/2000/svg"
+                class="w-6 h-6"
+                viewBox="0 0 512 512"
+              >
+                <path
+                  d="M64 192v-72a40 40 0 0140-40h75.89a40 40 0 0122.19 6.72l27.84 18.56a40 40 0 0022.19 6.72H408a40 40 0 0140 40v40"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+                <path
+                  d="M479.9 226.55L463.68 392a40 40 0 01-39.93 40H88.25a40 40 0 01-39.93-40L32.1 226.55A32 32 0 0164 192h384.1a32 32 0 0131.8 34.55z"
+                  fill="none"
+                  stroke="currentColor"
+                  stroke-linecap="round"
+                  stroke-linejoin="round"
+                  stroke-width="30"
+                />
+              </svg>
+            </span>
+            <h2 class="font-semibold tracking-widest">{{group}}</h2>
+          </div>
+        </a>
+        {%endif%} {%endfor%}
+      </div>
     </div>
-  </div>
-</div>
-<!-- nav ends -->
-
-<div class="sm:hidden relative w-full">
-  <input
-    type="search"
-    name="search"
-    id=""
-    placeholder="Search"
-    autocomplete="off"
-    class="w-full h-12 px-4 pl-10 tracking-wider font-medium text-shadeblack bg-white rounded-lg outline-none focus:ring-1 focus:ring-primary/70 duration-300"
-  />
-  <span
-    class="absolute inset-y-0 left-2 flex justify-center items-center cursor-pointer"
-  >
-    <svg
-      xmlns="http://www.w3.org/2000/svg"
-      class="w-6 h-6 stroke-shadeblack"
-      viewBox="0 0 512 512"
-    >
-      <path
-        d="M221.09 64a157.09 157.09 0 10157.09 157.09A157.1 157.1 0 00221.09 64z"
-        fill="none"
-        stroke-miterlimit="10"
-        stroke-width="30"
-      />
-      <path
-        fill="none"
-        stroke-linecap="round"
-        stroke-miterlimit="10"
-        stroke-width="30"
-        d="M338.29 338.29L448 448"
-      />
-    </svg>
-  </span>
-  <div
-    class="hidden w-full absolute bg-white mt-2 h-72 p-3 rounded-xl shadow-xl"
-  >
-    <div class="w-full h-full overflow-auto flex flex-col gap-2">
-      <a href="">
-        <div class="w-full p-2 bg-shadegray rounded-lg">
-          <h3 class="font-semibold text-blacktwo">Search result</h3>
-          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-        </div>
-      </a>
-      <a href="">
-        <div class="w-full p-2 bg-shadegray rounded-lg">
-          <h3 class="font-semibold text-blacktwo">Search result</h3>
-          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-        </div>
-      </a>
-      <a href="">
-        <div class="w-full p-2 bg-shadegray rounded-lg">
-          <h3 class="font-semibold text-blacktwo">Search result</h3>
-          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-        </div>
-      </a>
-      <a href="">
-        <div class="w-full p-2 bg-shadegray rounded-lg">
-          <h3 class="font-semibold text-blacktwo">Search result</h3>
-          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-        </div>
-      </a>
-      <a href="">
-        <div class="w-full p-2 bg-shadegray rounded-lg">
-          <h3 class="font-semibold text-blacktwo">Search result</h3>
-          <h6 class="text-sm text-shadeblacks">Tag or whatever</h6>
-        </div>
-      </a>
+    <div class="text-center">
+      <h6 id="current-year" class="text-shadeblack font-medium"></h6>
     </div>
   </div>
-</div>
-<!-- mobile search -->
+</main>
+
+<script>
+  // Get the current year
+  const currentYear = new Date().getFullYear();
+
+  // Update the content of the <h6> element with the current year
+  const currentYearElement = document.getElementById('current-year');
+  currentYearElement.innerHTML = `© ${currentYear} <b>GreatAPI</b>`;
+</script>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,27 +1,16 @@
 
-[Unknown INPUT type]
 
-__
-Admin
-***_Account_***
+*****_Dashboard_*****
 
-*** Dark ***
 
-*** Logout ***
+*****_History_*****
 
-[Unknown INPUT type]
-**** Search result ****
-* Tag or whatever *
+===============================================================================
+{%for group in sidebar_groups%} {%if group_name and group_item%}
 
-**** Search result ****
-* Tag or whatever *
+*****_{{group}}_*****
+ {%else%}
 
-**** Search result ****
-* Tag or whatever *
-
-**** Search result ****
-* Tag or whatever *
-
-**** Search result ****
-* Tag or whatever *
+*****_{{group}}_*****
+ {%endif%} {%endfor%}
```

### Comparing `greatapi-0.0.5/greatapi/core/auth/jwt_token.py` & `greatapi-0.0.6/greatapi/core/auth/jwt_token.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/core/auth/sites.py` & `greatapi-0.0.6/greatapi/core/auth/sites.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import status
 from fastapi.security import OAuth2PasswordRequestForm
 
 from greatapi.core.auth.hashing import Hash
 from greatapi.core.auth.jwt_token import create_access_token
+from greatapi.db.admin.user import User
 from greatapi.db.database import SessionLocal
-from greatapi.db.models.user import User
 from greatapi.utils.cbv import cbv
 from greatapi.utils.inferring_router import InferringRouter
 
 
 auth_router = InferringRouter(tags=['Authentication'])
 
 
@@ -38,7 +38,33 @@
                 detail='Incorrect Password',
             )
 
         # Generate a JWT token and return
         access_token = create_access_token(data={'sub': user.email})
 
         return {'access_token': access_token, 'token_type': 'bearer'}
+
+    @auth_router.post('/admin_login')
+    def admin_login(self, request: OAuth2PasswordRequestForm = Depends()) -> dict[str, Any]:
+        user = self.db.query(User).filter(User.email == request.username).first()
+        plain_password = request.password
+        if not user:
+            raise HTTPException(
+                status_code=status.HTTP_404_NOT_FOUND,
+                detail='Invalid Credentials',
+            )
+
+        if not Hash.verify(user.password, plain_password):
+            raise HTTPException(
+                status_code=status.HTTP_404_NOT_FOUND,
+                detail='Incorrect Password',
+            )
+
+        if not user.is_admin:  # Check if the user is an admin
+            raise HTTPException(
+                status_code=status.HTTP_403_FORBIDDEN,
+                detail='Access denied. Only admin users are allowed to login.',
+            )
+        # Generate a JWT token and return
+        access_token = create_access_token(data={'sub': user.email})
+
+        return {'access_token': access_token, 'token_type': 'bearer'}
```

### Comparing `greatapi-0.0.5/greatapi/core/history/sites.py` & `greatapi-0.0.6/greatapi/core/history/sites.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,78 @@
 from __future__ import annotations
 
 from typing import List
+from typing import Optional
 
 from fastapi import Depends
 from fastapi import HTTPException
+from fastapi import Query
 from fastapi import status
 from sqlalchemy.orm import Session
 
+from greatapi.core.history.repository import create_history
+from greatapi.core.history.repository import fetch_filtered_paginated_results
+from greatapi.core.history.schemas import CategoryEnum
+from greatapi.core.history.schemas import HistoryCreateSchema
 from greatapi.core.history.schemas import HistorySchema
 from greatapi.db.database import get_db
 from greatapi.db.database import SessionLocal
-from greatapi.db.models.default import History
 from greatapi.utils.cbv import cbv
 from greatapi.utils.inferring_router import InferringRouter
 
 history_router = InferringRouter(tags=['History'])
 
 
 @cbv(history_router)
 class HistorySite:
     db = SessionLocal()
 
     @history_router.get('/get_all_history', response_model=List[HistorySchema], status_code=200)
-    def get_all_history(self, db: Session = Depends(get_db)) -> list[HistorySchema]:
-        items = db.query(History).all()
-        return items
+    def get_all_history(
+        self,
+        page: int = Query(1, ge=1),
+        size: int = Query(10, ge=1, le=100),
+        db: Session = Depends(get_db),
+    ) -> List[HistorySchema]:
+        try:
+            paginated_results = fetch_filtered_paginated_results(page=page, size=size)
+            return paginated_results
+
+        except Exception as e:
+            # Return an error response if something goes wrong
+            raise HTTPException(
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e),
+            )
+        finally:
+            db.close()
 
     @history_router.post('/create_history', response_model=HistorySchema, status_code=status.HTTP_201_CREATED)
-    def create_an_item(self, item: HistorySchema) -> HistorySchema:
-        history_item = self.db.query(History).filter(History.name == item.name).first()
-
-        if history_item is not None:
-            raise HTTPException(status_code=400, detail='History item already exists')
-
-        new_history_item = History(
-            name=item.name,
-            category=item.category,
+    def create_an_item(self, item: HistoryCreateSchema) -> Optional[HistorySchema]:
+        new_history = create_history(
+            name=item.name, category=item.category, response=True,
         )
+        return new_history
 
-        self.db.add(new_history_item)
-        self.db.commit()
-
-        return new_history_item
+    # API endpoint to search history items with date filters
+    @history_router.get('/history/search/', response_model=List[HistorySchema], status_code=status.HTTP_200_OK)
+    def search_history(
+        self,
+        page: int = Query(1, ge=1),
+        size: int = Query(10, ge=1, le=100),
+        db: Session = Depends(get_db),
+        name: Optional[str] = Query(None, max_length=100),
+        category: Optional[CategoryEnum] = Query(None),
+        date_filter: Optional[str] = Query(None, max_length=50),
+    ) -> List[HistorySchema]:
+        try:
+            search_result = fetch_filtered_paginated_results(
+                page=page, size=size, name=name, category=category, date_filter=date_filter,
+            )
+            return search_result
+
+        except Exception as e:
+            # Return an error response if something goes wrong
+            raise HTTPException(
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e),
+            )
+        finally:
+            db.close()
```

### Comparing `greatapi-0.0.5/greatapi/core/test_auth/sites.py` & `greatapi-0.0.6/greatapi/core/test_auth/sites.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List
 from typing import Tuple
 
 from fastapi import Depends
 
 from greatapi.core.auth.jwt_token import get_current_user
 from greatapi.core.users.query import get_user_by_id
+from greatapi.db.admin.user import User
 from greatapi.db.database import SessionLocal
-from greatapi.db.models.user import User
 from greatapi.utils.cbv import cbv
 from greatapi.utils.inferring_router import InferringRouter
 
 test_auth_router = InferringRouter(tags=['Test Authentication'])
 
 
 @cbv(test_auth_router)
```

### Comparing `greatapi-0.0.5/greatapi/core/users/query.py` & `greatapi-0.0.6/greatapi/core/users/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fastapi import HTTPException
 from fastapi import status
 from sqlalchemy.orm import Session
 
 from greatapi.core.auth.hashing import Hash
 from greatapi.core.users.schemas import ShowUserSchema
 from greatapi.core.users.schemas import UserSchema
-from greatapi.db.models.user import User
+from greatapi.db.admin.user import User
 
 
 def create_new_user(request: UserSchema, db: Session) -> UserSchema:
     new_user = User(
         name=request.name,
         email=request.email,
         password=Hash.bcrypt(request.password),
```

### Comparing `greatapi-0.0.5/greatapi/core/users/sites.py` & `greatapi-0.0.6/greatapi/core/users/sites.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/db/database.py` & `greatapi-0.0.6/greatapi/db/database.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/utils/cbv.py` & `greatapi-0.0.6/greatapi/utils/cbv.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import TypeVar
 
 from fastapi import APIRouter
 from fastapi import Depends
 from starlette.routing import Route
 from starlette.routing import WebSocketRoute
 
+from greatapi.db.admin.user import User
 from greatapi.db.database import Base
-from greatapi.db.models.user import User
 # from typing import get_type_hints
 # from pydantic.typing import is_classvar
 
 T = TypeVar('T')
 
 CBV_CLASS_KEY = '__cbv_class__'
 DEFAULT_ADMIN_SETTINGS = {'user': {'users': User}}
```

### Comparing `greatapi-0.0.5/greatapi/utils/component.py` & `greatapi-0.0.6/greatapi/utils/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,86 @@
 from __future__ import annotations
 
 from typing import Any
+from typing import Optional
 
+from sqlalchemy import cast
 from sqlalchemy import func
+from sqlalchemy import inspect
+from sqlalchemy import or_
 from sqlalchemy import select
+from sqlalchemy import String
 from sqlalchemy.orm import Session
 
 from greatapi.core.history.schemas import HistorySchema
+from greatapi.db.admin.default import History
+from greatapi.db.admin.user import User
 from greatapi.db.database import Base
 from greatapi.db.database import engine
-from greatapi.db.models.default import History
 # from greatapi.utils.helpers import get_models_count
 
 
-def fetch_table_data(TABLE_CLASS: Base) -> tuple[list[str], list[dict[str, Any]]]:
+def fetch_table_data(TABLE_CLASS: Base, page: int = 1, name: Optional[str] = None) -> tuple[list[str], list[dict[str, Any]]]:
     query = select(TABLE_CLASS)
+
+    if name is not None and name != 'all_history':
+        # Get all columns in the TABLE_CLASS
+        columns = [
+            getattr(TABLE_CLASS, c_attr.key)
+            for c_attr in inspect(TABLE_CLASS).attrs
+        ]
+
+        # Create a list of filter conditions for each column containing the 'name' value
+        filter_conditions = [
+            cast(column, String).ilike(f'%{name}%') for column in columns
+        ]
+
+        # Combine the filter conditions using the 'or_' operator
+        query = query.filter(or_(*filter_conditions))
+
+    # Add DISTINCT clause to the query to eliminate duplicate rows
+    query = query.distinct()
+
+    # Calculate the offset and limit for pagination
+    PAGE_SIZE = 10
+    offset = (page - 1) * PAGE_SIZE
+    query = query.offset(offset).limit(PAGE_SIZE)
+
     result = engine.execute(query)
-    return (result._metadata.keys, result.fetchall())
+
+    # Extract specific attributes from the query result and convert them into a list of dictionaries
+    keys = result._metadata.keys
+    items = [(row) for row in result]
+
+    return (keys, items)
 
 
 def get_models_count(TABLE_CLASS: Base) -> int:
     query = select([func.count()]).select_from(TABLE_CLASS)
     result = engine.execute(query).scalar()
     return result
 
 
 def fetch_app_list(admin_settings: dict[str, dict[str, Any]]) -> list[str]:
     return [key.capitalize() for key in admin_settings.keys()]
 
 
 def fetch_app_list_with_count(admin_settings: dict[str, dict[str, Any]]) -> list[dict[str, Any]]:
-    return [{'name': key.capitalize(), 'total_count': len(values)} for key, values in admin_settings.items()]
+    return [{'name': key.capitalize(), 'total_count': len(values)} for key, values in admin_settings.items() if key != 'default']
 
 
 def fetch_models_by_app(admin_settings: dict[str, dict[str, Any]], app_name: str) -> list[str]:
     return [key for key in admin_settings[app_name].keys()]
 
 
 def fetch_models_by_app_with_count(admin_settings: dict[str, dict[str, Any]], app_name: str) -> list[dict[str, Any]]:
     return [{'name': key.capitalize(), 'total_count': get_models_count(values)} for key, values in admin_settings[app_name].items()]
 
 
 def query_history_table(db: Session, limit: int = 3) -> list[HistorySchema]:
     history = db.query(History).order_by(History.created_date.desc()).limit(limit).all()
     return history
+
+
+def get_user_by_email(email: str, db: Session) -> User:
+    user = db.query(User).filter(User.email == email).first()
+    return user
```

### Comparing `greatapi-0.0.5/greatapi/utils/inferring_router.py` & `greatapi-0.0.6/greatapi/utils/inferring_router.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/utils/management.py` & `greatapi-0.0.6/greatapi/utils/management.py`

 * *Files identical despite different names*

### Comparing `greatapi-0.0.5/greatapi/utils/urls.py` & `greatapi-0.0.6/greatapi/utils/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 
 # TODO: Substitute Any with AdminSite class type
 
 
 def get_route_app(class_name: Any) -> str:
     module_path = inspect.getmodule(class_name).__name__  # type: ignore
     split_by_dot = module_path.split('.')
-    if split_by_dot[-1] == 'admin':
-        return split_by_dot[-2]
-    else:
-        return split_by_dot[-1]
+    return split_by_dot[-2]
 
 
 def get_route_dict(REGISTERED_ADMINS: list[Any]) -> dict[str, dict[str, Base]]:
     registered_admins: dict[str, dict[str, Base]] = {}
 
     for admin_class in REGISTERED_ADMINS:
         app_name = get_route_app(admin_class)
```

### Comparing `greatapi-0.0.5/greatapi.egg-info/SOURCES.txt` & `greatapi-0.0.6/greatapi.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 greatapi/__init__.py
 greatapi/config.py
-greatapi/multiplication.py
 greatapi.egg-info/PKG-INFO
 greatapi.egg-info/SOURCES.txt
 greatapi.egg-info/dependency_links.txt
 greatapi.egg-info/entry_points.txt
 greatapi.egg-info/requires.txt
 greatapi.egg-info/top_level.txt
 greatapi/admin/__init__.py
 greatapi/admin/sites.py
 greatapi/admin/static/__init__.py
+greatapi/admin/static/favicon.ico
 greatapi/admin/static/greatapi_readme.svg
 greatapi/admin/static/logo.svg
 greatapi/admin/static/main.js
 greatapi/admin/static/styles.css
 greatapi/admin/templates/__init__.py
 greatapi/admin/templates/base.html
 greatapi/admin/templates/navbar.html
@@ -31,21 +31,21 @@
 greatapi/admin/templates/dashboard/group.html
 greatapi/admin/templates/dashboard/history.html
 greatapi/admin/templates/dashboard/index.html
 greatapi/admin/templates/dashboard/items.html
 greatapi/admin/templates/dashboard/settings.html
 greatapi/admin/templates/dashboard/visualization.html
 greatapi/commands/__init__.py
+greatapi/commands/createsuperuser.py
 greatapi/commands/runserver.py
 greatapi/commands/startapp.py
 greatapi/commands/startproject.py
 greatapi/conf/__init__.py
 greatapi/conf/app_template/__init__.py
 greatapi/conf/app_template/__init__.py-tpl
-greatapi/conf/app_template/admin.py-tpl
 greatapi/conf/app_template/models.py-tpl
 greatapi/conf/app_template/repository.py-tpl
 greatapi/conf/app_template/router.py-tpl
 greatapi/conf/app_template/schemas.py-tpl
 greatapi/conf/project_template/__init__.py
 greatapi/conf/project_template/main.py-tpl
 greatapi/conf/project_template/project_name/__init__.py
@@ -65,16 +65,16 @@
 greatapi/core/test_auth/sites.py
 greatapi/core/users/__init__.py
 greatapi/core/users/query.py
 greatapi/core/users/schemas.py
 greatapi/core/users/sites.py
 greatapi/db/__init__.py
 greatapi/db/database.py
-greatapi/db/models/__init__.py
-greatapi/db/models/default.py
-greatapi/db/models/user.py
+greatapi/db/admin/__init__.py
+greatapi/db/admin/default.py
+greatapi/db/admin/user.py
 greatapi/utils/__init__.py
 greatapi/utils/cbv.py
 greatapi/utils/component.py
 greatapi/utils/inferring_router.py
 greatapi/utils/management.py
 greatapi/utils/urls.py
```

### Comparing `greatapi-0.0.5/setup.cfg` & `greatapi-0.0.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = greatapi
-version = 0.0.5
+version = 0.0.6
 description = GreatAPI framework, Full stack FastAPI framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sahajrajmalla/greatapi
 author = Sahaj Raj Malla
 author_email = mallasahajraj@gmail.com
 license = MIT
@@ -34,15 +34,14 @@
 	Typing :: Typed
 
 [options]
 packages = find:
 install_requires = 
 	fastapi>=0.78.0,<0.79.0
 	jinja2>=2.11.2,<4.0.0
-	numpy>=1.18.1,<2.0.0
 	passlib[bcrypt]>=1.7.2,<2.0.0
 	pre-commit>=2.17.0,<3.0.0
 	python-jose[cryptography]>=3.3.0,<4.0.0
 	python-multipart>=0.0.5,<0.0.6
 	sqlalchemy>=1.3.18,<1.5.0
 	typer>=0.4.1,<0.5.0
 	uvicorn[standard]>=0.12.0,<0.18.0
@@ -62,14 +61,15 @@
 	pytest
 
 [options.package_data]
 greatapi.admin.static = 
 	*.css
 	*.js
 	*.svg
+	*.ico
 greatapi.admin.templates = 
 	*.html
 greatapi.admin.templates.authentication = 
 	*.html
 greatapi.admin.templates.dashboard = 
 	*.html
 greatapi.conf.app_template =
```

