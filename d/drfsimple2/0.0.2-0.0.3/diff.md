# Comparing `tmp/drfsimple2-0.0.2.tar.gz` & `tmp/drfsimple2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-4nvx1us5\drfsimple2-0.0.2.tar", last modified: Wed Aug  2 04:33:42 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-axyocm97\drfsimple2-0.0.3.tar", last modified: Wed Aug  2 10:35:21 2023, max compression
```

## Comparing `drfsimple2-0.0.2.tar` & `drfsimple2-0.0.3.tar`

### file list

```diff
@@ -1,72 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.778046 drfsimple2-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      630 2023-08-02 04:33:42.778553 drfsimple2-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-08-02 03:20:49.000000 drfsimple2-0.0.2/README.md
--rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.572323 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.617349 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/
--rw-rw-rw-   0        0        0      211 2023-08-02 03:15:34.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py
--rw-rw-rw-   0        0        0     4666 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/backends.py
--rw-rw-rw-   0        0        0     1300 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/compat.py
--rw-rw-rw-   0        0        0      994 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py
--rw-rw-rw-   0        0        0     3010 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/models.py
--rw-rw-rw-   0        0        0     4905 2023-08-02 03:20:07.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py
--rw-rw-rw-   0        0        0     3030 2023-08-02 03:18:19.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/settings.py
--rw-rw-rw-   0        0        0      327 2023-08-02 03:20:02.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/state.py
--rw-rw-rw-   0        0        0       68 2023-07-17 07:47:52.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/test.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.656523 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/
--rw-rw-rw-   0        0        0      145 2023-08-02 03:19:40.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      267 2023-08-02 03:19:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.658030 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.664409 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      356 2023-08-02 03:19:53.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/flushexpiredtokens.py
--rw-rw-rw-   0        0        0     1618 2023-08-02 03:56:21.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py
--rw-rw-rw-   0        0        0    11022 2023-08-02 03:18:36.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py
--rw-rw-rw-   0        0        0      651 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/utils.py
--rw-rw-rw-   0        0        0     3265 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/views.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.645039 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
--rw-rw-rw-   0        0        0      630 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4487 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.697404 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/
--rw-rw-rw-   0        0        0      230 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
--rw-rw-rw-   0        0        0     4666 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
--rw-rw-rw-   0        0        0     1300 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
--rw-rw-rw-   0        0        0      994 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
--rw-rw-rw-   0        0        0     3010 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
--rw-rw-rw-   0        0        0     4919 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
--rw-rw-rw-   0        0        0     3234 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py
--rw-rw-rw-   0        0        0      327 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/state.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.735238 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/
--rw-rw-rw-   0        0        0      159 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2292 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      281 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.741756 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.745142 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/flushexpiredtokens.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.776042 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/
--rw-rw-rw-   0        0        0     2004 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      367 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
--rw-rw-rw-   0        0        0      907 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py
--rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0004_auto_20171017_2013.py
--rw-rw-rw-   0        0        0      294 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
--rw-rw-rw-   0        0        0      339 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0006_auto_20171017_2113.py
--rw-rw-rw-   0        0        0      760 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py
--rw-rw-rw-   0        0        0      692 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      693 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      578 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py
--rw-rw-rw-   0        0        0      699 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
--rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-08-02 04:32:39.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py
--rw-rw-rw-   0        0        0    11049 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py
--rw-rw-rw-   0        0        0      651 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py
--rw-rw-rw-   0        0        0     3265 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py
--rw-rw-rw-   0        0        0      812 2023-08-02 04:33:42.780868 drfsimple2-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.407766 drfsimple2-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-08-02 10:35:21.407766 drfsimple2-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-08-02 10:34:55.000000 drfsimple2-0.0.3/README.md
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.291672 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.328871 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-08-02 10:35:21.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3191 2023-08-02 10:35:21.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:35:21.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 10:35:21.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.356695 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/
+-rw-rw-rw-   0        0        0      230 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
+-rw-rw-rw-   0        0        0     5405 2023-08-02 10:32:53.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
+-rw-rw-rw-   0        0        0     4666 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
+-rw-rw-rw-   0        0        0     1300 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
+-rw-rw-rw-   0        0        0      994 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
+-rw-rw-rw-   0        0        0     3010 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
+-rw-rw-rw-   0        0        0     5214 2023-08-02 10:33:19.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
+-rw-rw-rw-   0        0        0     3234 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py
+-rw-rw-rw-   0        0        0      327 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/state.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.365090 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/
+-rw-rw-rw-   0        0        0      159 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2292 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      281 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.369598 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.374207 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/flushexpiredtokens.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:35:21.406762 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/
+-rw-rw-rw-   0        0        0     2004 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      367 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-rw-rw-   0        0        0      907 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-rw-rw-   0        0        0      294 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-rw-rw-   0        0        0      339 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-rw-rw-   0        0        0      692 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      693 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      578 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py
+-rw-rw-rw-   0        0        0      699 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-08-02 04:32:39.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py
+-rw-rw-rw-   0        0        0    11049 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py
+-rw-rw-rw-   0        0        0      651 2023-07-22 18:34:57.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py
+-rw-rw-rw-   0        0        0     3273 2023-08-02 10:32:39.000000 drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py
+-rw-rw-rw-   0        0        0      812 2023-08-02 10:35:21.412638 drfsimple2-0.0.3/setup.cfg
```

### Comparing `drfsimple2-0.0.2/PKG-INFO` & `drfsimple2-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.2
+Version: 0.0.3
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
+
+remove regular rest_framework_simplejwt be for installing drksimple2
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib.auth import get_user_model
 from django.utils.translation import gettext_lazy as _
 from rest_framework import HTTP_HEADER_ENCODING, authentication
