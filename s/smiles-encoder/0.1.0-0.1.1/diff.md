# Comparing `tmp/smiles-encoder-0.1.0.tar.gz` & `tmp/smiles_encoder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smiles-encoder-0.1.0.tar", last modified: Mon Mar 27 01:15:15 2023, max compression
+gzip compressed data, was "smiles_encoder-0.1.1.tar", last modified: Wed Aug  2 20:11:05 2023, max compression
```

## Comparing `smiles-encoder-0.1.0.tar` & `smiles_encoder-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 01:15:15.320876 smiles-encoder-0.1.0/
--rw-rw-rw-   0        0        0     1078 2023-03-27 00:56:44.000000 smiles-encoder-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      450 2023-03-27 01:15:15.319891 smiles-encoder-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       96 2023-03-27 00:56:44.000000 smiles-encoder-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 01:15:15.320876 smiles-encoder-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-03-27 01:13:00.000000 smiles-encoder-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:15:15.308563 smiles-encoder-0.1.0/smiles_encoder/
--rw-rw-rw-   0        0        0       97 2023-03-27 00:59:58.000000 smiles-encoder-0.1.0/smiles_encoder/__init__.py
--rw-rw-rw-   0        0        0     6224 2023-03-27 00:58:38.000000 smiles-encoder-0.1.0/smiles_encoder/encoder.py
--rw-rw-rw-   0        0        0      116 2023-03-27 00:58:40.000000 smiles-encoder-0.1.0/smiles_encoder/version.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:15:15.319225 smiles-encoder-0.1.0/smiles_encoder.egg-info/
--rw-rw-rw-   0        0        0      450 2023-03-27 01:15:15.000000 smiles-encoder-0.1.0/smiles_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-03-27 01:15:15.000000 smiles-encoder-0.1.0/smiles_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 01:15:15.000000 smiles-encoder-0.1.0/smiles_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-27 01:15:15.000000 smiles-encoder-0.1.0/smiles_encoder.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-03-27 01:15:15.000000 smiles-encoder-0.1.0/smiles_encoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:11:05.916015 smiles_encoder-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-02 20:11:05.916015 smiles_encoder-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:11:05.916015 smiles_encoder-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:11:05.916015 smiles_encoder-0.1.1/smiles_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/smiles_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/smiles_encoder/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 20:10:56.000000 smiles_encoder-0.1.1/smiles_encoder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:11:05.916015 smiles_encoder-0.1.1/smiles_encoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-02 20:11:05.000000 smiles_encoder-0.1.1/smiles_encoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-02 20:11:05.000000 smiles_encoder-0.1.1/smiles_encoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:11:05.000000 smiles_encoder-0.1.1/smiles_encoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 20:11:05.000000 smiles_encoder-0.1.1/smiles_encoder.egg-info/top_level.txt
```

### Comparing `smiles-encoder-0.1.0/LICENSE` & `smiles_encoder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smiles-encoder-0.1.0/smiles_encoder/encoder.py` & `smiles_encoder-0.1.1/smiles_encoder/encoder.py`

 * *Files identical despite different names*

