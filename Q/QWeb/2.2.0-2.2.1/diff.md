# Comparing `tmp/QWeb-2.2.0.tar.gz` & `tmp/QWeb-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QWeb-2.2.0.tar", last modified: Wed Jun 14 07:39:39 2023, max compression
+gzip compressed data, was "QWeb-2.2.1.tar", last modified: Wed Aug  2 10:11:55 2023, max compression
```

## Comparing `QWeb-2.2.0.tar` & `QWeb-2.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.150060 QWeb-2.2.0/
--rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10191 2023-06-14 07:39:39.151056 QWeb-2.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.157669 QWeb-2.2.0/QWeb/
--rw-rw-rw-   0        0        0     6450 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/__init__.py
--rw-rw-rw-   0        0        0     2267 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/__main__.py
--rw-rw-rw-   0        0        0      519 2023-06-14 07:39:39.159663 QWeb-2.2.0/QWeb/_version.py
--rw-rw-rw-   0        0        0      905 2022-10-17 07:43:06.000000 QWeb-2.2.0/QWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.065395 QWeb-2.2.0/QWeb/internal/
--rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-2.2.0/QWeb/internal/__init__.py
--rw-rw-rw-   0        0        0    21882 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/actions.py
--rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/ajax.py
--rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/alert.py
--rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/blocks.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.088005 QWeb-2.2.0/QWeb/internal/browser/
--rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-2.2.0/QWeb/internal/browser/__init__.py
--rw-rw-rw-   0        0        0     1446 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/android.py
--rw-rw-rw-   0        0        0     2626 2022-06-23 10:57:52.000000 QWeb-2.2.0/QWeb/internal/browser/bs_desktop.py
--rw-rw-rw-   0        0        0     1716 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/bs_mobile.py
--rw-rw-rw-   0        0        0     5889 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/chrome.py
--rw-rw-rw-   0        0        0     4277 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/edge.py
--rw-rw-rw-   0        0        0     5140 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/browser/firefox.py
--rw-rw-rw-   0        0        0     1888 2022-11-23 07:04:05.000000 QWeb-2.2.0/QWeb/internal/browser/ie.py
--rw-rw-rw-   0        0        0     1077 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/browser/safari.py
--rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/checkbox.py
--rw-rw-rw-   0        0        0     4118 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/config.py
--rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/config_defaults.py
--rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/cookies.py
--rw-rw-rw-   0        0        0     9341 2023-06-12 09:33:39.000000 QWeb-2.2.0/QWeb/internal/decorators.py
--rw-rw-rw-   0        0        0     5294 2022-12-02 06:15:00.000000 QWeb-2.2.0/QWeb/internal/download.py
--rw-rw-rw-   0        0        0     3241 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/dragdrop.py
--rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-2.2.0/QWeb/internal/dropdown.py
--rw-rw-rw-   0        0        0    28249 2022-12-16 14:12:34.000000 QWeb-2.2.0/QWeb/internal/element.py
--rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/exceptions.py
--rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-2.2.0/QWeb/internal/file.py
--rw-rw-rw-   0        0        0    11767 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/frame.py
--rw-rw-rw-   0        0        0     1960 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/frame_checker.py
--rw-rw-rw-   0        0        0    20231 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/icon.py
--rw-rw-rw-   0        0        0    10703 2022-12-12 14:30:56.000000 QWeb-2.2.0/QWeb/internal/input_.py
--rw-rw-rw-   0        0        0     7244 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/internal/input_handler.py
--rw-rw-rw-   0        0        0    21040 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/internal/javascript.py
--rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/lists.py
--rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/meas.py
--rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-2.2.0/QWeb/internal/platform.py
--rw-rw-rw-   0        0        0    13379 2023-06-06 09:19:52.000000 QWeb-2.2.0/QWeb/internal/screenshot.py
--rw-rw-rw-   0        0        0     6850 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/search_strategy.py
--rw-rw-rw-   0        0        0     5531 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/secrets.py
--rw-rw-rw-   0        0        0    15645 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/internal/table.py
--rw-rw-rw-   0        0        0    16851 2023-03-16 07:45:30.000000 QWeb-2.2.0/QWeb/internal/text.py
--rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/user.py
--rw-rw-rw-   0        0        0    12833 2023-03-08 07:11:26.000000 QWeb-2.2.0/QWeb/internal/util.py
--rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/window.py
--rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/internal/xhr.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:39.148055 QWeb-2.2.0/QWeb/keywords/
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.0/QWeb/keywords/__init__.py
--rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-2.2.0/QWeb/keywords/ajax.py
--rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/alert.py
--rw-rw-rw-   0        0        0     5778 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/blocks.py
--rw-rw-rw-   0        0        0    18536 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/keywords/browser.py
--rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/checkbox.py
--rw-rw-rw-   0        0        0    36464 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/keywords/config.py
--rw-rw-rw-   0        0        0     2846 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/cookies.py
--rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/debug.py
--rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/download.py
--rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/dragdrop.py
--rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/dropdown.py
--rw-rw-rw-   0        0        0    27613 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/element.py
--rw-rw-rw-   0        0        0    12453 2023-02-03 08:50:04.000000 QWeb-2.2.0/QWeb/keywords/file.py
--rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/frame.py
--rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-2.2.0/QWeb/keywords/icon.py
--rw-rw-rw-   0        0        0    38042 2023-06-12 09:33:39.000000 QWeb-2.2.0/QWeb/keywords/input_.py
--rw-rw-rw-   0        0        0     1908 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/javascript.py
--rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-2.2.0/QWeb/keywords/lists.py
--rw-rw-rw-   0        0        0     2967 2022-06-23 10:57:52.000000 QWeb-2.2.0/QWeb/keywords/screenshot.py
--rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-2.2.0/QWeb/keywords/search_strategy.py
--rw-rw-rw-   0        0        0    11958 2022-11-22 10:56:24.000000 QWeb-2.2.0/QWeb/keywords/table.py
--rw-rw-rw-   0        0        0    66393 2022-09-07 11:01:14.000000 QWeb-2.2.0/QWeb/keywords/text.py
--rw-rw-rw-   0        0        0    17540 2023-06-07 09:41:10.000000 QWeb-2.2.0/QWeb/keywords/window.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:39:38.965558 QWeb-2.2.0/QWeb.egg-info/
--rw-rw-rw-   0        0        0    10191 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2039 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-2.2.0/QWeb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      418 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-14 07:39:38.000000 QWeb-2.2.0/QWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9400 2023-03-08 08:01:54.000000 QWeb-2.2.0/README.md
--rw-rw-rw-   0        0        0     1208 2023-06-14 07:39:39.156056 QWeb-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-06-14 07:12:14.000000 QWeb-2.2.0/setup.py
--rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-2.2.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.443058 QWeb-2.2.1/
+-rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10191 2023-08-02 10:11:55.444160 QWeb-2.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.477354 QWeb-2.2.1/QWeb/
+-rw-rw-rw-   0        0        0     6450 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/__init__.py
+-rw-rw-rw-   0        0        0     2267 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/__main__.py
+-rw-rw-rw-   0        0        0      519 2023-08-02 10:11:55.483464 QWeb-2.2.1/QWeb/_version.py
+-rw-rw-rw-   0        0        0      905 2022-10-17 07:43:06.000000 QWeb-2.2.1/QWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.325620 QWeb-2.2.1/QWeb/internal/
+-rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-2.2.1/QWeb/internal/__init__.py
+-rw-rw-rw-   0        0        0    21882 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/actions.py
+-rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/ajax.py
+-rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/alert.py
+-rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/blocks.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.360303 QWeb-2.2.1/QWeb/internal/browser/
+-rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-2.2.1/QWeb/internal/browser/__init__.py
+-rw-rw-rw-   0        0        0     1446 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/browser/android.py
+-rw-rw-rw-   0        0        0     2626 2022-06-23 10:57:52.000000 QWeb-2.2.1/QWeb/internal/browser/bs_desktop.py
+-rw-rw-rw-   0        0        0     1716 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/browser/bs_mobile.py
+-rw-rw-rw-   0        0        0     5889 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/internal/browser/chrome.py
+-rw-rw-rw-   0        0        0     4277 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/internal/browser/edge.py
+-rw-rw-rw-   0        0        0     5140 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/internal/browser/firefox.py
+-rw-rw-rw-   0        0        0     1888 2022-11-23 07:04:05.000000 QWeb-2.2.1/QWeb/internal/browser/ie.py
+-rw-rw-rw-   0        0        0     1077 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/browser/safari.py
+-rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/checkbox.py
+-rw-rw-rw-   0        0        0     4118 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/config.py
+-rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/config_defaults.py
+-rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/cookies.py
+-rw-rw-rw-   0        0        0     9341 2023-06-12 09:33:39.000000 QWeb-2.2.1/QWeb/internal/decorators.py
+-rw-rw-rw-   0        0        0     5294 2022-12-02 06:15:00.000000 QWeb-2.2.1/QWeb/internal/download.py
+-rw-rw-rw-   0        0        0     3241 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/dragdrop.py
+-rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-2.2.1/QWeb/internal/dropdown.py
+-rw-rw-rw-   0        0        0    28249 2023-07-31 11:43:47.000000 QWeb-2.2.1/QWeb/internal/element.py
+-rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/exceptions.py
+-rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-2.2.1/QWeb/internal/file.py
+-rw-rw-rw-   0        0        0    11767 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/frame.py
+-rw-rw-rw-   0        0        0     1960 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/internal/frame_checker.py
+-rw-rw-rw-   0        0        0    20231 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/icon.py
+-rw-rw-rw-   0        0        0    11050 2023-08-02 09:59:23.000000 QWeb-2.2.1/QWeb/internal/input_.py
+-rw-rw-rw-   0        0        0     7244 2023-03-23 15:17:25.000000 QWeb-2.2.1/QWeb/internal/input_handler.py
+-rw-rw-rw-   0        0        0    21104 2023-08-01 11:39:25.000000 QWeb-2.2.1/QWeb/internal/javascript.py
+-rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/lists.py
+-rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/meas.py
+-rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-2.2.1/QWeb/internal/platform.py
+-rw-rw-rw-   0        0        0    13379 2023-06-06 09:19:52.000000 QWeb-2.2.1/QWeb/internal/screenshot.py
+-rw-rw-rw-   0        0        0     6850 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/internal/search_strategy.py
+-rw-rw-rw-   0        0        0     5531 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/internal/secrets.py
+-rw-rw-rw-   0        0        0    15645 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/internal/table.py
+-rw-rw-rw-   0        0        0    16851 2023-03-16 07:45:30.000000 QWeb-2.2.1/QWeb/internal/text.py
+-rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/internal/user.py
+-rw-rw-rw-   0        0        0    12833 2023-03-08 07:11:26.000000 QWeb-2.2.1/QWeb/internal/util.py
+-rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/internal/window.py
+-rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/internal/xhr.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.439866 QWeb-2.2.1/QWeb/keywords/
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-2.2.1/QWeb/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-2.2.1/QWeb/keywords/ajax.py
+-rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/alert.py
+-rw-rw-rw-   0        0        0     5778 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/blocks.py
+-rw-rw-rw-   0        0        0    18536 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/keywords/browser.py
+-rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    36464 2023-03-23 15:17:25.000000 QWeb-2.2.1/QWeb/keywords/config.py
+-rw-rw-rw-   0        0        0     2846 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/keywords/cookies.py
+-rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/debug.py
+-rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/download.py
+-rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/keywords/dragdrop.py
+-rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/dropdown.py
+-rw-rw-rw-   0        0        0    27613 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/keywords/element.py
+-rw-rw-rw-   0        0        0    12453 2023-02-03 08:50:04.000000 QWeb-2.2.1/QWeb/keywords/file.py
+-rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/frame.py
+-rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-2.2.1/QWeb/keywords/icon.py
+-rw-rw-rw-   0        0        0    38042 2023-06-12 09:33:39.000000 QWeb-2.2.1/QWeb/keywords/input_.py
+-rw-rw-rw-   0        0        0     1908 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/javascript.py
+-rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-2.2.1/QWeb/keywords/lists.py
+-rw-rw-rw-   0        0        0     2967 2022-06-23 10:57:52.000000 QWeb-2.2.1/QWeb/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-2.2.1/QWeb/keywords/search_strategy.py
+-rw-rw-rw-   0        0        0    11958 2022-11-22 10:56:24.000000 QWeb-2.2.1/QWeb/keywords/table.py
+-rw-rw-rw-   0        0        0    66393 2022-09-07 11:01:14.000000 QWeb-2.2.1/QWeb/keywords/text.py
+-rw-rw-rw-   0        0        0    17540 2023-06-07 09:41:10.000000 QWeb-2.2.1/QWeb/keywords/window.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:11:55.202547 QWeb-2.2.1/QWeb.egg-info/
+-rw-rw-rw-   0        0        0    10191 2023-08-02 10:11:54.000000 QWeb-2.2.1/QWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2039 2023-08-02 10:11:55.000000 QWeb-2.2.1/QWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:11:54.000000 QWeb-2.2.1/QWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-2.2.1/QWeb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      418 2023-08-02 10:11:54.000000 QWeb-2.2.1/QWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-02 10:11:54.000000 QWeb-2.2.1/QWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9400 2023-03-08 08:01:54.000000 QWeb-2.2.1/README.md
+-rw-rw-rw-   0        0        0     1208 2023-08-02 10:11:55.466841 QWeb-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-06-14 07:12:14.000000 QWeb-2.2.1/setup.py
+-rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-2.2.1/versioneer.py
```

### Comparing `QWeb-2.2.0/LICENSE` & `QWeb-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/PKG-INFO` & `QWeb-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 2.2.0
+Version: 2.2.1
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QWeb-2.2.0/QWeb/__init__.py` & `QWeb-2.2.1/QWeb/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/__main__.py` & `QWeb-2.2.1/QWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/_version.py` & `QWeb-2.2.1/QWeb/_version.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-14T10:37:39+0300",
+ "date": "2023-08-02T13:08:55+0300",
  "dirty": false,
  "error": null,
