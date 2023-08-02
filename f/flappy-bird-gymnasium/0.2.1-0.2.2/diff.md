# Comparing `tmp/flappy-bird-gymnasium-0.2.1.tar.gz` & `tmp/flappy-bird-gymnasium-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flappy-bird-gymnasium-0.2.1.tar", last modified: Wed Mar 15 16:48:07 2023, max compression
+gzip compressed data, was "flappy-bird-gymnasium-0.2.2.tar", last modified: Wed Aug  2 05:04:30 2023, max compression
```

## Comparing `flappy-bird-gymnasium-0.2.1.tar` & `flappy-bird-gymnasium-0.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.343536 flappy-bird-gymnasium-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-15 16:48:07.343536 flappy-bird-gymnasium-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.339536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.335536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.339536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/
--rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/die.ogg
--rw-r--r--   0 runner    (1001) docker     (123)   194894 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/die.wav
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/hit.ogg
--rw-r--r--   0 runner    (1001) docker     (123)    96590 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/hit.wav
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/point.ogg
--rw-r--r--   0 runner    (1001) docker     (123)   177486 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/point.wav
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/swoosh.ogg
--rw-r--r--   0 runner    (1001) docker     (123)   354638 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/swoosh.wav
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/wing.ogg
--rw-r--r--   0 runner    (1001) docker     (123)    29902 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/wing.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.339536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/model/
--rw-r--r--   0 runner    (1001) docker     (123)   578608 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/model/model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.343536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/0.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/1.png
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/2.png
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/3.png
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/4.png
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/5.png
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/6.png
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/7.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/8.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/9.png
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/background-day.png
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/background-night.png
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/base.png
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/bluebird-downflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/bluebird-midflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/bluebird-upflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/gameover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/message.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/pipe-green.png
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/pipe-red.png
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/redbird-downflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/redbird-midflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/redbird-upflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/yellowbird-downflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/yellowbird-midflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/yellowbird-upflap.png
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.343536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/flappy_bird_env_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/flappy_bird_env_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/game_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:48:07.339536 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 16:48:07.000000 flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-15 16:48:07.343536 flappy-bird-gymnasium-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-03-15 16:47:57.000000 flappy-bird-gymnasium-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.465767 flappy-bird-gymnasium-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-02 05:04:30.465767 flappy-bird-gymnasium-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.449766 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.449766 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.457766 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/die.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)   194894 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/die.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/hit.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)    96590 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/hit.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/point.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)   177486 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/point.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/swoosh.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)   354638 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/swoosh.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/wing.ogg
+-rw-r--r--   0 runner    (1001) docker     (123)    29902 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/wing.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.457766 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   578608 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/model/model.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.465767 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/background-day.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/background-night.png
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/base.png
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/bluebird-downflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/bluebird-midflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/bluebird-upflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/gameover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/message.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/pipe-green.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/pipe-red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/redbird-downflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/redbird-midflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/redbird-upflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/yellowbird-downflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/yellowbird-midflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/yellowbird-upflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.465767 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/flappy_bird_env_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/flappy_bird_env_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/game_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-08-02 05:04:19.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:04:30.453766 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 05:04:30.000000 flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 05:04:30.465767 flappy-bird-gymnasium-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-02 05:04:20.000000 flappy-bird-gymnasium-0.2.2/setup.py
```

### Comparing `flappy-bird-gymnasium-0.2.1/LICENSE` & `flappy-bird-gymnasium-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/PKG-INFO` & `flappy-bird-gymnasium-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flappy-bird-gymnasium
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Gymnasium environment for the Flappy Bird game.
 Home-page: https://github.com/markub3327/flappy-bird-gymnasium
 Download-URL: https://github.com/markub3327/flappy-bird-gymnasium/releases
 Author: Martin Kubovcik
 Author-email: markub3327@gmail.com
 License: MIT License
