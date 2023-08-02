# Comparing `tmp/django-courseaffils-2.3.0.tar.gz` & `tmp/django-courseaffils-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-courseaffils-2.3.0.tar", last modified: Fri Feb 17 21:35:44 2023, max compression
+gzip compressed data, was "django-courseaffils-2.4.0.tar", last modified: Wed Aug  2 18:00:55 2023, max compression
```

## Comparing `django-courseaffils-2.3.0.tar` & `django-courseaffils-2.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.449099 django-courseaffils-2.3.0/
--rw-rw-r--   0 nik       (1000) nik       (1000)       28 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/MANIFEST.in
--rw-r--r--   0 nik       (1000) nik       (1000)      295 2023-02-17 21:35:44.449099 django-courseaffils-2.3.0/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     2181 2022-08-26 20:32:32.000000 django-courseaffils-2.3.0/README.md
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.444099 django-courseaffils-2.3.0/courseaffils/
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)      883 2022-10-24 16:52:30.000000 django-courseaffils-2.3.0/courseaffils/admin.py
--rw-r--r--   0 nik       (1000) nik       (1000)     9272 2022-11-28 23:01:07.000000 django-courseaffils-2.3.0/courseaffils/columbia.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     6473 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/forms.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     2777 2020-04-07 00:18:45.000000 django-courseaffils-2.3.0/courseaffils/lib.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      706 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/listener.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     6521 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/middleware.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.445099 django-courseaffils-2.3.0/courseaffils/migrations/
--rw-rw-r--   0 nik       (1000) nik       (1000)     3351 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/migrations/0001_initial.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      480 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/migrations/0002_auto_20160316_1223.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     1255 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/migrations/0003_auto_20160429_1353.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      647 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/migrations/0004_auto_20170623_1231.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     1498 2020-03-19 21:40:11.000000 django-courseaffils-2.3.0/courseaffils/migrations/0005_auto_20200318_1543.py
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/migrations/__init__.py
--rw-rw-r--   0 nik       (1000) nik       (1000)    10860 2020-08-18 20:42:37.000000 django-courseaffils-2.3.0/courseaffils/models.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.445099 django-courseaffils-2.3.0/courseaffils/templates/
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templates/base.html
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.446099 django-courseaffils-2.3.0/courseaffils/templates/courseaffils/
--rw-rw-r--   0 nik       (1000) nik       (1000)     4074 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templates/courseaffils/admin_change_form.html
--rw-rw-r--   0 nik       (1000) nik       (1000)      118 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templates/courseaffils/course_form.html
--rw-rw-r--   0 nik       (1000) nik       (1000)     2894 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templates/courseaffils/course_list.html
--rw-rw-r--   0 nik       (1000) nik       (1000)      831 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templates/courseaffils/course_row.html
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.446099 django-courseaffils-2.3.0/courseaffils/templatetags/
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templatetags/__init__.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     4166 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/templatetags/coursetags.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.448099 django-courseaffils-2.3.0/courseaffils/tests/
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     1099 2021-09-03 16:03:56.000000 django-courseaffils-2.3.0/courseaffils/tests/factories.py
--rw-r--r--   0 nik       (1000) nik       (1000)     1042 2022-08-26 20:32:32.000000 django-courseaffils-2.3.0/courseaffils/tests/mixins.py
--rw-r--r--   0 nik       (1000) nik       (1000)     5301 2022-11-28 23:01:07.000000 django-courseaffils-2.3.0/courseaffils/tests/test_columbia.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     3261 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_forms.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     2935 2020-04-07 00:18:45.000000 django-courseaffils-2.3.0/courseaffils/tests/test_lib.py
--rw-rw-r--   0 nik       (1000) nik       (1000)        0 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_listener.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     3789 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_middleware.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     9738 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_models.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     1954 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_settings.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      917 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_utils.py
--rw-rw-r--   0 nik       (1000) nik       (1000)     5288 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/test_views.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      327 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/tests/urls.py
--rw-rw-r--   0 nik       (1000) nik       (1000)      511 2020-03-18 19:57:25.000000 django-courseaffils-2.3.0/courseaffils/utils.py
--rw-r--r--   0 nik       (1000) nik       (1000)     6711 2022-05-19 17:41:51.000000 django-courseaffils-2.3.0/courseaffils/views.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-02-17 21:35:44.449099 django-courseaffils-2.3.0/django_courseaffils.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)      295 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)     1556 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/not-zip-safe
--rw-r--r--   0 nik       (1000) nik       (1000)        7 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       13 2023-02-17 21:35:44.000000 django-courseaffils-2.3.0/django_courseaffils.egg-info/top_level.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-02-17 21:35:44.449099 django-courseaffils-2.3.0/setup.cfg
--rw-r--r--   0 nik       (1000) nik       (1000)      660 2023-02-17 21:35:08.000000 django-courseaffils-2.3.0/setup.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.938173 django-courseaffils-2.4.0/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       28 2023-07-31 18:49:13.000000 django-courseaffils-2.4.0/MANIFEST.in
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      296 2023-08-02 18:00:55.938065 django-courseaffils-2.4.0/PKG-INFO
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2181 2023-07-31 18:49:13.000000 django-courseaffils-2.4.0/README.md
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.933140 django-courseaffils-2.4.0/courseaffils/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/__init__.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      883 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/admin.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     9272 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/columbia.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     6473 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/forms.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2777 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/lib.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      706 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/listener.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     6519 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/middleware.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.934048 django-courseaffils-2.4.0/courseaffils/migrations/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     3351 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/0001_initial.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      480 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/0002_auto_20160316_1223.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1255 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/0003_auto_20160429_1353.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      647 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/0004_auto_20170623_1231.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1498 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/0005_auto_20200318_1543.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/migrations/__init__.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    10860 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/models.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.934136 django-courseaffils-2.4.0/courseaffils/templates/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templates/base.html
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.934726 django-courseaffils-2.4.0/courseaffils/templates/courseaffils/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4074 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templates/courseaffils/admin_change_form.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      118 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templates/courseaffils/course_form.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2894 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templates/courseaffils/course_list.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      831 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templates/courseaffils/course_row.html
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.934968 django-courseaffils-2.4.0/courseaffils/templatetags/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templatetags/__init__.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4166 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/templatetags/coursetags.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.937107 django-courseaffils-2.4.0/courseaffils/tests/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/__init__.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1099 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/factories.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1042 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/mixins.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     5301 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_columbia.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     3261 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_forms.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2935 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_lib.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        0 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_listener.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     3801 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/tests/test_middleware.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     9731 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/tests/test_models.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1909 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/tests/test_settings.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      917 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_utils.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     5288 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/tests/test_views.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      323 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/tests/urls.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      511 2023-07-31 15:45:42.000000 django-courseaffils-2.4.0/courseaffils/utils.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     6779 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/courseaffils/views.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2023-08-02 18:00:55.937887 django-courseaffils-2.4.0/django_courseaffils.egg-info/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      296 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/PKG-INFO
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1556 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/SOURCES.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        1 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/dependency_links.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        1 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/not-zip-safe
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        7 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/requires.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       13 2023-08-02 18:00:55.000000 django-courseaffils-2.4.0/django_courseaffils.egg-info/top_level.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       38 2023-08-02 18:00:55.938208 django-courseaffils-2.4.0/setup.cfg
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      661 2023-08-02 17:59:38.000000 django-courseaffils-2.4.0/setup.py
```

### Comparing `django-courseaffils-2.3.0/README.md` & `django-courseaffils-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/admin.py` & `django-courseaffils-2.4.0/courseaffils/admin.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/columbia.py` & `django-courseaffils-2.4.0/courseaffils/columbia.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/forms.py` & `django-courseaffils-2.4.0/courseaffils/forms.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/lib.py` & `django-courseaffils-2.4.0/courseaffils/lib.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/listener.py` & `django-courseaffils-2.4.0/courseaffils/listener.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/middleware.py` & `django-courseaffils-2.4.0/courseaffils/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import unicode_literals
 
 from django.http import HttpResponseRedirect
 from django.conf import settings
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 
 from courseaffils.models import Course, CourseAccess
 from courseaffils.views import CourseListView
 from courseaffils.lib import AUTO_COURSE_SELECT, is_faculty
 from django.contrib.contenttypes.models import ContentType
 from django.utils.deprecation import MiddlewareMixin
 
