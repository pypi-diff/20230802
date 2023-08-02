# Comparing `tmp/panos_upgrade_assurance-0.1.2.tar.gz` & `tmp/panos_upgrade_assurance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.1.2.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.1.3.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.1.2.tar` & `panos_upgrade_assurance-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/LICENSE
--rw-r--r--   0        0        0      930 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    44638 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0     2472 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/exceptions.py
--rw-r--r--   0        0        0    39604 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    31684 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    12400 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0     1271 2023-07-19 01:44:40.161096 panos_upgrade_assurance-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-08-02 06:29:57.279485 panos_upgrade_assurance-0.1.3/LICENSE
+-rw-r--r--   0        0        0      930 2023-08-02 06:29:57.279485 panos_upgrade_assurance-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    44638 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2472 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    39719 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31684 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    12400 2023-08-02 06:29:57.283485 panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1271 2023-08-02 06:30:23.756152 panos_upgrade_assurance-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.3/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.1.2/LICENSE` & `panos_upgrade_assurance-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/README.md` & `panos_upgrade_assurance-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/check_firewall.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/exceptions.py` & `panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -873,15 +873,17 @@
             mount_point = row_items_trimmed[-1]
             try:
                 free_size_short = row_items_trimmed[3]
                 free_size_name = free_size_short[-1]
                 free_size_number = float(free_size_short[0:-1])
 
                 if not free_size_name.isnumeric():
-                    if free_size_name == "G":
+                    if free_size_name == "T":
+                        free_size = free_size_number * 1024 * 1024
+                    elif free_size_name == "G":
                         free_size = free_size_number * 1024
                     elif free_size_name == "M":
                         free_size = free_size_number
                     elif free_size_name == "K":
                         free_size = free_size_number / 1024
                     else:
                         raise exceptions.WrongDiskSizeFormatException("Free disk size has wrong format.")
```

### Comparing `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.1.3/panos_upgrade_assurance/utils.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.2/pyproject.toml` & `panos_upgrade_assurance-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
```

### Comparing `panos_upgrade_assurance-0.1.2/PKG-INFO` & `panos_upgrade_assurance-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

