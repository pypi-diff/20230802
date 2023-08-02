# Comparing `tmp/inhandtest-0.0.62.tar.gz` & `tmp/inhandtest-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.62.tar", last modified: Thu Jul 27 06:49:58 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.63.tar", last modified: Wed Aug  2 06:09:21 2023, max compression
```

## Comparing `inhandtest-0.0.62.tar` & `inhandtest-0.0.63.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.62/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-07-27 06:49:58.000000 inhandtest-0.0.62/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.62/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.62/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.62/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.62/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.62/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.62/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    66544 2023-07-26 06:03:35.000000 inhandtest-0.0.62/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.62/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.62/inhandtest/exception.py
--rw-rw-rw-   0        0        0     5565 2023-07-27 05:23:00.000000 inhandtest-0.0.62/inhandtest/file.py
--rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.62/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.62/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.62/inhandtest/inmqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/inrequest/
--rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.62/inhandtest/inrequest/__init__.py
--rw-rw-rw-   0        0        0    10424 2023-07-20 10:21:59.000000 inhandtest-0.0.62/inhandtest/inrequest/console.py
--rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.62/inhandtest/inrequest/dm.py
--rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.62/inhandtest/inrequest/dn.py
--rw-rw-rw-   0        0        0    14989 2023-07-24 08:32:31.000000 inhandtest-0.0.62/inhandtest/inrequest/er_default_config.py
--rw-rw-rw-   0        0        0    37418 2023-07-27 06:47:07.000000 inhandtest-0.0.62/inhandtest/inrequest/er_device.py
--rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.62/inhandtest/inrequest/ics.py
--rw-rw-rw-   0        0        0    11175 2023-07-24 02:46:52.000000 inhandtest-0.0.62/inhandtest/inrequest/inrequest.py
--rw-rw-rw-   0        0        0    52445 2023-07-27 01:28:14.000000 inhandtest-0.0.62/inhandtest/inrequest/nezha.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.62/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.62/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.62/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.62/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.62/inhandtest/log.py
--rw-rw-rw-   0        0        0    15229 2023-07-18 03:57:23.000000 inhandtest-0.0.62/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.62/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.62/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    68559 2023-07-24 09:52:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    76038 2023-07-21 09:18:02.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    12188 2023-07-24 09:42:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.62/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    35543 2023-07-27 03:55:47.000000 inhandtest-0.0.62/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    30974 2023-07-27 05:13:54.000000 inhandtest-0.0.62/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2023-07-24 08:29:33.000000 inhandtest-0.0.62/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 06:49:58.000000 inhandtest-0.0.62/setup.cfg
--rw-rw-rw-   0        0        0     1625 2023-07-27 06:46:21.000000 inhandtest-0.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.63/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-08-02 06:09:21.000000 inhandtest-0.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.63/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.63/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.63/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.63/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.63/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.63/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    66800 2023-07-28 06:14:30.000000 inhandtest-0.0.63/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    27535 2023-08-01 07:15:28.000000 inhandtest-0.0.63/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.63/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     6365 2023-08-01 03:34:58.000000 inhandtest-0.0.63/inhandtest/file.py
+-rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.63/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.63/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.63/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.63/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0    10424 2023-07-20 10:21:59.000000 inhandtest-0.0.63/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.63/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.63/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0    14989 2023-07-24 08:32:31.000000 inhandtest-0.0.63/inhandtest/inrequest/er_default_config.py
+-rw-rw-rw-   0        0        0    37418 2023-07-27 06:47:07.000000 inhandtest-0.0.63/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.63/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0    11198 2023-08-02 01:37:41.000000 inhandtest-0.0.63/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0    53371 2023-08-02 01:43:31.000000 inhandtest-0.0.63/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.63/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.63/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.63/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.63/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.63/inhandtest/log.py
+-rw-rw-rw-   0        0        0    15229 2023-07-18 03:57:23.000000 inhandtest-0.0.63/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.63/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.63/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    68401 2023-07-28 06:15:35.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    75780 2023-07-28 06:11:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3617 2023-07-28 06:11:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    12188 2023-07-24 09:42:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.63/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    35543 2023-07-27 03:55:47.000000 inhandtest-0.0.63/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    30974 2023-07-27 05:13:54.000000 inhandtest-0.0.63/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2023-07-24 08:29:33.000000 inhandtest-0.0.63/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 06:09:21.000000 inhandtest-0.0.63/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-08-02 06:09:07.000000 inhandtest-0.0.63/setup.py
```

### Comparing `inhandtest-0.0.62/PKG-INFO` & `inhandtest-0.0.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.62
+Version: 0.0.63
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.62/README.md` & `inhandtest-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.63/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.63/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.63/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/base_page/base_page.py` & `inhandtest-0.0.63/inhandtest/base_page/base_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,26 +36,28 @@
         :param port: 端口
         :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'|'IR305'|'IR615'
         :param page: 当page为None时，自动打开浏览器及页面，否则使用传入的page
         :param kwargs:
                       browser: 当没有传入page时，可以选择浏览器
                       locale: dict 国际化
                       bring_to_front: bool 是否将浏览器窗口置顶
