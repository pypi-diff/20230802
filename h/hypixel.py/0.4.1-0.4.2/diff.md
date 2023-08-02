# Comparing `tmp/hypixel.py-0.4.1.tar.gz` & `tmp/hypixel.py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypixel.py-0.4.1.tar", last modified: Tue Feb  7 07:10:02 2023, max compression
+gzip compressed data, was "hypixel.py-0.4.2.tar", last modified: Wed Aug  2 04:25:27 2023, max compression
```

## Comparing `hypixel.py-0.4.1.tar` & `hypixel.py-0.4.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.253364 hypixel.py-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1567 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1070 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       81 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6206 2023-02-07 07:10:02.253364 hypixel.py-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4077 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.249364 hypixel.py-0.4.1/hypixel/
--rw-r--r--   0 runner    (1001) docker     (116)      434 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3102 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/achievement.py
--rw-r--r--   0 runner    (1001) docker     (116)     3149 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/aliases.py
--rw-r--r--   0 runner    (1001) docker     (116)    33345 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     3614 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/color.py
--rw-r--r--   0 runner    (1001) docker     (116)     6830 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     6833 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/game.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.249364 hypixel.py-0.4.1/hypixel/models/
--rw-r--r--   0 runner    (1001) docker     (116)      321 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      779 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/aliases.py
--rw-r--r--   0 runner    (1001) docker     (116)      337 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/bans.py
--rw-r--r--   0 runner    (1001) docker     (116)      494 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/friend.py
--rw-r--r--   0 runner    (1001) docker     (116)      379 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/games.py
--rw-r--r--   0 runner    (1001) docker     (116)     3082 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (116)      335 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/key.py
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/leaderboards.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.253364 hypixel.py-0.4.1/hypixel/models/player/
--rw-r--r--   0 runner    (1001) docker     (116)      497 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18154 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/aliases.py
--rw-r--r--   0 runner    (1001) docker     (116)     1763 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/arcade.py
--rw-r--r--   0 runner    (1001) docker     (116)     5945 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/bedwars.py
--rw-r--r--   0 runner    (1001) docker     (116)      867 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/blitz.py
--rw-r--r--   0 runner    (1001) docker     (116)     3028 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/duels.py
--rw-r--r--   0 runner    (1001) docker     (116)     1685 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/murder_mystery.py
--rw-r--r--   0 runner    (1001) docker     (116)      558 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/paintball.py
--rw-r--r--   0 runner    (1001) docker     (116)     2528 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/parkour.py
--rw-r--r--   0 runner    (1001) docker     (116)     7197 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/player.py
--rw-r--r--   0 runner    (1001) docker     (116)     2034 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/skywars.py
--rw-r--r--   0 runner    (1001) docker     (116)      417 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/socials.py
--rw-r--r--   0 runner    (1001) docker     (116)      566 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/tkr.py
--rw-r--r--   0 runner    (1001) docker     (116)      229 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/tnt_games.py
--rw-r--r--   0 runner    (1001) docker     (116)     1977 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/uhc.py
--rw-r--r--   0 runner    (1001) docker     (116)     7734 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1400 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/player/wool_games.py
--rw-r--r--   0 runner    (1001) docker     (116)      479 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1939 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7340 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/hypixel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.249364 hypixel.py-0.4.1/hypixel.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6206 2023-02-07 07:10:02.000000 hypixel.py-0.4.1/hypixel.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1492 2023-02-07 07:10:02.000000 hypixel.py-0.4.1/hypixel.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-07 07:10:02.000000 hypixel.py-0.4.1/hypixel.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      400 2023-02-07 07:10:02.000000 hypixel.py-0.4.1/hypixel.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2023-02-07 07:10:02.000000 hypixel.py-0.4.1/hypixel.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2351 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-07 07:10:02.253364 hypixel.py-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1702 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-07 07:10:02.253364 hypixel.py-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      626 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_ban_info.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     2625 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     2578 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (116)     4722 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_guild.py
--rw-r--r--   0 runner    (1001) docker     (116)      935 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_leaderboards.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_player.py
--rw-r--r--   0 runner    (1001) docker     (116)      476 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_player_count.py
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_player_friends.py
--rw-r--r--   0 runner    (1001) docker     (116)     1880 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_player_status.py
--rw-r--r--   0 runner    (1001) docker     (116)      744 2023-02-07 07:09:46.000000 hypixel.py-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/
+-rw-r--r--   0 josh      (1000) josh      (1000)     2157 2023-08-02 04:16:40.000000 hypixel.py-0.4.2/CHANGELOG.md
+-rw-r--r--   0 josh      (1000) josh      (1000)     1070 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/LICENSE
+-rw-r--r--   0 josh      (1000) josh      (1000)      106 2023-06-14 20:42:23.000000 hypixel.py-0.4.2/MANIFEST.in
+-rw-r--r--   0 josh      (1000) josh      (1000)     6192 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)     4082 2023-07-10 17:12:52.000000 hypixel.py-0.4.2/README.rst
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.377298 hypixel.py-0.4.2/hypixel/
+-rw-r--r--   0 josh      (1000) josh      (1000)      434 2023-08-02 04:17:11.000000 hypixel.py-0.4.2/hypixel/__init__.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2980 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/achievement.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3023 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/aliases.py
+-rw-r--r--   0 josh      (1000) josh      (1000)    33423 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/client.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3614 2023-06-09 04:02:42.000000 hypixel.py-0.4.2/hypixel/color.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6830 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/errors.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6833 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/game.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/hypixel/models/
+-rw-r--r--   0 josh      (1000) josh      (1000)      321 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/__init__.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      779 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/aliases.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      337 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/bans.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      493 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/friend.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      379 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/games.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3082 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/guild.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      335 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/key.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1190 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/leaderboards.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/hypixel/models/player/
+-rw-r--r--   0 josh      (1000) josh      (1000)      497 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/__init__.py
+-rw-r--r--   0 josh      (1000) josh      (1000)    18195 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/aliases.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1890 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/arcade.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     5945 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/bedwars.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      867 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/blitz.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3028 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/duels.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1685 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/murder_mystery.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      558 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/paintball.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2528 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/parkour.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     8022 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/player.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2034 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/skywars.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      417 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/socials.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      566 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/tkr.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      229 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/tnt_games.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1977 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/uhc.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     7734 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/utils.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1400 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/player/wool_games.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      479 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/status.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1939 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/hypixel/models/utils.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-06-14 20:52:07.000000 hypixel.py-0.4.2/hypixel/py.typed
+-rw-r--r--   0 josh      (1000) josh      (1000)     7370 2023-07-10 17:12:52.000000 hypixel.py-0.4.2/hypixel/utils.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.377298 hypixel.py-0.4.2/hypixel.py.egg-info/
+-rw-r--r--   0 josh      (1000) josh      (1000)     6192 2023-08-02 04:25:27.000000 hypixel.py-0.4.2/hypixel.py.egg-info/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)     1500 2023-08-02 04:25:27.000000 hypixel.py-0.4.2/hypixel.py.egg-info/SOURCES.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        1 2023-08-02 04:25:27.000000 hypixel.py-0.4.2/hypixel.py.egg-info/dependency_links.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)      351 2023-08-02 04:25:27.000000 hypixel.py-0.4.2/hypixel.py.egg-info/requires.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        8 2023-08-02 04:25:27.000000 hypixel.py-0.4.2/hypixel.py.egg-info/top_level.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)     2289 2023-08-02 04:17:11.000000 hypixel.py-0.4.2/pyproject.toml
+-rw-r--r--   0 josh      (1000) josh      (1000)       16 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/requirements.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       38 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/setup.cfg
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-08-02 04:25:27.380631 hypixel.py-0.4.2/tests/
+-rw-r--r--   0 josh      (1000) josh      (1000)      626 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_ban_info.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_cache.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2625 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_client.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2578 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_dataclasses.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     4722 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_guild.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      935 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_key.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_leaderboards.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_player.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      476 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_player_count.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1210 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_player_friends.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1880 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_player_status.py
+-rw-r--r--   0 josh      (1000) josh      (1000)      744 2023-06-08 04:41:52.000000 hypixel.py-0.4.2/tests/test_utils.py
```

### Comparing `hypixel.py-0.4.1/CHANGELOG.md` & `hypixel.py-0.4.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,47 @@
 All notable changes to this project will be documented here.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.4.1] - 2022-2-6
