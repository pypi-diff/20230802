# Comparing `tmp/pyreason-1.8.7.tar.gz` & `tmp/pyreason-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.7.tar", last modified: Wed Jul 26 05:48:44 2023, max compression
+gzip compressed data, was "pyreason-1.8.8.tar", last modified: Wed Aug  2 16:04:05 2023, max compression
```

## Comparing `pyreason-1.8.7.tar` & `pyreason-1.8.8.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-26 05:48:32.000000 pyreason-1.8.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 05:48:32.000000 pyreason-1.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 05:48:44.011128 pyreason-1.8.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-26 05:48:32.000000 pyreason-1.8.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77016 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-26 05:48:44.000000 pyreason-1.8.7/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 05:48:44.011128 pyreason-1.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 05:48:32.000000 pyreason-1.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-26 05:48:32.000000 pyreason-1.8.7/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-08-02 16:03:55.000000 pyreason-1.8.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 16:03:55.000000 pyreason-1.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:04:05.924224 pyreason-1.8.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-08-02 16:03:55.000000 pyreason-1.8.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.908224 pyreason-1.8.8/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.916224 pyreason-1.8.8/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78323 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interpretation/interpretation_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.920224 pyreason-1.8.8/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-08-02 16:03:55.000000 pyreason-1.8.8/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.912224 pyreason-1.8.8/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 16:04:05.000000 pyreason-1.8.8/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:04:05.924224 pyreason-1.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 16:03:55.000000 pyreason-1.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:04:05.924224 pyreason-1.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-02 16:03:55.000000 pyreason-1.8.8/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.7/LICENSE.md` & `pyreason-1.8.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/PKG-INFO` & `pyreason-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.7
+Version: 1.8.8
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.7/README.md` & `pyreason-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/__init__.py` & `pyreason-1.8.8/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.8/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.8/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.8/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/pyreason.py` & `pyreason-1.8.8/pyreason/pyreason.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.8/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/args.py` & `pyreason-1.8.8/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/components/world.py` & `pyreason-1.8.8/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/diffuse.py` & `pyreason-1.8.8/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/facts/fact.py` & `pyreason-1.8.8/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.8/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.8/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.8/pyreason/scripts/interpretation/interpretation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pyreason.scripts.numba_wrapper.numba_types.world_type as world
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
+from pyreason.scripts.interpretation.interpretation_dict import InterpretationDict
 
 import numba
 from numba import objmode, prange
 
 
 # Parallel computing settings
 PARALLEL_COMPUTING = False
@@ -686,14 +687,49 @@
 		# This function is useful for pyreason gym, called externally
 		_add_edge(edge[0], edge[1], self.neighbors, self.reverse_neighbors, self.nodes, self.edges, l, self.interpretations_node, self.interpretations_edge)
 
 	def delete_edge(self, edge):
 		# This function is useful for pyreason gym, called externally
 		_delete_edge(edge, self.neighbors, self.reverse_neighbors, self.edges, self.interpretations_edge)
 
+	def get_interpretation_dict(self):
+		# This function can be called externally to retrieve a dict of the interpretation values
+		# Only values in the rule trace will be added
+
+		# Initialize interpretations for each time and node and edge
+		interpretations = {}
+		for t in range(self.tmax+1):
+			interpretations[t] = {}
+			for node in self.nodes:
+				interpretations[t][node] = InterpretationDict()
+			for edge in self.edges:
+				interpretations[t][edge] = InterpretationDict()
+
+		# Update interpretation nodes
+		for change in self.rule_trace_node:
+			time, _, node, l, bnd = change
+			interpretations[time][node][l._value] = (bnd.lower, bnd.upper)
+
+			# If canonical, update all following timesteps as well
+			if self. canonical:
+				for t in range(time+1, self.tmax+1):
+					interpretations[t][node][l._value] = (bnd.lower, bnd.upper)
+
+		# Update interpretation edges
+		for change in self.rule_trace_edge:
+			time, _, edge, l, bnd, = change
+			interpretations[time][edge][l._value] = (bnd.lower, bnd.upper)
+
+			# If canonical, update all following timesteps as well
+			if self. canonical:
+				for t in range(time+1, self.tmax+1):
+					interpretations[t][edge][l._value] = (bnd.lower, bnd.upper)
+
+		return interpretations
+
 
 @numba.njit(cache=CACHEING, parallel=PARALLEL_COMPUTING)
 def _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip):
 	# Extract rule params
 	rule_type = rule.get_type()
 	clauses = rule.get_clauses()
 	thresholds = rule.get_thresholds()
```

### Comparing `pyreason-1.8.7/pyreason/scripts/interval/interval.py` & `pyreason-1.8.8/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.8/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/program/program.py` & `pyreason-1.8.8/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/rules/rule.py` & `pyreason-1.8.8/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/filter.py` & `pyreason-1.8.8/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.8/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.8/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.8/pyreason/scripts/utils/rule_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.8/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.8/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.7/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.8/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.7
+Version: 1.8.8
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.7/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.8/pyreason.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 pyreason/scripts/components/world.py
 pyreason/scripts/facts/__init__.py
 pyreason/scripts/facts/fact.py
 pyreason/scripts/facts/fact_edge.py
 pyreason/scripts/facts/fact_node.py
 pyreason/scripts/interpretation/__init__.py
 pyreason/scripts/interpretation/interpretation.py
+pyreason/scripts/interpretation/interpretation_dict.py
 pyreason/scripts/interval/__init__.py
 pyreason/scripts/interval/interval.py
 pyreason/scripts/numba_wrapper/__init__.py
 pyreason/scripts/numba_wrapper/numba_types/__init__.py
 pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
 pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
 pyreason/scripts/numba_wrapper/numba_types/interval_type.py
```

### Comparing `pyreason-1.8.7/setup.py` & `pyreason-1.8.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.7',
+    version='1.8.8',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.7/tests/test_hello_world.py` & `pyreason-1.8.8/tests/test_hello_world.py`

 * *Files identical despite different names*

