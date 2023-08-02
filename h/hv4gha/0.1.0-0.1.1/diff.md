# Comparing `tmp/hv4gha-0.1.0.tar.gz` & `tmp/hv4gha-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hv4gha-0.1.0.tar", max compression
+gzip compressed data, was "hv4gha-0.1.1.tar", max compression
```

## Comparing `hv4gha-0.1.0.tar` & `hv4gha-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-30 08:46:36.589455 hv4gha-0.1.0/LICENSE
--rw-r--r--   0        0        0     2646 2023-07-30 08:46:36.589455 hv4gha-0.1.0/README.md
--rw-r--r--   0        0        0      355 2023-07-30 08:46:36.589455 hv4gha-0.1.0/hv4gha/__init__.py
--rw-r--r--   0        0        0     2557 2023-07-30 08:46:36.589455 hv4gha-0.1.0/hv4gha/entry.py
--rw-r--r--   0        0        0     4586 2023-07-30 08:46:36.589455 hv4gha-0.1.0/hv4gha/gh.py
--rw-r--r--   0        0        0        0 2023-07-30 08:46:36.589455 hv4gha-0.1.0/hv4gha/py.typed
--rw-r--r--   0        0        0     6566 2023-07-30 08:46:36.589455 hv4gha-0.1.0/hv4gha/vault.py
--rw-r--r--   0        0        0      679 2023-07-30 08:46:36.589455 hv4gha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 hv4gha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-02 16:20:13.730116 hv4gha-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2691 2023-08-02 16:20:13.730116 hv4gha-0.1.1/README.md
+-rw-r--r--   0        0        0      355 2023-08-02 16:20:13.730116 hv4gha-0.1.1/hv4gha/__init__.py
+-rw-r--r--   0        0        0     2557 2023-08-02 16:20:13.734116 hv4gha-0.1.1/hv4gha/entry.py
+-rw-r--r--   0        0        0     4586 2023-08-02 16:20:13.734116 hv4gha-0.1.1/hv4gha/gh.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:20:13.734116 hv4gha-0.1.1/hv4gha/py.typed
+-rw-r--r--   0        0        0     6566 2023-08-02 16:20:13.734116 hv4gha-0.1.1/hv4gha/vault.py
+-rw-r--r--   0        0        0      679 2023-08-02 16:20:13.734116 hv4gha-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 hv4gha-0.1.1/PKG-INFO
```

### Comparing `hv4gha-0.1.0/LICENSE` & `hv4gha-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hv4gha-0.1.0/README.md` & `hv4gha-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Hashicorp Vault for GitHub Apps
+# HashiCorp Vault for GitHub Apps
 
 Python library for using [HashiCorp Vault][1]'s [Transit Engine][2] to
 manage a GitHub App's private RSA key. More precisely, the library
 provides the following pieces of functionality.
 
 * Perform initial import of the App's private key into Vault
 * Have Vault sign the needed JWT and then request a GitHub Access Token
@@ -14,15 +14,15 @@
 ```shell
 pip install hv4gha
 ```
 
 ## Usage
 
 In addition to the examples below see also the
-[hv4gha/entry.py](hv4gha/entry.py) docstrings.
+[hv4gha/entry.py](https://github.com/andreaso/hv4gha/blob/main/hv4gha/entry.py) docstrings.
 
 ### Import App key
 
 ```python
 from hv4gha import import_app_key
 
 with open("/path/to/github-app.private-key.pem", "r") as akh:
```

### Comparing `hv4gha-0.1.0/hv4gha/entry.py` & `hv4gha-0.1.1/hv4gha/entry.py`

 * *Files identical despite different names*

### Comparing `hv4gha-0.1.0/hv4gha/gh.py` & `hv4gha-0.1.1/hv4gha/gh.py`

 * *Files identical despite different names*

### Comparing `hv4gha-0.1.0/hv4gha/vault.py` & `hv4gha-0.1.1/hv4gha/vault.py`

 * *Files identical despite different names*

### Comparing `hv4gha-0.1.0/PKG-INFO` & `hv4gha-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hv4gha
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use HashiCorp Vault to manage a GitHub App's private RSA key.
 Home-page: https://github.com/andreaso/hv4gha
 License: MIT
 Author: Andreas Olsson
 Author-email: andreas@arrakis.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=41.0.2,<42.0.0)
+Requires-Dist: cryptography (>=41.0.3,<42.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/andreaso/hv4gha
 Description-Content-Type: text/markdown
 
-# Hashicorp Vault for GitHub Apps
+# HashiCorp Vault for GitHub Apps
 
 Python library for using [HashiCorp Vault][1]'s [Transit Engine][2] to
 manage a GitHub App's private RSA key. More precisely, the library
 provides the following pieces of functionality.
 
 * Perform initial import of the App's private key into Vault
 * Have Vault sign the needed JWT and then request a GitHub Access Token
@@ -32,15 +32,15 @@
 ```shell
 pip install hv4gha
 ```
 
 ## Usage
 
 In addition to the examples below see also the
-[hv4gha/entry.py](hv4gha/entry.py) docstrings.
+[hv4gha/entry.py](https://github.com/andreaso/hv4gha/blob/main/hv4gha/entry.py) docstrings.
 
 ### Import App key
 
 ```python
 from hv4gha import import_app_key
 
 with open("/path/to/github-app.private-key.pem", "r") as akh:
```

