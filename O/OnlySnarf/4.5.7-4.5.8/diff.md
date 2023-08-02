# Comparing `tmp/OnlySnarf-4.5.7.tar.gz` & `tmp/OnlySnarf-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.7.tar", last modified: Wed Aug  2 18:51:35 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.8.tar", last modified: Wed Aug  2 19:13:12 2023, max compression
```

## Comparing `OnlySnarf-4.5.7.tar` & `OnlySnarf-4.5.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32087 2023-08-02 18:50:43.000000 OnlySnarf-4.5.7/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.675900 OnlySnarf-4.5.7/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.7/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/__main__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2165 2023-08-02 18:50:50.000000 OnlySnarf-4.5.7/OnlySnarf/api.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.7/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.7/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.7/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.7/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.7/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.7/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2249 2023-08-02 18:37:46.000000 OnlySnarf-4.5.7/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2353 2023-08-02 18:44:36.000000 OnlySnarf-4.5.7/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   166963 2023-08-02 18:48:15.000000 OnlySnarf-4.5.7/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.7/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.7/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.7/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.7/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.7/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12451 2023-08-02 18:39:19.000000 OnlySnarf-4.5.7/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20660 2023-08-02 18:45:04.000000 OnlySnarf-4.5.7/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.7/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.675900 OnlySnarf-4.5.7/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-08-02 18:51:35.000000 OnlySnarf-4.5.7/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.7/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-08-02 18:50:48.000000 OnlySnarf-4.5.7/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 18:51:35.679900 OnlySnarf-4.5.7/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.7/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32089 2023-08-02 19:13:00.000000 OnlySnarf-4.5.8/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.8/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/__main__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2165 2023-08-02 18:50:50.000000 OnlySnarf-4.5.8/OnlySnarf/api.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.8/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.8/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.8/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.8/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.8/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2249 2023-08-02 18:37:46.000000 OnlySnarf-4.5.8/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2353 2023-08-02 18:44:36.000000 OnlySnarf-4.5.8/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   167033 2023-08-02 19:00:43.000000 OnlySnarf-4.5.8/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.8/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.8/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.8/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12451 2023-08-02 18:39:19.000000 OnlySnarf-4.5.8/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20660 2023-08-02 18:45:04.000000 OnlySnarf-4.5.8/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.8/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.8/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-08-02 19:13:05.000000 OnlySnarf-4.5.8/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.7/CHANGELOG.md` & `OnlySnarf-4.5.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -711,15 +711,15 @@
   - updated driver.poll
   - fixed new message tests
   - added flask to package reqs
   - updated install script
   - updated api scripts to route through snarf
   **4.5.3,4,5,6 : 7/30/2023**
   - api debugging
-  **4.5.7 : 8/2/2023**
+  **4.5.7,8 : 8/2/2023**
   - fixed twitter login; added phone number to args&config
 
 ------------------------------------------------------------------------------------
 
 ## TODO
 
 - look into Marshmellow package for class / object cleanup
```

### Comparing `OnlySnarf-4.5.7/LICENSE.txt` & `OnlySnarf-4.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/api.py` & `OnlySnarf-4.5.8/OnlySnarf/api.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.8/OnlySnarf/classes/user.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.8/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.8/OnlySnarf/conf/test-config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.8/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.8/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.8/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.8/OnlySnarf/lib/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1255,15 +1255,15 @@
             bool
                 Whether or not the login check was successful
 
             """
 
             try:
                 Settings.dev_print("waiting for login check...")
-                WebDriverWait(self.browser, 16, poll_frequency=2).until(EC.visibility_of_element_located((By.CLASS_NAME, Element.get_element_by_name("loginCheck").getClass())))
+                WebDriverWait(self.browser, 30, poll_frequency=2).until(EC.visibility_of_element_located((By.CLASS_NAME, Element.get_element_by_name("loginCheck").getClass())))
                 Settings.print("OnlyFans login successful!")
                 Settings.dev_print("login successful - {}".format(which))
                 return True
             except TimeoutException as te:
                 Settings.dev_print(str(te))
                 Settings.print("Login Failure: Timed Out! Please check your credentials.")
                 Settings.print(": If the problem persists, OnlySnarf may require an update.")
@@ -1407,14 +1407,15 @@
                 password_ = self.browser.find_element("name", "session[password]")
                 password_.send_keys(password)
                 Settings.dev_print("password entered")
                 password_.send_keys(Keys.ENTER)
                 # check for phone number page
                 time.sleep(1)
                 if "Verify your identity by entering the phone number associated with your Twitter account." in str(self.browser.find_element(By.TAG_NAME, 'body').text):
+                    Settings.maybe_print("verifying phone number...")
                     element = self.browser.switch_to.active_element
                     element.send_keys(str(Settings.get_phone_number()))
                     element.send_keys(Keys.ENTER)
                     time.sleep(1)
                 return login_check("twitter")
             except Exception as e:
                 Settings.dev_print("twitter login failure")
```

### Comparing `OnlySnarf-4.5.7/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.8/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/menu.py` & `OnlySnarf-4.5.8/OnlySnarf/menu.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/snarf.py` & `OnlySnarf-4.5.8/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/args.py` & `OnlySnarf-4.5.8/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.8/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/config.py` & `OnlySnarf-4.5.8/OnlySnarf/util/config.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.8/OnlySnarf/util/defaults.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.8/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.8/OnlySnarf/util/optional_args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.8/OnlySnarf/util/settings.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.8/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.5.8/OnlySnarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.7
+Version: 4.5.8
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.7 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.8 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.7/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.8/OnlySnarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/PKG-INFO` & `OnlySnarf-4.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.7
+Version: 4.5.8
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.7 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.8 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.7/README.md` & `OnlySnarf-4.5.8/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/setup.py` & `OnlySnarf-4.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.7",
+    version="4.5.8",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `OnlySnarf-4.5.7/tests/test_profile.py` & `OnlySnarf-4.5.8/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.7/tests/test_promotion.py` & `OnlySnarf-4.5.8/tests/test_promotion.py`

 * *Files identical despite different names*

