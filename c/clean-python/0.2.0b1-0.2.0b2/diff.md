# Comparing `tmp/clean-python-0.2.0b1.tar.gz` & `tmp/clean-python-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-python-0.2.0b1.tar", last modified: Tue Jul 25 07:30:27 2023, max compression
+gzip compressed data, was "clean-python-0.2.0b2.tar", last modified: Wed Aug  2 11:46:47 2023, max compression
```

## Comparing `clean-python-0.2.0b1.tar` & `clean-python-0.2.0b2.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/base/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/application/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/in_memory_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/tmpdir_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/presentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/presentation/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/celery/celery_rmq_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/dramatiq/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/sleep_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/error_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/fluentbit/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fluentbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fluentbit/fluentbit_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/oauth2/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/sql_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/profilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:30:26.000000 clean-python-0.2.0b1/clean_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 07:30:27.210447 clean-python-0.2.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_celery_rmq_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/application/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/base/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/in_memory_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/tmpdir_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/base/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/presentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/presentation/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/celery/celery_rmq_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/dramatiq/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/error_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/fluentbit/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fluentbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fluentbit/fluentbit_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/oauth2/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/sql_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/profilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:46:46.000000 clean-python-0.2.0b2/clean_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_celery_rmq_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_value_object.py
```

### Comparing `clean-python-0.2.0b1/CHANGES.md` & `clean-python-0.2.0b2/CHANGES.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,44 @@
 # Changelog of clean-python
 
 
+0.2.0b2 (2023-08-02)
+--------------------
+
+- ApiKey authentication now uses `Authorization` header and `bearer` prefix by default.
+
+
+0.1.2 (2023-07-31)
+------------------
+
+- Added py.typed marker.
+
+
 0.2.0b1 (2023-07-25)
 --------------------
 
 - `BadRequest` needs `.errors()` method to be backwards compatible.
 
 - Added support for API key authentication.
 
 
 0.2.0b0 (2023-07-23)
 --------------------
 
 - Pydantic 2.x support. Drops Pydantic 1.x support, use 0.1.x for Pydantic 1.x.
 
 
+0.1.1 (2023-07-31)
+------------------
+
+- Various import fixes.
+
+- Avoid inject==5.* because of its incompatibility with VS Code (pylance / pyright).
+
+
 0.1.0 (2023-07-12)
