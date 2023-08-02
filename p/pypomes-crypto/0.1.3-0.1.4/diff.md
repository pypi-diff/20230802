# Comparing `tmp/pypomes_crypto-0.1.3.tar.gz` & `tmp/pypomes_crypto-0.1.4.tar.gz`

## Comparing `pypomes_crypto-0.1.3.tar` & `pypomes_crypto-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pkcs7.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/__init__.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pkcs7.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pomes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/README.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/PKG-INFO
```

### Comparing `pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pkcs7.py` & `pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pkcs7.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     hash_algorithm: str                  # the algorithm used to calculate the payload hash
     signature: bytes                     # the digital signature
     signature_algorithm: str             # the algorithm used to generate the signature
     signature_timestamp: datetime        # the signature's timestamp
     public_key: bytes                    # the serialized public key (in PEM format)
     cert_chain: list[bytes]              # the serialized X509 certificate chain (in PEM format)
 
-    def __init__(self, p7s_file: str | bytes):
+    def __init__(self, p7s_file: str | bytes) -> None:
         """
         Instantiate the PKCS#7 crypto class, and extract the relevant data.
 
         :param p7s_file: a p7s file path or the p7s file bytes
         """
         # is the input argument a file path ?
         if isinstance(p7s_file, str):
```

### Comparing `pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pomes.py` & `pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_crypto-0.1.3/LICENSE` & `pypomes_crypto-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_crypto-0.1.3/pyproject.toml` & `pypomes_crypto-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_crypto"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (cryptography modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_crypto-0.1.3/PKG-INFO` & `pypomes_crypto-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_crypto
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (cryptography modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Crypto
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Crypto/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

