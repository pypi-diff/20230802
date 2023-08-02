# Comparing `tmp/superduperdb-0.0.3.dev2.tar.gz` & `tmp/superduperdb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superduperdb-0.0.3.dev2.tar", max compression
+gzip compressed data, was "superduperdb-0.0.4.tar", last modified: Wed Aug  2 13:45:29 2023, max compression
```

## Comparing `superduperdb-0.0.3.dev2.tar` & `superduperdb-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,134 @@
--rw-r--r--   0        0        0    10225 2023-03-23 08:50:38.761856 superduperdb-0.0.3.dev2/LICENSE
--rw-r--r--   0        0        0       29 2023-07-10 16:07:41.816401 superduperdb-0.0.3.dev2/README.md
--rw-r--r--   0        0        0     2051 2023-07-10 16:07:04.158030 superduperdb-0.0.3.dev2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-10 16:06:48.602609 superduperdb-0.0.3.dev2/superduperdb/__init__.py
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 superduperdb-0.0.3.dev2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.252662 superduperdb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-08-02 13:45:20.000000 superduperdb-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-08-02 13:45:29.248662 superduperdb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-08-02 13:45:20.000000 superduperdb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 13:45:20.000000 superduperdb-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.236662 superduperdb-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 13:45:20.000000 superduperdb-0.0.4/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:45:29.252662 superduperdb-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.236662 superduperdb-0.0.4/superduperdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-02 13:45:21.000000 superduperdb-0.0.4/superduperdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.240662 superduperdb-0.0.4/superduperdb/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/config_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/jsonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/base/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.240662 superduperdb-0.0.4/superduperdb/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/cli/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/cli/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.240662 superduperdb-0.0.4/superduperdb/container/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/artifact_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/task_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/container/vector_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.240662 superduperdb-0.0.4/superduperdb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.240662 superduperdb-0.0.4/superduperdb/data/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/cache/key_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/cache/typed_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/cache/uri_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/data/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/tree/for_each.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/data/tree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/db/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/cdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/data_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31460 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/download_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/base/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/db/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/cdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/data_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/mongodb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/db/query_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/ext/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/numpy/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/ext/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/openai/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.244662 superduperdb-0.0.4/superduperdb/ext/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/pillow/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/ext/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/sklearn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/ext/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/torch/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/torch/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/ext/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/transformers/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/ext/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/vector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/ext/vector/vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/vector/vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/ext/vector/vectors/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/special_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/superduper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/misc/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/server/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/server/dask_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/server/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.248662 superduperdb-0.0.4/superduperdb/vector_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/faiss_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/inmemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/lancedb_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-02 13:45:20.000000 superduperdb-0.0.4/superduperdb/vector_search/table_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:45:29.236662 superduperdb-0.0.4/superduperdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-08-02 13:45:29.000000 superduperdb-0.0.4/superduperdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 13:45:29.000000 superduperdb-0.0.4/superduperdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:45:29.000000 superduperdb-0.0.4/superduperdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 13:45:29.000000 superduperdb-0.0.4/superduperdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 13:45:29.000000 superduperdb-0.0.4/superduperdb.egg-info/top_level.txt
```

### Comparing `superduperdb-0.0.3.dev2/LICENSE` & `superduperdb-0.0.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022- Duncan Blythe. All rights reserved.
+Copyright 2023- SuperDuperDB Inc. All rights reserved.
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