+                      viewport: {'width': 1366, 'height': 768}  浏览器窗口大小
         """
         self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
         self.username = username
         self.password = password
         self.language = language
         self.bring_to_front = kwargs.get('bring_to_front', False)
         self.__browser_type = kwargs.get('browser')
         self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
+        self.viewport = kwargs.get('viewport', {'width': 1366, 'height': 768})
         if self.page is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IG902', 'IG502'):
             self.content_locator = IGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IR302', 'IR305', 'IR615'):
@@ -105,16 +107,15 @@
             browser = self.__playwright.chromium
         self.__browser = browser.launch(headless=False)
         if self.model in self.__http_credentials_model:
             http_credentials = {'username': self.username, 'password': self.password}
         else:
             http_credentials = None
         self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials,
-                                                    viewport={'width': 1366, 'height': 768},
-                                                    permissions=['clipboard-read'])
+                                                    viewport=self.viewport, permissions=['clipboard-read'])
         logging.info('Start your journey browser is chrome')
         self.page = self.__context.new_page()
         self.page.on("dialog", dialog_)
 
     @allure.step("用户登录")
     def login(self, username=None, password=None, status='success') -> None:
         """
@@ -1046,14 +1047,16 @@
                     elif wait_for_.get('type') == 'visible':
                         wait_for_.get('locator').wait_for(state='visible', timeout=wait_for_.get('timeout'))
                     elif wait_for_.get('type') == 'hidden':
                         wait_for_.get('locator').wait_for(state='hidden', timeout=wait_for_.get('timeout'))
                     elif wait_for_.get('type') == 'tip_messages':
                         timeout = wait_for_.get('timeout') if wait_for_.get('timeout') else 30
                         self.tip_messages(wait_for_.get('messages'), timeout)
+            if param_locator.get('mouse_move'):
+                self.page.mouse.move(param_locator.get('mouse_move')[0], param_locator.get('mouse_move')[1])
 
         if action_dict:
             for option in locators:
                 assert type(option) in (tuple, list) and len(option) == 2, "type of option is incorrect"
                 if option[0] in [key for key, value in action_dict.items() if value is not None]:
                     if isinstance(option[1], dict):
                         if option[1].get("relation") and option[1].get("relation") not in relations:
```

### Comparing `inhandtest-0.0.62/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.63/inhandtest/base_page/table_tr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 # @Time    : 2023/3/21 10:13:10
 # @Author  : Pane Li
 # @File    : table_tr.py
 """
 table_tr
 
 """
-import re
 from typing import List
-from inhandtest.tools import replace_str
+from inhandtest.tools import replace_str, loop_inspector
 from playwright.sync_api import Locator, TimeoutError
 import logging
 
 
 class Table:
 
     def __init__(self, columns: list, table_locator: Locator, unique_columns: list, locale: dict = None, log_desc=None):
@@ -25,30 +24,30 @@
                         在表格只有查找功能是时，只要列属性不定义为check 都可以
         :param table_locator: table_locator 定位
         :param unique_columns:  list, 确认唯一的列资源名称, eg: ["列名称变量1", "列名称变量2"...]， 当表只有查找功能时，该项为列的所有值。
         :param locale: dict, 国际化文件,
         """
         self.columns = columns  # 列名要与实际的列相对应，不能多也不能少 [("acl_name", 'input'), ('action', 'select')]
         self.table_locator = table_locator
-        self.unique_columns = unique_columns  # 重复列名
+        self.unique_columns = unique_columns  # 唯一的列资源名称
         self.tr = self.table_locator.locator('//tbody').locator('//tr')
         self.locale = locale
         self.log_desc = log_desc
 
     def __filter_td_index(self, contain_check=False, **kwargs):
         self.table_locator.wait_for(state='visible')
         expect_result = []
         for input_key, input_value in kwargs.items():
             if not contain_check:
                 result = list(filter(lambda a: a[0] == input_key and a[1] != 'check' and a[0] in self.unique_columns,
                                      self.columns))  # 排除掉check
             else:
-                result = list(filter(lambda a: a[0] == input_key, self.columns))
+                result = list(filter(lambda a: a[0] == input_key and a[0] in self.unique_columns, self.columns))
             if len(result) == 1:
-                expect_result.append((self.columns.index(result[0]), input_value, result[0][1]))  # 找出td是第几个，也及值
+                expect_result.append((self.columns.index(result[0]), input_value, result[0][1]))  # 找出td是第几个，也及值, 以及类型
         return expect_result
 
     def __edit_add(self, **kwargs):
         for column in self.__filter_td_index(True, **kwargs):
             if column[1] is not None:
                 if column[2] == 'input':
                     self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.clear()
@@ -69,15 +68,14 @@
 
     def exist(self, find_one=True, locale=None, **kwargs) -> int or None or List[int]:
         """ 传入的资源是否存在, 对于check 项是不计入重复选项的，因为勾选其实只是开启功能而已
 
 
         :param find_one: 是否只查询一个，当查询一个时返回的是int值，索引从0 开始， 当没查询到时返回的是None
                          当查询多个时，如果没有找到返回的是[], 如果找到了是列表包含了多个索引值
