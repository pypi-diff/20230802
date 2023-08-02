# Comparing `tmp/globus-compute-endpoint-2.2.4a0.tar.gz` & `tmp/globus-compute-endpoint-2.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.2.4a0.tar", last modified: Fri Jul 14 15:14:09 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.3.0a0.tar", last modified: Wed Aug  2 19:09:13 2023, max compression
```

## Comparing `globus-compute-endpoint-2.2.4a0.tar` & `globus-compute-endpoint-2.3.0a0.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.984479 globus-compute-endpoint-2.2.4a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       83 2023-06-26 15:08:59.000000 globus-compute-endpoint-2.2.4a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-07-14 15:14:09.984562 globus-compute-endpoint-2.2.4a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.4a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.955977 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    17160 2023-07-14 14:46:26.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.965129 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.966337 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6533 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 lei        (501) staff       (20)      760 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)      146 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/default_config.yaml
--rw-r--r--   0 lei        (501) staff       (20)     3360 2023-07-14 14:46:29.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 lei        (501) staff       (20)    27495 2023-07-12 18:48:04.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    20355 2023-07-05 15:18:10.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    23242 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     3075 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.967512 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-07-12 18:48:25.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-07-06 21:09:25.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.968172 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.969148 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/
--rw-r--r--   0 lei        (501) staff       (20)      241 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6257 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 lei        (501) staff       (20)     3701 2023-07-14 14:46:26.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 lei        (501) staff       (20)     4608 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/helper.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.971613 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34560 2023-07-14 14:46:26.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/engine.py
--rw-r--r--   0 lei        (501) staff       (20)    49294 2023-07-07 19:04:06.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36121 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9295 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     7216 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5427 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     3680 2023-07-14 14:46:26.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     2020 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.971807 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.972104 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      422 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)     8499 2023-06-26 15:08:59.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.972230 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.972987 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.974222 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-07-14 15:12:58.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.962783 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     3729 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      353 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      342 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-07-14 15:14:09.000000 globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-07-14 15:14:09.984859 globus-compute-endpoint-2.2.4a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3677 2023-07-14 15:12:53.000000 globus-compute-endpoint-2.2.4a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.974869 globus-compute-endpoint-2.2.4a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.4a0/tests/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.975325 globus-compute-endpoint-2.2.4a0/tests/integration/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    11428 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.4a0/tests/integration/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.975670 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1679 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.976175 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:14:09.984319 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2256 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
--rw-r--r--   0 lei        (501) staff       (20)     2275 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_manager.py
--rw-r--r--   0 lei        (501) staff       (20)     1273 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     1126 2023-07-06 21:18:52.000000 globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/mock_executors.py
--rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.4a0/tests/utils.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.990392 globus-compute-endpoint-2.3.0a0/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       83 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/MANIFEST.in
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-08-02 19:09:13.990392 globus-compute-endpoint-2.3.0a0/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      871 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/PyPI.md
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.970392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      131 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    18333 2023-08-01 02:37:04.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/cli.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.974392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.978392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/
+-rw-rw-r--   0 reid      (1000) reid      (1000)       41 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     6533 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/config.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      760 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      146 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3360 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/model.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7693 2023-08-02 16:22:50.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/utils.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    27932 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    21865 2023-08-01 03:32:53.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    24345 2023-08-01 19:58:23.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3075 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.978392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      307 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      689 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11834 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3068 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    14231 2023-08-01 02:59:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5184 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7275 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.978392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/utils/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1017 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      110 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/utils/config.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.978392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      310 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     6337 2023-08-01 19:58:23.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5945 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/globus_compute.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     4608 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/helper.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.982392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1943 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/container_sched.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    34864 2023-08-01 19:58:23.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/engine.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    49295 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/interchange.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     9712 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      267 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
+-rwxrwxr-x   0 reid      (1000) reid      (1000)    36125 2023-08-01 02:59:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     9295 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/messages.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7216 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/worker.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    19094 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/worker_map.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5427 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3880 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/process_pool.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3680 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/thread_pool.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2020 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/exception_handling.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      220 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/exceptions.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.982392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/executors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      141 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/executors/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.982392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/executors/high_throughput/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      422 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     8499 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/logging_config.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.982392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      115 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/kubernetes/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    12926 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       50 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/kubernetes/template.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3325 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/self_diagnostic.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      280 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7424 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5470 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     6225 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/simple.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1610 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/test.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      806 2023-08-02 18:42:54.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/version.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.970392 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3820 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      353 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      342 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       30 2023-08-02 19:09:13.000000 globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-08-02 19:09:13.990392 globus-compute-endpoint-2.3.0a0/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3677 2023-08-02 18:42:30.000000 globus-compute-endpoint-2.3.0a0/setup.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/tests/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/tests/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     4000 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/conftest.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/tests/integration/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11428 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/tests/integration/conftest.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1679 2023-07-28 22:37:35.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/conftest.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.986392 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-08-02 19:09:13.990392 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2218 2023-08-01 19:58:23.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2275 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1273 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1182 2023-08-01 19:58:23.000000 globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/mock_executors.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2925 2023-07-28 22:41:17.000000 globus-compute-endpoint-2.3.0a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.2.4a0/LICENSE` & `globus-compute-endpoint-2.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/PKG-INFO` & `globus-compute-endpoint-2.3.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.4a0
+Version: 2.3.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.4a0/PyPI.md` & `globus-compute-endpoint-2.3.0a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
+import contextlib
 import difflib