+from bson.objectid import ObjectId
 
 from .exceptions import AuthenticationFailed, InvalidToken, TokenError
 from .settings import api_settings
 
 AUTH_HEADER_TYPES = api_settings.AUTH_HEADER_TYPES
 
 if not isinstance(api_settings.AUTH_HEADER_TYPES, (list, tuple)):
@@ -112,18 +113,19 @@
         """
         try:
             user_id = validated_token[api_settings.USER_ID_CLAIM]
         except KeyError:
             raise InvalidToken(_("Token contained no recognizable user identification"))
 
         try:
-            user = self.user_model.objects.get(**{api_settings.USER_ID_FIELD: user_id})
+            user = self.user_model.objects.get(_id=ObjectId(user_id))
         except self.user_model.DoesNotExist:
             raise AuthenticationFailed(_("User not found"), code="user_not_found")
 
+
         if not user.is_active:
             raise AuthenticationFailed(_("User is inactive"), code="user_inactive")
 
         return user
 
 
 class JWTStatelessUserAuthentication(JWTAuthentication):
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/backends.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/compat.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/models.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.conf import settings
 from django.contrib.auth import authenticate, get_user_model
 from django.contrib.auth.models import update_last_login
 from django.utils.translation import gettext_lazy as _
 from rest_framework import exceptions, serializers
 from rest_framework.exceptions import ValidationError
+from bson.objectid import ObjectId
+from account.models import Account
 
 from .settings import api_settings
 from .tokens import RefreshToken, SlidingToken, UntypedToken
 
 if api_settings.BLACKLIST_AFTER_ROTATION:
     from .token_blacklist.models import BlacklistedToken
 
@@ -28,29 +30,35 @@
 
     default_error_messages = {
         "no_active_account": _("No active account found with the given credentials")
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-
+        
         self.fields[self.username_field] = serializers.CharField()
         self.fields["password"] = PasswordField()
 
+
     def validate(self, attrs):
         authenticate_kwargs = {
             self.username_field: attrs[self.username_field],
             "password": attrs["password"],
         }
         try:
             authenticate_kwargs["request"] = self.context["request"]
         except KeyError:
             pass
-
-        self.user = authenticate(**authenticate_kwargs)
+        
+        try:
+            self.user = Account.objects.get(email=authenticate_kwargs["email"])
+            if self.user.check_password(authenticate_kwargs["password"]):
+                self.user = self.user
+        except Account.DoesNotExist:
+            return {}
 
         if not api_settings.USER_AUTHENTICATION_RULE(self.user):
             raise exceptions.AuthenticationFailed(
                 self.error_messages["no_active_account"],
                 "no_active_account",
             )
 
@@ -145,15 +153,15 @@
     token = serializers.CharField()
 
     def validate(self, attrs):
         token = UntypedToken(attrs["token"])
 
         if (
             api_settings.BLACKLIST_AFTER_ROTATION
-            and "drfsimple2.token_blacklist" in settings.INSTALLED_APPS
+            and "rest_framework_simplejwt.token_blacklist" in settings.INSTALLED_APPS
         ):
             jti = token.get(api_settings.JTI_CLAIM)
             if BlacklistedToken.objects.filter(token__jti=jti).exists():
                 raise ValidationError("Token is blacklisted")
 
         return {}
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/settings.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     "JSON_ENCODER": None,
     "JWK_URL": None,
     "LEEWAY": 0,
     "AUTH_HEADER_TYPES": ("Bearer",),
     "AUTH_HEADER_NAME": "HTTP_AUTHORIZATION",
     "USER_ID_FIELD": "id",
     "USER_ID_CLAIM": "user_id",
-    "USER_AUTHENTICATION_RULE": "drfsimple2.authentication.default_user_authentication_rule",
-    "AUTH_TOKEN_CLASSES": ("drfsimple2.tokens.AccessToken",),
+    "USER_AUTHENTICATION_RULE": "rest_framework_simplejwt.authentication.default_user_authentication_rule",
+    "AUTH_TOKEN_CLASSES": ("rest_framework_simplejwt.tokens.AccessToken",),
     "TOKEN_TYPE_CLAIM": "token_type",
     "JTI_CLAIM": "jti",
-    "TOKEN_USER_CLASS": "drfsimple2.models.TokenUser",
+    "TOKEN_USER_CLASS": "rest_framework_simplejwt.models.TokenUser",
     "SLIDING_TOKEN_REFRESH_EXP_CLAIM": "refresh_exp",
     "SLIDING_TOKEN_LIFETIME": timedelta(minutes=5),
     "SLIDING_TOKEN_REFRESH_LIFETIME": timedelta(days=1),
-    "TOKEN_OBTAIN_SERIALIZER": "drfsimple2.serializers.TokenObtainPairSerializer",
-    "TOKEN_REFRESH_SERIALIZER": "drfsimple2.serializers.TokenRefreshSerializer",
-    "TOKEN_VERIFY_SERIALIZER": "drfsimple2.serializers.TokenVerifySerializer",
-    "TOKEN_BLACKLIST_SERIALIZER": "drfsimple2.serializers.TokenBlacklistSerializer",
-    "SLIDING_TOKEN_OBTAIN_SERIALIZER": "drfsimple2.serializers.TokenObtainSlidingSerializer",
-    "SLIDING_TOKEN_REFRESH_SERIALIZER": "drfsimple2.serializers.TokenRefreshSlidingSerializer",
+    "TOKEN_OBTAIN_SERIALIZER": "rest_framework_simplejwt.serializers.TokenObtainPairSerializer",
+    "TOKEN_REFRESH_SERIALIZER": "rest_framework_simplejwt.serializers.TokenRefreshSerializer",
+    "TOKEN_VERIFY_SERIALIZER": "rest_framework_simplejwt.serializers.TokenVerifySerializer",
+    "TOKEN_BLACKLIST_SERIALIZER": "rest_framework_simplejwt.serializers.TokenBlacklistSerializer",
+    "SLIDING_TOKEN_OBTAIN_SERIALIZER": "rest_framework_simplejwt.serializers.TokenObtainSlidingSerializer",
+    "SLIDING_TOKEN_REFRESH_SERIALIZER": "rest_framework_simplejwt.serializers.TokenRefreshSlidingSerializer",
 }
 
 IMPORT_STRINGS = (
     "AUTH_TOKEN_CLASSES",
     "JSON_ENCODER",
     "TOKEN_USER_CLASS",
     "USER_AUTHENTICATION_RULE",
@@ -56,15 +56,15 @@
     "SECRET_KEY",
     "TOKEN_BACKEND_CLASS",
 )
 
 
 class APISettings(_APISettings):  # pragma: no cover
     def __check_user_settings(self, user_settings):
-        SETTINGS_DOC = ""
+        SETTINGS_DOC = "https://django-rest-framework-simplejwt.readthedocs.io/en/latest/settings.html"
 
         for setting in REMOVED_SETTINGS:
             if setting in user_settings:
                 raise RuntimeError(
                     format_lazy(
                         _(
                             "The '{}' setting has been removed. Please refer to '{}' for available settings."
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
 from .models import BlacklistedToken, OutstandingToken
 
+
 class OutstandingTokenAdmin(admin.ModelAdmin):
     list_display = (
         "jti",
         "user",
         "created_at",
         "expires_at",
     )
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.conf import settings
-# from django.db import models
 from djongo import models
 
+
 class OutstandingToken(models.Model):
     _id = models.ObjectIdField()
     user = models.ForeignKey(
         settings.AUTH_USER_MODEL, on_delete=models.SET_NULL, null=True, blank=True
     )
 
     jti = models.CharField(unique=True, max_length=255)
@@ -20,14 +20,15 @@
         #
         # Also see corresponding ticket:
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
             "rest_framework_simplejwt.token_blacklist" not in settings.INSTALLED_APPS
         )
         ordering = ("user",)
+        db_table = "outstanding_tokens"
 
     def __str__(self):
         return "Token for {} ({})".format(
             self.user,
             self.jti,
         )
 
@@ -43,10 +44,11 @@
         # https://code.djangoproject.com/ticket/19422
         #
         # Also see corresponding ticket:
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
             "rest_framework_simplejwt.token_blacklist" not in settings.INSTALLED_APPS
         )
+        db_table = "blacklisted_tokens"
 
     def __str__(self):
         return f"Blacklisted token for {self.token.user}"
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     _token_backend = None
 
     @property
     def token_backend(self):
         if self._token_backend is None:
             self._token_backend = import_string(
-                "drfsimple2.state.token_backend"
+                "rest_framework_simplejwt.state.token_backend"
             )
         return self._token_backend
 
     def get_token_backend(self):
         # Backward compatibility.
         return self.token_backend
 
@@ -208,15 +208,15 @@
     """
     If the `rest_framework_simplejwt.token_blacklist` app was configured to be
     used, tokens created from `BlacklistMixin` subclasses will insert
     themselves into an outstanding token list and also check for their
     membership in a token blacklist.
     """
 
-    if "drfsimeple2.token_blacklist" in settings.INSTALLED_APPS:
+    if "rest_framework_simplejwt.token_blacklist" in settings.INSTALLED_APPS:
 
         def verify(self, *args, **kwargs):
             self.check_blacklist()
 
             super().verify(*args, **kwargs)
 
         def check_blacklist(self):
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/utils.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/views.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return '{} realm="{}"'.format(
             AUTH_HEADER_TYPES[0],
             self.www_authenticate_realm,
         )
 
     def post(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data)
-
+        
         try:
             serializer.is_valid(raise_exception=True)
         except TokenError as e:
             raise InvalidToken(e.args[0])
 
         return Response(serializer.validated_data, status=status.HTTP_200_OK)
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.2
+Version: 0.0.3
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
+
+remove regular rest_framework_simplejwt be for installing drksimple2
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-rest_framework_simplejwt_byforde2/drfsimple2/__init__.py
-rest_framework_simplejwt_byforde2/drfsimple2/authentication.py
-rest_framework_simplejwt_byforde2/drfsimple2/backends.py
-rest_framework_simplejwt_byforde2/drfsimple2/compat.py
-rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py
-rest_framework_simplejwt_byforde2/drfsimple2/models.py
-rest_framework_simplejwt_byforde2/drfsimple2/serializers.py
-rest_framework_simplejwt_byforde2/drfsimple2/settings.py
-rest_framework_simplejwt_byforde2/drfsimple2/state.py
-rest_framework_simplejwt_byforde2/drfsimple2/test.py
-rest_framework_simplejwt_byforde2/drfsimple2/tokens.py
-rest_framework_simplejwt_byforde2/drfsimple2/utils.py
-rest_framework_simplejwt_byforde2/drfsimple2/views.py
 rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
 rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
 rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
 rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/__init__.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/apps.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/__init__.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/__init__.py
-rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/flushexpiredtokens.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
 rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
```

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py` & `drfsimple2-0.0.3/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.2/setup.cfg` & `drfsimple2-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 7369 6d70 6c65 320d 0a76   = drfsimple2..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
 00000030: 6175 7468 6f72 203d 2046 6f72 6465 0d0a  author = Forde..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2066  author_email = f
 00000050: 6f72 2e64 6576 406f 7574 6c6f 6f6b 2e63  or.dev@outlook.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 6669 7865 6420 5f69 6420 6669 656c  = fixed _id fiel
 00000080: 6473 2074 6f20 776f 726b 2077 6974 6820  ds to work with 
 00000090: 7079 6d6f 6e67 6f20 616e 6420 646a 6f6e  pymongo and djon
```

