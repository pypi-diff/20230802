# Comparing `tmp/casbin-django-orm-adapter-1.1.0.tar.gz` & `tmp/casbin-django-orm-adapter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-django-orm-adapter-1.1.0.tar", last modified: Mon Jul 31 16:26:22 2023, max compression
+gzip compressed data, was "casbin-django-orm-adapter-1.1.1.tar", last modified: Wed Aug  2 06:09:29 2023, max compression
```

## Comparing `casbin-django-orm-adapter-1.1.0.tar` & `casbin-django-orm-adapter-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.180070 casbin-django-orm-adapter-1.1.0/casbin_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/enforcer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.795650 casbin-django-orm-adapter-1.1.1/casbin_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/enforcer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.795650 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/tests/test_adapter.py
```

### Comparing `casbin-django-orm-adapter-1.1.0/LICENSE` & `casbin-django-orm-adapter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/PKG-INFO` & `casbin-django-orm-adapter-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin-django-orm-adapter-1.1.0/README.md` & `casbin-django-orm-adapter-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_adapter/adapter.py` & `casbin-django-orm-adapter-1.1.1/casbin_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_adapter/enforcer.py` & `casbin-django-orm-adapter-1.1.1/casbin_adapter/enforcer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from django.conf import settings
-from django.db import connection
+from django.db import connection, connections
 from django.db.utils import OperationalError, ProgrammingError
 
 from casbin import Enforcer
 
 from .utils import import_class
 
 logger = logging.getLogger(__name__)
@@ -60,15 +60,15 @@
 enforcer = ProxyEnforcer()
 
 
 def initialize_enforcer(db_alias=None):
     try:
         row = None
         if db_alias:
-            with connection[db_alias].cursor() as cursor:
+            with connections[db_alias].cursor() as cursor:
                 cursor.execute(
                     """
                     SELECT app, name applied FROM django_migrations
                     WHERE app = 'casbin_adapter' AND name = '0001_initial';
                     """
                 )
                 row = cursor.fetchone()
```

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/0001_initial.py` & `casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_adapter/models.py` & `casbin-django-orm-adapter-1.1.1/casbin_adapter/models.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/PKG-INFO` & `casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/SOURCES.txt` & `casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/setup.py` & `casbin-django-orm-adapter-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.0/tests/test_adapter.py` & `casbin-django-orm-adapter-1.1.1/tests/test_adapter.py`

 * *Files identical despite different names*