+## [0.4.2] - 2023-8-1
+
+### Added
+
+- publish.sh that's run after tbump pushes to github.
+- Player.build_achievements method.
+- Clarifying comments.
+- HypixelSays.top_score.
+- Typing metadata (PEP 561 compliant).
+
+### Changed
+
+- Documentation wording.
+- Documentation logo.
+
+### Removed
+
+- setup.py.
+- publish-to-pypi github action.
+- Player.known_aliases.
+- Logo in documentation sidebar.
+- Unused "Friend" code.
+- Unused imports.
 
 ### Fixed
 
-- Remote tests.
-- PyPI intended audience.
+- Start line in player_friend example documentation.
+- Documentation typos.
+- Player documentation attribute hyperlinks.
+- PlayerNotFound for Mojang API calls.
+- HypixelSays.losses.
 
-## [0.4.0] - 2022-2-6
+## [0.4.1] - 2022-2-6
 
 ### Added
 
 - This changelog file.
 - Achievement class.
 - Pyproject.toml for tbump and pytest configs.
 - Return documentation on dataclass class methods.
@@ -39,14 +64,16 @@
 
 ### Fixed
 
 - Documentation punctuation.
 - Version locking in setup.py.
 - Circular import bug.
 - Readthedocs config formatting.
+- Remote tests.
+- PyPI intended audience.
 
 ### Breaking Changes
 
 - Status.game_type is changed to Status.game.
 
 ## [0.3.1] - 2022-10-16
 
