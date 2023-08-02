# Comparing `tmp/cubicweb-forgotpwd-0.9.3.tar.gz` & `tmp/cubicweb-forgotpwd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-forgotpwd-0.9.3.tar", last modified: Mon Apr  4 15:29:35 2022, max compression
+gzip compressed data, was "cubicweb-forgotpwd-1.0.0.tar", last modified: Wed Aug  2 12:39:50 2023, max compression
```

## Comparing `cubicweb-forgotpwd-0.9.3.tar` & `cubicweb-forgotpwd-1.0.0.tar`

### file list

```diff
@@ -1,63 +1,43 @@
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/
--rw-rw-r--   0 katia     (1000) katia     (1000)      525 2022-03-02 15:40:11.000000 cubicweb-forgotpwd-0.9.3/MANIFEST.in
--rw-rw-r--   0 katia     (1000) katia     (1000)     1492 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/PKG-INFO
--rw-rw-r--   0 katia     (1000) katia     (1000)     1015 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/README.rst
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.309768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/
--rw-rw-r--   0 katia     (1000) katia     (1000)       70 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__init__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      203 2022-03-14 09:21:57.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__init__.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     1655 2022-04-04 15:28:50.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pkginfo__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1655 2022-04-04 14:49:39.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pkginfo__.py~
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.309768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/
--rw-rw-r--   0 katia     (1000) katia     (1000)      218 2022-03-14 09:21:01.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      222 2022-03-29 13:54:09.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     1774 2022-03-16 15:45:48.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/__pkginfo__.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     1773 2022-03-29 13:54:11.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/__pkginfo__.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      446 2022-03-14 09:21:04.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/entities.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      450 2022-03-29 13:54:13.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/entities.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     3070 2022-03-21 09:58:55.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/hooks.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     3123 2022-03-29 13:54:13.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/hooks.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      568 2022-03-16 15:45:48.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/site_cubicweb.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      582 2022-03-29 13:54:11.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/site_cubicweb.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     3121 2022-03-21 13:47:05.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/sobjects.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     3129 2022-03-29 13:54:13.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/sobjects.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     7531 2022-03-16 15:45:49.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/views.cpython-37.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)     7514 2022-03-29 13:54:13.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 katia     (1000) katia     (1000)      295 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/entities.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2906 2022-03-21 09:58:51.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/hooks.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3012 2022-03-21 09:49:37.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/hooks.py.orig
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.309768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/
--rw-rw-r--   0 katia     (1000) katia     (1000)     2597 2022-03-21 13:47:47.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/de.po
--rw-rw-r--   0 katia     (1000) katia     (1000)     2611 2022-04-04 15:28:50.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/en.po
--rw-rw-r--   0 katia     (1000) katia     (1000)     2596 2022-04-04 15:28:50.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/es.po
--rw-rw-r--   0 katia     (1000) katia     (1000)     3857 2022-04-04 15:28:50.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/fr.po
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/migration/
--rw-rw-r--   0 katia     (1000) katia     (1000)       80 2022-03-16 15:45:45.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/migration/0.3.0_Any.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      411 2022-03-02 15:40:52.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/migration/postcreate.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      402 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/migration/precreate.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      929 2022-03-02 15:40:52.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/schema.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      646 2022-03-16 15:45:45.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/site_cubicweb.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3356 2022-04-04 15:28:50.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/sobjects.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3348 2022-03-21 09:52:53.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/sobjects.py~
--rw-rw-r--   0 katia     (1000) katia     (1000)     6814 2022-03-16 15:45:45.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/views.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/wdoc/
--rw-rw-r--   0 katia     (1000) katia     (1000)      108 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/wdoc/ChangeLog_en
--rw-rw-r--   0 katia     (1000) katia     (1000)      125 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/wdoc/ChangeLog_fr
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.309768 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/
--rw-rw-r--   0 katia     (1000) katia     (1000)     1492 2022-04-04 15:29:34.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/PKG-INFO
--rw-rw-r--   0 katia     (1000) katia     (1000)     1957 2022-04-04 15:29:35.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/SOURCES.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)        1 2022-04-04 15:29:34.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/dependency_links.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)       48 2022-04-04 15:29:35.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/entry_points.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)        1 2022-03-02 16:30:07.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/not-zip-safe
--rw-rw-r--   0 katia     (1000) katia     (1000)       44 2022-04-04 15:29:35.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/requires.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)       19 2022-04-04 15:29:35.000000 cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/top_level.txt
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/doc/
--rw-rw-r--   0 katia     (1000) katia     (1000)     8820 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/doc/screenshot_login_box.png
--rw-rw-r--   0 katia     (1000) katia     (1000)     6910 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/doc/screenshot_password_reset_form.png
--rw-rw-r--   0 katia     (1000) katia     (1000)       38 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/setup.cfg
--rw-rw-r--   0 katia     (1000) katia     (1000)     2626 2022-03-09 11:34:29.000000 cubicweb-forgotpwd-0.9.3/setup.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/test/
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2022-04-04 15:29:35.313768 cubicweb-forgotpwd-0.9.3/test/data/
--rw-rw-r--   0 katia     (1000) katia     (1000)       10 2021-04-19 15:20:16.000000 cubicweb-forgotpwd-0.9.3/test/data/bootstrap_cubes
--rw-rw-r--   0 katia     (1000) katia     (1000)      477 2022-03-09 11:34:29.000000 cubicweb-forgotpwd-0.9.3/test/test_forgotpwd.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1314 2022-03-16 15:45:45.000000 cubicweb-forgotpwd-0.9.3/test/unittest_notifications.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1240 2022-03-16 15:45:45.000000 cubicweb-forgotpwd-0.9.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.370172 cubicweb-forgotpwd-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-08-02 12:39:50.370172 cubicweb-forgotpwd-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.346172 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.350172 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     3857 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.350172 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/migration/precreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.366172 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/wdoc/ChangeLog_fr
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.350172 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 12:39:50.000000 cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.366172 cubicweb-forgotpwd-1.0.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     8820 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/doc/screenshot_login_box.png
+-rw-rw-rw-   0 root         (0) root         (0)     6910 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/doc/screenshot_password_reset_form.png
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 12:39:50.370172 cubicweb-forgotpwd-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.366172 cubicweb-forgotpwd-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:39:50.370172 cubicweb-forgotpwd-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/test/test_forgotpwd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/test/unittest_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-08-02 12:39:03.000000 cubicweb-forgotpwd-1.0.0/tox.ini
```

### Comparing `cubicweb-forgotpwd-0.9.3/MANIFEST.in` & `cubicweb-forgotpwd-1.0.0/MANIFEST.in`

 * *Files 19% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 recursive-include test *.py
 include test/data/bootstrap_cubes
 
 exclude .gitlab-ci.yml
 exclude .yamllint
 exclude .cube-doctor.yml
 exclude .gitlab-ci-extended.yml
+exclude CHANGELOG.md
```