-
         :param locale: dict 国际化， 默认为类初始化的locale, 也可以单独传入
         :param kwargs: 支持传入表达式， 如 acl_name='${value} == '2''
         :return: int or list or None
         """
         search_tr = []
         one_tr = None
         expect_result = self.__filter_td_index(**kwargs)
@@ -105,14 +103,44 @@
                             one_tr = tr_nth
                             break
         if find_one:
             return one_tr
         else:
             return search_tr
 
+    @loop_inspector('table tr')
+    def assert_exist(self, timeout=90, interval=5, locale=None, **kwargs):
+        """ 传入的资源是否存在, 对于check 项是不计入重复选项的，因为勾选其实只是开启功能而已
+
+        :param locale: dict 国际化， 默认为类初始化的locale, 也可以单独传入
+        :param timeout: 超时时间
+        :param interval: 间隔时间
+        :param kwargs: 支持传入表达式， 如 acl_name='${value} == '2''
+               多增加参数：exist_number: 期望的数量， 默认为1, 可以是0 表示查找不到该项
+        :return:
+        """
+        exist_number = kwargs.get('exist_number', 1)
+        if exist_number == 0:
+            if self.exist(find_one=True, locale=locale, **kwargs) is None:
+                return True
+            else:
+                return False
+        elif exist_number == 1:
+            if self.exist(find_one=True, locale=locale, **kwargs) is not None:
+                return True
+            else:
+                return False
+        elif exist_number > 1:
+            if len(self.exist(find_one=False, locale=locale, **kwargs)) == exist_number:
+                return True
+            else:
+                return False
+        else:
+            return True
+
     def add(self, **kwargs) -> None:
         """ add 前是不查找是否存在的，直接加
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         self.__edit_add(**kwargs)
         for i in range(0, self.tr.get_by_role('button').count()):
@@ -270,51 +298,52 @@
         :param value: str 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化 ex: 192.168.2.1255.255.255.0
         :param locale: dict 国际化， 默认为类初始化的locale, 也可以单独传入
         :return: True|False
         """
         locale = self.locale if locale is None else locale
         if value:
             value = replace_str(str(value), locale)  # 期望的值
-            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
             if exist_tr.count() > 0:
                 return True
         return False
 
     def add(self, agg_in, **kwargs, ) -> None:
         """ add 前是不查找是否存在的，直接加
 
         :param agg_in: function, 导致该方法不能单独使用
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
             kwargs['save'] = True
+        cancel = kwargs.pop('cancel') if kwargs.get('cancel') is not None else False
         try:
             add_button = list(filter(lambda x: x[0] == 'add', self.columns))[0][1].get('locator')
         except Exception:
             add_button = self.table_locator.locator('//button').first
         if kwargs.get('is_exists'):
             is_exists = kwargs.pop('is_exists')
             if not self.exist(is_exists, self.locale):
                 add_button.click()
-                if not kwargs.get('cancel'):
+                if not cancel:
                     agg_in(self.columns, kwargs)
                     logging.debug(f'table resource {kwargs} add success')
                 else:
                     try:
                         agg_in(self.columns, kwargs)
                     except Exception:
                         raise
                     finally:
                         agg_in(self.columns, {'cancel': True})
             else:
                 logging.debug(f'table resource {kwargs} exist')
         else:
             add_button.click()
-            if not kwargs.get('cancel'):
+            if not cancel:
                 agg_in(self.columns, kwargs)
                 logging.debug(f'table resource {kwargs} add success')
             else:
                 try:
                     agg_in(self.columns, kwargs)
                 except Exception:
                     raise