@@ -56,11 +83,11 @@
 - Datetime tests are now fixed and enabled.
 - Documentation links now go to latest rather than dev (a deleted version).
 
 ### Deprecated
 
 - Player.version always returns ``None`` and will be removed in a later release.
 
-[Unreleased]: https://github.com/duhby/hypixel.py/compare/v0.4.1...master
+[Unreleased]: https://github.com/duhby/hypixel.py/compare/v0.4.2...master
+[0.4.2]: https://github.com/duhby/hypixel.py/releases/tag/v0.4.2
 [0.4.1]: https://github.com/duhby/hypixel.py/releases/tag/v0.4.1
-[0.4.0]: https://github.com/duhby/hypixel.py/releases/tag/v0.4.0
 [0.3.1]: https://github.com/duhby/hypixel.py/releases/tag/v0.3.1
```

### Comparing `hypixel.py-0.4.1/LICENSE` & `hypixel.py-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/PKG-INFO` & `hypixel.py-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: hypixel.py
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python wrapper for the Hypixel API
-Home-page: https://github.com/duhby/hypixel.py
 Author: duhby
 License: MIT License
         
         Copyright (c) 2021-present duhby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,19 +31,20 @@
 Project-URL: Bug Tracker, https://github.com/duhby/hypixel.py/issues/
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: speed
-Provides-Extra: data
 Provides-Extra: docs
+Provides-Extra: data
+Provides-Extra: speed
 Provides-Extra: test
 License-File: LICENSE
 
 hypixel.py (beta)
 =================
 
 .. .. image:: https://img.shields.io/discord/719949131497603123.svg?color=%237289da&label=discord&logo=discord&style=for-the-badge
@@ -66,15 +66,15 @@
 
 .. start_doc
 
 Hypixel.py is a modern, asynchronous, feature-rich, Hypixel API wrapper for Python.
 
 The purpose of this project is to simplify the task of writing scripts that interact with the Hypixel API by converting responses into organized python models and abstracting requests into asynchronous functions, while also offering customization options and useful features.
 
