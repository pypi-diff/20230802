# Comparing `tmp/odcs-0.6.0.tar.gz` & `tmp/odcs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odcs-0.6.0.tar", last modified: Fri May 19 17:05:05 2023, max compression
+gzip compressed data, was "odcs-0.7.0.tar", last modified: Wed Aug  2 09:19:34 2023, max compression
```

## Comparing `odcs-0.6.0.tar` & `odcs-0.7.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/contrib/
--rwxrwxr-x   0 hlin      (1000) hlin      (1000)    17671 2023-05-19 17:04:03.000000 odcs-0.6.0/client/contrib/odcs
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/odcs/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/odcs/client/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      155 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/client/__init__.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    25947 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/client/odcs.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/__init__.py
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/tests/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    23924 2023-05-19 17:04:03.000000 odcs-0.6.0/client/tests/test_client_odcs.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       40 2023-05-19 17:04:03.000000 odcs-0.6.0/client/requirements.txt
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/odcs/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/odcs/common/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/common/__init__.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3957 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/common/types.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/__init__.py
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/docs/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1608 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/about.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    14670 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/api.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3031 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/client.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      641 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/index.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      125 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/module.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2429 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/pulp.rst
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     8447 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/raw_config.rst
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    23029 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/PKG-INFO
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     5496 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/SOURCES.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)        1 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/dependency_links.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      254 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/entry_points.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)        1 2023-05-19 17:04:53.000000 odcs-0.6.0/odcs.egg-info/not-zip-safe
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      686 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/requires.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)        5 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/top_level.txt
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/conf/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       96 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/__init__.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     8515 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/config.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      258 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/odcs-httpd-krb.conf
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      632 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/odcs-httpd-openidc.conf
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3586 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/pungi.conf
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      277 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/raw_config_urls.conf
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       77 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/raw_config_wrapper.conf
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/contrib/
--rwxrwxr-x   0 hlin      (1000) hlin      (1000)    12884 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs-promote-compose
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      140 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs.wsgi
--rwxrwxr-x   0 hlin      (1000) hlin      (1000)    13660 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs_test_deployment
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/migrations/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/migrations/versions/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      661 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      776 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      461 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/11b350234051_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      917 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      711 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      420 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/4514febd31fa_add_builds.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      648 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1440 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/566733ac3811_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      872 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      480 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/7b143656694f_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      431 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/812f2745248f_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      466 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/82172e6a3154_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      639 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      437 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/a8e259e0208c_add_compose_state_reason.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      430 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b00f3b6efaed_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      445 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b2725d046624_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      421 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b75ad2afc207_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      423 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/c1b7e84ff39b_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      684 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      471 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/ca08065687c4_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      724 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      648 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/d1da07e15c54_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      818 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/de0a86d7de49_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      651 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/e186faabdafe_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      617 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/e2163db7b15d_.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      691 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      633 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       38 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/README
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      770 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/alembic.ini
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2807 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/env.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      412 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/script.py.mako
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/static/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/static/.gitkeep
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/templates/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      535 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/templates/apidoc.html
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1974 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/templates/index.html
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3297 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/__init__.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    14727 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/api_utils.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    10896 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/auth.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    45652 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/backend.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     8931 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/cache.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    13768 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/celery_tasks.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     4706 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/comps.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    21878 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/config.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1323 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/errors.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2722 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/events.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3074 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/logger.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     4593 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/manage.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12485 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mbs.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     7706 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mergerepo.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2794 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/messaging.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12080 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/metrics.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    13271 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mock_runroot.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    20949 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/models.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12560 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/openapi.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2329 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/proxy.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12737 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pulp.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    27479 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pungi.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3875 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pungi_compose.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     6042 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/utils.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    37813 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/views.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/__init__.py
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/data/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      226 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/data/custom_raw_config_wrapper.conf
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/repo/
-drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/repo/repodata/
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     4133 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      750 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1015 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2722 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      827 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2263 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     1884 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3533 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/repomd.xml
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    88568 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    80326 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    81258 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     6878 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     6970 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2808 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/Jenkinsfile
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       78 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/__init__.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     7971 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/mbs.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    18340 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_auth.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    60116 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_backend.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     8244 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_cache.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12694 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_celery_tasks.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     5411 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_events.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     5362 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_metrics.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     8849 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_mock_runroot.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12806 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_models.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    11052 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pulp.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    38575 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pungi.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     4667 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pungi_compose.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    12008 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_remove_expired_composes_thread.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     2985 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_utils.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    86954 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_views.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     4108 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/utils.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      477 2023-05-19 17:04:03.000000 odcs-0.6.0/server/requirements.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)      253 2023-05-19 17:04:03.000000 odcs-0.6.0/MANIFEST.in
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    19349 2023-05-19 17:04:03.000000 odcs-0.6.0/README.md
--rw-rw-r--   0 hlin      (1000) hlin      (1000)     3226 2023-05-19 17:04:03.000000 odcs-0.6.0/setup.py
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       47 2023-05-19 17:04:03.000000 odcs-0.6.0/test-requirements.txt
--rw-rw-r--   0 hlin      (1000) hlin      (1000)    23029 2023-05-19 17:05:05.000000 odcs-0.6.0/PKG-INFO
--rw-rw-r--   0 hlin      (1000) hlin      (1000)       38 2023-05-19 17:05:05.000000 odcs-0.6.0/setup.cfg
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.182247 odcs-0.7.0/
+-rw-r--r--   0 hlin       (501) wheel        (0)      253 2023-08-02 09:18:48.000000 odcs-0.7.0/MANIFEST.in
+-rw-r--r--   0 hlin       (501) wheel        (0)    23029 2023-08-02 09:19:34.181953 odcs-0.7.0/PKG-INFO
+-rw-r--r--   0 hlin       (501) wheel        (0)    19349 2023-08-02 09:18:48.000000 odcs-0.7.0/README.md
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.142682 odcs-0.7.0/client/
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.142948 odcs-0.7.0/client/contrib/
+-rwxr-xr-x   0 hlin       (501) wheel        (0)    17681 2023-08-02 09:18:48.000000 odcs-0.7.0/client/contrib/odcs
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.143296 odcs-0.7.0/client/odcs/
+-rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-08-02 09:18:48.000000 odcs-0.7.0/client/odcs/__init__.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.143850 odcs-0.7.0/client/odcs/client/
+-rw-r--r--   0 hlin       (501) wheel        (0)      155 2023-08-02 09:18:48.000000 odcs-0.7.0/client/odcs/client/__init__.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    25947 2023-08-02 09:18:48.000000 odcs-0.7.0/client/odcs/client/odcs.py
+-rw-r--r--   0 hlin       (501) wheel        (0)       40 2023-08-02 09:18:48.000000 odcs-0.7.0/client/requirements.txt
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.144220 odcs-0.7.0/client/tests/
+-rw-r--r--   0 hlin       (501) wheel        (0)    23924 2023-08-02 09:18:48.000000 odcs-0.7.0/client/tests/test_client_odcs.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.136719 odcs-0.7.0/common/
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.144544 odcs-0.7.0/common/odcs/
+-rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-08-02 09:18:48.000000 odcs-0.7.0/common/odcs/__init__.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.145036 odcs-0.7.0/common/odcs/common/
+-rw-r--r--   0 hlin       (501) wheel        (0)        0 2023-08-02 09:18:48.000000 odcs-0.7.0/common/odcs/common/__init__.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     3957 2023-08-02 09:18:48.000000 odcs-0.7.0/common/odcs/common/types.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.146833 odcs-0.7.0/docs/
+-rw-r--r--   0 hlin       (501) wheel        (0)     1608 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/about.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)    14670 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/api.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)     3031 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/client.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)      641 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/index.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)      125 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/module.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)     2429 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/pulp.rst
+-rw-r--r--   0 hlin       (501) wheel        (0)     9311 2023-08-02 09:18:48.000000 odcs-0.7.0/docs/raw_config.rst
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.149035 odcs-0.7.0/odcs.egg-info/
+-rw-r--r--   0 hlin       (501) wheel        (0)    23029 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/PKG-INFO
+-rw-r--r--   0 hlin       (501) wheel        (0)     5536 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/SOURCES.txt
+-rw-r--r--   0 hlin       (501) wheel        (0)        1 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/dependency_links.txt
+-rw-r--r--   0 hlin       (501) wheel        (0)      323 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/entry_points.txt
+-rw-r--r--   0 hlin       (501) wheel        (0)        1 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/not-zip-safe
+-rw-r--r--   0 hlin       (501) wheel        (0)      686 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/requires.txt
+-rw-r--r--   0 hlin       (501) wheel        (0)        5 2023-08-02 09:19:34.000000 odcs-0.7.0/odcs.egg-info/top_level.txt
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.149283 odcs-0.7.0/server/
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.151203 odcs-0.7.0/server/conf/
+-rw-r--r--   0 hlin       (501) wheel        (0)       96 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/__init__.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     8397 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/config.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      258 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/odcs-httpd-krb.conf
+-rw-r--r--   0 hlin       (501) wheel        (0)      632 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/odcs-httpd-openidc.conf
+-rw-r--r--   0 hlin       (501) wheel        (0)     3586 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/pungi.conf
+-rw-r--r--   0 hlin       (501) wheel        (0)      469 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/raw_config_urls.conf
+-rw-r--r--   0 hlin       (501) wheel        (0)       77 2023-08-02 09:18:48.000000 odcs-0.7.0/server/conf/raw_config_wrapper.conf
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.152157 odcs-0.7.0/server/contrib/
+-rwxr-xr-x   0 hlin       (501) wheel        (0)    12884 2023-08-02 09:18:48.000000 odcs-0.7.0/server/contrib/odcs-promote-compose
+-rw-r--r--   0 hlin       (501) wheel        (0)      140 2023-08-02 09:18:48.000000 odcs-0.7.0/server/contrib/odcs.wsgi
+-rwxr-xr-x   0 hlin       (501) wheel        (0)    13660 2023-08-02 09:18:48.000000 odcs-0.7.0/server/contrib/odcs_test_deployment
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.152437 odcs-0.7.0/server/odcs/
+-rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/__init__.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.160024 odcs-0.7.0/server/odcs/server/
+-rw-r--r--   0 hlin       (501) wheel        (0)     3297 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/__init__.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    14899 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/api_utils.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    10518 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/auth.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    45652 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/backend.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     8931 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/cache.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    13768 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/celery_tasks.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     4706 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/comps.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    23069 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/config.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     1167 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/credential_helper.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     1323 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/errors.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     2722 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/events.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     3074 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/logger.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     4593 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/manage.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12485 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/mbs.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     7706 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/mergerepo.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     2794 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/messaging.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    11207 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/metrics.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.161085 odcs-0.7.0/server/odcs/server/migrations/
+-rw-r--r--   0 hlin       (501) wheel        (0)       38 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/README
+-rw-r--r--   0 hlin       (501) wheel        (0)      770 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/alembic.ini
+-rw-r--r--   0 hlin       (501) wheel        (0)     2807 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/env.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      412 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/script.py.mako
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.168712 odcs-0.7.0/server/odcs/server/migrations/versions/
+-rw-r--r--   0 hlin       (501) wheel        (0)      661 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      776 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      461 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/11b350234051_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      917 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      711 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      420 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/4514febd31fa_add_builds.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      648 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     1440 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/566733ac3811_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      872 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      480 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/7b143656694f_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      431 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/812f2745248f_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      466 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/82172e6a3154_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      639 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      437 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/a8e259e0208c_add_compose_state_reason.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      430 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/b00f3b6efaed_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      445 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/b2725d046624_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      421 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/b75ad2afc207_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      423 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/c1b7e84ff39b_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      684 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      471 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/ca08065687c4_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      724 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      648 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/d1da07e15c54_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      818 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/de0a86d7de49_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      651 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/e186faabdafe_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      617 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/e2163db7b15d_.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      691 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      633 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    13271 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/mock_runroot.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    20949 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/models.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12560 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/openapi.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     2329 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/proxy.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12937 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/pulp.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    28205 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/pungi.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     3875 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/pungi_compose.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.169009 odcs-0.7.0/server/odcs/server/static/
+-rw-r--r--   0 hlin       (501) wheel        (0)        0 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/static/.gitkeep
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.169555 odcs-0.7.0/server/odcs/server/templates/
+-rw-r--r--   0 hlin       (501) wheel        (0)      535 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/templates/apidoc.html
+-rw-r--r--   0 hlin       (501) wheel        (0)     1974 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/templates/index.html
+-rw-r--r--   0 hlin       (501) wheel        (0)     6368 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/utils.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    37813 2023-08-02 09:18:48.000000 odcs-0.7.0/server/odcs/server/views.py
+-rw-r--r--   0 hlin       (501) wheel        (0)      477 2023-08-02 09:18:48.000000 odcs-0.7.0/server/requirements.txt
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.177059 odcs-0.7.0/server/tests/
+-rw-r--r--   0 hlin       (501) wheel        (0)     2808 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/Jenkinsfile
+-rw-r--r--   0 hlin       (501) wheel        (0)       78 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/__init__.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.177378 odcs-0.7.0/server/tests/data/
+-rw-r--r--   0 hlin       (501) wheel        (0)      226 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/data/custom_raw_config_wrapper.conf
+-rw-r--r--   0 hlin       (501) wheel        (0)     7971 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/mbs.py
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.179246 odcs-0.7.0/server/tests/repo/
+-rw-r--r--   0 hlin       (501) wheel        (0)    88568 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm
+-rw-r--r--   0 hlin       (501) wheel        (0)    80326 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm
+-rw-r--r--   0 hlin       (501) wheel        (0)    81258 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm
+-rw-r--r--   0 hlin       (501) wheel        (0)     6878 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm
+-rw-r--r--   0 hlin       (501) wheel        (0)     6970 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm
+drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-08-02 09:19:34.181475 odcs-0.7.0/server/tests/repo/repodata/
+-rw-r--r--   0 hlin       (501) wheel        (0)     4133 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2
+-rw-r--r--   0 hlin       (501) wheel        (0)      750 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz
+-rw-r--r--   0 hlin       (501) wheel        (0)     1015 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz
+-rw-r--r--   0 hlin       (501) wheel        (0)     2722 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2
+-rw-r--r--   0 hlin       (501) wheel        (0)      827 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz
+-rw-r--r--   0 hlin       (501) wheel        (0)     2263 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2
+-rw-r--r--   0 hlin       (501) wheel        (0)     1884 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz
+-rw-r--r--   0 hlin       (501) wheel        (0)     3533 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/repo/repodata/repomd.xml
+-rw-r--r--   0 hlin       (501) wheel        (0)    18310 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_auth.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    60116 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_backend.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     8244 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_cache.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12694 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_celery_tasks.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     5411 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_events.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     5583 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_metrics.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     8849 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_mock_runroot.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12806 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_models.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    11052 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_pulp.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    39006 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_pungi.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     4667 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_pungi_compose.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    12008 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_remove_expired_composes_thread.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     3443 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_utils.py
+-rw-r--r--   0 hlin       (501) wheel        (0)    86954 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/test_views.py
+-rw-r--r--   0 hlin       (501) wheel        (0)     4301 2023-08-02 09:18:48.000000 odcs-0.7.0/server/tests/utils.py
+-rw-r--r--   0 hlin       (501) wheel        (0)       38 2023-08-02 09:19:34.182339 odcs-0.7.0/setup.cfg
+-rw-r--r--   0 hlin       (501) wheel        (0)     3310 2023-08-02 09:18:48.000000 odcs-0.7.0/setup.py
+-rw-r--r--   0 hlin       (501) wheel        (0)       47 2023-08-02 09:18:48.000000 odcs-0.7.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odcs-0.6.0/client/contrib/odcs` & `odcs-0.7.0/client/contrib/odcs`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 create_build_parser = subparsers.add_parser(
     "create-build", help="Create new compose from Koji builds."
 )
 create_build_parser.set_defaults(command="create-build")
 create_build_parser.add_argument(
     "builds", metavar="NVR", nargs="+", help="Koji builds NVRs."
 )
-_add_arguments(create_build_parser, "--sigkey", "--flag", "--target-dir")
+_add_arguments(create_build_parser, "--sigkey", "--flag", "--target-dir", "--arch")
 
 
 wait_parser = subparsers.add_parser("wait", help="wait for a compose to finish")
 wait_parser.set_defaults(command="wait")
 wait_parser.add_argument("compose_id", default=None, help="ODCS compose id")
 wait_parser.add_argument("--watch", action="store_true", help="Watch compose logs")
```

