# Comparing `tmp/crypto-screening-8.4.1.tar.gz` & `tmp/crypto-screening-8.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.4.1.tar", last modified: Mon Jul 31 05:20:16 2023, max compression
+gzip compressed data, was "crypto-screening-8.4.2.tar", last modified: Wed Aug  2 06:38:23 2023, max compression
```

## Comparing `crypto-screening-8.4.1.tar` & `crypto-screening-8.4.2.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.779783 crypto-screening-8.4.1/
--rw-rw-rw-   0        0        0      196 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-31 05:20:16.778782 crypto-screening-8.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.736783 crypto-screening-8.4.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.753783 crypto-screening-8.4.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.4.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.4.1/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.757784 crypto-screening-8.4.1/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.1/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.1/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.759783 crypto-screening-8.4.1/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    21667 2023-07-31 05:19:43.000000 crypto-screening-8.4.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.768782 crypto-screening-8.4.1/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.1/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.1/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.770784 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.773782 crypto-screening-8.4.1/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.1/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.1/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.4.1/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.775782 crypto-screening-8.4.1/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.1/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.1/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.1/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.4.1/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.1/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.1/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.728858 crypto-screening-8.4.1/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.776783 crypto-screening-8.4.1/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.1/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.1/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.777783 crypto-screening-8.4.1/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.1/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.1/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.4.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.750783 crypto-screening-8.4.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 05:20:16.779783 crypto-screening-8.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-31 05:20:12.000000 crypto-screening-8.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.423722 crypto-screening-8.4.2/
+-rw-rw-rw-   0        0        0      196 2023-08-02 06:38:21.000000 crypto-screening-8.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-08-02 06:38:23.422722 crypto-screening-8.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.2/build.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.204575 crypto-screening-8.4.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.230547 crypto-screening-8.4.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16968 2023-08-02 06:37:38.000000 crypto-screening-8.4.2/crypto_screening/collect/assets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.231546 crypto-screening-8.4.2/crypto_screening/collect/foundation/
+-rw-rw-rw-   0        0        0     4943 2023-07-31 16:05:02.000000 crypto-screening-8.4.2/crypto_screening/collect/foundation/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.254546 crypto-screening-8.4.2/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.2/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.2/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.2/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.2/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.277611 crypto-screening-8.4.2/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.2/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.2/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.2/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.2/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15119 2023-07-31 16:05:02.000000 crypto-screening-8.4.2/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21677 2023-08-02 06:37:38.000000 crypto-screening-8.4.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.342147 crypto-screening-8.4.2/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.2/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.2/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.366147 crypto-screening-8.4.2/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.2/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.2/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.2/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.2/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.387753 crypto-screening-8.4.2/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.2/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.2/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.2/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.2/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.2/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.2/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    11146 2023-07-31 16:05:02.000000 crypto-screening-8.4.2/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.409723 crypto-screening-8.4.2/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.4.2/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.2/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.2/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.2/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.2/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.2/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.2/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.2/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.4.2/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.2/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.2/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.173067 crypto-screening-8.4.2/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.409723 crypto-screening-8.4.2/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.2/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.2/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.421755 crypto-screening-8.4.2/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.2/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.2/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3855 2023-08-02 06:33:48.000000 crypto-screening-8.4.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:38:23.222604 crypto-screening-8.4.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-08-02 06:38:23.000000 crypto-screening-8.4.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-08-02 06:38:23.000000 crypto-screening-8.4.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:38:23.000000 crypto-screening-8.4.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-08-02 06:38:23.000000 crypto-screening-8.4.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 06:38:23.000000 crypto-screening-8.4.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-08-02 06:38:21.000000 crypto-screening-8.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 06:38:23.423722 crypto-screening-8.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-08-02 06:38:16.000000 crypto-screening-8.4.2/setup.py
```

### Comparing `crypto-screening-8.4.1/PKG-INFO` & `crypto-screening-8.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.1
+Version: 8.4.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.1/README.md` & `crypto-screening-8.4.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/build.py` & `crypto-screening-8.4.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/assets.py` & `crypto-screening-8.4.2/crypto_screening/collect/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # assets.py
 
 from typing import Optional, Dict, Iterable, Set, Union
 
 from crypto_screening.utils.process import mutual_string_values
 from crypto_screening.symbols import symbol_to_parts, symbol_to_pair
