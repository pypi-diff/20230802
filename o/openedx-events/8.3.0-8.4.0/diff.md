# Comparing `tmp/openedx-events-8.3.0.tar.gz` & `tmp/openedx-events-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-8.3.0.tar", last modified: Thu Jul 20 10:08:16 2023, max compression
+gzip compressed data, was "openedx-events-8.4.0.tar", last modified: Wed Aug  2 16:33:46 2023, max compression
```

## Comparing `openedx-events-8.3.0.tar` & `openedx-events-8.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.791386 openedx-events-8.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     9658 2023-07-20 10:08:11.000000 openedx-events-8.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-20 10:08:11.000000 openedx-events-8.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-20 10:08:11.000000 openedx-events-8.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15686 2023-07-20 10:08:16.791386 openedx-events-8.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-07-20 10:08:11.000000 openedx-events-8.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7081 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11516 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    12453 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9087 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15686 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-20 10:08:11.000000 openedx-events-8.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-20 10:08:16.791386 openedx-events-8.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-07-20 10:08:11.000000 openedx-events-8.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-20 10:08:11.000000 openedx-events-8.3.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-08-02 16:33:40.000000 openedx-events-8.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-02 16:33:40.000000 openedx-events-8.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-08-02 16:33:40.000000 openedx-events-8.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-08-02 16:33:46.035698 openedx-events-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-08-02 16:33:40.000000 openedx-events-8.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7081 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11516 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12453 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10470 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7091 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-08-02 16:33:46.000000 openedx-events-8.4.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-02 16:33:40.000000 openedx-events-8.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-02 16:33:46.035698 openedx-events-8.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-08-02 16:33:40.000000 openedx-events-8.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-02 16:33:40.000000 openedx-events-8.4.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-8.3.0/CHANGELOG.rst` & `openedx-events-8.4.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.4.0] - 2023-07-20
+--------------------
+Added
+~~~~~
+* Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
+* Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
+
 [8.3.0] - 2023-07-10
 --------------------
-Changed
-~~~~~~~
+Added
+~~~~~
 * Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
 * Added new COURSE_CREATED event in content_authoring.
 * Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
 * Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
 
 [8.2.0] - 2023-06-08
 --------------------
```

### Comparing `openedx-events-8.3.0/LICENSE.txt` & `openedx-events-8.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/PKG-INFO` & `openedx-events-8.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.3.0
+Version: 8.4.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,18 +206,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.4.0] - 2023-07-20
+--------------------
+Added
+~~~~~
+* Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
+* Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
+
 [8.3.0] - 2023-07-10
 --------------------
-Changed
-~~~~~~~
+Added
+~~~~~
 * Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
 * Added new COURSE_CREATED event in content_authoring.
 * Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
 * Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
 
 [8.2.0] - 2023-06-08
 --------------------
```

### Comparing `openedx-events-8.3.0/README.rst` & `openedx-events-8.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/content_authoring/data.py` & `openedx-events-8.4.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/content_authoring/signals.py` & `openedx-events-8.4.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/data.py` & `openedx-events-8.4.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/__init__.py` & `openedx-events-8.4.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-8.4.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/exceptions.py` & `openedx-events-8.4.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/learning/data.py` & `openedx-events-8.4.0/openedx_events/learning/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -253,7 +253,46 @@
 
     user_ids = attr.ib(type=List[int])
     notification_type = attr.ib(type=str)
     content_url = attr.ib(type=str)
     app_name = attr.ib(type=str)
     course_key = attr.ib(type=CourseKey)
     context = attr.ib(type=dict, factory=dict)
+
+
+@attr.s(frozen=True)
+class ProgramData:
+    """
+    Attributes defined for the Open edX Program data object.
+
+    Arguments:
+        uuid (str): The UUID of the program (from Course-Discovery)
+        title (str): The title of the program
+        program_type (str): The type slug of the program (e.g. professional, microbachelors, micromasters, etc.)
+    """
+
+    uuid = attr.ib(type=str)
+    title = attr.ib(type=str)
+    program_type = attr.ib(type=str)
+
+
+@attr.s(frozen=True)
+class ProgramCertificateData:
+    """
+    Attributes defined for the Open edX Program Certificate data object.
+
+    Arguments:
+        user (UserData): User associated with the Program Certificate
+        program (ProgramData): Program data associated with the Program Certificate
+        uuid (str): UUID of the UserCredential record in Credentials
+        certificate_available_date (datetime): Optional. A DateTime describing when a learner is allowed to view the
+                                                credential
+        status (str): The status of the credential (e.g. `awarded` or `revoked`)
+        url (str): A URL to the learner's credential
+    """
+
+    user = attr.ib(type=UserData)
+    program = attr.ib(type=ProgramData)
+    uuid = attr.ib(type=str)
+    status = attr.ib(type=str)
+    url = attr.ib(type=str)
+    certificate_available_date = attr.ib(type=datetime, default=None)
```

### Comparing `openedx-events-8.3.0/openedx_events/learning/signals.py` & `openedx-events-8.4.0/openedx_events/learning/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from openedx_events.learning.data import (
     CertificateData,
     CohortData,
     CourseDiscussionConfigurationData,
     CourseEnrollmentData,
     PersistentCourseGradeData,
+    ProgramCertificateData,
     UserData,
     UserNotificationData,
     XBlockSkillVerificationData,
 )
 from openedx_events.tooling import OpenEdxPublicSignal
 
 # .. event_type: org.openedx.learning.student.registration.completed.v1
