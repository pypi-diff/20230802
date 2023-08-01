# Comparing `tmp/ethpwn-pyevmasm-0.2.4.tar.gz` & `tmp/ethpwn-pyevmasm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpwn-pyevmasm-0.2.4.tar", last modified: Mon Jul 31 17:51:28 2023, max compression
+gzip compressed data, was "ethpwn-pyevmasm-0.2.5.tar", last modified: Tue Aug  1 22:49:34 2023, max compression
```

## Comparing `ethpwn-pyevmasm-0.2.4.tar` & `ethpwn-pyevmasm-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)    11357 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/LICENSE
--rw-rw-r--   0 honululu  (1000) honululu  (1000)      328 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/PKG-INFO
--rw-rw-r--   0 honululu  (1000) honululu  (1000)     3045 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/README.md
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)      328 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/PKG-INFO
--rw-rw-r--   0 honululu  (1000) honululu  (1000)      350 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/SOURCES.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/dependency_links.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)       50 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/entry_points.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)       35 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/requires.txt
--rw-rw-r--   0 honululu  (1000) honululu  (1000)        9 2023-07-31 17:51:28.000000 ethpwn-pyevmasm-0.2.4/ethpwn_pyevmasm.egg-info/top_level.txt
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/pyevmasm/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)     1077 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/pyevmasm/__init__.py
--rwxrwxr-x   0 honululu  (1000) honululu  (1000)     4197 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/pyevmasm/__main__.py
--rw-rw-r--   0 honululu  (1000) honululu  (1000)    39932 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/pyevmasm/evmasm.py
--rw-rw-r--   0 honululu  (1000) honululu  (1000)       38 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/setup.cfg
--rw-rw-r--   0 honululu  (1000) honululu  (1000)      653 2023-07-31 17:48:00.000000 ethpwn-pyevmasm-0.2.4/setup.py
-drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-07-31 17:51:28.917376 ethpwn-pyevmasm-0.2.4/tests/
--rw-rw-r--   0 honululu  (1000) honululu  (1000)     6722 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.4/tests/test_EVMAssembler.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-08-01 22:49:34.292429 ethpwn-pyevmasm-0.2.5/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)    11357 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/LICENSE
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)      328 2023-08-01 22:49:34.292429 ethpwn-pyevmasm-0.2.5/PKG-INFO
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)     3045 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/README.md
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-08-01 22:49:34.288429 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)      328 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/PKG-INFO
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)      350 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        1 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)       50 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/entry_points.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)       35 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/requires.txt
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)        9 2023-08-01 22:49:34.000000 ethpwn-pyevmasm-0.2.5/ethpwn_pyevmasm.egg-info/top_level.txt
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-08-01 22:49:34.292429 ethpwn-pyevmasm-0.2.5/pyevmasm/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)     1077 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/pyevmasm/__init__.py
+-rwxrwxr-x   0 honululu  (1000) honululu  (1000)     4197 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/pyevmasm/__main__.py
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)    39932 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/pyevmasm/evmasm.py
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)       38 2023-08-01 22:49:34.292429 ethpwn-pyevmasm-0.2.5/setup.cfg
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)      653 2023-08-01 22:48:46.000000 ethpwn-pyevmasm-0.2.5/setup.py
+drwxrwxr-x   0 honululu  (1000) honululu  (1000)        0 2023-08-01 22:49:34.292429 ethpwn-pyevmasm-0.2.5/tests/
+-rw-rw-r--   0 honululu  (1000) honululu  (1000)     6722 2023-07-31 08:34:39.000000 ethpwn-pyevmasm-0.2.5/tests/test_EVMAssembler.py
```

### Comparing `ethpwn-pyevmasm-0.2.4/LICENSE` & `ethpwn-pyevmasm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpwn-pyevmasm-0.2.4/README.md` & `ethpwn-pyevmasm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ethpwn-pyevmasm-0.2.4/pyevmasm/__init__.py` & `ethpwn-pyevmasm-0.2.5/pyevmasm/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpwn-pyevmasm-0.2.4/pyevmasm/__main__.py` & `ethpwn-pyevmasm-0.2.5/pyevmasm/__main__.py`

 * *Files identical despite different names*

### Comparing `ethpwn-pyevmasm-0.2.4/pyevmasm/evmasm.py` & `ethpwn-pyevmasm-0.2.5/pyevmasm/evmasm.py`

 * *Files identical despite different names*

### Comparing `ethpwn-pyevmasm-0.2.4/setup.py` & `ethpwn-pyevmasm-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='ethpwn-pyevmasm',
-    version='0.2.4',
+    version='0.2.5',
     description='Ethereum Virtual Machine (EVM) assembler and disassembler',
     author='Trail of Bits',
     author_email='evmasm@trailofbits.com',
     url='https://github.com/trailofbits/pyevmasm',
     license='Apache License 2.0',
     packages=['pyevmasm'],
     python_requires='>2.7',
```

### Comparing `ethpwn-pyevmasm-0.2.4/tests/test_EVMAssembler.py` & `ethpwn-pyevmasm-0.2.5/tests/test_EVMAssembler.py`

 * *Files identical despite different names*