@@ -326,23 +355,24 @@
 
         :param agg_in: function, 导致该方法不能单独使用
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         old_value = replace_str(old_value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(old_value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=old_value)
         if exist_tr.count() > 0:
             if exist_tr.first.locator('//i[@class="anticon anticon-form"]').count() == 1:
                 exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
             else:
                 exist_tr.first.locator('//i[@class="anticon anticon-edit"]').click()
             if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
-            if not kwargs.get('cancel'):
+            cancel = kwargs.pop('cancel') if kwargs.get('cancel') is not None else False
+            if not cancel:
                 agg_in(self.columns, kwargs)
                 logging.debug(f'table resource {kwargs} edit success')
             else:
                 try:
                     agg_in(self.columns, kwargs)
                 except Exception:
                     raise
@@ -353,58 +383,58 @@
 
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         exist_tr_number = exist_tr.count()
         for i in range(0, exist_tr_number):
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
-            while exist_tr.count() + i + 1 != exist_tr_number:   # 等待删除完成,
+            while exist_tr.count() + i + 1 != exist_tr_number:  # 等待删除完成,
                 self.table_locator.page.wait_for_timeout(500)
         logging.debug(f'table resource {value} all delete')
 
     def associate_delete(self, value: str) -> None:
         """
         :param value str, 关联删除按钮，如VPN 中l2tp client表格中的删除按钮
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         while exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-close"]').click()
         logging.debug(f'table resource {value} all delete associate')
 
     def download(self, action, value: str, file_path: str, file_name: str = None):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str,
         :param file_path: str, 下载文件存放路径
         :param file_name: str, 下载文件名
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             action(exist_tr.first.locator('//i[@class="anticon anticon-download"]').first, file_path,
                    file_name=file_name)
         logging.debug(f'table resource {value} download success')
 
     def upload(self, action, value, file_path):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str, 待上传列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :param file_path: str, 上传文件全路径
         :return:
         """
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-upload"]').click()
             action(self.pop_up_locator.locator('.anticon.anticon-upload').nth(0), file_path)
             self.pop_up_locator.locator('.ant-btn.ant-btn-primary').nth(0).click()
         logging.debug(f'table resource {value}  click upload')
 
     def check(self, action, value, check_value):
@@ -414,92 +444,94 @@
         :param check_value: str, 待check值
         :return:
         """
         tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr')
         for i in range(0, tr.count()):
             for x in range(0, tr.nth(i).locator('//td').count()):
                 if tr.nth(i).locator('//td').nth(x).inner_text() == value:
-                    return action(tr.nth(i).locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
+                    return action(tr.nth(i).locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0),
+                                  check_value)
         else:
-            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
             if exist_tr.count() > 0:
-                action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
+                action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0),
+                       check_value)
         logging.debug(f'table resource {value}  {check_value}')
 
     def start(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-play-circle"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all start')
 
     def stop(self, value: str) -> None:
         """
         :param value str, 待停止列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-pause-circle"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all stop')
 
     def restart(self, value: str) -> None:
         """
         :param value str, 待重启列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-undo"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all restart')
 
     def clear_historical_data(self, value: str) -> None:
         """
         :param value str, 待重启列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all restart')
 
     def clear_log(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all clear log')
 
     def connect(self, value: str) -> None:
         """
         :param value str, WLAN 页面connect连接，每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :return:
         """
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=value)
         if exist_tr.count() > 0:
             if exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').is_enabled():
                 exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').click()
                 logging.info(f'table resource {value} connect success')
             else:
                 logging.debug(f'table resource {value} already connected')
 
@@ -507,10 +539,10 @@
         tr_locators = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr').locator(
             '//i[@class="anticon anticon-delete"]')
         exist_tr_number = tr_locators.count()
         for i in range(0, exist_tr_number):
             tr_locators.first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()
-            while tr_locators.count() + i + 1 != exist_tr_number:   # 等待删除完成,
+            while tr_locators.count() + i + 1 != exist_tr_number:  # 等待删除完成,
                 self.table_locator.page.wait_for_timeout(500)
         logging.debug('table resource all delete')
```

### Comparing `inhandtest-0.0.62/inhandtest/exception.py` & `inhandtest-0.0.63/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/file.py` & `inhandtest-0.0.63/inhandtest/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,29 @@
                 os.remove(c_path)
     elif os.path.isfile(file_path):
         os.remove(file_path)
     else:
         logging.debug(f"parameter file_path {file_path} is not exist")
 
 
+def del_file_by_key(file_dir: str, name_contain: str) -> None:
+    """根据文件名包含的关键字删除文件
+
+    :param file_dir: 需要删除的文件目录
+    :param name_contain: 文件名包含的关键字
+    :return:
+    """
+    if os.path.isdir(file_dir):
+        for i in os.listdir(file_dir):
+            c_path = os.path.join(file_dir, i)
+            if name_contain in i:
+                os.remove(c_path)
+                logging.info(f"delete {i} file")
+
+
 def check_file(file_path) -> None:
     """校验文件是否存在
 
     :param file_path: 文件夹路径或者文件路径
     :return:  检查到文件不存在时就抛异常FileNotFoundError
     """
     if not os.path.isfile(file_path) or not os.path.exists(file_path):
