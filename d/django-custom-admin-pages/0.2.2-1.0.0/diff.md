# Comparing `tmp/django_custom_admin_pages-0.2.2.tar.gz` & `tmp/django_custom_admin_pages-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_custom_admin_pages-0.2.2.tar", max compression
+gzip compressed data, was "django_custom_admin_pages-1.0.0.tar", max compression
```

## Comparing `django_custom_admin_pages-0.2.2.tar` & `django_custom_admin_pages-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-0.2.2/LICENSE
--rw-r--r--   0        0        0     5627 2023-07-30 23:40:04.183108 django_custom_admin_pages-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/__init__.py
--rw-r--r--   0        0        0     5638 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/admin.py
--rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/apps.py
--rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/default_settings.py
--rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-0.2.2/django_custom_admin_pages/templates/base_custom_admin.html
--rw-r--r--   0        0        0      777 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/urls.py
--rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/__init__.py
--rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/admin_base_view.py
--rw-r--r--   0        0        0     1921 2023-07-30 23:38:34.063109 django_custom_admin_pages-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 django_custom_admin_pages-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6225 2023-08-02 03:54:28.456719 django_custom_admin_pages-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/__init__.py
+-rw-r--r--   0        0        0     5638 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/admin.py
+-rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/apps.py
+-rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/default_settings.py
+-rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-1.0.0/django_custom_admin_pages/templates/base_custom_admin.html
+-rw-r--r--   0        0        0      777 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/urls.py
+-rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/admin_base_view.py
+-rw-r--r--   0        0        0     2333 2023-08-02 04:07:01.766715 django_custom_admin_pages-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7912 1970-01-01 00:00:00.000000 django_custom_admin_pages-1.0.0/PKG-INFO
```

### Comparing `django_custom_admin_pages-0.2.2/LICENSE` & `django_custom_admin_pages-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.2/README.md` & `django_custom_admin_pages-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+[![PyPI version](https://badge.fury.io/py/django-custom-admin-pages.svg)](https://badge.fury.io/py/django-custom-admin-pages)
+[![Tests](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml)
+[![codecov](https://codecov.io/gh/lekjos/django-custom-admin-pages/branch/master/graph/badge.svg?token=AJG2WICKXA)](https://codecov.io/gh/lekjos/django-custom-admin-pages)
+![Python Versions](https://img.shields.io/badge/Python_Versions-3.9,_3.10,_3.11-blue)
+![Django Versions](https://img.shields.io/badge/Django_Versions-3.2,_4.0,_4.1,_4.2-blue)
+
+
 # Django Custom Admin Pages
 A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
 
 ## Installation
 
 1. Install the app from pypi `pip install django_custom_admin_pages`
@@ -21,17 +28,14 @@
 
 ```python
 from django_custom_admin_pages.admin import CustomAdminConfig
 class MyCustomAdminSite(CustomAdminConfig):
    pass
 ```
 
-_This app is currently in beta and only tested in django 3.2 / python 3.10_
-
-
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
 To create a new custom admin view:
 
 1. Create a class-based view in `django_custom_admin_pages.views` which inherits from `custom_admin.views.admin_base_view.AdminBaseView`.
```

### Comparing `django_custom_admin_pages-0.2.2/django_custom_admin_pages/admin.py` & `django_custom_admin_pages-1.0.0/django_custom_admin_pages/admin.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.2/django_custom_admin_pages/urls.py` & `django_custom_admin_pages-1.0.0/django_custom_admin_pages/urls.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/admin_base_view.py` & `django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/admin_base_view.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.2/pyproject.toml` & `django_custom_admin_pages-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 [tool.poetry]
 name = "django-custom-admin-pages"
-version = "0.2.2"
+authors = [
+    "Leif Kjos <leif+pypi@leifkjos.com>",
+]
+maintainers = [
+    "Leif Kjos <leif+pypi@leifkjos.com>",
+]
+version = "1.0.0"
 description = "A django app that lets you add standard class-based views to the django admin index and navigation."
-authors = ["lekjos"]
-license = "BSD"
+license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/lekjos/django-custom-admin-pages"
 repository = "https://github.com/lekjos/django-custom-admin-pages"
-keywords = ["django", "django-admin", "django admin"]
+keywords = ["django", "admin", "django-admin", "django admin", "interface", "customize admin", "custom admin", "customize"]
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
-    "Development Status :: 4 - Beta",
+    "Framework :: Django", 
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0", 
+    "Framework :: Django :: 4.1", 
+    "Framework :: Django :: 4.2", 
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Framework :: Django :: 3.2", 
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules", 
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 include = [
     "LICENSE.md",
 ]
 exclude = [
     "django_custom_admin_pages/boot_django.py",
     "django_custom_admin_pages/conftest.py",
     "django_custom_admin_pages/pytest.ini",
     "django_custom_admin_pages/test_proj",
     "django_custom_admin_pages/tests",
 ]
+
 packages = [{include = "django_custom_admin_pages"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = "^3.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `django_custom_admin_pages-0.2.2/PKG-INFO` & `django_custom_admin_pages-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 Metadata-Version: 2.1
 Name: django-custom-admin-pages
-Version: 0.2.2
+Version: 1.0.0
 Summary: A django app that lets you add standard class-based views to the django admin index and navigation.
 Home-page: https://github.com/lekjos/django-custom-admin-pages
-License: BSD
-Keywords: django,django-admin,django admin
-Author: lekjos
+License: BSD-3-Clause
+Keywords: django,admin,django-admin,django admin,interface,customize admin,custom admin,customize
+Author: Leif Kjos
+Author-email: leif+pypi@leifkjos.com
+Maintainer: Leif Kjos
+Maintainer-email: leif+pypi@leifkjos.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/lekjos/django-custom-admin-pages
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/django-custom-admin-pages.svg)](https://badge.fury.io/py/django-custom-admin-pages)
+[![Tests](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml)
+[![codecov](https://codecov.io/gh/lekjos/django-custom-admin-pages/branch/master/graph/badge.svg?token=AJG2WICKXA)](https://codecov.io/gh/lekjos/django-custom-admin-pages)
+![Python Versions](https://img.shields.io/badge/Python_Versions-3.9,_3.10,_3.11-blue)
+![Django Versions](https://img.shields.io/badge/Django_Versions-3.2,_4.0,_4.1,_4.2-blue)
+
+
 # Django Custom Admin Pages
 A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
 
 ## Installation
 
 1. Install the app from pypi `pip install django_custom_admin_pages`
@@ -50,17 +65,14 @@
 
 ```python
 from django_custom_admin_pages.admin import CustomAdminConfig
 class MyCustomAdminSite(CustomAdminConfig):
    pass
 ```
 
-_This app is currently in beta and only tested in django 3.2 / python 3.10_
-
-
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
 To create a new custom admin view:
 
 1. Create a class-based view in `django_custom_admin_pages.views` which inherits from `custom_admin.views.admin_base_view.AdminBaseView`.
```