@@ -75,15 +75,15 @@
 
 
 class CourseManagerMiddleware(MiddlewareMixin):
     def process_response(self, request, response):
         if 'ANONYMIZE' in request.COOKIES:
             for user, uid in getattr(request, 'scrub_names', {}).items():
                 if len(user.last_name) > 3:
-                    response.content = smart_text(
+                    response.content = smart_str(
                         response.content,
                         errors='ignore').replace(
                             user.get_full_name(), 'User Name_%d' % uid)
         return response
 
     @staticmethod
     def decorate_request(request, course):
```

### Comparing `django-courseaffils-2.3.0/courseaffils/migrations/0001_initial.py` & `django-courseaffils-2.4.0/courseaffils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/migrations/0003_auto_20160429_1353.py` & `django-courseaffils-2.4.0/courseaffils/migrations/0003_auto_20160429_1353.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/migrations/0004_auto_20170623_1231.py` & `django-courseaffils-2.4.0/courseaffils/migrations/0004_auto_20170623_1231.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/migrations/0005_auto_20200318_1543.py` & `django-courseaffils-2.4.0/courseaffils/migrations/0005_auto_20200318_1543.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/models.py` & `django-courseaffils-2.4.0/courseaffils/models.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/templates/courseaffils/admin_change_form.html` & `django-courseaffils-2.4.0/courseaffils/templates/courseaffils/admin_change_form.html`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/templates/courseaffils/course_list.html` & `django-courseaffils-2.4.0/courseaffils/templates/courseaffils/course_list.html`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/templates/courseaffils/course_row.html` & `django-courseaffils-2.4.0/courseaffils/templates/courseaffils/course_row.html`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/templatetags/coursetags.py` & `django-courseaffils-2.4.0/courseaffils/templatetags/coursetags.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/factories.py` & `django-courseaffils-2.4.0/courseaffils/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/mixins.py` & `django-courseaffils-2.4.0/courseaffils/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_columbia.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_columbia.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_forms.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_lib.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_middleware.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,31 @@
         assert is_anonymous_path("/static/")
 
     def test_already_selected_course(self):
         assert already_selected_course(StubRequest(True))
         assert not already_selected_course(StubRequest(False))
 
     def test_cmm_process_response(self):
-        c = CourseManagerMiddleware()
+        c = CourseManagerMiddleware(self)
         assert c.process_response(StubRequest(True), "foo") == "foo"
 
     def test_cmm_process_response_anon(self):
-        c = CourseManagerMiddleware()
+        c = CourseManagerMiddleware(self)
         r = StubRequest(self.c)
         r.user = self.student
         r.COOKIES['ANONYMIZE'] = True
         r.scrub_names = {self.student: 1}
         resp = StubResponse()
         resp.content = str(self.student.get_full_name())
         assert "User Name" in c.process_response(r, resp).content
         resp.content = str(self.student.get_full_name())
         assert "long enough" not in c.process_response(r, resp).content
 
     def test_cmm_process_request(self):
-        c = CourseManagerMiddleware()
+        c = CourseManagerMiddleware(self)
         r = StubRequest(self.c)
         r.user = self.student
         assert c.process_request(r) is None
 
         r.path = "/favicon.ico"
         assert c.process_request(r) is None
```

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_models.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import unicode_literals
 
 from django.test import TestCase, override_settings
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 from courseaffils.columbia import CourseStringMapper
 from courseaffils.models import Course, CourseSettings
 from courseaffils.models import CourseInfo, CourseAccess
 from courseaffils.tests.factories import (
     AffilFactory, CourseFactory, UserFactory
 )
 from django.contrib.auth.models import Group, User
@@ -47,15 +47,15 @@
         self.c.delete()
         self.student_group.delete()
         self.faculty_group.delete()
         self.student.delete()
         self.faculty.delete()
 
     def test_str(self):
-        self.assertEqual(smart_text(self.c), "test course")
+        self.assertEqual(smart_str(self.c), "test course")
 
     def test_members(self):
         self.assertIn(self.student, self.c.members)
 
     def test_students(self):
         self.assertIn(self.student, self.c.students)
 
@@ -131,41 +131,41 @@
         self.assertIn("foo", self.c.details())
         self.assertEqual(self.c.details()["foo"].value, "bar")
         self.assertEqual(self.c.get_detail("foo", default="not bar"), "bar")
         self.assertEqual(self.c.get_detail(
             "nonexistant",
             default="a default value"), "a default value")
 
-        self.assertEqual(smart_text(self.c.details()["foo"]),
+        self.assertEqual(smart_str(self.c.details()["foo"]),
                          "(test course) foo: bar")
 
         # update
         self.c.add_detail("foo", "baz")
         self.assertEqual(self.c.details()["foo"].value, "baz")
 
     def test_coursesettings(self):
         cs = CourseSettings.objects.create(
             course=self.c,
             custom_headers="some headers")
-        self.assertEqual(smart_text(cs), "Settings for test course")
+        self.assertEqual(smart_str(cs), "Settings for test course")
 
     def test_courseinfo(self):
         # current behavior is that a CourseInfo object
         # is created automatically for each course
         # by a hook elsewhere. so verify that.
         self.assertNotEqual(CourseInfo.objects.all().count(), 0)
 
-        self.assertEqual(smart_text(self.c.info),
+        self.assertEqual(smart_str(self.c.info),
                          'test course () None None-None')
 
         self.c.info.year = 2013
         self.c.info.term = 1
         self.c.info.days = "MWF"
         self.c.info.save()
-        self.assertEqual(smart_text(self.c.info),
+        self.assertEqual(smart_str(self.c.info),
                          'test course (Spring 2013) MWF None-None')
 
         self.assertEqual(self.c.info.time(), 'MWF')
 
         self.assertEqual(self.c.info.display(), "Spring 2013 MWF None-None")
 
     def test_courseaccess(self):
@@ -187,15 +187,15 @@
         self.aa = AffilFactory(
             name='t1.y2016.s001.cf1002.scnc.st.course:columbia.edu')
 
     def test_is_valid_from_factory(self):
         self.aa.full_clean()
 
     def test_str(self):
-        self.assertEqual(smart_text(self.aa), self.aa.name)
+        self.assertEqual(smart_str(self.aa), self.aa.name)
 
     def test_past_present_future(self):
         with freeze_time('2012-01-14'):
             self.assertEqual(self.aa.past_present_future, 1)
         with freeze_time('2015-01-14'):
             self.assertEqual(self.aa.past_present_future, 1)
         with freeze_time('2015-08-15'):
```

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_settings.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 ]
 
 INSTALLED_APPS = (
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'courseaffils',
-    'django_markwhat',
-    'django_jenkins',
 )
 
 PROJECT_APPS = [
     'courseaffils',
 ]
 COVERAGE_EXCLUDES_FOLDERS = ['migrations']
```

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_utils.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/tests/test_views.py` & `django-courseaffils-2.4.0/courseaffils/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-courseaffils-2.3.0/courseaffils/views.py` & `django-courseaffils-2.4.0/courseaffils/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from courseaffils.forms import CourseCreateForm
 from courseaffils.models import Course, CourseAccess
 from django.db.models import Q
 from django.shortcuts import render, get_object_or_404
 from django.views.generic.edit import CreateView
 from django.views.generic.list import ListView
 from django.utils import timezone
-from django.utils.http import urlquote
 from django.http import HttpResponseForbidden, HttpResponse
 from django.contrib.auth.models import User
 
+try:
+    from urllib.parse import quote
+except ImportError:
+    from django.utils.http import urlquote as quote
+
 
 SESSION_KEY = 'ccnmtl.courseaffils.course'
 
 
 def get_courses_for_user(user):
     courses = Course.objects.none()
     if user.is_staff:
@@ -126,15 +130,15 @@
         if semester_view not in self.view_options:
             semester_view = 'current'
 
         next_redirect = ''
         if 'QUERY_STRING' in self.request.META \
            and 'unset_course' not in self.request.GET:
             # just GET (until someone complains)
-            escaped_path = urlquote(self.request.get_full_path())
+            escaped_path = quote(self.request.get_full_path())
             next_redirect = '&next=' + escaped_path
 
         context.update({
             'add_privilege': self.request.user.is_staff,
             'semester_view': semester_view,
             'next_redirect': next_redirect,
             'as_student': as_student,
@@ -169,15 +173,15 @@
                       response_dict)
 
     response_dict['next_redirect'] = ''
     if 'QUERY_STRING' in request.META \
             and 'unset_course' not in request.GET:
         # just GET (until someone complains)
         response_dict['next_redirect'] = '&next=%s' % (
-            urlquote(request.get_full_path()))
+            quote(request.get_full_path()))
 
     return render(request, 'courseaffils/select_course.html',
                   response_dict)
 
 
 def course_list_query(request):
     if not CourseAccess.allowed(request):
```

### Comparing `django-courseaffils-2.3.0/django_courseaffils.egg-info/SOURCES.txt` & `django-courseaffils-2.4.0/django_courseaffils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