+import gzip
 import json
 import logging
 import pathlib
 import re
 import shutil
 import sys
 import uuid
+from datetime import datetime
 
 import click
 from click import ClickException
 from globus_compute_endpoint.endpoint.config.utils import get_config, load_config_yaml
 from globus_compute_endpoint.endpoint.endpoint import Endpoint
 from globus_compute_endpoint.endpoint.endpoint_manager import EndpointManager
 from globus_compute_endpoint.logging_config import setup_logging
+from globus_compute_endpoint.self_diagnostic import run_self_diagnostic
 from globus_compute_endpoint.version import DEPRECATION_FUNCX_ENDPOINT
 from globus_compute_sdk.sdk.login_manager import LoginManager
 from globus_compute_sdk.sdk.login_manager.tokenstore import ensure_compute_dir
 from globus_compute_sdk.sdk.login_manager.whoami import print_whoami_info
 
 log = logging.getLogger(__name__)
 
@@ -530,14 +534,52 @@
             f"Are you sure you want to delete the endpoint named <{name}>?", abort=True
         )
 
     ep_dir = get_config_dir() / name
     Endpoint.delete_endpoint(ep_dir, get_config(ep_dir), force=force)
 
 
+@app.command("self-diagnostic")
+@click.option(
+    "-z",
+    "--gzip",
+    "compress",
+    default=False,
+    is_flag=True,
+    help="Save the output to a Gzip-compressed file.",
+)
+@click.option(
+    "--log-kb",
+    default=5120,
+    help=(
+        "Specify the number of kilobytes (KB) to read from log files."
+        " Defaults to 5,120 KB (5 MB)."
+    ),
+)
+@click.help_option("-h", "--help")
+def self_diagnostic(compress: bool, log_kb: int):
+    """Run several diagnostic commands to help identify issues.
+
+    This may produce a large amount of output.
+    """
+    log_bytes = log_kb * 1024
+
+    if not compress:
+        run_self_diagnostic(log_bytes=log_bytes)
+    else:
+        current_date = datetime.now().strftime("%Y-%m-%d")
+        filename = f"globus_compute_diagnostic_{current_date}.txt.gz"
+
+        with gzip.open(filename, "wb") as f:
+            with contextlib.redirect_stdout(f):  # type: ignore[type-var]
+                run_self_diagnostic(log_bytes=log_bytes)
+
+        click.echo(f"Successfully created {filename}")
+
+
 def cli_run():
     """Entry point for setuptools to point to"""
     app()
 
 
 def cli_run_funcx():
     """Entry point that prints a custom message. i.e. deprecation warnings"""
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/model.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,14 +135,21 @@
     config_dict = config_schema.dict(exclude_unset=True)
 
     try:
         config = Config(**config_dict)
     except Exception as err:
         raise ClickException(str(err)) from err
 
+    # Special case of 'display_name: None' converting to the empty
+    #   None instead of the string "None" which was the default
+    #   display_name since we started generating yaml configs from
+    #   Jun til Jul 2023.
+    # This has the side effect of disallowing the display name 'None'
+    if config.display_name == "None":
+        config.display_name = None
     return config
 
 
 def get_config(endpoint_dir: pathlib.Path) -> Config:
     config_py_path = endpoint_dir / "config.py"
     config_yaml_path = endpoint_dir / "config.yaml"
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,20 @@
 
         pid_check = Endpoint.check_pidfile(endpoint_dir)
         # if the pidfile exists, we should return early because we don't
         # want to attempt to create a new daemon when one is already
         # potentially running with the existing pidfile
         if pid_check["exists"]:
             if pid_check["active"]:
-                log.info("Endpoint is already active")
+                endpoint_name = endpoint_dir.name
+                if endpoint_config.display_name:
+                    endpoint_name = endpoint_config.display_name
+                active_msg = f"Endpoint '{endpoint_name}' is already active"
+                print(active_msg)
+                log.info(active_msg)
                 sys.exit(-1)
             else:
                 log.info(
                     "A prior Endpoint instance appears to have been terminated without "
                     "proper cleanup. Cleaning up now."
                 )
                 Endpoint.pidfile_cleanup(endpoint_dir)
@@ -318,15 +323,17 @@
                     multi_tenant=False,
                     display_name=endpoint_config.display_name,
                 )
 
             except GlobusAPIError as e:
                 if e.http_status in (409, 410, 423):
                     # CONFLICT, GONE or LOCKED