-* **Fast AF (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
+* **Blazing fast (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
 * **More asynchronous than online learning** --- Has full asynchronicity and uses modern pythonic ``async`` and ``await`` syntax.
 * **Cleaner than your room** --- Uses object oriented pythonic dot syntax for all of its models, so you can easily access any data point without worrying about dictionaries, strings, and any random inconsistencies you may encounter using the raw API.
 * **S Tier Docs** --- Highly maintained documentation with an ample amount of examples to get you started. It also has the highest player model and coverage documentation.
 
 .. end_doc
```

### Comparing `hypixel.py-0.4.1/README.rst` & `hypixel.py-0.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 .. start_doc
 
 Hypixel.py is a modern, asynchronous, feature-rich, Hypixel API wrapper for Python.
 
 The purpose of this project is to simplify the task of writing scripts that interact with the Hypixel API by converting responses into organized python models and abstracting requests into asynchronous functions, while also offering customization options and useful features.
 
-* **Fast AF (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
+* **Blazing fast (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
 * **More asynchronous than online learning** --- Has full asynchronicity and uses modern pythonic ``async`` and ``await`` syntax.
 * **Cleaner than your room** --- Uses object oriented pythonic dot syntax for all of its models, so you can easily access any data point without worrying about dictionaries, strings, and any random inconsistencies you may encounter using the raw API.
 * **S Tier Docs** --- Highly maintained documentation with an ample amount of examples to get you started. It also has the highest player model and coverage documentation.
 
 .. end_doc
```

### Comparing `hypixel.py-0.4.1/hypixel/achievement.py` & `hypixel.py-0.4.2/hypixel/achievement.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     type_name: :class:`str`
         The type name used to reference the achievement in the Hypixel
         API.
     points: :class:`int`
         Amount of achievement points the achievement is worth.
     name: :class:`str`
         The name of the achievement.
-    description: :class`str`
+    description: :class:`str`
         The description of the achievement.
     global_unlocked: Optional[:class:`float`]
         The percentage of players who have unlocked the achievement.
 
         .. note::
 
             For achievements which :attr:`legacy` is ``True``, this
@@ -61,27 +61,24 @@
     global_unlocked: Optional[float] = None
     game_unlocked: Optional[float] = None
     legacy: bool = False
 
     @classmethod
     @functools.lru_cache()
     def from_type(cls, type_name: str) -> Optional[Achievement]:
-        """Constructs a :class:`Achievement` from its type name.
+        """Constructs an :class:`Achievement` from its type name.
+
+        |data|
 
         .. warning::
 
             Some achievements that come from the Hypixel API will return
             ``None``. This is because the API does not provide the data
             for some older achievements.
 
-        .. warning::
-
-            If the module ``hypixel.py-data`` is not installed, this
-            method will always return ``None``.
-
         Parameters
         ----------
         type_name: :class:`str`
             The type name used in Hypixel API attributes.
 
         Returns
         -------
```

### Comparing `hypixel.py-0.4.1/hypixel/aliases.py` & `hypixel.py-0.4.2/hypixel/aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MIT License, see LICENSE for more details.
 """
 
 # Sorted alphabetically by category
 __all__ = [
     'ACHIEVEMENT',
     'BANS',
-    'FRIEND',
+    # 'FRIEND',
     'GUILD',
     'KEY',
     'LB',
     'PLAYER',
     'STATUS',
 ]
 
@@ -35,19 +35,20 @@
     'staff_rollingDaily': 'staff_day',
     'staff_total': 'staff_total',
     'watchdog_lastMinute': 'watchdog_recent',
     'watchdog_rollingDaily': 'watchdog_day',
     'watchdog_total': 'watchdog_total',
 }
 
-FRIEND = {
-    '_id': 'id',
-    'uuidReceiver': 'uuid',
-    'started': 'started',
-}
+# Deprecated by Hypixel
+# FRIEND = {
+#     '_id': 'id',
+#     'uuidReceiver': 'uuid',
+#     'started': 'started',
+# }
 
 GUILD = {
     '_id': 'id',
     'name': 'name',
     'exp': 'exp',
     'created': 'created',
     'winners': 'winners',
@@ -83,43 +84,47 @@
 }
 
 PLAYER = {
     '_id': 'id',
     'uuid': 'uuid',
     'firstLogin': 'first_login',
     'displayname': 'name',
-    # 'playername': 'name', # lowercase version of displayname
+    # Lowercase version of displayname, so basically useless
+    # 'playername'
     'lastLogin': 'last_login',
     'lastLogout': 'last_logout',
-    'knownAliases': 'known_aliases',
-    # 'knownAliasesLower'
     'achievementsOneTime': 'achievements',
-    # 'achievement_stats': 'achievement_stats',
+    # 'achievement_stats'
     'achievementPoints': 'achievement_points',
     'networkExp': 'network_exp',
     'karma': 'karma',
-    # 'mcVersionRp': 'version', # deprecated by Hypixel
-    # 'rank': 'rank_',
-    # 'newPackageRank': 'package_rank',
-    # 'rankPlusColor': 'rank_color',
-    # 'monthlyPackageRank': 'monthly_package_rank',
-    # 'monthlyRankColor': 'monthly_rank_color',
+    'currentGadget': 'current_gadget',
+    'channel': 'channel',
+    # 'rankPlusColor'
+    # 'monthlyPackageRank'
+    # 'monthlyRankColor'
     # 'lastAdsenseGenerateTime'
     # 'lastClaimedReward'
     # 'totalRewards'
     # 'totalDailyRewards'
     # 'rewardStreak'
     # 'rewardScore'
     # 'rewardHighScore'
-    # 'friendRequestsUuid': 'friend_requests_uuid'
+    # 'friendRequestsUuid'
     # 'achievementTracking'
-    'currentGadget': 'current_gadget',
-    'channel': 'channel',
+
     # Handled in Player class instead
-    # 'mostRecentGameType': 'most_recent_game',
+    # 'mostRecentGameType'
+    # 'rank'
+    # 'newPackageRank'
+
+    # Deprecated by hypixel
+    # 'knownAliases'
+    # 'knownAliasesLower'
+    # 'mcVersionRp'
 }
 
 STATUS = {
     'online': 'online',
     'gameType': 'game',
     'mode': 'mode',
     'map': 'map',
```

### Comparing `hypixel.py-0.4.1/hypixel/client.py` & `hypixel.py-0.4.2/hypixel/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         .. warning::
 
             Please note that using multiple keys is disallowed by
             Hypixel: "You may not use methods such as multiple accounts
             to bypass the API limits." Refer to
             (https://github.com/HypixelDev/PublicAPI/issues/229) and
             (https://api.hypixel.net/#section/Introduction/Rules) for
-            more information.
+            more information. Hypixel.py does not encourage the use of
+            multiple keys.
     loop: :class:`asyncio.AbstractEventLoop`
         The loop the client will use for asynchronous operations.
         Defaults to ``None`` in which case the event loop is created
         using :func:`asyncio.get_event_loop()`.
     autoverify: :class:`bool`
         Runs :meth:`validate_keys` on client initialization.
         Defaults to ``False``.
@@ -67,15 +68,15 @@
         Whether or not API calls are cached. If ``True``, new requests
         won't be made for the same calls to request methods if the
         response for the passed arguments is still stored.
         Defaults to ``False``.
 
         .. note::
 
-            Cached items will be stored either until the size limit is
+            Cached items will be accessible either until the size limit is
             reached (``self.cache_size``), or the cached data expires
             (``self.cache_time``).
 
         .. note::
 
             The cache uses an async, time-invalidating, least recently
             used implementation. This means it works on asynchronous
@@ -85,15 +86,15 @@
 
         .. admonition:: Limitations
 
             When a cached item is time-invalidated, it does not get
             removed from the cache and can inflate the cache size with
             multiple of the same item if they were called far enough
             apart from each other and ``self.cache_time`` is not
-            ``None``. ``self.cache_time`` is based on the time from when
+            ``None``. Also, ``self.cache_time`` is based on the time from when
             it's first added to the cache, and not refreshed on the last
             access to that cached item. This could also be considered a
             feature and is therefore a design decision.
     cache_h: :class:`bool`
         Whether or not to cache Hypixel API calls.
         Refer to ``self.cache`` for more information.
         Defaults to ``self.cache``.
@@ -345,15 +346,15 @@
         if response.status == 200:
             data = await response.json(loads=JSON_DECODER)
             uuid = data.get('id')
             if not uuid:
                 raise PlayerNotFound(name)
             return uuid
 
-        elif response.status == 204:
+        elif response.status == 404:
             raise PlayerNotFound(name)
 
         else:
             raise ApiError(response, 'mojang')
 
     async def _get_name_helper(self, uuid):
         return await self._session.get(
@@ -382,15 +383,15 @@
         if response.status == 200:
             data = await response.json(loads=JSON_DECODER)
             name = data.get('name')
             if not name:
                 raise PlayerNotFound(uuid)
             return name
 
-        elif response.status == 204:
+        elif response.status == 404:
             raise PlayerNotFound(uuid)
 
         else:
             raise ApiError(response, 'mojang')
 
     async def _get_helper(self, path, params):
         return await self._session.get(
```

### Comparing `hypixel.py-0.4.1/hypixel/color.py` & `hypixel.py-0.4.2/hypixel/color.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/errors.py` & `hypixel.py-0.4.2/hypixel/errors.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/game.py` & `hypixel.py-0.4.2/hypixel/game.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/aliases.py` & `hypixel.py-0.4.2/hypixel/models/aliases.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/guild.py` & `hypixel.py-0.4.2/hypixel/models/guild.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/leaderboards.py` & `hypixel.py-0.4.2/hypixel/models/leaderboards.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/aliases.py` & `hypixel.py-0.4.2/hypixel/models/player/aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,14 +368,15 @@
     'uhc_duel_bow_hits': 'arrows_hit',
     'uhc_duel_bow_shots': 'arrows_shot',
 }
 
 HYPIXEL_SAYS = {
     'rounds_simon_says': 'rounds',
     'wins_simon_says': 'wins',
+    'top_score_simon_says': 'top_score',
 }
 
 MINI_WALLS = {
     'kills_mini_walls': 'kills',
     'deaths_mini_walls': 'deaths',
     'wins_mini_walls': 'wins',
     'final_kills_mini_walls': 'final_kills',
```

### Comparing `hypixel.py-0.4.1/hypixel/models/player/arcade.py` & `hypixel.py-0.4.2/hypixel/models/player/arcade.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,20 @@
     captures: int = 0
     kills_assists: int = 0
 
 @dataclass
 class HypixelSays:
     rounds: int = 0
     wins: int = 0
-    losses: int = rounds - wins
+    top_score: int = 0
+    losses: int = field(init=False)
     wlr: float = field(init=False)
 
     def __post_init__(self):
+        self.losses = self.rounds - self.wins
         self.wlr = utils.safe_div(self.wins, self.losses)
 
 @dataclass
 class MiniWalls:
     kills: int = 0
     deaths: int = 0
     wins: int = 0
@@ -63,14 +65,15 @@
     coins: int = 0
     ctw: CaptureTheWool = field(init=False)
     hypixel_says: HypixelSays = field(init=False)
     mini_walls: MiniWalls = field(init=False)
     party_games: PartyGames = field(init=False)
 
     def __post_init__(self):
+        self.coins = int(self.coins) # Normally float
         modes = {
             'ctw': CaptureTheWool,
             'hypixel_says': HypixelSays,
             'mini_walls': MiniWalls,
             'party_games': PartyGames,
         }
         for mode, model in modes.items():
```

### Comparing `hypixel.py-0.4.1/hypixel/models/player/bedwars.py` & `hypixel.py-0.4.2/hypixel/models/player/bedwars.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/blitz.py` & `hypixel.py-0.4.2/hypixel/models/player/blitz.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/duels.py` & `hypixel.py-0.4.2/hypixel/models/player/duels.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/murder_mystery.py` & `hypixel.py-0.4.2/hypixel/models/player/murder_mystery.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/paintball.py` & `hypixel.py-0.4.2/hypixel/models/player/paintball.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/parkour.py` & `hypixel.py-0.4.2/hypixel/models/player/parkour.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/player.py` & `hypixel.py-0.4.2/hypixel/models/player/player.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MIT License, see LICENSE for more details.
 """
 
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Literal, List, Optional
 
+from ...achievement import Achievement
 from ...color import Color
 from ...game import Game
 
 from .arcade import Arcade
 from .bedwars import Bedwars
 from .blitz import Blitz
 from .duels import Duels
@@ -31,14 +32,19 @@
 ]
 
 
 @dataclass
 class Player:
     """Player model object.
 
+    .. tip::
+
+        You can use the ``==`` operator to compare two
+        :class:`~hypixel.models.player.Player` classes.
+
     Attributes
     ----------
     raw: :class:`dict`
         The raw json response returned from the API.
     id: :class:`str`
         Hypixel's unique identifier.
     uuid: :class:`str`
@@ -55,24 +61,23 @@
             then this attribute will be outdated.
     last_login: :class:`datetime.datetime`
         The last login time represented as a datetime in the UTC
         timezone.
     last_logout: :class:`datetime.datetime`
         The last logout time represented as a datetime in the UTC
         timezone.
-    known_aliases: List[:class:`str`]
-        A list of previous usernames the account has logged onto Hypixel
-        with.
     achievements: List[:class:`str`]
         A list of achievement name strings.
 
-        .. warning::
+        .. tip::
 
-            This will most likely be changed to List[Achievement] before
-            the 1.0 release.
+            You can use :meth:`hypixel.Achievement.from_type` to get
+            the achievement object from its type name string. You can
+            also use :meth:`build_achievements` to build a list of
+            :class:`~hypixel.Achievement` objects.
     network_exp: :class:`int`
         The player's current network experience points.
     karma: :class:`int`
         The player's current karma.
     achievement_points: :class:`int`
         The player's achievement points.
     current_gadget: :class:`str`
@@ -93,54 +98,55 @@
         ``'MOJANG'``, ``'GAME MASTER'``, ``'ADMIN'``, and ``'OWNER'``.
     plus_color: Optional[:class:`~hypixel.Color`]
         The player's plus color if their rank has a plus in it;
         otherwise ``None``.
     level: :class:`float`
         The player's Hypixel level.
     most_recent_game: Optional[:class:`~hypixel.Game`]
+        The player's most recent game they played.
+
         .. note::
 
             Will be ``None`` if the player's ``Recent Games`` API
             setting is disabled.
-    arcade: :class:`~models.playerdata.Arcade`
+    arcade: :class:`~hypixel.models.player.Arcade`
         A model for abstracting arcade data.
-    bedwars: :class:`~models.playerdata.Bedwars`
+    bedwars: :class:`~hypixel.models.player.Bedwars`
         A model for abstracting bedwars data.
-    blitz: :class:`~models.playerdata.Blitz`
+    blitz: :class:`~hypixel.models.player.Blitz`
         A model for abstracting blitz data.
-    duels: :class:`~models.playerdata.Duels`
+    duels: :class:`~hypixel.models.player.Duels`
         A model for abstracting duels data.
-    murder_mystery: :class:`~models.playerdata.MurderMystery`
+    murder_mystery: :class:`~hypixel.models.player.MurderMystery`
         A model for abstracting murder mystery data.
-    paintball: :class:`~models.playerdata.Paintball`
+    paintball: :class:`~hypixel.models.player.Paintball`
         A model for abstracting paintball data.
-    parkour: :class:`~models.playerdata.Parkour`
+    parkour: :class:`~hypixel.models.player.Parkour`
         A model for abstracting parkour data.
-    skywars: :class:`~models.playerdata.Skywars`
+    skywars: :class:`~hypixel.models.player.Skywars`
         A model for abstracting skywars data.
-    socials: :class:`~models.playerdata.Socials`
+    socials: :class:`~hypixel.models.player.Socials`
         A model for abstracting socials data.
-    tkr: :class:`~models.playerdata.TurboKartRacers`
+    tkr: :class:`~hypixel.models.player.TurboKartRacers`
         A model for abstracting tkr data.
-    tnt_games: :class:`~models.playerdata.TntGames`
+    tnt_games: :class:`~hypixel.models.player.TntGames`
         A model for abstracting tnt games data.
-    uhc: :class:`~models.playerdata.Uhc`
+    uhc: :class:`~hypixel.models.player.Uhc`
         A model for abstracting uhc data.
-    wool_games: :class:`~models.playerdata.WoolGames`
+    wool_games: :class:`~hypixel.models.player.WoolGames`
         A model for abstracting wool games data.
     """
     _data: dict = field(repr=False)
     raw: dict = field(repr=False)
     id: str = None
     uuid: str = None
     first_login: datetime = None
     name: str = None
     last_login: datetime = None
     last_logout: datetime = None
-    known_aliases: list = None
     achievements: list = field(default_factory=list, repr=False)
     network_exp: int = 0
     karma: int = 0
     achievement_points: int = 0
     current_gadget: str = None
     channel: str = None
     rank: Optional[str] = field(init=False)
@@ -178,15 +184,14 @@
         self.level = utils.get_network_level(self.network_exp)
         self.rank = utils.get_rank(self.raw)
         self.most_recent_game = Game.from_type(
             self.raw.get('player', {}).get('mostRecentGameType')
         )
         self.plus_color = Color.from_type(self._data.get('rankPlusColor'))
 
-        # playerdata
         modes = {
             'arcade': Arcade,
             'bedwars': Bedwars,
             'blitz': Blitz,
             'duels': Duels,
             'murder_mystery': MurderMystery,
             'paintball': Paintball,
@@ -198,11 +203,27 @@
             'uhc': Uhc,
             'wool_games': WoolGames,
         }
         for mode, model in modes.items():
             data = utils._clean(self._data, mode=mode.upper())
             setattr(self, mode, model(**data))
 
+    def build_achievements(self):
+        """Converts the achievements in :attr:`achievements` to
+        List[:class:`~hypixel.Achievement`].
+
+        .. warning::
+
+            If the package ``hypixel.py-data`` is not installed, this
+            will convert :attr:`achievements` to an empty list.
+        """
+        built_achievements = []
+        for achievement in self.achievements:
+            achievement = Achievement.from_type(achievement)
+            if achievement:
+                built_achievements.append(achievement)
+        self.achievements = built_achievements
+
     def __eq__(self, other: object):
         if isinstance(other, Player):
             return self.uuid == other.uuid
         return False
```

### Comparing `hypixel.py-0.4.1/hypixel/models/player/skywars.py` & `hypixel.py-0.4.2/hypixel/models/player/skywars.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/tkr.py` & `hypixel.py-0.4.2/hypixel/models/player/tkr.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/uhc.py` & `hypixel.py-0.4.2/hypixel/models/player/uhc.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/utils.py` & `hypixel.py-0.4.2/hypixel/models/player/utils.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/player/wool_games.py` & `hypixel.py-0.4.2/hypixel/models/player/wool_games.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/models/utils.py` & `hypixel.py-0.4.2/hypixel/models/utils.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/hypixel/utils.py` & `hypixel.py-0.4.2/hypixel/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 __all__ = [
     'ExponentialBackoff',
     'HashedDict',
     'strfdelta',
 ]
 
 
-def _clean(data: dict, mode: str, extra=None) -> dict:
+def _clean(data: dict, mode: str) -> dict:
     alias = globals()[mode]
 
     if mode == 'PLAYER':
         # Avoid name conflicts
         data['achievement_stats'] = data.pop('achievements', {})
 
-    elif mode == 'FRIEND':
-        # Sender and receiver could be either the player or the friend
-        # as the api stores the sender and receiver of the actual friend
-        # request.
-        # Extra is the player's uuid.
-        if data['uuidReceiver'] == extra:
-            data['uuidReceiver'] = data['uuidSender']
+    # Deprecated by Hypixel
+    # elif mode == 'FRIEND':
+    #     # Sender and receiver could be either the player or the friend
+    #     # as the api stores the sender and receiver of the actual friend
+    #     # request.
+    #     # Extra is the player's uuid.
+    #     if data['uuidReceiver'] == extra:
+    #         data['uuidReceiver'] = data['uuidSender']
 
     elif mode == 'STATUS':
         data['gameType'] = Game.from_type(data.get('gameType'))
 
     elif mode == 'GUILD':
         achievements = data.get('achievements', {})
         data['winners'] = achievements.get('WINNERS')
```

### Comparing `hypixel.py-0.4.1/hypixel.py.egg-info/PKG-INFO` & `hypixel.py-0.4.2/hypixel.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: hypixel.py
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python wrapper for the Hypixel API
-Home-page: https://github.com/duhby/hypixel.py
 Author: duhby
 License: MIT License
         
         Copyright (c) 2021-present duhby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,19 +31,20 @@
 Project-URL: Bug Tracker, https://github.com/duhby/hypixel.py/issues/
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: speed
-Provides-Extra: data
 Provides-Extra: docs
+Provides-Extra: data
+Provides-Extra: speed
 Provides-Extra: test
 License-File: LICENSE
 
 hypixel.py (beta)
 =================
 
 .. .. image:: https://img.shields.io/discord/719949131497603123.svg?color=%237289da&label=discord&logo=discord&style=for-the-badge
@@ -66,15 +66,15 @@
 
 .. start_doc
 
 Hypixel.py is a modern, asynchronous, feature-rich, Hypixel API wrapper for Python.
 
 The purpose of this project is to simplify the task of writing scripts that interact with the Hypixel API by converting responses into organized python models and abstracting requests into asynchronous functions, while also offering customization options and useful features.
 
-* **Fast AF (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
+* **Blazing fast (for python)** --- Prioritizes speed and efficiency by using built in libraries to achieve asynchronous timed caching, quick nested dataclass sterilization, and modern rate limit handling.
 * **More asynchronous than online learning** --- Has full asynchronicity and uses modern pythonic ``async`` and ``await`` syntax.
 * **Cleaner than your room** --- Uses object oriented pythonic dot syntax for all of its models, so you can easily access any data point without worrying about dictionaries, strings, and any random inconsistencies you may encounter using the raw API.
 * **S Tier Docs** --- Highly maintained documentation with an ample amount of examples to get you started. It also has the highest player model and coverage documentation.
 
 .. end_doc
```

### Comparing `hypixel.py-0.4.1/hypixel.py.egg-info/SOURCES.txt` & `hypixel.py-0.4.2/hypixel.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
-setup.py
 hypixel/__init__.py
 hypixel/achievement.py
 hypixel/aliases.py
 hypixel/client.py
 hypixel/color.py
 hypixel/errors.py
 hypixel/game.py
+hypixel/py.typed
 hypixel/utils.py
 hypixel.py.egg-info/PKG-INFO
 hypixel.py.egg-info/SOURCES.txt
 hypixel.py.egg-info/dependency_links.txt
 hypixel.py.egg-info/requires.txt
 hypixel.py.egg-info/top_level.txt
 hypixel/models/__init__.py
```

### Comparing `hypixel.py-0.4.1/pyproject.toml` & `hypixel.py-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
+    "Typing :: Typed",
 ]
 license = {file = "LICENSE"}
 dependencies = ["aiohttp>=3.8,<4"]
 dynamic = ['version']
 
 [project.optional-dependencies]
 docs = [
@@ -66,15 +67,15 @@
 [tool.setuptools.dynamic]
 version = {attr = "hypixel.__version__"}
 
 [tool.tbump]
 github_url = "https://github.com/duhby/hypixel.py/"
 
 [tool.tbump.version]
-current = "0.4.1"
+current = "0.4.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (.
@@ -94,12 +95,10 @@
 src = "docs/conf.py"
 search = "release = '{current_version}'"
 
 [[tool.tbump.before_commit]]
 name = "check changelog"
 cmd = "git grep -q {new_version} CHANGELOG.md"
 
-# Or run some commands after the git tag and the branch
-# have been pushed:
-#  [[tool.tbump.after_push]]
-#  name = "publish"
-#  cmd = "./publish.sh"
+[[tool.tbump.after_push]]
+name = "publish"
+cmd = "./publish.sh"
```

### Comparing `hypixel.py-0.4.1/tests/test_ban_info.py` & `hypixel.py-0.4.2/tests/test_ban_info.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_client.py` & `hypixel.py-0.4.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_dataclasses.py` & `hypixel.py-0.4.2/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_guild.py` & `hypixel.py-0.4.2/tests/test_guild.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_key.py` & `hypixel.py-0.4.2/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_player_friends.py` & `hypixel.py-0.4.2/tests/test_player_friends.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_player_status.py` & `hypixel.py-0.4.2/tests/test_player_status.py`

 * *Files identical despite different names*

### Comparing `hypixel.py-0.4.1/tests/test_utils.py` & `hypixel.py-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

