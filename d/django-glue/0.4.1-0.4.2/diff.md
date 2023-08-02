# Comparing `tmp/django-glue-0.4.1.tar.gz` & `tmp/django-glue-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.4.1.tar", last modified: Sat Jul 15 03:10:35 2023, max compression
+gzip compressed data, was "django-glue-0.4.2.tar", last modified: Wed Aug  2 16:09:27 2023, max compression
```

## Comparing `django-glue-0.4.1.tar` & `django-glue-0.4.2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-15 03:10:24.000000 django-glue-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 03:10:24.000000 django-glue-0.4.1/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-15 03:10:24.000000 django-glue-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-15 03:10:24.000000 django-glue-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-15 03:10:35.604376 django-glue-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-15 03:10:24.000000 django-glue-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 03:10:24.000000 django-glue-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-15 03:10:35.604376 django-glue-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-15 03:10:24.000000 django-glue-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-02 16:09:15.000000 django-glue-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-02 16:09:15.000000 django-glue-0.4.2/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 16:09:15.000000 django-glue-0.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 16:09:15.000000 django-glue-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 16:09:27.310497 django-glue-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-02 16:09:15.000000 django-glue-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.302497 django-glue-0.4.2/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 16:09:15.000000 django-glue-0.4.2/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.306497 django-glue-0.4.2/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 16:09:27.000000 django-glue-0.4.2/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 16:09:15.000000 django-glue-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 16:09:27.314497 django-glue-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 16:09:15.000000 django-glue-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:27.310497 django-glue-0.4.2/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-02 16:09:15.000000 django-glue-0.4.2/tests/wsgi.py
```

### Comparing `django-glue-0.4.1/CHANGELOG.md` & `django-glue-0.4.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog for Django Glue
 
+## 0.4.2
+
+### Changes
+- Context data to construct model object fields in js
+- Session data updated inside of keep live ajax
+- Cleaning js functions (more needed)
+
 ## 0.4.1
 
 #### Features
 - Event system implement for responses.
 
 #### Changes
 - Keep live system update to work with template and view loading.
```

### Comparing `django-glue-0.4.1/LICENSE.md` & `django-glue-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/PKG-INFO` & `django-glue-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.1
+Version: 0.4.2
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.1/README.md` & `django-glue-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/context_processors.py` & `django-glue-0.4.2/django_glue/context_processors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import json
+
 from django_glue.conf import settings
 from django_glue import __version__
+from django_glue.sessions import GlueSession
 
 
 def glue(request):
+    print(json.dumps(GlueSession(request).session))
     return {
         'DJANGO_GLUE_VERSION': __version__,
         settings.DJANGO_GLUE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_SESSION_NAME, {}).get('context'),
         settings.DJANGO_GLUE_KEEP_LIVE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_KEEP_LIVE_SESSION_NAME, {}),
         'DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS': settings.DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_SECONDS * 1000,
+        'GLUE_SESSION_DATA': json.dumps(GlueSession(request).session),
     }
```

### Comparing `django-glue-0.4.1/django_glue/data_classes.py` & `django-glue-0.4.2/django_glue/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     fields: dict[GlueModelFieldData] = None
     methods: list[str] = None
 
     def to_dict(self) -> dict:
         return asdict(self)
 
 
-
 @dataclass
 class GlueJsonData:
     fields: Optional[dict] = None
     simple_fields: Optional[dict] = None
     method_return: Optional[Any] = None
     custom: Optional[dict] = None
```

### Comparing `django-glue-0.4.1/django_glue/enums.py` & `django-glue-0.4.2/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/glue.py` & `django-glue-0.4.2/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/handlers.py` & `django-glue-0.4.2/django_glue/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         else:
             self.is_valid_request = False
 
         self.unique_name = self.body_data['unique_name']
 
         self.glue_session = GlueSession(request)
         self.context = self.glue_session['context']
+        self.method = request.method
 
         if self.unique_name in self.context:
-            self.method = request.method
 
             self.meta_data: GlueMetaData = GlueMetaData(
                 **self.glue_session['meta'][self.unique_name]
             )
 
             self.connection = GlueConnection(self.context[self.unique_name]['connection'])
```

### Comparing `django-glue-0.4.1/django_glue/middleware.py` & `django-glue-0.4.2/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/responses.py` & `django-glue-0.4.2/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/services/model_objects.py` & `django-glue-0.4.2/django_glue/services/model_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 
         json_data.simple_fields = generate_simple_field_dict(
             self.object,
             self.meta_data.fields,
             self.meta_data.exclude,
         )
 
-        # json_data.simple_fields['first_name'] = 'Humbugery'
-
         return generate_json_200_response_data(
             'THE GET ACTION',
             'this is a response from an model object get action!!! stay tuned!',
             json_data,
         )
 
     def process_create_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