-                    log.warning(f"Endpoint registration blocked.  [{e.text}]")
+                    blocked_msg = f"Endpoint registration blocked.  [{e.text}]"
+                    print(blocked_msg)
+                    log.warning(blocked_msg)
                     exit(os.EX_UNAVAILABLE)
                 raise
 
             except NetworkError as e:
                 # the output of a NetworkError exception is huge and unhelpful, so
                 # it seems better to just stringify it here and get a concise error
                 log.exception(
@@ -373,22 +380,22 @@
         ptitle += f" [{setproctitle.getproctitle()}]"
         setproctitle.setproctitle(ptitle)
 
         parent_pid = 0
         if die_with_parent:
             parent_pid = os.getppid()
 
-        log.info("Launching endpoint daemon process")
+        log.debug("Launching endpoint daemon process")
 
         # NOTE
         # It's important that this log is emitted before we enter the daemon context
         # because daemonization closes down everything, a log message inside the
         # context won't write the currently configured loggers
         logfile = endpoint_dir / "endpoint.log"
-        log.info(
+        log.debug(
             "Reconfiguring logging for daemonization. logfile: %s , debug: %s",
             logfile,
             self.debug,
         )
 
         ostream = None
         if sys.stdout.isatty():
@@ -434,27 +441,29 @@
         endpoint_uuid,
         endpoint_dir,
         endpoint_config: Config,
         reg_info,
         result_store: ResultStore,
         parent_pid: int,
     ):
+        log.info(f"\n\n========== Endpoint begins: {endpoint_uuid}")
+
         interchange = EndpointInterchange(
             config=endpoint_config,
             reg_info=reg_info,
             endpoint_id=endpoint_uuid,
             endpoint_dir=endpoint_dir,
             result_store=result_store,
             logdir=endpoint_dir,
             parent_pid=parent_pid,
         )
 
         interchange.start()
 
-        log.critical("Interchange terminated.")
+        log.info(f"\n---------- Endpoint shutdown: {endpoint_uuid}\n")
 
     @staticmethod
     def stop_endpoint(
         endpoint_dir: pathlib.Path,
         endpoint_config: Config | None,
         remote: bool = False,
     ):
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import socket
 import sys
 import threading
 import time
 import typing as t
 from datetime import datetime
 
-import globus_compute_sdk as gc
+import globus_compute_sdk as GC
 import setproctitle
+import yaml
 from globus_compute_endpoint import __version__
 from globus_compute_endpoint.endpoint.config import Config
 from globus_compute_endpoint.endpoint.config.utils import (
     render_config_user_template,
     serialize_config,
 )
 from globus_compute_endpoint.endpoint.endpoint import Endpoint
@@ -69,25 +70,27 @@
 
         try:
             client_options = {
                 "funcx_service_address": config.funcx_service_address,
                 "environment": config.environment,
             }
 
-            gcc = gc.Client(**client_options)
+            gcc = GC.Client(**client_options)
             reg_info = gcc.register_endpoint(
                 conf_dir.name,
                 endpoint_uuid,
                 metadata=EndpointManager.get_metadata(config),
                 multi_tenant=True,
             )
         except GlobusAPIError as e:
             if e.http_status == 409 or e.http_status == 423:
                 # RESOURCE_CONFLICT or RESOURCE_LOCKED
-                log.warning(f"Endpoint registration blocked.  [{e.text}]")
+                blocked_msg = f"Endpoint registration blocked.  [{e.text}]"
+                print(blocked_msg)
+                log.warning(blocked_msg)
                 exit(os.EX_UNAVAILABLE)
             raise
         except NetworkError as e:
             log.exception("Network error while registering multi-tenant endpoint")
             log.critical(f"Network failure; unable to register endpoint: {e}")
             exit(os.EX_TEMPFAIL)
 
@@ -296,15 +299,14 @@
             try:
                 server_cmd_ts = props.timestamp
                 if props.content_type != "application/json":
                     raise ValueError("Invalid message type; expecting JSON")
 
                 msg = json.loads(body)
                 command = msg.get("command")
-                user_opts = msg.get("user_opts", {})
                 command_args = msg.get("args", [])
                 command_kwargs = msg.get("kwargs", {})
             except Exception as e:
                 log.error(
                     f"Unable to deserialize Globus Compute services command."
                     f"  ({e.__class__.__name__}) {e}"
                 )
@@ -343,15 +345,15 @@
                 if not (command and valid_method_name_re.match(command)):
                     raise InvalidCommandError(f"Unknown or invalid command: {command}")
 
                 command_func = getattr(self, command, None)
                 if not command_func:
                     raise InvalidCommandError(f"Unknown or invalid command: {command}")
 
-                command_func(local_user, user_opts, command_args, command_kwargs)
+                command_func(local_user, command_args, command_kwargs)
                 log.info(
                     f"Command process successfully forked for '{globus_username}'"
                     f" ('{globus_uuid}')."
                 )
             except InvalidCommandError as err:
                 log.error(str(err))
 
@@ -363,20 +365,17 @@
                 )
             finally:
                 self._command.ack(d_tag)
 
     def cmd_start_endpoint(
         self,
         local_username: str,
-        user_opts: dict | None,
         args: list[str] | None,
         kwargs: dict | None,
     ):
-        if not user_opts:
-            user_opts = {}
         if not args:
             args = []
         if not kwargs:
             kwargs = {}
 
         ep_name = kwargs.get("name", "")
         if not ep_name:
@@ -405,20 +404,40 @@
             self._child_args[pid] = (uid, gid, local_username, proc_args_s)
             log.info(f"Creating new user endpoint (pid: {pid}) [{proc_args_s}]")
             return
 
         # Reminder: from this point on, we are now the *child* process.
         pid = os.getpid()
 
+        import shutil  # in the child process; no need to load this in MTEP space
+
         exit_code = 70
         try:
-            # TODO: PATH, which is crucial for execvpe, is currently required to
-            # be set by API call to /endpoint/command/<uuid>.  This will be
-            # addressed more thoroughly in SC-22804.
-            env = kwargs.get("env", {})
+            pybindir = pathlib.Path(sys.executable).parent
+            default_path = ("/usr/local/bin", "/usr/bin", "/bin", pybindir)
+            env: dict[str, str] = {"PATH": ":".join(map(str, default_path))}
+            env_path = self.conf_dir / "user_environment.yaml"
+            try:
+                if env_path.exists():
+                    log.debug("Load default environment variables from: %s", env_path)
+                    env_text = env_path.read_text()
+                    if env_text:
+                        env.update(
+                            {k: str(v) for k, v in yaml.safe_load(env_text).items()}
+                        )
+
+            except Exception as e:
+                log.warning(
+                    "Failed to parse user environment variables from %s.  Using "
+                    "default: %s\n  --- Exception ---\n(%s) %s",
+                    env_path,
+                    env,
+                    type(e).__name__,
+                    e,
+                )
             env.update({"HOME": udir, "USER": uname})
             if not os.path.isdir(udir):
                 udir = "/"
 
             wd = env.get("PWD", udir)
 
             os.chdir("/")  # always succeeds, so start from known place
@@ -439,15 +458,26 @@
             log.debug("Setting process group for %s to %s", pid, gid)
             os.setresgid(gid, gid, gid)  # raises (good!) on error
             exit_code += 1
             log.debug("Setting process uid for %s to %s (%s)", pid, uid, uname)
             os.setresuid(uid, uid, uid)  # raises (good!) on error
             exit_code += 1
 
+            # some Q&D verification for admin debugging purposes
+            if not shutil.which(proc_args[0], path=env["PATH"]):
+                log.warning(
+                    "Unable to find executable."
+                    f"\n  Executable (not found): {proc_args[0]}"
+                    f'\n  Path: "{env["PATH"]}"'
+                    f"\n\n  Will attempt exec anyway -- WARNING - it will likely fail."
+                    f"\n  (pid: {pid}, user: {uname}, {ep_name})"
+                )
+
             os.setsid()
+            exit_code += 1
 
             umask = 0o077  # Let child process set less restrictive, if desired
             log.debug("Setting process umask for %s to 0o%04o (%s)", pid, umask, uname)
             os.umask(umask)
             exit_code += 1
 
             log.debug("Changing directory to '%s'", wd)
@@ -457,14 +487,18 @@
             env["CWD"] = wd
 
             # in case "something gets stuck," let cmdline show it
             args_title = " ".join(proc_args)
             startup_proc_title = f"Endpoint starting up for {uname} [{args_title}]"
             setproctitle.setproctitle(startup_proc_title)
 
+            gc_dir: pathlib.Path = GC.sdk.login_manager.tokenstore.ensure_compute_dir()
+            (gc_dir / ep_name).mkdir(mode=0o700, parents=True, exist_ok=True)
+
+            user_opts = kwargs.get("user_opts", {})
             stdin_data_dict = {
                 "amqp_creds": kwargs.get("amqp_creds"),
                 "config": render_config_user_template(self.conf_dir, user_opts),
             }
             stdin_data = json.dumps(stdin_data_dict)
             exit_code += 1
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,19 @@
 # to annotate, we need the "real" class
 # see: https://github.com/python/typeshed/issues/4266
 from multiprocessing.synchronize import Event as EventType
 
 import globus_compute_endpoint.endpoint.config
 import pika.exceptions
 import setproctitle
-from globus_compute_common.messagepack import InvalidMessageError, pack, unpack
+from globus_compute_common.messagepack import InvalidMessageError, pack
 from globus_compute_common.messagepack.message_types import (
     EPStatusReport,
     Result,
     ResultErrorDetails,
-    Task,
 )
 from globus_compute_endpoint import __version__ as funcx_endpoint_version
 from globus_compute_endpoint.endpoint.rabbit_mq import (
     ResultQueuePublisher,
     TaskQueueSubscriber,
 )
 from globus_compute_endpoint.endpoint.result_store import ResultStore
@@ -199,20 +198,27 @@
 
         # kill_event must be set before quiesce_event because we need to guarantee that
         # once the quiesce is complete, the interchange will not try to start again
         self._kill_event.set()
         self._quiesce_event.set()
 
     def cleanup(self):
-        self.executor.shutdown()
+        self.executor.shutdown(block=True)
 
     def handle_sigterm(self, sig_num, curr_stack_frame):
         log.warning("Received SIGTERM, setting termination flag.")
         self.time_to_quit = True
 
+    def function_allowed(self, function_id: str):
+        if self.config.allowed_functions is None:
+            # Not a restricted endpoint
+            return True
+
+        return function_id in self.config.allowed_functions
+
     def start(self):
         """Start the Interchange"""
         signal.signal(signal.SIGHUP, self.handle_sigterm)
         signal.signal(signal.SIGQUIT, self.handle_sigterm)  # hint: Ctrl+\
         signal.signal(signal.SIGTERM, self.handle_sigterm)
         # Intentionally ignoring SIGINT for now, as we're unstable enough to
         # warrant Python's default developer-friendly Ctrl+C handling
@@ -356,77 +362,97 @@
                 # globus-compute-manager.  In terms of shutting down (or "rebooting")
                 # gracefully, iterate once a second whether or not a task has arrived.
                 nonlocal num_tasks_forwarded
                 while not self._quiesce_event.is_set():
                     if self.time_to_quit:
                         self.stop()
                         continue  # nominally == break; but let event do it
+
                     try:
-                        incoming_task = self.pending_task_queue.get(timeout=1)
-                        task_msg = unpack(incoming_task)
-                        if not isinstance(task_msg, Task):
-                            raise InvalidMessageError()
+                        prop_headers, body = self.pending_task_queue.get(timeout=1)
+
+                        fid: str = prop_headers.get("function_uuid")
+                        tid: str = prop_headers.get("task_uuid")
+                        if not fid or not tid:
+                            raise InvalidMessageError("Task message missing headers")
+
+                        if fid and not self.function_allowed(fid):
+                            # Same as web-service message but packed in a
+                            # result error
+                            reject_msg = (
+                                f"Function {fid} not permitted on "
+                                f"endpoint {self.endpoint_id}"
+                            )
+                            log.warning(reject_msg)
+
+                            failed_result = Result(
+                                task_id=tid,
+                                data=reject_msg,
+                                error_details=ResultErrorDetails(
+                                    code="FUNCTION_NOT_ALLOWED", user_message=reject_msg
+                                ),
+                            )
+                            results_publisher.publish(pack(failed_result))
+                            continue
 
                     except queue.Empty:
                         continue
 
                     except Exception:
                         log.exception("Unhandled error processing incoming task")
                         continue
 
                     try:
-                        executor.submit(
-                            task_id=task_msg.task_id, packed_task=incoming_task
-                        )
+                        executor.submit(task_id=tid, packed_task=body)
                         num_tasks_forwarded += 1  # Safe given GIL
 
                     except Exception as exc:
-                        log.exception(f"Failed to process {task_msg.task_id}")
+                        log.exception(f"Failed to process task {tid}")
                         code, msg = get_result_error_details()
                         failed_result = Result(
-                            task_id=task_msg.task_id,
+                            task_id=tid,
                             data=f"Failed to start task: {exc}",
                             error_details=ResultErrorDetails(
                                 code=code, user_message=msg
                             ),
                             task_statuses=[],
                         )
                         res = {
-                            "task_id": task_msg.task_id,
+                            "task_id": tid,
                             "message": pack(failed_result),
                         }
                         self.results_passthrough.put(res)
 
                 log.debug("Exit process-pending-tasks thread.")
 
             def process_pending_results():
                 # Forward incoming results from the globus-compute-manager to the
                 # Globus Compute services. For graceful handling of shutdown
                 # (or "reboot"), wait up to a second or incoming results before
                 # iterating the loop regardless.
                 nonlocal num_results_forwarded
                 while not self._quiesce_event.is_set():
                     try:
-                        packed_message = self.results_passthrough.get(timeout=1)
-                        unpacked_message = unpack(packed_message)
+                        msg = self.results_passthrough.get(timeout=1)
+                        packed_message: bytes = msg["message"]
+                        task_id: str | None = msg.get("task_id")
 
                     except queue.Empty:
                         # Empty queue!  Let's see if we have any prior results to send
                         continue
 
                     except Exception as exc:
                         log.warning(
-                            f"Invalid message received: no task_id.  Ignoring. {exc}"
+                            "Invalid message received.  Ignoring."
+                            f"  ([{type(exc).__name__}] {exc})"
                         )
                         continue
 
-                    task_id = None
-                    if isinstance(unpacked_message, Result):
+                    if task_id:
                         num_results_forwarded += 1
-                        task_id = unpacked_message.task_id
                         log.debug("Forwarding result for task: %s", task_id)
 
                     try:
                         results_publisher.publish(packed_message)
 
                     except Exception:
                         # Publishing didn't work -- quiesce and see if a simple restart
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,18 @@
         endpoint_id: endpoint uuid string
         """
 
         super().__init__()
         self.status = SubscriberProcessStatus.parent
 
         self.endpoint_id = endpoint_id
-        self.queue_info = queue_info
         self.external_queue = external_queue
+        self.queue_info = queue_info
         self.quiesce_event = quiesce_event
+
         self._channel_closed = multiprocessing.Event()
         self._cleanup_complete = multiprocessing.Event()
 
         self._connection: pika.SelectConnection | None = None
         self._channel: pika.channel.Channel | None = None
         self._consumer_tag: str | None = None
 
@@ -248,15 +249,17 @@
             properties.app_id,
             body,
         )
 
         # Not sure if we need to do this in a locked context,
         # rabbit's ACK system should make sure you don't lose tasks.
         try:
-            self.external_queue.put(body)
+            # TODO move ack'ing the message to final processing instead
+            headers = properties.headers if properties.headers else {}
+            self.external_queue.put([headers, body])
         except Exception:
             # No sense in waiting for the RMQ default 30m timeout; let it know
             # *now* that this message failed.
             logger.exception("External queue put failed")
             channel.basic_nack(basic_deliver.delivery_tag, requeue=True)
         else:
             channel.basic_ack(basic_deliver.delivery_tag)
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,42 +86,44 @@
         # remove these unused vars that we are adding to just keep
         # endpoint interchange happy
         self.container_type: t.Optional[str] = None
         self.funcx_service_address: t.Optional[str] = None
         self.run_dir: t.Optional[str] = None
         # This attribute could be set by the subclasses in their
         # start method if another component insists on owning the queue.
-        self.results_passthrough: queue.Queue = queue.Queue()
+        self.results_passthrough: queue.Queue[
+            dict[str, bytes | str | None]
+        ] = queue.Queue()
 
     @abstractmethod
     def start(
         self,
         *args,
         **kwargs,
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def get_status_report(self) -> EPStatusReport:
         raise NotImplementedError
 
-    def report_status(self):
+    def report_status(self) -> None:
         status_report = self.get_status_report()
-        packed_status = messagepack.pack(status_report)
-        self.results_passthrough.put(packed_status)
+        packed: bytes = messagepack.pack(status_report)
+        self.results_passthrough.put({"message": packed})
 
     def _status_report(
         self, shutdown_event: threading.Event, heartbeat_period_s: float
     ):
         while not shutdown_event.wait(timeout=heartbeat_period_s):
             status_report = self.get_status_report()
             packed = messagepack.pack(status_report)
-            self.results_passthrough.put(packed)
+            self.results_passthrough.put({"message": packed})
 
-    def _setup_future_done_callback(self, task_id: uuid.UUID, future: Future) -> None:
+    def _setup_future_done_callback(self, task_id: str, future: Future) -> None:
         """
         Set up the done() callback for the provided future.
 
         The done callback handles
         Callback to post result to the passthrough queue
         Parameters
         ----------
