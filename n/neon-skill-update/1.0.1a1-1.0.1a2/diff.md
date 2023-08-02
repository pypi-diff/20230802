# Comparing `tmp/neon-skill-update-1.0.1a1.tar.gz` & `tmp/neon-skill-update-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-1.0.1a1.tar", last modified: Mon Jul 31 22:14:23 2023, max compression
+gzip compressed data, was "neon-skill-update-1.0.1a2.tar", last modified: Wed Aug  2 18:12:41 2023, max compression
```

## Comparing `neon-skill-update-1.0.1a1.tar` & `neon-skill-update-1.0.1a2.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    22527 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.188552 neon-skill-update-1.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.188552 neon-skill-update-1.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_updating_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_downloading_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_system.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.396213 neon-skill-update-1.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.396213 neon-skill-update-1.0.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.412213 neon-skill-update-1.0.1a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/error_updating_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_downloading_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_downloading_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_os_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/update_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/update_system.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.412213 neon-skill-update-1.0.1a2/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 18:12:41.000000 neon-skill-update-1.0.1a2/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:12:41.416214 neon-skill-update-1.0.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-02 18:12:36.000000 neon-skill-update-1.0.1a2/version.py
```

### Comparing `neon-skill-update-1.0.1a1/LICENSE.md` & `neon-skill-update-1.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a1/PKG-INFO` & `neon-skill-update-1.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.1a1/README.md` & `neon-skill-update-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a1/__init__.py` & `neon-skill-update-1.0.1a2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,17 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 
 from random import randint
-from threading import Event
 from typing import Optional
 from adapt.intent import IntentBuilder
 from neon_utils.validator_utils import numeric_confirmation_validator
-from ovos_bus_client import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_utils.network_utils import is_connected_http
 from neon_utils.skills import NeonSkill
 from neon_utils.user_utils import get_user_prefs
 from ovos_workshop.decorators import intent_file_handler, intent_handler
@@ -108,16 +106,25 @@
         return self.settings.get("image_url")
 
     @property
     def image_drive(self):
         return self.settings.get("image_drive") or "/dev/sdb"
 
     def _on_ready(self, message):
-        LOG.debug("Checking latest core version")
-        self._check_latest_core_release(message)
+        if self.check_squashfs and self._check_squashfs_update(message):
+            if self.notify_updates:
+                text = self.dialog_renderer.render("notify_os_update_available")
+                LOG.info("OS Update Available")
+                callback_data = {**message.data, **{"notification": text}}
+                self.gui.show_notification(text,
+                                           action="update.gui.install_update",
+                                           callback_data=callback_data)
+        else:
+            LOG.debug("Checking latest core version")
+            self._check_latest_core_release(message)
 
         update_stat = self._check_update_status()
         LOG.debug(f"Update status is {update_stat}")
         if not update_stat:
             # No update was attempted
             return
         speak_version = self.pronounce_version(self.current_core_ver)
@@ -364,15 +371,16 @@
         if resp == "yes":
             self.add_event("neon.download_os_image.complete",
                            self.on_download_complete, once=True)
             self.speak_dialog("downloading_image")
             self.bus.emit(message.forward("neon.download_os_image",
                                           {"url": self.image_url}))
             self.speak_dialog("drive_instructions")
-            # TODO: Sticky notification during download
+            self.gui.show_controlled_notification(
+                self.translate("notify_downloading_os"))
         else:
             self.speak_dialog("not_updating")
 
     @intent_handler(IntentBuilder("SwitchUpdateTrackIntent").require("change")
                     .one_of("stable", "beta").require("updates").build())
     def handle_switch_update_track(self, message):
         """
@@ -409,14 +417,15 @@
     def on_download_complete(self, message):
         """
         After `handle_create_os_media`, this method will be called with the OS
         image download status. Displays a notification for the user to interact
         with to continue installation.
         :param message: message object associated with download completion
         """
+        self.gui.remove_controlled_notification()
         if message.data.get("success"):
             LOG.info(f"Showing Download Complete Notification")
             text = self.translate("notify_download_complete")
             self.gui.show_notification(
                 content=text,
                 action="update.gui.continue_installation",
                 callback_data={**message.data, **{"notification": text}})
```

### Comparing `neon-skill-update-1.0.1a1/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-1.0.1a2/neon_skill_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.1a1/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-1.0.1a2/neon_skill_update.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 locale/en-us/dialog/error_installing_os.dialog
 locale/en-us/dialog/error_offline.dialog
 locale/en-us/dialog/error_updating_os.dialog
 locale/en-us/dialog/installation_complete.dialog
 locale/en-us/dialog/not_updating.dialog
 locale/en-us/dialog/notify_download_complete.dialog
 locale/en-us/dialog/notify_download_failed.dialog
+locale/en-us/dialog/notify_downloading_os.dialog
 locale/en-us/dialog/notify_downloading_update.dialog
 locale/en-us/dialog/notify_installation_complete.dialog
 locale/en-us/dialog/notify_installation_failed.dialog
+locale/en-us/dialog/notify_os_update_available.dialog
 locale/en-us/dialog/notify_update_available.dialog
 locale/en-us/dialog/notify_update_failure.dialog
 locale/en-us/dialog/notify_update_success.dialog
 locale/en-us/dialog/notify_writing_image.dialog
 locale/en-us/dialog/point.dialog
 locale/en-us/dialog/starting_installation.dialog
 locale/en-us/dialog/starting_update.dialog
```

### Comparing `neon-skill-update-1.0.1a1/setup.py` & `neon-skill-update-1.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a1/skill.json` & `neon-skill-update-1.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a1/test/test_skill.py` & `neon-skill-update-1.0.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a1/version.py` & `neon-skill-update-1.0.1a2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.1a2"
```