### Comparing `cubicweb-forgotpwd-0.9.3/PKG-INFO` & `cubicweb-forgotpwd-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-forgotpwd
-Version: 0.9.3
+Version: 1.0.0
 Summary: password recovery component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-forgotpwd
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -42,9 +41,7 @@
       revocation-limit=30 # minutes
 
 3. If the link is valid, the user can change his password in a new form.
 
 There is an automatic task that delete periodically all old Fpasswd which are
 stored in the database. This task is started at the launching of the
 application.
-
-
```

### Comparing `cubicweb-forgotpwd-0.9.3/README.rst` & `cubicweb-forgotpwd-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/__pkginfo__.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/__pkginfo__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 from os import listdir as _listdir
 from os.path import join, isdir
 from glob import glob
 
 modname = "forgotpwd"
 distname = "cubicweb-forgotpwd"
 
-numversion = (0, 9, 3)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "password recovery component for the CubicWeb framework"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python",
     "Programming Language :: JavaScript",
 ]
 
 __depends__ = {
-    "cubicweb[crypto]": ">= 3.25.0, < 3.37.0",
+    "cubicweb[crypto]": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.0.0, < 2.0.0",
     "Pillow": None,
     "six": None,
 }
 
 
 # packaging ###
```

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/hooks.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,15 @@
 link expires in %(limit)s minutes.
 
 See you soon on %(base_url)s !
 """
     )
 
     def subject(self):
-        return self._cw._(
-            "[{}] Request to change your password".format(self._cw.base_url())
-        )
+        return self._cw._(f"[{self._cw.base_url()}] Request to change your password")
 
     def recipients(self):
         fpasswd = self.cw_rset.get_entity(self.cw_row or 0, self.cw_col or 0)
         user = fpasswd.reverse_has_fpasswd[0]
         return [
             (
                 user.cw_adapt_to("IEmailable").get_email(),
```

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/de.po` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/en.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: cubicweb 3.34.1\n"
-"PO-Revision-Date: 2008-03-28 18:14+0100\n"
+"Project-Id-Version: cubicweb 3.5.11\n"
+"PO-Revision-Date: 2010-02-04 19:13+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
-"Language-Team: fr <contact@logilab.fr>\n"
+"Language-Team: en <contact@logilab.fr>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: cubicweb-devtools\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -17,15 +17,15 @@
 
 msgid "An error occured, this email address is unknown."
 msgstr ""
 
 msgid "Forgot your password?"
 msgstr ""
 
-# schema pot file, generated on 2022-03-21 13:47:24
+# schema pot file, generated on 2010-01-21 16:01:14
 #
 # singular and plural forms for each entity type
 msgid "Fpasswd"
 msgstr ""
 
 msgid "Fpasswd_plural"
 msgstr ""
@@ -82,15 +82,15 @@
 msgid "add a Fpasswd"
 msgstr ""
 
 msgid "captcha"
 msgstr ""
 
 # subject and object forms for each relation type
-# (no object form for final or symmetric relation types)
+# (no object form for final or symetric relation types)
 msgid "has_fpasswd"
 msgstr ""
 
 msgctxt "CWUser"
 msgid "has_fpasswd"
 msgstr ""
 
@@ -110,15 +110,15 @@
 msgid "please copy the letters from the image"
 msgstr ""
 
 msgid "required attribute"
 msgstr ""
 
 msgid "revocation_date"
-msgstr ""
+msgstr "revocation date"
 
 msgctxt "Fpasswd"
 msgid "revocation_date"
 msgstr ""
 
 msgid "revocation_id"
 msgstr ""
```

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/en.po` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/es.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: cubicweb 3.5.11\n"
 "PO-Revision-Date: 2010-02-04 19:13+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
-"Language-Team: en <contact@logilab.fr>\n"
+"Language-Team: es <contact@logilab.fr>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: cubicweb-devtools\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -110,15 +110,15 @@
 msgid "please copy the letters from the image"
 msgstr ""
 
 msgid "required attribute"
 msgstr ""
 
 msgid "revocation_date"
-msgstr "revocation date"
+msgstr ""
 
 msgctxt "Fpasswd"
 msgid "revocation_date"
 msgstr ""
 
 msgid "revocation_id"
 msgstr ""
```

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/i18n/fr.po` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/schema.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/site_cubicweb.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/sobjects.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/sobjects.py`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd/views.py` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,42 +2,40 @@
 
 :organization: Logilab
 :copyright: 2001-2011 LOGILAB S.A. (Paris, FRANCE), license is LGPL v2.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
 
-from six import text_type
-
 from yams import ValidationError
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb import _
-from cubicweb.view import StartupView
+from cubicweb_web.view import StartupView
 from cubicweb.crypto import decrypt
-from cubicweb.web import (
+from cubicweb_web import (
     Redirect,
     controller,
     form,
     captcha,
     formwidgets as wdg,
     formfields as ff,
 )
-from cubicweb.web.views import forms, urlrewrite, basetemplates
+from cubicweb_web.views import forms, urlrewrite, basetemplates
 
 
 # Login form
 # ----------
 
 
 class ForgotPasswordLinkWidget(wdg.FieldWidget):
     def render(self, form, field, renderer):
         req = form._cw
-        ret = '<span class="forgotpwdLink"><a href="%s">%s</a></span>' % (
+        ret = '<span class="forgotpwdLink"><a href="{}">{}</a></span>'.format(
             xml_escape(req.build_url("forgottenpassword")),
             req._("Forgot your password?"),
         )
         return ret
 
 
 basetemplates.LogForm.append_field(
@@ -69,15 +67,15 @@
 
 
 class ForgottenPasswordFormView(form.FormViewMixIn, StartupView):
     __regid__ = "forgottenpassword"
 
     def call(self):
         form = self._cw.vreg["forms"].select("forgottenpassword", self._cw)
-        self.w("<p>%s</p>" % self._cw._("Forgot your password?"))
+        self.w(f"<p>{self._cw._('Forgot your password?')}</p>")
         form.render(w=self.w)
 
 
 class ForgottenPasswordSendMailController(controller.Controller):
     __regid__ = "forgottenpassword_sendmail"
 
     def publish(self, rset=None):
@@ -85,15 +83,15 @@
         try:
             with self.appli.repo.internal_cnx() as cnx:
                 cnx.call_service("forgotpwd_send_email", use_email=data["use_email"])
                 cnx.commit()
         except ValidationError:
             raise
         except Exception as exc:
-            msg = text_type(exc)
+            msg = str(exc)
         else:
             msg = self._cw._(
                 "An email has been sent, follow instructions in there to "
                 "change your password."
             )
         raise Redirect(self._cw.build_url("pwdsent", __message=msg))
 
@@ -156,15 +154,15 @@
             raise Redirect(self._cw.build_url("forgottenpassword", __message=msg))
 
     def call(self):
         key = self.check_key()
         form = self._cw.vreg["forms"].select("forgottenpasswordrequest", self._cw)
         form.add_hidden("use_email", key["use_email"])
         form.add_hidden("revocation_id", key["revocation_id"])
-        self.w("<p>%s</p>" % self._cw._("Update your password:"))
+        self.w(f"<p>{self._cw._('Update your password:')}</p>")
         form.render(w=self.w)
 
 
 class ForgottenPasswordRequestConfirm(controller.Controller):
     __regid__ = "forgottenpassword-requestconfirm"
 
     def publish(self, rset=None):
```

