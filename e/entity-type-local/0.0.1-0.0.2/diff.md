# Comparing `tmp/entity-type-local-0.0.1.tar.gz` & `tmp/entity-type-local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity-type-local-0.0.1.tar", last modified: Wed May 24 02:08:33 2023, max compression
+gzip compressed data, was "entity-type-local-0.0.2.tar", last modified: Wed Aug  2 13:29:42 2023, max compression
```

## Comparing `entity-type-local-0.0.1.tar` & `entity-type-local-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:08:33.492831 entity-type-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 02:08:33.492831 entity-type-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-24 02:08:20.000000 entity-type-local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:08:33.492831 entity-type-local-0.0.1/entity_type_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 02:08:33.000000 entity-type-local-0.0.1/entity_type_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 02:08:33.000000 entity-type-local-0.0.1/entity_type_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:08:33.000000 entity-type-local-0.0.1/entity_type_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:08:33.000000 entity-type-local-0.0.1/entity_type_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:08:33.492831 entity-type-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 02:08:20.000000 entity-type-local-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/entity_type_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:29:42.000000 entity-type-local-0.0.2/entity_type_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:29:42.383643 entity-type-local-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 13:29:11.000000 entity-type-local-0.0.2/tests/test_entity.py
```

### Comparing `entity-type-local-0.0.1/setup.py` & `entity-type-local-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
-     # TODO: Please update the name
      name='entity-type-local',
-     version='0.0.1',
+     version='0.0.2',
      author="Circles",
      author_email="info@circles.life",
-     description="PyPI Package for Circles Local importer Python",
+     description="PyPI Package for Circles Local Entity Type Python (Currently empty package)",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
```