@@ -147,33 +149,33 @@
                 result_message = dict(
                     task_id=task_id,
                     data=get_error_string(exc=exc),
                     exception=get_error_string(exc=exc),
                     error_details=error_details,
                     task_statuses=[exec_beg, exec_end],  # only transition info we have
                 )
-                packed_result = messagepack.pack(Result(**result_message))
+                packed = messagepack.pack(Result(**result_message))
             else:
-                packed_result = f.result()
+                packed = f.result()
 
-            self.results_passthrough.put(packed_result)
+            self.results_passthrough.put({"task_id": task_id, "message": packed})
 
         future.add_done_callback(_done_cb)
 
     @abstractmethod
     def _submit(
         self,
         func: t.Callable,
         *args: t.Any,
         **kwargs: t.Any,
     ) -> Future:
         """Subclass should use the internal execution system to implement this"""
         raise NotImplementedError()
 
-    def submit(self, task_id: uuid.UUID, packed_task: bytes) -> Future:
+    def submit(self, task_id: str, packed_task: bytes) -> Future:
         """GC Endpoints should submit tasks via this method so that tasks are
         tracked properly.
         Parameters
         ----------
         packed_task: messagepack bytes buffer
         Returns
         -------
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/container_sched.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/engine.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 of functions within containerized workers in a distributed setting.
 """
 from __future__ import annotations
 
 import concurrent.futures
 import ipaddress
 import logging
+import multiprocessing
 import os
 import queue
 import threading
 import time
 import typing as t
 import uuid
 from concurrent.futures import Future
@@ -298,15 +299,15 @@
         self.worker_port_range = worker_port_range
         self.interchange_port_range = interchange_port_range
         self.heartbeat_threshold = heartbeat_threshold
         self.heartbeat_period = heartbeat_period
         self.poll_period = poll_period
         self.suppress_failure = suppress_failure
         self.run_dir = run_dir
-        self.queue_proc = None
+        self.queue_proc: multiprocessing.Process | None = None
         self.passthrough = passthrough
         self.task_status_queue = task_status_queue
         self.tasks = {}
 
         self.outgoing_q: zmq_pipes.TasksOutgoing | None = None
         self.incoming_q: zmq_pipes.ResultsIncoming | None = None
         self.command_client: zmq_pipes.CommandClient | None = None
@@ -534,15 +535,15 @@
                     return
 
                 elif isinstance(msgs, EPStatusReport):
                     log.debug(f"Received {msgs!r}")
                     if self.passthrough:
                         external_ep_status = convert_ep_status_report(msgs)
                         self.results_passthrough.put(
-                            messagepack.pack(external_ep_status)
+                            {"message": messagepack.pack(external_ep_status)}
                         )
 
                 else:
                     log.debug("Unpacking results")
                     for serialized_msg in msgs:
                         try:
                             msg = dill.loads(serialized_msg)
@@ -588,15 +589,19 @@
 
                         if self.passthrough is True:
                             log.debug(f"Pushing results for task:{tid}")
                             # we are only interested in actual task ids here, not
                             # identifiers for other message types
                             sent_task_id = tid if isinstance(tid, str) else None
                             packed_result = self._convert_result_to_outgoing(msg)
-                            self.results_passthrough.put(packed_result)
+                            task_result = {
+                                "task_id": sent_task_id,
+                                "message": packed_result,
+                            }
+                            self.results_passthrough.put(task_result)
                             self.tasks[sent_task_id].set_result(packed_result)
                             continue
 
                         try:
                             task_fut = self.tasks.pop(tid)
                         except KeyError:
                             # This is triggered when the result of a cancelled task is
@@ -700,15 +705,15 @@
         workers = self.command_client.run("MANAGERS")
         log.debug(f"Got managers: {workers}")
         return workers
 
     def _submit(self, func: t.Callable, *args: t.Any, **kwargs: t.Any) -> Future:
         raise RuntimeError("Invalid attempt to _submit()")
 
-    def submit(self, task_id: uuid.UUID, packed_task: bytes) -> HTEXFuture:
+    def submit(self, task_id: str, packed_task: bytes) -> HTEXFuture:
         """Submits a messagepacked.Task for execution
 
         Parameters
         ----------
         Packed Task (messages.Task) - A packed Task object which contains task_id,
         container_id, and serialized fn, args, kwargs packages.
 
@@ -717,20 +722,19 @@
         """
         if self._engine_bad_state.is_set():
             # If the flag is set the exception body must exist
             raise self._engine_exception  # type: ignore
 
         self._task_counter += 1
 
-        task_id_str = str(task_id)
-        future = HTEXFuture(self, task_id_str)
-        self.tasks[task_id_str] = future
+        future = HTEXFuture(self, task_id)
+        self.tasks[task_id] = future
 
         ser = serializer.serialize((execute_task, [task_id, packed_task], {}))