+------------------
 
 - Initial project structure created with cookiecutter and
   [cookiecutter-python-template](https://github.com/nens/cookiecutter-python-template).
 
 - Ported base functions from internal raster-service project.
```

### Comparing `clean-python-0.2.0b1/LICENSE` & `clean-python-0.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/PKG-INFO` & `clean-python-0.2.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b1/README.md` & `clean-python-0.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/base/application/manage.py` & `clean-python-0.2.0b2/clean_python/base/application/manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/domain_event.py` & `clean-python-0.2.0b2/clean_python/base/domain/domain_event.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/exceptions.py` & `clean-python-0.2.0b2/clean_python/base/domain/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         error = self._internal_error
         if isinstance(error, ValidationError):
             error = error.errors()[0]
             loc = "'" + ",".join([str(x) for x in error["loc"]]) + "' "
             if loc == "'*' ":
                 loc = ""
             return f"validation error: {loc}{error['msg']}"
-        return super().__str__()
+        return f"validation error: {super().__str__()}"
 
 
 class Unauthorized(Exception):
     pass
 
 
 class PermissionDenied(Exception):
```

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/gateway.py` & `clean-python-0.2.0b2/clean_python/base/domain/gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/repository.py` & `clean-python-0.2.0b2/clean_python/base/domain/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .filter import Filter
 from .gateway import Gateway
 from .json import Json
 from .pagination import Page
 from .pagination import PageOptions
 from .root_entity import RootEntity
 
+__all__ = ["Repository"]
+
 T = TypeVar("T", bound=RootEntity)
 
 
 class Repository(Generic[T]):
     entity: Type[T]
 
     def __init__(self, gateway: Gateway):
```

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/root_entity.py` & `clean-python-0.2.0b2/clean_python/base/domain/root_entity.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from .exceptions import BadRequest
 from .value_object import ValueObject
 
+__all__ = ["RootEntity", "now"]
+
 
 def now():
     # this function is there so that we can mock it in tests
     return datetime.now(timezone.utc)
 
 
 T = TypeVar("T", bound="RootEntity")
 
-__all__ = ["RootEntity", "now"]
-
 
 class RootEntity(ValueObject):
     id: Optional[int] = None
     created_at: datetime
     updated_at: datetime
 
     @classmethod
```

### Comparing `clean-python-0.2.0b1/clean_python/base/domain/value_object.py` & `clean-python-0.2.0b2/clean_python/base/domain/value_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pydantic import BaseModel
 from pydantic import ConfigDict
 from pydantic import ValidationError
 
 from .exceptions import BadRequest
 
-__all__ = ["ValueObject"]
+__all__ = ["ValueObject", "ValueObjectWithId"]
 
 
 T = TypeVar("T", bound="ValueObject")
 
 
 class ValueObject(BaseModel):
     model_config = ConfigDict(frozen=True)
```

### Comparing `clean-python-0.2.0b1/clean_python/base/infrastructure/in_memory_gateway.py` & `clean-python-0.2.0b2/clean_python/base/infrastructure/in_memory_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/base/infrastructure/internal_gateway.py` & `clean-python-0.2.0b2/clean_python/base/infrastructure/internal_gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from clean_python.base.domain import BadRequest
 from clean_python.base.domain import DoesNotExist
 from clean_python.base.domain import Filter
 from clean_python.base.domain import PageOptions
 from clean_python.base.domain import RootEntity
 from clean_python.base.domain import ValueObject
 
+__all__ = ["InternalGateway"]
+
+
 E = TypeVar("E", bound=RootEntity)  # External
 T = TypeVar("T", bound=ValueObject)  # Internal
 
 
 # don't subclass Gateway; Gateway makes Json objects
 class InternalGateway(Generic[E, T]):
     @abstractproperty
```

### Comparing `clean-python-0.2.0b1/clean_python/celery/celery_rmq_broker.py` & `clean-python-0.2.0b2/clean_python/celery/celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/dramatiq/async_actor.py` & `clean-python-0.2.0b2/clean_python/dramatiq/async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/dramatiq/dramatiq_task_logger.py` & `clean-python-0.2.0b2/clean_python/dramatiq/dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/dramatiq/sleep_task.py` & `clean-python-0.2.0b2/clean_python/dramatiq/testing.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import asyncio
 
 from dramatiq.middleware import SkipMessage
 
 from .async_actor import async_actor
 
+__all__ = ["sleep_task"]
+
 
 @async_actor(
     retry_when=lambda x, y: isinstance(y, KeyError),
     max_retries=1,
 )
 async def sleep_task(seconds: int, return_value=None, event="success"):
     event = event.lower()
```

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/context.py` & `clean-python-0.2.0b2/clean_python/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/error_responses.py` & `clean-python-0.2.0b2/clean_python/fastapi/error_responses.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/fastapi_access_logger.py` & `clean-python-0.2.0b2/clean_python/fastapi/fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/request_query.py` & `clean-python-0.2.0b2/clean_python/fastapi/request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/resource.py` & `clean-python-0.2.0b2/clean_python/fastapi/resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/fastapi/service.py` & `clean-python-0.2.0b2/clean_python/fastapi/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 from .fastapi_access_logger import FastAPIAccessLogger
 from .resource import APIVersion
 from .resource import clean_resources
 from .resource import Resource
 
 logger = logging.getLogger(__name__)
 
+__all__ = ["Service"]
+
 
 class OAuth2Dependable(OAuth2AuthorizationCodeBearer):
     """A fastapi 'dependable' configuring OAuth2.
 
     This does two things:
     - Verify the token in each request
     - (through FastAPI magic) add the scheme to the OpenAPI spec
@@ -92,15 +94,15 @@
         "swagger_ui_init_oauth": {
             "clientId": auth.client_id,
             "usePkceWithAuthorizationCodeGrant": True,
         },
     }
 
 
-api_key_header = APIKeyHeader(name="access_token", auto_error=False)
+api_key_header = APIKeyHeader(name="Authorization", auto_error=True)
 
 
 class ApiKeyDependable:
     def __init__(self, scope, settings: AccessTokenVerifierSettings):
         self.verifier = sync_to_async(
             OAuth2AccessTokenVerifier(
                 scope,
@@ -108,18 +110,24 @@
                 resource_server_id=settings.resource_server_id,
                 algorithms=settings.algorithms,
                 admin_users=settings.admin_users,
                 verify_scope_enabled=settings.scope_validation_enabled,
             ),
             thread_sensitive=False,
         )
+        self.prefix = settings.prefix
 
     async def __call__(
         self, request: Request, api_key_header: str = Security(api_key_header)
     ) -> None:
+        if not api_key_header.lower().startswith(self.prefix.lower()):
+            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
+
+        # skip bearer part
+        api_key_header = api_key_header[len(self.prefix) + 1, :]
         try:
             claims = await self.verifier(api_key_header)
             request.scope["user"] = claims
         except Unauthorized:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
         except PermissionDenied:
             raise HTTPException(status_code=HTTP_403_FORBIDDEN)
```

### Comparing `clean-python-0.2.0b1/clean_python/oauth2/oauth2.py` & `clean-python-0.2.0b2/clean_python/oauth2/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 class AccessTokenVerifierSettings(BaseModel):
     issuer: str
     resource_server_id: str
     algorithms: List[str] = ["RS256"]
     admin_users: List[str]
     scope_validation_enabled: bool = True
+    prefix: str = "bearer"
 
 
 class OAuth2AccessTokenVerifier:
     """A class for verifying OAuth2 Access Tokens from AWS Cognito
 
     The verification steps followed are documented here:
```

### Comparing `clean-python-0.2.0b1/clean_python/sql/sql_gateway.py` & `clean-python-0.2.0b2/clean_python/sql/sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/sql/sql_provider.py` & `clean-python-0.2.0b2/clean_python/sql/sql_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/sql/testing.py` & `clean-python-0.2.0b2/clean_python/sql/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python/testing/debugger.py` & `clean-python-0.2.0b2/clean_python/testing/debugger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+__all__ = ["setup_debugger"]
+
 
 def setup_debugger(*, host: str = "0.0.0.0", port: int = 5678):
     """Configure debugging via debugpy."""
 
     # Only to be used in development. Should someone inadvertently set DEBUG to True in
     # staging or production, a ModuleNotFoundError will be raised, because debugpy is
     # only available via requirements-dev.txt - this is intentionally.
```

### Comparing `clean-python-0.2.0b1/clean_python/testing/profilers.py` & `clean-python-0.2.0b2/clean_python/testing/profilers.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/clean_python.egg-info/PKG-INFO` & `clean-python-0.2.0b2/clean_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b1/clean_python.egg-info/SOURCES.txt` & `clean-python-0.2.0b2/clean_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 clean_python/__init__.py
+clean_python/py.typed
 clean_python.egg-info/PKG-INFO
 clean_python.egg-info/SOURCES.txt
 clean_python.egg-info/dependency_links.txt
 clean_python.egg-info/not-zip-safe
 clean_python.egg-info/requires.txt
 clean_python.egg-info/top_level.txt
 clean_python/base/__init__.py
@@ -33,15 +34,15 @@
 clean_python/base/presentation/__init__.py
 clean_python/base/presentation/link.py
 clean_python/celery/__init__.py
 clean_python/celery/celery_rmq_broker.py
 clean_python/dramatiq/__init__.py
 clean_python/dramatiq/async_actor.py
 clean_python/dramatiq/dramatiq_task_logger.py
-clean_python/dramatiq/sleep_task.py
+clean_python/dramatiq/testing.py
 clean_python/fastapi/__init__.py
 clean_python/fastapi/context.py
 clean_python/fastapi/error_responses.py
 clean_python/fastapi/fastapi_access_logger.py
 clean_python/fastapi/request_query.py
 clean_python/fastapi/resource.py
 clean_python/fastapi/service.py
```

### Comparing `clean-python-0.2.0b1/pyproject.toml` & `clean-python-0.2.0b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 readme = "README.md"
 license = {text = "MIT"}
 # Get classifier strings from http://www.python.org/pypi?%3Aaction=list_classifiers
 classifiers = ["Programming Language :: Python"]
 keywords = []
 requires-python = ">=3.7"
-dependencies = ["pydantic==2.*", "inject", "asgiref", "blinker"]
+dependencies = ["pydantic==2.*", "inject==4.*", "asgiref", "blinker"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-asyncio",
```

### Comparing `clean-python-0.2.0b1/tests/test_async_actor.py` & `clean-python-0.2.0b2/tests/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_celery_rmq_broker.py` & `clean-python-0.2.0b2/tests/test_celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_dramatiq_task_logger.py` & `clean-python-0.2.0b2/tests/test_dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_exceptions.py` & `clean-python-0.2.0b2/tests/test_exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from clean_python import BadRequest
 from clean_python import DoesNotExist
 from clean_python import ValueObject
 
 
 def test_bad_request_short_str():
     e = BadRequest("bla bla bla")
-    assert str(e) == "bla bla bla"
+    assert str(e) == "validation error: bla bla bla"
 
 
 def test_does_not_exist_str():
     e = DoesNotExist("raster", id=12)
     assert str(e) == "does not exist: raster with id=12"
```

### Comparing `clean-python-0.2.0b1/tests/test_fastapi_access_logger.py` & `clean-python-0.2.0b2/tests/test_fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_gateway.py` & `clean-python-0.2.0b2/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_internal_gateway.py` & `clean-python-0.2.0b2/tests/test_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_manage.py` & `clean-python-0.2.0b2/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_oauth2.py` & `clean-python-0.2.0b2/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_repository.py` & `clean-python-0.2.0b2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_request_query.py` & `clean-python-0.2.0b2/tests/test_request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_resource.py` & `clean-python-0.2.0b2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_root_entity.py` & `clean-python-0.2.0b2/tests/test_root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_service.py` & `clean-python-0.2.0b2/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_sql_gateway.py` & `clean-python-0.2.0b2/tests/test_sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b1/tests/test_value_object.py` & `clean-python-0.2.0b2/tests/test_value_object.py`

 * *Files identical despite different names*

