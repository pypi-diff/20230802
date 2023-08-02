# Comparing `tmp/django-advanced-pdf-0.2.5.tar.gz` & `tmp/django-advanced-pdf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pdf-0.2.5.tar", last modified: Tue Aug  1 15:06:01 2023, max compression
+gzip compressed data, was "django-advanced-pdf-0.2.6.tar", last modified: Wed Aug  2 08:46:15 2023, max compression
```

## Comparing `django-advanced-pdf-0.2.5.tar` & `django-advanced-pdf-0.2.6.tar`

### file list

```diff
@@ -1,149 +1,160 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.908891 django-advanced-pdf-0.2.5/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-08-01 15:06:01.908712 django-advanced-pdf-0.2.5/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.866811 django-advanced-pdf-0.2.5/django_advanced_pdf/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/.DS_Store
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.867704 django-advanced-pdf-0.2.5/django_advanced_pdf/_trial_temp/
--rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/_trial_temp/_trial_marker
--rw-r--r--   0 tom        (501) staff       (20)       41 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/_trial_temp/test.log
--rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.868579 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.869415 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/parser.py
--rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/style.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.870076 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/data.py
--rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
--rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/png_images.py
--rw-r--r--   0 tom        (501) staff       (20)    56778 2023-08-01 15:04:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/report_xml.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.871003 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/svglib.py
--rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/engine/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.871479 django-advanced-pdf-0.2.5/django_advanced_pdf/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.871990 django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7952 2023-05-03 09:14:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/base.py
--rw-r--r--   0 tom        (501) staff       (20)     5049 2023-05-03 09:07:57.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/border.py
--rw-r--r--   0 tom        (501) staff       (20)     2577 2023-06-14 11:07:49.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/tasks.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.872403 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.872727 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.874714 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.875141 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.875743 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.876958 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.877722 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.879690 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.881148 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.885451 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.888146 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.890843 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/
--rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/abs2.xml
--rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/abs3.xml
--rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/background_colour.xml
--rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/basic.xml
--rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/border.xml
--rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/change_header.xml
--rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/hidden.xml
--rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/keep_with_next.xml
--rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.864119 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.892362 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.893127 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-06-14 10:53:14.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:14.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.893612 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-06-14 10:53:14.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:14.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.894595 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-06-14 10:53:15.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:15.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.895291 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-06-14 10:53:15.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:15.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.897300 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.898471 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-06-14 10:53:16.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-06-14 10:53:17.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:17.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.902746 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-06-14 10:53:17.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-06-14 10:53:17.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-06-14 10:53:17.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:18.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.907645 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-06-14 10:53:20.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-06-14 10:53:20.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-14 10:53:20.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
--rw-r--r--   0 tom        (501) staff       (20)     4852 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/tests.py
--rw-r--r--   0 tom        (501) staff       (20)      336 2023-05-04 10:30:08.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/urls.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.908486 django-advanced-pdf-0.2.5/django_advanced_pdf/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-03 10:37:37.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-05-04 09:14:22.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/views/standard.py
--rw-r--r--   0 tom        (501) staff       (20)     1471 2023-08-01 15:04:51.000000 django-advanced-pdf-0.2.5/django_advanced_pdf/views/tasks.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-01 15:06:01.867493 django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-08-01 15:06:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     5599 2023-08-01 15:06:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-01 15:06:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       20 2023-08-01 15:06:01.000000 django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-08-01 15:06:01.908954 django-advanced-pdf-0.2.5/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      672 2023-08-01 15:04:35.000000 django-advanced-pdf-0.2.5/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.375132 django-advanced-pdf-0.2.6/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-08-02 08:46:15.375011 django-advanced-pdf-0.2.6/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.354812 django-advanced-pdf-0.2.6/django_advanced_pdf/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/.DS_Store
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.355673 django-advanced-pdf-0.2.6/django_advanced_pdf/_trial_temp/
+-rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/_trial_temp/_trial_marker
+-rw-r--r--   0 tom        (501) staff       (20)       41 2023-06-14 10:53:13.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/_trial_temp/test.log
+-rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.356322 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.356963 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/parser.py
+-rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/style.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.357514 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/data.py
+-rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
+-rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/png_images.py
+-rw-r--r--   0 tom        (501) staff       (20)    57073 2023-08-02 08:35:48.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/report_xml.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.358009 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/svglib.py
+-rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/engine/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.358379 django-advanced-pdf-0.2.6/django_advanced_pdf/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.358759 django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7952 2023-05-03 09:14:16.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     5049 2023-05-03 09:07:57.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/border.py
+-rw-r--r--   0 tom        (501) staff       (20)     2577 2023-06-14 11:07:49.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.358989 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.359101 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.359613 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.359867 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.360139 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.360431 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.360693 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.361499 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.362138 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/estimate/
+-rw-r--r--   0 tom        (501) staff       (20)   235980 2023-08-02 08:43:05.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/estimate/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   117474 2023-08-02 08:43:05.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/estimate/2.png
+-rw-r--r--   0 tom        (501) staff       (20)    37939 2023-08-02 08:43:05.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/estimate/3.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:43:05.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/estimate/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.362618 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.364170 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.365063 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.366126 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/
+-rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/abs2.xml
+-rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/abs3.xml
+-rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/background_colour.xml
+-rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/basic.xml
+-rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/border.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/change_header.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7063 2023-08-02 08:36:26.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/estimate.xml
+-rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/hidden.xml
+-rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/keep_with_next.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.352488 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.366591 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-08-02 08:44:18.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-08-02 08:44:19.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:19.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.366826 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-08-02 08:44:19.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:19.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.367047 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-08-02 08:44:19.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:20.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.367324 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-08-02 08:44:20.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:20.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.367578 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-08-02 08:44:20.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:20.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.368331 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.368959 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/estimate/
+-rw-r--r--   0 tom        (501) staff       (20)   235980 2023-08-02 08:44:21.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/estimate/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   117474 2023-08-02 08:44:22.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/estimate/2.png
+-rw-r--r--   0 tom        (501) staff       (20)    37939 2023-08-02 08:44:22.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/estimate/3.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:22.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/estimate/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.369403 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-08-02 08:44:23.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-08-02 08:44:23.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:23.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.371107 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-08-02 08:44:23.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-08-02 08:44:23.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:24.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.372021 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-08-02 08:44:26.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-08-02 08:44:27.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:44:27.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
+-rw-r--r--   0 tom        (501) staff       (20)     4923 2023-08-02 08:43:01.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)      336 2023-05-04 10:30:08.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/urls.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.372702 django-advanced-pdf-0.2.6/django_advanced_pdf/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-03 10:37:37.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-05-04 09:14:22.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/views/standard.py
+-rw-r--r--   0 tom        (501) staff       (20)     1471 2023-08-01 15:04:51.000000 django-advanced-pdf-0.2.6/django_advanced_pdf/views/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-02 08:46:15.355438 django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-08-02 08:46:15.000000 django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     6068 2023-08-02 08:46:15.000000 django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-02 08:46:15.000000 django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       20 2023-08-02 08:46:15.000000 django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-08-02 08:46:15.375171 django-advanced-pdf-0.2.6/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      672 2023-08-02 08:44:57.000000 django-advanced-pdf-0.2.6/setup.py
```

### Comparing `django-advanced-pdf-0.2.5/LICENSE` & `django-advanced-pdf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/PKG-INFO` & `django-advanced-pdf-0.2.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.2.5
+Version: 0.2.6
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/.DS_Store` & `django-advanced-pdf-0.2.6/django_advanced_pdf/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/parser.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/parser.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_paragraph/style.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_paragraph/style.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/data.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/data.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/data_paragraph.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/data_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/png_images.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/png_images.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/report_xml.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/report_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import copy
 import re
 from io import StringIO, BytesIO
