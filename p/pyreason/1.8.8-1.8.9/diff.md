# Comparing `tmp/pyreason-1.8.8.tar.gz` & `tmp/pyreason-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.8.tar", last modified: Wed Aug  2 16:04:05 2023, max compression
+gzip compressed data, was "pyreason-1.8.9.tar", last modified: Wed Aug  2 16:12:28 2023, max compression
```

## Comparing `pyreason-1.8.8.tar` & `pyreason-1.8.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-08-02 16:03:55.000000 pyreason-1.8.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 16:03:55.000000 pyreason-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:04:05.924224 pyreason-1.8.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-08-02 16:03:55.000000 pyreason-1.8.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.908224 pyreason-1.8.8/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78323 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/interpretation_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:04:05.924224 pyreason-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 16:03:55.000000 pyreason-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-02 16:03:55.000000 pyreason-1.8.8/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-08-02 16:12:15.000000 pyreason-1.8.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 16:12:15.000000 pyreason-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:12:28.534494 pyreason-1.8.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-08-02 16:12:15.000000 pyreason-1.8.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.526495 pyreason-1.8.9/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.526495 pyreason-1.8.9/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32173 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78323 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/interpretation/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/interpretation/interpretation_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.530495 pyreason-1.8.9/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-08-02 16:12:15.000000 pyreason-1.8.9/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.526495 pyreason-1.8.9/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:12:28.000000 pyreason-1.8.9/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 16:12:28.000000 pyreason-1.8.9/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:12:28.000000 pyreason-1.8.9/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 16:12:28.000000 pyreason-1.8.9/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 16:12:28.000000 pyreason-1.8.9/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:12:28.538495 pyreason-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 16:12:15.000000 pyreason-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:12:28.534494 pyreason-1.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-02 16:12:15.000000 pyreason-1.8.9/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.8/LICENSE.md` & `pyreason-1.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/PKG-INFO` & `pyreason-1.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.8
+Version: 1.8.9
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.8/README.md` & `pyreason-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/__init__.py` & `pyreason-1.8.9/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.9/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.9/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.9/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/pyreason.py` & `pyreason-1.8.9/pyreason/pyreason.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # This is the file that will be imported when "import pyreason" is called. All content will be run automatically
 import networkx as nx
 import numba
 import time
 import sys
 import warnings
+import pandas as pd
 import memory_profiler as mp
-from typing import List, Type, Callable
+from typing import List, Type, Callable, Tuple
 
 from pyreason.scripts.utils.output import Output
 from pyreason.scripts.utils.filter import Filter
 from pyreason.scripts.program.program import Program
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
 import pyreason.scripts.utils.rule_parser as rule_parser
@@ -671,28 +672,44 @@
     # Run Program and get final interpretation
     interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, all_node_facts, all_edge_facts, settings.verbose)
 
     return interpretation
 
 
 def save_rule_trace(interpretation, folder: str='./'):
-    """Saves the trace of the program. This includes every change that has occured to the interpretation. If `atom_trace` was set to true
+    """Saves the trace of the program. This includes every change that has occurred to the interpretation. If `atom_trace` was set to true
     this gives us full explainability of why interpretations changed
 
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param folder: the folder in which to save the result, defaults to './'
     """
     global __timestamp, settings
 
     assert settings.store_interpretation_changes, 'store interpretation changes setting is off, turn on to save rule trace'
 
     output = Output(__timestamp)
     output.save_rule_trace(interpretation, folder)
 
 
+def get_rule_trace(interpretation) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    """Returns the trace of the program as 2 pandas dataframes (one for nodes, one for edges).
+    This includes every change that has occurred to the interpretation. If `atom_trace` was set to true
+    this gives us full explainability of why interpretations changed
+
+    :param interpretation: the output of `pyreason.reason()`, the final interpretation
+    :returns two pandas dataframes (nodes, edges) representing the changes that occurred during reasoning
+    """
+    global __timestamp, settings
+
+    assert settings.store_interpretation_changes, 'store interpretation changes setting is off, turn on to save rule trace'
+
+    output = Output(__timestamp)
+    return output.get_rule_trace(interpretation)
+
+
 def filter_and_sort_nodes(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
     """Filters and sorts the node changes in the interpretation and returns as a list of Pandas dataframes that are easy to access
 
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param labels: A list of strings, labels that are in the interpretation that are to be filtered
     :param bound: The bound that will filter any interpretation that is not in it. the default does not filter anything, defaults to interval.closed(0,1)
     :param sort_by: String that is either 'lower' or 'upper', sorts by the lower/upper bound, defaults to 'lower'
```

### Comparing `pyreason-1.8.8/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.9/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/args.py` & `pyreason-1.8.9/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/components/world.py` & `pyreason-1.8.9/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/diffuse.py` & `pyreason-1.8.9/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/facts/fact.py` & `pyreason-1.8.9/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.9/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.9/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.9/pyreason/scripts/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/interpretation/interpretation_dict.py` & `pyreason-1.8.9/pyreason/scripts/interpretation/interpretation_dict.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/interval/interval.py` & `pyreason-1.8.9/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.9/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/program/program.py` & `pyreason-1.8.9/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/rules/rule.py` & `pyreason-1.8.9/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/filter.py` & `pyreason-1.8.9/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.9/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/output.py` & `pyreason-1.8.9/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.9/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.9/pyreason/scripts/utils/rule_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.9/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.9/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.9/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.8
+Version: 1.8.9
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.8/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.9/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.8/setup.py` & `pyreason-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.8',
+    version='1.8.9',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.8/tests/test_hello_world.py` & `pyreason-1.8.9/tests/test_hello_world.py`

 * *Files identical despite different names*