@@ -159,9 +174,20 @@
     :return:
     """
     import pandas
     df = pandas.DataFrame(content)
     df.to_csv(file_path, index=False, header=header)
 
 
+def file_content_read(file_path):
+    """
+    读取文件内容，返回列表
+    :param file_path: 文件路径
+    :return: 返回的文件内容，list
+    """
+    with open(file_path, 'r', encoding='utf-8') as f:
+        str_file_content = f.read()
+    return str_file_content.split('\n')
+
+
 if __name__ == '__main__':
     create_file('./test.txt', 'test\n1234123', mode='a')
```

### Comparing `inhandtest-0.0.62/inhandtest/inmodbus.py` & `inhandtest-0.0.63/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inmongodb.py` & `inhandtest-0.0.63/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inmqtt.py` & `inhandtest-0.0.63/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/__init__.py` & `inhandtest-0.0.63/inhandtest/inrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/console.py` & `inhandtest-0.0.63/inhandtest/inrequest/console.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/dm.py` & `inhandtest-0.0.63/inhandtest/inrequest/dm.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/dn.py` & `inhandtest-0.0.63/inhandtest/inrequest/dn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/er_default_config.py` & `inhandtest-0.0.63/inhandtest/inrequest/er_default_config.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/er_device.py` & `inhandtest-0.0.63/inhandtest/inrequest/er_device.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/ics.py` & `inhandtest-0.0.63/inhandtest/inrequest/ics.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/inrequest.py` & `inhandtest-0.0.63/inhandtest/inrequest/inrequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,57 +127,57 @@
         :param params_type: 参数类型，用于post请求，参数值：form|json
         :param header: 请求头 只支持字典
         :param code: 验证返回code
         :param auth: 是否认证， 默认需要的
         :param url: 请求地址，如果不传就是默认组装，传了就是他
         :return:
         """
-        header = dict_merge(self.headers, header) if auth else header
+        headers = dict_merge(self.headers, header) if auth else header
         urllib3.disable_warnings()  # 去除https warnings提示
         method = method.upper()
         params_type = params_type.upper()
         url = self.__url_pre(path) if not url else url
         param = self.remove_none_values(param) if self.__param_remove_none_key and param else param
         body = self.remove_none_values(body) if self.__body_remove_none_key and body else body
         if method == 'GET':
-            res = requests.get(url=url, params=param, headers=header, verify=False)
+            res = requests.get(url=url, params=param, headers=headers, verify=False)
             if file_path:
                 with open(file_path, 'w', encoding='UTF-8') as f:
                     f.write(res.text)
         elif method == 'POST':
             if params_type == 'FORM':
                 if file_path:
                     if self.type_ == 'device':
                         files = {
                             'file': (
                                 os.path.basename(file_path), open(file_path, 'rb'), 'application/octet-stream')}
-                        res = requests.post(url, params=param, files=files, headers=header, verify=False)
+                        res = requests.post(url, params=param, files=files, headers=headers, verify=False)
                     else:
                         with open(file_path, 'rb') as f:
                             file_info = {"file": f}
-                            res = requests.post(url, data=param, files=file_info, headers=header, verify=False)
+                            res = requests.post(url, data=param, files=file_info, headers=headers, verify=False)
                 else:
-                    res = requests.post(url=url, data=param, headers=header, verify=False)
+                    res = requests.post(url=url, data=param, headers=headers, verify=False)
             elif params_type == 'JSON':
-                res = requests.post(url=url, params=param, json=body, headers=header, verify=False)
+                res = requests.post(url=url, params=param, json=body, headers=headers, verify=False)
             else:
-                res = requests.post(url=url, headers=header, verify=False)
+                res = requests.post(url=url, headers=headers, verify=False)
         elif method == 'DELETE':
             if body:
                 if params_type == 'JSON':
-                    res = requests.delete(url, headers=header, json=body, verify=False)
+                    res = requests.delete(url, headers=headers, json=body, verify=False)
                 else:
-                    res = requests.delete(url, headers=header, data=body, verify=False)
+                    res = requests.delete(url, headers=headers, data=body, verify=False)
             else:
-                res = requests.delete(url, params=param, headers=header, verify=False)
+                res = requests.delete(url, params=param, headers=headers, verify=False)
         elif method == 'PUT':
             if params_type == 'JSON':
-                res = requests.put(url, json=body, params=param, headers=header, verify=False)
+                res = requests.put(url, json=body, params=param, headers=headers, verify=False)
             else:
-                res = requests.put(url, data=param, headers=header, verify=False)
+                res = requests.put(url, data=param, headers=headers, verify=False)
         else:
             logging.exception(f"requests method {method} not support")
             raise ParameterValueError(f"requests method {method} not support")
         # logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
         if res.status_code != 401:
             if self.type_ == 'device':
                 if res.status_code == 404:
@@ -191,15 +191,15 @@
             try:
                 logging.debug(f'Requests Response json is {res.json()}')
             except Exception:
                 logging.warning(f'Requests Response json is None')
         else:
             # 当token过期时，统一重新登录后再次调API
             self.__login()
