# Comparing `tmp/ledgereth-0.8.0.tar.gz` & `tmp/ledgereth-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgereth-0.8.0.tar", last modified: Tue Aug  1 23:32:41 2023, max compression
+gzip compressed data, was "ledgereth-0.8.1.tar", last modified: Wed Aug  2 16:22:37 2023, max compression
```

## Comparing `ledgereth-0.8.0.tar` & `ledgereth-0.8.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:31:35.000000 ledgereth-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-01 23:32:41.794832 ledgereth-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 23:31:35.000000 ledgereth-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/ledgereth/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-08-01 23:31:35.000000 ledgereth-0.8.0/ledgereth/web3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:32:41.794832 ledgereth-0.8.0/ledgereth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 23:32:41.000000 ledgereth-0.8.0/ledgereth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 23:32:41.794832 ledgereth-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-01 23:31:35.000000 ledgereth-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:22:37.287169 ledgereth-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 16:21:36.000000 ledgereth-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-02 16:22:37.287169 ledgereth-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-02 16:21:36.000000 ledgereth-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:22:37.287169 ledgereth-0.8.1/ledgereth/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-08-02 16:21:36.000000 ledgereth-0.8.1/ledgereth/web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:22:37.287169 ledgereth-0.8.1/ledgereth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-02 16:22:37.000000 ledgereth-0.8.1/ledgereth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 16:22:37.000000 ledgereth-0.8.1/ledgereth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:22:37.000000 ledgereth-0.8.1/ledgereth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 16:22:37.000000 ledgereth-0.8.1/ledgereth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 16:22:37.000000 ledgereth-0.8.1/ledgereth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 16:22:37.287169 ledgereth-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-02 16:21:36.000000 ledgereth-0.8.1/setup.py
```

### Comparing `ledgereth-0.8.0/LICENSE` & `ledgereth-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/PKG-INFO` & `ledgereth-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgereth
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library to interface with ledger-app-eth on Ledger hardware wallets
 Home-page: https://github.com/mikeshultz/ledger-eth-lib
 Author: Mike Shultz
 Author-email: mike@mikeshultz.com
 License: UNKNOWN
 Keywords: solidity ethereum development
 Platform: UNKNOWN
```

### Comparing `ledgereth-0.8.0/README.md` & `ledgereth-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/__init__.py` & `ledgereth-0.8.1/ledgereth/__init__.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/__main__.py` & `ledgereth-0.8.1/ledgereth/__main__.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/accounts.py` & `ledgereth-0.8.1/ledgereth/accounts.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/comms.py` & `ledgereth-0.8.1/ledgereth/comms.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/constants.py` & `ledgereth-0.8.1/ledgereth/constants.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/exceptions.py` & `ledgereth-0.8.1/ledgereth/exceptions.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/messages.py` & `ledgereth-0.8.1/ledgereth/messages.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/objects.py` & `ledgereth-0.8.1/ledgereth/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     is_bip32_path,
     is_bytes,
     is_optional_bytes,
     parse_bip32_path,
 )
 
 address = Binary.fixed_length(20, allow_empty=False)
+address_allow_empty = Binary.fixed_length(20, allow_empty=True)
 access_list_sede_type = CountableList(
     ListSedes(
         [
             address,
             CountableList(BigEndianInt(32)),
         ]
     ),
@@ -248,15 +249,15 @@
     .. _`EIP-155`: https://eips.ethereum.org/EIPS/eip-155
     """
 
     fields = [
         ("nonce", big_endian_int),
         ("gas_price", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("chain_id", big_endian_int),
         # Expected nine elements as part of EIP-155 transactions
         ("dummy1", big_endian_int),
         ("dummy2", big_endian_int),
     ]
@@ -328,15 +329,15 @@
     """
 
     fields = [
         ("chain_id", big_endian_int),
         ("nonce", big_endian_int),
         ("gas_price", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("access_list", access_list_sede_type),
     ]
 
     #: The EIP-2718 transaction type
     transaction_type = TransactionType.EIP_2930
@@ -408,15 +409,15 @@
 
     fields = [
         ("chain_id", big_endian_int),
         ("nonce", big_endian_int),
         ("max_priority_fee_per_gas", big_endian_int),
         ("max_fee_per_gas", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("access_list", access_list_sede_type),
     ]
 
     #: The EIP-2718 transaction type
     transaction_type = TransactionType.EIP_1559
@@ -484,15 +485,15 @@
 class SignedTransaction(SerializableTransaction):
     """Signed legacy or EIP-155 transaction"""
 
     fields = [
         ("nonce", big_endian_int),
         ("gas_price", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("v", big_endian_int),
         ("r", big_endian_int),
         ("s", big_endian_int),
     ]
 
@@ -563,15 +564,15 @@
     """A signed Type 1 transaction."""
 
     fields = [
         ("chain_id", big_endian_int),
         ("nonce", big_endian_int),
         ("gas_price", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("access_list", access_list_sede_type),
         ("y_parity", big_endian_int),
         ("sender_r", big_endian_int),
         ("sender_s", big_endian_int),
     ]
@@ -665,15 +666,15 @@
 
     fields = [
         ("chain_id", big_endian_int),
         ("nonce", big_endian_int),
         ("max_priority_fee_per_gas", big_endian_int),
         ("max_fee_per_gas", big_endian_int),
         ("gas_limit", big_endian_int),
-        ("destination", address),
+        ("destination", address_allow_empty),
         ("amount", big_endian_int),
         ("data", binary),
         ("access_list", access_list_sede_type),
         ("y_parity", big_endian_int),
         ("sender_r", big_endian_int),
         ("sender_s", big_endian_int),
     ]
```

### Comparing `ledgereth-0.8.0/ledgereth/transactions.py` & `ledgereth-0.8.1/ledgereth/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,18 +208,14 @@
 
     # EIP-1559 transactions should never have gas_price
     if gas_price and (max_priority_fee_per_gas or max_fee_per_gas):
         raise ValueError(
             "gas_price is incompatible with max_priority_fee_per_gas and max_fee_per_gas"
         )
 
-    # we need a gas price for a valid transaction
-    if not gas_price and not max_fee_per_gas:
-        raise ValueError("gas_price or max_fee_per_gas must be provided")
-
     # Create a serializable tx object
     if max_fee_per_gas:
         tx = Type2Transaction(
             destination=destination,
             amount=amount,
             gas_limit=gas,
             data=data,
```

### Comparing `ledgereth-0.8.0/ledgereth/utils.py` & `ledgereth-0.8.1/ledgereth/utils.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth/web3.py` & `ledgereth-0.8.1/ledgereth/web3.py`

 * *Files identical despite different names*

### Comparing `ledgereth-0.8.0/ledgereth.egg-info/PKG-INFO` & `ledgereth-0.8.1/ledgereth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgereth
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library to interface with ledger-app-eth on Ledger hardware wallets
 Home-page: https://github.com/mikeshultz/ledger-eth-lib
 Author: Mike Shultz
 Author-email: mike@mikeshultz.com
 License: UNKNOWN
 Keywords: solidity ethereum development
 Platform: UNKNOWN
```

### Comparing `ledgereth-0.8.0/setup.py` & `ledgereth-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,12 +66,13 @@
         + requirements_to_list("requirements.docs.txt"),
     },
     package_data={
         "": [
             "README.md",
             "LICENSE",
         ],
+        "ledgereth": ["py.typed"],
     },
     cmdclass={
         "lint": LintCommand,
     },
 )
```

