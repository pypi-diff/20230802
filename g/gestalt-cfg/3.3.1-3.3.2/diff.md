# Comparing `tmp/gestalt-cfg-3.3.1.tar.gz` & `tmp/gestalt-cfg-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gestalt-cfg-3.3.1.tar", last modified: Thu Jul  6 18:37:03 2023, max compression
+gzip compressed data, was "gestalt-cfg-3.3.2.tar", last modified: Wed Aug  2 20:17:18 2023, max compression
```

## Comparing `gestalt-cfg-3.3.1.tar` & `gestalt-cfg-3.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.681786 gestalt-cfg-3.3.1/gestalt/
--rw-r--r--   0 runner    (1001) docker     (123)    25382 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/test_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/gestalt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25382 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/gestalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/gestalt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/gestalt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/gestalt/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-08-02 20:17:18.000000 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 20:17:18.000000 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:17:18.000000 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 20:17:18.000000 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 20:17:18.000000 gestalt-cfg-3.3.2/gestalt_cfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:17:18.712638 gestalt-cfg-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/tests/test_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 20:17:04.000000 gestalt-cfg-3.3.2/tests/test_vault.py
```

### Comparing `gestalt-cfg-3.3.1/LICENSE` & `gestalt-cfg-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/PKG-INFO` & `gestalt-cfg-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.3.1
+Version: 3.3.2
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.3.1/README.md` & `gestalt-cfg-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/gestalt/__init__.py` & `gestalt-cfg-3.3.2/gestalt/__init__.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/gestalt/provider.py` & `gestalt-cfg-3.3.2/gestalt/provider.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/gestalt/utils.py` & `gestalt-cfg-3.3.2/gestalt/utils.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/gestalt/vault.py` & `gestalt-cfg-3.3.2/gestalt/vault.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/gestalt_cfg.egg-info/PKG-INFO` & `gestalt-cfg-3.3.2/gestalt_cfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.3.1
+Version: 3.3.2
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.3.1/setup.py` & `gestalt-cfg-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("requirements.txt") as reqs_file:
     reqs = filter(lambda x: not x.startswith("-"), reqs_file.readlines())
     reqs_list = list(map(lambda x: x.rstrip(), reqs))
 
 setup(name='gestalt-cfg',
-      version='3.3.1',
+      version='3.3.2',
       description='A sensible configuration library for Python',
       long_description=readme(),
       long_description_content_type="text/markdown",
       url='https://github.com/clear-street/gestalt',
       author='Clear Street',
       author_email='engineering@clearstreet.io',
       license='MIT',
```

### Comparing `gestalt-cfg-3.3.1/tests/conftest.py` & `gestalt-cfg-3.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/tests/test_gestalt.py` & `gestalt-cfg-3.3.2/tests/test_gestalt.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.1/tests/test_vault.py` & `gestalt-cfg-3.3.2/tests/test_vault.py`

 * *Files identical despite different names*