### Comparing `odcs-0.6.0/client/odcs/client/odcs.py` & `odcs-0.7.0/client/odcs/client/odcs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/client/tests/test_client_odcs.py` & `odcs-0.7.0/client/tests/test_client_odcs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/common/odcs/common/types.py` & `odcs-0.7.0/common/odcs/common/types.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/about.rst` & `odcs-0.7.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/api.rst` & `odcs-0.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/client.rst` & `odcs-0.7.0/docs/client.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/index.rst` & `odcs-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/pulp.rst` & `odcs-0.7.0/docs/pulp.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/docs/raw_config.rst` & `odcs-0.7.0/docs/raw_config.rst`

 * *Files 4% similar despite different names*

```diff
@@ -108,22 +108,44 @@
   - ``pungi_timeout`` - [optional] - If set, defines the timeout in seconds in
     which the compose must be finished, otherwise the compose is marked as
     ``failed``.
   - ``raw_config_wrapper`` - [optional] - If set, defines the full path to
     custom ``raw_config_wrapper.conf`` file which is used by this Raw config
     compose.
 
+There's a parallel config option ``raw_config_credentials`` for configuring
+credentials to use with git commands to download the configuration. If Pungi is
+configured to use ``odcs-credential-helper``, these credentials will be
+available to it too. This option should also be a dict with the same name of
+raw config as a key. The values should be another dict.
+
+The key in this nested mapping is a regular expression matching URL of the
+repo, and the values should contain password and optionally username (unless
+it's provided in the url).
+
+Make sure that the regular expressions for URLs do not overlap, since it's
+undefined which one would be used.
+
 For example:
 
 .. sourcecode:: none
 
     RAW_CONFIG_URLS = {
         "releng_fedora": {
             "url": "https://pagure.io/pungi-fedora.git",
-            "config_filename": "fedora.conf"
+            "config_filename": "fedora.conf",
+        }
+    }
+
+    RAW_CONFIG_CREDENTIALS = {
+        "releng_fedora": {
+            "^https://gitlab.com/": {
+                "username": "oauth1",
+                "password": "this-is-secret"
+            }
         }
     }
 
 
 Enabling ``pungi-config-validate``
 -------------------------------------
```

### Comparing `odcs-0.6.0/odcs.egg-info/PKG-INFO` & `odcs-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odcs
-Version: 0.6.0
+Version: 0.7.0
 Summary: On Demand Compose Service
 Home-page: https://pagure.io/odcs/
 Author: The Compose Team
 Author-email: odcs-owner@fedoraproject.org
 License: MIT
 Description: # On Demand Compose Service - ODCS