+Project-URL: Bug Tracker, https://github.com/markub3327/flappy-bird-gymnasium/issues
 Keywords: Flappy-BirdGame Gymnasium Farama-Foundation Reinforcement-Learning Reinforcement-Learning-Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -74,23 +75,15 @@
 * +1.0 - **successfully passing a pipe**
 * -1.0 - **dying**
 
 <br>
 
 <p align="center">
   <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/yellow_bird_playing.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/red_bird_start_screen.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/blue_bird_playing.gif?raw=true" 
+       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/dqn.gif?raw=true" 
        width="200"/>
 </p>
 
 ## Installation
 
 To install `flappy-bird-gymnasium`, simply run the following command:
 
@@ -98,15 +91,15 @@
     
 ## Usage
 
 Like with other `gymnasium` environments, it's very easy to use `flappy-bird-gymnasium`.
 Simply import the package and create the environment with the `make` function.
 Take a look at the sample code below:
 
-```
+```python
 import time
 import flappy_bird_gymnasium
 import gymnasium
 env = gymnasium.make("FlappyBird-v0")
 
 obs, _ = env.reset()
 while True:
```

### Comparing `flappy-bird-gymnasium-0.2.1/README.md` & `flappy-bird-gymnasium-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -44,23 +44,15 @@
 * +1.0 - **successfully passing a pipe**
 * -1.0 - **dying**
 
 <br>
 
 <p align="center">
   <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/yellow_bird_playing.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/red_bird_start_screen.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/blue_bird_playing.gif?raw=true" 
+       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/dqn.gif?raw=true" 
        width="200"/>
 </p>
 
 ## Installation
 
 To install `flappy-bird-gymnasium`, simply run the following command:
 
@@ -68,15 +60,15 @@
     
 ## Usage
 
 Like with other `gymnasium` environments, it's very easy to use `flappy-bird-gymnasium`.
 Simply import the package and create the environment with the `make` function.
 Take a look at the sample code below:
 
