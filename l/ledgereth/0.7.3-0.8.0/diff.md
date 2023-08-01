# Comparing `tmp/ledgereth-0.7.3.tar.gz` & `tmp/ledgereth-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgereth-0.7.3.tar", last modified: Wed Nov  9 05:29:13 2022, max compression
+gzip compressed data, was "ledgereth-0.8.0.tar", last modified: Tue Aug  1 23:32:41 2023, max compression
```

## Comparing `ledgereth-0.7.3.tar` & `ledgereth-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 05:29:13.453242 ledgereth-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-11-09 05:29:13.453242 ledgereth-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-09 05:28:41.000000 ledgereth-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 05:29:13.453242 ledgereth-0.7.3/ledgereth/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6311 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2751 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/comms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)    25343 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     9952 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6747 2022-11-09 05:28:41.000000 ledgereth-0.7.3/ledgereth/web3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 05:29:13.453242 ledgereth-0.7.3/ledgereth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-11-09 05:29:13.000000 ledgereth-0.7.3/ledgereth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-11-09 05:29:13.000000 ledgereth-0.7.3/ledgereth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 05:29:13.000000 ledgereth-0.7.3/ledgereth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-11-09 05:29:13.000000 ledgereth-0.7.3/ledgereth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-09 05:29:13.000000 ledgereth-0.7.3/ledgereth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-09 05:29:13.453242 ledgereth-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-11-09 05:28:41.000000 ledgereth-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:31:35.000000 ledgereth-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-01 23:32:41.794832 ledgereth-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 23:31:35.000000 ledgereth-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/ledgereth/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/ledgereth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 23:32:41.794832 ledgereth-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-01 23:31:35.000000 ledgereth-0.8.0/setup.py
```

### Comparing `ledgereth-0.7.3/PKG-INFO` & `ledgereth-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: ledgereth
-Version: 0.7.3
+Version: 0.8.0
 Summary: Library to interface with ledger-app-eth on Ledger hardware wallets
 Home-page: https://github.com/mikeshultz/ledger-eth-lib
 Author: Mike Shultz
 Author-email: mike@mikeshultz.com
 License: UNKNOWN