-from crypto_screening.collect.exchanges import exchanges_data
+from crypto_screening.collect.foundation.exchanges import exchanges_data
 from crypto_screening.collect.symbols import (
     all_exchange_symbols, exchange_symbols
 )
 
 __all__ = [
     "exchanges_assets",
     "mutual_exchanges_assets",
```

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/exchanges.py` & `crypto-screening-8.4.2/crypto_screening/collect/foundation/exchanges.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,11 +164,11 @@
         callers.append(caller)
         data[exchange] = caller
     # end for
 
     multi_threaded_call(callers=callers)
 
     return {
-        key: value.results.returns
+        key: value.result.returns
         for key, value in data.items() if value
     }
 # end exchanges_data
```

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/orders.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/market/trades.py` & `crypto-screening-8.4.2/crypto_screening/collect/market/trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
         return assets_market_values(
-            exchange=exchange, symbol=symbol, data=self.pricess,
+            exchange=exchange, symbol=symbol, data=self.prices,
             separator=separator, provider=self
         )
     # end price
 
     def side(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, str]]:
@@ -314,15 +314,15 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
         return symbols_market_values(
-            exchange=exchange, symbol=symbol, data=self.pricess,
+            exchange=exchange, symbol=symbol, data=self.prices,
             provider=self
         )
     # end price
 
     def side(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, str]]:
         """
         Returns the ask price for the symbol.
```

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/screeners.py` & `crypto-screening-8.4.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/collect/symbols.py` & `crypto-screening-8.4.2/crypto_screening/collect/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     mutual_string_values, string_in_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
     symbol_to_parts, adjust_symbol, Separator, Pair
 )
 from crypto_screening.validate import validate_exchange
-from crypto_screening.collect.exchanges import exchanges_data
+from crypto_screening.collect.foundation.exchanges import exchanges_data
 
 __all__ = [
     "exchanges_symbols",
     "mutual_exchanges_symbols",
     "include_symbols",
     "exclude_symbols",
     "exchange_symbols",
@@ -368,15 +368,15 @@
                     adjust=adjust, test=test
                 ), identifier=exchange
             ) for exchange in exchanges
         ]
     )
 
     return {
-        exchange: results.results(exchange).returns
+        exchange: results.result(exchange).returns
         for exchange in exchanges
     }
 # end all_exchanges_symbols
 
 def exchange_symbols(
         exchange: Optional[str] = None,
         separator: Optional[str] = None,
```

### Comparing `crypto-screening-8.4.1/crypto_screening/dataset.py` & `crypto-screening-8.4.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/exchanges.py` & `crypto-screening-8.4.2/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/interval.py` & `crypto-screening-8.4.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/base.py` & `crypto-screening-8.4.2/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.4.2/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.4.2/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.4.2/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.4.2/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.4.2/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.4.2/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/combined.py` & `crypto-screening-8.4.2/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/container.py` & `crypto-screening-8.4.2/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/database.py` & `crypto-screening-8.4.2/crypto_screening/screeners/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,18 @@
     :param screener: The screener object.
     :param engine: The database engine.
     :param length: The length of data to extract.
     :param start: The start index.
     """
 
     interval = (
-        screener.interval if (screener.NAME == "OHLCV") else None
+        screener.interval if (
+            hasattr(screener, "interval") and
+            (screener.NAME == "OHLCV")
+        ) else None
     )
 
     data = extract_database_record(
         name=screener.NAME, exchange=screener.exchange,
         symbol=screener.symbol, interval=interval, start=start,
         length=length, engine=engine
     )