- "full-revisionid": "be2b1a01f9575fd1d577a7c5c6a6ee8ab227924c",
- "version": "v2.2.0"
+ "full-revisionid": "ba76350928839a179f3a209dfff5489298c9069a",
+ "version": "v2.2.1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `QWeb-2.2.0/QWeb/config.py` & `QWeb-2.2.1/QWeb/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/actions.py` & `QWeb-2.2.1/QWeb/internal/actions.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/ajax.py` & `QWeb-2.2.1/QWeb/internal/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/alert.py` & `QWeb-2.2.1/QWeb/internal/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/blocks.py` & `QWeb-2.2.1/QWeb/internal/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/__init__.py` & `QWeb-2.2.1/QWeb/internal/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/android.py` & `QWeb-2.2.1/QWeb/internal/browser/android.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/bs_desktop.py` & `QWeb-2.2.1/QWeb/internal/browser/bs_desktop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/bs_mobile.py` & `QWeb-2.2.1/QWeb/internal/browser/bs_mobile.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/chrome.py` & `QWeb-2.2.1/QWeb/internal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/edge.py` & `QWeb-2.2.1/QWeb/internal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/firefox.py` & `QWeb-2.2.1/QWeb/internal/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/ie.py` & `QWeb-2.2.1/QWeb/internal/browser/ie.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/browser/safari.py` & `QWeb-2.2.1/QWeb/internal/browser/safari.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/checkbox.py` & `QWeb-2.2.1/QWeb/internal/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/config.py` & `QWeb-2.2.1/QWeb/internal/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/config_defaults.py` & `QWeb-2.2.1/QWeb/internal/config_defaults.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/cookies.py` & `QWeb-2.2.1/QWeb/internal/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/decorators.py` & `QWeb-2.2.1/QWeb/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/download.py` & `QWeb-2.2.1/QWeb/internal/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/dragdrop.py` & `QWeb-2.2.1/QWeb/internal/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/dropdown.py` & `QWeb-2.2.1/QWeb/internal/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/element.py` & `QWeb-2.2.1/QWeb/internal/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/exceptions.py` & `QWeb-2.2.1/QWeb/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/file.py` & `QWeb-2.2.1/QWeb/internal/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/frame.py` & `QWeb-2.2.1/QWeb/internal/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/frame_checker.py` & `QWeb-2.2.1/QWeb/internal/frame_checker.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/icon.py` & `QWeb-2.2.1/QWeb/internal/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/input_.py` & `QWeb-2.2.1/QWeb/internal/input_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,234 +1,237 @@
-# -*- coding: utf-8 -*-
-# --------------------------
-# Copyright © 2014 -            Qentinel Group.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ---------------------------
-from __future__ import annotations
-from typing import Optional, Union
-from selenium.webdriver.remote.webelement import WebElement
-
-from robot.api import logger
-from QWeb.internal.exceptions import QWebElementNotFoundError, \
-    QWebInstanceDoesNotExistError
-from QWeb.internal import element, text, frame, javascript, util
-from QWeb.internal.table import Table
-from QWeb.internal.config_defaults import CONFIG
-
-
-def get_input_element_by_locator(locator: str, anchor: Union[str, int], **kwargs) -> WebElement:
-    """Find input element.
-
-    Parameters
-    ----------
-    locator : str
-        Text that locates the input field. The input field that is closest
-        to the text is selected. Also one can use xpath by adding xpath= prefix
-        and then the xpath. Error is raised if the xpath matches to multiple
-        elements.
-    anchor : str
-        Text near the input field's locator element. If the page contains
-        many places where the locator is then anchor is used to get the
-        one that is closest to it.
-    """
-    if locator.startswith("xpath=") or locator.startswith("//") or locator.startswith("(//"):
-        if locator.startswith("xpath="):
-            xpath = locator.split("=", 1)[1]
-        else:
-            xpath = locator
-        input_element = element.get_unique_element_by_xpath(xpath, index=anchor, **kwargs)
-    else:  # Search using text
-        input_xpath = CONFIG["MatchingInputElement"].format(locator)
-        input_elements = element.get_webelements_in_active_area(input_xpath, **kwargs)
-        if not input_elements:  # Find input element using locator
-            locator_element = text.get_text_using_anchor(locator, str(anchor), **kwargs)
-            input_elements = _get_all_input_elements()
-
-            shadow_dom = CONFIG['ShadowDOM']
-            if shadow_dom:
-                shadow_inputs = element.get_all_inputs_from_shadow_dom()
-                #  remove duplicates (normal search and including shadow search)
-                input_elements = util.remove_duplicates_from_list(shadow_inputs, input_elements)
-
-            input_element = element.get_closest_element(locator_element, input_elements)
-        elif len(input_elements) == 1:
-            input_element = input_elements[0]  # pylint: disable=unsubscriptable-object
-        else:  # Found many
-            input_element = text.get_element_using_anchor(input_elements, anchor, **kwargs)
-    return input_element
-
-
-def _get_all_input_elements() -> list[WebElement]:
-    input_elements = element.get_webelements_in_active_area(CONFIG["AllInputElements"],
-                                                            stay_in_current_frame=True)
-    return input_elements
-
-
-def get_input_elements_from_all_documents(
-        locator: str,
-        anchor: str,
-        timeout: Union[int, float, str],  # pylint: disable=unused-argument
-        index: Union[int, str] = 1,
-        enable_check: bool = False,
-        **kwargs) -> WebElement:
-    """Function for finding input elements.
-    Parameters
-    ----------
-    locator : str
-       Label text or attribute that points to the checkbox.
-    anchor : str
-       in case there is duplicates.
-    timeout : str
-       How long we are finding before fail.
-       Default = Search Strategy global default = 10 sec)
-    index : int
-       If table cell contains more than one input elements or if there is some kind of
-       nested structure inside of given input index may needed. Default = 1 (first)
-    enable_check : bool
-        When CSS Selectors are used, we are not return disabled input element
-        always by default. Element is needed with verify input status kw
-        so if enable_check= True, disabled input_element is returned
-    kwargs:
-        limit_traverse : bool
-            If set to false. We are heading up to fifth parent element if needed when
-            finding relative input element for some label text.
-    Returns
-    -------
-    WebElement
-    """
-    input_element: Optional[WebElement]
-    index = int(index) - 1
-    css = 'input:not([type="hidden"]):not([type="submit"]):not([type="button"])' \
-          ':not([type="reset"]):not([type="checkbox"]):not([type="radio"])' \
-          ':not([aria-hidden="true"]),' \
-          'textarea:not([type="hidden"]),[contenteditable="true"]'
-    kwargs['css'] = kwargs.get('css', css)
-    if Table.is_table_coordinates(locator):
-        table = Table.ACTIVE_TABLE.update_table()
-        if table is None:
-            raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
-        locator_element = table.get_table_cell(locator, anchor)
-        input_elements = element.get_element_from_childnodes(locator_element,
-                                                             kwargs['css'],
-                                                             dom_traversing=False)
-        if input_elements:
-            return input_elements[int(index)]
-        raise QWebElementNotFoundError('No matching table input found')
-    css_selector = CONFIG["CssSelectors"]
-    if not css_selector or locator.startswith('xpath=') or locator.startswith('//'):
-        input_element = get_input_element_by_locator(locator, index, **kwargs)
-    else:
-        logger.debug('Uses CSS-selectors to locate element')
-        input_element = get_input_element_by_css_selector(locator, anchor, int(index), enable_check,
-                                                          **kwargs)
-        if not input_element:
-            input_element = get_input_element_by_locator(locator, index, **kwargs)
-    if input_element:
-        if CONFIG['SearchMode']:
-            element.draw_borders(input_element)
-        return input_element
-    raise QWebElementNotFoundError('No matching input elements found')
-
-
-def get_input_element_by_css_selector(locator: str,
-                                      anchor: str,
-                                      index: int = 0,
-                                      enable_check: bool = False,
-                                      **kwargs) -> Optional[WebElement]:
-    """Get input element using css selectors.
-       Parameters
-       ----------
-       locator : str
-           Label text or attribute that points to the input.
-           Looking for placeholder and commonly used tooltip-attributes first.
-           If locator is label text, finds input element by it's for attribute.
-           if for attribute is not available, then finds element by doing some
-           DOM traversing.
-       anchor : str
-           Text near the locator element or index. If placeholder or another
-           direct attribute (title, tooltip, value) exists then anchor
-           has to be index. Text is aloud when searching by label or some other
-           text which is near to input element.
-       index: int
-            If multiple input elements is nested or in same table cell, index is needed.
-       enable_check: bool
-            If enable_check is set to true returns first match even if disabled one.
-       Returns
-       -------
-       WebElement
-       """
-    input_element: Union[Optional[WebElement], list[WebElement]]
-    partial_matches: list[WebElement] = []
-    upload = kwargs.get('upload')
-    if upload:
-        try:
-            index = int(locator) - 1
-            kwargs['any_element'] = True
-            input_elements = element.get_elements_by_attributes(**kwargs)
-            if input_elements:
-                return input_elements[index]
-        except ValueError:
-            logger.debug('locator was text')
-    if 'qweb_old' not in kwargs:
-        full_matches, partial_matches = get_input_elements_by_css(locator, **kwargs)
-
-        if full_matches:
-            full_matches = text.filter_by_modal_ancestor(full_matches)
-            input_element = element.get_visible_elements_from_elements(full_matches, **kwargs)
-            if input_element and str(anchor) == '1':
-                input_element = input_element[index]
-                return input_element
-            if input_element:
-                input_element = text.get_element_using_anchor(input_element, anchor, **kwargs)
-                return input_element
-    try:
-        locator_element = text.get_text_using_anchor(locator, anchor, **kwargs)
-        input_elements = list(
-            dict.fromkeys(
-                element.get_element_from_childnodes(locator_element, **kwargs) + partial_matches))
-    except QWebElementNotFoundError:
-        logger.trace('Element not found by visible text. Trying with partial match')
-        input_elements = partial_matches
-    if input_elements:
-        input_elements = text.filter_by_modal_ancestor(input_elements)
-        visibles = element.get_visible_elements_from_elements(input_elements, **kwargs)
-        if visibles:
-            if element.is_enabled(visibles[index]) or enable_check is True:
-                return visibles[index]
-    return None
-
-
-@frame.all_frames
-def get_inputs_including_shadow_dom(locator: str, **kwargs) -> list[WebElement]:
-    web_elements = element.get_visible_elements_from_elements(
-        javascript.get_all_input_elements_from_shadow_dom(), **kwargs)
-
-    matches = javascript.get_by_attributes(web_elements, locator, False)
-    full, partial = matches.get('full', []), matches.get('partial', [])
-    shadow_elements = full + partial
-    if shadow_elements:
-        logger.debug(f'Found {len(shadow_elements)} inputs when extending search to shadow dom')
-    return shadow_elements
-
-
-def get_input_elements_by_css(locator: str, **kwargs):
-    full_matches, partial_matches = element.get_elements_by_css(locator, **kwargs)
-
-    shadow_dom = CONFIG['ShadowDOM']
-    if shadow_dom:
-        shadow_elements = get_inputs_including_shadow_dom(locator, **kwargs)
-        #  remove duplicates (normal search and including shadow search)
-        for el in shadow_elements:
-            if full_matches is not None and el not in list(full_matches):
-                full_matches.append(el)  # type: ignore[union-attr]
-    return full_matches, partial_matches
+# -*- coding: utf-8 -*-
+# --------------------------
+# Copyright © 2014 -            Qentinel Group.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ---------------------------
+from __future__ import annotations
+from typing import Optional, Union
+from selenium.webdriver.remote.webelement import WebElement
+
+from robot.api import logger
+from QWeb.internal.exceptions import QWebElementNotFoundError, \
+    QWebInstanceDoesNotExistError
+from QWeb.internal import element, text, frame, javascript, util
+from QWeb.internal.table import Table
+from QWeb.internal.config_defaults import CONFIG
+
+
+def get_input_element_by_locator(locator: str, anchor: Union[str, int], **kwargs) -> WebElement:
+    """Find input element.
+
+    Parameters
+    ----------
+    locator : str
+        Text that locates the input field. The input field that is closest
+        to the text is selected. Also one can use xpath by adding xpath= prefix
+        and then the xpath. Error is raised if the xpath matches to multiple
+        elements.
+    anchor : str
+        Text near the input field's locator element. If the page contains
+        many places where the locator is then anchor is used to get the
+        one that is closest to it.
+    """
+    if locator.startswith("xpath=") or locator.startswith("//") or locator.startswith("(//"):
+        if locator.startswith("xpath="):
+            xpath = locator.split("=", 1)[1]
+        else:
+            xpath = locator
+        input_element = element.get_unique_element_by_xpath(xpath, index=anchor, **kwargs)
+    else:  # Search using text
+        input_xpath = CONFIG["MatchingInputElement"].format(locator)
+        input_elements = element.get_webelements_in_active_area(input_xpath, **kwargs)
+        if not input_elements:  # Find input element using locator
+            locator_element = text.get_text_using_anchor(locator, str(anchor), **kwargs)
+            input_elements = _get_all_input_elements()
+
+            shadow_dom = CONFIG['ShadowDOM']
+            if shadow_dom:
+                shadow_inputs = element.get_all_inputs_from_shadow_dom()
+                #  remove duplicates (normal search and including shadow search)
+                input_elements = util.remove_duplicates_from_list(shadow_inputs, input_elements)
+
+            input_element = element.get_closest_element(locator_element, input_elements)
+        elif len(input_elements) == 1:
+            input_element = input_elements[0]  # pylint: disable=unsubscriptable-object
+        else:  # Found many
+            input_element = text.get_element_using_anchor(input_elements, anchor, **kwargs)
+    return input_element
+
+
+def _get_all_input_elements() -> list[WebElement]:
+    input_elements = element.get_webelements_in_active_area(CONFIG["AllInputElements"],
+                                                            stay_in_current_frame=True)
+    return input_elements
+
+
+def get_input_elements_from_all_documents(
+        locator: str,
+        anchor: str,
+        timeout: Union[int, float, str],  # pylint: disable=unused-argument
+        index: Union[int, str] = 1,
+        enable_check: bool = False,
+        **kwargs) -> WebElement:
+    """Function for finding input elements.
+    Parameters
+    ----------
+    locator : str
+       Label text or attribute that points to the checkbox.
+    anchor : str
+       in case there is duplicates.
+    timeout : str
+       How long we are finding before fail.
+       Default = Search Strategy global default = 10 sec)
+    index : int
+       If table cell contains more than one input elements or if there is some kind of
+       nested structure inside of given input index may needed. Default = 1 (first)
+    enable_check : bool
+        When CSS Selectors are used, we are not return disabled input element
+        always by default. Element is needed with verify input status kw
+        so if enable_check= True, disabled input_element is returned
+    kwargs:
+        limit_traverse : bool
+            If set to false. We are heading up to fifth parent element if needed when
+            finding relative input element for some label text.
+    Returns
+    -------
+    WebElement
+    """
+    input_element: Optional[WebElement]
+    index = int(index) - 1
+    css = 'input:not([type="hidden"]):not([type="submit"]):not([type="button"])' \
+          ':not([type="reset"]):not([type="checkbox"]):not([type="radio"])' \
+          ':not([aria-hidden="true"]),' \
+          'textarea:not([type="hidden"]),[contenteditable="true"]'
+    kwargs['css'] = kwargs.get('css', css)
+    if Table.is_table_coordinates(locator):
+        table = Table.ACTIVE_TABLE.update_table()
+        if table is None:
+            raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        locator_element = table.get_table_cell(locator, anchor)
+        input_elements = element.get_element_from_childnodes(locator_element,
+                                                             kwargs['css'],
+                                                             dom_traversing=False)
+        if input_elements:
+            return input_elements[int(index)]
+        raise QWebElementNotFoundError('No matching table input found')
+    css_selector = CONFIG["CssSelectors"]
+    if not css_selector or locator.startswith('xpath=') or locator.startswith('//'):
+        input_element = get_input_element_by_locator(locator, index, **kwargs)
+    else:
+        logger.debug('Uses CSS-selectors to locate element')
+        input_element = get_input_element_by_css_selector(locator, anchor, int(index), enable_check,
+                                                          **kwargs)
+        if not input_element:
+            input_element = get_input_element_by_locator(locator, index, **kwargs)
+    if input_element:
+        if CONFIG['SearchMode']:
+            element.draw_borders(input_element)
+        return input_element
+    raise QWebElementNotFoundError('No matching input elements found')
+
+
+def get_input_element_by_css_selector(locator: str,
+                                      anchor: str,
+                                      index: int = 0,
+                                      enable_check: bool = False,
+                                      **kwargs) -> Optional[WebElement]:
+    """Get input element using css selectors.
+       Parameters
+       ----------
+       locator : str
+           Label text or attribute that points to the input.
+           Looking for placeholder and commonly used tooltip-attributes first.
+           If locator is label text, finds input element by it's for attribute.
+           if for attribute is not available, then finds element by doing some
+           DOM traversing.
+       anchor : str
+           Text near the locator element or index. If placeholder or another
+           direct attribute (title, tooltip, value) exists then anchor
+           has to be index. Text is aloud when searching by label or some other
+           text which is near to input element.
+       index: int
+            If multiple input elements is nested or in same table cell, index is needed.
+       enable_check: bool
+            If enable_check is set to true returns first match even if disabled one.
+       Returns
+       -------
+       WebElement
+       """
+    input_element: Union[Optional[WebElement], list[WebElement]]
+    partial_matches: list[WebElement] = []
+    upload = kwargs.get('upload')
+    if upload:
+        try:
+            index = int(locator) - 1
+            kwargs['any_element'] = True
+            input_elements = element.get_elements_by_attributes(**kwargs)
+            if input_elements:
+                return input_elements[index]
+        except ValueError:
+            logger.debug('locator was text')
+    if 'qweb_old' not in kwargs:
+        full_matches, partial_matches = get_input_elements_by_css(locator, **kwargs)
+
+        if full_matches:
+            full_matches = text.filter_by_modal_ancestor(full_matches)
+            input_element = element.get_visible_elements_from_elements(full_matches, **kwargs)
+            if input_element and str(anchor) == '1':
+                input_element = input_element[index]
+                return input_element
+            if input_element:
+                input_element = text.get_element_using_anchor(input_element, anchor, **kwargs)
+                return input_element
+    try:
+        locator_element = text.get_text_using_anchor(locator, anchor, **kwargs)
+        input_elements = list(
+            dict.fromkeys(
+                element.get_element_from_childnodes(locator_element, **kwargs) + partial_matches))
+    except QWebElementNotFoundError:
+        logger.trace('Element not found by visible text. Trying with partial match')
+        input_elements = partial_matches
+    if input_elements:
+        input_elements = text.filter_by_modal_ancestor(input_elements)
+        visibles = element.get_visible_elements_from_elements(input_elements, **kwargs)
+        if visibles:
+            if element.is_enabled(visibles[index]) or enable_check is True:
+                return visibles[index]
+    return None
+
+
+@frame.all_frames
+def get_inputs_including_shadow_dom(locator: str, **kwargs) -> list[WebElement]:
+    web_elements = element.get_visible_elements_from_elements(
+        javascript.get_all_input_elements_from_shadow_dom(), **kwargs)
+
+    matches = javascript.get_by_attributes(web_elements, locator, False)
+    full, partial = matches.get('full', []), matches.get('partial', [])
+    shadow_elements = full + partial
+    if shadow_elements:
+        logger.debug(f'Found {len(shadow_elements)} inputs when extending search to shadow dom')
+    return shadow_elements
+
+
+def get_input_elements_by_css(locator: str, **kwargs):
+    full_matches, partial_matches = element.get_elements_by_css(locator, **kwargs)
+    # return if we already get a full match
+    if full_matches:
+        return full_matches, partial_matches
+
+    shadow_dom = CONFIG['ShadowDOM']
+    if shadow_dom:
+        shadow_elements = get_inputs_including_shadow_dom(locator, **kwargs)
+        #  remove duplicates (normal search and including shadow search)
+        for el in shadow_elements:
+            if full_matches is not None and el not in list(full_matches):
+                full_matches.append(el)  # type: ignore[union-attr]
+    return full_matches, partial_matches
```

### Comparing `QWeb-2.2.0/QWeb/internal/input_handler.py` & `QWeb-2.2.1/QWeb/internal/input_handler.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/javascript.py` & `QWeb-2.2.1/QWeb/internal/javascript.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,17 +159,19 @@
                var attrs = elems[i].attributes;
                if (attrs == null){
                 continue;
                }
                for (var j = 0; j < attrs.length; j++) {
                     if (attrs[j].value.trim() == locator) {
                         full.push(elems[i]);
+                        break;
                     }
                     else if (partial && attrs[j].value.includes(locator)){
                         part.push(elems[i]);
+                        break;
                     }
                }
             }
             matches = {full:full, partial:part};
             return matches;
         }
         return(web_elements(arguments[0], arguments[1], arguments[2]));"""
```

### Comparing `QWeb-2.2.0/QWeb/internal/lists.py` & `QWeb-2.2.1/QWeb/internal/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/meas.py` & `QWeb-2.2.1/QWeb/internal/meas.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/platform.py` & `QWeb-2.2.1/QWeb/internal/platform.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/screenshot.py` & `QWeb-2.2.1/QWeb/internal/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/search_strategy.py` & `QWeb-2.2.1/QWeb/internal/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/secrets.py` & `QWeb-2.2.1/QWeb/internal/secrets.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/table.py` & `QWeb-2.2.1/QWeb/internal/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/text.py` & `QWeb-2.2.1/QWeb/internal/text.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/user.py` & `QWeb-2.2.1/QWeb/internal/user.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/util.py` & `QWeb-2.2.1/QWeb/internal/util.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/window.py` & `QWeb-2.2.1/QWeb/internal/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/internal/xhr.py` & `QWeb-2.2.1/QWeb/internal/xhr.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/ajax.py` & `QWeb-2.2.1/QWeb/keywords/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/alert.py` & `QWeb-2.2.1/QWeb/keywords/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/blocks.py` & `QWeb-2.2.1/QWeb/keywords/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/browser.py` & `QWeb-2.2.1/QWeb/keywords/browser.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/checkbox.py` & `QWeb-2.2.1/QWeb/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/config.py` & `QWeb-2.2.1/QWeb/keywords/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/cookies.py` & `QWeb-2.2.1/QWeb/keywords/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/debug.py` & `QWeb-2.2.1/QWeb/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/download.py` & `QWeb-2.2.1/QWeb/keywords/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/dragdrop.py` & `QWeb-2.2.1/QWeb/keywords/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/dropdown.py` & `QWeb-2.2.1/QWeb/keywords/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/element.py` & `QWeb-2.2.1/QWeb/keywords/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/file.py` & `QWeb-2.2.1/QWeb/keywords/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/frame.py` & `QWeb-2.2.1/QWeb/keywords/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/icon.py` & `QWeb-2.2.1/QWeb/keywords/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/input_.py` & `QWeb-2.2.1/QWeb/keywords/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/javascript.py` & `QWeb-2.2.1/QWeb/keywords/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/lists.py` & `QWeb-2.2.1/QWeb/keywords/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/screenshot.py` & `QWeb-2.2.1/QWeb/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/search_strategy.py` & `QWeb-2.2.1/QWeb/keywords/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/table.py` & `QWeb-2.2.1/QWeb/keywords/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/text.py` & `QWeb-2.2.1/QWeb/keywords/text.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb/keywords/window.py` & `QWeb-2.2.1/QWeb/keywords/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/QWeb.egg-info/PKG-INFO` & `QWeb-2.2.1/QWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 2.2.0
+Version: 2.2.1
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QWeb-2.2.0/QWeb.egg-info/SOURCES.txt` & `QWeb-2.2.1/QWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/README.md` & `QWeb-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/setup.cfg` & `QWeb-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/setup.py` & `QWeb-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `QWeb-2.2.0/versioneer.py` & `QWeb-2.2.1/versioneer.py`

 * *Files identical despite different names*