```

### Comparing `odcs-0.6.0/odcs.egg-info/SOURCES.txt` & `odcs-0.7.0/odcs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 server/odcs/server/api_utils.py
 server/odcs/server/auth.py
 server/odcs/server/backend.py
 server/odcs/server/cache.py
 server/odcs/server/celery_tasks.py
 server/odcs/server/comps.py
 server/odcs/server/config.py
+server/odcs/server/credential_helper.py
 server/odcs/server/errors.py
 server/odcs/server/events.py
 server/odcs/server/logger.py
 server/odcs/server/manage.py
 server/odcs/server/mbs.py
 server/odcs/server/mergerepo.py
 server/odcs/server/messaging.py
```

### Comparing `odcs-0.6.0/odcs.egg-info/requires.txt` & `odcs-0.7.0/odcs.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 openidc-client
 requests
 requests-gssapi
 
 [all]
-openidc-client
-sqlalchemy
-pyOpenSSL
-jinja2
 kobo
-productmd
 Flask-SQLAlchemy
-flufl.lock
-koji
-prometheus_client
-marshmallow
-apispec==5.2.2
 Flask-Login<0.5.0
+psutil
+Flask<=2.0.3,>=0.11
+jinja2
 requests
-defusedxml
 python-ldap
-psutil
+requests-gssapi
+prometheus_client
+productmd
+koji
+defusedxml
 apispec-webframeworks==0.5.2
-Werkzeug<=2.0.3
 Flask-Migrate
-Flask<=2.0.3,>=0.11
+marshmallow
+flufl.lock
+openidc-client
+apispec==5.2.2
+pyOpenSSL
+sqlalchemy
+Werkzeug<=2.0.3
 pygobject
 celery
-requests-gssapi
 
 [client]
 openidc-client
 requests
 requests-gssapi
 
 [server]
```

### Comparing `odcs-0.6.0/server/conf/config.py` & `odcs-0.7.0/server/conf/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,19 +85,14 @@
     AUTH_BACKEND = "noauth"
 
     # Used for Kerberos authentication and to query user's groups.
     # Format: ldap://hostname[:port]
     # For example: ldap://ldap.example.com/
     AUTH_LDAP_SERVER = ""
 
-    # This option is deprecated and will be removed in future release, please use AUTH_LDAP_GROUPS instead.
-    # Group base to query groups from LDAP server.
-    # Generally, it would be, for example, ou=groups,dc=example,dc=com
-    AUTH_LDAP_GROUP_BASE = ""
-
     # List of (base, filter) pairs to query groups from LDAP server.
     # ODCS can query groups from multi base with different filter, for example:
     # AUTH_LDAP_GROUPS = [
     #     ("ou=groups,dc=example,dc=com", "memberUid={}"),
     #     ("ou=adhoc,ou=managedGroups,dc=example,dc=com", "uniqueMember=uid={},ou=users,dc=example,dc=com")
     # ]
     AUTH_LDAP_GROUPS = []
@@ -181,14 +176,16 @@
         PULP_SSL_KEY = environ.get("PULP_SSL_KEY")
     if "PULP_SSL_CERT" in environ:
         PULP_SSL_CERT = environ.get("PULP_SSL_CERT")
     if "TARGET_DIR_URL" in environ:
         TARGET_DIR_URL = environ.get("TARGET_DIR_URL")
     if "RAW_CONFIG_URLS" in environ:
         RAW_CONFIG_URLS = json.loads(environ.get("RAW_CONFIG_URLS"))
+    if "RAW_CONFIG_CREDENTIALS" in environ:
+        RAW_CONFIG_CREDENTIALS = json.loads(environ.get("RAW_CONFIG_CREDENTIALS"))
 
 
 class DevConfiguration(BaseConfiguration):
     DEBUG = True
     LOG_BACKEND = "console"
     LOG_LEVEL = "debug"
 
@@ -233,15 +230,15 @@
         if ex.errno != errno.EEXIST:
             raise RuntimeError(
                 "Can't create compose target dir %s: %s" % (TARGET_DIR, ex.strerror)
             )
 
     AUTH_BACKEND = "noauth"
     AUTH_LDAP_SERVER = "ldap://ldap.example.com"
-    AUTH_LDAP_GROUP_BASE = "ou=groups,dc=example,dc=com"
+    AUTH_LDAP_GROUPS = [("ou=groups,dc=example,dc=com", "memberUid={}")]
 
     MESSAGING_BACKEND = "rhmsg"
     KOJI_PROFILE = "koji"
 
 
 class ProdConfiguration(BaseConfiguration):
     pass
```

### Comparing `odcs-0.6.0/server/conf/odcs-httpd-openidc.conf` & `odcs-0.7.0/server/conf/odcs-httpd-openidc.conf`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/conf/pungi.conf` & `odcs-0.7.0/server/conf/pungi.conf`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/contrib/odcs-promote-compose` & `odcs-0.7.0/server/contrib/odcs-promote-compose`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/contrib/odcs_test_deployment` & `odcs-0.7.0/server/contrib/odcs_test_deployment`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/566733ac3811_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/566733ac3811_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/d1da07e15c54_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/d1da07e15c54_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/de0a86d7de49_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/de0a86d7de49_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/e186faabdafe_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/e186faabdafe_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/e2163db7b15d_.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/e2163db7b15d_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py` & `odcs-0.7.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/alembic.ini` & `odcs-0.7.0/server/odcs/server/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/migrations/env.py` & `odcs-0.7.0/server/odcs/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/templates/apidoc.html` & `odcs-0.7.0/server/odcs/server/templates/apidoc.html`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/templates/index.html` & `odcs-0.7.0/server/odcs/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/__init__.py` & `odcs-0.7.0/server/odcs/server/__init__.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/api_utils.py` & `odcs-0.7.0/server/odcs/server/api_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 # SOFTWARE.
 
 import copy
 import flask
 from flask import request, url_for, Response
 from functools import wraps
 from odcs.server.models import Compose
-from odcs.server import conf
+from odcs.server import conf, log
+from odcs.server.auth import has_role
 from odcs.server.errors import Forbidden
 from odcs.common.types import (
     COMPOSE_RESULTS,
     COMPOSE_FLAGS,
     INVERSE_PUNGI_SOURCE_TYPE_NAMES,
 )
 
@@ -108,14 +109,18 @@
 
     The decision whether the user is allowed or not is done based on
     conf.allowed_clients value.
     """
     if conf.auth_backend == "noauth":
         return
 
+    if has_role("admins"):
+        log.info("Skipping permission check for admin %s", flask.g.user.username)
+        return
+
     errors = set()
     for attrs in _load_allowed_clients_attr(kwargs.keys()):
         found_error = False
         for name, values in kwargs.items():
             if name not in attrs:
                 # This should not happen, but be defensive in this part of code...
                 errors.add(
@@ -136,15 +141,15 @@
                 if values == conf.target_dir:
                     continue
                 inverse_extra_target_dirs = {
                     v: k for k, v in conf.extra_target_dirs.items()
                 }
                 values = inverse_extra_target_dirs[values]
 
-            if type(values) == int:
+            if isinstance(values, int):
                 values = [values]
             elif isinstance(values, str):
                 # `arches` and `sources` are white-space separated lists.
                 values = values.split(" ")
             elif values is None:
                 # If value is not set, it means it is not available for this compose
                 # type and we need to skip its check later. Set the values to empty
```

### Comparing `odcs-0.6.0/server/odcs/server/auth.py` & `odcs-0.7.0/server/odcs/server/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,18 @@
     errors = []
     if not conf.auth_ldap_server:
         errors.append(
             "kerberos authentication enabled with no LDAP server configured, "
             "check AUTH_LDAP_SERVER in your config."
         )
 
-    if not conf.auth_ldap_group_base:
+    if not conf.auth_ldap_groups:
         errors.append(
-            "kerberos authentication enabled with no LDAP group base configured, "
-            "check AUTH_LDAP_GROUP_BASE in your config."
+            "kerberos authentication enabled with no LDAP groups configured, "
+            "check AUTH_LDAP_GROUPS in your config."
         )
 
     if errors:
         for error in errors:
             log.exception(error)
         raise ValueError("Invalid configuration for kerberos authentication.")
 
@@ -135,24 +135,14 @@
     else:
         return load_ssl_user_from_request(request)
 
 
 def query_ldap_groups(uid):
     client = ldap.initialize(conf.auth_ldap_server)
     groups = []
-    if conf.auth_ldap_group_base:
-        log.warning(
-            "conf.auth_ldap_group_base is deprecated, please use AUTH_LDAP_GROUPS instead."
-        )
-        groups = client.search_s(
-            conf.auth_ldap_group_base,
-            ldap.SCOPE_ONELEVEL,
-            attrlist=["cn", "gidNumber"],
-            filterstr="memberUid={0}".format(uid),
-        )
     for ldap_base, ldap_filter in conf.auth_ldap_groups:
         groups.extend(
             client.search_s(
                 ldap_base,
                 ldap.SCOPE_ONELEVEL,
                 attrlist=["cn"],
                 filterstr=ldap_filter.format(uid),
```

### Comparing `odcs-0.6.0/server/odcs/server/backend.py` & `odcs-0.7.0/server/odcs/server/backend.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/cache.py` & `odcs-0.7.0/server/odcs/server/cache.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/celery_tasks.py` & `odcs-0.7.0/server/odcs/server/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/comps.py` & `odcs-0.7.0/server/odcs/server/comps.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/config.py` & `odcs-0.7.0/server/odcs/server/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Written by Jan Kaluza <jkaluza@redhat.com>
 
-import imp
 import os
 import sys
 
+from importlib.machinery import SourceFileLoader
+
 from kobo.conf import PyConfigParser
 
 from odcs.server import logger
 from odcs.common.types import COMPOSE_RESULTS, COMPOSE_FLAGS
 
 
 def init_config(app):
@@ -62,15 +63,17 @@
     ):
         config_section = "DevConfiguration"
         sys.stderr.write("WARN: DevConfiguration will be used.\n")
 
     # Try loading configuration from file
     config_file = os.path.join(config_dir, "config.py")
     try:
-        config_module = imp.load_source("odcs_runtime_config", config_file)
+        config_module = SourceFileLoader(
+            "odcs_runtime_config", config_file
+        ).load_module()
     except Exception as e:
         raise SystemError(
             "Error when loading configuration file {} : {}.".format(config_file, str(e))
         )
 
     # finally configure ODCS
     config_section_obj = getattr(config_module, config_section)
@@ -194,19 +197,14 @@
             "desc": "Allowed compose types.",
         },
         "auth_ldap_server": {
             "type": str,
             "default": "",
             "desc": "Server URL to query user's groups.",
         },
