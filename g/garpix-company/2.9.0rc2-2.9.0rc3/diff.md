# Comparing `tmp/garpix_company-2.9.0rc2.tar.gz` & `tmp/garpix_company-2.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.9.0rc2.tar", last modified: Thu Jul 27 11:38:53 2023, max compression
+gzip compressed data, was "garpix_company-2.9.0rc3.tar", last modified: Wed Aug  2 09:27:56 2023, max compression
```

## Comparing `garpix_company-2.9.0rc2.tar` & `garpix_company-2.9.0rc3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.293902 garpix_company-2.9.0rc2/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-07-27 11:38:53.293741 garpix_company-2.9.0rc2/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.272252 garpix_company-2.9.0rc2/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2821 2023-07-26 15:35:47.000000 garpix_company-2.9.0rc2/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc2/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.278260 garpix_company-2.9.0rc2/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.9.0rc2/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.9.0rc2/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.279564 garpix_company-2.9.0rc2/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.279708 garpix_company-2.9.0rc2/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.279808 garpix_company-2.9.0rc2/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.280035 garpix_company-2.9.0rc2/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.9.0rc2/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.289276 garpix_company-2.9.0rc2/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      222 2023-06-21 15:54:39.000000 garpix_company-2.9.0rc2/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6252 2023-06-21 15:49:16.000000 garpix_company-2.9.0rc2/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc2/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4539 2023-06-21 15:54:04.000000 garpix_company-2.9.0rc2/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc2/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.291861 garpix_company-2.9.0rc2/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc2/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1069 2023-06-21 15:51:24.000000 garpix_company-2.9.0rc2/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.9.0rc2/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      545 2023-06-21 15:50:30.000000 garpix_company-2.9.0rc2/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc2/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.292680 garpix_company-2.9.0rc2/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc2/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc2/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5838 2023-07-27 11:38:35.000000 garpix_company-2.9.0rc2/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc2/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.9.0rc2/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      926 2023-05-12 11:36:47.000000 garpix_company-2.9.0rc2/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.292943 garpix_company-2.9.0rc2/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc2/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.9.0rc2/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.9.0rc2/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-07-27 11:38:35.000000 garpix_company-2.9.0rc2/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc2/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc2/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.293529 garpix_company-2.9.0rc2/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.9.0rc2/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.9.0rc2/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.9.0rc2/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.9.0rc2/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 11:38:53.274985 garpix_company-2.9.0rc2/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-27 11:38:53.293951 garpix_company-2.9.0rc2/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-07-27 11:38:53.000000 garpix_company-2.9.0rc2/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.296766 garpix_company-2.9.0rc3/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-08-02 09:27:56.296634 garpix_company-2.9.0rc3/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.291958 garpix_company-2.9.0rc3/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2821 2023-07-26 15:35:47.000000 garpix_company-2.9.0rc3/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc3/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.292981 garpix_company-2.9.0rc3/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.9.0rc3/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.9.0rc3/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.293280 garpix_company-2.9.0rc3/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.293394 garpix_company-2.9.0rc3/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.293476 garpix_company-2.9.0rc3/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.293667 garpix_company-2.9.0rc3/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.9.0rc3/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.294192 garpix_company-2.9.0rc3/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      222 2023-06-21 15:54:39.000000 garpix_company-2.9.0rc3/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6252 2023-06-21 15:49:16.000000 garpix_company-2.9.0rc3/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc3/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4539 2023-06-21 15:54:04.000000 garpix_company-2.9.0rc3/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc3/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.295012 garpix_company-2.9.0rc3/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc3/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1077 2023-08-02 09:13:21.000000 garpix_company-2.9.0rc3/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.9.0rc3/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      545 2023-06-21 15:50:30.000000 garpix_company-2.9.0rc3/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc3/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.295759 garpix_company-2.9.0rc3/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc3/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc3/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5838 2023-07-27 11:38:35.000000 garpix_company-2.9.0rc3/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc3/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.9.0rc3/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      926 2023-05-12 11:36:47.000000 garpix_company-2.9.0rc3/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.295983 garpix_company-2.9.0rc3/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc3/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.9.0rc3/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.9.0rc3/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-08-02 09:13:29.000000 garpix_company-2.9.0rc3/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc3/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc3/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.296467 garpix_company-2.9.0rc3/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.9.0rc3/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.9.0rc3/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.9.0rc3/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.9.0rc3/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-08-02 09:27:56.292638 garpix_company-2.9.0rc3/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-08-02 09:27:56.296811 garpix_company-2.9.0rc3/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-08-02 09:27:56.000000 garpix_company-2.9.0rc3/setup.py
```

### Comparing `garpix_company-2.9.0rc2/PKG-INFO` & `garpix_company-2.9.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.9.0rc2
+Version: 2.9.0rc3
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.9.0rc2/garpix_company/CHANGELOG.md` & `garpix_company-2.9.0rc3/garpix_company/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/CONTRIBUTING.md` & `garpix_company-2.9.0rc3/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/README.md` & `garpix_company-2.9.0rc3/garpix_company/README.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/helpers.py` & `garpix_company-2.9.0rc3/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/models/company.py` & `garpix_company-2.9.0rc3/garpix_company/models/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/models/invite.py` & `garpix_company-2.9.0rc3/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/models/user_company.py` & `garpix_company-2.9.0rc3/garpix_company/models/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/models/user_role.py` & `garpix_company-2.9.0rc3/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/permissions/company_admin.py` & `garpix_company-2.9.0rc3/garpix_company/permissions/company_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         company_role_service = UserCompanyRoleService()
 
         if isinstance(obj, Company):
             return request.user.is_authenticated and request.user.id in UserCompany.active_objects.filter(
                 role=company_role_service.get_admin_role(), company=obj).values_list('user', flat=True)
         if isinstance(obj, InviteToCompany) or isinstance(obj, UserCompany):
             return request.user.is_authenticated and UserCompany.active_objects.filter(
-                role=company_role_service.get_admin_role(), user=request.user, company=obj)
+                role=company_role_service.get_admin_role(), user=request.user, company=obj.company)
         return False
```

### Comparing `garpix_company-2.9.0rc2/garpix_company/permissions/company_owner.py` & `garpix_company-2.9.0rc3/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/permissions/company_user.py` & `garpix_company-2.9.0rc3/garpix_company/permissions/company_user.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/serializers/company.py` & `garpix_company-2.9.0rc3/garpix_company/serializers/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/serializers/invite.py` & `garpix_company-2.9.0rc3/garpix_company/serializers/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/serializers/user_company.py` & `garpix_company-2.9.0rc3/garpix_company/serializers/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/services/role_service.py` & `garpix_company-2.9.0rc3/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/settings.py` & `garpix_company-2.9.0rc3/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/setup.py` & `garpix_company-2.9.0rc3/garpix_company/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.9.0-rc2',
+    version='2.9.0-rc3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.9.0rc2/garpix_company/urls.py` & `garpix_company-2.9.0rc3/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/views/company.py` & `garpix_company-2.9.0rc3/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/views/invite.py` & `garpix_company-2.9.0rc3/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company/views/user_company.py` & `garpix_company-2.9.0rc3/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.9.0rc3/garpix_company.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.9.0rc2
+Version: 2.9.0rc3
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.9.0rc2/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.9.0rc3/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.9.0rc2/setup.py` & `garpix_company-2.9.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.9.0-rc2',
+    version='2.9.0-rc3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