-from time import sleep
 
 from lxml import etree
 from reportlab.lib.colors import HexColor, black
 from reportlab.lib.units import mm
 from reportlab.platypus import TableStyle, PageBreak, Spacer, Table
 
 from .enhanced_paragraph.enhanced_paragraph import EnhancedParagraph
@@ -77,14 +76,15 @@
         self.border_left_continuation = 0
         self.border_right_continuation = 0
         self.border_top_continuation = 0
         self.border_bottom_continuation = 0
         self.page_style = None
         self.test_mode = test_mode
         self.status_method = status_method
+        self.held_variables = None
 
         if pager_kwargs is None:
             self.pager_kwargs = {}
         else:
             self.pager_kwargs = pager_kwargs
 
     def load_xml_and_make_pdf(self, xml, add_doctype=True, background_image_first=None,
@@ -273,14 +273,16 @@
             return None
 
         min_rows_top = int(table.get('min_rows_top', 0))
         min_rows_bottom = int(table.get('min_rows_bottom', 0))
 
         rows_variables = []
         variables = {}
+        if self.held_variables is not None:
+            variables = {**self.held_variables}
 
         row_count = -1
         col_widths = []
 
         layout_widths = table.get('layout_widths')
         if layout_widths is not None:
             for col_width in layout_widths.split(','):
@@ -439,14 +441,19 @@
                               repeat_rows=0,
                               headers=headers,
                               footers=footers,
                               h_align=h_align,
                               v_align=v_align,
                               col_widths=new_column_widths,
                               initial=True)