-        "auth_ldap_group_base": {
-            "type": str,
-            "default": "",
-            "desc": "Deprecated. Use auth_ldap_groups instead. Group base to query user's groups from LDAP server.",
-        },
         "auth_ldap_groups": {
             "type": list,
             "default": [],
             "desc": "List of pairs (search base, filter pattern) to query user's groups from LDAP server.",
         },
         "allowed_clients": {
             "type": dict,
@@ -283,14 +281,29 @@
             "desc": "Messaging topic to which internal ODCS-only messages are sent.",
         },
         "oidc_base_namespace": {
             "type": str,
             "default": "https://pagure.io/odcs/",
             "desc": "Base namespace of OIDC scopes.",
         },
+        "oidc_client_id": {
+            "type": str,
+            "default": "",
+            "desc": "OIDC client ID for CTS authentication.",
+        },
+        "oidc_client_secret": {
+            "type": str,
+            "default": "",
+            "desc": "OIDC client secret for CTS authentication.",
+        },
+        "oidc_token_url": {
+            "type": str,
+            "default": "",
+            "desc": "URL to the OIDC token endpoint for CTS authentication.",
+        },
         "sigkeys": {
             "type": list,
             "default": [],
             "desc": "Default list of sigkeys. Any package in a compose must "
             "be signed by one of those keys. Can be overriden in a "
             "compose request.",
         },
@@ -333,14 +346,20 @@
             "type": dict,
             "default": {},
             "desc": 'URLs to get the raw Pungi config from for "raw_config" '
             'source_type. Key is the name of the raw_config "source", '
             "value is the URL in which the %s string is replaced with, "
             '"commit_hash" value.',
         },