-            res = self.send_request(path, method, param, body, expect, file_path, params_type, header, code)
+            res = self.send_request(path, method, param, body, expect, file_path, params_type, header, code, auth, url)
         if code:
             assert res.status_code == code, res.text
         if expect:
             if isinstance(expect, list):
                 if len(expect) > 0:
                     for i in expect:
                         if isinstance(i, str) or isinstance(i, int):
```

### Comparing `inhandtest-0.0.62/inhandtest/inrequest/nezha.py` & `inhandtest-0.0.63/inhandtest/inrequest/nezha.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,33 +80,37 @@
         :param expect:  {"result":{"connected":518,"disconnected":167,"disabled":154,"exception":54}}
         :param param:  {"org": "5f0f1e9b9d6b4e0001a3e2b0"}
         :return:
         """
         self.api.send_request('/api/v1/uplinks/status', method='get', expect=expect, param=param)
 
     @allure.step("概览上行链路列表验证")
-    def assert_uplinks_list(self, sn: str, interfaces: list, param=None):
+    def assert_uplinks_list(self, sn: str, interfaces: list, param=None, expect=None):
         """
 
         :param sn: 当sn为空时就对整体列表做验证
         :param interfaces:
         :param param: 查询参数
+        :param expect: 期望值
         :return:
         """
+
+        param = dict_merge({'limit': 100, 'page': 0}, param) if param else {'limit': 100, 'page': 0}
         if interfaces and sn:
-            param = dict_merge({'limit': 100, 'page': 0}, param) if param else {'limit': 100, 'page': 0}
             result = self.api.send_request('/api/v1/uplinks', 'get', param).json().get('result')
             _id = self.__device.info(sn).get('_id')
             for interface in interfaces:
                 for device in result:
                     if device.get('deviceId') == _id and device.get('name') == interface.get('name'):
                         dict_in(device, interface)
                         break
                 else:
                     raise ResourceNotFoundError(f'the {sn} not found in uplinks list')
+        else:
+            self.api.send_request('/api/v1/uplinks', 'get', param, expect=expect)
 
 
 class Device(Base):
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__firmware = Firmware(api, email, host)
 
@@ -304,15 +308,15 @@
         firmware_id = self.__firmware.info(product, version).get('_id')
         payload = {"jobs": [{"targets": _id, "firmware": firmware_id}], "targetType": "device"}
         if schedule:
             payload["scheduledAt"] = get_time_stamp(delta=schedule, delta_type='m')
         try:
             return self.api.send_request('/api/v1/firmwares/batch/jobs', 'post', body=payload).json().get('result')[0][
                 '_id']
-        except IndexError:
+        except (IndexError, KeyError):
             logging.exception(f'firmware upgrade failed')
             raise UpgradeFailedError(f'firmware upgrade failed')
 
     @allure.step("设备取消最近固件升级任务")
     def cancel_latest_task(self, sn: str):
         detail = self.info(sn, 'detail')
         if detail.get('firmwareUpgradeStatus'):
@@ -331,28 +335,38 @@
         """
         sn = [sn] if isinstance(sn, str) else sn
         ids = [self.info(sn_).get('_id') for sn_ in sn]
         body = {"deviceIds": ids, "method": method}
         self.api.send_request('/api/v1/devices/bulk-invoke-methods', 'post', body=body, expect={'result': 'ok'})
 
     @allure.step("在线下载日志")
-    def download_log_online(self, sn: str, type_='diagnostic'):
+    def download_log_online(self, sn: str, type_='diagnostic', expect_file=None, expect_content=None):
         """
 
         :param sn:
         :param type_:diagnostic|syslog
+        :param expect_file: 期望下载的文件路径
+        :param expect_content: 期望下载的文件内容
         :return:
         """
         _id = self.info(sn).get('_id')