+
+            if len(rows_variables) > 0 and len(rows_variables[-1]) > 0:
+                self.held_variables = rows_variables[-1]
+            else:
+                self.held_variables = None
         else:
             return None
 
         if pos_y is not None and pos_x is not None and page_height is not None:
             ref_is_top = table.get('pos_y_ref', 'top') == 'top'
             ref_is_right = table.get('pos_x_ref', 'left') == 'right'
             ignore_margin = table.get('ignore_margin', 'no') == 'yes'
```

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/svglib.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/svglib.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/svglib/utils.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/svglib/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/engine/utils.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/engine/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/migrations/0001_initial.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/models.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/base.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/pagers/border.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/pagers/border.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/tasks.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/tasks.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/.DS_Store` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/.DS_Store` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs2/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/abs3/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/background_colour/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/basic/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/border/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/3.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/change_header/4.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/hidden/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/3.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/4.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/5.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/6.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/7.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/keep_with_next/8.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/held/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/held/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/abs2.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/abs2.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/abs3.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/abs3.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/basic.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/basic.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/border.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/border.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/change_header.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/change_header.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/hidden.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/hidden.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/keep_with_next.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/keep_with_next.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/reports/overflow_gt_height.xml` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/reports/overflow_gt_height.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs2/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/abs3/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/background_colour/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/basic/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/border/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/3.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/change_header/4.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/hidden/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/3.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/4.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/5.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/6.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/7.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/keep_with_next/8.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.6/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/tests.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
     def test_overflow_gt_height(self):
         self.run_report(name='overflow_gt_height', object_lookup=self.get_sample_objects())
 
     def test_hidden(self):
         self.run_report(name='hidden')
 