-```
+```python
 import time
 import flappy_bird_gymnasium
 import gymnasium
 env = gymnasium.make("FlappyBird-v0")
 
 obs, _ = env.reset()
 while True:
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/__init__.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/die.ogg` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/die.ogg`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/die.wav` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/die.wav`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/hit.ogg` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/hit.ogg`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/hit.wav` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/hit.wav`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/point.ogg` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/point.ogg`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/point.wav` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/point.wav`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/swoosh.ogg` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/swoosh.ogg`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/swoosh.wav` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/swoosh.wav`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/wing.ogg` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/wing.ogg`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/audio/wing.wav` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/audio/wing.wav`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/background-day.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/background-day.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/background-night.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/background-night.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/gameover.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/gameover.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/message.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/message.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/pipe-green.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/pipe-green.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/assets/sprites/pipe-red.png` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/assets/sprites/pipe-red.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/cli.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/cli.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/__init__.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/flappy_bird_env_rgb.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/flappy_bird_env_rgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __init__(
         self,
         screen_size: Tuple[int, int] = (288, 512),
         audio_on: bool = True,
         pipe_gap: int = 100,
         bird_color: str = "yellow",
         pipe_color: str = "green",
-        render_mode=None,
+        render_mode: Optional[str] = None,
         background: Optional[str] = None,
     ) -> None:
         self.action_space = gymnasium.spaces.Discrete(2)
         self.observation_space = gymnasium.spaces.Box(0, 255, [*screen_size, 3])
 
         self._screen_size = screen_size
         self._pipe_gap = pipe_gap
@@ -92,15 +92,17 @@
         return pygame.surfarray.array3d(self.renderer.surface)
 
     def reset(self, seed=None, options=None):
         """Resets the environment (starts a new game)."""
         super().reset(seed=seed)
 
         self._game = FlappyBirdLogic(
-            screen_size=self._screen_size, pipe_gap_size=self._pipe_gap
+            np_random=self.np_random,
+            screen_size=self._screen_size,
+            pipe_gap_size=self._pipe_gap,
         )
 
         self.renderer.game = self._game
         info = {"score": self._game.score}
         return self._get_observation(), info
 
     def step(
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/flappy_bird_env_simple.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/flappy_bird_env_simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 # ==============================================================================
 
 """ Implementation of a Flappy Bird OpenAI gymnasium environment that yields simple
 numerical information about the game's state as observations.
 """
 
+import time
 from typing import Dict, Optional, Tuple, Union
 
 import gymnasium
 import numpy as np
 import pygame
 
 from flappy_bird_gymnasium.envs.game_logic import (
@@ -66,24 +67,25 @@
         pipe_color (str): Color of the pipes. The currently available colors are
             "green" and "red".
         background (Optional[str]): Type of background image. The currently
             available types are "day" and "night". If `None`, no background will
             be drawn.
     """
 
-    metadata = {"render_modes": ["human"], "render_fps": 30}
+    metadata = {"render_modes": ["human", "rgb_array"], "render_fps": 30}
 
     def __init__(
         self,
         screen_size: Tuple[int, int] = (288, 512),
-        audio_on: bool = True,
+        audio_on: bool = False,
         normalize_obs: bool = True,
         pipe_gap: int = 100,
         bird_color: str = "yellow",
         pipe_color: str = "green",
+        render_mode: Optional[str] = None,
         background: Optional[str] = "day",
     ) -> None:
         self.action_space = gymnasium.spaces.Discrete(2)
         self.observation_space = gymnasium.spaces.Box(
             -np.inf, np.inf, shape=(12,), dtype=np.float64
         )
         self._screen_size = screen_size
@@ -94,14 +96,26 @@
         self._game = None
         self._renderer = None
 
         self._bird_color = bird_color
         self._pipe_color = pipe_color
         self._bg_type = background
 
+        assert render_mode is None or render_mode in self.metadata["render_modes"]
+        self.render_mode = render_mode
+
+        if render_mode is not None:
+            self._renderer = FlappyBirdRenderer(
+                screen_size=self._screen_size,
+                audio_on=audio_on,
+                bird_color=bird_color,
+                pipe_color=pipe_color,
+                background=background,
+            )
+
     def _get_observation(self):
         pipes = []
         for up_pipe, low_pipe in zip(self._game.upper_pipes, self._game.lower_pipes):
             # the pipe is behind the screen?
             if low_pipe["x"] > self._screen_size[0]:
                 pipes.append((self._screen_size[0], 0, self._screen_size[1]))
             else:
@@ -173,37 +187,40 @@
         return obs, reward, done, False, info
 
     def reset(self, seed=None, options=None):
         """Resets the environment (starts a new game)."""
         super().reset(seed=seed)
 
         self._game = FlappyBirdLogic(
-            screen_size=self._screen_size, pipe_gap_size=self._pipe_gap
+            np_random=self.np_random,
+            screen_size=self._screen_size,
+            pipe_gap_size=self._pipe_gap,
         )
         if self._renderer is not None:
             self._renderer.game = self._game
 
         info = {"score": self._game.score}
         return self._get_observation(), info
 
+    def set_color(self, color):
+        if self._renderer is not None:
+            self._renderer.set_color(color)
+
     def render(self) -> None:
         """Renders the next frame."""
-        if self._renderer is None:
-            self._renderer = FlappyBirdRenderer(
-                screen_size=self._screen_size,
-                audio_on=self._audio_on,
-                bird_color=self._bird_color,
-                pipe_color=self._pipe_color,
-                background=self._bg_type,
-            )
-            self._renderer.game = self._game
-            self._renderer.make_display()
-
         self._renderer.draw_surface(show_score=True)
-        self._renderer.update_display()
+        if self.render_mode == "rgb_array":
+            # Flip the image to retrieve a correct aspect
+            return np.transpose(pygame.surfarray.array3d(self._renderer.surface), axes=(1, 0, 2))
+        else:
+            if self._renderer.display is None:
+                self._renderer.make_display()
+
+            self._renderer.update_display()
+            time.sleep(1 / self.metadata["render_fps"])
 
     def close(self):
         """Closes the environment."""
         if self._renderer is not None:
             pygame.display.quit()
             pygame.quit()
             self._renderer = None
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/game_logic.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/game_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 Some of the code in this module is an adaption of the code in the `FlapPyBird`
 GitHub repository by `sourahbhv` (https://github.com/sourabhv/FlapPyBird),
 released under the MIT license.
 """
 
 
-import random
 from enum import IntEnum
 from itertools import cycle
 from typing import Dict, Tuple, Union
 
 import pygame
 
 ############################ Speed and Acceleration ############################
@@ -92,28 +91,32 @@
         last_action (Optional[FlappyBirdLogic.Actions]): The last action taken
             by the player. If `None`, the player hasn't taken any action yet.
         sound_cache (Optional[str]): Stores the name of the next sound to be
             played. If `None`, then no sound should be played.
         player_idx (int): Current index of the bird's animation cycle.
     """
 
-    def __init__(self, screen_size: Tuple[int, int], pipe_gap_size: int = 100) -> None:
+    def __init__(
+        self, np_random, screen_size: Tuple[int, int], pipe_gap_size: int = 100
+    ) -> None:
         self._screen_width = screen_size[0]
         self._screen_height = screen_size[1]
 
         self.player_x = int(self._screen_width * 0.2)
         self.player_y = int((self._screen_height - PLAYER_HEIGHT) / 2)
 
         self.base_x = 0
         self.base_y = self._screen_height * 0.79
         self._base_shift = BASE_WIDTH - BACKGROUND_WIDTH
 
         self.score = 0
         self._pipe_gap_size = pipe_gap_size
 
+        self._np_random = np_random
+
         # Generate 3 new pipes to add to upper_pipes and lower_pipes lists
         new_pipe1 = self._get_random_pipe()
         new_pipe2 = self._get_random_pipe()
         new_pipe3 = self._get_random_pipe()
 
         # List of upper pipes:
         self.upper_pipes = [
@@ -157,15 +160,17 @@
         """Possible actions for the player to take."""
 
         IDLE, FLAP = 0, 1
 
     def _get_random_pipe(self) -> Dict[str, int]:
         """Returns a randomly generated pipe."""
         # y of gap between upper and lower pipe
-        gap_y = random.randrange(0, int(self.base_y * 0.6 - self._pipe_gap_size))
+        gap_y = self._np_random.integers(
+            0, int(self.base_y * 0.6 - self._pipe_gap_size)
+        )
         gap_y += int(self.base_y * 0.2)
 
         pipe_x = self._screen_width + PIPE_WIDTH + (self._screen_width * 0.2)
         return [
             {"x": pipe_x, "y": gap_y - PIPE_HEIGHT},  # upper pipe
             {"x": pipe_x, "y": gap_y + self._pipe_gap_size},  # lower pipe
         ]
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/renderer.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         bird_color: str = "yellow",
         pipe_color: str = "green",
         background: Optional[str] = "day",
     ) -> None:
         self._screen_width = screen_size[0]
         self._screen_height = screen_size[1]
 
+        self._color = None
         self.display = None
         self.surface = pygame.Surface(screen_size)
         self.images = utils.load_images(
             convert=False,
             bird_color=bird_color,
             pipe_color=pipe_color,
             bg_type=background,
@@ -157,14 +158,17 @@
 
         # Player
         player_surface = pygame.transform.rotate(
             self.images["player"][self.game.player_idx],
             visible_rot,
         )
 
+        if self._color is not None:
+            player_surface.fill(self._color, special_flags=pygame.BLEND_RGBA_ADD)
+
         self.surface.blit(player_surface, (self.game.player_x, self.game.player_y))
 
     def update_display(self) -> None:
         """Updates the display with the current surface of the renderer.
 
         A call to this method is usually preceded by a call to
         :meth:`.draw_surface()`. This method simply updates the display by
@@ -174,14 +178,18 @@
         if self.display is None:
             raise RuntimeError(
                 "Tried to update the display, but a display hasn't been "
                 "created yet! To create a display for the renderer, you must "
                 "call the `make_display()` method."
             )
 
+        pygame.event.get()
         self.display.blit(self.surface, [0, 0])
         pygame.display.update()
 
         # Sounds:
         if self.audio_on and self.game.sound_cache is not None:
             sound_name = self.game.sound_cache
             self.sounds[sound_name].play()
+
+    def set_color(self, color):
+        self._color = color
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium/envs/utils.py` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium/envs/utils.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/PKG-INFO` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flappy-bird-gymnasium
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Gymnasium environment for the Flappy Bird game.
 Home-page: https://github.com/markub3327/flappy-bird-gymnasium
 Download-URL: https://github.com/markub3327/flappy-bird-gymnasium/releases
 Author: Martin Kubovcik
 Author-email: markub3327@gmail.com
 License: MIT License
+Project-URL: Bug Tracker, https://github.com/markub3327/flappy-bird-gymnasium/issues
 Keywords: Flappy-BirdGame Gymnasium Farama-Foundation Reinforcement-Learning Reinforcement-Learning-Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -74,23 +75,15 @@
 * +1.0 - **successfully passing a pipe**
 * -1.0 - **dying**
 
 <br>
 
 <p align="center">
   <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/yellow_bird_playing.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/red_bird_start_screen.gif?raw=true" 
-       width="200"/>
-  &nbsp;&nbsp;&nbsp;&nbsp;
-  <img align="center" 
-       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/blue_bird_playing.gif?raw=true" 
+       src="https://github.com/markub3327/flappy-bird-gymnasium/blob/main/imgs/dqn.gif?raw=true" 
        width="200"/>
 </p>
 
 ## Installation
 
 To install `flappy-bird-gymnasium`, simply run the following command:
 
@@ -98,15 +91,15 @@
     
 ## Usage
 
 Like with other `gymnasium` environments, it's very easy to use `flappy-bird-gymnasium`.
 Simply import the package and create the environment with the `make` function.
 Take a look at the sample code below:
 
-```
+```python
 import time
 import flappy_bird_gymnasium
 import gymnasium
 env = gymnasium.make("FlappyBird-v0")
 
 obs, _ = env.reset()
 while True:
```

