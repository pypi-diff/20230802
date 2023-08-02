# Comparing `tmp/drfsimple2-0.0.1.tar.gz` & `tmp/drfsimple2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-wxt23m7a\drfsimple2-0.0.1.tar", last modified: Wed Aug  2 03:21:55 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-4nvx1us5\drfsimple2-0.0.2.tar", last modified: Wed Aug  2 04:33:42 2023, max compression
```

## Comparing `drfsimple2-0.0.1.tar` & `drfsimple2-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.723517 drfsimple2-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      630 2023-08-02 03:21:55.723517 drfsimple2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-08-02 03:20:49.000000 drfsimple2-0.0.1/README.md
--rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.634853 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.675823 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/
--rw-rw-rw-   0        0        0      211 2023-08-02 03:15:34.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py
--rw-rw-rw-   0        0        0     4666 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/backends.py
--rw-rw-rw-   0        0        0     1300 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/compat.py
--rw-rw-rw-   0        0        0      994 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py
--rw-rw-rw-   0        0        0     3010 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/models.py
--rw-rw-rw-   0        0        0     4905 2023-08-02 03:20:07.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py
--rw-rw-rw-   0        0        0     3030 2023-08-02 03:18:19.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/settings.py
--rw-rw-rw-   0        0        0      327 2023-08-02 03:20:02.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/state.py
--rw-rw-rw-   0        0        0       68 2023-07-17 07:47:52.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/test.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.710492 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/
--rw-rw-rw-   0        0        0      145 2023-08-02 03:19:40.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      267 2023-08-02 03:19:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.716741 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.720739 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      356 2023-08-02 03:19:53.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/flushexpiredtokens.py
--rw-rw-rw-   0        0        0     1590 2023-08-02 03:19:17.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py
--rw-rw-rw-   0        0        0    11022 2023-08-02 03:18:36.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py
--rw-rw-rw-   0        0        0      651 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/utils.py
--rw-rw-rw-   0        0        0     3265 2023-06-30 12:37:25.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/views.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:21:55.702662 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
--rw-rw-rw-   0        0        0      630 2023-08-02 03:21:55.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1610 2023-08-02 03:21:55.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 03:21:55.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 03:21:55.000000 drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2023-08-02 03:21:55.726002 drfsimple2-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.778046 drfsimple2-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 drfsimple2-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      630 2023-08-02 04:33:42.778553 drfsimple2-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-08-02 03:20:49.000000 drfsimple2-0.0.2/README.md
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 drfsimple2-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.572323 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.617349 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/
+-rw-rw-rw-   0        0        0      211 2023-08-02 03:15:34.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/__init__.py
+-rw-rw-rw-   0        0        0     5387 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py
+-rw-rw-rw-   0        0        0     4666 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/backends.py
+-rw-rw-rw-   0        0        0     1300 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/compat.py
+-rw-rw-rw-   0        0        0      994 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py
+-rw-rw-rw-   0        0        0     3010 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/models.py
+-rw-rw-rw-   0        0        0     4905 2023-08-02 03:20:07.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py
+-rw-rw-rw-   0        0        0     3030 2023-08-02 03:18:19.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/settings.py
+-rw-rw-rw-   0        0        0      327 2023-08-02 03:20:02.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/state.py
+-rw-rw-rw-   0        0        0       68 2023-07-17 07:47:52.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/test.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.656523 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/
+-rw-rw-rw-   0        0        0      145 2023-08-02 03:19:40.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      267 2023-08-02 03:19:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.658030 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.664409 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      356 2023-08-02 03:19:53.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/management/commands/flushexpiredtokens.py
+-rw-rw-rw-   0        0        0     1618 2023-08-02 03:56:21.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py
+-rw-rw-rw-   0        0        0    11022 2023-08-02 03:18:36.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py
+-rw-rw-rw-   0        0        0      651 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/utils.py
+-rw-rw-rw-   0        0        0     3265 2023-06-30 12:37:25.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/views.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.645039 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/
+-rw-rw-rw-   0        0        0      630 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4487 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-08-02 04:33:42.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.697404 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/
+-rw-rw-rw-   0        0        0      230 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/__init__.py
+-rw-rw-rw-   0        0        0     5387 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/authentication.py
+-rw-rw-rw-   0        0        0     4666 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/backends.py
+-rw-rw-rw-   0        0        0     1300 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/compat.py
+-rw-rw-rw-   0        0        0      994 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/exceptions.py
+-rw-rw-rw-   0        0        0     3010 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/models.py
+-rw-rw-rw-   0        0        0     4919 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/serializers.py
+-rw-rw-rw-   0        0        0     3234 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/settings.py
+-rw-rw-rw-   0        0        0      327 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/state.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.735238 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/
+-rw-rw-rw-   0        0        0      159 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2292 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      281 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.741756 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.745142 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/management/commands/flushexpiredtokens.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:33:42.776042 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/
+-rw-rw-rw-   0        0        0     2004 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      367 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-rw-rw-   0        0        0      907 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-rw-rw-   0        0        0      370 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-rw-rw-   0        0        0      294 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-rw-rw-   0        0        0      339 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-rw-rw-   0        0        0      692 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      693 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      578 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0011_linearizes_history.py
+-rw-rw-rw-   0        0        0      699 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-08-02 04:32:39.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/token_blacklist/models.py
+-rw-rw-rw-   0        0        0    11049 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/tokens.py
+-rw-rw-rw-   0        0        0      651 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/utils.py
+-rw-rw-rw-   0        0        0     3265 2023-07-22 18:34:57.000000 drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt/views.py
+-rw-rw-rw-   0        0        0      812 2023-08-02 04:33:42.780868 drfsimple2-0.0.2/setup.cfg
```

### Comparing `drfsimple2-0.0.1/PKG-INFO` & `drfsimple2-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.1
+Version: 0.0.2
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/authentication.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/backends.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/backends.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/compat.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/compat.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/models.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/models.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/serializers.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/settings.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/settings.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/token_blacklist/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     class Meta:
         # Work around for a bug in Django:
         # https://code.djangoproject.com/ticket/19422
         #
         # Also see corresponding ticket:
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
-            "drfsimple2.token_blacklist" not in settings.INSTALLED_APPS
+            "rest_framework_simplejwt.token_blacklist" not in settings.INSTALLED_APPS
         )
         ordering = ("user",)
 
     def __str__(self):
         return "Token for {} ({})".format(
             self.user,
             self.jti,
@@ -41,12 +41,12 @@
     class Meta:
         # Work around for a bug in Django:
         # https://code.djangoproject.com/ticket/19422
         #
         # Also see corresponding ticket:
         # https://github.com/encode/django-rest-framework/issues/705
         abstract = (
-            "drfsimple2.token_blacklist" not in settings.INSTALLED_APPS
+            "rest_framework_simplejwt.token_blacklist" not in settings.INSTALLED_APPS
         )
 
     def __str__(self):
         return f"Blacklisted token for {self.token.user}"
```

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/tokens.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/utils.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/utils.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2/views.py` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2/views.py`

 * *Files identical despite different names*

### Comparing `drfsimple2-0.0.1/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO` & `drfsimple2-0.0.2/rest_framework_simplejwt_byforde2/drfsimple2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfsimple2
-Version: 0.0.1
+Version: 0.0.2
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drfsimple2-0.0.1/setup.cfg` & `drfsimple2-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 7369 6d70 6c65 320d 0a76   = drfsimple2..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
 00000030: 6175 7468 6f72 203d 2046 6f72 6465 0d0a  author = Forde..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2066  author_email = f
 00000050: 6f72 2e64 6576 406f 7574 6c6f 6f6b 2e63  or.dev@outlook.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 6669 7865 6420 5f69 6420 6669 656c  = fixed _id fiel
 00000080: 6473 2074 6f20 776f 726b 2077 6974 6820  ds to work with 
 00000090: 7079 6d6f 6e67 6f20 616e 6420 646a 6f6e  pymongo and djon
```

