# Comparing `tmp/django-appointment-1.0.0.tar.gz` & `tmp/django-appointment-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-1.0.0.tar", last modified: Mon May  8 20:53:02 2023, max compression
+gzip compressed data, was "django-appointment-1.1.0.tar", last modified: Wed Aug  2 20:09:47 2023, max compression
```

## Comparing `django-appointment-1.0.0.tar` & `django-appointment-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,73 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.359257 django-appointment-1.0.0/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.0.0/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      415 2023-04-27 14:39:53.000000 django-appointment-1.0.0/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-05-08 20:53:02.359346 django-appointment-1.0.0/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.0.0/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.353898 django-appointment-1.0.0/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1022 2023-05-08 14:50:44.000000 django-appointment-1.0.0/appointment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/apps.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      517 2023-04-27 14:53:53.000000 django-appointment-1.0.0/appointment/email_messages.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.354515 django-appointment-1.0.0/appointment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.0.0/appointment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2107 2023-04-27 16:04:51.000000 django-appointment-1.0.0/appointment/email_sender/email_sender.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      227 2023-04-20 14:50:01.000000 django-appointment-1.0.0/appointment/forms.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.355180 django-appointment-1.0.0/appointment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7030 2023-04-24 23:34:09.000000 django-appointment-1.0.0/appointment/migrations/0001_initial.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.0.0/appointment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    10188 2023-05-08 16:54:11.000000 django-appointment-1.0.0/appointment/models.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      844 2023-05-08 14:16:54.000000 django-appointment-1.0.0/appointment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.349265 django-appointment-1.0.0/appointment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.355779 django-appointment-1.0.0/appointment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.0.0/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1827 2023-04-16 18:56:49.000000 django-appointment-1.0.0/appointment/static/css/appointments.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      738 2023-04-22 21:17:10.000000 django-appointment-1.0.0/appointment/static/css/thank_you.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.356015 django-appointment-1.0.0/appointment/static/js/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7251 2023-04-22 17:43:11.000000 django-appointment-1.0.0/appointment/static/js/appointments.js
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.349566 django-appointment-1.0.0/appointment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.357253 django-appointment-1.0.0/appointment/templates/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     7448 2023-05-08 20:49:49.000000 django-appointment-1.0.0/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3442 2023-04-22 17:43:11.000000 django-appointment-1.0.0/appointment/templates/appointment/appointments.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1098 2023-04-22 17:26:13.000000 django-appointment-1.0.0/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1854 2023-05-08 14:48:35.000000 django-appointment-1.0.0/appointment/templates/appointment/enter_verification_code.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.357547 django-appointment-1.0.0/appointment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.0.0/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.358050 django-appointment-1.0.0/appointment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1729 2023-04-27 14:53:53.000000 django-appointment-1.0.0/appointment/templates/email_sender/thank_you_email.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.0.0/appointment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.0.0/appointment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3799 2023-04-22 19:25:04.000000 django-appointment-1.0.0/appointment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    13055 2023-05-08 17:39:26.000000 django-appointment-1.0.0/appointment/views.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.358914 django-appointment-1.0.0/django_appointment.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1197 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-05-08 20:53:02.000000 django-appointment-1.0.0/django_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-05-08 20:53:02.359043 django-appointment-1.0.0/docs/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.0.0/docs/README.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.0.0/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-05-08 20:53:02.359709 django-appointment-1.0.0/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.0.0/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.132937 django-appointment-1.1.0/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.1.0/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      471 2023-07-26 17:35:01.000000 django-appointment-1.1.0/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-08-02 20:09:47.133040 django-appointment-1.1.0/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.1.0/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.124662 django-appointment-1.1.0/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.1.0/appointment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/apps.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.1.0/appointment/email_messages.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.125099 django-appointment-1.1.0/appointment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.1.0/appointment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2109 2023-08-02 20:07:21.000000 django-appointment-1.1.0/appointment/email_sender/email_sender.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.1.0/appointment/forms.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      426 2023-08-02 15:56:11.000000 django-appointment-1.1.0/appointment/logger_config.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.125522 django-appointment-1.1.0/appointment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9615 2023-08-02 20:06:18.000000 django-appointment-1.1.0/appointment/migrations/0001_initial.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    13276 2023-08-02 19:34:58.000000 django-appointment-1.1.0/appointment/models.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.126149 django-appointment-1.1.0/appointment/operations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.1.0/appointment/operations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4226 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/operations/database_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2902 2023-07-31 15:59:24.000000 django-appointment-1.1.0/appointment/operations/email_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3273 2023-07-31 16:46:08.000000 django-appointment-1.1.0/appointment/operations/session_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.1.0/appointment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.119776 django-appointment-1.1.0/appointment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.126890 django-appointment-1.1.0/appointment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.1.0/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5475 2023-07-28 00:05:15.000000 django-appointment-1.1.0/appointment/static/css/appointments.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1272 2023-07-27 15:06:07.000000 django-appointment-1.1.0/appointment/static/css/thank_you.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1241 2023-07-27 14:52:09.000000 django-appointment-1.1.0/appointment/static/css/verification_code.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.127074 django-appointment-1.1.0/appointment/static/js/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8832 2023-07-27 22:28:43.000000 django-appointment-1.1.0/appointment/static/js/appointments.js
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.120127 django-appointment-1.1.0/appointment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.127982 django-appointment-1.1.0/appointment/templates/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8362 2023-07-27 14:32:53.000000 django-appointment-1.1.0/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4869 2023-07-27 23:42:29.000000 django-appointment-1.1.0/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1652 2023-07-27 15:10:09.000000 django-appointment-1.1.0/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1899 2023-07-27 14:52:44.000000 django-appointment-1.1.0/appointment/templates/appointment/enter_verification_code.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.128162 django-appointment-1.1.0/appointment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.1.0/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.128344 django-appointment-1.1.0/appointment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2166 2023-07-27 15:22:04.000000 django-appointment-1.1.0/appointment/templates/email_sender/thank_you_email.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.129077 django-appointment-1.1.0/appointment/tests/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 13:38:19.000000 django-appointment-1.1.0/appointment/tests/__init__.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.130814 django-appointment-1.1.0/appointment/tests/models/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 19:12:45.000000 django-appointment-1.1.0/appointment/tests/models/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5427 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_appointment.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2802 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_appointment_request.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1881 2023-08-02 19:15:12.000000 django-appointment-1.1.0/appointment/tests/models/test_model_config.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1596 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_email_verification.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2785 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_payment_info.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4894 2023-08-02 19:59:36.000000 django-appointment-1.1.0/appointment/tests/models/test_model_service.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8386 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/tests/test_utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     6493 2023-08-02 19:57:09.000000 django-appointment-1.1.0/appointment/tests/test_views.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.1.0/appointment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.1.0/appointment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8306 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    15141 2023-08-02 19:59:36.000000 django-appointment-1.1.0/appointment/views.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.131645 django-appointment-1.1.0/django_appointment.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1932 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.132645 django-appointment-1.1.0/docs/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.1.0/docs/README.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8434 2023-07-31 06:46:57.000000 django-appointment-1.1.0/docs/models.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2595 2023-08-01 14:26:24.000000 django-appointment-1.1.0/docs/operations.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5162 2023-08-01 15:00:53.000000 django-appointment-1.1.0/docs/views.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.1.0/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-08-02 20:09:47.133712 django-appointment-1.1.0/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.1.0/setup.py
```

### Comparing `django-appointment-1.0.0/LICENSE` & `django-appointment-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/PKG-INFO` & `django-appointment-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.0/README.md` & `django-appointment-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/admin.py` & `django-appointment-1.1.0/appointment/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib import admin
 
