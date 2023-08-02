# Comparing `tmp/kount_ris_sdk-3.4.3.tar.gz` & `tmp/kount_ris_sdk-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kount_ris_sdk-3.4.3.tar", last modified: Tue Jul 11 15:52:06 2023, max compression
+gzip compressed data, was "kount_ris_sdk-3.4.4.tar", last modified: Wed Aug  2 19:00:55 2023, max compression
```

## Comparing `kount_ris_sdk-3.4.3.tar` & `kount_ris_sdk-3.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/LICENSE
--rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) nogroup  (65534)      600 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/README.md
--rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/setup.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.343776 kount_ris_sdk-3.4.3/src/
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/client.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/config.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/inquiry.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    13902 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/request.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/resources/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/resources/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/resources/correct_key_cryp.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/response.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/settings.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/util/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/a85.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/address.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/cartitem.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/khash.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/payment.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/version.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/
--rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/LICENSE
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      600 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/README.md
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-08-02 19:00:55.902504 kount_ris_sdk-3.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/setup.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.894504 kount_ris_sdk-3.4.4/src/
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/src/kount/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/client.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/config.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/inquiry.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    13906 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/request.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/src/kount/resources/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/resources/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/resources/correct_key_cryp.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/response.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/settings.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/src/kount/util/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/a85.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/address.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/cartitem.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/khash.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/util/payment.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-08-02 19:00:51.000000 kount_ris_sdk-3.4.4/src/kount/version.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-08-02 19:00:55.898504 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-08-02 19:00:55.000000 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-08-02 19:00:55.000000 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-08-02 19:00:55.000000 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-08-02 19:00:55.000000 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-08-02 19:00:55.000000 kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/top_level.txt
```

### Comparing `kount_ris_sdk-3.4.3/LICENSE` & `kount_ris_sdk-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/PKG-INFO` & `kount_ris_sdk-3.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kount_ris_sdk
-Version: 3.4.3
+Version: 3.4.4
 Summary: Kount Python RIS SDK
 Home-page: https://github.com/Kount/kount-ris-python-sdk
 Author: Kount
 Author-email: sdkadmin@kount.com
 License: Kount
 Keywords: kount,sdk,ris
 Platform: any
```

### Comparing `kount_ris_sdk-3.4.3/README.md` & `kount_ris_sdk-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/setup.py` & `kount_ris_sdk-3.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/__init__.py` & `kount_ris_sdk-3.4.4/src/kount/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/client.py` & `kount_ris_sdk-3.4.4/src/kount/client.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/config.py` & `kount_ris_sdk-3.4.4/src/kount/config.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/inquiry.py` & `kount_ris_sdk-3.4.4/src/kount/inquiry.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/request.py` & `kount_ris_sdk-3.4.4/src/kount/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,16 +301,16 @@
         """Encodes the provided payment token according to the MASK
            encoding scheme
            Args: token -  the Payment token for this request
            return - MASK-encoded token
         """
         encoded = token[0:6]
         for _ in range(6, len(token) - 4, 1):
-            encoded.append('X')
-        encoded.append(token[-4:])
+            encoded = encoded + 'X'
+        encoded = encoded + token[-4:]
         LOG.debug("mask_token = %s", token)
         return encoded
 
     def set_payment_by_type(self, ptyp, ptok):
         """ Set a payment by payment type and payment token.
         The payment type parameter provided is checked
         if it's one of the predefined payment types
@@ -341,15 +341,15 @@
         If the provided Payment parameter is not a card payment,
         standard encoding will be applied.
         This method sets the following RIS Request fields:
         PTOK, PTYP, LAST4, PENC.
         Args: payment - card payment
         """
         token = payment.payment_token
-        if isinstance(self.payment, payment.CardPayment) and \
+        if isinstance(payment, payments.CardPayment) and \
                 not payment.khashed:
             token = self._mask_token(token)
             self.set_param("PTOK", token)
             self.set_param("PTYP", payment.payment_type)
             self.set_param("LAST4", payment.last4)
             self.set_param("PENC", "MASK")
         else:
```

### Comparing `kount_ris_sdk-3.4.3/src/kount/resources/correct_key_cryp.py` & `kount_ris_sdk-3.4.4/src/kount/resources/correct_key_cryp.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/response.py` & `kount_ris_sdk-3.4.4/src/kount/response.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/util/__init__.py` & `kount_ris_sdk-3.4.4/src/kount/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/util/address.py` & `kount_ris_sdk-3.4.4/src/kount/util/address.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/util/cartitem.py` & `kount_ris_sdk-3.4.4/src/kount/util/cartitem.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/util/khash.py` & `kount_ris_sdk-3.4.4/src/kount/util/khash.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount/util/payment.py` & `kount_ris_sdk-3.4.4/src/kount/util/payment.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/PKG-INFO` & `kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kount-ris-sdk
-Version: 3.4.3
+Version: 3.4.4
 Summary: Kount Python RIS SDK
 Home-page: https://github.com/Kount/kount-ris-python-sdk
 Author: Kount
 Author-email: sdkadmin@kount.com
 License: Kount
 Keywords: kount,sdk,ris
 Platform: any
```

### Comparing `kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/SOURCES.txt` & `kount_ris_sdk-3.4.4/src/kount_ris_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

