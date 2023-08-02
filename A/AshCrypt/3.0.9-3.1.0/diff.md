# Comparing `tmp/AshCrypt-3.0.9.tar.gz` & `tmp/AshCrypt-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.9.tar", last modified: Tue Aug  1 18:36:44 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.1.0.tar", last modified: Wed Aug  2 11:50:57 2023, max compression
```

## Comparing `AshCrypt-3.0.9.tar` & `AshCrypt-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:50:57.000000 AshCrypt-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-02 11:50:44.000000 AshCrypt-3.1.0/setup.py
```

### Comparing `AshCrypt-3.0.9/AshCrypt/clicrypt.py` & `AshCrypt-3.1.0/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.9/AshCrypt/crypt.py` & `AshCrypt-3.1.0/AshCrypt/crypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self, num: any) -> None:
         self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num}'
         super().__init__(self.display)
 
 
 class Enc:
-    """Class to encrypt data of either type bytes or strings"""
+    """Class to encrypt data of either type bytes or str"""
 
     def __init__(self, message: Union[str, bytes], mainkey: str,
                  iterations: Optional[int] = 50) -> None:
         if isinstance(message, str):
             self.message = message.encode()
         elif isinstance(message, bytes):
             self.message = message
@@ -54,79 +54,78 @@
     @staticmethod
     def genkey(raw_bytes: Optional[bool] = False,
                desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
         """Generates a random 256-bit ( by default )
         key as either raw bytes or a hex string. Set raw_bytes to True to get
         the key in bytes. Set the number of desired_bytes to a strictly positive integer
         to override the default value"""
-        if desired_bytes <= 0:
+        if desired_bytes < 1:
             raise ValueError("desired_bytes must be strictly greater than 0")
         key = os.urandom(desired_bytes)
         return key if raw_bytes else key.hex()
 
-    def mode(self):
+    def _mode(self):
         """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
         return modes.CBC(self._iv)
 
-    def cipher(self):
+    def _cipher(self):
         """Creates AES cipher object using the encryption key and CBC mode"""
         return Cipher(
             algorithms.AES(
                 key=self.enc_key),
-            mode=self.mode(),
+            mode=self._mode(),
             backend=default_backend())
 
-    def cipher_encryptor(self):
+    def _cipher_encryptor(self):
         """Returns the encryptor for the AES cipher"""
-        return self.cipher().encryptor()
+        return self._cipher().encryptor()
 
     def padded_message(self) -> bytes:
         """Pads the message to a multiple of the block size using PKCS#7 padding"""
         padder = padding.PKCS7(128).padder()
         return padder.update(self.message) + padder.finalize()
 
     def ciphertext(self) -> bytes:
         """Encrypts the padded message using AES and returns the ciphertext"""
-        return self.cipher_encryptor().update(self.padded_message()) + \
-            self.cipher_encryptor().finalize()
+        return self._cipher_encryptor().update(self.padded_message()) + \
+            self._cipher_encryptor().finalize()
 
-    def hmac(self) -> bytes:
+    def hmac_final(self) -> bytes:
         """Computes the HMAC-SHA512 of the ciphertext"""
         hmac_ = self.hmac_key
         hmac_ = hmac.HMAC(hmac_, hashes.SHA512())
         hmac_.update(self.ciphertext())
         return hmac_.finalize()
 
-    def setup_iterations(self) -> bytes:
+    def iterations_bytes(self) -> bytes:
         """Packs the number of iterations into bytes using the 'big-endian' format"""
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
-    def enc_to_bytes(self) -> bytes:
+    def encrypt(self,get_bytes: Optional[bool] = False) -> Union[str,bytes]:
         """Returns the encrypted data as bytes in the form 'HMAC' -> 'IV'
-        -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext """
-        return self.hmac() + self._iv + self.salt + self.pepper + \
-            self.setup_iterations() + self.ciphertext()
-
-    def enc_to_str(self) -> str:
-        """Returns a URL safe base 64 encoded string of the encrypted data"""
-        return base64.urlsafe_b64encode(self.enc_to_bytes()).decode('UTF-8')
+        -> 'Salt value' -> 'pepper value' -> 'iterations' -> 'ciphertext.
+        Or a URL safe base 64 encoded string of the encrypted bytes data,
+        which is the default return value"""
+        raw = self.hmac_final() + self._iv + self.salt + self.pepper + \
+            self.iterations_bytes() + self.ciphertext()
+        return raw if get_bytes else base64.urlsafe_b64encode(raw).decode('UTF-8')
 
 
 class MessageTamperingError(Exception):
     """Raised when any part of the message gets tampered with. DISCARD THE MESSAGE"""
 
     def __init__(self) -> None:
         self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
                        ' or Possible key difference'
         super().__init__(self.display)
 
 
 class Dec:
-    """Class to decrypt data of either type bytes or strings"""
+    """Class to decrypt data of either type bytes or str"""
 
     def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
         if isinstance(message, str):
             mess = message.encode('UTF-8')
             self.message = base64.urlsafe_b64decode(mess)
         elif isinstance(message, bytes):
             self.message = message
@@ -154,40 +153,37 @@
         hmac_.update(self.rec_ciphertext)
         return hmac_.finalize()
 
     def verify_hmac(self) -> bool:
         """Verifies the received HMAC-SHA512 against the calculated HMAC"""
         return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
 
-    def mode(self):
+    def _mode(self):
         """Returns the AES Cipher Block Chaining (CBC) mode with the received  IV"""
         return modes.CBC(self.rec_iv)
 
-    def cipher(self):
+    def _cipher(self):
         """Creates an AES cipher object using the decryption key and CBC mode"""
         return Cipher(
             algorithms.AES(
                 key=self.dec_key),
-            mode=self.mode(),
+            mode=self._mode(),
             backend=default_backend())
 
-    def cipher_decryptor(self):
+    def _cipher_decryptor(self):
         """Returns the decryptor for the AES cipher"""
-        return self.cipher().decryptor()
+        return self._cipher().decryptor()
 
-    def pre_unpadding_dec(self) -> bytes:
+    def _pre_unpadding_dec(self) -> bytes:
         """Decrypts the received ciphertext and returns the pre-unpadded data"""
-        return self.cipher_decryptor().update(self.rec_ciphertext) + \
-            self.cipher_decryptor().finalize()
+        return self._cipher_decryptor().update(self.rec_ciphertext) + \
+            self._cipher_decryptor().finalize()
 
-    def unpadded_m(self) -> bytes:
+    def unpadded_message(self) -> bytes:
         """Unpads the pre-unpadded data and returns the original message """
         unpadder = padding.PKCS7(128).unpadder()
-        return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
+        return unpadder.update(self._pre_unpadding_dec()) + unpadder.finalize()
 
-    def dec_to_bytes(self) -> bytes:
-        """Returns the decrypted message as bytes"""
-        return self.unpadded_m()
-
-    def dec_to_str(self) -> str:
-        """Returns the decrypted message as a UTF-8 encoded string"""
-        return self.unpadded_m().decode('UTF-8')
+    def decrypt(self,get_bytes: Optional[bool] = False) -> Union[str,bytes]:
+        """Returns the decrypted message as a UTF-8 encoded string or a bytes object"""
+        raw = self.unpadded_message()
+        return raw if get_bytes else raw.decode('UTF-8')
```

### Comparing `AshCrypt-3.0.9/AshCrypt/database.py` & `AshCrypt-3.1.0/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.9/AshCrypt/filecrypt.py` & `AshCrypt-3.1.0/AshCrypt/filecrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     with open(self.filename, 'rb') as f:
                         filecontent = f.read()
                     with open(self.filename, 'wb') as f:
                         if filecontent:
                             try:
                                 ins = crypt.Enc(
                                     message=filecontent, mainkey=self.key)
-                                new_content = ins.enc_to_bytes()
+                                new_content = ins.encrypt(get_bytes=True)
                                 f.write(new_content)
                                 go_ahead_rename_crypt = 1
                             except BaseException:
                                 f.write(filecontent)
                                 return 0
                         else:
                             f.write(filecontent)
@@ -87,15 +87,15 @@
                     with open(self.filename, 'rb') as f:
                         enc_content = f.read()
                     with open(self.filename, 'wb') as f:
                         if enc_content:
                             try:
                                 ins = crypt.Dec(
                                     message=enc_content, mainkey=self.key)
-                                a = ins.dec_to_bytes()
+                                a = ins.decrypt(get_bytes=True)
                                 f.write(a)
                                 go_ahead_remove_crypt = 1
                             except Exception:
                                 f.write(enc_content)
                                 return 0
                         else:
                             f.write(enc_content)
@@ -108,8 +108,8 @@
         except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
+        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `AshCrypt-3.0.9/AshCrypt/gui.py` & `AshCrypt-3.1.0/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.9/AshCrypt/textcrypt.py` & `AshCrypt-3.1.0/AshCrypt/textcrypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,27 +36,27 @@
         else:
             return 2
 
     def encrypt(self) -> tuple:
         if self.text:
             try:
                 ins = cp.Enc(self.text, self.key)
-                new_content = ins.enc_to_str()
+                new_content = ins.encrypt()
                 return 1, new_content
             except BaseException:
                 output = 'E'
                 return 0, output
         else:
             return 0.0, 'Empty'
 
     def decrypt(self) -> tuple:
         if self.text:
             try:
                 dec_instance = cp.Dec(message=self.text, mainkey=self.key)
-                a = dec_instance.dec_to_str()
+                a = dec_instance.decrypt()
                 output = a
                 return 1, output
             except Exception:
                 output = self.text
                 return 0, output
         else:
             return 0.0, 'Empty'
```

### Comparing `AshCrypt-3.0.9/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.1.0/AshCrypt/unittests/unittest_crypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import AshCrypt.crypt as cp
+import AshCrypt.crypt as ac
 import unittest
 import struct
 
 
 class CryptModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
         self.message2 = b'this is bytes now'
         self.mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
-        self.ins1 = cp.Enc(message=self.message1, mainkey=self.mainkey)
-        self.string_message = self.ins1.enc_to_str()
-        self.bytes_message = self.ins1.enc_to_bytes()
-        self.ins2 = cp.Dec(message=self.bytes_message, mainkey=self.mainkey)
+        self.ins1 = ac.Enc(message=self.message1, mainkey=self.mainkey)
+        self.string_message = self.ins1.encrypt()
+        self.bytes_message = self.ins1.encrypt(get_bytes=True)
+        self.ins2 = ac.Dec(message=self.bytes_message, mainkey=self.mainkey)
 
     def tearDown(self) -> None:
         pass
 
     def test_KeyLength(self):
-        self.assertEqual(32, bytes.fromhex(cp.Enc.genkey()).__len__())
+        self.assertEqual(32, bytes.fromhex(ac.Enc.genkey()).__len__())
 
     def test_KeyType(self):
-        self.assertIs(str, type(cp.Enc.genkey()))
+        self.assertIs(str, type(ac.Enc.genkey()))
 
     def test_HMAC(self):
-        self.assertTrue(self.bytes_message[:64] == self.ins1.hmac())
+        self.assertTrue(self.bytes_message[:64] == self.ins1.hmac_final())
 
     def test_IV(self):
         self.assertTrue(self.bytes_message[64:80] == self.ins1._iv)
 
     def test_Salt(self):
         self.assertTrue(self.bytes_message[80:96] == self.ins1.salt)
 
     def test_Pepper(self):
         self.assertTrue(self.bytes_message[96:112] == self.ins1.pepper)
 
     def test_Iterations(self):
         self.assertTrue(
-            self.bytes_message[112:116] == self.ins1.setup_iterations())
+            self.bytes_message[112:116] == self.ins1.iterations_bytes())
 
     def test_Ciphertext(self):
         self.assertTrue(self.bytes_message[116:] == self.ins1.ciphertext())
 
     def test_TypeIterations(self):
-        self.assertIs(bytes, type(self.ins1.setup_iterations()))
+        self.assertIs(bytes, type(self.ins1.iterations_bytes()))
 
     def test_IterationsFixed_size(self):
-        self.assertEqual(4, self.ins1.setup_iterations().__len__())
+        self.assertEqual(4, self.ins1.iterations_bytes().__len__())
 
     def test_EncOutputBytes(self):
-        self.assertIs(bytes, type(self.ins1.enc_to_bytes()))
+        self.assertIs(bytes, type(self.ins1.encrypt(get_bytes=True)))
 
     def test_EncOutputString(self):
-        self.assertIs(str, type(self.ins1.enc_to_str()))
+        self.assertIs(str, type(self.ins1.encrypt()))
 
     def test_HMAC_Comp(self):
-        self.assertEqual(self.ins1.hmac(), self.ins2.rec_hmac)
+        self.assertEqual(self.ins1.hmac_final(), self.ins2.rec_hmac)
 
     def test_IV_Comp(self):
         self.assertEqual(self.ins1._iv, self.ins2.rec_iv)
 
     def test_Salt_Comp(self):
         self.assertEqual(self.ins1.salt, self.ins2.rec_salt)
 
@@ -68,27 +68,27 @@
     def test_Iterations_Comp(self):
         self.assertEqual(self.ins1.iterations, self.ins2.rec_iterations)
 
     def test_Ciphertext_Comp(self):
         self.assertEqual(self.ins1.ciphertext(), self.ins2.rec_ciphertext)
 
     def test_HMAC_MismatchError(self):
-        tampered_hmac = self.ins1.enc_to_bytes()[:63] + b'1'
-        tampered_message = tampered_hmac + self.ins1.enc_to_bytes()[64:]
-        with self.assertRaises(cp.MessageTamperingError):
-            cp.Dec(message=tampered_message, mainkey=self.mainkey)
+        tampered_hmac = self.ins1.encrypt(get_bytes=True)[:63] + b'1'
+        tampered_message = tampered_hmac + self.ins1.encrypt(get_bytes=True)[64:]
+        with self.assertRaises(ac.MessageTamperingError):
+            ac.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
-        enb = self.ins1.enc_to_bytes()
+        enb = self.ins1.encrypt(get_bytes=True)
         tampered_message = enb[:112] + struct.pack('!I', 100001) + enb[116:]
-        with self.assertRaises(cp.IterationsOutofRangeError):
-            cp.Dec(message=tampered_message, mainkey=self.mainkey)
+        with self.assertRaises(ac.IterationsOutofRangeError):
+            ac.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_DecOutputBytes(self):
-        self.assertEqual(bytes, type(self.ins2.dec_to_bytes()))
+        self.assertEqual(bytes, type(self.ins2.decrypt(get_bytes=True)))
 
     def test_DecOutputString(self):
-        self.assertEqual(str, type(self.ins2.dec_to_str()))
+        self.assertEqual(str, type(self.ins2.decrypt()))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `AshCrypt-3.0.9/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.1.0/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.9
+Version: 3.1.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.9/PKG-INFO` & `AshCrypt-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.9
+Version: 3.1.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.9/README.md` & `AshCrypt-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -142,21 +142,22 @@
 ```python
 a = Enc(message=message, mainkey=mainkey)
 ```
 
 4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
 <br> Here I chose to encrypt to bytes
 ```python
-output = a.enc_to_bytes()
+output = a.encrypt(get_bytes=True)
 ```
 you can also encrypt to a URL safe string
 ```python
-output = a.enc_to_str()
+output = a.encrypt()
 ```
-<br> The same logic applies to the decryption process simply switch `Enc` with `Dec` and `enc_to_bytes` to `dec_to_bytes`
+<br> 
+The same logic applies to the decryption process simply switch `Enc` with `Dec` and `encrypt()` to `decrypt()`
 That simple, that's it.
 
 
 
 
 ## Features ## 
 - AES 256 CBC mode 
@@ -172,19 +173,36 @@
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
 - In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure its security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
+
+
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 <br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
+<br>Or check it by running this with various `iterations` values:
+```python
+import time
+from AshCrypt import crypt
 
+key = crypt.Enc.genkey()
+t1 = time.perf_counter()
+a = crypt.Enc('hello',key,iterations=50)
+a.encrypt()
+print(time.perf_counter() - t1)
+
+t2 = time.perf_counter()
+b = crypt.Enc('hello',key,iterations=200)
+b.encrypt()
+print(time.perf_counter() -t2)
+```
 
 ## filecrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 my_instance = CryptFile('target.txt', key)
```

### Comparing `AshCrypt-3.0.9/setup.py` & `AshCrypt-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.9',
+    version='3.1.0',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