### Comparing `cubicweb-forgotpwd-0.9.3/cubicweb_forgotpwd.egg-info/PKG-INFO` & `cubicweb-forgotpwd-1.0.0/cubicweb_forgotpwd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-forgotpwd
-Version: 0.9.3
+Version: 1.0.0
 Summary: password recovery component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-forgotpwd
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -42,9 +41,7 @@
       revocation-limit=30 # minutes
 
 3. If the link is valid, the user can change his password in a new form.
 
 There is an automatic task that delete periodically all old Fpasswd which are
 stored in the database. This task is started at the launching of the
 application.
-
-
```

### Comparing `cubicweb-forgotpwd-0.9.3/doc/screenshot_login_box.png` & `cubicweb-forgotpwd-1.0.0/doc/screenshot_login_box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/doc/screenshot_password_reset_form.png` & `cubicweb-forgotpwd-1.0.0/doc/screenshot_password_reset_form.png`

 * *Files identical despite different names*

### Comparing `cubicweb-forgotpwd-0.9.3/setup.py` & `cubicweb-forgotpwd-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-forgotpwd-0.9.3/test/unittest_notifications.py` & `cubicweb-forgotpwd-1.0.0/test/unittest_notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from cubicweb_web.devtools.testlib import WebCWTC
 from logilab.common.testlib import unittest_main
 
