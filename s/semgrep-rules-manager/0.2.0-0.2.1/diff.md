# Comparing `tmp/semgrep_rules_manager-0.2.0.tar.gz` & `tmp/semgrep_rules_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semgrep_rules_manager-0.2.0.tar", max compression
+gzip compressed data, was "semgrep_rules_manager-0.2.1.tar", max compression
```

## Comparing `semgrep_rules_manager-0.2.0.tar` & `semgrep_rules_manager-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0     1818 2023-08-01 08:51:28.710258 semgrep_rules_manager-0.2.0/README.pypi.md
--rw-r--r--   0        0        0     1437 2023-08-01 08:59:07.269003 semgrep_rules_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.2.0/semgrep_rules_manager/__init__.py
--rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.2.0/semgrep_rules_manager/cli.py
--rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.2.0/semgrep_rules_manager/core.py
--rw-r--r--   0        0        0     1590 2023-08-01 08:51:22.410389 semgrep_rules_manager-0.2.0/semgrep_rules_manager/data/sources.yaml
--rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.2.0/semgrep_rules_manager/exception.py
--rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.2.0/semgrep_rules_manager/sources.py
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4815 2023-08-02 05:23:47.717061 semgrep_rules_manager-0.2.1/README.pypi.md
+-rw-r--r--   0        0        0     1437 2023-08-02 09:10:18.030521 semgrep_rules_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.2.1/semgrep_rules_manager/__init__.py
+-rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.2.1/semgrep_rules_manager/cli.py
+-rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.2.1/semgrep_rules_manager/core.py
+-rw-r--r--   0        0        0     1590 2023-08-01 08:51:22.410389 semgrep_rules_manager-0.2.1/semgrep_rules_manager/data/sources.yaml
+-rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.2.1/semgrep_rules_manager/exception.py
+-rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.2.1/semgrep_rules_manager/sources.py
+-rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.2.1/PKG-INFO
```

### Comparing `semgrep_rules_manager-0.2.0/LICENSE` & `semgrep_rules_manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.2.0/pyproject.toml` & `semgrep_rules_manager-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semgrep_rules_manager"
-version = "0.2.0"
+version = "0.2.1"
 description = "Manager of third-party Semgrep rules"
 keywords = ["semgrep", "semgrep-rules", "semgrep-rules-manager", "sast"]
 authors = ["George-Andrei Iosif <andrei.iosif@canonical.com>"]
 readme = "README.pypi.md"
 license = "MIT"
 packages = [{include = "semgrep_rules_manager"}]
 repository = "https://github.com/iosifache/semgrep-rules-manager"
```

### Comparing `semgrep_rules_manager-0.2.0/semgrep_rules_manager/cli.py` & `semgrep_rules_manager-0.2.1/semgrep_rules_manager/cli.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.2.0/semgrep_rules_manager/core.py` & `semgrep_rules_manager-0.2.1/semgrep_rules_manager/core.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.2.0/semgrep_rules_manager/data/sources.yaml` & `semgrep_rules_manager-0.2.1/semgrep_rules_manager/data/sources.yaml`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.2.0/semgrep_rules_manager/sources.py` & `semgrep_rules_manager-0.2.1/semgrep_rules_manager/sources.py`

 * *Files identical despite different names*