+        "raw_config_credentials": {
+            "type": dict,
+            "default": {},
+            "desc": "Secrets to use for a particular raw config configuration "
+            "source_type.",
+        },
         "raw_config_wrapper_conf_path": {
             "type": str,
             "default": "/etc/odcs/raw_config_wrapper.conf",
             "desc": "Full path to the raw_config_wrapper.conf configuration "
             "file. This file holds Pungi configuration which should "
             "import real pungi configuration from raw_config.conf "
             "in order to override some variables.",
@@ -491,56 +510,67 @@
 
         if os.path.isfile(raw_config_urls_conf):
             mtime = os.path.getmtime(raw_config_urls_conf)
             if mtime > self._raw_config_urls_mtime:
                 c = PyConfigParser()
                 c.load_from_file(raw_config_urls_conf)
                 self._setifok_raw_config_urls(c["RAW_CONFIG_URLS"])
+                self._setifok_raw_config_credentials(
+                    c.get("RAW_CONFIG_CREDENTIALS", {})
+                )
                 self._raw_config_urls_mtime = mtime
 
         return self._raw_config_urls
 
     #
     # Register your _setifok_* handlers here
     #
 
     def _setifok_allowed_clients(self, clients):
-        if type(clients) != dict:
+        if not isinstance(clients, dict):
             raise TypeError("allowed_clients must be a dict.")
         for role, role_dict in clients.items():
             if role not in ["users", "groups"]:
                 raise ValueError("Unknown role %s in allowed_clients." % role)
-            if type(role_dict) != dict:
+            if not isinstance(role_dict, dict):
                 raise TypeError("allowed_clients['%s'] is not a dict" % role)
             for user, user_dict in role_dict.items():
-                if type(user_dict) != dict:
+                if not isinstance(user_dict, dict):
                     raise TypeError(
                         "allowed_clients['%s']['%s'] is not a dict" % (role, user)
                     )
                 for key, value in user_dict.items():
-                    if type(value) not in [set, list]:
+                    if not isinstance(value, (set, list)):
                         raise ValueError(
                             "allowed_clients['%s']['%s']['%s'] is not a "
                             "list" % (role, user, key)
                         )
         self._allowed_clients = clients
 
     def _setifok_raw_config_urls(self, raw_config_urls):
-        if type(raw_config_urls) != dict:
+        if not isinstance(raw_config_urls, dict):
             raise TypeError("raw_config_urls must be a dict.")
         for name, url_data in raw_config_urls.items():
-            if type(url_data) != dict:
+            if not isinstance(url_data, dict):
                 raise TypeError("raw_config_urls['%s'] is not a dict." % name)
             for key in ["url", "config_filename"]:
                 if key not in url_data:
                     raise ValueError(
                         "raw_config_urls['%s']['%s'] is not defined." % (name, key)
                     )
         self._raw_config_urls = raw_config_urls
 
+    def _setifok_raw_config_credentials(self, raw_config_credentials):
+        if not isinstance(raw_config_credentials, dict):
+            raise TypeError("raw_config_credentials must be a dict.")
+        for name, creds in raw_config_credentials.items():
+            if not isinstance(creds, dict):
+                raise TypeError("raw_config_credentials['%s'] is not a dict." % name)
+        self._raw_config_credentials = raw_config_credentials
+
     def _setifok_log_backend(self, s):
         if s is None:
             self._log_backend = "console"
         elif s not in logger.supported_log_backends():
             raise ValueError("Unsupported log backend")
         self._log_backend = str(s)
 
@@ -561,20 +591,20 @@
 
     def _setifok_pungi_conf_path(self, s):
         if not os.path.isfile(s):
             raise ValueError("Pungi config template doesn't exist: %s" % s)
         self._pungi_conf_path = s
 
     def _setifok_celery_router_config(self, celery_router_config):
-        if type(celery_router_config) != dict:
+        if not isinstance(celery_router_config, dict):
             raise TypeError("celery_router_config must be a dict.")
 
         required_config_keys = ["routing_rules", "cleanup_task", "default_queue"]
 
         for conf_key in required_config_keys:
             if not celery_router_config.get(conf_key):
                 raise KeyError("celery_router_config is missing %s" % conf_key)
 
-        if type(celery_router_config["routing_rules"]) != dict:
+        if not isinstance(celery_router_config["routing_rules"], dict):
             raise TypeError("routing_rules must be a dict.")
 
         self._celery_router_config = celery_router_config
```

### Comparing `odcs-0.6.0/server/odcs/server/errors.py` & `odcs-0.7.0/server/odcs/server/errors.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/events.py` & `odcs-0.7.0/server/odcs/server/events.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/logger.py` & `odcs-0.7.0/server/odcs/server/logger.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/manage.py` & `odcs-0.7.0/server/odcs/server/manage.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/mbs.py` & `odcs-0.7.0/server/odcs/server/mbs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/mergerepo.py` & `odcs-0.7.0/server/odcs/server/mergerepo.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/messaging.py` & `odcs-0.7.0/server/odcs/server/messaging.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/metrics.py` & `odcs-0.7.0/server/odcs/server/metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 # SOFTWARE.
 #
 # Written by Jan Kaluza <jkaluza@redhat.com>
 
 import time
 import threading
 from sqlalchemy import func
-from prometheus_client import CollectorRegistry, Gauge
-from prometheus_client.core import GaugeMetricFamily, CounterMetricFamily
+from prometheus_client import CollectorRegistry, Gauge, Counter
 
 from odcs.common.types import (
     COMPOSE_STATES,
     PUNGI_SOURCE_TYPE_NAMES,
     INVERSE_COMPOSE_STATES,
 )
 from odcs.server.models import Compose
@@ -45,127 +44,27 @@
 except ImportError:
     CELERY_AVAILABLE = False
 
 
 registry = CollectorRegistry()
 
 
-class ComposesCollector(object):
-    def composes_total(self):
-        """
-        Returns `composes_total` GaugeMetricFamily with number of composes
-        for each state and source_type.
-        """
-        counter = GaugeMetricFamily(
-            "composes_total",
-            "Total number of composes",
-            labels=["source_type", "state"],
-        )
-        for state in COMPOSE_STATES:
-            for source_type in PUNGI_SOURCE_TYPE_NAMES:
-                count = Compose.query.filter(
-                    Compose.source_type == PUNGI_SOURCE_TYPE_NAMES[source_type],
-                    Compose.state == COMPOSE_STATES[state],
-                ).count()
-
-                counter.add_metric([source_type, state], count)
-        return counter
-
-    def raw_config_composes_count(self):
-        """
-        Returns `raw_config_composes_count` CounterMetricFamily with number of raw_config
-        composes for each `Compose.source`. For raw_config composes, the Compose.source is
-        stored in the `raw_config_key#commit_or_branch` format. If particular `Compose.source` is
-        generated only few times (less than 5), it is grouped by the `raw_config_key` and
-        particular `commit_or_branch` is replaced with "other_commits_or_branches" string.
-
-        This is needed to handle the situation when particular raw_config compose is generated
-        just once using particular commit hash (and not a branch name). These single composes
-        are not that important in the metrics and therefore we group them like that.
-        """
-        counter = CounterMetricFamily(
-            "raw_config_composes_count",
-            "Total number of raw_config composes per source",
-            labels=["source"],
-        )
-        composes = (
-            Compose.query.with_entities(Compose.source, func.count(Compose.source))
-            .filter(Compose.source_type == PUNGI_SOURCE_TYPE_NAMES["raw_config"])
-            .group_by(Compose.source)
-            .all()
-        )
-
-        sources = {}
-        for source, count in composes:
-            if count < 5:
-                name = "%s#other_commits_or_branches" % source.split("#")[0]
-                if name not in sources:
-                    sources[name] = 0
-                sources[name] += count
-            else:
-                sources[source] = count
-
-        for source, count in sources.items():
-            counter.add_metric([source], count)
-
-        return counter
-
-    def raw_config_types(self):
-        """
-        Returns `raw_config_composes` CounterMetricFamily with number of composes
-        for each source and state.
-        """
-        counter = CounterMetricFamily(
-            "raw_config_composes",
-            "State with count",
-            labels=["source", "state"],
-        )
-        composes = (
-            Compose.query.with_entities(
-                Compose.source, Compose.state, func.count(Compose.source)
-            )
-            .filter(Compose.source_type == PUNGI_SOURCE_TYPE_NAMES["raw_config"])
-            .group_by(Compose.state, Compose.source)
-            .all()
-        )
-
-        removed_sources = {}
-        for source, state, count in composes:
-            state = INVERSE_COMPOSE_STATES[state]
-            if state == "removed" and count < 5:
-                name = "%s#other_commits_or_branches" % source.split("#")[0]
-                if name not in removed_sources:
-                    removed_sources[name] = 0
-                removed_sources[name] += count
-            else:
-                counter.add_metric([source, state], count)
-
-        # removed_sources contains sources with state = "removed"
-        for source, count in removed_sources.items():
-            counter.add_metric([source, "removed"], count)
-
-        return counter
-
-    def collect(self):
-        yield self.composes_total()
-        yield self.raw_config_composes_count()
-        yield self.raw_config_types()
-
-
-class WorkerCountThread(threading.Thread):
+class MetricsCollectorThread(threading.Thread):
     """
     Thread providing and updating following metrics:
 
     - celery_workers_expected - Number of expected workers.
     - celery_workers_totals - Number of alive workers.
     - celery_workers[worker_name] - 1 if worker is online, 0 if offline.
+    - celery_queue_length[queue_name] - Number of tasks waiting in the queue.
+    - celery_queue_worker[queue_name] - Number of workers consume tasks from the queue.
     """
 
     def __init__(self, registry=None):
-        super(WorkerCountThread, self).__init__()
+        super(MetricsCollectorThread, self).__init__()
         self.daemon = True
         self.workers_expected = Gauge(
             "celery_workers_expected", "Number of expected workers", registry=registry
         )
         self.workers_expected.set(conf.expected_backend_number)
 
         self.workers_total = Gauge(
@@ -177,15 +76,63 @@
             "celery_workers",
             "Number of alive workers",
             ["worker_name"],
             registry=registry,
         )
         self.worker_names = set()
 
-    def update_metrics(self):
+        self.queue_length = Gauge(
+            "celery_queue_length",
+            "Number of tasks in the queue.",
+            ["queue_name"],
+            registry=registry,
+        )
+
+        # Get all the possible queue names from the config.
+        self.queues = [conf.celery_cleanup_queue]
+        for rules in conf.celery_router_config["routing_rules"].values():
+            self.queues += rules.keys()
+        # Initialize the queue length to 0.
+        for queue in self.queues:
+            self.queue_length.labels(queue).set(0)
+
+        # Get the Celery connetion.
+        self.connection = celery_app.connection_or_acquire()
+        if isinstance(self.connection, FallbackContext):
+            self.connection = self.connection.fallback()
+
+        self.queue_worker = Gauge(
+            "celery_queue_worker",
+            "Number of workers consume tasks from the queue.",
+            ["queue_name"],
+            registry=registry,
+        )
+
+        self.composes_total = Gauge(
+            "composes_total",
+            "Total number of composes",
+            ["source_type", "state"],
+            registry=registry,
+        )
+        self.raw_config_composes_count_data = {}
+        self.raw_config_composes_count = Counter(
+            "raw_config_composes_count",
+            "Total number of raw_config composes per source",
+            ["source"],
+            registry=registry,
+        )
+        self.raw_config_composes_data = {}
+        self.raw_config_composes = Counter(
+            "raw_config_composes",
+            "State with count",
+            ["source", "state"],
+            registry=registry,
+        )
+
+    def update_worker_metrics(self):
         log.info("[metrics] Getting number of workers.")
         try:
             celery_ping = celery_app.control.ping(timeout=15)
         except Exception:  # pragma: no cover
             log.exception("[metrics] Error pinging workers.")
             return
 
@@ -201,96 +148,36 @@
         # Set online workers to 1.
         for workers in celery_ping:
             for worker_name in workers.keys():
                 self.workers.labels(worker_name).set(1)
 
     def run(self):
         while True:
-            self.update_metrics()
+            self.update_compose_metrics()
+            if CELERY_AVAILABLE:
+                self.update_worker_metrics()
+                self.update_queue_metrics()
+                self.update_queue_worker_metrics()
             time.sleep(30)
 
-
-class QueueLengthThread(threading.Thread):
-    """
-    Thread providing and updating following metrics:
-
-    - celery_queue_length[queue_name] - Number of tasks waiting in the queue.
-    """
-
-    def __init__(self, registry=None):
-        super(QueueLengthThread, self).__init__()
-        self.daemon = True
-        self.queue_length = Gauge(
-            "celery_queue_length",
-            "Number of tasks in the queue.",
-            ["queue_name"],
-            registry=registry,
-        )
-
-        # Get all the possible queue names from the config.
-        self.queues = [conf.celery_cleanup_queue]
-        for rules in conf.celery_router_config["routing_rules"].values():
-            self.queues += rules.keys()
-        # Initialize the queue length to 0.
-        for queue in self.queues:
-            self.queue_length.labels(queue).set(0)
-
-        # Get the Celery connetion.
-        self.connection = celery_app.connection_or_acquire()
-        if isinstance(self.connection, FallbackContext):
-            self.connection = self.connection.fallback()
-
-    def update_metrics(self):
+    def update_queue_metrics(self):
         for queue in self.queues:
             try:
                 log.info("[metrics] Getting %s queue length." % queue)
                 length = self.connection.default_channel.queue_declare(
                     queue=queue, passive=True
                 ).message_count
                 self.queue_length.labels(queue).set(length)
             except amqp.exceptions.ChannelError:
                 # Queue not created yet.
                 pass
             except Exception:  # pragma: no cover
                 log.exception("[metrics] Error getting queue length.")
 
-    def run(self):
-        while True:
-            self.update_metrics()
-            time.sleep(30)
-
-
-class QueueWorkerThread(threading.Thread):
-    """
-    Thread providing and updating following metrics:
-
-    - celery_queue_worker[queue_name] - Number of workers consume tasks from the queue.
-    """
-
-    def __init__(self, registry=None):
-        super(QueueWorkerThread, self).__init__()
-        self.daemon = True
-        self.queue_worker = Gauge(
-            "celery_queue_worker",
-            "Number of workers consume tasks from the queue.",
-            ["queue_name"],
-            registry=registry,
-        )
-
-        # Get all the possible queue names from the config.
-        self.queues = [conf.celery_cleanup_queue]
-        for rules in conf.celery_router_config["routing_rules"].values():
-            self.queues += rules.keys()
-
-        # Get the Celery connetion.
-        self.connection = celery_app.connection_or_acquire()
-        if isinstance(self.connection, FallbackContext):
-            self.connection = self.connection.fallback()
-
-    def update_metrics(self):
+    def update_queue_worker_metrics(self):
         log.info("[metrics] Getting queue worker number.")
         try:
             active_queues = celery_app.control.inspect().active_queues()
         except Exception:  # pragma: no cover
             log.exception("[metrics] Error inspect active queues.")
             return
 
@@ -298,40 +185,106 @@
         for queue in self.queues:
             self.queue_worker.labels(queue).set(0)
 
         for queues in active_queues.values():
             for q in queues:
                 self.queue_worker.labels(q["name"]).inc()
 
-    def run(self):
-        while True:
-            self.update_metrics()
-            time.sleep(30)
+    def update_composes_total(self):
+        """
+        Updates `composes_total` metric with number of composes for each state
+        and source_type.
+        """
+        for state in COMPOSE_STATES:
+            for source_type in PUNGI_SOURCE_TYPE_NAMES:
+                count = Compose.query.filter(
+                    Compose.source_type == PUNGI_SOURCE_TYPE_NAMES[source_type],
+                    Compose.state == COMPOSE_STATES[state],
+                ).count()
 
+                self.composes_total.labels(source_type, state).set(count)
 
-class ComposeCollectorThread(threading.Thread):
-    def __init__(self):
-        super(ComposeCollectorThread, self).__init__()
-        self.daemon = True
+    def update_raw_config_composes_count(self):
+        """
+        Updates `raw_config_composes_count_total` metrics with number of
+        raw_config composes for each `Compose.source`. For raw_config composes,
+        the Compose.source is stored in the `raw_config_key#commit_or_branch`
+        format. If particular `Compose.source` is generated only few times
+        (less than 5), it is grouped by the `raw_config_key` and particular
+        `commit_or_branch` is replaced with "other_commits_or_branches" string.
+
+        This is needed to handle the situation when particular raw_config
+        compose is generated just once using particular commit hash (and not a
+        branch name). These single composes are not that important in the
+        metrics and therefore we group them like that.
+        """
+        composes = (
+            Compose.query.with_entities(Compose.source, func.count(Compose.source))
+            .filter(Compose.source_type == PUNGI_SOURCE_TYPE_NAMES["raw_config"])
+            .group_by(Compose.source)
+            .all()
+        )
 
-    def run(self):
-        registry.register(ComposesCollector())
+        sources = {}
+        for source, count in composes:
+            if count < 5:
+                name = "%s#other_commits_or_branches" % source.split("#")[0]
+                if name not in sources:
+                    sources[name] = 0
+                sources[name] += count
+            else:
+                sources[source] = count
+
+        for source, count in sources.items():
+            increment = count - self.raw_config_composes_count_data.get(source, 0)
+            self.raw_config_composes_count_data[source] = count
+            self.raw_config_composes_count.labels(source).inc(increment)
+
+    def update_raw_config_types(self):
+        composes = (
+            Compose.query.with_entities(
+                Compose.source, Compose.state, func.count(Compose.source)
+            )
+            .filter(Compose.source_type == PUNGI_SOURCE_TYPE_NAMES["raw_config"])
+            .group_by(Compose.state, Compose.source)
+            .all()
+        )
 
+        removed_sources = {}
+        for source, state, count in composes:
+            state = INVERSE_COMPOSE_STATES[state]
+            if state == "removed" and count < 5:
+                name = "%s#other_commits_or_branches" % source.split("#")[0]
+                if name not in removed_sources:
+                    removed_sources[name] = 0
+                removed_sources[name] += count
+            else:
+                increment = count - self.raw_config_composes_data.get(
+                    (source, state), 0
+                )
+                self.raw_config_composes_data[(source, state)] = count
+                self.raw_config_composes.labels(source, state).inc(increment)
+
+        # removed_sources contains sources with state = "removed"
+        for source, count in removed_sources.items():
+            increment = count - self.raw_config_composes_data.get(
+                (source, "removed"), 0
+            )
+            self.raw_config_composes_data[(source, "removed")] = count
+            self.raw_config_composes.labels(source, "removed").inc(increment)
 
-composes_collector_thread = ComposeCollectorThread()
-composes_collector_thread.start()
+    def update_compose_metrics(self):
+        log.info("[metrics] Getting compose counts.")
+        self.update_composes_total()
+        self.update_raw_config_composes_count()
+        self.update_raw_config_types()
 
 
 # Start the Celery metrics only on Frontend using the `before_first_request` decorator.
 @app.before_first_request
 def start_celery_metrics():
-    if CELERY_AVAILABLE:
-        # These threads are "daemonic". This means they are stopped automatically
-        # by Python when main Python thread is stopped. There is no need to .join()
-        # and since they are only updating metrics, they do not have to end up
-        # gracefully and can just be "killed" by Python.
-        worker_count_thread = WorkerCountThread(registry=registry)
-        worker_count_thread.start()
-        queue_length_thread = QueueLengthThread(registry=registry)
-        queue_length_thread.start()
-        queue_worker_thread = QueueWorkerThread(registry=registry)
-        queue_worker_thread.start()
+    # This thread is "daemonic". This means it is stopped automatically by
+    # Python when main Python thread is stopped. There is no need to .join()
+    # and since it is only updating metrics, it does not have to end up
+    # gracefully and can just be "killed" by Python.
+    metrics_collector_thread = MetricsCollectorThread(registry=registry)
+    metrics_collector_thread.start()
```

### Comparing `odcs-0.6.0/server/odcs/server/mock_runroot.py` & `odcs-0.7.0/server/odcs/server/mock_runroot.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/models.py` & `odcs-0.7.0/server/odcs/server/models.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/openapi.py` & `odcs-0.7.0/server/odcs/server/openapi.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/proxy.py` & `odcs-0.7.0/server/odcs/server/proxy.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/pulp.py` & `odcs-0.7.0/server/odcs/server/pulp.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,18 @@
                     product_versions = json.loads(repo["product_versions"])
                 except ValueError:
                     log.debug(
                         "Skipping sorting repos: invalid JSON in product_versions."
                     )
                     can_sort = False
                     break
+                if not isinstance(product_versions, list):
+                    log.debug("Skipping sorting repos: no product versions.")
+                    can_sort = False
+                    break
                 if len(product_versions) != 1:
                     log.debug(
                         "Skipping sorting repos: more than one version for a repo."
                     )
                     can_sort = False
                     break
                 if not re.match(r"\d+(\.\d+)*$", product_versions[0]):
```

### Comparing `odcs-0.6.0/server/odcs/server/pungi.py` & `odcs-0.7.0/server/odcs/server/pungi.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         """Write configuration into files"""
         raise NotImplementedError("Concrete config object must implement.")
 
     def validate(self, topdir, compose_dir):
         """Validate configuration. Raises an exception of error found."""
         pass
 
+    def get_env(self):
+        """Return a dict with environment variables used for the Pungi run."""
+        return None
+
 
 class RawPungiConfig(BasePungiConfig):
     def __init__(self, compose):
         super(RawPungiConfig, self).__init__()
         self.compose = compose
         source_name, source_hash = compose.source.split("#")
 
@@ -92,14 +96,18 @@
         self.raw_config_wrapper_conf_path = url_data.get(
             "raw_config_wrapper", conf.raw_config_wrapper_conf_path
         )
         self.pungi_cfg = url_data
         self.pungi_koji_args = conf.raw_config_pungi_koji_args.get(
             source_name, conf.pungi_koji_args
         )
+        self.env = {"ODCS_RAW_CONFIG_SOURCE_NAME": source_name}
+
+    def get_env(self):
+        return self.env | os.environ
 
     def apply_raw_config_wrapper_overrides(self, cfg_path):
         try:
             with open(cfg_path) as fd:
                 raw_config_wrapper = jinja2.Template(fd.read())
             with open(cfg_path, "w") as fd:
                 fd.write(raw_config_wrapper.render(compose=self.compose.json()))
@@ -128,15 +136,20 @@
             )
             self.apply_raw_config_wrapper_overrides(os.path.join(topdir, "pungi.conf"))
         else:
             main_cfg_path = os.path.join(topdir, "pungi.conf")
 
         # Clone the git repo with raw_config pungi config files.
         repo_dir = os.path.join(topdir, "raw_config_repo")