@@ -87,14 +88,24 @@
 CERTIFICATE_CREATED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.certificate.created.v1",
     data={
         "certificate": CertificateData,
     }
 )
 
+# .. event_type: org.openedx.learning.program.certificate.awarded.v1
+# .. event_name: PROGRAM_CERTIFICATE_AWARDED
+# .. event_description: Emit when a program certificate is awarded to a learner
+# .. event_data: ProgramCertificateData
+PROGRAM_CERTIFICATE_AWARDED = OpenEdxPublicSignal(
+    event_type="org.openedx.learning.program.certificate.awarded.v1",
+    data={
+        "program_certificate": ProgramCertificateData,
+    }
+)
 
 # .. event_type: org.openedx.learning.certificate.changed.v1
 # .. event_name: CERTIFICATE_CHANGED
 # .. event_description: emitted when the user's certificate update process is completed.
 # .. event_data: CertificateData
 CERTIFICATE_CHANGED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.certificate.changed.v1",
@@ -111,14 +122,24 @@
 CERTIFICATE_REVOKED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.certificate.revoked.v1",
     data={
         "certificate": CertificateData,
     }
 )
 
+# .. event_type: org.openedx.learning.program.certificate.revoked.v1
+# .. event_name: PROGRAM_CERTIFICATE_REVOKED
+# .. event_description: Emit when a program certificate is revoked from a learner
+# .. event_data: ProgramCertificateData
+PROGRAM_CERTIFICATE_REVOKED = OpenEdxPublicSignal(
+    event_type="org.openedx.learning.program.certificate.revoked.v1",
+    data={
+        "program_certificate": ProgramCertificateData,
+    }
+)
 
 # .. event_type: org.openedx.learning.cohort_membership.changed.v1
 # .. event_name: COHORT_MEMBERSHIP_CHANGED
 # .. event_description: emitted when the user's cohort update is completed.
 # .. event_data: CohortData
 COHORT_MEMBERSHIP_CHANGED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.cohort_membership.changed.v1",
```

### Comparing `openedx-events-8.3.0/openedx_events/management/commands/consume_events.py` & `openedx-events-8.4.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-8.4.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     Schemas will be saved in openedx_events/avro/tests/schemas. The folder will be created if it does not already exist.
     Should only be used for new signals. Even if a schema is changing, it is recommended you leave the original
     in place. Only overwrite the file for an exceptional case, like the schema still being under development.
 
     Example::
 
         # one signal
-        python manage.py cms generate_avro_schemas org.openedx.learning.course.enrollment.changed.v1
+        python manage.py generate_avro_schemas org.openedx.learning.course.enrollment.changed.v1
 
         # multiple signals
-        python manage.py cms generate_avro_schemas org.openedx.learning.course.enrollment.changed.v1 /
+        python manage.py generate_avro_schemas org.openedx.learning.course.enrollment.changed.v1 /
             org.openedx.learning.course.unenrollment.completed.v1
 
         # all signals
-        python manage.py cms generate_avro_schemas --all
+        python manage.py generate_avro_schemas --all
 
     """
 
     def add_arguments(self, parser):
         """
         Add arguments for either individual event types or all of them.
         """
```

### Comparing `openedx-events-8.3.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-8.4.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-8.4.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/tests/test_tooling.py` & `openedx-events-8.4.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/tests/utils.py` & `openedx-events-8.4.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/tooling.py` & `openedx-events-8.4.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events/utils.py` & `openedx-events-8.4.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-8.4.0/openedx_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.3.0
+Version: 8.4.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,18 +206,25 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.4.0] - 2023-07-20
+--------------------
+Added
+~~~~~
+* Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
+* Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
+
 [8.3.0] - 2023-07-10
 --------------------
-Changed
-~~~~~~~
+Added
+~~~~~
 * Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
 * Added new COURSE_CREATED event in content_authoring.
 * Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
 * Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
 
 [8.2.0] - 2023-06-08
 --------------------
```

### Comparing `openedx-events-8.3.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-8.4.0/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.3.0/setup.py` & `openedx-events-8.4.0/setup.py`

 * *Files identical despite different names*