```

### Comparing `django-glue-0.4.1/django_glue/services/query_sets.py` & `django-glue-0.4.2/django_glue/services/query_sets.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/services/services.py` & `django-glue-0.4.2/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/services/templates.py` & `django-glue-0.4.2/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/sessions.py` & `django-glue-0.4.2/django_glue/sessions.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_ajax.js` & `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,27 @@
 class GlueKeepLive {
     constructor() {
         window.glue_keep_live_unique_names = []
+        window.glue_session_data = {}
     }
 
     add_unique_name(unique_name) {
         if (!window.glue_keep_live_unique_names.includes(unique_name)) {
             window.glue_keep_live_unique_names.push(unique_name)
         }
     }
 
-    update(keep_live_url) {
+    async update(keep_live_url) {
         const request_options = {
             method: 'QUERY',
             headers: {
                 'Content-Type': 'application/json',
                 'X-CSRFToken': glue_get_cookie('csrftoken'),
             },
             body: JSON.stringify({
                 'unique_names': window.glue_keep_live_unique_names,
             }),
         }
-        const response = fetch(keep_live_url, request_options)
+        const response = await fetch(keep_live_url, request_options)
+        window.glue_session_data = await response.json()
     }
-
 }
```

### Comparing `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,105 +1,89 @@
 class GlueModelObject {
     constructor(unique_name) {
-        this.unique_name = unique_name
-        window.glue_keep_live.add_unique_name(unique_name)
-        this.context_data = {
-            fields: {}
-        }
-    }
+        this.glue_unique_name = unique_name
 
-    generate_field_data() {
-        let data = {}
-        for (let key in this.context_data.fields) {
-            data[key] = this[key]
+        for (let key in window.glue_session_data['context'][unique_name].fields) {
+            this[key] = null
         }
-        return data
-    }
-
-    async get(load_value = true) {
-        await glue_ajax_request(
-            this.unique_name,
-            'get'
-        ).then((response) => {
-            console.log(response)
-            glue_dispatch_response_event(response)
-            let simple_fields = response.data.simple_fields
-            for (let key in simple_fields) {
-                if (load_value) {
-                    this[key] = simple_fields[key]
-                } else {
-                    this[key] = null
-                }
-
-                this.context_data.fields[key] = simple_fields[key]
-            }
-        })
-    }
 
-    async update(field = null) {
-        let data = {}
-
-        if (field) {
-            data[field] = this[field]
-        } else {
-            data = this.generate_field_data()
-        }
-
-        await glue_ajax_request(
-            this.unique_name,
-            'update',
-            data
-        ).then((response) => {
-            glue_dispatch_response_event(response)
-            console.log(response)
-        })
+        window.glue_keep_live.add_unique_name(unique_name)
     }
 
     async create() {
-        let data = this.generate_field_data()
-
         return await glue_ajax_request(
-            this.unique_name,
+            this.glue_unique_name,
             'create',
-            data
+            this.get_properties()
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
-            let model_object = new GlueModelObject(this.unique_name)
-
-            let simple_fields = response.data.simple_fields
-            for (let key in simple_fields) {
-                model_object[key] = simple_fields[key]
-            }
-            return model_object
+            return this
         })
-
     }
 
     delete() {
         glue_ajax_request(
-            this.unique_name,
+            this.glue_unique_name,
             'delete'
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
         })
     }
 
+    async get() {
+        await glue_ajax_request(
+            this.glue_unique_name,
+            'get'
+        ).then((response) => {
+            console.log(response)
+            glue_dispatch_response_event(response)
+            this.set_properties(response.data.simple_fields)
+        })
+    }
+
     async method(method, kwargs = {}) {
         let data = {
             'method': method,
             'kwargs': kwargs,
         }
 
         return await glue_ajax_request(
-            this.unique_name,
+            this.glue_unique_name,
             'method',
             data
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
             return response.data.method_return
         })
     }
 
+    async update(field = null) {
+        await glue_ajax_request(
+            this.glue_unique_name,
+            'update',
+            this.get_properties()
+        ).then((response) => {
+            glue_dispatch_response_event(response)
+            console.log(response)
+        })
+    }
+
+    get_properties() {
+        let properties = {}
+        Object.entries(this).forEach(([key, value]) => {
+            if (!key.startsWith('glue')) {
+                properties[key] = value
+            }
+        });
+        return properties
+    }
+
+    set_properties(properties) {
+        for (let key in properties) {
+            this[key] = properties[key]
+        }
+    }
+
 }
```

### Comparing `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_template.js` & `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_view.js` & `django-glue-0.4.2/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/templates/django_glue/django_glue.html` & `django-glue-0.4.2/django_glue/templates/django_glue/django_glue.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 {% load static %}
 
 {% load django_glue %}
 
 {% csrf_token %}
 
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_keep_live.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
-
 <script type="application/javascript">
     const DJANGO_DEBUG = {% if debug %}true{% else %}false{% endif %}
     const DJANGO_GLUE_AJAX_URL = '{% url 'django_glue:django_glue_data_handler' %}'
     const DJANGO_GLUE_KEEP_LIVE_URL = '{% url 'django_glue:django_glue_keep_live_handler' %}'
 
     window.glue_keep_live = new GlueKeepLive()