-        if type_ == 'diagnostic':
-            host = 'https://nezha-demo-device-files.s3.cn-northwest-1.amazonaws.com.cn'
-        else:
-            host = 'https://nezha-demo-tmp-files.s3.cn-northwest-1.amazonaws.com.cn'
-        self.api.send_request(f'/api/v1/devices/{_id}/logs/download', 'get', {'type': type_},
-                              expect=f'"downloadUrl":"{host}/uploads/{_id}')
+        result = self.api.send_request(f'/api/v1/devices/{_id}/logs/download', 'get', {'type': type_},
+                                       expect=f'"downloadUrl"').json().get('result')
+        time.sleep(3)
+        lines = self.api.send_request('', 'get', url=result.get('downloadUrl'), auth=False).text
+        lines = lines.replace('\r', '')
+        if expect_file:
+            with open(expect_file, 'r', encoding='utf-8') as f:
+                expect_lines = ''.join(f.readlines())
+            assert lines == expect_lines, f'文件下载失败'
+        if expect_content:
+            lines = lines.replace('\n', '')
+            logging.info(f'lines: {lines}')
+            logging.info(f'expect_content: {expect_content}')
+            assert lines == expect_content, f'文件下载失败'
 
     @allure.step("设备蜂窝历史数据")
     def assert_cellular_history(self, sn: str, state, delta_day=-1, data_interval=None):
         """
 
         :param sn:
         :param state:
@@ -510,14 +524,34 @@
                 for device in result:
                     if device.get('name') == interface.get('name'):
                         dict_in(device, interface)
                         break
                 else:
                     raise ResourceNotFoundError(f'the {sn} not found in uplinks list')
 
+    @allure.step("客户端验证")
+    def assert_client(self, sn: str, clients: list):
+        """
+
+        :param sn:
+        :param clients:
+        :return:
+        """
+        if clients:
+            _id = self.info(sn).get('_id')
+            result = self.api.send_request(f'/api/v1/devices/{_id}/clients', 'get', ).json().get('result').get(
+                'clients')
+            for client in clients:
+                for device in result:
+                    if device.get('name') == client.get('name'):
+                        dict_in(device, client)
+                        break
+                else:
+                    raise ResourceNotFoundError(f'the {sn} not found in cient list')
+
     @allure.step("获取设备interface")
     def get_interface(self, sn: str):
         """
 
         :param sn:
         :return:
         """
@@ -626,26 +660,14 @@
             compatibilities = list(function.keys())
             body = {"ids": [_id], "compatibilities": compatibilities, "type": "device"}
             result = self.api.send_request(f'/api/v1/product-compatibilities/bulk-validate', 'post',
                                            body=body).json().get('result')[0]
             contain_ = {key: {"support": value} for key, value in function.items()}
             dict_in(result, {"compatibilities": contain_})
 
-    @allure.step("设备上行链路历史校验")
-    def assert_uplink_history(self, sn: str, expect: dict, param=None):
-        """
-
-        :param sn:
-        :param expect: {'uplinkHistory': [{'timestamp': 1621574400000, 'uplink': 0.0}]}
-        :param param: {'from': 1621574400000, 'to': 1621574400000, 'interval': 86400000}
-        :return:
-        """
-        _id = self.info(sn).get('_id')
-        self.api.send_request(f'/api/v1/devices/{_id}/uplinks/perf-trend', 'get', param, expect=expect)
-
 
 class Config(Base):
 
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__device = Device(api, email, host)
         self.__group = Group(api, email, host)
```

### Comparing `inhandtest-0.0.62/inhandtest/inserial.py` & `inhandtest-0.0.63/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/insocket.py` & `inhandtest-0.0.63/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/inssh.py` & `inhandtest-0.0.63/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/ip.py` & `inhandtest-0.0.63/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/log.py` & `inhandtest-0.0.63/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/mail.py` & `inhandtest-0.0.63/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,35 +528,33 @@
                 '.ant-btn.ant-btn-primary.ant-btn-sm').first, 'type': 'button'}),
         ]
 
     @property
     def controller_template_locator(self) -> list:
         return [
             ('import', {'locator': self.page.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
-            ('import_confirm', {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary'), 'type': 'button'}),
             ('export', {'locator': self.page.locator('.anticon.anticon-download').first, 'type': 'download_file'}),
             ('check_all', {'locator': self.page.locator('.ant-checkbox-input').first, 'type': 'check'}),
             ('table',
              {'locator': {
                  'locator': self.page.locator('.ant-table-content').nth(0),
                  'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
                      '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                  "columns": [
                      ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                      ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                      ('save', {'locator': self.pop_up.locator(
-                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
-                         'wait_for': {'type': 'tip_messages', 'messages': self.locale.submit_success}}),
+                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                      ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
                  ]},
                  'type': 'table_tr', }),
-            ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first,
-                             'type': 'button'}),
+            ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first, 'type': 'button',
+                             'mouse_move': (-100, 0)}),  # 鼠标移动开，防止遮挡
             ('delete_bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
                 '.ant-btn.ant-btn-primary.ant-btn-sm'), 'type': 'button'}),
         ]
 
     @property
     def alarm_rules_locator(self) -> list:
         return [
```

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,16 +488,15 @@
                     [('check_all', value,)]
                         value: bool  勾选或取消勾选全部分组 True | False
                     [('delete_bulk', name, value1)]  # 批量删除分组
                         name: str or list 一个或多个分组名称
                         value1: {'tip_messages': 'submit_success'} or None 提示信息
               controller_template: [('action_type', value, value1)]
                     [('import', value, value1)]
-                        value: str  导入文件路径
-                        value1: 导入时的确认，默认为True， 也可以校验导入后的提示
+                        value: str  or dict  导入文件路径
                     [('export', value,)]
                         value: str  or dict   # 导出分组
                         str: 导出文件夹
                         dict: {"file_path": "./", "file_name": None}
                     [('edit', 'old_template_name', kwargs)]
                         kwargs:
                             name: 名称
@@ -549,17 +548,15 @@
         if kwargs.get('controller_template') and isinstance(kwargs.get('controller_template'), list):
             self.access_menu('edge_computing.device_supervisor.measure_monitor.controller_template')
             for template in kwargs.get('controller_template'):
                 if template[0] in ('edit', 'check', 'delete'):
                     self.agg_in(self.edge_locators.controller_template_locator, {'table': [template]})
                 else:
                     if template[0] == 'import':
-                        import_confirm = True if template[2] is None else template[2]
-                        self.agg_in(self.edge_locators.controller_template_locator,
-                                    {'import': template[1], 'import_confirm': import_confirm})
+                        self.agg_in(self.edge_locators.controller_template_locator, {'import': template[1]})
                     elif template[0] == 'delete_bulk':
                         try:
                             delete_bulk_confirm = template[2]
                         except IndexError:
                             delete_bulk_confirm = True
                         self.agg_in(self.edge_locators.controller_template_locator, {'check_all': False})
                         check_group = [template[1]] if isinstance(template[1], str) else template[1]
@@ -1161,15 +1158,15 @@
         if transform_type == 1:
             if reverse:
                 operator_value = ((input_value - lower_limit_of_proportion) * (data_high_limit - data_lower_limit) / \
                                   (high_limit_of_proportion - lower_limit_of_proportion)) + data_lower_limit
             else:
                 operation_value = (Decimal(high_limit_of_proportion) - Decimal(lower_limit_of_proportion)) / \
                                   (Decimal(data_high_limit) - Decimal(data_lower_limit)) * (
-                                              Decimal(input_value) - Decimal(data_lower_limit)) + \
+                                          Decimal(input_value) - Decimal(data_lower_limit)) + \
                                   Decimal(lower_limit_of_proportion)
         elif transform_type == 2:
             if reverse:
                 operator_value = (input_value - offset) / magnification
             else:
                 operation_value = Decimal(input_value) * Decimal(magnification) + Decimal(offset)
         elif transform_type == 3:
```

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/ingateway.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,42 +16,47 @@
 import dynaconf
 import os
 
 
 class InGateway(BasePage):
 
     def __init__(self, host: str, super_user: str, super_password: str, page: Page = None, model='IG902',
-                 language='en', protocol='https', port=443, username='adm', password='123456', telnet=True,
-                 locale_yaml_path=None, bring_to_front=False):
+                 language='en', protocol='https', port=443, username='adm', password='123456',
+                 bring_to_front=False, **kwargs):
         """
 
         :param host:   设备主机地址
         :param super_user:  超级用户
         :param super_password: 超级用户密码
         :param page:  playwright page
         :param model:  设备型号  IG902 IG502
         :param language: 语言 en cn
         :param protocol: 协议  http https
         :param port:    端口
         :param username: 用户名
         :param password: 密码
