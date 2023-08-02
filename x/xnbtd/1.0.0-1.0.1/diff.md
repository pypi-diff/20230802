# Comparing `tmp/xnbtd-1.0.0.tar.gz` & `tmp/xnbtd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-1.0.0.tar", max compression
+gzip compressed data, was "xnbtd-1.0.1.tar", max compression
```

## Comparing `xnbtd-1.0.0.tar` & `xnbtd-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,39 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-1.0.0/README.md
--rwxr-xr-x   0        0        0     3622 2023-08-02 17:52:14.796219 xnbtd-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      222 2023-07-21 21:52:15.409174 xnbtd-1.0.0/xnbtd/__init__.py
--rwxr-xr-x   0        0        0      281 2023-07-24 18:46:24.620500 xnbtd-1.0.0/xnbtd/admin.py
--rwxr-xr-x   0        0        0      288 2023-07-21 21:49:55.059033 xnbtd-1.0.0/xnbtd/apps.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-1.0.0/xnbtd/asgi.py
--rwxr-xr-x   0        0        0      610 2023-08-02 17:47:49.000000 xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     1080 2023-08-02 17:47:22.504710 xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-1.0.0/xnbtd/plannings/__init__.py
--rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-1.0.0/xnbtd/plannings/admin.py
--rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-1.0.0/xnbtd/plannings/apps.py
--rwxr-xr-x   0        0        0      581 2023-08-02 17:47:50.000000 xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0      953 2023-08-02 17:47:22.441722 xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      914 2023-07-21 21:35:35.367721 xnbtd-1.0.0/xnbtd/plannings/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-20 11:49:50.131931 xnbtd-1.0.0/xnbtd/plannings/migrations/__init__.py
--rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-1.0.0/xnbtd/plannings/models.py
--rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-1.0.0/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-1.0.0/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5841 2023-07-21 20:58:24.764238 xnbtd-1.0.0/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-1.0.0/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-1.0.0/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-1.0.0/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0     1391 2023-07-21 21:31:26.839640 xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/change_list.html
--rwxr-xr-x   0        0        0     1656 2023-07-20 12:50:03.246479 xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/index.html
--rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-1.0.0/xnbtd/templatetags/events.py
--rwxr-xr-x   0        0        0     1499 2023-07-24 16:48:20.567679 xnbtd-1.0.0/xnbtd/templatetags/tours.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-1.0.0/xnbtd/tours/__init__.py
--rwxr-xr-x   0        0        0    16856 2023-08-02 17:39:30.074888 xnbtd-1.0.0/xnbtd/tours/admin.py
--rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-1.0.0/xnbtd/tours/apps.py
--rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-1.0.0/xnbtd/tours/forms.py
--rwxr-xr-x   0        0        0     4732 2023-08-02 17:47:50.000000 xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     8447 2023-08-02 17:48:31.196994 xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     8264 2023-07-21 21:35:35.397000 xnbtd-1.0.0/xnbtd/tours/migrations/0001_initial.py
--rwxr-xr-x   0        0        0     1912 2023-07-24 15:47:49.294370 xnbtd-1.0.0/xnbtd/tours/migrations/0002_chronopostpickup_and_more.py
--rwxr-xr-x   0        0        0     2282 2023-07-24 16:10:57.506588 xnbtd-1.0.0/xnbtd/tours/migrations/0003_chronopostdelivery_linked_user_and_more.py
--rwxr-xr-x   0        0        0      826 2023-07-24 19:00:42.569177 xnbtd-1.0.0/xnbtd/tours/migrations/0004_alter_chronopostdelivery_options_and_more.py
--rwxr-xr-x   0        0        0     1121 2023-08-02 17:41:02.878443 xnbtd-1.0.0/xnbtd/tours/migrations/0005_alter_chronopostdelivery_options_and_more.py
--rwxr-xr-x   0        0        0        0 2023-07-20 11:49:44.075539 xnbtd-1.0.0/xnbtd/tours/migrations/__init__.py
--rwxr-xr-x   0        0        0     4777 2023-08-02 17:39:56.090739 xnbtd-1.0.0/xnbtd/tours/models.py
--rwxr-xr-x   0        0        0      120 2023-07-21 08:12:20.934692 xnbtd-1.0.0/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-1.0.0/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-1.0.1/README.md
+-rwxr-xr-x   0        0        0     3622 2023-08-02 18:17:18.067408 xnbtd-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      222 2023-07-21 21:52:15.409174 xnbtd-1.0.1/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      281 2023-07-24 18:46:24.620500 xnbtd-1.0.1/xnbtd/admin.py
+-rwxr-xr-x   0        0        0      288 2023-07-21 21:49:55.059033 xnbtd-1.0.1/xnbtd/apps.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-1.0.1/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0      610 2023-08-02 17:47:49.000000 xnbtd-1.0.1/xnbtd/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     1080 2023-08-02 17:47:22.504710 xnbtd-1.0.1/xnbtd/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-1.0.1/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-1.0.1/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-1.0.1/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-08-02 17:47:50.000000 xnbtd-1.0.1/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      953 2023-08-02 17:47:22.441722 xnbtd-1.0.1/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      914 2023-07-21 21:35:35.367721 xnbtd-1.0.1/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:50.131931 xnbtd-1.0.1/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-1.0.1/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-1.0.1/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-1.0.1/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5841 2023-07-21 20:58:24.764238 xnbtd-1.0.1/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-1.0.1/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-1.0.1/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-1.0.1/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0     1391 2023-07-21 21:31:26.839640 xnbtd-1.0.1/xnbtd/templates/xnbtd/admin/change_list.html
+-rwxr-xr-x   0        0        0     1656 2023-07-20 12:50:03.246479 xnbtd-1.0.1/xnbtd/templates/xnbtd/admin/index.html
+-rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-1.0.1/xnbtd/templatetags/events.py
+-rwxr-xr-x   0        0        0     1499 2023-07-24 16:48:20.567679 xnbtd-1.0.1/xnbtd/templatetags/tours.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-1.0.1/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0    16856 2023-08-02 17:39:30.074888 xnbtd-1.0.1/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-1.0.1/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-1.0.1/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     4732 2023-08-02 17:47:50.000000 xnbtd-1.0.1/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     8447 2023-08-02 17:48:31.196994 xnbtd-1.0.1/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0    10803 2023-08-02 18:13:32.307882 xnbtd-1.0.1/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:44.075539 xnbtd-1.0.1/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     4777 2023-08-02 17:39:56.090739 xnbtd-1.0.1/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      120 2023-07-21 08:12:20.934692 xnbtd-1.0.1/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-1.0.1/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-1.0.1/PKG-INFO
```

### Comparing `xnbtd-1.0.0/LICENSE` & `xnbtd-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/README.md` & `xnbtd-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/pyproject.toml` & `xnbtd-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "1.0.0"
+version = "1.0.1"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.1/xnbtd/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.1/xnbtd/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.1/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.1/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/plannings/migrations/0001_initial.py` & `xnbtd-1.0.1/xnbtd/plannings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/publish.py` & `xnbtd-1.0.1/xnbtd/publish.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/settings/base.py` & `xnbtd-1.0.1/xnbtd/settings/base.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/settings/local.py` & `xnbtd-1.0.1/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/change_list.html` & `xnbtd-1.0.1/xnbtd/templates/xnbtd/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/index.html` & `xnbtd-1.0.1/xnbtd/templates/xnbtd/admin/index.html`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/templatetags/events.py` & `xnbtd-1.0.1/xnbtd/templatetags/events.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/templatetags/tours.py` & `xnbtd-1.0.1/xnbtd/templatetags/tours.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/tours/admin.py` & `xnbtd-1.0.1/xnbtd/tours/admin.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.1/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.1/xnbtd/tours/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/xnbtd/tours/models.py` & `xnbtd-1.0.1/xnbtd/tours/models.py`

 * *Files identical despite different names*

### Comparing `xnbtd-1.0.0/PKG-INFO` & `xnbtd-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 1.0.0
+Version: 1.0.1
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

