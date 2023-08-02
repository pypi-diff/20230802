# Comparing `tmp/propelauth-django-rest-framework-2.1.3.tar.gz` & `tmp/propelauth-django-rest-framework-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-django-rest-framework-2.1.3.tar", last modified: Tue Jun  6 17:38:04 2023, max compression
+gzip compressed data, was "propelauth-django-rest-framework-2.1.4.tar", last modified: Wed Aug  2 18:18:18 2023, max compression
```

## Comparing `propelauth-django-rest-framework-2.1.3.tar` & `propelauth-django-rest-framework-2.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:04.200513 propelauth-django-rest-framework-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 17:37:44.000000 propelauth-django-rest-framework-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-06 17:38:04.200513 propelauth-django-rest-framework-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-06 17:37:44.000000 propelauth-django-rest-framework-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:04.196513 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-06 17:37:44.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-06 17:37:44.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework/auth_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:04.200513 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-06 17:38:04.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-06 17:38:04.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:38:04.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 17:38:04.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 17:38:04.000000 propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:38:04.200513 propelauth-django-rest-framework-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 17:37:44.000000 propelauth-django-rest-framework-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:18:18.676277 propelauth-django-rest-framework-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 18:18:02.000000 propelauth-django-rest-framework-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 18:18:18.676277 propelauth-django-rest-framework-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-02 18:18:02.000000 propelauth-django-rest-framework-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:18:18.676277 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-08-02 18:18:02.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-08-02 18:18:02.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework/auth_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:18:18.676277 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 18:18:18.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-02 18:18:18.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:18:18.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 18:18:18.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 18:18:18.000000 propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:18:18.676277 propelauth-django-rest-framework-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-02 18:18:02.000000 propelauth-django-rest-framework-2.1.4/setup.py
```

### Comparing `propelauth-django-rest-framework-2.1.3/LICENSE` & `propelauth-django-rest-framework-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.3/PKG-INFO` & `propelauth-django-rest-framework-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.3
+Version: 2.1.4
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.3
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.4
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.3/README.md` & `propelauth-django-rest-framework-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework/__init__.py` & `propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework/auth_helpers.py` & `propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.3/propelauth_django_rest_framework.egg-info/PKG-INFO` & `propelauth-django-rest-framework-2.1.4/propelauth_django_rest_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.3
+Version: 2.1.4
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.3
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.4
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.3/setup.py` & `propelauth-django-rest-framework-2.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-django-rest-framework",
-    version="2.1.3",
+    version="2.1.4",
     description="A library for managing authentication in Django Rest Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-django-rest-framework",
     packages=find_packages(include=["propelauth_django_rest_framework"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["django", "djangorestframework", "propelauth-py==3.1.3", "requests"],
+    install_requires=["django", "djangorestframework", "propelauth-py==3.1.4", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