-        :param telnet: 是否开启telnet
-        :param locale_yaml_path: 语言文件 默认为None
-        :param bring_to_front: 是否将浏览器窗口置顶
+        :param kwargs:
+            telnet: 是否开启telnet, 默认为True 开启
+            locale_yaml_path: 本地国际化文件路径
+            bring_to_front: 是否将浏览器窗口置顶  默认为False 不置顶
+            viewport: {'width': 1366, 'height': 768}  窗口大小
         """
-
+        telnet = kwargs.get('telnet', True)
+        locale_yaml_path = kwargs.get('locale_yaml_path', None)
+        bring_to_front = kwargs.get('bring_to_front', False)
+        viewport = kwargs.get('viewport', {'width': 1366, 'height': 768})
         if locale_yaml_path:
             in_setting = dynaconf.Dynaconf(
                 settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml'), locale_yaml_path],
                 merge_enabled=True)
         else:
             in_setting = dynaconf.Dynaconf(
                 settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml')])
         super().__init__(host, username, password, protocol, port, model, language, page, locale=in_setting,
-                         bring_to_front=bring_to_front)
+                         bring_to_front=bring_to_front, viewport=viewport)
         if telnet:
             self.telnet = Telnet(model, host, super_user, super_password)
         else:
             self.telnet = None
         if self.language == 'en':
             self.telnet.send_cli(command='language English', type_='user')
         else:
```

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.63/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.63/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/pytest_email.html` & `inhandtest-0.0.63/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/telnet.py` & `inhandtest-0.0.63/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest/tools.py` & `inhandtest-0.0.63/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.63/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.62
+Version: 0.0.63
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.62/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.63/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.62/setup.py` & `inhandtest-0.0.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.62',
+    version='0.0.63',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

