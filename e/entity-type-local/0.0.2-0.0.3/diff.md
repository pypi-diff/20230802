# Comparing `tmp/entity-type-local-0.0.2.tar.gz` & `tmp/entity-type-local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity-type-local-0.0.2.tar", last modified: Wed Aug  2 13:29:42 2023, max compression
+gzip compressed data, was "entity-type-local-0.0.3.tar", last modified: Wed Aug  2 16:46:31 2023, max compression
```

## Comparing `entity-type-local-0.0.2.tar` & `entity-type-local-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/entity_type_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/tests/test_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/entity_type_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:31.000000 entity-type-local-0.0.3/entity_type_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:31.494531 entity-type-local-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 16:46:12.000000 entity-type-local-0.0.3/tests/test_entity.py
```

### Comparing `entity-type-local-0.0.2/setup.py` & `entity-type-local-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='entity-type-local',
-     version='0.0.2',
+     version='0.0.3',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Entity Type Python (Currently empty package)",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `entity-type-local-0.0.2/tests/test_entity.py` & `entity-type-local-0.0.3/tests/test_entity.py`

 * *Files identical despite different names*