-        clone_repo(self.pungi_cfg["url"], repo_dir, commit=self.pungi_cfg["commit"])
+        clone_repo(
+            self.pungi_cfg["url"],
+            repo_dir,
+            commit=self.pungi_cfg["commit"],
+            env=self.get_env(),
+        )
 
         # If the 'path' is defined, copy only the files from the 'path'
         # to topdir.
         if "path" in self.pungi_cfg:
             repo_dir = os.path.join(repo_dir, self.pungi_cfg["path"])
 
         copytree(repo_dir, topdir)
@@ -619,22 +632,33 @@
             if pungi_conf.get("cts_url") and pungi_conf.get("cts_keytab"):
                 compose_id_thread = ReadComposeIdThread(compose)
                 compose_id_thread.start()
 
             log_out_path = os.path.join(compose_dir, "pungi-stdout.log")
             log_err_path = os.path.join(compose_dir, "pungi-stderr.log")
 
+            env = self.pungi_cfg.get_env()
+            if conf.oidc_token_url:
+                env["CTS_OIDC_TOKEN_URL"] = conf.oidc_token_url
+
+            if conf.oidc_client_id:
+                env["CTS_OIDC_CLIENT_ID"] = conf.oidc_client_id
+
+            if conf.oidc_client_secret:
+                env["CTS_OIDC_CLIENT_SECRET"] = conf.oidc_client_secret
+
             with open(log_out_path, "w") as log_out:
                 with open(log_err_path, "w") as log_err:
                     odcs.server.utils.execute_cmd(
                         pungi_cmd,
                         cwd=td,
                         timeout=self.pungi_cfg.pungi_timeout,
                         stdout=log_out,
                         stderr=log_err,
+                        env=env or None,
                     )
         finally:
             if compose_id_thread:
                 compose_id_thread.stop()
             try:
                 if td is not None:
                     shutil.rmtree(td)
```

### Comparing `odcs-0.6.0/server/odcs/server/pungi_compose.py` & `odcs-0.7.0/server/odcs/server/pungi_compose.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/odcs/server/utils.py` & `odcs-0.7.0/server/odcs/server/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,41 +88,43 @@
 def _kill_process_group(proc, args):
     log.error("Timeout occured while running: %s", args)
     pgrp = os.getpgid(proc.pid)
     log.info("Sending SIGTERM to group %s of process %s" % (pgrp, proc.pid))
     os.killpg(pgrp, signal.SIGTERM)
 
 
-def execute_cmd(args, stdout=None, stderr=None, cwd=None, timeout=None):
+def execute_cmd(args, stdout=None, stderr=None, cwd=None, timeout=None, env=None):
     """
     Executes command defined by `args`. If `stdout` or `stderr` is set to
     Python file object, the stderr/stdout output is redirecter to that file.
     If `cwd` is set, current working directory is set accordingly for the
     executed command.
 
     :param args: list defining the command to execute.
     :param stdout: Python file object to redirect the stdout to.
     :param stderr: Python file object to redirect the stderr to.
     :param cwd: string defining the current working directory for command.
     :param timeout: Timeout in seconds after which the process and all its
         children are killed.
+    :param env: Environment variables to set for the child process. This is not
+        additive, it replaces what would otherwise be inherited.
     :raises RuntimeError: Raised when command exits with non-zero exit code.
     """
     out_log_msg = ""
     if stdout:
         out_log_msg += ", stdout log: %s" % stdout.name
     if stderr:
         out_log_msg += ", stderr log: %s" % stderr.name
 
     # Execute command and use `os.setsid` in preexec_fn to create new process
     # group so we can kill the main process and also children processes in
     # case of timeout.
     log.info("Executing command: %s%s" % (args, out_log_msg))
     proc = subprocess.Popen(
-        args, stdout=stdout, stderr=stderr, cwd=cwd, preexec_fn=os.setsid
+        args, stdout=stdout, stderr=stderr, cwd=cwd, preexec_fn=os.setsid, env=env
     )
 
     # Setup timer to kill whole process group if needed.
     if timeout:
         timeout_timer = Timer(timeout, _kill_process_group, [proc, args])
 
     try:
@@ -147,20 +149,27 @@
             args,
             proc.returncode,
             out_log_msg,
         )
         raise RuntimeError(err_msg)
 
 
-def clone_repo(url, dest, branch=None, commit=None):
-    cmd = ["git", "clone"]
+def clone_repo(url, dest, branch=None, commit=None, env=None):
+    cmd = [
+        "git",
+        "-c",
+        "credential.useHttpPath=true",
+        "-c",
+        "credential.helper=!odcs-credential-helper",
+        "clone",
+    ]
     if branch:
         cmd += ["-b", branch]
     cmd += [url, dest]
-    execute_cmd(cmd)
+    execute_cmd(cmd, env=env)
 
     if commit:
         cmd = ["git", "checkout", commit]
         execute_cmd(cmd, cwd=dest)
 
     return dest
```

### Comparing `odcs-0.6.0/server/odcs/server/views.py` & `odcs-0.7.0/server/odcs/server/views.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2` & `odcs-0.7.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz` & `odcs-0.7.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz` & `odcs-0.7.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2` & `odcs-0.7.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz` & `odcs-0.7.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2` & `odcs-0.7.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz` & `odcs-0.7.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/repodata/repomd.xml` & `odcs-0.7.0/server/tests/repo/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm` & `odcs-0.7.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm` & `odcs-0.7.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm` & `odcs-0.7.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm` & `odcs-0.7.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm` & `odcs-0.7.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/Jenkinsfile` & `odcs-0.7.0/server/tests/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/mbs.py` & `odcs-0.7.0/server/tests/mbs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_auth.py` & `odcs-0.7.0/server/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,19 +329,19 @@
                     ctx.exception.description,
                 )
 
 
 class TestQueryLdapGroups(unittest.TestCase):
     """Test auth.query_ldap_groups"""
 
-    @patch.object(conf, "auth_ldap_group_base", new="ou=Groups,dc=example,dc=com")
     @patch.object(
         conf,
         "auth_ldap_groups",
         new=[
+            ("ou=Groups,dc=example,dc=com", "memberUid={}"),
             ("ou=otherGroups,dc=example,dc=com", "memberUid={}"),
             (
                 "ou=adhoc,ou=managedGroups,dc=example,dc=com",
                 "uniqueMember=uid={},ou=users,dc=example,dc=com",
             ),
         ],
     )
@@ -409,16 +409,16 @@
         self.assertRaises(ValueError, init_auth, self.login_manager, "")
         self.assertRaises(ValueError, init_auth, self.login_manager, None)
 
     def test_init_auth_no_ldap_server(self):
         with patch.object(odcs.server.auth.conf, "auth_ldap_server", ""):
             self.assertRaises(ValueError, init_auth, self.login_manager, "kerberos")
 
-    def test_init_auths_no_ldap_group_base(self):
-        with patch.object(odcs.server.auth.conf, "auth_ldap_group_base", ""):
+    def test_init_auths_no_ldap_groups(self):
+        with patch.object(odcs.server.auth.conf, "auth_ldap_groups", []):
             self.assertRaises(ValueError, init_auth, self.login_manager, "kerberos")
 
 
 class TestDecoratorRequireScopes(unittest.TestCase):
     """Test decorator require_scopes"""
 
     @patch.object(conf, "oidc_base_namespace", new="http://example.com/")
```

### Comparing `odcs-0.6.0/server/tests/test_backend.py` & `odcs-0.7.0/server/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_cache.py` & `odcs-0.7.0/server/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_celery_tasks.py` & `odcs-0.7.0/server/tests/test_celery_tasks.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_events.py` & `odcs-0.7.0/server/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_metrics.py` & `odcs-0.7.0/server/tests/test_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 from mock import patch
 
 from odcs.server import db
 from odcs.server.models import Compose
 from odcs.common.types import COMPOSE_RESULTS
 from odcs.server.pungi import PungiSourceType
-from odcs.server.metrics import ComposesCollector, QueueLengthThread, WorkerCountThread
+from odcs.server.metrics import MetricsCollectorThread
 from .utils import ModelsBaseTest
 
 
 class TestComposesCollector(ModelsBaseTest):
     def setUp(self):
         super(TestComposesCollector, self).setUp()
-        self.collector = ComposesCollector()
+        self.thread = MetricsCollectorThread()
 
     def test_composes_total(self):
         Compose.create(
             db.session,
             "unknown",
             PungiSourceType.MODULE,
             "testmodule:master",
@@ -50,16 +50,17 @@
             PungiSourceType.KOJI_TAG,
             "f26",
             COMPOSE_RESULTS["repository"],
             60,
         )
         db.session.commit()
 
-        r = self.collector.composes_total()
-        for sample in r.samples:
+        self.thread.update_compose_metrics()
+        metrics = self.thread.raw_config_composes_count.collect()
+        for sample in metrics[0].samples:
             if (
                 sample.labels["source_type"] in ["module", "tag"]
                 and sample.labels["state"] == "wait"
             ):
                 self.assertEqual(sample.value, 1)
             else:
                 self.assertEqual(sample.value, 0)
@@ -80,31 +81,33 @@
                 "me",
                 PungiSourceType.RAW_CONFIG,
                 "foo#hash%d" % i,
                 COMPOSE_RESULTS["repository"],
                 60,
             )
         db.session.commit()
-        r = self.collector.raw_config_composes_count()
-        for sample in r.samples:
-            if sample.labels["source"] == "foo#bar":
-                self.assertEqual(sample.value, 15)
-            elif sample.labels["source"] == "foo#other_commits_or_branches":
-                self.assertEqual(sample.value, 10)
+        self.thread.update_compose_metrics()
+        metrics = self.thread.raw_config_composes_count.collect()
+        for sample in metrics[0].samples:
+            if sample.name == "raw_config_composes_count_total":
+                if sample.labels["source"] == "foo#bar":
+                    self.assertEqual(sample.value, 15)
+                elif sample.labels["source"] == "foo#other_commits_or_branches":
+                    self.assertEqual(sample.value, 10)
 
 
 class TestQueueLengthThread(ModelsBaseTest):
     @patch("odcs.server.metrics.celery_app")
     def test_update_metrics(self, celery_app):
         conn = celery_app.connection_or_acquire.return_value
         queue_declare = conn.default_channel.queue_declare
         queue_declare.return_value.message_count = 10
 
-        thread = QueueLengthThread()
-        thread.update_metrics()
+        thread = MetricsCollectorThread()
+        thread.update_queue_metrics()
         metrics = thread.queue_length.collect()
         for metric in metrics:
             queues = set()
             for sample in metric.samples:
                 queues.add(sample.labels["queue_name"])
                 self.assertEqual(sample.value, 10)
             self.assertEqual(
@@ -120,25 +123,25 @@
                 {"worker-1@localhost": {"ok": "pong"}},
                 {"worker-2@localhost": {"ok": "pong"}},
             ],
             [{"worker-1@localhost": {"ok": "pong"}}],
         ]
 
         # Both workers online.
-        thread = WorkerCountThread()
-        thread.update_metrics()
+        thread = MetricsCollectorThread()
+        thread.update_worker_metrics()
         metrics = thread.workers_total.collect()
         self.assertEqual(metrics[0].samples[0].value, 2)
         metrics = thread.workers.collect()
         for metric in metrics:
             for sample in metric.samples:
                 self.assertEqual(sample.value, 1)
 
         # The worker-2 went offline.
-        thread.update_metrics()
+        thread.update_worker_metrics()
         metrics = thread.workers_total.collect()
         self.assertEqual(metrics[0].samples[0].value, 1)
         metrics = thread.workers.collect()
         for metric in metrics:
             for sample in metric.samples:
                 if sample.labels["worker_name"] == "worker-1@localhost":
                     self.assertEqual(sample.value, 1)
```

### Comparing `odcs-0.6.0/server/tests/test_mock_runroot.py` & `odcs-0.7.0/server/tests/test_mock_runroot.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_models.py` & `odcs-0.7.0/server/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_pulp.py` & `odcs-0.7.0/server/tests/test_pulp.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_pungi.py` & `odcs-0.7.0/server/tests/test_pungi.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     PungiLogs,
     RawPungiConfig,
 )
 from odcs.server import conf, db
 from odcs.server.models import Compose
 from odcs.common.types import COMPOSE_STATES, COMPOSE_RESULTS, COMPOSE_FLAGS
 from odcs.server.utils import makedirs
-from .utils import AnyStringWith, ModelsBaseTest
+from .utils import AnyDictWith, AnyStringWith, ModelsBaseTest
 
 test_dir = os.path.abspath(os.path.dirname(__file__))
 
 
 class TestPungiConfig(unittest.TestCase):
     def setUp(self):
         super(TestPungiConfig, self).setUp()
@@ -405,15 +405,15 @@
         pass
 
 
 class TestPungi(ModelsBaseTest):
     def setUp(self):
         super(TestPungi, self).setUp()
 