+    def test_estimate(self):
+        self.run_report(name='estimate')
+
     @staticmethod
     def get_sample_objects():
         # Define the data for the table
         data = [['Name', 'Age'],
                 ['John', 25],
                 ['Mary', 30],
                 ['Bob', 20],
```

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf/views/tasks.py` & `django-advanced-pdf-0.2.6/django_advanced_pdf/views/tasks.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/PKG-INFO` & `django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.2.5
+Version: 0.2.6
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.2.5/django_advanced_pdf.egg-info/SOURCES.txt` & `django-advanced-pdf-0.2.6/django_advanced_pdf.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 django_advanced_pdf/test_data/held/border/1.png
 django_advanced_pdf/test_data/held/border/page_count.txt
 django_advanced_pdf/test_data/held/change_header/1.png
 django_advanced_pdf/test_data/held/change_header/2.png
 django_advanced_pdf/test_data/held/change_header/3.png
 django_advanced_pdf/test_data/held/change_header/4.png
 django_advanced_pdf/test_data/held/change_header/page_count.txt
+django_advanced_pdf/test_data/held/estimate/1.png
+django_advanced_pdf/test_data/held/estimate/2.png
+django_advanced_pdf/test_data/held/estimate/3.png
+django_advanced_pdf/test_data/held/estimate/page_count.txt
 django_advanced_pdf/test_data/held/hidden/1.png
 django_advanced_pdf/test_data/held/hidden/2.png
 django_advanced_pdf/test_data/held/hidden/page_count.txt
 django_advanced_pdf/test_data/held/keep_with_next/1.png
 django_advanced_pdf/test_data/held/keep_with_next/2.png
 django_advanced_pdf/test_data/held/keep_with_next/3.png
 django_advanced_pdf/test_data/held/keep_with_next/4.png
@@ -71,14 +75,15 @@
 django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
 django_advanced_pdf/test_data/reports/abs2.xml
 django_advanced_pdf/test_data/reports/abs3.xml
 django_advanced_pdf/test_data/reports/background_colour.xml
 django_advanced_pdf/test_data/reports/basic.xml
 django_advanced_pdf/test_data/reports/border.xml
 django_advanced_pdf/test_data/reports/change_header.xml
+django_advanced_pdf/test_data/reports/estimate.xml
 django_advanced_pdf/test_data/reports/hidden.xml
 django_advanced_pdf/test_data/reports/keep_with_next.xml
 django_advanced_pdf/test_data/reports/overflow_gt_height.xml
 django_advanced_pdf/test_data/temp/abs2/1.png
 django_advanced_pdf/test_data/temp/abs2/2.png
 django_advanced_pdf/test_data/temp/abs2/page_count.txt
 django_advanced_pdf/test_data/temp/abs3/1.png
@@ -90,14 +95,18 @@
 django_advanced_pdf/test_data/temp/border/1.png
 django_advanced_pdf/test_data/temp/border/page_count.txt
 django_advanced_pdf/test_data/temp/change_header/1.png
 django_advanced_pdf/test_data/temp/change_header/2.png
 django_advanced_pdf/test_data/temp/change_header/3.png
 django_advanced_pdf/test_data/temp/change_header/4.png
 django_advanced_pdf/test_data/temp/change_header/page_count.txt
+django_advanced_pdf/test_data/temp/estimate/1.png
+django_advanced_pdf/test_data/temp/estimate/2.png
+django_advanced_pdf/test_data/temp/estimate/3.png
+django_advanced_pdf/test_data/temp/estimate/page_count.txt
 django_advanced_pdf/test_data/temp/hidden/1.png
 django_advanced_pdf/test_data/temp/hidden/2.png
 django_advanced_pdf/test_data/temp/hidden/page_count.txt
 django_advanced_pdf/test_data/temp/keep_with_next/1.png
 django_advanced_pdf/test_data/temp/keep_with_next/2.png
 django_advanced_pdf/test_data/temp/keep_with_next/3.png
 django_advanced_pdf/test_data/temp/keep_with_next/4.png
```

### Comparing `django-advanced-pdf-0.2.5/setup.py` & `django-advanced-pdf-0.2.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-pdf",
-    version="0.2.5",
+    version="0.2.6",
     author="Thomas Turner",
     description="Django app that helps one create pdf",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-pdf",
     include_package_data=True,
     packages=['django_advanced_pdf'],
```

