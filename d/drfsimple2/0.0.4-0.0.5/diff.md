# Comparing `tmp/drfsimple2-0.0.4.tar.gz` & `tmp/drfsimple2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-hlwuq4be\drfsimple2-0.0.4.tar", last modified: Wed Aug  2 11:34:36 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-pno692e3\drfsimple2-0.0.5.tar", last modified: Wed Aug  2 13:20:44 2023, max compression
```

## Comparing `drfsimple2-0.0.4.tar` & `drfsimple2-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.170705 drfsimple2-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      702 2023-08-02 11:34:36.170705 drfsimple2-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-08-02 10:34:55.000000 drfsimple2-0.0.4/README.md
--rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.068270 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.104940 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
--rw-rw-rw-   0        0        0      702 2023-08-02 11:34:36.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3191 2023-08-02 11:34:36.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 11:34:36.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 11:34:36.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.127081 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/
--rw-rw-rw-   0        0        0      230 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
--rw-rw-rw-   0        0        0     5508 2023-08-02 11:33:53.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
--rw-rw-rw-   0        0        0     4666 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
--rw-rw-rw-   0        0        0     1300 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
--rw-rw-rw-   0        0        0      994 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
--rw-rw-rw-   0        0        0     3010 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
--rw-rw-rw-   0        0        0     5214 2023-08-02 10:33:19.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
--rw-rw-rw-   0        0        0     3234 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py
--rw-rw-rw-   0        0        0      327 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/state.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.134497 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/
--rw-rw-rw-   0        0        0      159 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2292 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      281 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.136851 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.140110 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/flushexpiredtokens.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:34:36.169462 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/
--rw-rw-rw-   0        0        0     2004 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      367 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
--rw-rw-rw-   0        0        0      907 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py
--rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0004_auto_20171017_2013.py
--rw-rw-rw-   0        0        0      294 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
--rw-rw-rw-   0        0        0      339 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0006_auto_20171017_2113.py
--rw-rw-rw-   0        0        0      760 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py
--rw-rw-rw-   0        0        0      692 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      693 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      578 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py
--rw-rw-rw-   0        0        0      699 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-08-02 04:32:39.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py
--rw-rw-rw-   0        0        0    11049 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py
--rw-rw-rw-   0        0        0      651 2023-07-22 18:34:57.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py
--rw-rw-rw-   0        0        0     3273 2023-08-02 10:32:39.000000 drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py
--rw-rw-rw-   0        0        0      812 2023-08-02 11:34:36.172722 drfsimple2-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.776028 drfsimple2-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-08-02 13:20:44.777030 drfsimple2-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-08-02 13:20:32.000000 drfsimple2-0.0.5/README.md
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.624724 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.666775 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-08-02 13:20:44.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3191 2023-08-02 13:20:44.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:20:44.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 13:20:44.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.704256 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/
+-rw-rw-rw-   0        0        0      230 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
+-rw-rw-rw-   0        0        0     5508 2023-08-02 11:33:53.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
+-rw-rw-rw-   0        0        0     4666 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
+-rw-rw-rw-   0        0        0     1300 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
+-rw-rw-rw-   0        0        0      994 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
+-rw-rw-rw-   0        0        0     3010 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
+-rw-rw-rw-   0        0        0     5214 2023-08-02 10:33:19.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
+-rw-rw-rw-   0        0        0     3234 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py
+-rw-rw-rw-   0        0        0      327 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/state.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.720023 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/
+-rw-rw-rw-   0        0        0      159 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2292 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      281 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.724032 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.732889 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/flushexpiredtokens.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:20:44.775029 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/
+-rw-rw-rw-   0        0        0     2004 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      367 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-rw-rw-   0        0        0      907 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-rw-rw-   0        0        0      294 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-rw-rw-   0        0        0      339 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-rw-rw-   0        0        0      692 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      693 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      578 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py
+-rw-rw-rw-   0        0        0      699 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-08-02 04:32:39.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py
+-rw-rw-rw-   0        0        0    11049 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py
+-rw-rw-rw-   0        0        0      651 2023-07-22 18:34:57.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py
+-rw-rw-rw-   0        0        0     3273 2023-08-02 10:32:39.000000 drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py
+-rw-rw-rw-   0        0        0      812 2023-08-02 13:20:44.794145 drfsimple2-0.0.5/setup.cfg
```

### Comparing `drfsimple2-0.0.4/PKG-INFO` & `drfsimple2-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.4
+Version: 0.0.5
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Hello World
 
-remove regular rest_framework_simplejwt be for installing drksimple2
+remove regular rest_framework_simplejwt before installing drksimple2
```

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.4
+Version: 0.0.5
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Hello World
 
-remove regular rest_framework_simplejwt be for installing drksimple2
+remove regular rest_framework_simplejwt before installing drksimple2
```

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py` & `drfsimple2-0.0.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.4/setup.cfg` & `drfsimple2-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 7369 6d70 6c65 320d 0a76   = drfsimple2..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
 00000030: 6175 7468 6f72 203d 2046 6f72 6465 0d0a  author = Forde..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2066  author_email = f
 00000050: 6f72 2e64 6576 406f 7574 6c6f 6f6b 2e63  or.dev@outlook.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 6669 7865 6420 5f69 6420 6669 656c  = fixed _id fiel
 00000080: 6473 2074 6f20 776f 726b 2077 6974 6820  ds to work with 
 00000090: 7079 6d6f 6e67 6f20 616e 6420 646a 6f6e  pymongo and djon
```