-from .models import Service, AppointmentRequest, Appointment, EmailVerificationCode
+from .models import Service, AppointmentRequest, Appointment, EmailVerificationCode, Config
 
 
 @admin.register(Service)
 class ServiceAdmin(admin.ModelAdmin):
     list_display = ('name', 'duration', 'price', 'created_at', 'updated_at',)
     search_fields = ('name',)
     list_filter = ('duration',)
@@ -23,7 +23,12 @@
     search_fields = ('client__user__username', 'appointment_request__service__name',)
     list_filter = ('client', 'appointment_request__service',)
 
 
 @admin.register(EmailVerificationCode)
 class EmailVerificationCodeAdmin(admin.ModelAdmin):
     list_display = ('user', 'code')
+
+
+@admin.register(Config)
+class ConfigAdmin(admin.ModelAdmin):
+    list_display = ('slot_duration', 'lead_time', 'finish_time', 'appointment_buffer_time', 'website_name')
```

### Comparing `django-appointment-1.0.0/appointment/email_sender/email_sender.py` & `django-appointment-1.1.0/appointment/email_sender/email_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from django.conf import settings
 from django.core.mail import mail_admins, send_mail
 from django.template import loader
-from django.conf import settings
 
 from appointment.settings import APP_DEFAULT_FROM_EMAIL
 
 
 def has_required_email_settings():
     required_settings = [
         'EMAIL_BACKEND',
@@ -20,14 +20,15 @@
     for setting_name in required_settings:
         if not hasattr(settings, setting_name):
             print(f"Warning: '{setting_name}' not found in settings. Email functionality will be disabled.")
             return False
 
     return True
 
+
 def send_email(recipient_list, subject: str, template_url: str = None, context: dict = None, from_email=None,
                message: str = None):
     if not has_required_email_settings():
         return
 
     if from_email is None:
         from_email = APP_DEFAULT_FROM_EMAIL
@@ -48,14 +49,15 @@
             from_email=from_email,
             recipient_list=recipient_list,
             fail_silently=False,
         )
     except Exception as e:
         print(f"Error sending email: {e}")
 