### Comparing `flappy-bird-gymnasium-0.2.1/flappy_bird_gymnasium.egg-info/SOURCES.txt` & `flappy-bird-gymnasium-0.2.2/flappy_bird_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flappy-bird-gymnasium-0.2.1/setup.py` & `flappy-bird-gymnasium-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """ Setup of the flappy-bird-gymnasium package.
 """
 
 from typing import List
 
 import setuptools
 
-_VERSION = "0.2.1"
+_VERSION = "0.2.2"
 
 # Short description.
 short_description = "A Gymnasium environment for the Flappy Bird game."
 
 # Packages needed for the environment to run.
 # The compatible release operator (`~=`) is used to match any candidate version
 # that is expected to be compatible with the specified version.
@@ -55,14 +55,17 @@
     version=_VERSION,
     author="Martin Kubovcik",
     author_email="markub3327@gmail.com",
     description=short_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/markub3327/flappy-bird-gymnasium",
+    project_urls={
+        "Bug Tracker": "https://github.com/markub3327/flappy-bird-gymnasium/issues",
+    },
     download_url="https://github.com/markub3327/flappy-bird-gymnasium/releases",
     # Contained modules and scripts:
     packages=setuptools.find_packages(),
     package_data={
         "flappy_bird_gymnasium": [
             "assets/sprites/*",
             "assets/audio/*",
```