-from cubicweb.devtools.testlib import MAILBOX, CubicWebTC
+from cubicweb.devtools.testlib import MAILBOX
 
 
-class ForgotTC(CubicWebTC):
+class ForgotTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             for index in range(4):
-                user = self.create_user(cnx, "test_user%s" % index)
+                user = self.create_user(cnx, f"test_user{index}")
                 cnx.create_entity(
                     "EmailAddress",
-                    address="test_user%s@logilab.fr" % index,
+                    address=f"test_user{index}@logilab.fr",
                     reverse_use_email=user,
                 )
             cnx.commit()
 
     def test_reset_password(self):
         with self.admin_access.cnx() as cnx:
             count = cnx.execute("Any COUNT(X) WHERE X is Fpasswd")[0][0]
```

### Comparing `cubicweb-forgotpwd-0.9.3/tox.ini` & `cubicweb-forgotpwd-1.0.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
 envlist = py3,check-manifest,yamllint,black,flake8
 
 [testenv]
 deps =
   pytest
+  webtest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
 
 [testenv:check-manifest]
 basepython = python3
 skip_install = true
@@ -19,15 +20,15 @@
 [pytest]
 testpaths = test
 python_files = *test_*.py
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -41,30 +42,29 @@
 commands =
   yamllint .
 
 [testenv:black]
 basepython = python3
 skip_install = true
 deps =
-  black >= 22.1.0
+  black >= 22.12
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
-  black >= 22.1.0
+  black >= 22.12
 commands = black .
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
   flake8 >= 3.6
 commands = flake8
 
 [flake8]
 basepython = python3
-format = pylint
 ignore = W503, E203, E731, E231
 max-line-length = 100
-exclude = cubicweb_risc/migration/*,test/data/*,.tox/*
+exclude = cubicweb_risc/migration/*,test/data/*,.tox/*
```