+
 def notify_admin(subject: str, template_url: str = None, context: dict = None, message: str = None):
     if not has_required_email_settings():
         return
 
     html_message = ""
     if template_url:
         html_message = loader.render_to_string(
```

### Comparing `django-appointment-1.0.0/appointment/migrations/0001_initial.py` & `django-appointment-1.1.0/appointment/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-04-24 23:34
+# Generated by Django 4.2.3 on 2023-08-02 20:06
 
 from django.conf import settings
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 
 
@@ -78,27 +78,39 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "slot_duration",
                     models.PositiveIntegerField(
-                        default=30, help_text="Duration of each slot in minutes"
+                        help_text="Minimum time for an appointment in minutes, recommended 30.",
+                        null=True,
                     ),
                 ),
                 (
                     "lead_time",
                     models.TimeField(
-                        default="09:00", help_text="Time when slots start"
+                        help_text="Time when we start working.", null=True
                     ),
                 ),
                 (
                     "finish_time",
-                    models.TimeField(
-                        default="16:30", help_text="Time when we stop working"
+                    models.TimeField(help_text="Time when we stop working.", null=True),
+                ),
+                (
+                    "appointment_buffer_time",
+                    models.FloatField(
+                        help_text="Time between now and the first available slot for the current day (doesn't affect tomorrow).",
+                        null=True,
+                    ),
+                ),
+                (
+                    "website_name",
+                    models.CharField(
+                        default="", help_text="Name of your website.", max_length=255
                     ),
                 ),
             ],
         ),
         migrations.CreateModel(
             name="Service",
             fields=[
@@ -110,16 +122,42 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("name", models.CharField(max_length=100)),
                 ("description", models.TextField(blank=True, null=True)),
                 ("duration", models.DurationField()),
-                ("price", models.DecimalField(decimal_places=2, max_digits=6)),
-                ("currency", models.CharField(default="USD", max_length=3)),
+                (
+                    "price",
+                    models.DecimalField(
+                        decimal_places=2,
+                        max_digits=6,
+                        validators=[django.core.validators.MinValueValidator(0)],
+                    ),
+                ),
+                (
+                    "down_payment",
+                    models.DecimalField(
+                        decimal_places=2,
+                        default=0,
+                        max_digits=6,
+                        validators=[django.core.validators.MinValueValidator(0)],
+                    ),
+                ),
+                (
+                    "currency",
+                    models.CharField(
+                        default="USD",
+                        max_length=3,
+                        validators=[
+                            django.core.validators.MaxLengthValidator(3),
+                            django.core.validators.MinLengthValidator(3),
+                        ],
+                    ),
+                ),
                 (
                     "image",
                     models.ImageField(blank=True, null=True, upload_to="services/"),
                 ),
                 ("created_at", models.DateTimeField(auto_now_add=True)),
                 ("updated_at", models.DateTimeField(auto_now=True)),
             ],
@@ -144,28 +182,60 @@
                         on_delete=django.db.models.deletion.CASCADE,
                         to="appointment.appointment",
                     ),
                 ),
             ],
         ),
         migrations.CreateModel(
+            name="EmailVerificationCode",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("code", models.CharField(max_length=6)),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                (
+                    "user",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to=settings.AUTH_USER_MODEL,
+                    ),
+                ),
+            ],
+        ),
+        migrations.CreateModel(
             name="AppointmentRequest",
             fields=[
                 (
                     "id",
                     models.BigAutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("date", models.DateField()),
                 ("start_time", models.TimeField()),
                 ("end_time", models.TimeField()),
+                (
+                    "payment_type",
+                    models.CharField(
+                        choices=[("full", "Full payment"), ("down", "Down payment")],
+                        default="full",
+                        max_length=4,
+                    ),
+                ),
                 ("id_request", models.CharField(blank=True, max_length=100, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True)),
                 ("updated_at", models.DateTimeField(auto_now=True)),
                 (
                     "service",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
```

### Comparing `django-appointment-1.0.0/appointment/models.py` & `django-appointment-1.1.0/appointment/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import random
 import string
 
 from django.core.exceptions import ValidationError
-from django.core.validators import RegexValidator
+from django.core.validators import RegexValidator, MinValueValidator, MinLengthValidator, MaxLengthValidator
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from appointment.utils import Utility
 from .settings import APPOINTMENT_CLIENT_MODEL
 
 phone_regex = RegexValidator(
@@ -18,20 +18,27 @@
 PAYMENT_TYPES = (
     ('full', _('Full payment')),
     ('down', _('Down payment')),
 )
 
 
 class Service(models.Model):
+    """
+    Represents a service provided by the appointment system.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.0.0
+    """
     name = models.CharField(max_length=100)
     description = models.TextField(blank=True, null=True)
     duration = models.DurationField()
-    price = models.DecimalField(max_digits=6, decimal_places=2)
-    down_payment = models.DecimalField(max_digits=6, decimal_places=2, default=0)
-    currency = models.CharField(max_length=3, default='USD')
+    price = models.DecimalField(max_digits=6, decimal_places=2, validators=[MinValueValidator(0)])
+    down_payment = models.DecimalField(max_digits=6, decimal_places=2, default=0, validators=[MinValueValidator(0)])
+    currency = models.CharField(max_length=3, default='USD', validators=[MaxLengthValidator(3), MinLengthValidator(3)])
     image = models.ImageField(upload_to='services/', blank=True, null=True)
 
     # meta data
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
@@ -39,20 +46,46 @@
 
     def get_name(self):
         return self.name
 
     def get_description(self):
         return self.description
 
+    def get_duration_parts(self):
+        total_seconds = int(self.duration.total_seconds())
+        days = total_seconds // 86400
+        hours = (total_seconds % 86400) // 3600
+        minutes = (total_seconds % 3600) // 60
+        seconds = total_seconds % 60
+        return days, hours, minutes, seconds
+
     def get_duration(self):
-        return self.duration.seconds // 3600
+        days, hours, minutes, seconds = self.get_duration_parts()
+        parts = []
+
+        if days:
+            parts.append(f"{days} day{'s' if days > 1 else ''}")
+        if hours:
+            parts.append(f"{hours} hour{'s' if hours > 1 else ''}")
+        if minutes:
+            parts.append(f"{minutes} minute{'s' if minutes > 1 else ''}")
+        if seconds:
+            parts.append(f"{seconds} second{'s' if seconds > 1 else ''}")
+
+        return ' '.join(parts)
 
     def get_price(self):
         return self.price
 
+    def get_price_text(self):
+        if self.price == 0:
+            return "Free"
+        else:
+            return f"{self.price} {self.currency}"
+
     def get_down_payment(self):
         return self.down_payment
 
     def get_currency(self):
         return self.currency
 
     def get_image(self):
@@ -66,30 +99,45 @@
 
     def get_updated_at(self):
         return self.updated_at
 
     def is_a_paid_service(self):
         return self.price > 0
 
+    def accepts_down_payment(self):
+        return self.down_payment > 0
+
 
 class AppointmentRequest(models.Model):
+    """
+    Represents an appointment request made by a client.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.0.0
+    """
     date = models.DateField()
     start_time = models.TimeField()
     end_time = models.TimeField()
     service = models.ForeignKey(Service, on_delete=models.CASCADE)
     payment_type = models.CharField(max_length=4, choices=PAYMENT_TYPES, default='full')
     id_request = models.CharField(max_length=100, blank=True, null=True)
 
     # meta data
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
         return f"{self.date} - {self.start_time} to {self.end_time} - {self.service.name}"
 
+    def clean(self):
+        if self.start_time is not None and self.end_time is not None:
+            if self.start_time >= self.end_time:
+                raise ValueError("Start time must be before end time")
+
     def save(self, *args, **kwargs):
         if self.id_request is None:
             self.id_request = f"{Utility.get_timestamp()}{self.service.id}{Utility.generate_random_id()}"
         return super().save(*args, **kwargs)
 
     def get_date(self):
         return self.date
@@ -126,25 +174,35 @@
 
     def get_id_request(self):
         return self.id_request
 
     def is_a_paid_service(self):
         return self.service.is_a_paid_service()
 
+    def accepts_down_payment(self):
+        return self.service.accepts_down_payment()
+
     def get_payment_type(self):
         return self.payment_type
 
     def get_created_at(self):
         return self.created_at
 
     def get_updated_at(self):
         return self.updated_at
 
 
 class Appointment(models.Model):
+    """
+    Represents an appointment made by a client. It is created when the client confirms the appointment request.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.0.0
+    """
     client = models.ForeignKey(APPOINTMENT_CLIENT_MODEL, on_delete=models.CASCADE)
     appointment_request = models.OneToOneField(AppointmentRequest, on_delete=models.CASCADE)
     phone = models.CharField(validators=[phone_regex], max_length=10, blank=True, null=True, default="",
                              help_text=_("Phone number must not contain spaces, letters, parentheses or "
                                          "dashes. It must contain 10 digits."))
     address = models.CharField(max_length=255, blank=True, null=True, default="",
                                help_text=_("Does not have to be specific, just the city and the state"))
@@ -238,41 +296,68 @@
 
     def set_appointment_paid_status(self, status: bool):
         self.paid = status
         self.save()
 
 
 class Config(models.Model):
+    """
+    Represents configuration settings for the appointment system. There can only be one Config object in the database.
+    If you want to change the settings, you must edit the existing Config object.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.1.0
+    """
     slot_duration = models.PositiveIntegerField(
-        default=30,
-        help_text=_("Duration of each slot in minutes"),
+        null=True,
+        help_text=_("Minimum time for an appointment in minutes, recommended 30."),
     )
     lead_time = models.TimeField(
-        default="09:00",
-        help_text=_("Time when slots start"),
+        null=True,
+        help_text=_("Time when we start working."),
     )
     finish_time = models.TimeField(
-        default="16:30",
-        help_text=_("Time when we stop working"),
+        null=True,
+        help_text=_("Time when we stop working."),
+    )
+    appointment_buffer_time = models.FloatField(
+        null=True,
+        help_text=_("Time between now and the first available slot for the current day (doesn't affect tomorrow)."),
+    )
+    website_name = models.CharField(
+        max_length=255,
+        default="",
+        help_text=_("Name of your website."),
     )
 
     def clean(self):
         if Config.objects.exists() and not self.pk:
             raise ValidationError(_("You can only create one Config object"))
+        if self.lead_time is not None and self.finish_time is not None:
+            if self.lead_time >= self.finish_time:
+                raise ValidationError(_("Lead time must be before finish time"))
 
     def save(self, *args, **kwargs):
         self.clean()
         super(Config, self).save(*args, **kwargs)
 
     def __str__(self):
         return f"Config {self.pk}: slot_duration={self.slot_duration}, lead_time={self.lead_time}, " \
                f"finish_time={self.finish_time}"
 
 
 class PaymentInfo(models.Model):
+    """
+    Represents payment information for an appointment.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.0.0
+    """
     appointment = models.ForeignKey(Appointment, on_delete=models.CASCADE)
 
     # meta data
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
@@ -300,14 +385,21 @@
         return self.appointment.get_client().first_name
 
     def get_user_email(self):
         return self.appointment.get_client().email
 
 
 class EmailVerificationCode(models.Model):
+    """
+    Represents an email verification code for a user when the email already exists in the database.
+
+    Author: Adams Pierre David
+    Version: 1.1.0
+    Since: 1.1.0
+    """
     user = models.ForeignKey(APPOINTMENT_CLIENT_MODEL, on_delete=models.CASCADE)
     code = models.CharField(max_length=6)
 
     # meta data
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
```

### Comparing `django-appointment-1.0.0/appointment/settings.py` & `django-appointment-1.1.0/appointment/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,10 +3,12 @@
 
 APPOINTMENT_CLIENT_MODEL = getattr(settings, 'APPOINTMENT_CLIENT_MODEL', 'auth.User')
 APPOINTMENT_BASE_TEMPLATE = getattr(settings, 'APPOINTMENT_BASE_TEMPLATE', 'base_templates/base.html')
 APPOINTMENT_WEBSITE_NAME = getattr(settings, 'APPOINTMENT_WEBSITE_NAME', 'Website')
 APPOINTMENT_PAYMENT_URL = getattr(settings, 'APPOINTMENT_PAYMENT_URL', None)
 APPOINTMENT_THANK_YOU_URL = getattr(settings, 'APPOINTMENT_THANK_YOU_URL', None)
 APPOINTMENT_SLOT_DURATION = getattr(settings, 'APPOINTMENT_SLOT_DURATION', 30)
+APPOINTMENT_BUFFER_TIME = getattr(settings, 'APPOINTMENT_BUFFER_TIME', 0)
 APPOINTMENT_LEAD_TIME = getattr(settings, 'APPOINTMENT_LEAD_TIME', (9, 0))
-APPOINTMENT_FINISH_TIME = getattr(settings, 'APPOINTMENT_FINISH_TIME', (16, 30))
+APPOINTMENT_FINISH_TIME = getattr(settings, 'APPOINTMENT_FINISH_TIME', (18, 30))
 APP_DEFAULT_FROM_EMAIL = getattr(settings, 'DEFAULT_FROM_EMAIL', DEFAULT_FROM_EMAIL)
+APP_TIME_ZONE = getattr(settings, 'TIME_ZONE', 'America/New_York')
```

### Comparing `django-appointment-1.0.0/appointment/static/css/appointments-user-details.css` & `django-appointment-1.1.0/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/static/js/appointments.js` & `django-appointment-1.1.0/appointment/static/js/appointments.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,206 +1,220 @@
 const calendarEl = document.getElementById('calendar');
-const nextAvailableDateSelector = $('.next-available-date')
+let nextAvailableDateSelector = $('.djangoAppt_next-available-date')
 const body = $('body');
 
 const calendar = new FullCalendar.Calendar(calendarEl, {
     initialView: 'dayGridMonth',
     headerToolbar: {
         left: 'title',
         right: 'prev,today,next',
     },
     height: '400px',
-    width: '80%',
     themeSystem: 'bootstrap',
-    color: 'black',
+    nowIndicator: true,
+    bootstrapFontAwesome: {
+        close: 'fa-times',
+        prev: 'fa-chevron-left',
+        next: 'fa-chevron-right',
+        prevYear: 'fa-angle-double-left',
+        nextYear: 'fa-angle-double-right'
+    },
     selectable: true,
     dateClick: function(info) {
-        // Convert the selected date string to a Date object
-        const selectedDate = new Date(info.dateStr);
-
-        // Get today's date
-        const today = new Date();
-        today.setHours(0, 0, 0, 0);
-        const slotContainer = $('.slot-container');
-        const appointmentSlot = $('.appointment-slot');
-        // Check if the selected date is in the past
-        if (selectedDate < today) {
-            // Show an error message
-            if (slotContainer.find('.no-availability-text').length === 0) {
-                slotContainer.append('<p class="no-availability-text">Date is in the past.</p>');
-                appointmentSlot.remove();
-            }
-        } else {
-            // Call the getAvailableSlots function
-            getAvailableSlots(info.dateStr);
-        }
+        getAvailableSlots(info.dateStr);
     },
     selectAllow: function(info) {
         return (info.start >= getDateWithoutTime(new Date()));
     },
 });
 
 calendar.setOption('locale', locale);
 
-function getDateWithoutTime(dt) {
-    dt.setHours(0, 0, 0, 0);
-    return dt;
-}
-
 $(document).ready(function() {
     calendar.render();
     const currentDate = new Date().toISOString().slice(0, 10);
     getAvailableSlots(currentDate);
 });
 
+body.on('click', '.djangoAppt_btn-request-next-slot', function() {
+    const serviceId = $(this).data('service-id');
+    requestNextAvailableSlot(serviceId);
+})
+
+body.on('click', '.btn-submit-appointment', function() {
+    const selectedSlot = $('.djangoAppt_appointment-slot.selected').text();
+    const selectedDate = $('.djangoAppt_date_chosen').text();
+    if (!selectedSlot || !selectedDate) {
+        alert('Please select a date and time');
+        return;
+    }
+    if (selectedSlot && selectedDate) {
+        const startTime = convertTo24Hour(selectedSlot);
+        const APPOINTMENT_BASE_TEMPLATE = localStorage.getItem('APPOINTMENT_BASE_TEMPLATE');
+        // Convert the selectedDate string to a valid format
+        const dateParts = selectedDate.split(', ');
+        const monthDayYear = dateParts[1] + "," + dateParts[2];
+        const formattedDate = new Date(monthDayYear + " " + startTime);
+
+        const date = formattedDate.toISOString().slice(0, 10);
+        const endTimeDate = new Date(formattedDate.getTime() + serviceDuration * 60000);
+        const endTime = formatTime(endTimeDate);
+
+        const form = $('.appointment-form');
+
+        form.append($('<input>', {
+            type: 'hidden',
+            name: 'date',
+            value: date
+        }));
+        form.append($('<input>', {
+            type: 'hidden',
+            name: 'start_time',
+            value: startTime
+        }));
+        form.append($('<input>', {
+            type: 'hidden',
+            name: 'end_time',
+            value: endTime
+        }));
+        form.append($('<input>', {
+            type: 'hidden',
+            name: 'service',
+            value: serviceId
+        }));
+        form.submit();
+    } else {
+        const warningContainer = $('.warning-message');
+        if (warningContainer.find('submit-warning') === 0) {
+            warningContainer.append('<p class="submit-warning">Please select a time slot before submitting the appointment request.</p>');
+        }
+    }
+});
+
+function getDateWithoutTime(dt) {
+    dt.setHours(0, 0, 0, 0);
+    return dt;
+}
+
+function convertTo24Hour(time12h) {
+    const [time, modifier] = time12h.split(' ');
+    let [hours, minutes] = time.split(':');
+
+    if (hours === '12') {
+        hours = '00';
+    }
+
+    if (modifier.toUpperCase() === 'PM') {
+        hours = parseInt(hours, 10) + 12;
+    }
+
+    return `${hours}:${minutes}`;
+}
+
+function formatTime(date) {
+    const hours = date.getHours();
+    const minutes = date.getMinutes();
+    return (hours < 10 ? '0' + hours : hours) + ':' + (minutes < 10 ? '0' + minutes : minutes);
+}
+
 function getAvailableSlots(selectedDate) {
     // Send an AJAX request to get the available slots for the selected date
     $.ajax({
         url: availableSlotsAjaxURL,
         data: {
             'selected_date': selectedDate,
         },
         dataType: 'json',
         success: function(data) {
             // Update the slot list with the available slots for the selected date
             const slotList = $('#slot-list');
             slotList.empty();
             const slotContainer = $('.slot-container');
+            // Remove the "Next available date" message
+            nextAvailableDateSelector = $('.djangoAppt_next-available-date'); // Update the selector
+            nextAvailableDateSelector.remove();
+            const errorMessageContainer = $('.error-message');
+
             if (data.available_slots.length === 0) {
-                if (slotContainer.find('.no-availability-text').length === 0) {
-                    slotContainer.append('<p class="no-availability-text">No availability</p>');
+                const selectedDateObj = moment.tz(selectedDate, timezone);
+                const selectedD = selectedDateObj.toDate();
+                const today = new Date();
+                today.setHours(0, 0, 0, 0);
+
+                if (selectedD < today) {
+                    errorMessageContainer.find('.djangoAppt_no-availability-text').remove();
+                    // Show an error message
+                    errorMessageContainer.append('<p class="djangoAppt_no-availability-text">Date is in the past.</p>');
+                    if (slotContainer.find('.djangoAppt_btn-request-next-slot').length === 0) {
+                        slotContainer.append(`<button class="btn btn-danger djangoAppt_btn-request-next-slot" data-service-id="${serviceId}">Request next available slot</button>`);
+                    }
+                    // Disable the submit button
+                    $('.btn-submit-appointment').attr('disabled', 'disabled');
+                } else {
+                    errorMessageContainer.find('.djangoAppt_no-availability-text').remove();
+                    if (errorMessageContainer.find('.djangoAppt_no-availability-text').length === 0) {
+                        errorMessageContainer.append('<p class="djangoAppt_no-availability-text">No availability</p>');
+                    }
+                    if (slotContainer.find('.djangoAppt_btn-request-next-slot').length === 0) {
+                        slotContainer.append(`<button class="btn btn-danger djangoAppt_btn-request-next-slot" data-service-id="${serviceId}">Request next available slot</button>`);
+                    }
                 }
-                slotContainer.append(`<button class="btn btn-dark btn-request-next-slot" data-service-id="${serviceId}">Request for next available slot</button>`);
             } else {
                 // remove the button to request for next available slot
-                $('.no-availability-text').remove();
-                $('.btn-request-next-slot').remove();
-                nextAvailableDateSelector.remove();
+                $('.djangoAppt_no-availability-text').remove();
+                $('.djangoAppt_btn-request-next-slot').remove();
                 const uniqueSlots = [...new Set(data.available_slots)]; // remove duplicates
                 for (let i = 0; i < uniqueSlots.length; i++) {
-                    slotList.append('<li class="appointment-slot">' + uniqueSlots[i] + '</li>');
+                    slotList.append('<li class="djangoAppt_appointment-slot">' + uniqueSlots[i] + '</li>');
                 }
+
+                // Attach click event to the slots
+                $('.djangoAppt_appointment-slot').on('click', function() {
+                    // Remove the 'selected' class from all other appointment slots
+                    $('.djangoAppt_appointment-slot').removeClass('selected');
+
+                    // Add the 'selected' class to the clicked appointment slot
+                    $(this).addClass('selected');
+
+                    // Enable the submit button
+                    $('.btn-submit-appointment').removeAttr('disabled');
+
+                    // Continue with the existing logic
+                    const selectedSlot = $(this).text();
+                    $('#service-datetime-chosen').text(data.date_chosen + ' ' + selectedSlot);
+                });
             }
             // Update the date chosen
-            $('.date_chosen').text(data.date_chosen);
-
-            $('.appointment-slot').on('click', function() {
-                // Remove the 'selected' class from all other appointment slots
-                $('.appointment-slot').removeClass('selected');
-
-                // Add the 'selected' class to the clicked appointment slot
-                $(this).addClass('selected');
-
-                // Continue with the existing logic
-                const selectedSlot = $(this).text();
-                $('#service-datetime-chosen').text(data.date_chosen + ' ' + selectedSlot);
-            });
-
+            $('.djangoAppt_date_chosen').text(data.date_chosen);
         }
     });
 }
 
-body.on('click', '.btn-request-next-slot', function() {
-    const serviceId = $(this).data('service-id');
-    requestNextAvailableSlot(serviceId);
-})
-
 function requestNextAvailableSlot(serviceId) {
     const requestNextAvailableSlotURL = requestNextAvailableSlotURLTemplate.replace('0', serviceId);
     $.ajax({
         url: requestNextAvailableSlotURL,
         dataType: 'json',
         success: function(data) {
             // Set the date in the calendar to the next available date
-            const nextAvailableDate = new Date(data.next_available_date);
+            const nextAvailableDateResponse = data.next_available_date;
+            const selectedDateObj = moment.tz(nextAvailableDateResponse, timezone);
+            const nextAvailableDate = selectedDateObj.toDate();
             const formattedDate = new Intl.DateTimeFormat('en-US', {
                 year: 'numeric',
                 month: 'long',
                 day: 'numeric'
             }).format(nextAvailableDate);
 
-
             // Check if the .next-available-date element already exists
+            nextAvailableDateSelector = $('.djangoAppt_next-available-date'); // Update the selector
             if (nextAvailableDateSelector.length > 0) {
                 // Update the content of the existing .next-available-date element
                 nextAvailableDateSelector.text(`Next available date: ${formattedDate}`);
             } else {
                 // If the .next-available-date element doesn't exist, create and append it
-                const nextDateText = `<p class="next-available-date">Next available date: <br>${formattedDate}</p>`;
-                $('.btn-request-next-slot').after(nextDateText);
+                const nextDateText = `<p class="djangoAppt_next-available-date">Next available date: <br>${formattedDate}</p>`;
+                $('.djangoAppt_btn-request-next-slot').after(nextDateText);
             }
         }
     });
-}
-
-function convertTo24Hour(time12h) {
-    const [time, modifier] = time12h.split(' ');
-    let [hours, minutes] = time.split(':');
-
-    if (hours === '12') {
-        hours = '00';
-    }
-
-    if (modifier.toUpperCase() === 'PM') {
-        hours = parseInt(hours, 10) + 12;
-    }
-
-    return `${hours}:${minutes}`;
-}
-
-function formatTime(date) {
-    const hours = date.getHours();
-    const minutes = date.getMinutes();
-    return (hours < 10 ? '0' + hours : hours) + ':' + (minutes < 10 ? '0' + minutes : minutes);
-}
-
-body.on('click', '.btn-submit-appointment', function() {
-    const selectedSlot = $('.appointment-slot.selected').text();
-    const selectedDate = $('.date_chosen').text();
-    if (selectedSlot && selectedDate) {
-        const startTime = convertTo24Hour(selectedSlot);
-
-        // Convert the selectedDate string to a valid format
-        const dateParts = selectedDate.split(', ');
-        const monthDayYear = dateParts[1] + "," + dateParts[2];
-        const formattedDate = new Date(monthDayYear + " " + startTime);
-
-        const date = formattedDate.toISOString().slice(0, 10);
-        const endTimeDate = new Date(formattedDate.getTime() + serviceDuration * 60000);
-        const endTime = formatTime(endTimeDate);
-
-        console.log("Testing...")
-        console.log("end time date: " + endTimeDate);
-        console.log("date: " + date);
-        console.log("start time: " + startTime);
-        console.log("end time: " + endTime);
-        console.log("service: " + serviceId);
-
-        const form = $('.appointment-form');
-
-        form.append($('<input>', {
-            type: 'hidden',
-            name: 'date',
-            value: date
-        }));
-        form.append($('<input>', {
-            type: 'hidden',
-            name: 'start_time',
-            value: startTime
-        }));
-        form.append($('<input>', {
-            type: 'hidden',
-            name: 'end_time',
-            value: endTime
-        }));
-        form.append($('<input>', {
-            type: 'hidden',
-            name: 'service',
-            value: serviceId
-        }));
-
-        console.log("Submitting form...");
-        form.submit();
-    } else {
-        alert('Please select a time slot before submitting the appointment request.');
-    }
-});
+}
```

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/appointments.html` & `django-appointment-1.1.0/appointment/templates/appointment/appointments.html`

 * *Files 24% similar despite different names*

```diff
@@ -7,69 +7,86 @@
 {% block title %}
     {{ page_title }}
 {% endblock %}
 {% block description %}
     {{ page_description }}
 {% endblock %}
 {% block body %}
-    <div class="main-container">
-        <div class="body-container">
-            <h1 class="page-title">{{ service.name }}</h1>
-            <small class="page-description">
-                {% trans "Check out our availability and book the date and time that works for you" %}
-            </small>
-            <hr>
+    <div class="container">
+        <div class="djangoAppt_main-container">
+            <div class="djangoAppt_body-container">
+                <h1 class="page-title">{{ service.name }}</h1>
+                <small class="page-description">
+                    {% trans "Check out our availability and book the date and time that works for you" %}
+                </small>
+                <hr>
 
-            <div class="page-body">
-                <div class="appointment-calendar">
-                    <div class="appointment-calendar-title-timezone">
-                        <div class="title">
-                            {% trans "Select a date and time" %}
+                <div class="djangoAppt_page-body">
+                    <div class="djangoAppt_appointment-calendar">
+                        <div class="djangoAppt_appointment-calendar-title-timezone">
+                            <div class="djangoAppt_title">
+                                {% trans "Select a date and time" %}
+                            </div>
+                            <div class="djangoAppt_timezone-details">
+                                {% trans "Timezone" %}:&nbsp;{{ timezoneTxt }}
+                            </div>
                         </div>
-                        <div class="timezone-details">
-                            {% trans "Timezone" %}:&nbsp;{% trans "Eastern Daylight Time (EDT)" %}
+                        <hr class="djangoAppt_second-part">
+                        <div class="djangoAppt_calendar-and-slot">
+                            <div class="djangoAppt_calendar" id="calendar">
+                            </div>
+                            <div class="djangoAppt_slot">
+                                <div class="djangoAppt_date_chosen">{{ date_chosen }}</div>
+                                <div class="slot-container">
+                                    <div class="error-message"></div>
+                                    <ul id="slot-list" class="djangoAppt_slot-list">
+                                        <!-- Slot list will be updated dynamically by the AJAX request -->
+                                    </ul>
+                                </div>
+
+                            </div>
                         </div>
                     </div>
-                    <hr class="second-part">
-                    <div class="calendar-and-slot">
-                        <div class="calendar" id="calendar">
-                        </div>
-                        <div class="slot">
-                            <div class="date_chosen">{{ date_chosen }}</div>
-                            <div class="slot-container">
-                                <ul id="slot-list" class="slot-list">
-                                    <!-- Slot list will be updated dynamically by the AJAX request -->
-                                </ul>
+                    <div class="djangoAppt_service-description">
+                        <form method="post" action="{% url 'appointment:appointment_request_submit' %}"
+                              class="appointment-form">
+                            {% csrf_token %}
+                            <div>{% trans "Service Details" %}</div>
+                            <hr class="djangoAppt_second-part">
+                            <div class="djangoAppt_service-description-content">
+                                <p class="djangoAppt_item-name">{{ service.name }}</p>
+                                <p id="service-datetime-chosen" class="service-datetime-chosen">{{ date_chosen }}</p>
+                                <p>{{ service.get_duration }}</p>
+                                <p>{{ service.get_price_text }}</p>
+                                <button type="submit"
+                                        class="btn btn-primary btn-submit-appointment"
+                                        disabled>{% trans 'Next' %}</button>
                             </div>
-                        </div>
+                        </form>
                     </div>
                 </div>
-                <div class="service-description">
-                    <form method="post" action="{% url 'appointment:appointment_request_submit' %}"
-                    class="appointment-form">
-                        {% csrf_token %}
-                        <div>{% trans "Service Details" %}</div>
-                        <hr class="second-part">
-                        <div class="service-description-content">
-                            <p class="item-name">{{ service.name }}</p>
-                            <p id="service-datetime-chosen" class="service-datetime-chosen">{{ date_chosen }}</p>
-                            <p>{{ service.get_duration }} hr</p>
-                            <p>${{ service.price }}</p>
-                            <button type="submit" class="btn btn-dark btn-submit-appointment">{% trans 'Next' %}</button>
-                        </div>
-                    </form>
-                </div>
+                {% if messages %}
+                    {% for message in messages %}
+                        <div class="alert alert-dismissible {% if message.tags %}alert-{% if message.level == DEFAULT_MESSAGE_LEVELS.ERROR %}danger{% else %}{{ message.tags }}{% endif %}{% endif %}"
+                             role="alert">{{ message }}</div>
+                    {% endfor %}
+                {% endif %}
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block customJS %}
+    <script src='https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.4/moment.min.js'></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/moment-timezone/0.5.43/moment-timezone-with-data.min.js"
+            integrity="sha512-KCI+fR3bUbOcU0ZC3UcaPwCLuO5LEkukaWBYddmhLPXgpAPWJ8j6pJLmTI6t9CMYczE4YCrWZQ/wrZz/JsyC+A=="
+            crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src='https://cdn.jsdelivr.net/npm/fullcalendar@6.1.5/index.global.min.js'></script>
     <script>
+        const timezone = "{{ timezone }}";
         const locale = "{{ locale }}";
         const availableSlotsAjaxURL = "{% url 'appointment:available_slots_ajax' %}";
         const requestNextAvailableSlotURLTemplate = "{% url 'appointment:request_next_available_slot' service_id=0 %}";
         const serviceId = "{{ service.id }}";
         const serviceDuration = parseInt("{{ service.duration.total_seconds }}") / 60;
     </script>
     <script src="{% static 'js/appointments.js' %}"></script>
```

#### html2text {}

```diff
@@ -3,20 +3,23 @@
  {% endblock %} {% block title %} {{ page_title }} {% endblock %} {% block
 description %} {{ page_description }} {% endblock %} {% block body %}
 ****** {{ service.name }} ******
 {% trans "Check out our availability and book the date and time that works for
 you" %}
 ===============================================================================
 {% trans "Select a date and time" %}
-{% trans "Timezone" %}: {% trans "Eastern Daylight Time (EDT)" %}
+{% trans "Timezone" %}: {{ timezoneTxt }}
 ===============================================================================
 {{ date_chosen }}
 {% csrf_token %}
 {% trans "Service Details" %}
 ===============================================================================
 {{ service.name }}
 {{ date_chosen }}
-{{ service.get_duration }} hr
-${{ service.price }}
+{{ service.get_duration }}
+{{ service.get_price_text }}
 {% trans 'Next' %}
+{% if messages %} {% for message in messages %}
+{{ message }}
+{% endfor %} {% endif %}
 {% endblock %} {% block customJS %}
  {% endblock %}
```

### Comparing `django-appointment-1.0.0/appointment/templates/appointment/enter_verification_code.html` & `django-appointment-1.1.0/appointment/templates/appointment/enter_verification_code.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 {% extends APPOINTMENT_BASE_TEMPLATE %}
 {% load i18n %}
 {% load static %}
 {% block customCSS %}
-    <link rel="stylesheet" type="text/css" href="{% static 'css/thank_you.css' %}"/>
+    <link rel="stylesheet" type="text/css" href="{% static 'css/verification_code.css' %}"/>
 {% endblock %}
 {% block title %}
     Enter Verification Code
 {% endblock %}
 {% block description %}
     Enter Verification Code
 {% endblock %}
 {% block body %}
     <div class="container">
-        {% if messages %}
-            {% for message in messages %}
-                <div class="alert alert-dismissible {% if message.tags %}alert-{% if message.level == DEFAULT_MESSAGE_LEVELS.ERROR %}danger{% else %}{{ message.tags }}{% endif %}{% endif %}"
-                     role="alert">{{ message }}</div>
-            {% endfor %}
-        {% endif %}
         <div class="main-container">
             <div class="body-container">
                 <h1>Enter Verification Code</h1>
                 <p>We've sent a verification code to your email. Please enter it below:</p>
                 <form method="post"
                       action="{% url 'appointment:enter_verification_code' appointment_request_id id_request %}">
                     {% csrf_token %}
                     <label>Code:
-                        <input type="text" name="code" placeholder="Verification Code" required>
+                        <input type="text" name="code" placeholder="X1Y2Z3" required>
                     </label>
-                    <button type="submit">Submit</button>
+                    <button class="btn btn-primary" type="submit">Submit</button>
                 </form>
             </div>
+            {% if messages %}
+                {% for message in messages %}
+                    <div class="alert alert-dismissible {% if message.tags %}alert-{% if message.level == DEFAULT_MESSAGE_LEVELS.ERROR %}danger{% else %}{{ message.tags }}{% endif %}{% endif %}"
+                         role="alert">{{ message }}</div>
+                {% endfor %}
+            {% endif %}
         </div>
     </div>
 {% endblock %}
 {% block customJS %}
     <script>
         document.addEventListener('DOMContentLoaded', function () {
             const messageElements = document.querySelectorAll('.alert-dismissible');
```

### Comparing `django-appointment-1.0.0/appointment/templates/base_templates/base.html` & `django-appointment-1.1.0/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/tests.py` & `django-appointment-1.1.0/appointment/tests.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/appointment/urls.py` & `django-appointment-1.1.0/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/django_appointment.egg-info/PKG-INFO` & `django-appointment-1.1.0/django_appointment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-appointment-1.0.0/docs/README.md` & `django-appointment-1.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.0.0/setup.cfg` & `django-appointment-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-appointment
-version = 1.0.0
+version = 1.1.0
 description = A Django app for managing appointment scheduling with ease and flexibility.
 url = https://github.com/adamspd/django-appointment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
```