-        def mocked_clone_repo(url, dest, branch="master", commit=None):
+        def mocked_clone_repo(url, dest, branch="master", commit=None, env=None):
             makedirs(dest)
             makedirs(os.path.join(dest, "another"))
             with open(os.path.join(dest, "pungi.conf"), "w") as fd:
                 lines = [
                     'release_name = "fake pungi conf 1"',
                     'release_short = "compose-1"',
                     'release_version = "10"',
@@ -477,14 +477,15 @@
                 AnyStringWith("--compose-dir="),
                 "--test",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=3600,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=None,
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_pungi_run_parent_pungi_compose_ids(self, execute_cmd):
         self.compose.parent_pungi_compose_ids = "Fedora-1-1 Fedora-2-2"
         pungi_cfg = PungiConfig(
             "MBS-512", "1", PungiSourceType.MODULE, "testmodule:master:1:1"
@@ -508,14 +509,15 @@
                 "--parent-compose-id=Fedora-1-1",
                 "--parent-compose-id=Fedora-2-2",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=3600,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=None,
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_pungi_run_respin_of(self, execute_cmd):
         self.compose.respin_of = "Fedora-1-1"
         pungi_cfg = PungiConfig(
             "MBS-512", "1", PungiSourceType.MODULE, "testmodule:master:1:1"
@@ -538,14 +540,15 @@
                 "--test",
                 "--respin-of=Fedora-1-1",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=3600,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=None,
         )
 
     @patch("odcs.server.utils.execute_cmd")
     @patch("odcs.server.pungi.PyConfigParser")
     def test_pungi_run_cts(self, py_config_parser, execute_cmd):
         self.patch_ci_dump.stop()
         py_config_parser.return_value = FakePyConfigParser(
@@ -592,14 +595,15 @@
                 AnyStringWith("--compose-dir="),
                 "--test",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=3600,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=None,
         )
 
         self.assertEqual(self.compose.pungi_compose_id, "Fedora-Rawhide-20200517.n.1")
 
     @patch("odcs.server.utils.execute_cmd")
     def test_pungi_run_compose_type(self, execute_cmd):
         for compose_type in [None, "test", "ci", "nightly", "production"]:
@@ -628,14 +632,15 @@
                     AnyStringWith("--compose-dir="),
                     "--%s" % (compose_type or "test"),
                 ],
                 cwd=AnyStringWith("/tmp/"),
                 timeout=3600,
                 stderr=AnyStringWith("pungi-stderr.log"),
                 stdout=AnyStringWith("pungi-stdout.log"),
+                env=None,
             )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_pungi_run_raw_config(self, execute_cmd):
         def mocked_execute_cmd(*args, **kwargs):
             topdir = kwargs["cwd"]
             with open(os.path.join(topdir, "pungi.conf"), "r") as f:
@@ -662,14 +667,15 @@
         )
 
         execute_cmd.assert_called_once()
         self.clone_repo.assert_called_once_with(
             "http://localhost/test.git",
             AnyStringWith("/raw_config_repo"),
             commit="hash",
+            env=AnyDictWith(ODCS_RAW_CONFIG_SOURCE_NAME="pungi.conf"),
         )
         compose_date = time.strftime("%Y%m%d", time.localtime())
         self.assertEqual(
             self.compose.pungi_compose_id, "compose-1-10-%s.t.0" % compose_date
         )
 
     @patch("odcs.server.utils.execute_cmd")
@@ -731,14 +737,15 @@
             pungi.run(self.compose)
 
         execute_cmd.assert_called_once()
         self.clone_repo.assert_called_once_with(
             "http://localhost/test.git",
             AnyStringWith("/raw_config_repo"),
             commit="hash",
+            env=AnyDictWith(ODCS_RAW_CONFIG_SOURCE_NAME="pungi.conf"),
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_raw_config_validate(self, execute_cmd):
         fake_raw_config_urls = {
             "pungi.conf": {
                 "url": "http://localhost/test.git",
@@ -796,14 +803,15 @@
                 AnyStringWith("--compose-dir="),
                 "--test",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=7200,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=AnyDictWith(ODCS_RAW_CONFIG_SOURCE_NAME="pungi.conf"),
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_pungi_run_raw_config_label(self, execute_cmd):
         self.compose.label = "Alpha-0.1"
 
         fake_raw_config_urls = {
@@ -827,14 +835,15 @@
                 "--test",
                 "--label=Alpha-0.1",
             ],
             cwd=AnyStringWith("/tmp/"),
             timeout=7200,
             stderr=AnyStringWith("pungi-stderr.log"),
             stdout=AnyStringWith("pungi-stdout.log"),
+            env=AnyDictWith(ODCS_RAW_CONFIG_SOURCE_NAME="pungi.conf"),
         )
 
 
 class TestRawPungiConfig(ModelsBaseTest):
     def setUp(self):
         super(TestRawPungiConfig, self).setUp()
         self.compose = Compose.create(
@@ -843,15 +852,15 @@
             PungiSourceType.RAW_CONFIG,
             "test.conf#hash",
             COMPOSE_RESULTS["repository"],
             3600,
         )
         db.session.commit()
 
-        def mocked_clone_repo(url, dest, branch="master", commit=None):
+        def mocked_clone_repo(url, dest, branch="master", commit=None, env=None):
             makedirs(dest)
             with open(os.path.join(dest, "test.conf"), "w") as fd:
                 lines = [
                     'release_name = "fake pungi conf 1"',
                     'release_short = "compose-1"',
                     'release_version = "10"',
                 ]
```

### Comparing `odcs-0.6.0/server/tests/test_pungi_compose.py` & `odcs-0.7.0/server/tests/test_pungi_compose.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_remove_expired_composes_thread.py` & `odcs-0.7.0/server/tests/test_remove_expired_composes_thread.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/test_utils.py` & `odcs-0.7.0/server/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,36 +47,60 @@
     @patch("odcs.server.utils._kill_process_group")
     def test_execute_cmd_timeout_not_called(self, killpg):
         execute_cmd(["/usr/bin/true"], timeout=1)
         time.sleep(2)
         killpg.assert_not_called()
 
 
+GIT_COMMAND = [
+    "git",
+    "-c",
+    "credential.useHttpPath=true",
+    "-c",
+    "credential.helper=!odcs-credential-helper",
+]
+
+
 class TestCloneRepo(unittest.TestCase):
     @patch("odcs.server.utils.execute_cmd")
     def test_clone_repo(self, ec):
         clone_repo("git://localhost/test.git", "/tmp")
 
         self.assertEqual(
-            ec.mock_calls, [call(["git", "clone", "git://localhost/test.git", "/tmp"])]
+            ec.mock_calls,
+            [
+                call(
+                    GIT_COMMAND + ["clone", "git://localhost/test.git", "/tmp"],
+                    env=None,
+                ),
+            ],
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_clone_repo_branch(self, ec):
         clone_repo("git://localhost/test.git", "/tmp", branch="main")
 
         self.assertEqual(
             ec.mock_calls,
-            [call(["git", "clone", "-b", "main", "git://localhost/test.git", "/tmp"])],
+            [
+                call(
+                    GIT_COMMAND
+                    + ["clone", "-b", "main", "git://localhost/test.git", "/tmp"],
+                    env=None,
+                ),
+            ],
         )
 
     @patch("odcs.server.utils.execute_cmd")
     def test_clone_repo_commit(self, ec):
         clone_repo("git://localhost/test.git", "/tmp", commit="hash")
 
         self.assertEqual(
             ec.mock_calls,
             [
-                call(["git", "clone", "git://localhost/test.git", "/tmp"]),
+                call(
+                    GIT_COMMAND + ["clone", "git://localhost/test.git", "/tmp"],
+                    env=None,
+                ),
                 call(["git", "checkout", "hash"], cwd="/tmp"),
             ],
         )
```

### Comparing `odcs-0.6.0/server/tests/test_views.py` & `odcs-0.7.0/server/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/server/tests/utils.py` & `odcs-0.7.0/server/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,22 @@
 
 
 class AnyStringWith(str):
     def __eq__(self, other):
         return self in str(other)
 
 
+class AnyDictWith(dict):
+    def __eq__(self, another):
+        for k, v in self.items():
+            if k not in another or another[k] != v:
+                return False
+        return True
+
+
 class ConfigPatcher(object):
     def __init__(self, config_obj):
         self.objects = []
         self.config_obj = config_obj
 
     def patch(self, key, value):
         try:
```

### Comparing `odcs-0.6.0/README.md` & `odcs-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `odcs-0.6.0/setup.py` & `odcs-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     long_description = f.read()
 
 setup(
     name="odcs",
     description="On Demand Compose Service",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.0",
+    version="0.7.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Build Tools",
     ],
     keywords="on demand compose service modularity fedora",
     author="The Compose Team",
     # TODO: Not sure which name would be used for mail alias,
@@ -88,14 +88,15 @@
     scripts=["client/contrib/odcs", "server/contrib/odcs-promote-compose"],
     entry_points={
         "console_scripts": [
             "odcs-gencert = odcs.server.manage:generatelocalhostcert [server]",
             "odcs-frontend = odcs.server.manage:runssl [server]",
             "odcs-mock-runroot = odcs.server.mock_runroot:mock_runroot_main [server]",
             "odcs-manager = odcs.server.manage:cli [server]",
+            "odcs-credential-helper = odcs.server.credential_helper:main [server]",
         ],
     },
     data_files=[
         (
             get_dir(["etc", "odcs"]),
             [
                 "server/conf/config.py",
```

### Comparing `odcs-0.6.0/PKG-INFO` & `odcs-0.7.0/odcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odcs
-Version: 0.6.0
+Version: 0.7.0
 Summary: On Demand Compose Service
 Home-page: https://pagure.io/odcs/
 Author: The Compose Team
 Author-email: odcs-owner@fedoraproject.org
 License: MIT
 Description: # On Demand Compose Service - ODCS
```

