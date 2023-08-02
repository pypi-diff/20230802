# Comparing `tmp/caluma_alexandria-2.0.0.tar.gz` & `tmp/caluma_alexandria-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma_alexandria-2.0.0.tar", max compression
+gzip compressed data, was "caluma_alexandria-2.0.1.tar", max compression
```

## Comparing `caluma_alexandria-2.0.0.tar` & `caluma_alexandria-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11730 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    35148 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/LICENSE
--rw-r--r--   0        0        0     4660 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/__init__.py
--rw-r--r--   0        0        0      863 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/apps.py
--rw-r--r--   0        0        0      195 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/collections.py
--rw-r--r--   0        0        0     1966 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/factories.py
--rw-r--r--   0        0        0     5022 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/filters.py
--rw-r--r--   0        0        0    13121 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0001_initial.py
--rw-r--r--   0        0        0      490 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0002_tags_monolingual.py
--rw-r--r--   0        0        0      644 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0003_file_upload_status.py
--rw-r--r--   0        0        0     2982 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0004_tag_synonym_group.py
--rw-r--r--   0        0        0     1065 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py
--rw-r--r--   0        0        0     1146 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
--rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/migrations/__init__.py
--rw-r--r--   0        0        0     6353 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/models.py
--rw-r--r--   0        0        0     4645 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/permissions.py
--rw-r--r--   0        0        0     6967 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/serializers.py
--rw-r--r--   0        0        0     2902 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/storage_clients.py
--rw-r--r--   0        0        0     1588 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/thumbs.py
--rw-r--r--   0        0        0      462 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/urls.py
--rw-r--r--   0        0        0     1754 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/validation.py
--rw-r--r--   0        0        0     6069 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/views.py
--rw-r--r--   0        0        0     5021 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/core/visibilities.py
--rw-r--r--   0        0        0        0 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/oidc_auth/__init__.py
--rw-r--r--   0        0        0     4224 2023-08-02 09:55:41.665165 caluma_alexandria-2.0.0/alexandria/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/oidc_auth/models.py
--rw-r--r--   0        0        0       30 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/__init__.py
--rw-r--r--   0        0        0     3816 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/alexandria.py
--rw-r--r--   0        0        0     4817 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/settings/django.py
--rw-r--r--   0        0        0      162 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/urls.py
--rw-r--r--   0        0        0      407 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/alexandria/wsgi.py
--rw-r--r--   0        0        0     2901 2023-08-02 09:55:41.669165 caluma_alexandria-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 caluma_alexandria-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11907 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35148 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4660 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/__init__.py
+-rw-r--r--   0        0        0      863 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/apps.py
+-rw-r--r--   0        0        0      195 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/collections.py
+-rw-r--r--   0        0        0     1966 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/factories.py
+-rw-r--r--   0        0        0     5022 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/filters.py
+-rw-r--r--   0        0        0    13121 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      490 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/migrations/0002_tags_monolingual.py
+-rw-r--r--   0        0        0      644 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/migrations/0003_file_upload_status.py
+-rw-r--r--   0        0        0     2982 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/migrations/0004_tag_synonym_group.py
+-rw-r--r--   0        0        0     1065 2023-08-02 12:35:10.845934 caluma_alexandria-2.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py
+-rw-r--r--   0        0        0     1146 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/migrations/__init__.py
+-rw-r--r--   0        0        0     6353 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/models.py
+-rw-r--r--   0        0        0     4645 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/permissions.py
+-rw-r--r--   0        0        0     6967 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/serializers.py
+-rw-r--r--   0        0        0     2902 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/storage_clients.py
+-rw-r--r--   0        0        0     1588 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/thumbs.py
+-rw-r--r--   0        0        0      462 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/urls.py
+-rw-r--r--   0        0        0     1754 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/validation.py
+-rw-r--r--   0        0        0     6069 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/views.py
+-rw-r--r--   0        0        0     5021 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/core/visibilities.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     4224 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/oidc_auth/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/settings/__init__.py
+-rw-r--r--   0        0        0     3816 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/settings/alexandria.py
+-rw-r--r--   0        0        0     4817 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/settings/django.py
+-rw-r--r--   0        0        0      162 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/urls.py
+-rw-r--r--   0        0        0      407 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/alexandria/wsgi.py
+-rw-r--r--   0        0        0     2901 2023-08-02 12:35:10.849934 caluma_alexandria-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 caluma_alexandria-2.0.1/PKG-INFO
```

### Comparing `caluma_alexandria-2.0.0/CHANGELOG.md` & `caluma_alexandria-2.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# v2.0.1
+### Fix
+* **settings:** Remove import in settings init file ([`3a86060`](https://github.com/projectcaluma/alexandria/commit/3a8606069ef257b8d8fa08d12e0cc46ab3d2e05c))
+
 # v2.0.0
 ### Fix
 * **docker:** Remove obsolete system dependencies ([`2e2f8a2`](https://github.com/projectcaluma/alexandria/commit/2e2f8a2081aa0603157d7df41e0981ac4824def4))
 * **settings:** Prefix alexandria settings ([`5791f3d`](https://github.com/projectcaluma/alexandria/commit/5791f3d8fbb7cf4a9fa37917ac2b1ac2a1b71ce2))
 
 ### Breaking
 * Removed image previews for RAW, VTK and scribus files. ([`2e2f8a2`](https://github.com/projectcaluma/alexandria/commit/2e2f8a2081aa0603157d7df41e0981ac4824def4))
```

### Comparing `caluma_alexandria-2.0.0/LICENSE` & `caluma_alexandria-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/README.md` & `caluma_alexandria-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/apps.py` & `caluma_alexandria-2.0.1/alexandria/core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/factories.py` & `caluma_alexandria-2.0.1/alexandria/core/factories.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/filters.py` & `caluma_alexandria-2.0.1/alexandria/core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/migrations/0001_initial.py` & `caluma_alexandria-2.0.1/alexandria/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/migrations/0003_file_upload_status.py` & `caluma_alexandria-2.0.1/alexandria/core/migrations/0003_file_upload_status.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/migrations/0004_tag_synonym_group.py` & `caluma_alexandria-2.0.1/alexandria/core/migrations/0004_tag_synonym_group.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/migrations/0005_rename_type_and_meta.py` & `caluma_alexandria-2.0.1/alexandria/core/migrations/0005_rename_type_and_meta.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py` & `caluma_alexandria-2.0.1/alexandria/core/migrations/0006_rename_metainfo_jsonfield_verbose_name.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/models.py` & `caluma_alexandria-2.0.1/alexandria/core/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/permissions.py` & `caluma_alexandria-2.0.1/alexandria/core/permissions.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/serializers.py` & `caluma_alexandria-2.0.1/alexandria/core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/storage_clients.py` & `caluma_alexandria-2.0.1/alexandria/core/storage_clients.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/thumbs.py` & `caluma_alexandria-2.0.1/alexandria/core/thumbs.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/validation.py` & `caluma_alexandria-2.0.1/alexandria/core/validation.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/views.py` & `caluma_alexandria-2.0.1/alexandria/core/views.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/core/visibilities.py` & `caluma_alexandria-2.0.1/alexandria/core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/oidc_auth/authentication.py` & `caluma_alexandria-2.0.1/alexandria/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/oidc_auth/models.py` & `caluma_alexandria-2.0.1/alexandria/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/settings/alexandria.py` & `caluma_alexandria-2.0.1/alexandria/settings/alexandria.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/alexandria/settings/django.py` & `caluma_alexandria-2.0.1/alexandria/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma_alexandria-2.0.0/pyproject.toml` & `caluma_alexandria-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma-alexandria"
-version = "2.0.0"
+version = "2.0.1"
 description = "Document management service"
 repository = "https://github.com/projectcaluma/alexandria"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `caluma_alexandria-2.0.0/PKG-INFO` & `caluma_alexandria-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma-alexandria
-Version: 2.0.0
+Version: 2.0.1
 Summary: Document management service
 Home-page: https://github.com/projectcaluma/alexandria
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