+    window.glue_session_data = {{ GLUE_SESSION_DATA|safe }}
+
 
-    setInterval(() => {
-        window.glue_keep_live.update(DJANGO_GLUE_KEEP_LIVE_URL)
-    }, 2000)
 
 </script>
 
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_csrf.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_ajax.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_event.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_response.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_message.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_model_object.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_query_set.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_template.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_view.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
+<script type="application/javascript" src="{% static 'django_glue/js/django_glue_utils.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_shortcuts.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
```

### Comparing `django-glue-0.4.1/django_glue/templatetags/django_glue.py` & `django-glue-0.4.2/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/utils.py` & `django-glue-0.4.2/django_glue/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/django_glue/views.py` & `django-glue-0.4.2/django_glue/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
 
+from django.http import JsonResponse
 from django.shortcuts import HttpResponse
 
 from django_glue.handlers import GlueDataRequestHandler
-from django_glue.sessions import GlueKeepLiveSession
+from django_glue.responses import generate_json_200_response_data
+from django_glue.sessions import GlueKeepLiveSession, GlueSession
 
 
 def glue_data_ajax_handler_view(request):
     return GlueDataRequestHandler(request).process_response()
 
 
 def glue_keep_live_handler_view(request):
     data = json.loads(request.body.decode('utf-8'))
     unique_names = data['unique_names']
 
     GlueKeepLiveSession(request).update_unique_names(unique_names)
 
-    return HttpResponse(status=204)
+    return JsonResponse(
+        data=GlueSession(request).session
+    )
+
```

### Comparing `django-glue-0.4.1/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.2/django_glue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.1
+Version: 0.4.2
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.1/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.2/django_glue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 django_glue/static/django_glue/js/django_glue_keep_live.js
 django_glue/static/django_glue/js/django_glue_message.js
 django_glue/static/django_glue/js/django_glue_model_object.js
 django_glue/static/django_glue/js/django_glue_query_set.js
 django_glue/static/django_glue/js/django_glue_response.js
 django_glue/static/django_glue/js/django_glue_shortcuts.js
 django_glue/static/django_glue/js/django_glue_template.js
+django_glue/static/django_glue/js/django_glue_utils.js
 django_glue/static/django_glue/js/django_glue_view.js
 django_glue/templates/django_glue/django_glue.html
 django_glue/templatetags/__init__.py
 django_glue/templatetags/django_glue.py
 tests/__init__.py
 tests/admin.py
 tests/manage.py
```

### Comparing `django-glue-0.4.1/setup.py` & `django-glue-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/manage.py` & `django-glue-0.4.2/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/migrations/0001_initial.py` & `django-glue-0.4.2/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/models.py` & `django-glue-0.4.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/settings.py` & `django-glue-0.4.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/urls.py` & `django-glue-0.4.2/tests/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.views.generic import TemplateView
 
 from tests import views
 
 urlpatterns = [
     path("", views.ModelObjectView.as_view(), name="model_object"),
     path("query_set/", views.QuerySetView.as_view(), name="query_set"),
+    path("query_set/list/", views.query_set_list_view, name="query_set_list"),
     path("other/", views.OtherView.as_view(), name="other_glue"),
     path("no_glue/", TemplateView.as_view(template_name='page/no_glue_page.html'), name="no_glue"),
     path("benchmark/", views.benchmark_view, name="benchmark"),
     path("django_glue/", include('django_glue.urls', namespace='django_glue')),
     path("template/", views.template_view, name="template"),
     path("view/", views.view_view, name="view"),
     path("view/card/", views.view_card_view, name="view_card"),
```

### Comparing `django-glue-0.4.1/tests/utils.py` & `django-glue-0.4.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.1/tests/views.py` & `django-glue-0.4.2/tests/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,26 @@
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
         add_glue(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('birth_date', 'anniversary_datetime'), methods=['is_lighter_than', 'get_full_name'])
         add_glue(self.request, 'test_query_2', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'add', exclude=('birth_date', 'anniversary_datetime'))
         add_glue(self.request, 'test_query_3', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'change', exclude=('birth_date', 'anniversary_datetime'))
 
+        context_data['model_object_id'] = TestModel.objects.filter(id__gte=1).filter(id__lte=10000).first().id
         return context_data
 
 
+def query_set_list_view(request):
+    add_glue(request, 'test_query_1', TestModel.objects.all(), 'delete')
+    return TemplateResponse(
+        request,
+        template='page/query_set_list_page.html'
+    )
+
+
 class OtherView(TemplateView):
     template_name = 'page/other_glue_page.html'
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
         other_test_model_object = generate_randomized_test_model()
```