@@ -403,12 +406,15 @@
     :return: The table names in the database for the screeners.
     """
 
     return {
         screener: parts_to_database_table_name(
             name=screener.NAME, exchange=screener.exchange,
             symbol=screener.symbol, interval=(
-                screener.interval if (screener.NAME == "OHLCV") else None
+                screener.interval if (
+                    hasattr(screener, "interval") and
+                    (screener.NAME == "OHLCV")
+                ) else None
             )
         ) for screener in screeners
     }
 # end screeners_tables_names
```

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.4.2/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.4.2/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.4.2/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.4.2/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/market.py` & `crypto-screening-8.4.2/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.4.2/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.4.2/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/orders.py` & `crypto-screening-8.4.2/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/recorder.py` & `crypto-screening-8.4.2/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/trades.py` & `crypto-screening-8.4.2/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/screeners/waiting.py` & `crypto-screening-8.4.2/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.4.2/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/symbols.py` & `crypto-screening-8.4.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/utils/base.py` & `crypto-screening-8.4.2/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/utils/process.py` & `crypto-screening-8.4.2/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.1/crypto_screening/validate.py` & `crypto-screening-8.4.2/crypto_screening/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from crypto_screening.exchanges import EXCHANGE_NAMES
 
 __all__ = [
     "is_valid_symbol",
     "validate_exchange",
     "validate_symbol",
     "is_valid_exchange",
-    "validate_interval"
+    "validate_interval",
+    "is_valid_interval"
 ]
 
 def is_valid_symbol(symbol: str, symbols: Iterable[str]) -> bool:
     """
     Returns a value for the symbol being valid for the source exchange.
 
     :param symbol: The symbol of the assets.
@@ -43,15 +44,15 @@
 
     :param exchange: The name of the exchange platform.
     :param symbol: The symbol of the assets.
     :param symbols: The valid symbols.
     :param exchanges: The valid exchanges.
     :param provider: Any provider object.
 
-    :return: The validation-value.
+    :return: The valid symbol.
     """
 
     validate_exchange(
         exchange=exchange, exchanges=exchanges, provider=provider
     )
 
     if not is_valid_symbol(symbol=symbol, symbols=symbols):
@@ -64,26 +65,45 @@
     # end if
 
     return symbol
 # end validate_symbol
 
 def validate_interval(interval: str) -> str:
     """
-    Validates the symbol value.
+    Validates the interval value.
 
     :param interval: The interval for the data.
 
-    :return: The validates symbol.
+    :return: The valid interval.
     """
 
     interval_to_total_time(interval)
 
     return interval
 # end validate_interval
 
+def is_valid_interval(interval: str) -> bool:
+    """
+    Validates the interval value.
+
+    :param interval: The interval for the data.
+
+    :return: The validates value.
+    """
+
+    try:
+        validate_interval(interval)
+
+        return True
+
+    except ValueError:
+        return False
+    # end try
+# end is_valid_interval
+
 def is_valid_exchange(
         exchange: str, exchanges: Optional[Iterable[str]] = None
 ) -> bool:
     """
     checks of the source os a valid exchange name.
 
     :param exchange: The source name to validate.
@@ -107,15 +127,15 @@
     """
     Validates the source value.
 
     :param exchange: The name of the exchange platform.
     :param exchanges: The valid exchanges.
     :param provider: Any provider object.
 
-    :return: The validates symbol.
+    :return: The valid exchange.
     """
 
     if exchanges is None:
         exchanges = EXCHANGE_NAMES
     # end if
 
     if not is_valid_exchange(exchange=exchange, exchanges=exchanges):
```

### Comparing `crypto-screening-8.4.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.4.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.1
+Version: 8.4.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.4.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 crypto_screening/validate.py
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
-crypto_screening/collect/exchanges.py
 crypto_screening/collect/screeners.py
 crypto_screening/collect/symbols.py
+crypto_screening/collect/foundation/exchanges.py
 crypto_screening/collect/market/__init__.py
 crypto_screening/collect/market/ohlcv.py
 crypto_screening/collect/market/orderbook.py
 crypto_screening/collect/market/orders.py
 crypto_screening/collect/market/trades.py
 crypto_screening/collect/market/state/__init__.py
 crypto_screening/collect/market/state/assets.py
```

### Comparing `crypto-screening-8.4.1/pyproject.toml` & `crypto-screening-8.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.4.1'
+version = '8.4.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.4.1/setup.py` & `crypto-screening-8.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.4.1',
+        version='8.4.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