-        payload = Task(task_id_str, "RAW", ser).pack()
+        payload = Task(task_id, "RAW", ser).pack()
         assert self.outgoing_q  # Placate mypy
         self.outgoing_q.put(payload)
 
         return future
 
     def _get_block_and_job_ids(self):
         # Not using self.blocks.keys() and self.blocks.values() simultaneously
@@ -824,24 +828,26 @@
             - block (Bool): To block for confirmations or not
 
         Raises:
              NotImplementedError
         """
 
         log.info("Attempting HighThroughputEngine shutdown")
-        # self.outgoing_q.close()
-        # self.incoming_q.close()
         if self.queue_proc:
             try:
                 self.queue_proc.terminate()
             except AttributeError:
                 log.info("Engine interchange terminate skipped due to wrong context")
             except Exception:
                 log.exception("Terminating the interchange failed")
-        log.info("Finished HighThroughputEngine shutdown attempt")
+            if block:
+                self.queue_proc.join(timeout=5)
+                if self.queue_proc.exitcode is None:
+                    self.queue_proc.kill()
+            log.info("Finished HighThroughputEngine shutdown attempt")
         return True
 
     def cancel_task(self, task_id: uuid.UUID | str) -> bool:
         """
         Attempt to cancel the task `task_id` by requesting cancellation
         from the interchange.  Task cancellation is attempted only if the
         future is cancellable (i.e., not already in a terminal state).  This
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/interchange.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/interchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,15 +672,15 @@
     def stop(self):
         """Prepare the interchange for shutdown"""
         self._kill_event.set()
 
         self._task_puller_thread.join()
         self._command_thread.join()
         self._status_report_thread.join()
-        log.info("HighThroughput Interchange stopped")
+        log.debug("HighThroughput Interchange stopped")
 
     def start(self, poll_period: int | None = None) -> None:
         """Start the Interchange
 
         Parameters:
         ----------
         poll_period : int
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/manager.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
                 last_interchange_contact = time.time()
 
                 if message == "STOP":
                     log.critical("Received stop request")
                     kill_event.set()
                     break
 
-                elif type(message) == tuple and message[0] == "TASK_CANCEL":
+                elif isinstance(message, tuple) and message[0] == "TASK_CANCEL":
                     with self.task_finalization_lock:
                         task_id = message[1]
                         log.info(f"Received TASK_CANCEL request for task: {task_id}")
                         if task_id not in self.task_worker_map:
                             log.warning(f"Task:{task_id} is not in task_worker_map.")
                             log.warning("Possible duplicate cancel or race-condition")
                             continue
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/messages.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/worker.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/worker_map.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import threading
 import time
+import typing as t
 
 log = logging.getLogger(__name__)
 
 
 class BaseStrategy:
     """Implements threshold-interval based flow control.
 
@@ -35,15 +36,15 @@
 
     TODO: When the debug logs are enabled this module emits duplicate messages.
     This issue needs more debugging. What I've learnt so far is that the duplicate
     messages are present only when the timer thread is started, so this could be
     from a duplicate logger being added by the thread.
     """
 
-    def __init__(self, *args, threshold=20, interval=5):
+    def __init__(self, *args, threshold: int = 20, interval: float = 5.0):
         """Initialize the flowcontrol object.
 
         We start the timer thread here
         Parameters
         ----------
         - threshold (int) : Tasks after which the callback is triggered
         - interval (int) : seconds after which timer expires
@@ -53,30 +54,34 @@
         self.threshold = threshold
         self.interval = interval
 
         self.cb_args = args
         self.callback = self.strategize
         self._handle = None
         self._event_count = 0
-        self._event_buffer = []
+        self._event_buffer: t.List[t.Any] = []
         self._wake_up_time = time.time() + 1
         self._kill_event = threading.Event()
-        self._thread = threading.Thread(
-            target=self._wake_up_timer, args=(self._kill_event,), name="Base-Strategy"
-        )
-        self._thread.daemon = True
+        self._thread: t.Optional[threading.Thread] = None
 
     def start(self, interchange):
         """Actually start the strategy
         Parameters
         ----------
         interchange:
          globus_compute_endpoint.executors.high_throughput.interchange.Interchange
             Interchange to bind the strategy to
         """
