# Comparing `tmp/logprep-6.7.0.tar.gz` & `tmp/logprep-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.7.0.tar", last modified: Mon Jul 17 09:06:39 2023, max compression
+gzip compressed data, was "logprep-6.8.0.tar", last modified: Wed Aug  2 13:30:17 2023, max compression
```

## Comparing `logprep-6.7.0.tar` & `logprep-6.8.0.tar`

### file list

```diff
@@ -1,537 +1,537 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-17 09:06:25.000000 logprep-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:06:25.000000 logprep-6.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-17 09:06:39.496904 logprep-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-07-17 09:06:25.000000 logprep-6.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 09:06:39.496904 logprep-6.7.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/grok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.436904 logprep-6.7.0/logprep/util/grok/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/aws
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bind
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/exim
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/java
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/maven
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/rails
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/redis
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/squid
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/zeek
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/logprep/util/grok/patterns/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/aws
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bind
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/exim
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/java
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/maven
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mcollective-patterns
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/rails
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/redis
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/squid
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.444904 logprep-6.7.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 09:06:25.000000 logprep-6.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 09:06:39.496904 logprep-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-17 09:06:25.000000 logprep-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_grok_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-07-17 09:06:25.000000 logprep-6.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.024057 logprep-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-02 13:30:11.000000 logprep-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 13:30:11.000000 logprep-6.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-08-02 13:30:17.024057 logprep-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-08-02 13:30:11.000000 logprep-6.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.024057 logprep-6.8.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 13:30:17.024057 logprep-6.8.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.960057 logprep-6.8.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.960057 logprep-6.8.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.964057 logprep-6.8.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.968057 logprep-6.8.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.972057 logprep-6.8.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.976057 logprep-6.8.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.980057 logprep-6.8.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.984057 logprep-6.8.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.984057 logprep-6.8.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.984057 logprep-6.8.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.988057 logprep-6.8.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.988057 logprep-6.8.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.988057 logprep-6.8.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.948057 logprep-6.8.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.992057 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-08-02 13:30:11.000000 logprep-6.8.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.960057 logprep-6.8.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 13:30:16.000000 logprep-6.8.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:30:11.000000 logprep-6.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 13:30:17.024057 logprep-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-02 13:30:11.000000 logprep-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:16.996057 logprep-6.8.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.000058 logprep-6.8.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.000058 logprep-6.8.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.000058 logprep-6.8.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.000058 logprep-6.8.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.004058 logprep-6.8.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.008057 logprep-6.8.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.012057 logprep-6.8.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.016058 logprep-6.8.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.020058 logprep-6.8.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.020058 logprep-6.8.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.020058 logprep-6.8.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.024057 logprep-6.8.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_grok_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:17.024057 logprep-6.8.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-02 13:30:11.000000 logprep-6.8.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-08-02 13:30:11.000000 logprep-6.8.0/versioneer.py
```

### Comparing `logprep-6.7.0/LICENSE` & `logprep-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/PKG-INFO` & `logprep-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.7.0
+Version: 6.8.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -48,15 +48,15 @@
 
 Logprep is primarily designed to process log messages. Generally, Logprep can handle JSON messages,
 allowing further applications besides log handling.
 
 This readme provides basic information about the following topics:
 - [About Logprep](#about-logprep)    
 - [Getting Started](#getting-started)
-- [Docker Quickstart](#docker-quickstart-environment)
+- [Docker Quickstart](#logprep-quickstart-environment)
 - [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 More detailed information can be found in the 
 [Documentation](https://logprep.readthedocs.io/en/latest/).
 
@@ -410,63 +410,66 @@
 This can be useful in case of containerized environments (such as Kubernetes), when pod volumes often change
 on the fly.
 
 If the configuration does not pass a consistency check, then an error message is logged and 
 Logprep keeps running with the previous configuration.
 The configuration should be then checked and corrected on the basis of the error message.
 
-## Docker Quickstart Environment
+## Logprep Quickstart Environment
 
-Logprep was designed to work with the Elastic Stack or Opensearch and Kafka.
-This repository comes with a docker-compose file that builds a pre-configured Elastic Stack with 
-Kafka and Logprep.
-To get it running docker and docker-compose (version >= 1.28) must be first installed.
-The docker-compose file is located in the directory quickstart.
-
-### Running the Test Environment
-
-Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started.
-The environment can either be started with a Logprep container or without one.
-
-#### Running Test Environment without Logprep Container (default way)
-
-  * Run from within the `quickstart` directory: `docker-compose up -d` 
-    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
-  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
-
-#### Running Test Environment with Logprep Container
-
-  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
-    * (maybe needs change of config path in container)
+To demonstrate the functionality of logprep this repo comes with a complete `kafka`, `lokgprep` and
+`opensearch` stack. 
+To get it running `docker` and `docker-compose` (version >= 1.28) must be first installed.
+The docker-compose file is located in the directory `quickstart`.
+A prerequisite is to run `sysctl -w vm.max_map_count=262144`, otherwise Opensearch might not
+properly start.
+
+The environment can either be started with a Logprep container or without one:
+
+### Run without Logprep Container (default)
+
+  1. Run from within the `quickstart` directory: 
+     ```bash
+     docker-compose up -d
+     ```
+     It starts and connects `Kafka`, `logprep`, `Opensearch` and `Opensearch Dashboards`.
+  2. Run Logprep against loaded environment from main `Logprep` directory:
+     ```bash
+     logprep quickstart/exampledata/config/pipeline.yml
+     ```
+
+### Run with Logprep Container
+
+  * Run from within the `quickstart` directory: 
+    ```bash
+    docker-compose --profile logprep up -d
+    ```
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
-
-Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
-address `127.0.0.1:5601`.
-Kafka can be accessed with the console producer and consumer from Kafka with the 
-address `127.0.0.1:9092` or from within the docker container `Kafka`.
-The table below shows which ports have been exposed on localhost for the services.
-
-#### Table of Ports for Services
-
-|          | Kafka | Opensearch    | Dashboards |
-| ---      | ---   | ---           | ---        |
-| **Port** | 9092  | 9200          | 5601       |
+The start up takes a few seconds to complete, but once everything is up
+and running it is possible to write JSON events into Kafka and read the processed events in
+Opensearch Dashboards. Following services are available after start up:
+
+| Service | Location |
+|:----------|:----|
+| Kafka: | `localhost:9092` |
+| Logprep metrics: | `localhost:8000` |
+| Opensearch: | `localhost:9200` |
+| Opensearch Dashboards: | `localhost:5601` |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
-These events can be added to Kafka with the Kafka console producer within the Kafka container by 
-executing the following command:
+These events can be added to Kafka with the following command:
 
-`(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
+```bash
+(docker exec -i kafka kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl
+```
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
 and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.7.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.8.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -27,15 +27,15 @@
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
 the following topics: - [About Logprep](#about-logprep) - [Getting Started]
-(#getting-started) - [Docker Quickstart](#docker-quickstart-environment) -
+(#getting-started) - [Docker Quickstart](#logprep-quickstart-environment) -
 [Documentation](#documentation) - [Contributing](#contributing) - [License]
 (#license) More detailed information can be found in the [Documentation](https:
 //logprep.readthedocs.io/en/latest/). ## About Logprep ### Pipelines Logprep
 processes incoming log messages with a configured pipeline that can be spawned
 multiple times via multiprocessing. The following chart shows a basic setup
 that represents this behaviour. The pipeline consists of three processors: the
 `Dissector`, `Geo-IP Enricher` and the `Dropper`. Each pipeline runs
@@ -176,50 +176,45 @@
 configuration. For this, the signal `SIGUSR1` must be send to the Logprep
 process. Additionally, a `config_refresh_interval` can be set to periodically
 and automatically refresh the given configuration. This can be useful in case
 of containerized environments (such as Kubernetes), when pod volumes often
 change on the fly. If the configuration does not pass a consistency check, then
 an error message is logged and Logprep keeps running with the previous
 configuration. The configuration should be then checked and corrected on the
-basis of the error message. ## Docker Quickstart Environment Logprep was
-designed to work with the Elastic Stack or Opensearch and Kafka. This
-repository comes with a docker-compose file that builds a pre-configured
-Elastic Stack with Kafka and Logprep. To get it running docker and docker-
-compose (version >= 1.28) must be first installed. The docker-compose file is
-located in the directory quickstart. ### Running the Test Environment Before
-running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started. The environment can either be
-started with a Logprep container or without one. #### Running Test Environment
-without Logprep Container (default way) * Run from within the `quickstart`
-directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
-Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
-from main `Logprep` directory: `logprep quickstart/exampledata/config/
-pipeline.yml` #### Running Test Environment with Logprep Container * Run from
-within the `quickstart` directory: `docker-compose --profile logprep up -d` *
-(maybe needs change of config path in container) ### Interacting with the
-Quickstart Environment It is now possible to write JSON events into Kafka and
-read the processed events in Opensearch Dashboards. Once everything has
-started, Opensearch Dashboards can be accessed by a web-browser with the
-address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
-consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
-container `Kafka`. The table below shows which ports have been exposed on
-localhost for the services. #### Table of Ports for Services | | Kafka |
-Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
-5601 | The example rules that are used in the docker instance of Logprep can be
-found in `quickstart/exampledata/rules`. Example events that trigger for the
-example rules can be found in `quickstart/exampledata/input_logdata/
-test_input.jsonl`. These events can be added to Kafka with the Kafka console
-producer within the Kafka container by executing the following command: `
-(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
-test_input.jsonl` Once the events have been processed for the first time, the
-new indices *processed*, *sre* and *pseudonyms* should be available in
-Opensearch Dashboards. The environment can be stopped via `docker-compose
-down`. ## Documentation The documentation for Logprep is online at https://
-logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
-via `pip3 install tox`). Building the documentation is done by executing the
-following command from within the project root directory: ``` tox -e py39-docs
-``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
-Contributing Every contribution is highly appreciated. If you have ideas or
-improvements feel free to create a fork and open a pull requests. Issues and
-engagement in open discussions are also welcome. ## License Logprep is
-distributed under the LGPL-2.1 License. See LICENSE file for more information.
+basis of the error message. ## Logprep Quickstart Environment To demonstrate
+the functionality of logprep this repo comes with a complete `kafka`,
+`lokgprep` and `opensearch` stack. To get it running `docker` and `docker-
+compose` (version >= 1.28) must be first installed. The docker-compose file is
+located in the directory `quickstart`. A prerequisite is to run `sysctl -
+w vm.max_map_count=262144`, otherwise Opensearch might not properly start. The
+environment can either be started with a Logprep container or without one: ###
+Run without Logprep Container (default) 1. Run from within the `quickstart`
+directory: ```bash docker-compose up -d ``` It starts and connects `Kafka`,
+`logprep`, `Opensearch` and `Opensearch Dashboards`. 2. Run Logprep against
+loaded environment from main `Logprep` directory: ```bash logprep quickstart/
+exampledata/config/pipeline.yml ``` ### Run with Logprep Container * Run from
+within the `quickstart` directory: ```bash docker-compose --profile logprep up
+-d ``` ### Interacting with the Quickstart Environment The start up takes a few
+seconds to complete, but once everything is up and running it is possible to
+write JSON events into Kafka and read the processed events in Opensearch
+Dashboards. Following services are available after start up: | Service |
+Location | |:----------|:----| | Kafka: | `localhost:9092` | | Logprep metrics:
+| `localhost:8000` | | Opensearch: | `localhost:9200` | | Opensearch
+Dashboards: | `localhost:5601` | The example rules that are used in the docker
+instance of Logprep can be found in `quickstart/exampledata/rules`. Example
+events that trigger for the example rules can be found in `quickstart/
+exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
+with the following command: ```bash (docker exec -i kafka kafka-console-
+producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
+input_logdata/test_input.jsonl ``` Once the events have been processed for the
+first time, the new indices *processed*, *sre* and *pseudonyms* should be
+available in Opensearch Dashboards. The environment can be stopped via `docker-
+compose down`. ## Documentation The documentation for Logprep is online at
+https://logprep.readthedocs.io/en/latest/ or it can be built locally via tox
+(install via `pip3 install tox`). Building the documentation is done by
+executing the following command from within the project root directory: ``` tox
+-e py39-docs ``` A HTML documentation can be then found in `doc/_build/html/
+index.html`. ## Contributing Every contribution is highly appreciated. If you
+have ideas or improvements feel free to create a fork and open a pull requests.
+Issues and engagement in open discussions are also welcome. ## License Logprep
+is distributed under the LGPL-2.1 License. See LICENSE file for more
+information.
```

### Comparing `logprep-6.7.0/README.md` & `logprep-6.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Logprep is primarily designed to process log messages. Generally, Logprep can handle JSON messages,
 allowing further applications besides log handling.
 
 This readme provides basic information about the following topics:
 - [About Logprep](#about-logprep)    
 - [Getting Started](#getting-started)
-- [Docker Quickstart](#docker-quickstart-environment)
+- [Docker Quickstart](#logprep-quickstart-environment)
 - [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 More detailed information can be found in the 
 [Documentation](https://logprep.readthedocs.io/en/latest/).
 
@@ -391,63 +391,66 @@
 This can be useful in case of containerized environments (such as Kubernetes), when pod volumes often change
 on the fly.
 
 If the configuration does not pass a consistency check, then an error message is logged and 
 Logprep keeps running with the previous configuration.
 The configuration should be then checked and corrected on the basis of the error message.
 
-## Docker Quickstart Environment
+## Logprep Quickstart Environment
 
-Logprep was designed to work with the Elastic Stack or Opensearch and Kafka.
-This repository comes with a docker-compose file that builds a pre-configured Elastic Stack with 
-Kafka and Logprep.
-To get it running docker and docker-compose (version >= 1.28) must be first installed.
-The docker-compose file is located in the directory quickstart.
-
-### Running the Test Environment
-
-Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started.
-The environment can either be started with a Logprep container or without one.
-
-#### Running Test Environment without Logprep Container (default way)
-
-  * Run from within the `quickstart` directory: `docker-compose up -d` 
-    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
-  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
-
-#### Running Test Environment with Logprep Container
-
-  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
-    * (maybe needs change of config path in container)
+To demonstrate the functionality of logprep this repo comes with a complete `kafka`, `lokgprep` and
+`opensearch` stack. 
+To get it running `docker` and `docker-compose` (version >= 1.28) must be first installed.
+The docker-compose file is located in the directory `quickstart`.
+A prerequisite is to run `sysctl -w vm.max_map_count=262144`, otherwise Opensearch might not
+properly start.
+
+The environment can either be started with a Logprep container or without one:
+
+### Run without Logprep Container (default)
+
+  1. Run from within the `quickstart` directory: 
+     ```bash
+     docker-compose up -d
+     ```
+     It starts and connects `Kafka`, `logprep`, `Opensearch` and `Opensearch Dashboards`.
+  2. Run Logprep against loaded environment from main `Logprep` directory:
+     ```bash
+     logprep quickstart/exampledata/config/pipeline.yml
+     ```
+
+### Run with Logprep Container
+
+  * Run from within the `quickstart` directory: 
+    ```bash
+    docker-compose --profile logprep up -d
+    ```
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
-
-Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
-address `127.0.0.1:5601`.
-Kafka can be accessed with the console producer and consumer from Kafka with the 
-address `127.0.0.1:9092` or from within the docker container `Kafka`.
-The table below shows which ports have been exposed on localhost for the services.
-
-#### Table of Ports for Services
-
-|          | Kafka | Opensearch    | Dashboards |
-| ---      | ---   | ---           | ---        |
-| **Port** | 9092  | 9200          | 5601       |
+The start up takes a few seconds to complete, but once everything is up
+and running it is possible to write JSON events into Kafka and read the processed events in
+Opensearch Dashboards. Following services are available after start up:
+
+| Service | Location |
+|:----------|:----|
+| Kafka: | `localhost:9092` |
+| Logprep metrics: | `localhost:8000` |
+| Opensearch: | `localhost:9200` |
+| Opensearch Dashboards: | `localhost:5601` |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
-These events can be added to Kafka with the Kafka console producer within the Kafka container by 
-executing the following command:
+These events can be added to Kafka with the following command:
 
-`(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
+```bash
+(docker exec -i kafka kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl
+```
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
 and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
 the following topics: - [About Logprep](#about-logprep) - [Getting Started]
-(#getting-started) - [Docker Quickstart](#docker-quickstart-environment) -
+(#getting-started) - [Docker Quickstart](#logprep-quickstart-environment) -
 [Documentation](#documentation) - [Contributing](#contributing) - [License]
 (#license) More detailed information can be found in the [Documentation](https:
 //logprep.readthedocs.io/en/latest/). ## About Logprep ### Pipelines Logprep
 processes incoming log messages with a configured pipeline that can be spawned
 multiple times via multiprocessing. The following chart shows a basic setup
 that represents this behaviour. The pipeline consists of three processors: the
 `Dissector`, `Geo-IP Enricher` and the `Dropper`. Each pipeline runs
@@ -166,50 +166,45 @@
 configuration. For this, the signal `SIGUSR1` must be send to the Logprep
 process. Additionally, a `config_refresh_interval` can be set to periodically
 and automatically refresh the given configuration. This can be useful in case
 of containerized environments (such as Kubernetes), when pod volumes often
 change on the fly. If the configuration does not pass a consistency check, then
 an error message is logged and Logprep keeps running with the previous
 configuration. The configuration should be then checked and corrected on the
-basis of the error message. ## Docker Quickstart Environment Logprep was
-designed to work with the Elastic Stack or Opensearch and Kafka. This
-repository comes with a docker-compose file that builds a pre-configured
-Elastic Stack with Kafka and Logprep. To get it running docker and docker-
-compose (version >= 1.28) must be first installed. The docker-compose file is
-located in the directory quickstart. ### Running the Test Environment Before
-running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started. The environment can either be
-started with a Logprep container or without one. #### Running Test Environment
-without Logprep Container (default way) * Run from within the `quickstart`
-directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
-Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
-from main `Logprep` directory: `logprep quickstart/exampledata/config/
-pipeline.yml` #### Running Test Environment with Logprep Container * Run from
-within the `quickstart` directory: `docker-compose --profile logprep up -d` *
-(maybe needs change of config path in container) ### Interacting with the
-Quickstart Environment It is now possible to write JSON events into Kafka and
-read the processed events in Opensearch Dashboards. Once everything has
-started, Opensearch Dashboards can be accessed by a web-browser with the
-address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
-consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
-container `Kafka`. The table below shows which ports have been exposed on
-localhost for the services. #### Table of Ports for Services | | Kafka |
-Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
-5601 | The example rules that are used in the docker instance of Logprep can be
-found in `quickstart/exampledata/rules`. Example events that trigger for the
-example rules can be found in `quickstart/exampledata/input_logdata/
-test_input.jsonl`. These events can be added to Kafka with the Kafka console
-producer within the Kafka container by executing the following command: `
-(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
-test_input.jsonl` Once the events have been processed for the first time, the
-new indices *processed*, *sre* and *pseudonyms* should be available in
-Opensearch Dashboards. The environment can be stopped via `docker-compose
-down`. ## Documentation The documentation for Logprep is online at https://
-logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
-via `pip3 install tox`). Building the documentation is done by executing the
-following command from within the project root directory: ``` tox -e py39-docs
-``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
-Contributing Every contribution is highly appreciated. If you have ideas or
-improvements feel free to create a fork and open a pull requests. Issues and
-engagement in open discussions are also welcome. ## License Logprep is
-distributed under the LGPL-2.1 License. See LICENSE file for more information.
+basis of the error message. ## Logprep Quickstart Environment To demonstrate
+the functionality of logprep this repo comes with a complete `kafka`,
+`lokgprep` and `opensearch` stack. To get it running `docker` and `docker-
+compose` (version >= 1.28) must be first installed. The docker-compose file is
+located in the directory `quickstart`. A prerequisite is to run `sysctl -
+w vm.max_map_count=262144`, otherwise Opensearch might not properly start. The
+environment can either be started with a Logprep container or without one: ###
+Run without Logprep Container (default) 1. Run from within the `quickstart`
+directory: ```bash docker-compose up -d ``` It starts and connects `Kafka`,
+`logprep`, `Opensearch` and `Opensearch Dashboards`. 2. Run Logprep against
+loaded environment from main `Logprep` directory: ```bash logprep quickstart/
+exampledata/config/pipeline.yml ``` ### Run with Logprep Container * Run from
+within the `quickstart` directory: ```bash docker-compose --profile logprep up
+-d ``` ### Interacting with the Quickstart Environment The start up takes a few
+seconds to complete, but once everything is up and running it is possible to
+write JSON events into Kafka and read the processed events in Opensearch
+Dashboards. Following services are available after start up: | Service |
+Location | |:----------|:----| | Kafka: | `localhost:9092` | | Logprep metrics:
+| `localhost:8000` | | Opensearch: | `localhost:9200` | | Opensearch
+Dashboards: | `localhost:5601` | The example rules that are used in the docker
+instance of Logprep can be found in `quickstart/exampledata/rules`. Example
+events that trigger for the example rules can be found in `quickstart/
+exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
+with the following command: ```bash (docker exec -i kafka kafka-console-
+producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
+input_logdata/test_input.jsonl ``` Once the events have been processed for the
+first time, the new indices *processed*, *sre* and *pseudonyms* should be
+available in Opensearch Dashboards. The environment can be stopped via `docker-
+compose down`. ## Documentation The documentation for Logprep is online at
+https://logprep.readthedocs.io/en/latest/ or it can be built locally via tox
+(install via `pip3 install tox`). Building the documentation is done by
+executing the following command from within the project root directory: ``` tox
+-e py39-docs ``` A HTML documentation can be then found in `doc/_build/html/
+index.html`. ## Contributing Every contribution is highly appreciated. If you
+have ideas or improvements feel free to create a fork and open a pull requests.
+Issues and engagement in open discussions are also welcome. ## License Logprep
+is distributed under the LGPL-2.1 License. See LICENSE file for more
+information.
```

### Comparing `logprep-6.7.0/logprep/abc/component.py` & `logprep-6.8.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/abc/connector.py` & `logprep-6.8.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/abc/getter.py` & `logprep-6.8.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/abc/input.py` & `logprep-6.8.0/logprep/abc/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 
     def __init__(self, input_connector: "Input", message, raw_input):
         self.raw_input = raw_input
         input_connector.metrics.number_of_errors += 1
         super().__init__(input_connector, f"{message} -> {raw_input}")
 
 
+class CriticalInputParsingError(CriticalInputError):
+    """The input couldn't be parsed correctly."""
+
+    def __init__(self, input_connector: "Input", message, raw_input):
+        super().__init__(input_connector, message, raw_input)
+
+
 class FatalInputError(InputError):
     """Must not be catched."""
 
     def __init__(self, input_connector: "Input", message: str) -> None:
         input_connector.metrics.number_of_errors += 1
         super().__init__(input_connector, message)
```

### Comparing `logprep-6.7.0/logprep/abc/output.py` & `logprep-6.8.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/abc/processor.py` & `logprep-6.8.0/logprep/abc/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,16 @@
         )
 
     def _apply_rules_wrapper(self, event, rule):
         try:
             self._apply_rules(event, rule)
         except ProcessingWarning as error:
             self._handle_warning_error(event, rule, error)
+        except ProcessingCriticalError as error:
+            raise error
         except BaseException as error:
             raise ProcessingCriticalError(self, str(error), event) from error
         if not hasattr(rule, "delete_source_fields"):
             return
         if rule.delete_source_fields:
             for dotted_field in rule.source_fields:
                 pop_dotted_field_value(event, dotted_field)
```

### Comparing `logprep-6.7.0/logprep/configuration.py` & `logprep-6.8.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.8.0/logprep/connector/confluent_kafka/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from socket import getfqdn
 from typing import Any, List, Optional, Tuple, Union
 
 import msgspec
 from attrs import define, field, validators
 from confluent_kafka import Consumer, KafkaException, TopicPartition
 
-from logprep.abc.input import CriticalInputError, Input
+from logprep.abc.input import CriticalInputError, Input, CriticalInputParsingError
 from logprep.abc.output import FatalOutputError
 from logprep.util.validators import dict_with_keys_validator
 
 
 class ConfluentKafkaInput(Input):
     """A kafka input connector."""
 
@@ -226,19 +226,19 @@
         """
         raw_event = self._get_raw_event(timeout)
         if raw_event is None:
             return None, None
         try:
             event_dict = self._decoder.decode(raw_event)
         except msgspec.DecodeError as error:
-            raise CriticalInputError(
+            raise CriticalInputParsingError(
                 self, "Input record value is not a valid json string", raw_event
             ) from error
         if not isinstance(event_dict, dict):
-            raise CriticalInputError(
+            raise CriticalInputParsingError(
                 self, "Input record value could not be parsed as dict", event_dict
             )
         return event_dict, raw_event
 
     @cached_property
     def _confluent_settings(self) -> dict:
         """Generate confluence settings, mapped from the given kafka logprep configuration.
```

### Comparing `logprep-6.7.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.8.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/console/output.py` & `logprep-6.8.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/dummy/input.py` & `logprep-6.8.0/logprep/connector/dummy/input.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,38 +14,48 @@
     :linenos:
 
     input:
       mydummyinput:
         type: dummy_input
         documents: [{"document":"one"}, "Exception", {"document":"two"}]
 """
-from typing import List, Union
+import copy
+from functools import cached_property
+from typing import List, Union, Optional
 
+from attr import field, validators
 from attrs import define
 
 from logprep.abc.input import Input, SourceDisconnectedError
 
 
 class DummyInput(Input):
     """DummyInput Connector"""
 
     @define(kw_only=True)
     class Config(Input.Config):
         """DummyInput specific configuration"""
 
         documents: List[Union[dict, type, BaseException]]
         """A list of documents that should be returned."""
+        repeat_documents: Optional[str] = field(
+            validator=validators.instance_of(bool), default=False
+        )
+        """If set to :code:`true`, then the given input documents will be repeated after the last
+        one is reached. Default: :code:`False`"""
 
-    @property
+    @cached_property
     def _documents(self):
-        return self._config.documents
+        return copy.copy(self._config.documents)
 
     def _get_event(self, timeout: float) -> tuple:
-        """Retriev next document from configuration and raise error if found"""
+        """Retrieve next document from configuration and raise error if found"""
         if not self._documents:
-            raise SourceDisconnectedError(self, "no documents left")
+            if not self._config.repeat_documents:
+                raise SourceDisconnectedError(self, "no documents left")
+            del self.__dict__["_documents"]
 
         document = self._documents.pop(0)
 
         if (document.__class__ == type) and issubclass(document, BaseException):
             raise document
         return document, None
```

### Comparing `logprep-6.7.0/logprep/connector/dummy/output.py` & `logprep-6.8.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/elasticsearch/output.py` & `logprep-6.8.0/logprep/connector/elasticsearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/file/input.py` & `logprep-6.8.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/http/input.py` & `logprep-6.8.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/jsonl/output.py` & `logprep-6.8.0/logprep/connector/jsonl/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ^^^^^^^
 ..  code-block:: yaml
     :linenos:
 
     output:
       my_jsonl_output:
         type: jsonl_output
-        output_file = path/to/output.file
-        output_file_custom = ""
-        output_file_error = ""
+        output_file: path/to/output.file
+        output_file_custom: ""
+        output_file_error: ""
 """
 
 import json
 from logging import Logger
 
 from attrs import define, field, validators
```

### Comparing `logprep-6.7.0/logprep/connector/opensearch/output.py` & `logprep-6.8.0/logprep/connector/opensearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/connector/s3/output.py` & `logprep-6.8.0/logprep/connector/s3/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/factory.py` & `logprep-6.8.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/factory_error.py` & `logprep-6.8.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/filter/expression/filter_expression.py` & `logprep-6.8.0/logprep/filter/expression/filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/filter/lucene_filter.py` & `logprep-6.8.0/logprep/filter/lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/framework/pipeline.py` & `logprep-6.8.0/logprep/framework/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """This module contains all Pipeline functionality.
 
 Pipelines contain a list of processors that can be executed in order to process input log data.
 They can be multi-processed.
 
 """
+import copy
+
 # pylint: disable=logging-fstring-interpolation
 import queue
 import warnings
-from ctypes import c_bool, c_double, c_ulonglong
+from ctypes import c_bool, c_ulonglong
 from functools import cached_property
 from logging import INFO, NOTSET, Handler, Logger
 from multiprocessing import Lock, Process, Value, current_process
-from time import time
 from typing import Any, List, Tuple
 
 import attrs
 import msgspec
 import numpy as np
+from schedule import Scheduler
 
 from logprep._version import get_versions
 from logprep.abc.component import Component
 from logprep.abc.connector import Connector
 from logprep.abc.input import (
     CriticalInputError,
     FatalInputError,
     Input,
     SourceDisconnectedError,
     WarningInputError,
+    CriticalInputParsingError,
 )
 from logprep.abc.output import (
     CriticalOutputError,
     FatalOutputError,
     Output,
     WarningOutputError,
 )
@@ -55,68 +58,66 @@
 class MustProvideAnMPLogHandlerError(BaseException):
     """Raise if no multiprocessing log handler was provided."""
 
 
 class SharedCounter:
     """A shared counter for multiprocessing pipelines."""
 
-    CHECKING_PERIOD = 0.5
-
     def __init__(self):
         self._val = Value(c_ulonglong, 0)
-        self._lock = Lock()
-        self._timer = Value(c_double, 0)
-        self._checking_timer = 0
+        self._printed = Value(c_bool, False)
+        self._lock = None
         self._logger = None
         self._period = None
+        self.scheduler = Scheduler()
 
     def _init_timer(self, period: float):
         if self._period is None:
             self._period = period
-        with self._lock:
-            self._timer.value = time() + self._period
+        jobs = map(lambda job: job.job_func.func, self.scheduler.jobs)
+        if self.print_value not in jobs and self.reset_printed not in jobs:
+            self.scheduler.every(int(self._period)).seconds.do(self.print_value)
+            self.scheduler.every(int(self._period + 1)).seconds.do(self.reset_printed)
 
     def _create_logger(self, log_handler: Handler):
         if self._logger is None:
             logger = Logger("Processing Counter", level=log_handler.level)
             for handler in logger.handlers:
                 logger.removeHandler(handler)
             logger.addHandler(log_handler)
-
             self._logger = logger
 
-    def setup(self, print_processed_period: float, log_handler: Handler):
+    def setup(self, print_processed_period: float, log_handler: Handler, lock: Lock):
         """Setup shared counter for multiprocessing pipeline."""
         self._create_logger(log_handler)
         self._init_timer(print_processed_period)
-        self._checking_timer = time() + self.CHECKING_PERIOD
+        self._lock = lock
 
     def increment(self):
         """Increment the counter."""
         with self._lock:
             self._val.value += 1
 
-    def print_if_ready(self):
-        """Periodically print the counter and reset it."""
-        current_time = time()
-        if current_time > self._checking_timer:
-            self._checking_timer = current_time + self.CHECKING_PERIOD
-            if self._timer.value != 0 and current_time >= self._timer.value:
-                with self._lock:
-                    if self._period / 60.0 < 1:
-                        msg = f"Processed events per {self._period} seconds: {self._val.value}"
-                    else:
-                        msg = (
-                            f"Processed events per {self._period / 60.0:.2f} minutes: "
-                            f"{self._val.value}"
-                        )
-                    if self._logger:
-                        self._logger.info(msg)
-                    self._val.value = 0
-                    self._timer.value = time() + self._period
+    def reset_printed(self):
+        """Reset the printed flag after the configured period + 1"""
+        with self._lock:
+            self._printed.value = False
+
+    def print_value(self):
+        """Print the number of processed event in the last interval"""
+        with self._lock:
+            if not self._printed.value:
+                period_human_form = f"{self._period} seconds"
+                if self._period / 60.0 > 1:
+                    period_human_form = f"{self._period / 60.0:.2f} minutes"
+                self._logger.info(
+                    f"Processed events per {period_human_form}: " f"{self._val.value}"
+                )
+                self._val.value = 0
+                self._printed.value = True
 
 
 def _handle_pipeline_error(func):
     def _inner(self: "Pipeline") -> Any:
         try:
             return func(self)
         except SourceDisconnectedError as error:
@@ -230,14 +231,17 @@
         self._timeout = config.get("timeout")
         self._log_handler = log_handler
         self._continue_iterating = Value(c_bool)
 
         self._lock = lock
         self._shared_dict = shared_dict
         self._processing_counter = counter
+        if self._processing_counter:
+            print_processed_period = self._logprep_config.get("print_processed_period", 300)
+            self._processing_counter.setup(print_processed_period, log_handler, lock)
         self._used_server_ports = used_server_ports
         self._metric_targets = metric_targets
         self.pipeline_index = pipeline_index
         self._encoder = msgspec.msgpack.Encoder()
         self._decoder = msgspec.msgpack.Decoder()
 
     @cached_property
@@ -383,27 +387,44 @@
 
     @_handle_pipeline_error
     def process_pipeline(self) -> Tuple[dict, list]:
         """Retrieve next event, process event with full pipeline and store or return results"""
         assert self._input, "Run process_pipeline only with an valid input connector"
         self._metrics_exposer.expose(self.metrics)
         Component.run_pending_tasks()
+        if self._processing_counter:
+            self._processing_counter.scheduler.run_pending()
         extra_outputs = []
-        if event := self._get_event():
+        event = None
+        try:
+            event = self._get_event()
+        except CriticalInputParsingError as error:
+            input_data = error.raw_input
+            if isinstance(input_data, bytes):
+                input_data = input_data.decode("utf8")
+            error_event = self._encoder.encode({"invalid_json": input_data})
+            self._store_failed_event(error, "", error_event)
+            self.logger.error(f"{error}, event was written to error output")
+        if event:
             extra_outputs = self.process_event(event)
         if event and self._output:
             self._store_event(event)
         return event, extra_outputs
 
     def _store_event(self, event: dict) -> None:
         for output_name, output in self._output.items():
             if output.default:
                 output.store(event)
                 self.logger.debug(f"Stored output in {output_name}")
 
+    def _store_failed_event(self, error, event, event_received):
+        for _, output in self._output.items():
+            if output.default:
+                output.store_failed(str(error), self._decoder.decode(event_received), event)
+
     def _get_event(self) -> dict:
         event, non_critical_error_msg = self._input.get_next(self._timeout)
         if non_critical_error_msg and self._output:
             for _, output in self._output.items():
                 if output.default:
                     output.store_failed(non_critical_error_msg, event, None)
         try:
@@ -424,24 +445,20 @@
                         self._store_extra_data(extra_data)
                     extra_outputs.append(extra_data)
             except ProcessingWarning as error:
                 self.logger.warning(str(error))
             except ProcessingCriticalError as error:
                 self.logger.error(str(error))
                 if self._output:
-                    for _, output in self._output.items():
-                        if output.default:
-                            output.store_failed(
-                                str(error), self._decoder.decode(event_received), event
-                            )
+                    self._store_failed_event(error, copy.deepcopy(event), event_received)
+                    event.clear()
             if not event:
                 break
         if self._processing_counter:
             self._processing_counter.increment()
-            self._processing_counter.print_if_ready()
         if self.metrics:
             self.metrics.number_of_processed_events += 1
         return extra_outputs
 
     def _store_extra_data(self, extra_data: List[tuple]) -> None:
         self.logger.debug("Storing extra data")
         if isinstance(extra_data, tuple):
@@ -491,16 +508,14 @@
         used_server_ports: dict,
         metric_targets: MetricTargets = None,
     ) -> None:
         if not isinstance(log_handler, MultiprocessingLogHandler):
             raise MustProvideAnMPLogHandlerError
 
         self._profile = config.get("profile_pipelines", False)
-        print_processed_period = config.get("print_processed_period", 300)
-        self.processed_counter.setup(print_processed_period, log_handler)
 
         Pipeline.__init__(
             self,
             pipeline_index=pipeline_index,
             config=config,
             counter=self.processed_counter,
             log_handler=log_handler,
```

### Comparing `logprep-6.7.0/logprep/framework/pipeline_manager.py` & `logprep-6.8.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/framework/rule_tree/node.py` & `logprep-6.8.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.8.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.8.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/metrics/metric.py` & `logprep-6.8.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/metrics/metric_exposer.py` & `logprep-6.8.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/metrics/metric_targets.py` & `logprep-6.8.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/amides/detection.py` & `logprep-6.8.0/logprep/processor/amides/detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/amides/features.py` & `logprep-6.8.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/amides/normalize.py` & `logprep-6.8.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/amides/processor.py` & `logprep-6.8.0/logprep/processor/amides/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/amides/rule.py` & `logprep-6.8.0/logprep/processor/amides/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/base/exceptions.py` & `logprep-6.8.0/logprep/processor/base/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,17 +56,18 @@
         super().__init__(f"{self.__class__.__name__} in {processor.describe()}: {message}")
 
 
 class ProcessingCriticalError(ProcessingError):
     """A critical error occurred - stop processing of this event"""
 
     def __init__(self, processor: "Processor", message: str, event: dict):
-        event.clear()
         processor.metrics.number_of_errors += 1
-        super().__init__(processor, f"{message} -> event was deleted")
+        super().__init__(
+            processor, f"{message} -> event was send to error output and further processing stopped"
+        )
 
 
 class ProcessingWarning(Warning):
     """A minor error occurred - log the error, but continue processing the event."""
 
     def __init__(self, processor: "Processor", message: str, rule: "Rule", event: dict):
         processor.metrics.number_of_warnings += 1
```

### Comparing `logprep-6.7.0/logprep/processor/base/rule.py` & `logprep-6.8.0/logprep/processor/base/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/calculator/fourFn.py` & `logprep-6.8.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/calculator/processor.py` & `logprep-6.8.0/logprep/processor/calculator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/calculator/rule.py` & `logprep-6.8.0/logprep/processor/calculator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/clusterer/processor.py` & `logprep-6.8.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/clusterer/rule.py` & `logprep-6.8.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.8.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/concatenator/processor.py` & `logprep-6.8.0/logprep/processor/concatenator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/concatenator/rule.py` & `logprep-6.8.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.8.0/logprep/processor/datetime_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/datetime_extractor/rule.py` & `logprep-6.8.0/logprep/processor/datetime_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/deleter/processor.py` & `logprep-6.8.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/deleter/rule.py` & `logprep-6.8.0/logprep/processor/deleter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/dissector/processor.py` & `logprep-6.8.0/logprep/processor/dissector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/dissector/rule.py` & `logprep-6.8.0/logprep/processor/dissector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.8.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.8.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.8.0/logprep/processor/domain_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.8.0/logprep/processor/domain_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/dropper/processor.py` & `logprep-6.8.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/dropper/rule.py` & `logprep-6.8.0/logprep/processor/dropper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/field_manager/processor.py` & `logprep-6.8.0/logprep/processor/field_manager/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/field_manager/rule.py` & `logprep-6.8.0/logprep/processor/field_manager/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.8.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/generic_adder/processor.py` & `logprep-6.8.0/logprep/processor/generic_adder/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/generic_adder/rule.py` & `logprep-6.8.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.8.0/logprep/processor/generic_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.8.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.8.0/logprep/processor/geoip_enricher/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.8.0/logprep/processor/geoip_enricher/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/grokker/processor.py` & `logprep-6.8.0/logprep/processor/grokker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/grokker/rule.py` & `logprep-6.8.0/logprep/processor/grokker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.8.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.8.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/ip_informer/processor.py` & `logprep-6.8.0/logprep/processor/ip_informer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/ip_informer/rule.py` & `logprep-6.8.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/key_checker/processor.py` & `logprep-6.8.0/logprep/processor/key_checker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/key_checker/rule.py` & `logprep-6.8.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.8.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/labeler/processor.py` & `logprep-6.8.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/labeler/rule.py` & `logprep-6.8.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/list_comparison/processor.py` & `logprep-6.8.0/logprep/processor/list_comparison/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/list_comparison/rule.py` & `logprep-6.8.0/logprep/processor/list_comparison/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/normalizer/processor.py` & `logprep-6.8.0/logprep/processor/normalizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/normalizer/rule.py` & `logprep-6.8.0/logprep/processor/normalizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.8.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pre_detector/processor.py` & `logprep-6.8.0/logprep/processor/pre_detector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pre_detector/rule.py` & `logprep-6.8.0/logprep/processor/pre_detector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/processor_strategy.py` & `logprep-6.8.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.8.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.8.0/logprep/processor/pseudonymizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.8.0/logprep/processor/pseudonymizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/requester/processor.py` & `logprep-6.8.0/logprep/processor/requester/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/requester/rule.py` & `logprep-6.8.0/logprep/processor/requester/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.8.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.8.0/logprep/processor/selective_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/string_splitter/processor.py` & `logprep-6.8.0/logprep/processor/string_splitter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/string_splitter/rule.py` & `logprep-6.8.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/template_replacer/processor.py` & `logprep-6.8.0/logprep/processor/template_replacer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/template_replacer/rule.py` & `logprep-6.8.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/timestamp_differ/processor.py` & `logprep-6.8.0/logprep/processor/timestamp_differ/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.8.0/logprep/processor/timestamp_differ/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/timestamper/processor.py` & `logprep-6.8.0/logprep/processor/timestamper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/processor/timestamper/rule.py` & `logprep-6.8.0/logprep/processor/timestamper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/registry.py` & `logprep-6.8.0/logprep/registry.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/run_logprep.py` & `logprep-6.8.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/runner.py` & `logprep-6.8.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/aggregating_logger.py` & `logprep-6.8.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.8.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.8.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.8.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/cache.py` & `logprep-6.8.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/configuration.py` & `logprep-6.8.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/decorators.py` & `logprep-6.8.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/getter.py` & `logprep-6.8.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/grok.py` & `logprep-6.8.0/logprep/util/grok/grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/aws` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bacula` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bind` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bind`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bro` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/exim` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/firewalls` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/grok-patterns` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/haproxy` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/httpd` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/java` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/java`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/junos` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/linux-syslog` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mongodb` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/nagios` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/rails` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/squid` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/squid`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/zeek` & `logprep-6.8.0/logprep/util/grok/patterns/ecs-v1/zeek`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/aws` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/bacula` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/bro` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/exim` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/firewalls` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/grok-patterns` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/haproxy` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/httpd` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/java` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/java`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/junos` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/linux-syslog` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/mongodb` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/nagios` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok/patterns/legacy/rails` & `logprep-6.8.0/logprep/util/grok/patterns/legacy/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/grok_pattern_loader.py` & `logprep-6.8.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/hasher.py` & `logprep-6.8.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/helper.py` & `logprep-6.8.0/logprep/util/helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/json_handling.py` & `logprep-6.8.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/log_aggregator.py` & `logprep-6.8.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.8.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/pipeline_profiler.py` & `logprep-6.8.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.8.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/processor_generator.py` & `logprep-6.8.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/prometheus_exporter.py` & `logprep-6.8.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/rule_dry_runner.py` & `logprep-6.8.0/logprep/util/rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.8.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/time.py` & `logprep-6.8.0/logprep/util/time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/time_measurement.py` & `logprep-6.8.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep/util/validators.py` & `logprep-6.8.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/logprep.egg-info/PKG-INFO` & `logprep-6.8.0/logprep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.7.0
+Version: 6.8.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -48,15 +48,15 @@
 
 Logprep is primarily designed to process log messages. Generally, Logprep can handle JSON messages,
 allowing further applications besides log handling.
 
 This readme provides basic information about the following topics:
 - [About Logprep](#about-logprep)    
 - [Getting Started](#getting-started)
-- [Docker Quickstart](#docker-quickstart-environment)
+- [Docker Quickstart](#logprep-quickstart-environment)
 - [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 More detailed information can be found in the 
 [Documentation](https://logprep.readthedocs.io/en/latest/).
 
@@ -410,63 +410,66 @@
 This can be useful in case of containerized environments (such as Kubernetes), when pod volumes often change
 on the fly.
 
 If the configuration does not pass a consistency check, then an error message is logged and 
 Logprep keeps running with the previous configuration.
 The configuration should be then checked and corrected on the basis of the error message.
 
-## Docker Quickstart Environment
+## Logprep Quickstart Environment
 
-Logprep was designed to work with the Elastic Stack or Opensearch and Kafka.
-This repository comes with a docker-compose file that builds a pre-configured Elastic Stack with 
-Kafka and Logprep.
-To get it running docker and docker-compose (version >= 1.28) must be first installed.
-The docker-compose file is located in the directory quickstart.
-
-### Running the Test Environment
-
-Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started.
-The environment can either be started with a Logprep container or without one.
-
-#### Running Test Environment without Logprep Container (default way)
-
-  * Run from within the `quickstart` directory: `docker-compose up -d` 
-    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
-  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
-
-#### Running Test Environment with Logprep Container
-
-  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
-    * (maybe needs change of config path in container)
+To demonstrate the functionality of logprep this repo comes with a complete `kafka`, `lokgprep` and
+`opensearch` stack. 
+To get it running `docker` and `docker-compose` (version >= 1.28) must be first installed.
+The docker-compose file is located in the directory `quickstart`.
+A prerequisite is to run `sysctl -w vm.max_map_count=262144`, otherwise Opensearch might not
+properly start.
+
+The environment can either be started with a Logprep container or without one:
+
+### Run without Logprep Container (default)
+
+  1. Run from within the `quickstart` directory: 
+     ```bash
+     docker-compose up -d
+     ```
+     It starts and connects `Kafka`, `logprep`, `Opensearch` and `Opensearch Dashboards`.
+  2. Run Logprep against loaded environment from main `Logprep` directory:
+     ```bash
+     logprep quickstart/exampledata/config/pipeline.yml
+     ```
+
+### Run with Logprep Container
+
+  * Run from within the `quickstart` directory: 
+    ```bash
+    docker-compose --profile logprep up -d
+    ```
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
-
-Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
-address `127.0.0.1:5601`.
-Kafka can be accessed with the console producer and consumer from Kafka with the 
-address `127.0.0.1:9092` or from within the docker container `Kafka`.
-The table below shows which ports have been exposed on localhost for the services.
-
-#### Table of Ports for Services
-
-|          | Kafka | Opensearch    | Dashboards |
-| ---      | ---   | ---           | ---        |
-| **Port** | 9092  | 9200          | 5601       |
+The start up takes a few seconds to complete, but once everything is up
+and running it is possible to write JSON events into Kafka and read the processed events in
+Opensearch Dashboards. Following services are available after start up:
+
+| Service | Location |
+|:----------|:----|
+| Kafka: | `localhost:9092` |
+| Logprep metrics: | `localhost:8000` |
+| Opensearch: | `localhost:9200` |
+| Opensearch Dashboards: | `localhost:5601` |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
-These events can be added to Kafka with the Kafka console producer within the Kafka container by 
-executing the following command:
+These events can be added to Kafka with the following command:
 
-`(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
+```bash
+(docker exec -i kafka kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl
+```
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
 and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.7.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.8.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -27,15 +27,15 @@
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
 the following topics: - [About Logprep](#about-logprep) - [Getting Started]
-(#getting-started) - [Docker Quickstart](#docker-quickstart-environment) -
+(#getting-started) - [Docker Quickstart](#logprep-quickstart-environment) -
 [Documentation](#documentation) - [Contributing](#contributing) - [License]
 (#license) More detailed information can be found in the [Documentation](https:
 //logprep.readthedocs.io/en/latest/). ## About Logprep ### Pipelines Logprep
 processes incoming log messages with a configured pipeline that can be spawned
 multiple times via multiprocessing. The following chart shows a basic setup
 that represents this behaviour. The pipeline consists of three processors: the
 `Dissector`, `Geo-IP Enricher` and the `Dropper`. Each pipeline runs
@@ -176,50 +176,45 @@
 configuration. For this, the signal `SIGUSR1` must be send to the Logprep
 process. Additionally, a `config_refresh_interval` can be set to periodically
 and automatically refresh the given configuration. This can be useful in case
 of containerized environments (such as Kubernetes), when pod volumes often
 change on the fly. If the configuration does not pass a consistency check, then
 an error message is logged and Logprep keeps running with the previous
 configuration. The configuration should be then checked and corrected on the
-basis of the error message. ## Docker Quickstart Environment Logprep was
-designed to work with the Elastic Stack or Opensearch and Kafka. This
-repository comes with a docker-compose file that builds a pre-configured
-Elastic Stack with Kafka and Logprep. To get it running docker and docker-
-compose (version >= 1.28) must be first installed. The docker-compose file is
-located in the directory quickstart. ### Running the Test Environment Before
-running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Opensearch is not properly started. The environment can either be
-started with a Logprep container or without one. #### Running Test Environment
-without Logprep Container (default way) * Run from within the `quickstart`
-directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
-Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
-from main `Logprep` directory: `logprep quickstart/exampledata/config/
-pipeline.yml` #### Running Test Environment with Logprep Container * Run from
-within the `quickstart` directory: `docker-compose --profile logprep up -d` *
-(maybe needs change of config path in container) ### Interacting with the
-Quickstart Environment It is now possible to write JSON events into Kafka and
-read the processed events in Opensearch Dashboards. Once everything has
-started, Opensearch Dashboards can be accessed by a web-browser with the
-address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
-consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
-container `Kafka`. The table below shows which ports have been exposed on
-localhost for the services. #### Table of Ports for Services | | Kafka |
-Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
-5601 | The example rules that are used in the docker instance of Logprep can be
-found in `quickstart/exampledata/rules`. Example events that trigger for the
-example rules can be found in `quickstart/exampledata/input_logdata/
-test_input.jsonl`. These events can be added to Kafka with the Kafka console
-producer within the Kafka container by executing the following command: `
-(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
-test_input.jsonl` Once the events have been processed for the first time, the
-new indices *processed*, *sre* and *pseudonyms* should be available in
-Opensearch Dashboards. The environment can be stopped via `docker-compose
-down`. ## Documentation The documentation for Logprep is online at https://
-logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
-via `pip3 install tox`). Building the documentation is done by executing the
-following command from within the project root directory: ``` tox -e py39-docs
-``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
-Contributing Every contribution is highly appreciated. If you have ideas or
-improvements feel free to create a fork and open a pull requests. Issues and
-engagement in open discussions are also welcome. ## License Logprep is
-distributed under the LGPL-2.1 License. See LICENSE file for more information.
+basis of the error message. ## Logprep Quickstart Environment To demonstrate
+the functionality of logprep this repo comes with a complete `kafka`,
+`lokgprep` and `opensearch` stack. To get it running `docker` and `docker-
+compose` (version >= 1.28) must be first installed. The docker-compose file is
+located in the directory `quickstart`. A prerequisite is to run `sysctl -
+w vm.max_map_count=262144`, otherwise Opensearch might not properly start. The
+environment can either be started with a Logprep container or without one: ###
+Run without Logprep Container (default) 1. Run from within the `quickstart`
+directory: ```bash docker-compose up -d ``` It starts and connects `Kafka`,
+`logprep`, `Opensearch` and `Opensearch Dashboards`. 2. Run Logprep against
+loaded environment from main `Logprep` directory: ```bash logprep quickstart/
+exampledata/config/pipeline.yml ``` ### Run with Logprep Container * Run from
+within the `quickstart` directory: ```bash docker-compose --profile logprep up
+-d ``` ### Interacting with the Quickstart Environment The start up takes a few
+seconds to complete, but once everything is up and running it is possible to
+write JSON events into Kafka and read the processed events in Opensearch
+Dashboards. Following services are available after start up: | Service |
+Location | |:----------|:----| | Kafka: | `localhost:9092` | | Logprep metrics:
+| `localhost:8000` | | Opensearch: | `localhost:9200` | | Opensearch
+Dashboards: | `localhost:5601` | The example rules that are used in the docker
+instance of Logprep can be found in `quickstart/exampledata/rules`. Example
+events that trigger for the example rules can be found in `quickstart/
+exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
+with the following command: ```bash (docker exec -i kafka kafka-console-
+producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
+input_logdata/test_input.jsonl ``` Once the events have been processed for the
+first time, the new indices *processed*, *sre* and *pseudonyms* should be
+available in Opensearch Dashboards. The environment can be stopped via `docker-
+compose down`. ## Documentation The documentation for Logprep is online at
+https://logprep.readthedocs.io/en/latest/ or it can be built locally via tox
+(install via `pip3 install tox`). Building the documentation is done by
+executing the following command from within the project root directory: ``` tox
+-e py39-docs ``` A HTML documentation can be then found in `doc/_build/html/
+index.html`. ## Contributing Every contribution is highly appreciated. If you
+have ideas or improvements feel free to create a fork and open a pull requests.
+Issues and engagement in open discussions are also welcome. ## License Logprep
+is distributed under the LGPL-2.1 License. See LICENSE file for more
+information.
```

### Comparing `logprep-6.7.0/logprep.egg-info/SOURCES.txt` & `logprep-6.8.0/logprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/setup.py` & `logprep-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_amides.py` & `logprep-6.8.0/tests/acceptance/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_config_refresh.py` & `logprep-6.8.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_file_input.py` & `logprep-6.8.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_full_configuration.py` & `logprep-6.8.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_http_input.py` & `logprep-6.8.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.8.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_pre_detection.py` & `logprep-6.8.0/tests/acceptance/test_pre_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_preprocessing.py` & `logprep-6.8.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.8.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.8.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.8.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.8.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/acceptance/util.py` & `logprep-6.8.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.8.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.8.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/testdata/FilledTempFile.py` & `logprep-6.8.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/testdata/metadata.py` & `logprep-6.8.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/testdata/ruledata.py` & `logprep-6.8.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.8.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/component/base.py` & `logprep-6.8.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/base.py` & `logprep-6.8.0/tests/unit/connector/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.8.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.8.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=no-self-use
 from copy import deepcopy
 from unittest import mock
 
 import pytest
 
-from logprep.abc.input import CriticalInputError
+from logprep.abc.input import CriticalInputError, CriticalInputParsingError
 from logprep.abc.output import FatalOutputError
 from logprep.factory import Factory
 from tests.unit.connector.base import BaseInputTestCase
 from tests.unit.connector.test_confluent_kafka_common import (
     CommonConfluentKafkaTestCase,
 )
 
@@ -153,7 +153,13 @@
         mock_consumer.assert_called_with(kafka_config)
 
     def test_setup_raises_fatal_output_error_on_invalid_config(self):
         config = {"myconfig": "the config"}
         self.object._config.kafka_config = config
         with pytest.raises(FatalOutputError, match="No such configuration property"):
             self.object.setup()
+
+    def test_get_next_raises_critical_input_parsing_error(self):
+        return_value = b'{"invalid": "json'
+        self.object._get_raw_event = mock.MagicMock(return_value=return_value)
+        with pytest.raises(CriticalInputParsingError, match="is not a valid json"):
+            self.object.get_next(0.01)
```

### Comparing `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.8.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_console_output.py` & `logprep-6.8.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.8.0/tests/unit/connector/test_dummy_input.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # pylint: disable=missing-docstring
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=protected-access
+import copy
+
 from pytest import raises
 
 from logprep.abc.input import SourceDisconnectedError
+from logprep.factory import Factory
 from tests.unit.connector.base import BaseInputTestCase
 
 
 class DummyError(BaseException):
     pass
 
 
@@ -35,7 +38,17 @@
         event, _ = self.object.get_next(self.timeout)
         assert event.get("order") == 1
 
     def test_raises_exceptions_instead_of_returning_them(self):
         self.object._config.documents = [BaseException]
         with raises(BaseException):
             self.object.get_next(self.timeout)
+
+    def test_repeat_documents_repeats_documents(self):
+        config = copy.deepcopy(self.CONFIG)
+        config["repeat_documents"] = True
+        object = Factory.create(configuration={"Test Instance Name": config}, logger=self.logger)
+        object._config.documents = [{"order": 0}, {"order": 1}, {"order": 2}]
+
+        for order in range(0, 9):
+            event, _ = object.get_next(self.timeout)
+            assert event.get("order") == order % 3
```

### Comparing `logprep-6.7.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.8.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.8.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.8.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.8.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.8.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_http_input.py` & `logprep-6.8.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_json_input.py` & `logprep-6.8.0/tests/unit/connector/test_jsonl_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # pylint: disable=missing-docstring
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=protected-access
+import copy
 from unittest import mock
 
 import pytest
+
 from logprep.abc.input import CriticalInputError
+from logprep.factory import Factory
 from tests.unit.connector.base import BaseInputTestCase
 
 
-class DummyError(BaseException):
-    pass
-
-
-class TestJsonInput(BaseInputTestCase):
+class TestJsonlInput(BaseInputTestCase):
     timeout = 0.1
 
-    CONFIG = {"type": "json_input", "documents_path": "/does/not/matter"}
+    CONFIG = {"type": "jsonl_input", "documents_path": "/does/not/matter"}
 
-    parse_function = "logprep.connector.json.input.parse_json"
+    parse_function = "logprep.connector.jsonl.input.parse_jsonl"
 
     @mock.patch(parse_function)
     def test_documents_returns(self, mock_parse):
         return_value = [{"message": "test_message"}]
         mock_parse.return_value = return_value
         assert self.object._documents == return_value
 
@@ -31,25 +30,34 @@
         expected = {"message": "test_message"}
         document, _ = self.object.get_next(self.timeout)
         assert document == expected
 
     @mock.patch(parse_function)
     def test_get_next_returns_multiple_documents(self, mock_parse):
         mock_parse.return_value = [{"order": 0}, {"order": 1}]
-        event, _ = self.object.get_next(self.timeout)
-        assert {"order": 0} == event
-        event, _ = self.object.get_next(self.timeout)
-        assert {"order": 1} == event
+        assert ({"order": 0}, None) == self.object.get_next(self.timeout)
+        assert ({"order": 1}, None) == self.object.get_next(self.timeout)
 
     @mock.patch(parse_function)
     def test_raises_exception_if_not_a_dict(self, mock_parse):
         mock_parse.return_value = ["no dict"]
         with pytest.raises(CriticalInputError, match=r"not a dict"):
-            _, _ = self.object.get_next(self.timeout)
+            _ = self.object.get_next(self.timeout)
 
     @mock.patch(parse_function)
     def test_raises_exception_if_one_element_is_not_a_dict(self, mock_parse):
         mock_parse.return_value = [{"order": 0}, "not a dict", {"order": 1}]
         with pytest.raises(CriticalInputError, match=r"not a dict"):
-            _, _ = self.object.get_next(self.timeout)
-            _, _ = self.object.get_next(self.timeout)
-            _, _ = self.object.get_next(self.timeout)
+            _ = self.object.get_next(self.timeout)
+            _ = self.object.get_next(self.timeout)
+            _ = self.object.get_next(self.timeout)
+
+    @mock.patch(parse_function)
+    def test_repeat_documents_repeats_documents(self, mock_parse):
+        config = copy.deepcopy(self.CONFIG)
+        config["repeat_documents"] = True
+        mock_parse.return_value = [{"order": 0}, {"order": 1}, {"order": 2}]
+        object = Factory.create(configuration={"Test Instance Name": config}, logger=self.logger)
+
+        for order in range(0, 9):
+            event, _ = object.get_next(self.timeout)
+            assert event.get("order") == order % 3
```

### Comparing `logprep-6.7.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.8.0/tests/unit/connector/test_json_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # pylint: disable=missing-docstring
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=protected-access
+import copy
 from unittest import mock
 
 import pytest
+
 from logprep.abc.input import CriticalInputError
+from logprep.factory import Factory
 from tests.unit.connector.base import BaseInputTestCase
 
 
-class TestJsonlInput(BaseInputTestCase):
+class DummyError(BaseException):
+    pass
+
+
+class TestJsonInput(BaseInputTestCase):
     timeout = 0.1
 
-    CONFIG = {"type": "jsonl_input", "documents_path": "/does/not/matter"}
+    CONFIG = {"type": "json_input", "documents_path": "/does/not/matter"}
 
-    parse_function = "logprep.connector.jsonl.input.parse_jsonl"
+    parse_function = "logprep.connector.json.input.parse_json"
 
     @mock.patch(parse_function)
     def test_documents_returns(self, mock_parse):
         return_value = [{"message": "test_message"}]
         mock_parse.return_value = return_value
         assert self.object._documents == return_value
 
@@ -27,23 +34,36 @@
         expected = {"message": "test_message"}
         document, _ = self.object.get_next(self.timeout)
         assert document == expected
 
     @mock.patch(parse_function)
     def test_get_next_returns_multiple_documents(self, mock_parse):
         mock_parse.return_value = [{"order": 0}, {"order": 1}]
-        assert ({"order": 0}, None) == self.object.get_next(self.timeout)
-        assert ({"order": 1}, None) == self.object.get_next(self.timeout)
+        event, _ = self.object.get_next(self.timeout)
+        assert {"order": 0} == event
+        event, _ = self.object.get_next(self.timeout)
+        assert {"order": 1} == event
 
     @mock.patch(parse_function)
     def test_raises_exception_if_not_a_dict(self, mock_parse):
         mock_parse.return_value = ["no dict"]
         with pytest.raises(CriticalInputError, match=r"not a dict"):
-            _ = self.object.get_next(self.timeout)
+            _, _ = self.object.get_next(self.timeout)
 
     @mock.patch(parse_function)
     def test_raises_exception_if_one_element_is_not_a_dict(self, mock_parse):
         mock_parse.return_value = [{"order": 0}, "not a dict", {"order": 1}]
         with pytest.raises(CriticalInputError, match=r"not a dict"):
-            _ = self.object.get_next(self.timeout)
-            _ = self.object.get_next(self.timeout)
-            _ = self.object.get_next(self.timeout)
+            _, _ = self.object.get_next(self.timeout)
+            _, _ = self.object.get_next(self.timeout)
+            _, _ = self.object.get_next(self.timeout)
+
+    @mock.patch(parse_function)
+    def test_repeat_documents_repeats_documents(self, mock_parse):
+        config = copy.deepcopy(self.CONFIG)
+        config["repeat_documents"] = True
+        mock_parse.return_value = [{"order": 0}, {"order": 1}, {"order": 2}]
+        object = Factory.create(configuration={"Test Instance Name": config}, logger=self.logger)
+
+        for order in range(0, 9):
+            event, _ = object.get_next(self.timeout)
+            assert event.get("order") == order % 3
```

### Comparing `logprep-6.7.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.8.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.8.0/tests/unit/connector/test_opensearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/connector/test_s3_output.py` & `logprep-6.8.0/tests/unit/connector/test_s3_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.8.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.8.0/tests/unit/filter/test_filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/filter/test_lucene_filter.py` & `logprep-6.8.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.8.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.8.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.8.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/framework/test_pipeline.py` & `logprep-6.8.0/tests/unit/framework/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=attribute-defined-outside-init
+import logging
+import re
+import time
 from copy import deepcopy
 from logging import DEBUG, WARNING, getLogger
 from multiprocessing import Lock, active_children
 from unittest import mock
 
 import pytest
 import requests
@@ -12,14 +15,15 @@
 from _pytest.python_api import raises
 
 from logprep.abc.input import (
     CriticalInputError,
     FatalInputError,
     SourceDisconnectedError,
     WarningInputError,
+    CriticalInputParsingError,
 )
 from logprep.abc.output import (
     CriticalOutputError,
     FatalOutputError,
     Output,
     WarningOutputError,
 )
@@ -31,15 +35,14 @@
     MustProvideAnMPLogHandlerError,
     Pipeline,
     SharedCounter,
 )
 from logprep.metrics.metric import MetricTargets
 from logprep.processor.base.exceptions import (
     ProcessingCriticalError,
-    ProcessingError,
     ProcessingWarning,
 )
 from logprep.processor.deleter.rule import DeleterRule
 from logprep.util.getter import GetterFactory
 from logprep.util.multiprocessing_log_handler import MultiprocessingLogHandler
 
 original_create = Factory.create
@@ -147,15 +150,15 @@
             {"filter": "delete_me", "deleter": {"delete": True}}
         )
         deleter_processor._specific_tree.add_rule(deleter_rule)
         self.pipeline._pipeline = [mock.MagicMock(), deleter_processor, mock.MagicMock()]
         self.pipeline.logger.setLevel(DEBUG)
         while self.pipeline._input._documents:
             self.pipeline.process_pipeline()
-        assert len(input_data) == 0, "all events were processed"
+        assert len(self.pipeline._input._documents) == 0, "all events were processed"
         assert self.pipeline._pipeline[0].process.call_count == 3, "called for all events"
         assert self.pipeline._pipeline[2].process.call_count == 2, "not called for deleted event"
         assert {"delete_me": "2"} not in self.pipeline._output["dummy"].events
         assert len(self.pipeline._output["dummy"].events) == 2
 
     def test_not_empty_documents_are_stored_in_the_output(self, _):
         self.pipeline._setup()
@@ -315,15 +318,15 @@
             )
 
         self.pipeline._pipeline[1].process.side_effect = raise_critical_processing_error
         self.pipeline.process_pipeline()
         self.pipeline._input.get_next.return_value = (input_event2, None)
         self.pipeline.process_pipeline()
         assert self.pipeline._input.get_next.call_count == 2, "2 events gone into processing"
-        assert mock_error.call_count == 2, "two errors occured"
+        assert mock_error.call_count == 2, "two errors occurred"
         mock_error.assert_called_with(
             str(
                 ProcessingCriticalError(
                     self.pipeline._pipeline[1], "really bad things happened", input_event1
                 )
             )
         )
@@ -674,14 +677,30 @@
         self.pipeline._store_event = mock.MagicMock()
         self.pipeline.process_event = mock.MagicMock()
         output["dummy"]._schedule_task(task=mock_task, seconds=30)
         with mock.patch("schedule.Job.should_run", return_value=True):
             self.pipeline.process_pipeline()
         mock_task.assert_called()
 
+    def test_event_with_critical_input_parsing_error_is_stored_in_error_output(self, _):
+        self.pipeline._setup()
+        error = CriticalInputParsingError(self.pipeline._input, "test-error", "raw_input")
+        self.pipeline._input.get_next = mock.MagicMock()
+        self.pipeline._input.get_next.side_effect = error
+        self.pipeline._output = {"dummy": mock.MagicMock()}
+        self.pipeline.process_pipeline()
+        self.pipeline._output["dummy"].store_failed.assert_called()
+
+    def test_process_pipeline_calls_shared_counter_scheduler(self, _):
+        self.pipeline._setup()
+        self.pipeline._input.get_next.return_value = ({}, {})
+        self.pipeline._processing_counter = mock.MagicMock()
+        self.pipeline.process_pipeline()
+        assert self.pipeline._processing_counter.scheduler.run_pending.call_count == 1
+
 
 class TestPipelineWithActualInput:
     def setup_method(self):
         self.config = GetterFactory.from_string("tests/testdata/config/config.yml").get_yaml()
         del self.config["output"]
         self.config["process_count"] = 1
         self.config["input"] = {
@@ -907,7 +926,28 @@
         wrapper.start()
         children_running = active_children()
 
         wrapper.stop()
         wrapper.join()
 
         return children_running
+
+
+class TestSharedCounter:
+    test_logger = getLogger("test-logger")
+
+    def test_shared_counter_prints_value_after_configured_period(self, caplog):
+        with caplog.at_level(logging.INFO):
+            shared_counter = SharedCounter()
+            print_period = 1
+            shared_counter._logger = self.test_logger
+            shared_counter.setup(print_period, None, Lock())
+            test_counter = 0
+            test_counter_limit = 100
+            start_time = time.time()
+            while time.time() - start_time < print_period:
+                if test_counter < test_counter_limit:
+                    shared_counter.increment()
+                    test_counter += 1
+                shared_counter.scheduler.run_pending()
+            message = f".*Processed events per {print_period} seconds: {test_counter_limit}.*"
+            assert re.match(message, caplog.text)
```

### Comparing `logprep-6.7.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.8.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.8.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.8.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/metrics/test_metrics.py` & `logprep-6.8.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/amides/test_amides.py` & `logprep-6.8.0/tests/unit/processor/amides/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.8.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/amides/test_detection.py` & `logprep-6.8.0/tests/unit/processor/amides/test_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/amides/test_normalize.py` & `logprep-6.8.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.8.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/base.py` & `logprep-6.8.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.8.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.8.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.8.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.8.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.8.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.8.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.8.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.8.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.8.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.8.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.8.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.8.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.8.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.8.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.8.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.8.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.8.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.8.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.8.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.8.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.8.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.8.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.8.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.8.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.8.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/grokker/test_grok.py` & `logprep-6.8.0/tests/unit/processor/grokker/test_grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.8.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.8.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.8.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.8.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.8.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.8.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.8.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.8.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.8.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.8.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.8.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.8.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.8.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.8.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.8.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.8.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.8.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.8.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.8.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.8.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.8.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.8.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.8.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.8.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.8.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.8.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.8.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/test_processor_strategy.py` & `logprep-6.8.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.8.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.8.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper.py` & `logprep-6.8.0/tests/unit/processor/timestamper/test_timestamper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper_rule.py` & `logprep-6.8.0/tests/unit/processor/timestamper/test_timestamper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/test_configuration.py` & `logprep-6.8.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/test_factory.py` & `logprep-6.8.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/test_run_logprep.py` & `logprep-6.8.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/test_runner.py` & `logprep-6.8.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.8.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.8.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_cache.py` & `logprep-6.8.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_configuration.py` & `logprep-6.8.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_getter.py` & `logprep-6.8.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_grok_pattern.py` & `logprep-6.8.0/tests/unit/util/test_grok_pattern.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.8.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_helper.py` & `logprep-6.8.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.8.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.8.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_processor_generator.py` & `logprep-6.8.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.8.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.8.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_time.py` & `logprep-6.8.0/tests/unit/util/test_time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_time_measurement.py` & `logprep-6.8.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/test_validators.py` & `logprep-6.8.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/unit/util/tests_json_handling.py` & `logprep-6.8.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/tests/util/testhelpers.py` & `logprep-6.8.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.7.0/versioneer.py` & `logprep-6.8.0/versioneer.py`

 * *Files identical despite different names*

