# Comparing `tmp/AshCrypt-3.1.0.tar.gz` & `tmp/ashcrypt-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.1.0.tar", last modified: Wed Aug  2 11:50:57 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.1.tar", last modified: Wed Aug  2 21:00:50 2023, max compression
```

## Comparing `AshCrypt-3.1.0.tar` & `ashcrypt-3.1.1.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39554 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/ashcrypt/utils/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:00:50.000000 ashcrypt-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 21:00:37.000000 ashcrypt-3.1.1/setup.py
```

### Comparing `AshCrypt-3.1.0/AshCrypt/clicrypt.py` & `ashcrypt-3.1.1/ashcrypt/clicrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from AshCrypt import filecrypt as af
-from AshCrypt import textcrypt as at
+from ashcrypt import filecrypt as af
+from ashcrypt import textcrypt as at
 from typing import Optional
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
```

### Comparing `AshCrypt-3.1.0/AshCrypt/crypt.py` & `ashcrypt-3.1.1/ashcrypt/crypt.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,29 +3,21 @@
 
 from typing import Union, Optional
 import hmac as hmc
 import base64
 import os
 import struct
 import bcrypt
+from ashcrypt.utils import exceptions
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac
 from cryptography.hazmat.primitives import padding
 
 
-class IterationsOutofRangeError(Exception):
-    """Exception raised when iterations come to be out of range usually due to message tampering
-    where the bytes representing the KDF iterations get touched"""
-
-    def __init__(self, num: any) -> None:
-        self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num}'
-        super().__init__(self.display)
-
-
 class Enc:
     """Class to encrypt data of either type bytes or str"""
 
     def __init__(self, message: Union[str, bytes], mainkey: str,
                  iterations: Optional[int] = 50) -> None:
         if isinstance(message, str):
             self.message = message.encode()
@@ -34,15 +26,15 @@
 
         self.mainkey = mainkey
         self._iv = os.urandom(16)
         self.salt = os.urandom(16)
         self.pepper = os.urandom(16)
         self.iterations = iterations
         if self.iterations < 50 or self.iterations > 100000:
-            raise IterationsOutofRangeError(self.iterations)
+            raise exceptions.IterationsOutofRangeError(self.iterations)
         self.enc_key = self.derkey(self.mainkey, self.salt, self.iterations)
         self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
 
     @staticmethod
     def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
         """AES Key & HMAC derivation function"""
         return bcrypt.kdf(
@@ -54,16 +46,16 @@
     @staticmethod
     def genkey(raw_bytes: Optional[bool] = False,
                desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
         """Generates a random 256-bit ( by default )
         key as either raw bytes or a hex string. Set raw_bytes to True to get
         the key in bytes. Set the number of desired_bytes to a strictly positive integer
         to override the default value"""
-        if desired_bytes < 1:
-            raise ValueError("desired_bytes must be strictly greater than 0")
+        if desired_bytes < 32:
+            raise ValueError("desired_bytes must be greater or equal to 32")
         key = os.urandom(desired_bytes)
         return key if raw_bytes else key.hex()
 
     def _mode(self):
         """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
         return modes.CBC(self._iv)
 
@@ -85,80 +77,75 @@
         return padder.update(self.message) + padder.finalize()
 
     def ciphertext(self) -> bytes:
         """Encrypts the padded message using AES and returns the ciphertext"""
         return self._cipher_encryptor().update(self.padded_message()) + \
             self._cipher_encryptor().finalize()
 
-    def hmac_final(self) -> bytes:
-        """Computes the HMAC-SHA512 of the ciphertext"""
-        hmac_ = self.hmac_key
-        hmac_ = hmac.HMAC(hmac_, hashes.SHA512())
-        hmac_.update(self.ciphertext())
-        return hmac_.finalize()
-
     def iterations_bytes(self) -> bytes:
         """Packs the number of iterations into bytes using the 'big-endian' format"""
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
-    def encrypt(self,get_bytes: Optional[bool] = False) -> Union[str,bytes]:
+    def hmac_final(self) -> bytes:
+        """Computes the HMAC-SHA256 of the ciphertext"""
+        hmac_ = self.hmac_key
+        hmac_ = hmac.HMAC(hmac_, hashes.SHA256())
+        hmac_.update(self._iv + self.salt + self.pepper +
+                     self.iterations_bytes() + self.ciphertext())
+        return hmac_.finalize()
+
+    def encrypt(self, get_bytes: Optional[bool] = False) -> Union[str, bytes]:
         """Returns the encrypted data as bytes in the form 'HMAC' -> 'IV'
         -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext.
         Or a URL safe base 64 encoded string of the encrypted bytes data,
         which is the default return value"""
         raw = self.hmac_final() + self._iv + self.salt + self.pepper + \
             self.iterations_bytes() + self.ciphertext()
-        return raw if get_bytes else base64.urlsafe_b64encode(raw).decode('UTF-8')
-
-
-class MessageTamperingError(Exception):
-    """Raised when any part of the message gets tampered with. DISCARD THE MESSAGE"""
-
-    def __init__(self) -> None:
-        self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
-                       ' or Possible key difference'
-        super().__init__(self.display)
+        return raw if get_bytes else base64.urlsafe_b64encode(
+            raw).decode('UTF-8')
 
 
 class Dec:
     """Class to decrypt data of either type bytes or str"""
 
     def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
         if isinstance(message, str):
             mess = message.encode('UTF-8')
             self.message = base64.urlsafe_b64decode(mess)
         elif isinstance(message, bytes):
             self.message = message
         self.key = mainkey
-        self.rec_hmac = self.message[:64]
-        self.rec_iv = self.message[64:80]
-        self.rec_salt = self.message[80:96]
-        self.rec_pepper = self.message[96:112]
-        self.rec_iterations = struct.unpack('!I', self.message[112:116])[0]
+        self.rec_hmac = self.message[:32]
+        self.rec_iv = self.message[32:48]
+        self.rec_salt = self.message[48:64]
+        self.rec_pepper = self.message[64:80]
+        self.rec_iters_raw = self.message[80:84]
+        self.rec_iterations = struct.unpack('!I', self.rec_iters_raw)[0]
         if self.rec_iterations < 50 or self.rec_iterations > 100000:
-            raise IterationsOutofRangeError(self.rec_iterations)
-        self.rec_ciphertext = self.message[116:]
+            raise exceptions.IterationsOutofRangeError(self.rec_iterations)
+        self.rec_ciphertext = self.message[84:]
         self.dec_key = Enc.derkey(self.key, self.rec_salt, self.rec_iterations)
         self.hmac_k = Enc.derkey(
             self.key,
             self.rec_pepper,
             self.rec_iterations)
         if self.verify_hmac() is False:
-            raise MessageTamperingError()
+            raise exceptions.MessageTamperingError()
 
     def calculated_hmac(self) -> bytes:
-        """Computes the HMAC-SHA512 of the received ciphertext"""
+        """Computes the HMAC-SHA256 of the received ciphertext"""
         hmac_ = self.hmac_k
-        hmac_ = hmac.HMAC(hmac_, hashes.SHA512())
-        hmac_.update(self.rec_ciphertext)
+        hmac_ = hmac.HMAC(hmac_, hashes.SHA256())
+        hmac_.update(self.rec_iv + self.rec_salt + self.rec_pepper +
+                     self.rec_iters_raw + self.rec_ciphertext)
         return hmac_.finalize()
 
     def verify_hmac(self) -> bool:
-        """Verifies the received HMAC-SHA512 against the calculated HMAC"""
+        """Verifies the received HMAC-SHA256 against the calculated HMAC"""
         return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
 
     def _mode(self):
         """Returns the AES Cipher Block Chaining (CBC) mode with the received  IV"""
         return modes.CBC(self.rec_iv)
 
     def _cipher(self):
@@ -179,11 +166,11 @@
             self._cipher_decryptor().finalize()
 
     def unpadded_message(self) -> bytes:
         """Unpads the pre-unpadded data and returns the original message """
         unpadder = padding.PKCS7(128).unpadder()
         return unpadder.update(self._pre_unpadding_dec()) + unpadder.finalize()
 
-    def decrypt(self,get_bytes: Optional[bool] = False) -> Union[str,bytes]:
+    def decrypt(self, get_bytes: Optional[bool] = False) -> Union[str, bytes]:
         """Returns the decrypted message as a UTF-8 encoded string or a bytes object"""
         raw = self.unpadded_message()
-        return raw if get_bytes else raw.decode('UTF-8')
+        return raw if get_bytes else raw.decode('UTF-8')
```

### Comparing `AshCrypt-3.1.0/AshCrypt/database.py` & `ashcrypt-3.1.1/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.1.0/AshCrypt/filecrypt.py` & `ashcrypt-3.1.1/ashcrypt/utils/gui/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 """This module is used to encrypt and decrypt files of either type str or bytes"""
 
 
-from AshCrypt import crypt
+from ashcrypt import crypt
 import os
 
-
-class KeyLengthError(Exception):
-    def __init__(self):
-        self.display = 'Key must be 256 Bit long !'
-        super().__init__(self.display)
-
-
 class CryptFile:
     '''Class to encrypt/decrypt a given file. Pass in the filename
                 as well as a 256-bit key '''
     def __init__(self, filename : str, key : str):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
-            self.not_256_bit_key = 1  # Raise KeyError() / you can switch error handling
+            self.not_256_bit_key = 1
 
     @staticmethod
     def genkey() -> str:
         return crypt.Enc.genkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
```

### Comparing `AshCrypt-3.1.0/AshCrypt/gui.py` & `ashcrypt-3.1.1/ashcrypt/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import AshCrypt.textcrypt as At
-import AshCrypt.filecrypt as Af
-import AshCrypt.database as Ad
+import ashcrypt.utils.gui.text as At
+import ashcrypt.utils.gui.file as Af
+import ashcrypt.database as Ad
 import ttkbootstrap as tk
-import AshCrypt.qr as qr
+import ashcrypt.qr as qr
 import platform
 import secrets
 import os.path
 import string
 import atexit
 import json
 import re
 
 
 '''------------------------FRAMING STARTED-------------------'''
 
 main_object = tk.Window(themename='vapor')
 main_object.resizable(False, False)
-main_object.title('AshCrypt')
+main_object.title('ashcrypt')
 main_object.geometry('1500x800')
 
 
 databaseFrame = tk.Frame(master=main_object, width=500, height=800)
 databaseFrame.place(x=0, y=0)
 
 frameFile1 = tk.Frame(master=main_object, width=500, height=250)
```

### Comparing `AshCrypt-3.1.0/AshCrypt/textcrypt.py` & `ashcrypt-3.1.1/ashcrypt/utils/gui/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module is used to encrypt and decrypt text data"""
 
 
-from AshCrypt import crypt as cp
+from ashcrypt import crypt as cp
 from typing import Union
 
 
 class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
```

### Comparing `AshCrypt-3.1.0/AshCrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.1/ashcrypt/unittests/unittest_crypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import AshCrypt.crypt as ac
+import ashcrypt.crypt as ac
+from ashcrypt.utils import exceptions
 import unittest
 import struct
 
 
 class CryptModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
@@ -19,31 +20,31 @@
     def test_KeyLength(self):
         self.assertEqual(32, bytes.fromhex(ac.Enc.genkey()).__len__())
 
     def test_KeyType(self):
         self.assertIs(str, type(ac.Enc.genkey()))
 
     def test_HMAC(self):
-        self.assertTrue(self.bytes_message[:64] == self.ins1.hmac_final())
+        self.assertTrue(self.bytes_message[:32] == self.ins1.hmac_final())
 
     def test_IV(self):
-        self.assertTrue(self.bytes_message[64:80] == self.ins1._iv)
+        self.assertTrue(self.bytes_message[32:48] == self.ins1._iv)
 
     def test_Salt(self):
-        self.assertTrue(self.bytes_message[80:96] == self.ins1.salt)
+        self.assertTrue(self.bytes_message[48:64] == self.ins1.salt)
 
     def test_Pepper(self):
-        self.assertTrue(self.bytes_message[96:112] == self.ins1.pepper)
+        self.assertTrue(self.bytes_message[64:80] == self.ins1.pepper)
 
     def test_Iterations(self):
         self.assertTrue(
-            self.bytes_message[112:116] == self.ins1.iterations_bytes())
+            self.bytes_message[80:84] == self.ins1.iterations_bytes())
 
     def test_Ciphertext(self):
-        self.assertTrue(self.bytes_message[116:] == self.ins1.ciphertext())
+        self.assertTrue(self.bytes_message[84:] == self.ins1.ciphertext())
 
     def test_TypeIterations(self):
         self.assertIs(bytes, type(self.ins1.iterations_bytes()))
 
     def test_IterationsFixed_size(self):
         self.assertEqual(4, self.ins1.iterations_bytes().__len__())
 
@@ -69,22 +70,23 @@
         self.assertEqual(self.ins1.iterations, self.ins2.rec_iterations)
 
     def test_Ciphertext_Comp(self):
         self.assertEqual(self.ins1.ciphertext(), self.ins2.rec_ciphertext)
 
     def test_HMAC_MismatchError(self):
         tampered_hmac = self.ins1.encrypt(get_bytes=True)[:63] + b'1'
-        tampered_message = tampered_hmac + self.ins1.encrypt(get_bytes=True)[64:]
-        with self.assertRaises(ac.MessageTamperingError):
+        tampered_message = tampered_hmac + \
+            self.ins1.encrypt(get_bytes=True)[64:]
+        with self.assertRaises(exceptions.MessageTamperingError):
             ac.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
         enb = self.ins1.encrypt(get_bytes=True)
-        tampered_message = enb[:112] + struct.pack('!I', 100001) + enb[116:]
-        with self.assertRaises(ac.IterationsOutofRangeError):
+        tampered_message = enb[:80] + struct.pack('!I', 100001) + enb[84:]
+        with self.assertRaises(exceptions.IterationsOutofRangeError):
             ac.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_DecOutputBytes(self):
         self.assertEqual(bytes, type(self.ins2.decrypt(get_bytes=True)))
 
     def test_DecOutputString(self):
         self.assertEqual(str, type(self.ins2.decrypt()))
```

### Comparing `AshCrypt-3.1.0/AshCrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: AshCrypt
-Version: 3.1.0
+Name: ashcrypt
+Version: 3.1.1
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.1.0/PKG-INFO` & `ashcrypt-3.1.1/ashcrypt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: AshCrypt
-Version: 3.1.0
+Name: ashcrypt
+Version: 3.1.1
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.1.0/README.md` & `ashcrypt-3.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,125 +1,101 @@
 # Cryptography App & Library w/ AES-256
 ##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
-## Reason Behind It
-In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
-
-This led me to develop a set of tools in Python that leverages the AES-256 algorithm to make it easier for individuals to safeguard their data without blindly relying on third parties to do it for them. 
-
-My aim here is to make these tools accessible and user-friendly, even for individuals with a limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
+#### Enhanced Security, Simplicity & Ease of use For Anyone Willing To Use AES 256.
 ## Overview ## 
 ![alt text](important/GUI.png)
-The project incorporates an App & a library called **AshCrypt** : 
+The project incorporates an App & a library called **ashcrypt** : 
 
 **App :** 
 <br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check [GUI](https://github.com/AshGw/AES-256#GUI) header for more info.
+<br>check [GUI](https://github.com/AshGw/AES-256#gui) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
 <br>The core of the library is the module `crypt`
 It offers cryptographic capabilities and top security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
 
 ### For Developers ###
 The project uses `crypt` module to ensure secure data encryption and decryption for files and text while keeping it very easy and simple to use .
-view the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
+View the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
-It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
+It also incorporates a database module that serve the same purpose which is allowing for key management & storage of classified content in a secure, 
 safe and simple manner.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
 
 ## Installation ##
 ### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
 ```
 Then install the Library 
 ```bash
-pip install AshCrypt
+pip install ashcrypt
 ```
-This will install the latest version of `AshCrypt`.
+This will install the latest version of `ashcrypt`.
 You can start using it in your code by importing its modules :
 
 ```python
-from AshCrypt import crypt as ac
+from ashcrypt import crypt as ac
 ```
 That's it.
 
 ### Whole repo installation 
 Now if you want to get the whole repo with no manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
-<details>
-<summary>Got Errors ?</summary>
-
-<h5>For Debian based systems</h5>
-
-1) Install `curl` if you don't have it already 
-```bash
-sudo apt-get install curl
-```
-2) If you're running a lightweight python version it might not include `tkinter` in the standard library so run
-```bash
-sudo apt-get update
-sudo apt-get install python3-tk 
-```
-3) If you're running `python 3.6` or older, then you might need to install `dataclasses`
-```
-pip install dataclasses
-```
-<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
-</details>
-
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
-python -m AshCrypt.gui
+python -m ashcrypt.gui
 ```
 
 **NOTE**:
 You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
 
 
 To run the CLI 
 ```shell
-python -m AshCrypt.clicrypt
+python -m ashcrypt.clicrypt
 ```
 
-## "crypt" Module ##
+## `crypt` Module ##
 The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
-<br>You can check the [unittesting file](AshCrypt/unittests/unittest_crypt.py) to verify how it works.
+<br>You can check the [unittesting file](ashcrypt/unittests/unittest_crypt.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
-<br>Set the correct mainkey ( 32 byte long key ) 
+<br>This will output a string type key (hex) you can change that to render bytes:
+```python
+mainkey = Enc.genkey(raw_bytes=True)
+```
 ```python
 mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
 The message can be of type string or bytes.
 <br>Normal string message :  
 ```python 
 message = 'Hello There'
@@ -136,15 +112,15 @@
 ```python
 message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
 ```
 3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
 <br><br>So first create an instance of either the `Enc` or `Dec` class. 
 <br>Here I chose to encrypt a message 
 ```python
-a = Enc(message=message, mainkey=mainkey)
+a = Enc(message, mainkey)
 ```
 
 4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
 <br> Here I chose to encrypt to bytes
 ```python
 output = a.encrypt(get_bytes=True)
 ```
@@ -162,140 +138,124 @@
 ## Features ## 
 - AES 256 CBC mode 
 - Generates a randomly secure 256-bit main key 
 - Derives the HMAC and the AES key from the mainkey using bcrypt's KDFs with a configurable number of iterations with :
     - Salt : Random 128 bit value is generated  each time and passed to the KDF to generate the AES key
     - Pepper : Random 128 bit value is generated  each time and passed to the KDF to generate the HMAC
 - AES Key : 256 bit
-- HMAC : 256 bit hashed using SHA512
+- HMAC : 256 bit hashed using SHA256
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure its security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
+- In `crypt` module the key is flexible it must be **at least** 256-bit , so can go higher if you want ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
-<br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
-<br>Or check it by running this with various `iterations` values:
+<br>Check it by running this with various `iterations` values:
+
 ```python
 import time
-from AshCrypt import crypt
+from ashcrypt import crypt
 
 key = crypt.Enc.genkey()
 t1 = time.perf_counter()
-a = crypt.Enc('hello',key,iterations=50)
+a = crypt.Enc('hello', key, iterations=50)
 a.encrypt()
 print(time.perf_counter() - t1)
 
 t2 = time.perf_counter()
-b = crypt.Enc('hello',key,iterations=200)
+b = crypt.Enc('hello', key, iterations=200)
 b.encrypt()
-print(time.perf_counter() -t2)
+print(time.perf_counter() - t2)
 ```
 
-## filecrypt ## 
+## `filecrypt` ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 my_instance = CryptFile('target.txt', key)
 ```
 ```python
-my_instance = CryptFile('testDataBase.db', key)
+my_instance = CryptFile('test.db', key)
 ```
 The file can be of anything : image`.png`, movie `.mp4`,`.sqlite`  etc..
 <br>It doesn't have to just be of `.txt` extension ,can be of anything really.  
 <br>**Note** : 
 If the file is not in the working directory you can specify the whole path: 
 <br>**For windows**
 ```python
 target = CryptFile('C:\\Users\\offic\\MyProjects\\SomeOtherfolder\\myfile.txt',key) 
 ```
 <br>**On Mac and Linux :**
 ```python
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
-3) Apply either the encryption or decryption functions to that instance :
+3) Apply either the `encrypt()` or `decrypt()` over that instance :
 ```python
 my_instance = CryptFile('qrv10.png',key)
 my_instance.encrypt()
 ```
 you can apply `print()` on `my_instance.encrypt()`to check the result :
-<br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
-<br> 2 : File is empty
-<br> 3 : File doesn't exist
-<br> 4 : Unknown Error usually a system related one 
-<br> 5 : Key is denied for cryptographic use
-<br> 6 : File is already encrypted/decrypted
-<br> 7 : File is not a file it's a directory
-<br> 0 : Error in enc/dec probable file distortion, tampering or wrong key
+<br>If the output is 1 then the file has been successfully encrypted/decrypted + added/removed .crypt extension 
+<br> Other than that it should raise an Exception with the specified Error.
 ```python
 my_instance.encrypt()
 ```
 ```python
 my_instance.decrypt()
 ```
 
 That's it, if you follow the steps above then everything should work just fine.
-## textcrypt ## 
-Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
+## `textcrypt` ## 
+Follow the same steps above the naming is just differs, and keep in mind both accept either strings or bytes 
 ```python
 my_instance = Crypt('Hello Wold !',key)
 ```
 ```python
 my_instance.encrypt()[1]
 ```
 ```python
 my_instance.decrypt()[1]
 ```
-The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occurred.
-<br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
-
-**Note**:
-<br>Unlike the `crypt` module where if you try to decrypt a non-encrypted message you get all kinds of errors.
-
-in `filecrypt` & `textcrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
-<br>`1`'s for success.
-<br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
-
-Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
+The result simply returns a tuple so index `[0]` is going to be the confirmation if it's `1` then it worked, else some Error has occurred.
+<br>Index `[1]` contains the encrypted/decrypted content.
 
-
-### QR ## 
-The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
-
-## database ##
-To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
+## `database` ##
+To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using sqlite3 type database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
 **Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+Run:
+```python
+pip install dataclasses
+```
 
 ### Usage ## 
-In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
+In this module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
-**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferably off-grid and completely separate from any vulnerable devices on you can have it on a separate database stored safely away, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
-
+**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key.
 1) Create a connection to the database :
 ```python
 conn = Database('test.db')
 ```
 This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
 ```python
-conn = Database('test.db','MyDefaultTable')
+conn = Database('test.db','mytable')
 ```
 2) create/add the table to the database :
 ```python
 conn.addtable()
 ```
 Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
 
@@ -360,29 +320,30 @@
 - Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
 - The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
 #### Database
 - Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
 1) Specifying the actual path where you want your database to be 
 2) Give it a name, it must be a valid file name that ends with `.db` .<br>
 If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
-3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
-<br>The only common data that these two separate databases have in common is the key reference values.  
+3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to the name. This database holds the actual keys and the reference to these keys.
+<br>The only piece of data that these two separate databases have in common is the key reference values.  
 
    
-**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
-`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+**Info**: 
+<br>Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although for the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
 <br>`Content` in the main db, that holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
 <br>`Key` in  both db's that holds the `KeyRef` or key reference value
 #### Usage 
 The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
 <br>Just click buttons and check the result in the output console, it will guide you through the process.
 
 <br>To run the GUI anywhere
 ```shell
-python -m AshCrypt.gui
+python -m ashcrypt.gui
 ```
 
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-3.1.0/setup.py` & `ashcrypt-3.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
-with open('AshCrypt/README.md', 'r') as f:
+with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    name='AshCrypt',
-    version='3.1.0',
+    name='ashcrypt',
+    version='3.1.1',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
-    packages=find_packages(exclude=['important', 'Docker-build', '.github', 'Executables', 'demo']),
+    packages=find_packages(exclude=['important', 'Docker-build', '.github']),
     package_data={
-        'AshCrypt': ['**'],
+        'ashcrypt': ['**'],
     },
     exclude_package_data={
         '': ['.gitignore', 'LICENSE', 'README'],
     },
     install_requires=[
         'bcrypt==4.0.1',
         'cryptography==40.0.2',
```