-Description: # ledgereth
-        
-        [![Documentation Status](https://readthedocs.org/projects/ledgereth/badge/?version=latest)](https://ledgereth.readthedocs.io/en/latest/?badge=latest)
-        
-        **This library is beta.  Please [report any bugs](https://github.com/mikeshultz/ledger-eth-lib/issues/new) you find.**
-        
-        This is a library to interact with [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger nice and simple with well known Ethereum+Python tools.
-        
-        ## Quickstart
-        
-        Here’s the quickest way to get started.
-        
-            pip install ledgereth
-        
-        Please see [the ledgereth documentation](https://ledgereth.readthedocs.io/) for more detailed information.
-        
-        ## Compatability
-        
-        ### Ledger Devices
-        
-        This lib has been tested to work on Ledger Nano S and Nano X.  It will probalby work with Ledger Blue and any devices the [`ledgerblue` library](https://github.com/LedgerHQ/blue-loader-python) and [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth) supports.
-        
-        ### Ledger Account Derivations
-        
-        The Ledger-provided desktop apps have changed the way accounts are derived with the release of Ledger Live.  If you created your Ledger account(s) with the older Chrome app and want to use those account(s) with this library, you will need to set the `LEDGER_LEGACY_ACCOUNTS` env var. You can only use one or the other at a time.  See [the notes in source for more information](https://github.com/mikeshultz/ledger-eth-lib/blob/master/ledgereth/web3.py#L8-L34).
-        
 Keywords: solidity ethereum development
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+# ledgereth
+
+[![Documentation Status](https://readthedocs.org/projects/ledgereth/badge/?version=latest)](https://ledgereth.readthedocs.io/en/latest/?badge=latest)
+
+**This library is beta.  Please [report any bugs](https://github.com/mikeshultz/ledger-eth-lib/issues/new) you find.**
+
+This is a library to interact with [app-ethereum](https://github.com/LedgerHQ/app-ethereum), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger easy.
+
+## Quickstart
+
+Here’s the quickest way to get started.
+
+    pip install ledgereth
+
+Please see [the ledgereth documentation](https://ledgereth.readthedocs.io/) for more detailed information.
+
+## Compatability
+
+### Ledger Devices
+
+This lib has been tested to work on Ledger Nano S and Nano X.  It will probalby work with Ledger Blue and any devices the [`ledgerblue` library](https://github.com/LedgerHQ/blue-loader-python) and [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth) supports.
+
+### Ledger Account Derivations
+
+The Ledger-provided desktop apps have changed the way accounts are derived with the release of Ledger Live.  If you created your Ledger account(s) with the older Chrome app and want to use those account(s) with this library, you will need to set the `LEDGER_LEGACY_ACCOUNTS` env var. You can only use one or the other at a time.  See [the notes in source for more information](https://github.com/mikeshultz/ledger-eth-lib/blob/master/ledgereth/web3.py#L8-L34).
+
+
```

### Comparing `ledgereth-0.7.3/README.md` & `ledgereth-0.8.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ledgereth
 
 [![Documentation Status](https://readthedocs.org/projects/ledgereth/badge/?version=latest)](https://ledgereth.readthedocs.io/en/latest/?badge=latest)
 
 **This library is beta.  Please [report any bugs](https://github.com/mikeshultz/ledger-eth-lib/issues/new) you find.**
 
-This is a library to interact with [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger nice and simple with well known Ethereum+Python tools.
+This is a library to interact with [app-ethereum](https://github.com/LedgerHQ/app-ethereum), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger easy.
 
 ## Quickstart
 
 Here’s the quickest way to get started.
 
     pip install ledgereth
```

### Comparing `ledgereth-0.7.3/ledgereth/__init__.py` & `ledgereth-0.8.0/ledgereth/__init__.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/__main__.py` & `ledgereth-0.8.0/ledgereth/__main__.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/accounts.py` & `ledgereth-0.8.0/ledgereth/accounts.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/comms.py` & `ledgereth-0.8.0/ledgereth/comms.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/constants.py` & `ledgereth-0.8.0/ledgereth/constants.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/exceptions.py` & `ledgereth-0.8.0/ledgereth/exceptions.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/messages.py` & `ledgereth-0.8.0/ledgereth/messages.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/objects.py` & `ledgereth-0.8.0/ledgereth/objects.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/transactions.py` & `ledgereth-0.8.0/ledgereth/transactions.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/utils.py` & `ledgereth-0.8.0/ledgereth/utils.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth/web3.py` & `ledgereth-0.8.0/ledgereth/web3.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.7.3/ledgereth.egg-info/PKG-INFO` & `ledgereth-0.8.0/ledgereth.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: ledgereth
-Version: 0.7.3
+Version: 0.8.0
 Summary: Library to interface with ledger-app-eth on Ledger hardware wallets
 Home-page: https://github.com/mikeshultz/ledger-eth-lib
 Author: Mike Shultz
 Author-email: mike@mikeshultz.com
 License: UNKNOWN
-Description: # ledgereth
-        
-        [![Documentation Status](https://readthedocs.org/projects/ledgereth/badge/?version=latest)](https://ledgereth.readthedocs.io/en/latest/?badge=latest)
-        
-        **This library is beta.  Please [report any bugs](https://github.com/mikeshultz/ledger-eth-lib/issues/new) you find.**
-        
-        This is a library to interact with [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger nice and simple with well known Ethereum+Python tools.
-        
-        ## Quickstart
-        
-        Here’s the quickest way to get started.
-        
-            pip install ledgereth
-        
-        Please see [the ledgereth documentation](https://ledgereth.readthedocs.io/) for more detailed information.
-        
-        ## Compatability
-        
-        ### Ledger Devices
-        
-        This lib has been tested to work on Ledger Nano S and Nano X.  It will probalby work with Ledger Blue and any devices the [`ledgerblue` library](https://github.com/LedgerHQ/blue-loader-python) and [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth) supports.
-        
-        ### Ledger Account Derivations
-        
-        The Ledger-provided desktop apps have changed the way accounts are derived with the release of Ledger Live.  If you created your Ledger account(s) with the older Chrome app and want to use those account(s) with this library, you will need to set the `LEDGER_LEGACY_ACCOUNTS` env var. You can only use one or the other at a time.  See [the notes in source for more information](https://github.com/mikeshultz/ledger-eth-lib/blob/master/ledgereth/web3.py#L8-L34).
-        
 Keywords: solidity ethereum development
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+# ledgereth
+
+[![Documentation Status](https://readthedocs.org/projects/ledgereth/badge/?version=latest)](https://ledgereth.readthedocs.io/en/latest/?badge=latest)
+
+**This library is beta.  Please [report any bugs](https://github.com/mikeshultz/ledger-eth-lib/issues/new) you find.**
+
+This is a library to interact with [app-ethereum](https://github.com/LedgerHQ/app-ethereum), the Ethereum app for the [Ledger hardware wallets](https://www.ledger.com/).  It's goal is to make interfacing with the Ledger easy.
+
+## Quickstart
+
+Here’s the quickest way to get started.
+
+    pip install ledgereth
+
+Please see [the ledgereth documentation](https://ledgereth.readthedocs.io/) for more detailed information.
+
+## Compatability
+
+### Ledger Devices
+
+This lib has been tested to work on Ledger Nano S and Nano X.  It will probalby work with Ledger Blue and any devices the [`ledgerblue` library](https://github.com/LedgerHQ/blue-loader-python) and [ledger-app-eth](https://github.com/LedgerHQ/ledger-app-eth) supports.
+
+### Ledger Account Derivations
+
+The Ledger-provided desktop apps have changed the way accounts are derived with the release of Ledger Live.  If you created your Ledger account(s) with the older Chrome app and want to use those account(s) with this library, you will need to set the `LEDGER_LEGACY_ACCOUNTS` env var. You can only use one or the other at a time.  See [the notes in source for more information](https://github.com/mikeshultz/ledger-eth-lib/blob/master/ledgereth/web3.py#L8-L34).
+
+
```

### Comparing `ledgereth-0.7.3/setup.py` & `ledgereth-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,26 +48,26 @@
     author_email=meta.email,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="solidity ethereum development",
     packages=find_packages(exclude=["docs", "tests", "scripts", "build"]),
     install_requires=requirements_to_list("requirements.txt"),
     extras_require={
         "dev": requirements_to_list("requirements.dev.txt"),
-        "docs": requirements_to_list("requirements.docs.txt"),
+        "docs": requirements_to_list("requirements.dev.txt")
+        + requirements_to_list("requirements.docs.txt"),
     },
     package_data={
         "": [
             "README.md",
             "LICENSE",
         ],
     },
```