+        # This thread is created here to ensure a new thread is created whenever start
+        # is called. This is to avoid errors from tests reusing strategy objects which
+        # would attempt to restart stopped threads.
+        self._thread = threading.Thread(
+            target=self._wake_up_timer, args=(self._kill_event,), name="Base-Strategy"
+        )
+        self._thread.daemon = True
         self.interchange = interchange
         if hasattr(interchange, "provider"):
             log.debug(
                 "Strategy bounds-> init:{}, min:{}, max:{}".format(
                     interchange.provider.init_blocks,
                     interchange.provider.min_blocks,
                     interchange.provider.max_blocks,
@@ -109,15 +114,15 @@
                 return
 
             if prev == self._wake_up_time:
                 self.make_callback(kind="timer")
             else:
                 print("Sleeping a bit more")
 
-    def notify(self, event_id):
+    def notify(self, event_id: t.Any):
         """Let the FlowControl system know that there is an event.
 
         This method is to be called from the Interchange to notify the flowcontrol
         """
         self._event_buffer.extend([event_id])
         self._event_count += 1
         if self._event_count >= self.threshold:
@@ -133,16 +138,18 @@
         """
         self._wake_up_time = time.time() + self.interval
         self.callback(tasks=self._event_buffer, kind=kind)
         self._event_buffer = []
 
     def close(self):
         """Merge the threads and terminate."""
+        if self._thread is None:
+            return
         self._kill_event.set()
-        self._thread.join()
+        self._thread.join(timeout=0.1)
 
 
 class Timer:
     """This timer is a simplified version of the FlowControl timer.
     This timer does not employ notify events.
 
     This is based on the following logic :
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,34 @@
 
 log = logging.getLogger(__name__)
 
 
 class SimpleStrategy(BaseStrategy):
     """Implements the simple strategy"""
 
-    def __init__(self, *args, threshold=20, interval=1, max_idletime=60):
+    def __init__(
+        self,
+        *args,
+        threshold: int = 20,
+        interval: float = 1.0,
+        max_idletime: float = 60.0,
+    ):
         """Initialize the flowcontrol object.
 
         We start the timer thread here
 
         Parameters
         ----------
         threshold:(int)
           Tasks after which the callback is triggered
 
-        interval (int)
+        interval (float)
           seconds after which timer expires
 
-        max_idletime: (int)
+        max_idletime: (float)
           maximum idle time(seconds) allowed for resources after which strategy will
           try to kill them.
           default: 60s
 
         """
         log.info("SimpleStrategy Initialized")
         super().__init__(*args, threshold=threshold, interval=interval)
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.4a0"
+__version__ = "2.3.0a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.4a0
+Version: 2.3.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.4a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.3.0a0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 globus_compute_endpoint/__init__.py
 globus_compute_endpoint/cli.py
 globus_compute_endpoint/exception_handling.py
 globus_compute_endpoint/exceptions.py
 globus_compute_endpoint/logging_config.py
+globus_compute_endpoint/self_diagnostic.py
 globus_compute_endpoint/version.py
 globus_compute_endpoint.egg-info/PKG-INFO
 globus_compute_endpoint.egg-info/SOURCES.txt
 globus_compute_endpoint.egg-info/dependency_links.txt
 globus_compute_endpoint.egg-info/entry_points.txt
 globus_compute_endpoint.egg-info/requires.txt
 globus_compute_endpoint.egg-info/top_level.txt
@@ -35,14 +36,15 @@
 globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
 globus_compute_endpoint/endpoint/utils/__init__.py
 globus_compute_endpoint/endpoint/utils/config.py
 globus_compute_endpoint/engines/__init__.py
 globus_compute_endpoint/engines/base.py
 globus_compute_endpoint/engines/globus_compute.py
 globus_compute_endpoint/engines/helper.py
+globus_compute_endpoint/engines/process_pool.py
 globus_compute_endpoint/engines/thread_pool.py
 globus_compute_endpoint/engines/high_throughput/__init__.py
 globus_compute_endpoint/engines/high_throughput/container_sched.py
 globus_compute_endpoint/engines/high_throughput/engine.py
 globus_compute_endpoint/engines/high_throughput/interchange.py
 globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
 globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
```

### Comparing `globus-compute-endpoint-2.2.4a0/setup.py` & `globus-compute-endpoint-2.3.0a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.2.4a0",
+    "globus-compute-sdk==2.3.0a0",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/conftest.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/conftest.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,29 @@
     task_arg = random.randint(1, 1000)
     task_body = ez_pack_function(serializer, double, (task_arg,), {})
     task_message = messagepack.pack(
         messagepack.message_types.Task(
             task_id=task_id, container_id=uuid.uuid1(), task_buffer=task_body
         )
     )
-    future = engine.submit(task_id, task_message)
+    future = engine.submit(str(task_id), task_message)
     packed_result = future.result()
 
     # Confirm that the future got the right answer
     assert isinstance(packed_result, bytes)
     result = messagepack.unpack(packed_result)
     assert isinstance(result, messagepack.message_types.Result)
     assert result.task_id == task_id
 
     # Confirm that the same result got back though the queue
     for _i in range(10):
-        packed_result_q = q.get(timeout=0.1)
-        assert isinstance(
-            packed_result_q, bytes
-        ), "Expected bytes from the passthrough_q"
+        q_msg = q.get(timeout=5)
+        assert isinstance(q_msg, dict)
 
+        packed_result_q = q_msg["message"]
         result = messagepack.unpack(packed_result_q)
         # Handle a sneaky EPStatusReport that popped in ahead of the result
         if isinstance(result, messagepack.message_types.EPStatusReport):
             continue
 
         # At this point the message should be the result
         assert (
```

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_manager.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.4a0/tests/integration/endpoint/executors/mock_executors.py` & `globus-compute-endpoint-2.3.0a0/tests/integration/endpoint/executors/mock_executors.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,8 +27,9 @@
         self.endpoint_id = endpoint_id
         self.run_dir = run_dir
 
     def submit(self, task_id: uuid.UUID, packed_task: bytes):
         task: Task = messagepack.unpack(packed_task)
         res = Result(task_id=task_id, data=task.task_buffer)
         packed_result = messagepack.pack(res)
-        self.results_passthrough.put(packed_result)
+        msg = {"task_id": str(task_id), "message": packed_result}
+        self.results_passthrough.put(msg)
```

### Comparing `globus-compute-endpoint-2.2.4a0/tests/utils.py` & `globus-compute-endpoint-2.3.0a0/tests/utils.py`

 * *Files identical despite different names*

